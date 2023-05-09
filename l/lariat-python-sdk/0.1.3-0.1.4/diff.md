# Comparing `tmp/lariat_python_sdk-0.1.3.tar.gz` & `tmp/lariat_python_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lariat_python_sdk-0.1.3.tar", last modified: Fri May  5 04:25:20 2023, max compression
+gzip compressed data, was "lariat_python_sdk-0.1.4.tar", last modified: Tue May  9 14:33:32 2023, max compression
```

## Comparing `lariat_python_sdk-0.1.3.tar` & `lariat_python_sdk-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-05 04:25:20.558365 lariat_python_sdk-0.1.3/
--rw-r--r--   0 vikas      (501) staff       (20)     1498 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.3/LICENSE
--rw-r--r--   0 vikas      (501) staff       (20)     2407 2023-05-05 04:25:20.558208 lariat_python_sdk-0.1.3/PKG-INFO
--rw-r--r--   0 vikas      (501) staff       (20)     1427 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.3/README.md
-drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-05 04:25:20.556843 lariat_python_sdk-0.1.3/lariat_client/
--rw-r--r--   0 vikas      (501) staff       (20)      332 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.3/lariat_client/__init__.py
--rw-r--r--   0 vikas      (501) staff       (20)    19981 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.3/lariat_client/lariat_client.py
-drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-05 04:25:20.557809 lariat_python_sdk-0.1.3/lariat_python_sdk.egg-info/
--rw-r--r--   0 vikas      (501) staff       (20)     2407 2023-05-05 04:25:20.000000 lariat_python_sdk-0.1.3/lariat_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 vikas      (501) staff       (20)      321 2023-05-05 04:25:20.000000 lariat_python_sdk-0.1.3/lariat_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 vikas      (501) staff       (20)        1 2023-05-05 04:25:20.000000 lariat_python_sdk-0.1.3/lariat_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 vikas      (501) staff       (20)       43 2023-05-05 04:25:20.000000 lariat_python_sdk-0.1.3/lariat_python_sdk.egg-info/requires.txt
--rw-r--r--   0 vikas      (501) staff       (20)       14 2023-05-05 04:25:20.000000 lariat_python_sdk-0.1.3/lariat_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 vikas      (501) staff       (20)     1102 2023-05-05 04:25:11.000000 lariat_python_sdk-0.1.3/pyproject.toml
--rw-r--r--   0 vikas      (501) staff       (20)       38 2023-05-05 04:25:20.558411 lariat_python_sdk-0.1.3/setup.cfg
-drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-05 04:25:20.557965 lariat_python_sdk-0.1.3/tests/
--rw-r--r--   0 vikas      (501) staff       (20)     6746 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.3/tests/test_lariat_client.py
+drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-09 14:33:32.300390 lariat_python_sdk-0.1.4/
+-rw-r--r--   0 vikas      (501) staff       (20)     1498 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.4/LICENSE
+-rw-r--r--   0 vikas      (501) staff       (20)     2403 2023-05-09 14:33:32.300240 lariat_python_sdk-0.1.4/PKG-INFO
+-rw-r--r--   0 vikas      (501) staff       (20)     1423 2023-05-09 13:33:08.000000 lariat_python_sdk-0.1.4/README.md
+drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-09 14:33:32.298936 lariat_python_sdk-0.1.4/lariat_client/
+-rw-r--r--   0 vikas      (501) staff       (20)      332 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.4/lariat_client/__init__.py
+-rw-r--r--   0 vikas      (501) staff       (20)    20104 2023-05-09 14:26:22.000000 lariat_python_sdk-0.1.4/lariat_client/lariat_client.py
+drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-09 14:33:32.299839 lariat_python_sdk-0.1.4/lariat_python_sdk.egg-info/
+-rw-r--r--   0 vikas      (501) staff       (20)     2403 2023-05-09 14:33:32.000000 lariat_python_sdk-0.1.4/lariat_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 vikas      (501) staff       (20)      321 2023-05-09 14:33:32.000000 lariat_python_sdk-0.1.4/lariat_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 vikas      (501) staff       (20)        1 2023-05-09 14:33:32.000000 lariat_python_sdk-0.1.4/lariat_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 vikas      (501) staff       (20)       43 2023-05-09 14:33:32.000000 lariat_python_sdk-0.1.4/lariat_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 vikas      (501) staff       (20)       14 2023-05-09 14:33:32.000000 lariat_python_sdk-0.1.4/lariat_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 vikas      (501) staff       (20)     1102 2023-05-09 14:28:41.000000 lariat_python_sdk-0.1.4/pyproject.toml
+-rw-r--r--   0 vikas      (501) staff       (20)       38 2023-05-09 14:33:32.300434 lariat_python_sdk-0.1.4/setup.cfg
+drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-09 14:33:32.299973 lariat_python_sdk-0.1.4/tests/
+-rw-r--r--   0 vikas      (501) staff       (20)     6746 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.4/tests/test_lariat_client.py
```

### Comparing `lariat_python_sdk-0.1.3/LICENSE` & `lariat_python_sdk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lariat_python_sdk-0.1.3/PKG-INFO` & `lariat_python_sdk-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lariat_python_sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python module to interact with Lariat API to access data quality metrics and diagnostics
 Author-email: Lariat Data Team <info@lariatdata.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://www.lariatdata.com
 Project-URL: documentation, https://lariat-python-sdk.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/lariat-data/lariat-python-sdk
 Classifier: Development Status :: 3 - Alpha
@@ -76,15 +76,15 @@
 
 Query an indicator:
 
 ```python
 from_ts = datetime.datetime(2022, 1, 1)
 to_ts = datetime.datetime(2022, 2, 1)
 group_by = ["country"]
-filter_clause = FilterClause(field="country", operator="in", values=["US", "UK"])
+filter_clause = FilterClause(field="country", operator="in", values="US,UK"])
 query_filter = Filter(clauses=[filter_clause], operator="and")
 
 results = query(indicator["id"], from_ts, to_ts, group_by, query_filter=query_filter)
 
 # Convert results to a DataFrame
 results_df = results.to_df()
```

### Comparing `lariat_python_sdk-0.1.3/README.md` & `lariat_python_sdk-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 Query an indicator:
 
 ```python
 from_ts = datetime.datetime(2022, 1, 1)
 to_ts = datetime.datetime(2022, 2, 1)
 group_by = ["country"]
-filter_clause = FilterClause(field="country", operator="in", values=["US", "UK"])
+filter_clause = FilterClause(field="country", operator="in", values="US,UK"])
 query_filter = Filter(clauses=[filter_clause], operator="and")
 
 results = query(indicator["id"], from_ts, to_ts, group_by, query_filter=query_filter)
 
 # Convert results to a DataFrame
 results_df = results.to_df()
```

### Comparing `lariat_python_sdk-0.1.3/lariat_client/lariat_client.py` & `lariat_python_sdk-0.1.4/lariat_client/lariat_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,16 +107,15 @@
         Fetches the unique values of the specified dimensions for the indicator.
 
         Args:
             dimensions (List[str], optional): The list of dimensions to fetch values for.
                 If not provided, all dimensions will be fetched.
 
         Returns:
-            Dict[str, List[str]]: A dictionary with dimension names as keys and lists of
-                unique values as values.
+            Dict[str, List[str]]: A dictionary with dimension names as keys and lists of unique values as values.
         """
         try:
             r = s.get(
                 f"{LARIAT_PUBLIC_API_ENDPOINT}/indicators/{self.id}/dimensions",
                 params={"dimensions": dimensions},
             )
             r.raise_for_status()
@@ -211,15 +210,15 @@
 
 
 class FilterClause:
     """A class representing a clause to filter metrics by.
 
     Attributes:
         field (str): The field to filter on.
-        operator (str): The operator to apply to the filter values. (in, eq, not_in, neq, etc.)
+        operator (str): The operator to apply to the filter values. Supported operators: [in, not_in, eq, neq]
         values (list or str): A string or list of values to filter on.
     """
 
     def __init__(self, field: str, operator: str, values: Union[str, List[str]]):
         self.field = field
         self.operator = operator
         self.values = values
@@ -229,15 +228,15 @@
 
 
 class Filter:
     """A class representing a filter to use when querying metrics.
 
     Attributes:
         clauses (list): A list of filter clauses to apply when querying metrics.
-        operator (str): The operator to apply to the filter clauses. (AND, OR, etc.)
+        operator (str): The operator to apply to the filter clauses. The options for this are [any, all]. The default operator is 'all'. 'any' corresponds to an "OR"ing of the clauses, and 'all' corresponds to an "AND"ing of the clauses
     """
 
     def __init__(self, clauses: List[FilterClause], operator: str):
         self.clauses = clauses
         self.operator = operator
 
     def __repr__(self):
@@ -308,16 +307,15 @@
         return record
 
     def to_df(self) -> pd.DataFrame:
         """
         Converts the MetricRecord list into a pandas dataframe.
 
         Returns:
-            Pandas DataFrame: A Dataframe consisting of the metric records
-                returned by an indicator query.
+            Pandas DataFrame: A Dataframe consisting of the metric records returned by an indicator query.
         """
         return pd.DataFrame.from_records([record.to_dict() for record in self.records])
 
     def to_csv(self, filename, header=True):
         """
         Writes the MetricRecord list to a csv.
         """
@@ -337,16 +335,15 @@
     """
     Gets the raw datasets given a list of dataset ids.
 
     Args:
         dataset_ids (list): A list of dataset ids to filter on.
 
     Returns:
-        List[RawDataset]: A list of raw datasets that the provided dataset_ids
-            are created from.
+        List[RawDataset]: A list of raw datasets that the provided dataset_ids are created from.
     """
     try:
         r = s.get(
             f"{LARIAT_PUBLIC_API_ENDPOINT}/raw-datasets",
             params={"dataset_id": dataset_ids},
         )
         r.raise_for_status()
```

### Comparing `lariat_python_sdk-0.1.3/lariat_python_sdk.egg-info/PKG-INFO` & `lariat_python_sdk-0.1.4/lariat_python_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lariat-python-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python module to interact with Lariat API to access data quality metrics and diagnostics
 Author-email: Lariat Data Team <info@lariatdata.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://www.lariatdata.com
 Project-URL: documentation, https://lariat-python-sdk.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/lariat-data/lariat-python-sdk
 Classifier: Development Status :: 3 - Alpha
@@ -76,15 +76,15 @@
 
 Query an indicator:
 
 ```python
 from_ts = datetime.datetime(2022, 1, 1)
 to_ts = datetime.datetime(2022, 2, 1)
 group_by = ["country"]
-filter_clause = FilterClause(field="country", operator="in", values=["US", "UK"])
+filter_clause = FilterClause(field="country", operator="in", values="US,UK"])
 query_filter = Filter(clauses=[filter_clause], operator="and")
 
 results = query(indicator["id"], from_ts, to_ts, group_by, query_filter=query_filter)
 
 # Convert results to a DataFrame
 results_df = results.to_df()
```

### Comparing `lariat_python_sdk-0.1.3/pyproject.toml` & `lariat_python_sdk-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lariat_python_sdk"
-version = "0.1.3"
+version = "0.1.4"
 description = "A Python module to interact with Lariat API to access data quality metrics and diagnostics"
 readme = "README.md"
 authors = [
     { name = "Lariat Data Team", email = "info@lariatdata.com"}
 ]
 license = {text = "BSD-3-Clause"}
 dependencies = [
```

### Comparing `lariat_python_sdk-0.1.3/tests/test_lariat_client.py` & `lariat_python_sdk-0.1.4/tests/test_lariat_client.py`

 * *Files identical despite different names*

