# Comparing `tmp/spswarehouse-0.0.9.0.tar.gz` & `tmp/spswarehouse-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spswarehouse-0.0.9.0.tar", last modified: Wed Jan  4 23:42:11 2023, max compression
+gzip compressed data, was "spswarehouse-0.1.0.tar", last modified: Mon May  8 23:35:07 2023, max compression
```

## Comparing `spswarehouse-0.0.9.0.tar` & `spswarehouse-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-01-04 23:42:11.967055 spswarehouse-0.0.9.0/
--rw-rw-rw-   0        0        0    35823 2022-12-01 20:45:52.000000 spswarehouse-0.0.9.0/LICENSE
--rw-rw-rw-   0        0        0      448 2022-12-01 20:45:52.000000 spswarehouse-0.0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8202 2023-01-04 23:42:11.967055 spswarehouse-0.0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     7815 2022-12-01 20:45:52.000000 spswarehouse-0.0.9.0/README.md
--rw-rw-rw-   0        0        0       42 2023-01-04 23:42:11.968059 spswarehouse-0.0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      724 2023-01-04 23:39:39.000000 spswarehouse-0.0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-04 23:42:11.955406 spswarehouse-0.0.9.0/spswarehouse/
--rw-rw-rw-   0        0        0      576 2022-12-01 20:45:52.000000 spswarehouse-0.0.9.0/spswarehouse/__init__.py
--rw-rw-rw-   0        0        0      709 2022-12-01 20:45:52.000000 spswarehouse-0.0.9.0/spswarehouse/credentials.py.template
--rw-rw-rw-   0        0        0     2037 2022-12-01 20:45:52.000000 spswarehouse-0.0.9.0/spswarehouse/googledrive.py
--rw-rw-rw-   0        0        0     1923 2022-12-01 20:45:52.000000 spswarehouse-0.0.9.0/spswarehouse/googlesheets.py
--rw-rw-rw-   0        0        0     1957 2022-12-01 20:45:52.000000 spswarehouse-0.0.9.0/spswarehouse/googleslides.py
--rw-rw-rw-   0        0        0      173 2023-01-04 23:30:21.000000 spswarehouse-0.0.9.0/spswarehouse/requirements.txt
--rw-rw-rw-   0        0        0     1269 2022-12-01 20:45:52.000000 spswarehouse-0.0.9.0/spswarehouse/table_names.py
--rw-rw-rw-   0        0        0     7878 2023-01-04 22:56:50.000000 spswarehouse-0.0.9.0/spswarehouse/table_utils.py
--rw-rw-rw-   0        0        0     4685 2022-12-01 20:45:52.000000 spswarehouse-0.0.9.0/spswarehouse/warehouse.py
-drwxrwxrwx   0        0        0        0 2023-01-04 23:42:11.965055 spswarehouse-0.0.9.0/spswarehouse.egg-info/
--rw-rw-rw-   0        0        0     8202 2023-01-04 23:42:11.000000 spswarehouse-0.0.9.0/spswarehouse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-01-04 23:42:11.000000 spswarehouse-0.0.9.0/spswarehouse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-04 23:42:11.000000 spswarehouse-0.0.9.0/spswarehouse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-01-04 23:42:11.000000 spswarehouse-0.0.9.0/spswarehouse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 23:35:07.814081 spswarehouse-0.1.0/
+-rw-rw-rw-   0        0        0    35823 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      448 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8200 2023-05-08 23:35:07.812086 spswarehouse-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7815 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 23:35:07.814081 spswarehouse-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-05-08 23:34:09.000000 spswarehouse-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:35:07.797666 spswarehouse-0.1.0/spswarehouse/
+-rw-rw-rw-   0        0        0      576 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/spswarehouse/__init__.py
+-rw-rw-rw-   0        0        0    28240 2023-05-08 23:04:57.000000 spswarehouse-0.1.0/spswarehouse/calpads.py
+-rw-rw-rw-   0        0        0     1035 2023-05-08 23:22:00.000000 spswarehouse-0.1.0/spswarehouse/credentials.py.template
+-rw-rw-rw-   0        0        0     2037 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/spswarehouse/googledrive.py
+-rw-rw-rw-   0        0        0     1923 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/spswarehouse/googlesheets.py
+-rw-rw-rw-   0        0        0     1957 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/spswarehouse/googleslides.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:35:07.810128 spswarehouse-0.1.0/spswarehouse/powerschool/
+-rw-rw-rw-   0        0        0        0 2023-05-08 23:11:00.000000 spswarehouse-0.1.0/spswarehouse/powerschool/__init__.py
+-rw-rw-rw-   0        0        0    19518 2023-05-08 23:32:25.000000 spswarehouse-0.1.0/spswarehouse/powerschool/powerschool.py
+-rw-rw-rw-   0        0        0    25294 2023-05-08 22:51:29.000000 spswarehouse-0.1.0/spswarehouse/powerschool/powerschool_calpads.py
+-rw-rw-rw-   0        0        0      300 2023-05-08 22:51:29.000000 spswarehouse-0.1.0/spswarehouse/requirements.txt
+-rw-rw-rw-   0        0        0     1269 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/spswarehouse/table_names.py
+-rw-rw-rw-   0        0        0     7878 2023-01-04 22:56:50.000000 spswarehouse-0.1.0/spswarehouse/table_utils.py
+-rw-rw-rw-   0        0        0     4685 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/spswarehouse/warehouse.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:35:07.804854 spswarehouse-0.1.0/spswarehouse.egg-info/
+-rw-rw-rw-   0        0        0     8200 2023-05-08 23:35:07.000000 spswarehouse-0.1.0/spswarehouse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2023-05-08 23:35:07.000000 spswarehouse-0.1.0/spswarehouse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 23:35:07.000000 spswarehouse-0.1.0/spswarehouse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-08 23:35:07.000000 spswarehouse-0.1.0/spswarehouse.egg-info/top_level.txt
```

### Comparing `spswarehouse-0.0.9.0/LICENSE` & `spswarehouse-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.0.9.0/PKG-INFO` & `spswarehouse-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse
-Version: 0.0.9.0
+Version: 0.1.0
 Summary: Summit Public Schools Snowflake warehouse
 Home-page: https://github.com/SummitPublicSchools/spswarehouse
 Author: Summit Public Schools; Harry Li Consulting, LLC
 Author-email: warehouse@summitps.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spswarehouse-0.0.9.0/README.md` & `spswarehouse-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.0.9.0/setup.py` & `spswarehouse-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spswarehouse",
-    version="0.0.9.0",
+    version="0.1.0",
     author="Summit Public Schools; Harry Li Consulting, LLC",
     author_email="warehouse@summitps.org",
     description="Summit Public Schools Snowflake warehouse",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SummitPublicSchools/spswarehouse",
     packages=setuptools.find_packages(),
```

### Comparing `spswarehouse-0.0.9.0/spswarehouse/__init__.py` & `spswarehouse-0.1.0/spswarehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.0.9.0/spswarehouse/googledrive.py` & `spswarehouse-0.1.0/spswarehouse/googledrive.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.0.9.0/spswarehouse/googlesheets.py` & `spswarehouse-0.1.0/spswarehouse/googlesheets.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.0.9.0/spswarehouse/googleslides.py` & `spswarehouse-0.1.0/spswarehouse/googleslides.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.0.9.0/spswarehouse/table_names.py` & `spswarehouse-0.1.0/spswarehouse/table_names.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.0.9.0/spswarehouse/table_utils.py` & `spswarehouse-0.1.0/spswarehouse/table_utils.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.0.9.0/spswarehouse/warehouse.py` & `spswarehouse-0.1.0/spswarehouse/warehouse.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.0.9.0/spswarehouse.egg-info/PKG-INFO` & `spswarehouse-0.1.0/spswarehouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse
-Version: 0.0.9.0
+Version: 0.1.0
 Summary: Summit Public Schools Snowflake warehouse
 Home-page: https://github.com/SummitPublicSchools/spswarehouse
 Author: Summit Public Schools; Harry Li Consulting, LLC
 Author-email: warehouse@summitps.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

