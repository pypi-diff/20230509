# Comparing `tmp/emanifest-3.0.3.tar.gz` & `tmp/emanifest-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emanifest-3.0.3.tar", last modified: Wed Mar  1 16:25:20 2023, max compression
+gzip compressed data, was "emanifest-3.0.4.tar", last modified: Tue May  9 19:45:32 2023, max compression
```

## Comparing `emanifest-3.0.3.tar` & `emanifest-3.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:25:20.095304 emanifest-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-01 16:25:02.000000 emanifest-3.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-03-01 16:25:20.095304 emanifest-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-03-01 16:25:02.000000 emanifest-3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-01 16:25:02.000000 emanifest-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 16:25:20.095304 emanifest-3.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:25:20.091304 emanifest-3.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:25:20.095304 emanifest-3.0.3/src/emanifest/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-01 16:25:02.000000 emanifest-3.0.3/src/emanifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37641 2023-03-01 16:25:02.000000 emanifest-3.0.3/src/emanifest/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-03-01 16:25:02.000000 emanifest-3.0.3/src/emanifest/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:25:20.095304 emanifest-3.0.3/src/emanifest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-03-01 16:25:20.000000 emanifest-3.0.3/src/emanifest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-01 16:25:20.000000 emanifest-3.0.3/src/emanifest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 16:25:20.000000 emanifest-3.0.3/src/emanifest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-01 16:25:20.000000 emanifest-3.0.3/src/emanifest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-01 16:25:20.000000 emanifest-3.0.3/src/emanifest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:45:32.757695 emanifest-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-09 19:45:14.000000 emanifest-3.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-05-09 19:45:32.757695 emanifest-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-05-09 19:45:14.000000 emanifest-3.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-09 19:45:14.000000 emanifest-3.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:45:32.757695 emanifest-3.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:45:32.757695 emanifest-3.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:45:32.757695 emanifest-3.0.4/src/emanifest/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-09 19:45:14.000000 emanifest-3.0.4/src/emanifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37641 2023-05-09 19:45:14.000000 emanifest-3.0.4/src/emanifest/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-09 19:45:14.000000 emanifest-3.0.4/src/emanifest/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:45:32.757695 emanifest-3.0.4/src/emanifest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-05-09 19:45:32.000000 emanifest-3.0.4/src/emanifest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-09 19:45:32.000000 emanifest-3.0.4/src/emanifest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:45:32.000000 emanifest-3.0.4/src/emanifest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-09 19:45:32.000000 emanifest-3.0.4/src/emanifest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 19:45:32.000000 emanifest-3.0.4/src/emanifest.egg-info/top_level.txt
```

### Comparing `emanifest-3.0.3/LICENSE.txt` & `emanifest-3.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `emanifest-3.0.3/PKG-INFO` & `emanifest-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: emanifest
-Version: 3.0.3
-Summary: An API utility wrapper for accessing the e-Manifest hazardous waste tracking system maintainedby the US Environmental Protection Agency
+Version: 3.0.4
+Summary: An API utility wrapper for accessing the e-Manifest hazardous waste tracking system maintained by the US Environmental Protection Agency
 Author-email: William Nicholas  <nicholas.william@epa.gov>, David Graham <graham.david@epa.gov>
 Maintainer-email: William Nicholas <nicholas.william@epa.gov>, David Graham <graham.david@epa.gov>, Scott Christian <christian.scott@epa.gov>
 License: CCO 1.0
 Project-URL: issues, https://github.com/USEPA/e-Manifest/issues
 Project-URL: documentation, https://github.com/USEPA/e-Manifest/emanifest-py
 Project-URL: homepage, https://github.com/USEPA/e-Manifest
 Project-URL: repository, https://github.com/USEPA/e-Manifest
```

### Comparing `emanifest-3.0.3/README.md` & `emanifest-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `emanifest-3.0.3/pyproject.toml` & `emanifest-3.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "emanifest"
-version = "3.0.3"
-description = "An API utility wrapper for accessing the e-Manifest hazardous waste tracking system maintainedby the US Environmental Protection Agency"
+version = "3.0.4"
+description = "An API utility wrapper for accessing the e-Manifest hazardous waste tracking system maintained by the US Environmental Protection Agency"
 readme = "README.md"
 authors = [
     { name = "William Nicholas ", email = "nicholas.william@epa.gov" },
     { name = "David Graham", email = "graham.david@epa.gov" },
 ]
 maintainers = [
     { name = "William Nicholas", email = "nicholas.william@epa.gov" },
```

### Comparing `emanifest-3.0.3/src/emanifest/client.py` & `emanifest-3.0.4/src/emanifest/client.py`

 * *Files identical despite different names*

### Comparing `emanifest-3.0.3/src/emanifest/test_client.py` & `emanifest-3.0.4/src/emanifest/test_client.py`

 * *Files identical despite different names*

### Comparing `emanifest-3.0.3/src/emanifest.egg-info/PKG-INFO` & `emanifest-3.0.4/src/emanifest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: emanifest
-Version: 3.0.3
-Summary: An API utility wrapper for accessing the e-Manifest hazardous waste tracking system maintainedby the US Environmental Protection Agency
+Version: 3.0.4
+Summary: An API utility wrapper for accessing the e-Manifest hazardous waste tracking system maintained by the US Environmental Protection Agency
 Author-email: William Nicholas  <nicholas.william@epa.gov>, David Graham <graham.david@epa.gov>
 Maintainer-email: William Nicholas <nicholas.william@epa.gov>, David Graham <graham.david@epa.gov>, Scott Christian <christian.scott@epa.gov>
 License: CCO 1.0
 Project-URL: issues, https://github.com/USEPA/e-Manifest/issues
 Project-URL: documentation, https://github.com/USEPA/e-Manifest/emanifest-py
 Project-URL: homepage, https://github.com/USEPA/e-Manifest
 Project-URL: repository, https://github.com/USEPA/e-Manifest
```

