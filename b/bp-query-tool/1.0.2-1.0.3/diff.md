# Comparing `tmp/bp_query_tool-1.0.2.tar.gz` & `tmp/bp_query_tool-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_query_tool-1.0.2.tar", last modified: Thu May  4 09:43:18 2023, max compression
+gzip compressed data, was "bp_query_tool-1.0.3.tar", last modified: Tue May  9 05:58:13 2023, max compression
```

## Comparing `bp_query_tool-1.0.2.tar` & `bp_query_tool-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 09:43:18.311529 bp_query_tool-1.0.2/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 bp_query_tool-1.0.2/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 bp_query_tool-1.0.2/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3833 2023-05-04 09:43:18.311007 bp_query_tool-1.0.2/PKG-INFO
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 09:43:18.300072 bp_query_tool-1.0.2/bp_query_tool.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3833 2023-05-04 09:43:18.000000 bp_query_tool-1.0.2/bp_query_tool.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      674 2023-05-04 09:43:18.000000 bp_query_tool-1.0.2/bp_query_tool.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-04 09:43:18.000000 bp_query_tool-1.0.2/bp_query_tool.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-05-04 09:43:18.000000 bp_query_tool-1.0.2/bp_query_tool.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-05-04 09:43:18.000000 bp_query_tool-1.0.2/bp_query_tool.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 09:43:18.300682 bp_query_tool-1.0.2/query_tool/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3985 2023-05-04 09:33:22.000000 bp_query_tool-1.0.2/query_tool/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 09:43:18.295766 bp_query_tool-1.0.2/query_tool/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 09:43:18.301805 bp_query_tool-1.0.2/query_tool/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 09:43:18.303304 bp_query_tool-1.0.2/query_tool/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-04 09:40:18.000000 bp_query_tool-1.0.2/query_tool/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1040683 2023-05-04 09:40:18.000000 bp_query_tool-1.0.2/query_tool/frontend/dist/assets/index-e2f3e6a4.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      568 2023-05-04 09:41:11.000000 bp_query_tool-1.0.2/query_tool/frontend/dist/index.html
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-05-04 09:40:17.000000 bp_query_tool-1.0.2/query_tool/frontend/dist/vite.svg
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 09:43:18.310075 bp_query_tool-1.0.2/query_tool/services/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 bp_query_tool-1.0.2/query_tool/services/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1661 2023-05-04 07:12:03.000000 bp_query_tool-1.0.2/query_tool/services/dimension_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 bp_query_tool-1.0.2/query_tool/services/entities_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3839 2023-04-26 08:59:45.000000 bp_query_tool-1.0.2/query_tool/services/filters_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 bp_query_tool-1.0.2/query_tool/services/query_tool_factory.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2414 2023-05-04 07:36:07.000000 bp_query_tool-1.0.2/query_tool/services/query_tool_service.py
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 bp_query_tool-1.0.2/query_tool/services/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-04 09:43:18.311704 bp_query_tool-1.0.2/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      790 2023-05-04 09:43:06.000000 bp_query_tool-1.0.2/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-09 05:58:13.515966 bp_query_tool-1.0.3/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 bp_query_tool-1.0.3/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 bp_query_tool-1.0.3/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3833 2023-05-09 05:58:13.515311 bp_query_tool-1.0.3/PKG-INFO
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-09 05:58:13.505498 bp_query_tool-1.0.3/bp_query_tool.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3833 2023-05-09 05:58:13.000000 bp_query_tool-1.0.3/bp_query_tool.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      674 2023-05-09 05:58:13.000000 bp_query_tool-1.0.3/bp_query_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-09 05:58:13.000000 bp_query_tool-1.0.3/bp_query_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-05-09 05:58:13.000000 bp_query_tool-1.0.3/bp_query_tool.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-05-09 05:58:13.000000 bp_query_tool-1.0.3/bp_query_tool.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-09 05:58:13.506024 bp_query_tool-1.0.3/query_tool/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3985 2023-05-04 09:33:22.000000 bp_query_tool-1.0.3/query_tool/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-09 05:58:13.501250 bp_query_tool-1.0.3/query_tool/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-09 05:58:13.507248 bp_query_tool-1.0.3/query_tool/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-09 05:58:13.508625 bp_query_tool-1.0.3/query_tool/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-04 09:40:18.000000 bp_query_tool-1.0.3/query_tool/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1040683 2023-05-04 09:40:18.000000 bp_query_tool-1.0.3/query_tool/frontend/dist/assets/index-e2f3e6a4.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      568 2023-05-04 09:41:11.000000 bp_query_tool-1.0.3/query_tool/frontend/dist/index.html
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-05-04 09:40:17.000000 bp_query_tool-1.0.3/query_tool/frontend/dist/vite.svg
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-09 05:58:13.514603 bp_query_tool-1.0.3/query_tool/services/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 bp_query_tool-1.0.3/query_tool/services/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1661 2023-05-04 07:12:03.000000 bp_query_tool-1.0.3/query_tool/services/dimension_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 bp_query_tool-1.0.3/query_tool/services/entities_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3839 2023-04-26 08:59:45.000000 bp_query_tool-1.0.3/query_tool/services/filters_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 bp_query_tool-1.0.3/query_tool/services/query_tool_factory.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2643 2023-05-09 05:18:33.000000 bp_query_tool-1.0.3/query_tool/services/query_tool_service.py
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 bp_query_tool-1.0.3/query_tool/services/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-09 05:58:13.516116 bp_query_tool-1.0.3/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      790 2023-05-09 05:30:23.000000 bp_query_tool-1.0.3/setup.py
```

### Comparing `bp_query_tool-1.0.2/LICENSE` & `bp_query_tool-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.2/PKG-INFO` & `bp_query_tool-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bp_query_tool
-Version: 1.0.2
+Version: 1.0.3
 Summary: Query tool to generate query from selection
 Home-page: UNKNOWN
 Author: Bluepinapple
 Author-email: vivek.sthul@bluepinapple.com
 License: UNKNOWN
 Description: # Query Tool
```

### Comparing `bp_query_tool-1.0.2/bp_query_tool.egg-info/PKG-INFO` & `bp_query_tool-1.0.3/bp_query_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bp-query-tool
-Version: 1.0.2
+Version: 1.0.3
 Summary: Query tool to generate query from selection
 Home-page: UNKNOWN
 Author: Bluepinapple
 Author-email: vivek.sthul@bluepinapple.com
 License: UNKNOWN
 Description: # Query Tool
```

### Comparing `bp_query_tool-1.0.2/bp_query_tool.egg-info/SOURCES.txt` & `bp_query_tool-1.0.3/bp_query_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.2/query_tool/__init__.py` & `bp_query_tool-1.0.3/query_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.2/query_tool/frontend/dist/assets/index-e2f3e6a4.js` & `bp_query_tool-1.0.3/query_tool/frontend/dist/assets/index-e2f3e6a4.js`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.2/query_tool/frontend/dist/index.html` & `bp_query_tool-1.0.3/query_tool/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.2/query_tool/frontend/dist/vite.svg` & `bp_query_tool-1.0.3/query_tool/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.2/query_tool/services/dimension_service.py` & `bp_query_tool-1.0.3/query_tool/services/dimension_service.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.2/query_tool/services/entities_service.py` & `bp_query_tool-1.0.3/query_tool/services/entities_service.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.2/query_tool/services/filters_service.py` & `bp_query_tool-1.0.3/query_tool/services/filters_service.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.2/query_tool/services/query_tool_service.py` & `bp_query_tool-1.0.3/query_tool/services/query_tool_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,34 +20,36 @@
         return self.__get_query(
             entities_columns,
             relations,
             filters,
             dimensions,
             measures,
             entities_tables_with_aliases,
-            measure_columns
+            measure_columns,
+            query_json
         )
 
     def __get_query(
         self,
         entities_columns,
         relations,
         filters,
         dimensions,
         measures,
         entities_tables_with_aliases,
-        measure_columns
+        measure_columns,
+        query_json
     ) -> str:
         sql_array = ["SELECT"]
         select_query = ""
 
         if len(entities_columns) > 0:
             # Check select columns are in group by clause or in aggregate columns list
             if len(dimensions) > 0:
-                select_columns = [select_column for select_column in entities_columns if select_column in dimensions or select_column in measure_columns]
+                select_columns = [select_column for select_column in entities_columns if select_column in dimensions]
                 select_query += ", ".join(select_columns)
             else: 
                 select_query += ", ".join(entities_columns)
 
         if len(measures) > 0:
             select_query = f"{select_query}, " if select_query else select_query
             select_query += ", ".join(measures)
@@ -65,8 +67,12 @@
             sql_array.append("WHERE")
             sql_array.append(" ".join(filters))
 
         if len(dimensions) > 0:
             sql_array.append("GROUP BY")
             sql_array.append(", ".join(dimensions))
 
+        options = query_json.get("options", {})
+        limit_records = options.get("limit", None)
+        if limit_records is not None and limit_records != -1:
+            sql_array.append("LIMIT " + str(limit_records))
         return " ".join(sql_array)
```

### Comparing `bp_query_tool-1.0.2/query_tool/services/register.py` & `bp_query_tool-1.0.3/query_tool/services/register.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.2/setup.py` & `bp_query_tool-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="bp_query_tool",
-    version="1.0.2",
+    version="1.0.3",
     author="Bluepinapple",
     author_email="vivek.sthul@bluepinapple.com",
     description="Query tool to generate query from selection",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

