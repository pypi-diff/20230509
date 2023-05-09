# Comparing `tmp/hagis-0.7.1.tar.gz` & `tmp/hagis-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.7.1.tar", last modified: Mon May  8 17:54:45 2023, max compression
+gzip compressed data, was "hagis-0.7.2.tar", last modified: Tue May  9 12:42:11 2023, max compression
```

## Comparing `hagis-0.7.1.tar` & `hagis-0.7.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 17:54:45.706810 hagis-0.7.1/
--rw-rw-rw-   0        0        0      923 2023-05-08 17:54:45.704807 hagis-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 17:54:45.702820 hagis-0.7.1/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-05-08 17:54:45.000000 hagis-0.7.1/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-05-08 17:54:45.000000 hagis-0.7.1/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 17:54:45.000000 hagis-0.7.1/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-08 17:54:45.000000 hagis-0.7.1/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    23365 2023-05-08 17:53:26.000000 hagis-0.7.1/hagis.py
--rw-rw-rw-   0        0        0      589 2023-05-08 17:54:17.000000 hagis-0.7.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 17:54:45.706810 hagis-0.7.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 12:42:11.471745 hagis-0.7.2/
+-rw-rw-rw-   0        0        0      923 2023-05-09 12:42:11.463751 hagis-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 12:42:11.455492 hagis-0.7.2/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-05-09 12:42:11.000000 hagis-0.7.2/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-05-09 12:42:11.000000 hagis-0.7.2/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 12:42:11.000000 hagis-0.7.2/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-09 12:42:11.000000 hagis-0.7.2/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    23599 2023-05-09 12:26:32.000000 hagis-0.7.2/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-05-09 12:40:09.000000 hagis-0.7.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 12:42:11.471745 hagis-0.7.2/setup.cfg
```

### Comparing `hagis-0.7.1/PKG-INFO` & `hagis-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.7.1
+Version: 0.7.2
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.7.1/hagis.egg-info/PKG-INFO` & `hagis-0.7.2/hagis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.7.1
+Version: 0.7.2
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.7.1/hagis.py` & `hagis-0.7.2/hagis.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from inspect import getsource, signature
 from itertools import chain, islice
 from json import dumps, loads
 from time import time
 from types import SimpleNamespace
 from typing import Any, Callable, Dict, Generic, Iterator, List, Optional, Tuple, Type, TypeVar, Union
 from uuid import UUID
-from requests import post
+from requests import Session
+from requests.adapters import HTTPAdapter, Retry
 
 T = TypeVar("T")
 
 
 class Layer(Generic[T]):  # pylint: disable=too-many-instance-attributes
     """ Layer class.
 
@@ -301,15 +302,18 @@
             else:
                 attributes[field] = value
 
         return dictionary
 
     def _post(self, url: str, **kwargs: Any) -> SimpleNamespace:
         kwargs["f"] = "json"
-        response = post(url, data=kwargs, timeout=10)
+
+        session = Session()
+        session.mount("https://", HTTPAdapter(max_retries=Retry(total=7, backoff_factor=0.1)))
+        response = session.post(url, data=kwargs, timeout=10)
         obj = loads(response.text, object_hook=lambda x: SimpleNamespace(**x))
 
         if hasattr(obj, "error"):
             raise RuntimeError(obj.error.message)
 
         return obj
 
@@ -338,15 +342,15 @@
                     feature.attributes.__dict__[key] = datetime.utcfromtimestamp(value / 1000)
                 elif key in uuid_fields:
                     feature.attributes.__dict__[key] = UUID(value)
                 elif not self._is_dynamic:
                     lower_field: str = key.lower()
                     if lower_field in self._lower_field_to_property_name_type:
                         _, property_type = self._lower_field_to_property_name_type[lower_field]
-                        if issubclass(property_type, Enum):
+                        if issubclass(property_type, Enum) and value in property_type._value2member_map_:
                             feature.attributes.__dict__[key] = property_type(value)
 
             if hasattr(feature, "geometry") and feature.geometry and hasattr(obj, "spatialReference"):
                 feature.geometry.spatialReference = obj.spatialReference.__dict__
 
         return (obj.features, obj.exceededTransferLimit if hasattr(obj, "exceededTransferLimit") else False)
```

### Comparing `hagis-0.7.1/pyproject.toml` & `hagis-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

