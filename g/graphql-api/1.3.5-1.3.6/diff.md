# Comparing `tmp/graphql-api-1.3.5.tar.gz` & `tmp/graphql-api-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql-api-1.3.5.tar", last modified: Sat May  6 01:37:09 2023, max compression
+gzip compressed data, was "graphql-api-1.3.6.tar", last modified: Tue May  9 14:49:41 2023, max compression
```

## Comparing `graphql-api-1.3.5.tar` & `graphql-api-1.3.6.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:37:09.025891 graphql-api-1.3.5/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-06 01:36:58.000000 graphql-api-1.3.5/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       73 2023-05-06 01:36:58.000000 graphql-api-1.3.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1946 2023-05-06 01:37:09.025891 graphql-api-1.3.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1270 2023-05-06 01:36:58.000000 graphql-api-1.3.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-06 01:37:08.000000 graphql-api-1.3.5/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:37:09.019890 graphql-api-1.3.5/graphql_api/
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7527 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/api.py
--rwxrwxrwx   0 root         (0) root         (0)      558 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/context.py
--rwxrwxrwx   0 root         (0) root         (0)     3422 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/dataclass_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/decorators.py
--rwxrwxrwx   0 root         (0) root         (0)      593 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/error.py
--rwxrwxrwx   0 root         (0) root         (0)       52 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/exception.py
--rwxrwxrwx   0 root         (0) root         (0)     5868 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/executor.py
--rwxrwxrwx   0 root         (0) root         (0)    24042 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/mapper.py
--rwxrwxrwx   0 root         (0) root         (0)     3070 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/middleware.py
--rwxrwxrwx   0 root         (0) root         (0)     6756 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/reduce.py
--rwxrwxrwx   0 root         (0) root         (0)     3154 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/relay.py
--rwxrwxrwx   0 root         (0) root         (0)    32869 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/remote.py
--rwxrwxrwx   0 root         (0) root         (0)     3372 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/types.py
--rwxrwxrwx   0 root         (0) root         (0)     5896 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:37:09.021890 graphql-api-1.3.5/graphql_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1946 2023-05-06 01:37:08.000000 graphql-api-1.3.5/graphql_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      806 2023-05-06 01:37:08.000000 graphql-api-1.3.5/graphql_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 01:37:08.000000 graphql-api-1.3.5/graphql_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-06 01:37:08.000000 graphql-api-1.3.5/graphql_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-06 01:37:08.000000 graphql-api-1.3.5/graphql_api.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-06 01:37:09.025891 graphql-api-1.3.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1413 2023-05-06 01:36:58.000000 graphql-api-1.3.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:37:09.024891 graphql-api-1.3.5/tests/
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5129 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_custom_types.py
--rwxrwxrwx   0 root         (0) root         (0)     5183 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_docstrings.py
--rwxrwxrwx   0 root         (0) root         (0)     3316 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_error.py
--rwxrwxrwx   0 root         (0) root         (0)     6939 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_filtering.py
--rwxrwxrwx   0 root         (0) root         (0)    35981 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_graphql.py
--rwxrwxrwx   0 root         (0) root         (0)     4026 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_relay.py
--rwxrwxrwx   0 root         (0) root         (0)    21648 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_remote.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3543 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:49:41.141230 graphql-api-1.3.6/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-09 14:49:31.000000 graphql-api-1.3.6/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       73 2023-05-09 14:49:31.000000 graphql-api-1.3.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-05-09 14:49:41.141230 graphql-api-1.3.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1270 2023-05-09 14:49:31.000000 graphql-api-1.3.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-09 14:49:40.000000 graphql-api-1.3.6/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:49:41.135230 graphql-api-1.3.6/graphql_api/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7527 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/api.py
+-rwxrwxrwx   0 root         (0) root         (0)      558 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/context.py
+-rwxrwxrwx   0 root         (0) root         (0)     3422 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/dataclass_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/decorators.py
+-rwxrwxrwx   0 root         (0) root         (0)      593 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/error.py
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/exception.py
+-rwxrwxrwx   0 root         (0) root         (0)     5868 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/executor.py
+-rwxrwxrwx   0 root         (0) root         (0)    24096 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/mapper.py
+-rwxrwxrwx   0 root         (0) root         (0)     3070 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/middleware.py
+-rwxrwxrwx   0 root         (0) root         (0)     6756 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/reduce.py
+-rwxrwxrwx   0 root         (0) root         (0)     3154 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    32869 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/remote.py
+-rwxrwxrwx   0 root         (0) root         (0)     4155 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/types.py
+-rwxrwxrwx   0 root         (0) root         (0)     5896 2023-05-09 14:49:31.000000 graphql-api-1.3.6/graphql_api/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:49:41.137230 graphql-api-1.3.6/graphql_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-05-09 14:49:41.000000 graphql-api-1.3.6/graphql_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      830 2023-05-09 14:49:41.000000 graphql-api-1.3.6/graphql_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 14:49:41.000000 graphql-api-1.3.6/graphql_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-09 14:49:41.000000 graphql-api-1.3.6/graphql_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-09 14:49:41.000000 graphql-api-1.3.6/graphql_api.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-09 14:49:41.141230 graphql-api-1.3.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1413 2023-05-09 14:49:31.000000 graphql-api-1.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:49:41.141230 graphql-api-1.3.6/tests/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5704 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_custom_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1350 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_dataclass.py
+-rwxrwxrwx   0 root         (0) root         (0)     5183 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_docstrings.py
+-rwxrwxrwx   0 root         (0) root         (0)     3316 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_error.py
+-rwxrwxrwx   0 root         (0) root         (0)     6939 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_filtering.py
+-rwxrwxrwx   0 root         (0) root         (0)    35981 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_graphql.py
+-rwxrwxrwx   0 root         (0) root         (0)     4026 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    21648 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_remote.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-05-09 14:49:31.000000 graphql-api-1.3.6/tests/test_subscriptions.py
```

### Comparing `graphql-api-1.3.5/LICENSE` & `graphql-api-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/PKG-INFO` & `graphql-api-1.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.3.5
+Version: 1.3.6
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.5/graphql-api-v1.3.5.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.6/graphql-api-v1.3.6.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql-api-1.3.5/README.md` & `graphql-api-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/graphql_api/api.py` & `graphql-api-1.3.6/graphql_api/api.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/graphql_api/context.py` & `graphql-api-1.3.6/graphql_api/context.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/graphql_api/dataclass_mapping.py` & `graphql-api-1.3.6/graphql_api/dataclass_mapping.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/graphql_api/error.py` & `graphql-api-1.3.6/graphql_api/error.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/graphql_api/executor.py` & `graphql-api-1.3.6/graphql_api/executor.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/graphql_api/mapper.py` & `graphql-api-1.3.6/graphql_api/mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import typing_inspect
 
 from uuid import UUID
 
 from typing import List, Union, Type, Callable, Tuple, Any, Dict, Set
 
 from typing_inspect import get_origin
-from datetime import datetime
+from datetime import datetime, date
 
 from graphql import (
     GraphQLObjectType,
     GraphQLField,
     GraphQLString,
     GraphQLList,
     GraphQLBoolean,
@@ -42,14 +42,15 @@
 from graphql_api.types import (
     GraphQLBytes,
     GraphQLUUID,
     GraphQLDateTime,
     GraphQLJSON,
     JsonType,
     GraphQLMappedEnumType,
+    GraphQLDate,
 )
 
 from graphql_api.utils import (
     to_camel_case,
     to_snake_case,
     to_input_value,
     to_camel_case_text,
@@ -329,14 +330,15 @@
         ([str], GraphQLString),
         ([bytes], GraphQLBytes),
         ([bool], GraphQLBoolean),
         ([int], GraphQLInt),
         ([dict, list, set], GraphQLJSON),
         ([float], GraphQLFloat),
         ([datetime], GraphQLDateTime),
+        ([date], GraphQLDate),
         ([type(None)], None),
     ]
 
     def scalar_classes(self):
         classes = []
         for scalar_class_map in self.scalar_map:
             for scalar_class in scalar_class_map[0]:
```

### Comparing `graphql-api-1.3.5/graphql_api/middleware.py` & `graphql-api-1.3.6/graphql_api/middleware.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/graphql_api/reduce.py` & `graphql-api-1.3.6/graphql_api/reduce.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/graphql_api/relay.py` & `graphql-api-1.3.6/graphql_api/relay.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/graphql_api/remote.py` & `graphql-api-1.3.6/graphql_api/remote.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/graphql_api/types.py` & `graphql-api-1.3.6/graphql_api/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -61,14 +61,45 @@
     "the datetime should be in the format `2018-01-22 17:46:32`",
     serialize=serialize_datetime,
     parse_value=parse_datetime_value,
     parse_literal=parse_datetime_literal,
 )
 
 
+def serialize_date(dt: datetime.date):
+    return dt.isoformat()
+
+
+def parse_date_value(value):
+    date_formats = ["%Y-%m-%d"]
+
+    for date_format in date_formats:
+        try:
+            return datetime.datetime.strptime(value, date_format).date()
+        except ValueError:
+            pass
+
+    raise ValueError(f"Date{value} did not fit any " f"of the formats {date_formats}.")
+
+
+def parse_date_literal(node):
+    if isinstance(node, StringValueNode):
+        return parse_date_value(node.value)
+
+
+GraphQLDate = GraphQLScalarType(
+    name="Date",
+    description="The `Date` scalar type represents a datetime, "
+    "the datetime should be in the format `2018-01-22`",
+    serialize=serialize_date,
+    parse_value=parse_date_value,
+    parse_literal=parse_date_literal,
+)
+
+
 JsonType = Union[None, int, float, str, bool, List, Dict]
 
 
 def serialize_json(data: JsonType) -> str:
     return json.dumps(data)
```

### Comparing `graphql-api-1.3.5/graphql_api/utils.py` & `graphql-api-1.3.6/graphql_api/utils.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/graphql_api.egg-info/PKG-INFO` & `graphql-api-1.3.6/graphql_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.3.5
+Version: 1.3.6
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.5/graphql-api-v1.3.5.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.6/graphql-api-v1.3.6.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql-api-1.3.5/graphql_api.egg-info/SOURCES.txt` & `graphql-api-1.3.6/graphql_api.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 graphql_api.egg-info/PKG-INFO
 graphql_api.egg-info/SOURCES.txt
 graphql_api.egg-info/dependency_links.txt
 graphql_api.egg-info/requires.txt
 graphql_api.egg-info/top_level.txt
 tests/__init__.py
 tests/test_custom_types.py
+tests/test_dataclass.py
 tests/test_docstrings.py
 tests/test_error.py
 tests/test_filtering.py
 tests/test_graphql.py
 tests/test_relay.py
 tests/test_remote.py
 tests/test_schema.py
```

### Comparing `graphql-api-1.3.5/setup.py` & `graphql-api-1.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/tests/test_custom_types.py` & `graphql-api-1.3.6/tests/test_custom_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import uuid
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, date
 from uuid import UUID
 
 from graphql_api.api import GraphQLAPI
 from graphql_api.types import JsonType
 
 
 class TestCustomTypes:
@@ -67,14 +67,35 @@
 
         result = executor.execute(test_time_query)
 
         expected = {"addOneHour": str(now + timedelta(hours=1))}
         assert not result.errors
         assert result.data == expected
 
+    def test_date_type(self):
+        api = GraphQLAPI()
+
+        now = date.today()
+
+        @api.type(root=True)
+        class Root:
+            @api.field
+            def add_one_day(self, date: date) -> date:
+                return date + timedelta(days=1)
+
+        executor = api.executor()
+
+        test_time_query = f'query GetTimeInOneHour {{ addOneDay(date: "{now}") }}'
+
+        result = executor.execute(test_time_query)
+
+        expected = {"addOneDay": str(now + timedelta(days=1))}
+        assert not result.errors
+        assert result.data == expected
+
     def test_json_type(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Root:
             @api.field
             def adapt_profile(self, profile: dict) -> dict:
```

### Comparing `graphql-api-1.3.5/tests/test_docstrings.py` & `graphql-api-1.3.6/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/tests/test_error.py` & `graphql-api-1.3.6/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/tests/test_filtering.py` & `graphql-api-1.3.6/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/tests/test_graphql.py` & `graphql-api-1.3.6/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/tests/test_relay.py` & `graphql-api-1.3.6/tests/test_relay.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/tests/test_remote.py` & `graphql-api-1.3.6/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/tests/test_schema.py` & `graphql-api-1.3.6/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.5/tests/test_subscriptions.py` & `graphql-api-1.3.6/tests/test_subscriptions.py`

 * *Files identical despite different names*

