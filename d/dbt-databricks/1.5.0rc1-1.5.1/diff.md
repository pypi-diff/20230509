# Comparing `tmp/dbt-databricks-1.5.0rc1.tar.gz` & `tmp/dbt-databricks-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-databricks-1.5.0rc1.tar", last modified: Tue May  2 22:21:00 2023, max compression
+gzip compressed data, was "dbt-databricks-1.5.1.tar", last modified: Tue May  9 15:23:38 2023, max compression
```

## Comparing `dbt-databricks-1.5.0rc1.tar` & `dbt-databricks-1.5.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.339738 dbt-databricks-1.5.0rc1/
--rw-r--r--   0 andre.furlan   (502) staff       (20)       46 2022-11-22 20:51:35.000000 dbt-databricks-1.5.0rc1/MANIFEST.in
--rw-r--r--   0 andre.furlan   (502) staff       (20)     5378 2023-05-02 22:21:00.339449 dbt-databricks-1.5.0rc1/PKG-INFO
--rw-r--r--   0 andre.furlan   (502) staff       (20)     4572 2023-05-02 22:20:31.000000 dbt-databricks-1.5.0rc1/README.md
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.315986 dbt-databricks-1.5.0rc1/dbt/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.315626 dbt-databricks-1.5.0rc1/dbt/adapters/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.324968 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/
--rw-r--r--   0 andre.furlan   (502) staff       (20)      626 2023-02-28 19:04:11.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/__init__.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)       25 2023-05-02 22:20:31.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/__version__.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2708 2023-05-02 22:11:51.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/auth.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)      586 2023-02-28 19:04:11.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/column.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)    26590 2023-05-02 22:11:51.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/connections.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)    19041 2023-05-02 22:20:31.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/impl.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)    17731 2023-05-02 22:11:51.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/python_submissions.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2863 2023-02-28 19:04:11.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/relation.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2117 2023-02-28 19:04:11.000000 dbt-databricks-1.5.0rc1/dbt/adapters/databricks/utils.py
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.316267 dbt-databricks-1.5.0rc1/dbt/include/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.326407 dbt-databricks-1.5.0rc1/dbt/include/databricks/
--rw-r--r--   0 andre.furlan   (502) staff       (20)       52 2022-11-22 20:51:35.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/__init__.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)       77 2022-11-22 20:51:35.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/dbt_project.yml
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.329448 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/
--rw-r--r--   0 andre.furlan   (502) staff       (20)    10178 2023-05-02 22:12:17.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/adapters.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      592 2022-11-22 20:51:35.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/catalog.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2409 2023-02-28 19:04:11.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/copy_into.sql
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.332059 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.333883 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/incremental/
--rw-r--r--   0 andre.furlan   (502) staff       (20)     4128 2023-05-02 16:19:19.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     3910 2023-05-02 16:19:19.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2066 2023-05-02 16:19:19.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/incremental/validate.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2451 2022-11-22 20:51:35.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/seed.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     5397 2023-02-28 19:04:11.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/snapshot.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     1616 2023-04-19 17:58:37.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/table.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      119 2022-11-22 20:51:35.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/view.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      648 2022-11-22 20:51:35.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/statement.sql
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.335116 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/utils/
--rw-r--r--   0 andre.furlan   (502) staff       (20)      318 2023-02-28 19:04:11.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/utils/dateadd.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      338 2023-02-28 19:04:11.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/utils/datediff.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      535 2023-05-02 22:11:51.000000 dbt-databricks-1.5.0rc1/dbt/include/databricks/profile_template.yml
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-02 22:21:00.338739 dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/
--rw-r--r--   0 andre.furlan   (502) staff       (20)     5378 2023-05-02 22:21:00.000000 dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/PKG-INFO
--rw-r--r--   0 andre.furlan   (502) staff       (20)     1421 2023-05-02 22:21:00.000000 dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-05-02 22:21:00.000000 dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-05-02 22:20:40.000000 dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/not-zip-safe
--rw-r--r--   0 andre.furlan   (502) staff       (20)       88 2023-05-02 22:21:00.000000 dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/requires.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)        4 2023-05-02 22:21:00.000000 dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/top_level.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)       38 2023-05-02 22:21:00.339805 dbt-databricks-1.5.0rc1/setup.cfg
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2547 2023-05-02 22:12:17.000000 dbt-databricks-1.5.0rc1/setup.py
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-09 15:23:38.508041 dbt-databricks-1.5.1/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       46 2022-11-22 20:51:35.000000 dbt-databricks-1.5.1/MANIFEST.in
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     5375 2023-05-09 15:23:38.507836 dbt-databricks-1.5.1/PKG-INFO
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     4572 2023-05-02 22:20:31.000000 dbt-databricks-1.5.1/README.md
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-09 15:23:38.484805 dbt-databricks-1.5.1/dbt/
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-09 15:23:38.484362 dbt-databricks-1.5.1/dbt/adapters/
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-09 15:23:38.494494 dbt-databricks-1.5.1/dbt/adapters/databricks/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      626 2023-02-28 19:04:11.000000 dbt-databricks-1.5.1/dbt/adapters/databricks/__init__.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       22 2023-05-09 15:13:49.000000 dbt-databricks-1.5.1/dbt/adapters/databricks/__version__.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2708 2023-05-02 22:11:51.000000 dbt-databricks-1.5.1/dbt/adapters/databricks/auth.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      586 2023-02-28 19:04:11.000000 dbt-databricks-1.5.1/dbt/adapters/databricks/column.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)    26590 2023-05-02 22:11:51.000000 dbt-databricks-1.5.1/dbt/adapters/databricks/connections.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)    19041 2023-05-02 22:20:31.000000 dbt-databricks-1.5.1/dbt/adapters/databricks/impl.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)    17731 2023-05-02 22:11:51.000000 dbt-databricks-1.5.1/dbt/adapters/databricks/python_submissions.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2863 2023-02-28 19:04:11.000000 dbt-databricks-1.5.1/dbt/adapters/databricks/relation.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2117 2023-02-28 19:04:11.000000 dbt-databricks-1.5.1/dbt/adapters/databricks/utils.py
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-09 15:23:38.484985 dbt-databricks-1.5.1/dbt/include/
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-09 15:23:38.496348 dbt-databricks-1.5.1/dbt/include/databricks/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       52 2022-11-22 20:51:35.000000 dbt-databricks-1.5.1/dbt/include/databricks/__init__.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       77 2022-11-22 20:51:35.000000 dbt-databricks-1.5.1/dbt/include/databricks/dbt_project.yml
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-09 15:23:38.498479 dbt-databricks-1.5.1/dbt/include/databricks/macros/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)    10178 2023-05-02 22:12:17.000000 dbt-databricks-1.5.1/dbt/include/databricks/macros/adapters.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      592 2022-11-22 20:51:35.000000 dbt-databricks-1.5.1/dbt/include/databricks/macros/catalog.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2409 2023-02-28 19:04:11.000000 dbt-databricks-1.5.1/dbt/include/databricks/macros/copy_into.sql
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-09 15:23:38.500692 dbt-databricks-1.5.1/dbt/include/databricks/macros/materializations/
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-09 15:23:38.502510 dbt-databricks-1.5.1/dbt/include/databricks/macros/materializations/incremental/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     4128 2023-05-02 16:19:19.000000 dbt-databricks-1.5.1/dbt/include/databricks/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     3910 2023-05-02 16:19:19.000000 dbt-databricks-1.5.1/dbt/include/databricks/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2066 2023-05-02 16:19:19.000000 dbt-databricks-1.5.1/dbt/include/databricks/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2451 2022-11-22 20:51:35.000000 dbt-databricks-1.5.1/dbt/include/databricks/macros/materializations/seed.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     5397 2023-02-28 19:04:11.000000 dbt-databricks-1.5.1/dbt/include/databricks/macros/materializations/snapshot.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     1616 2023-04-19 17:58:37.000000 dbt-databricks-1.5.1/dbt/include/databricks/macros/materializations/table.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      119 2022-11-22 20:51:35.000000 dbt-databricks-1.5.1/dbt/include/databricks/macros/materializations/view.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      648 2022-11-22 20:51:35.000000 dbt-databricks-1.5.1/dbt/include/databricks/macros/statement.sql
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-09 15:23:38.503759 dbt-databricks-1.5.1/dbt/include/databricks/macros/utils/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      318 2023-02-28 19:04:11.000000 dbt-databricks-1.5.1/dbt/include/databricks/macros/utils/dateadd.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      338 2023-02-28 19:04:11.000000 dbt-databricks-1.5.1/dbt/include/databricks/macros/utils/datediff.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      535 2023-05-02 22:11:51.000000 dbt-databricks-1.5.1/dbt/include/databricks/profile_template.yml
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-05-09 15:23:38.507451 dbt-databricks-1.5.1/dbt_databricks.egg-info/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     5375 2023-05-09 15:23:38.000000 dbt-databricks-1.5.1/dbt_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     1421 2023-05-09 15:23:38.000000 dbt-databricks-1.5.1/dbt_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-05-09 15:23:38.000000 dbt-databricks-1.5.1/dbt_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-05-02 22:20:40.000000 dbt-databricks-1.5.1/dbt_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      105 2023-05-09 15:23:38.000000 dbt-databricks-1.5.1/dbt_databricks.egg-info/requires.txt
+-rw-r--r--   0 andre.furlan   (502) staff       (20)        4 2023-05-09 15:23:38.000000 dbt-databricks-1.5.1/dbt_databricks.egg-info/top_level.txt
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       38 2023-05-09 15:23:38.508095 dbt-databricks-1.5.1/setup.cfg
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2607 2023-05-09 15:23:03.000000 dbt-databricks-1.5.1/setup.py
```

### Comparing `dbt-databricks-1.5.0rc1/PKG-INFO` & `dbt-databricks-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.5.0rc1
+Version: 1.5.1
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-databricks-1.5.0rc1/README.md` & `dbt-databricks-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/adapters/databricks/__init__.py` & `dbt-databricks-1.5.1/dbt/adapters/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/adapters/databricks/auth.py` & `dbt-databricks-1.5.1/dbt/adapters/databricks/auth.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/adapters/databricks/column.py` & `dbt-databricks-1.5.1/dbt/adapters/databricks/column.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/adapters/databricks/connections.py` & `dbt-databricks-1.5.1/dbt/adapters/databricks/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/adapters/databricks/impl.py` & `dbt-databricks-1.5.1/dbt/adapters/databricks/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/adapters/databricks/python_submissions.py` & `dbt-databricks-1.5.1/dbt/adapters/databricks/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/adapters/databricks/relation.py` & `dbt-databricks-1.5.1/dbt/adapters/databricks/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/adapters/databricks/utils.py` & `dbt-databricks-1.5.1/dbt/adapters/databricks/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/adapters.sql` & `dbt-databricks-1.5.1/dbt/include/databricks/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/catalog.sql` & `dbt-databricks-1.5.1/dbt/include/databricks/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/copy_into.sql` & `dbt-databricks-1.5.1/dbt/include/databricks/macros/copy_into.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/incremental/incremental.sql` & `dbt-databricks-1.5.1/dbt/include/databricks/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/incremental/strategies.sql` & `dbt-databricks-1.5.1/dbt/include/databricks/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/incremental/validate.sql` & `dbt-databricks-1.5.1/dbt/include/databricks/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/seed.sql` & `dbt-databricks-1.5.1/dbt/include/databricks/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/snapshot.sql` & `dbt-databricks-1.5.1/dbt/include/databricks/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/materializations/table.sql` & `dbt-databricks-1.5.1/dbt/include/databricks/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/include/databricks/macros/statement.sql` & `dbt-databricks-1.5.1/dbt/include/databricks/macros/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt/include/databricks/profile_template.yml` & `dbt-databricks-1.5.1/dbt/include/databricks/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/PKG-INFO` & `dbt-databricks-1.5.1/dbt_databricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.5.0rc1
+Version: 1.5.1
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-databricks-1.5.0rc1/dbt_databricks.egg-info/SOURCES.txt` & `dbt-databricks-1.5.1/dbt_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.0rc1/setup.py` & `dbt-databricks-1.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,16 @@
     url="https://github.com/databricks/dbt-databricks",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-spark>=1.5.0",
         "databricks-sql-connector>=2.5.0",
         "databricks-sdk>=0.1.1",
-        "keyring>=23.13.0"
+        "keyring>=23.13.0",
+        "protobuf>=4.21.0" # workaround for dbt-core issue
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
```

