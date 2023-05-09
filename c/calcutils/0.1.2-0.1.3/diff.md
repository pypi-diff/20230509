# Comparing `tmp/calcutils-0.1.2.tar.gz` & `tmp/calcutils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Python\calcutils\dist\.tmp-e4pdnkbe\calcutils-0.1.2.tar", last modified: Mon May  8 10:36:25 2023, max compression
+gzip compressed data, was "D:\Python\calcutils\dist\.tmp-52dgkw2o\calcutils-0.1.3.tar", last modified: Tue May  9 05:31:14 2023, max compression
```

## Comparing `calcutils-0.1.2.tar` & `calcutils-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 10:36:25.000000 calcutils-0.1.2/
--rw-rw-rw-   0        0        0       11 2023-05-08 09:36:20.000000 calcutils-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      584 2023-05-08 10:36:25.000000 calcutils-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        8 2023-05-08 07:30:00.000000 calcutils-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 10:36:25.000000 calcutils-0.1.2/calcutils/
--rw-rw-rw-   0        0        0     1098 2023-05-08 08:27:36.000000 calcutils-0.1.2/calcutils/calcu.p
--rw-rw-rw-   0        0        0     7827 2023-05-08 10:35:32.000000 calcutils-0.1.2/calcutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:36:25.000000 calcutils-0.1.2/calcutils.egg-info/
--rw-rw-rw-   0        0        0      584 2023-05-08 10:36:24.000000 calcutils-0.1.2/calcutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-08 10:36:25.000000 calcutils-0.1.2/calcutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 10:36:24.000000 calcutils-0.1.2/calcutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-08 10:36:24.000000 calcutils-0.1.2/calcutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      512 2023-05-08 10:35:59.000000 calcutils-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 10:36:25.000000 calcutils-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-05-08 10:35:59.000000 calcutils-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 05:31:14.000000 calcutils-0.1.3/
+-rw-rw-rw-   0        0        0       11 2023-05-08 09:36:20.000000 calcutils-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      584 2023-05-09 05:31:14.000000 calcutils-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        8 2023-05-08 07:30:00.000000 calcutils-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 05:31:14.000000 calcutils-0.1.3/calcutils/
+-rw-rw-rw-   0        0        0     1098 2023-05-08 08:27:36.000000 calcutils-0.1.3/calcutils/calcu.p
+-rw-rw-rw-   0        0        0    24574 2023-05-09 05:27:26.000000 calcutils-0.1.3/calcutils/calcus.py
+-rw-rw-rw-   0        0        0     7827 2023-05-08 10:35:32.000000 calcutils-0.1.3/calcutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 05:31:14.000000 calcutils-0.1.3/calcutils.egg-info/
+-rw-rw-rw-   0        0        0      584 2023-05-09 05:31:14.000000 calcutils-0.1.3/calcutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-05-09 05:31:14.000000 calcutils-0.1.3/calcutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 05:31:14.000000 calcutils-0.1.3/calcutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-09 05:31:14.000000 calcutils-0.1.3/calcutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      512 2023-05-09 05:30:38.000000 calcutils-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 05:31:14.000000 calcutils-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      489 2023-05-09 04:58:44.000000 calcutils-0.1.3/setup.py
```

### Comparing `calcutils-0.1.2/PKG-INFO` & `calcutils-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcutils
-Version: 0.1.2
+Version: 0.1.3
 Summary: A small calcu package
 Home-page: https://github.com/calcu_utils/calcu_utils
 Author: Lahani_Allen
 Author-email: Lahani_Allen <lahani_Allen@utc.com>
 Project-URL: Homepage, https://github.com/calcu_utils/calcu_utils
 Project-URL: Bug Tracker, https://github.com/calcu_utils/calcu_utils/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `calcutils-0.1.2/calcutils/calcu.p` & `calcutils-0.1.3/calcutils/calcu.p`

 * *Files identical despite different names*

### Comparing `calcutils-0.1.2/calcutils/utils.py` & `calcutils-0.1.3/calcutils/utils.py`

 * *Files identical despite different names*

### Comparing `calcutils-0.1.2/calcutils.egg-info/PKG-INFO` & `calcutils-0.1.3/calcutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcutils
-Version: 0.1.2
+Version: 0.1.3
 Summary: A small calcu package
 Home-page: https://github.com/calcu_utils/calcu_utils
 Author: Lahani_Allen
 Author-email: Lahani_Allen <lahani_Allen@utc.com>
 Project-URL: Homepage, https://github.com/calcu_utils/calcu_utils
 Project-URL: Bug Tracker, https://github.com/calcu_utils/calcu_utils/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `calcutils-0.1.2/pyproject.toml` & `calcutils-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "calcutils"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Lahani_Allen", email="lahani_Allen@utc.com" },
 ]
 description = "A small calcu package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

