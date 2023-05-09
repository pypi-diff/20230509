# Comparing `tmp/Flask-RESTful-DBBase-0.3.5.tar.gz` & `tmp/Flask-RESTful-DBBase-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-RESTful-DBBase-0.3.5.tar", last modified: Sat Apr 17 18:39:31 2021, max compression
+gzip compressed data, was "Flask-RESTful-DBBase-0.4.0.tar", last modified: Tue May  9 21:07:58 2023, max compression
```

## Comparing `Flask-RESTful-DBBase-0.3.5.tar` & `Flask-RESTful-DBBase-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,33 @@
-drwxr-xr-x   0 don       (1000) don       (1000)        0 2021-04-17 18:39:31.000000 Flask-RESTful-DBBase-0.3.5/
-drwxr-xr-x   0 don       (1000) don       (1000)        0 2021-04-17 18:39:31.000000 Flask-RESTful-DBBase-0.3.5/Flask_RESTful_DBBase.egg-info/
--rw-r--r--   0 don       (1000) don       (1000)     2370 2021-04-17 18:39:31.000000 Flask-RESTful-DBBase-0.3.5/Flask_RESTful_DBBase.egg-info/PKG-INFO
--rw-r--r--   0 don       (1000) don       (1000)      664 2021-04-17 18:39:31.000000 Flask-RESTful-DBBase-0.3.5/Flask_RESTful_DBBase.egg-info/SOURCES.txt
--rw-r--r--   0 don       (1000) don       (1000)        1 2021-04-17 18:39:31.000000 Flask-RESTful-DBBase-0.3.5/Flask_RESTful_DBBase.egg-info/dependency_links.txt
--rw-r--r--   0 don       (1000) don       (1000)        1 2020-06-18 21:33:06.000000 Flask-RESTful-DBBase-0.3.5/Flask_RESTful_DBBase.egg-info/not-zip-safe
--rw-r--r--   0 don       (1000) don       (1000)       91 2021-04-17 18:39:31.000000 Flask-RESTful-DBBase-0.3.5/Flask_RESTful_DBBase.egg-info/requires.txt
--rw-r--r--   0 don       (1000) don       (1000)       21 2021-04-17 18:39:31.000000 Flask-RESTful-DBBase-0.3.5/Flask_RESTful_DBBase.egg-info/top_level.txt
--rw-r--r--   0 don       (1000) don       (1000)     2370 2021-04-17 18:39:31.000000 Flask-RESTful-DBBase-0.3.5/PKG-INFO
--rw-r--r--   0 don       (1000) don       (1000)     1246 2020-07-03 17:37:43.000000 Flask-RESTful-DBBase-0.3.5/README.md
-drwxr-xr-x   0 don       (1000) don       (1000)        0 2021-04-17 18:39:31.000000 Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/
--rw-r--r--   0 don       (1000) don       (1000)     1650 2020-07-13 17:44:07.000000 Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/__init__.py
--rw-r--r--   0 don       (1000) don       (1000)       36 2021-04-17 18:26:07.000000 Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/_version.py
--rw-r--r--   0 don       (1000) don       (1000)    10058 2020-08-27 17:50:37.000000 Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/doc_utils.py
--rw-r--r--   0 don       (1000) don       (1000)     2822 2020-07-13 22:36:27.000000 Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/generator.py
-drwxr-xr-x   0 don       (1000) don       (1000)        0 2021-04-17 18:39:31.000000 Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/resources/
--rw-r--r--   0 don       (1000) don       (1000)      270 2020-06-11 23:44:41.000000 Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/resources/__init__.py
--rw-r--r--   0 don       (1000) don       (1000)     4993 2020-10-23 23:26:17.000000 Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/resources/collection_model_resource.py
--rw-r--r--   0 don       (1000) don       (1000)    18102 2020-11-16 02:46:22.000000 Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/resources/dbbase_resource.py
--rw-r--r--   0 don       (1000) don       (1000)     3457 2020-08-13 22:51:27.000000 Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/resources/meta_resource.py
--rw-r--r--   0 don       (1000) don       (1000)    18903 2020-07-13 17:44:07.000000 Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/resources/model_resource.py
--rw-r--r--   0 don       (1000) don       (1000)       38 2021-04-17 18:39:31.000000 Flask-RESTful-DBBase-0.3.5/setup.cfg
--rw-r--r--   0 don       (1000) don       (1000)     2122 2020-07-13 17:44:07.000000 Flask-RESTful-DBBase-0.3.5/setup.py
+drwxr-xr-x   0 don       (1000) don       (1000)        0 2023-05-09 21:07:58.548650 Flask-RESTful-DBBase-0.4.0/
+drwxr-xr-x   0 don       (1000) don       (1000)        0 2023-05-09 21:07:58.545317 Flask-RESTful-DBBase-0.4.0/Flask_RESTful_DBBase.egg-info/
+-rw-r--r--   0 don       (1000) don       (1000)     2346 2023-05-09 21:07:58.000000 Flask-RESTful-DBBase-0.4.0/Flask_RESTful_DBBase.egg-info/PKG-INFO
+-rw-r--r--   0 don       (1000) don       (1000)      931 2023-05-09 21:07:58.000000 Flask-RESTful-DBBase-0.4.0/Flask_RESTful_DBBase.egg-info/SOURCES.txt
+-rw-r--r--   0 don       (1000) don       (1000)        1 2023-05-09 21:07:58.000000 Flask-RESTful-DBBase-0.4.0/Flask_RESTful_DBBase.egg-info/dependency_links.txt
+-rw-r--r--   0 don       (1000) don       (1000)        1 2020-06-18 21:33:06.000000 Flask-RESTful-DBBase-0.4.0/Flask_RESTful_DBBase.egg-info/not-zip-safe
+-rw-r--r--   0 don       (1000) don       (1000)      106 2023-05-09 21:07:58.000000 Flask-RESTful-DBBase-0.4.0/Flask_RESTful_DBBase.egg-info/requires.txt
+-rw-r--r--   0 don       (1000) don       (1000)       21 2023-05-09 21:07:58.000000 Flask-RESTful-DBBase-0.4.0/Flask_RESTful_DBBase.egg-info/top_level.txt
+-rw-r--r--   0 don       (1000) don       (1000)     1067 2020-06-11 23:44:41.000000 Flask-RESTful-DBBase-0.4.0/LICENSE.txt
+-rw-r--r--   0 don       (1000) don       (1000)     2346 2023-05-09 21:07:58.548650 Flask-RESTful-DBBase-0.4.0/PKG-INFO
+-rw-r--r--   0 don       (1000) don       (1000)     1246 2020-07-03 17:37:43.000000 Flask-RESTful-DBBase-0.4.0/README.md
+drwxr-xr-x   0 don       (1000) don       (1000)        0 2023-05-09 21:07:58.545317 Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/
+-rw-r--r--   0 don       (1000) don       (1000)     1650 2020-07-13 17:44:07.000000 Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/__init__.py
+-rw-r--r--   0 don       (1000) don       (1000)       36 2023-05-08 22:55:47.000000 Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/_version.py
+-rw-r--r--   0 don       (1000) don       (1000)    10027 2023-05-09 20:51:48.000000 Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/doc_utils.py
+-rw-r--r--   0 don       (1000) don       (1000)     2852 2021-07-13 21:10:27.000000 Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/generator.py
+drwxr-xr-x   0 don       (1000) don       (1000)        0 2023-05-09 21:07:58.548650 Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/resources/
+-rw-r--r--   0 don       (1000) don       (1000)      270 2020-06-11 23:44:41.000000 Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/resources/__init__.py
+-rw-r--r--   0 don       (1000) don       (1000)    13262 2023-05-09 20:53:34.000000 Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/resources/collection_model_resource.py
+-rw-r--r--   0 don       (1000) don       (1000)    18096 2023-05-09 20:15:04.000000 Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/resources/dbbase_resource.py
+-rw-r--r--   0 don       (1000) don       (1000)     3430 2023-05-09 20:46:42.000000 Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/resources/meta_resource.py
+-rw-r--r--   0 don       (1000) don       (1000)    17725 2023-05-09 20:45:29.000000 Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/resources/model_resource.py
+-rw-r--r--   0 don       (1000) don       (1000)     1118 2023-05-09 20:15:04.000000 Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/validations.py
+-rw-r--r--   0 don       (1000) don       (1000)       84 2023-05-09 21:07:58.548650 Flask-RESTful-DBBase-0.4.0/setup.cfg
+-rw-r--r--   0 don       (1000) don       (1000)     2237 2023-05-08 23:03:52.000000 Flask-RESTful-DBBase-0.4.0/setup.py
+drwxr-xr-x   0 don       (1000) don       (1000)        0 2023-05-09 21:07:58.548650 Flask-RESTful-DBBase-0.4.0/tests/
+-rw-r--r--   0 don       (1000) don       (1000)    30883 2023-05-08 22:54:19.000000 Flask-RESTful-DBBase-0.4.0/tests/test_collection_model_resource.py
+-rw-r--r--   0 don       (1000) don       (1000)    56425 2023-05-08 22:54:19.000000 Flask-RESTful-DBBase-0.4.0/tests/test_dbbase_resource.py
+-rw-r--r--   0 don       (1000) don       (1000)    49492 2023-05-08 22:54:19.000000 Flask-RESTful-DBBase-0.4.0/tests/test_doc_utils.py
+-rw-r--r--   0 don       (1000) don       (1000)     2960 2023-05-08 22:54:19.000000 Flask-RESTful-DBBase-0.4.0/tests/test_generator.py
+-rw-r--r--   0 don       (1000) don       (1000)    34518 2023-05-08 22:54:19.000000 Flask-RESTful-DBBase-0.4.0/tests/test_meta_resource.py
+-rw-r--r--   0 don       (1000) don       (1000)    36680 2023-05-08 22:54:19.000000 Flask-RESTful-DBBase-0.4.0/tests/test_model_modifications.py
+-rw-r--r--   0 don       (1000) don       (1000)    58087 2023-05-08 22:54:19.000000 Flask-RESTful-DBBase-0.4.0/tests/test_model_resource.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Flask-RESTful-DBBase-0.3.5/Flask_RESTful_DBBase.egg-info/PKG-INFO` & `Flask-RESTful-DBBase-0.4.0/Flask_RESTful_DBBase.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: Flask-RESTful-DBBase
-Version: 0.3.5
+Version: 0.4.0
 Summary: A package that extends Flask-RESTful resources to make creating resources for database use easier and faster.
 Home-page: https://sidorof.github.io/flask-restful-dbbase/
 Author: Donald Smiley
 Author-email: dsmiley@sidorof.com
 License: MIT
-Description: ## Introduction
-        
-        This package extends Flask-RESTful by implementing datacentric Web API Resources using [DBBase](https://sidorof.github.io/dbbase/) for enabling the use of SQLAlchemy.
-        
-        DBBase enables the same coding of database models to be used within Flask or without, such as from message queues.
-        
-        Creating a website can result in a fair amount of boilerplate code as the same characteristics for table models are recreated at each layer. Then, the boilerplate code must be tested as well, resulting in boilerplate testcode.
-        
-        Using this package, the database models are introspected and applied to the API, resulting in less code over all.
-        
-        This package should be thought of as a tool rather than a framework. It can coexist with other Flask packages. A framework can get awkward on edge cases as a seemingly straight-forward idea turns out to be very difficult due to trying to fit it into the framework design.
-        
-        Inherent in the design is an understanding that the simplest cases can be done simply, but that there are additional ways to open up the functionality to accommodate more complex issues.
-        
-        And, if the issue encountered does not fit this package's approach, the original resource classes can be used with no loss of functionality.
-        
-Platform: UNKNOWN
 Classifier: Framework :: Flask
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE.txt
+
+## Introduction
+
+This package extends Flask-RESTful by implementing datacentric Web API Resources using [DBBase](https://sidorof.github.io/dbbase/) for enabling the use of SQLAlchemy.
+
+DBBase enables the same coding of database models to be used within Flask or without, such as from message queues.
+
+Creating a website can result in a fair amount of boilerplate code as the same characteristics for table models are recreated at each layer. Then, the boilerplate code must be tested as well, resulting in boilerplate testcode.
+
+Using this package, the database models are introspected and applied to the API, resulting in less code over all.
+
+This package should be thought of as a tool rather than a framework. It can coexist with other Flask packages. A framework can get awkward on edge cases as a seemingly straight-forward idea turns out to be very difficult due to trying to fit it into the framework design.
+
+Inherent in the design is an understanding that the simplest cases can be done simply, but that there are additional ways to open up the functionality to accommodate more complex issues.
+
+And, if the issue encountered does not fit this package's approach, the original resource classes can be used with no loss of functionality.
```

### Comparing `Flask-RESTful-DBBase-0.3.5/Flask_RESTful_DBBase.egg-info/SOURCES.txt` & `Flask-RESTful-DBBase-0.4.0/Flask_RESTful_DBBase.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,27 @@
+LICENSE.txt
 README.md
+setup.cfg
 setup.py
 Flask_RESTful_DBBase.egg-info/PKG-INFO
 Flask_RESTful_DBBase.egg-info/SOURCES.txt
 Flask_RESTful_DBBase.egg-info/dependency_links.txt
 Flask_RESTful_DBBase.egg-info/not-zip-safe
 Flask_RESTful_DBBase.egg-info/requires.txt
 Flask_RESTful_DBBase.egg-info/top_level.txt
 flask_restful_dbbase/__init__.py
 flask_restful_dbbase/_version.py
 flask_restful_dbbase/doc_utils.py
 flask_restful_dbbase/generator.py
+flask_restful_dbbase/validations.py
 flask_restful_dbbase/resources/__init__.py
 flask_restful_dbbase/resources/collection_model_resource.py
 flask_restful_dbbase/resources/dbbase_resource.py
 flask_restful_dbbase/resources/meta_resource.py
-flask_restful_dbbase/resources/model_resource.py
+flask_restful_dbbase/resources/model_resource.py
+tests/test_collection_model_resource.py
+tests/test_dbbase_resource.py
+tests/test_doc_utils.py
+tests/test_generator.py
+tests/test_meta_resource.py
+tests/test_model_modifications.py
+tests/test_model_resource.py
```

### Comparing `Flask-RESTful-DBBase-0.3.5/PKG-INFO` & `Flask-RESTful-DBBase-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: Flask-RESTful-DBBase
-Version: 0.3.5
+Version: 0.4.0
 Summary: A package that extends Flask-RESTful resources to make creating resources for database use easier and faster.
 Home-page: https://sidorof.github.io/flask-restful-dbbase/
 Author: Donald Smiley
 Author-email: dsmiley@sidorof.com
 License: MIT
-Description: ## Introduction
-        
-        This package extends Flask-RESTful by implementing datacentric Web API Resources using [DBBase](https://sidorof.github.io/dbbase/) for enabling the use of SQLAlchemy.
-        
-        DBBase enables the same coding of database models to be used within Flask or without, such as from message queues.
-        
-        Creating a website can result in a fair amount of boilerplate code as the same characteristics for table models are recreated at each layer. Then, the boilerplate code must be tested as well, resulting in boilerplate testcode.
-        
-        Using this package, the database models are introspected and applied to the API, resulting in less code over all.
-        
-        This package should be thought of as a tool rather than a framework. It can coexist with other Flask packages. A framework can get awkward on edge cases as a seemingly straight-forward idea turns out to be very difficult due to trying to fit it into the framework design.
-        
-        Inherent in the design is an understanding that the simplest cases can be done simply, but that there are additional ways to open up the functionality to accommodate more complex issues.
-        
-        And, if the issue encountered does not fit this package's approach, the original resource classes can be used with no loss of functionality.
-        
-Platform: UNKNOWN
 Classifier: Framework :: Flask
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE.txt
+
+## Introduction
+
+This package extends Flask-RESTful by implementing datacentric Web API Resources using [DBBase](https://sidorof.github.io/dbbase/) for enabling the use of SQLAlchemy.
+
+DBBase enables the same coding of database models to be used within Flask or without, such as from message queues.
+
+Creating a website can result in a fair amount of boilerplate code as the same characteristics for table models are recreated at each layer. Then, the boilerplate code must be tested as well, resulting in boilerplate testcode.
+
+Using this package, the database models are introspected and applied to the API, resulting in less code over all.
+
+This package should be thought of as a tool rather than a framework. It can coexist with other Flask packages. A framework can get awkward on edge cases as a seemingly straight-forward idea turns out to be very difficult due to trying to fit it into the framework design.
+
+Inherent in the design is an understanding that the simplest cases can be done simply, but that there are additional ways to open up the functionality to accommodate more complex issues.
+
+And, if the issue encountered does not fit this package's approach, the original resource classes can be used with no loss of functionality.
```

### Comparing `Flask-RESTful-DBBase-0.3.5/README.md` & `Flask-RESTful-DBBase-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/__init__.py` & `Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/doc_utils.py` & `Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/doc_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,18 @@
             documentation.
 
     """
 
     all_methods = ("get", "post", "put", "patch", "delete")
 
     def __init__(
-        self, resource_class, requirements=None, methods=None,
+        self,
+        resource_class,
+        requirements=None,
+        methods=None,
     ):
         self.resource_class = resource_class
         self.model_class = resource_class.model_class._class()
         self.url_prefix = resource_class.url_prefix
         self.base_url = resource_class.create_url()
         if methods:
             if isinstance(methods, dict):
@@ -183,17 +186,17 @@
             ]
         else:
             key = keys[0]
             return {key: db.doc_column(resource_class.model_class, key)}
 
     @staticmethod
     def _get_input_props(resource_class):
-
         return resource_class.model_class.filter_columns(
-            column_props=["!readOnly"], to_camel_case=True,
+            column_props=["!readOnly"],
+            to_camel_case=True,
         )
 
     @staticmethod
     def _get_url(doc, method, resource_class):
         if method in ["get", "put", "patch", "delete"]:
             if resource_class.is_collection():
                 doc["url"] = resource_class.get_urls()[0]
@@ -201,16 +204,14 @@
                 doc["url"] = resource_class.get_urls()[1]
         else:
             doc["url"] = resource_class.get_urls()[0]
 
     def to_dict(self, meta_doc):
         """Convert attributes to a dictionary"""
         resource_class = meta_doc.resource_class
-        model_class = resource_class.model_class
-        db = model_class.db
         doc = {}
         self._get_url(doc, self.method, resource_class)
 
         doc["requirements"] = self.get_method_decorators(meta_doc)
         if meta_doc.resource_class.is_collection():
             doc["queryString"] = self._get_inputs(resource_class)
 
@@ -260,49 +261,49 @@
                     item.__name__ for item in method_decorators[self.method]
                 ]
 
         return None
 
     def get_default_response(self, meta_doc):
         """
-        This function returns the standard response for the method. If something
-        special is done, then the default response would be supressed.
+        This function returns the standard response for the method.
+        If something special is done, then the default response would be
+        supressed.
         """
         resource = meta_doc.resource_class
         method = self.method
         db = resource.model_class.db
 
         outputs = {}
         if method != "delete":
-
             serial_fields = resource._get_serial_fields(
                 method, with_class=True
             )
 
             if isinstance(serial_fields, dict):
                 # foreign class
                 foreign_class, serial_fields = list(serial_fields.items())[0]
                 # NOTE: serial field relations is unresolved
                 doc = db.doc_table(
                     foreign_class,
                     serial_fields=serial_fields,
-                    serial_field_relations=resource._get_serial_field_relations(
-                        method
+                    serial_field_relations=(
+                        resource._get_serial_field_relations(method)
                     ),
                     to_camel_case=True,
                 )[foreign_class._class()]
             else:
                 if serial_fields is None:
                     serial_fields = resource.model_class.get_serial_fields()
 
                 doc = db.doc_table(
                     resource.model_class,
                     serial_fields=serial_fields,
-                    serial_field_relations=resource._get_serial_field_relations(
-                        method
+                    serial_field_relations=(
+                        resource._get_serial_field_relations(method)
                     ),
                     to_camel_case=True,
                 )[resource.model_class._class()]
 
             outputs["fields"] = doc["properties"]
             # NOTE: here is where the default sort would go for collections
```

### Comparing `Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/generator.py` & `Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,14 +75,18 @@
         class_dict["methods"] = set([method.upper() for method in methods])
 
     class_dict.update(params)
 
     if class_vars is not None:
         class_dict.update(class_vars)
 
-    new_class = type(name, (DBBaseResource,), class_dict,)
+    new_class = type(
+        name,
+        (DBBaseResource,),
+        class_dict,
+    )
 
     # required model check
     if new_class.model_class is None:
         raise ValueError("A model class must be defined")
 
     return new_class
```

### Comparing `Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/resources/dbbase_resource.py` & `Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/resources/dbbase_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             raise ValueError(msg)
         self.model_name = self.model_class._class()
 
         super().__init__()
 
     @classmethod
     def get_key_names(cls, formatted=False):
-        """ get_key_names
+        """get_key_names
 
         This function returns column names marked as primary_key.
 
         Args:
             formatted: (bool) : will return in form [<int:id>]
 
         Returns:
@@ -341,15 +341,14 @@
         #     # dict is only used with meta information
         #     serial_field_relations = serial_field_relations.values()[0]
 
         return serial_field_relations
 
     @classmethod
     def _get_serializations(cls, method):
-
         return (
             cls._get_serial_fields(method),
             cls._get_serial_field_relations(method),
         )
 
     @classmethod
     def _check_config_error(cls):
@@ -362,15 +361,15 @@
             return (
                 {"message": "Configuration error: missing model_class."},
                 500,
             )
 
     @classmethod
     def create_url(cls):
-        """ create_url
+        """create_url
 
         Url can come from:
         * url_name resource variable
 
         but if None
         * snake_case version of class name
 
@@ -439,39 +438,39 @@
                     if tmp_errors:
                         errors.extend(tmp_errors)
 
                     if self.use_date_conversions:
                         dtstatus, value = self._check_date_casting(
                             col_key, value, col_params
                         )
+
                         if dtstatus:
                             data[col_key] = value
                         else:
                             errors.extend(value)
                 else:
                     # is it required
                     if col_params.get("nullable") is False:
                         required.append(col_key)
             else:
                 if read_only and col_key in data:
                     del data[col_key]
 
-
         if not skip_missing_data:
             if required:
                 errors.append({"missing_columns": required})
 
         if errors:
             return False, errors
 
         return True, data
 
     @staticmethod
     def _check_numeric_casting(col_key, value, col_params):
-        """ _check_numeric_casting
+        """_check_numeric_casting
 
         This function just makes a quick to see if a numeric field
         data, if in string form, can be converted to a number.
 
         No check is made on integer or float sizes.
         """
         errors = []
@@ -486,15 +485,15 @@
                         {col_key: f"The value {value} is not a number"}
                     )
 
         return errors
 
     @staticmethod
     def _check_max_text_lengths(col_key, value, col_params):
-        """ _check_max_text_lengths
+        """_check_max_text_lengths
 
         This function compares a maximum length, if available with
         the data value.
         """
         errors = []
 
         max_len = col_params.get("maxLength")
@@ -508,15 +507,15 @@
                     }
                 )
 
         return errors
 
     @classmethod
     def _check_date_casting(cls, col_key, value, col_params):
-        """ _check_date_casting
+        """_check_date_casting
 
         This function attempts to change a string date to date object.
 
         Unlike the other checking functions, this function
         does a conversion to an object if possible.
         """
         errors = []
```

### Comparing `Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/resources/meta_resource.py` & `Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/resources/meta_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 a model resource.
 
 Assumes a get method.
 """
 
 from os import path
 from flask import request
-from . import Resource, CollectionModelResource
+from . import Resource
 
 
 class MetaResource(Resource):
-    """ MetaResource
+    """MetaResource
 
     This class enables documentation for a model resource.
 
     **Class variables**:
 
     resource_class: This is the model resource that you wish to documnent.
 
@@ -66,15 +66,15 @@
         except Exception as err:
             msg = err.args[0]
 
             return {"message": msg}, 400
 
     @classmethod
     def get_urls(cls):
-        """ get_urls
+        """get_urls
 
         This function returns a default url for the resource. To keep
         consistency with the get_urls functions in other resources,
         it returns the url in a list, even though there would never be
         more than one.
 
         The approach enables a code consistent approach when using the
```

### Comparing `Flask-RESTful-DBBase-0.3.5/flask_restful_dbbase/resources/model_resource.py` & `Flask-RESTful-DBBase-0.4.0/flask_restful_dbbase/resources/model_resource.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # flask_restful_dbbase/resources/model_resource.py
 """"
 This module implements a starting point for model resources.
 
 """
+import logging
 from flask_restful import request
 from .dbbase_resource import DBBaseResource
-import logging
+from ..validations import validate_process
 
-logger = logging.getLogger(__file__)
+logger = logging.getLogger(__name__)
 
 
 class ModelResource(DBBaseResource):
     """
     ModelResource Class
 
     This model class implements the base class.
@@ -52,58 +53,54 @@
     process_delete_input = None
 
     def get(self, **kwargs):
         """
         This function is the HTTP GET method for a resource handling
         a single item.
         """
-        url = request.path
+        # may be used later
+        # url = request.path
         FUNC_NAME = "get"
 
         # the correct key test - raises error if improper url
         kdict = self._check_key(kwargs)
 
         # for use only with self.process_get_input
-        data = request.args
-
+        data = request.args.to_dict(flat=False)
         query = self.model_class.query
         if self.process_get_input is not None:
-            # 3 ways to end this
-            # success: result is an updated query
-            # failure:
-            #   exit with a tuple that is a
-            #       (JSON message, status_code)
-            #   exit with message, 500 error - failure of func
-            status, result = self.process_get_input(query, data, kwargs)
-            if status is False:
-                if isinstance(result, tuple) and len(result) == 2:
-                    return result
-                else:
-                    func = self.process_get_input.__name__
-                    msg = f"malformed error in {func}: {result}"
-                    return {"message": msg}, 500
+            output = self.process_get_input(query, data, kwargs)
+            validate_process(output, true_keys=["query", "data"])
+
+            if output["status"]:
+                query = output["query"]
+                data = output["data"]
+            else:
+                message = output["message"]
+                status_code = output["status_code"]
+
+                return message, status_code
 
-            query, data = result
         try:
             for key_name, key in kdict.items():
                 query = query.filter(
                     getattr(self.model_class, key_name) == key
                 )
             item = query.first()
         except Exception as err:
             msg = err.args[0]
-            return_msg = f"Internal Server Error: method {FUNC_NAME}: {url}"
-            logger.error(f"{url} method {FUNC_NAME}: {msg}")
-            return {"message": return_msg}, 500
+            logger.error(msg)
+            return {"message": msg}, 500
 
         sfields, sfield_relations = self._get_serializations(FUNC_NAME)
 
         if item:
             result = item.to_dict(
-                serial_fields=sfields, serial_field_relations=sfield_relations,
+                serial_fields=sfields,
+                serial_field_relations=sfield_relations,
             )
 
             logger.debug(result)
 
             return result, 200
 
         msg = f"{self.model_name} with {kdict} not found"
@@ -112,49 +109,56 @@
 
     def post(self):
         """
         This function is the HTTP POST method for a resource handling
         a single item.
         """
         FUNC_NAME = "post"
-        url = request.path
+        # may be used later
+        # url = request.path
         status_code = 201
 
         if request.is_json:
             try:
                 data = request.json
             except Exception as err:
                 msg = err
                 return_msg = f"A JSON format problem:{msg}: {request.data}"
+                logger.error(return_msg)
                 return {"message": return_msg}, 400
 
         else:
+            logger.info("JSON format is required")
             return {"message": "JSON format is required"}, 415
 
         if self.process_post_input is not None:
-            status, result = self.process_post_input(data)
+            output = self.process_post_input(data)
+            validate_process(output, true_keys=["data"])
 
-            if status is False:
-                # exit the scene, result should be a
-                # tuple of message and status
-                if isinstance(result, tuple) and len(result) == 2:
-                    return result
-                else:
-                    func = self.process_post_input.__name__
-                    msg = f"malformed error in {func}: {result}"
-                    return {"message": msg}, 500
+            if output["status"]:
+                data = output["data"]
+            else:
+                message = output["message"]
+                status_code = output["status_code"]
 
-            data = result
+                return message, status_code
 
         obj_params = self.get_obj_params()
-        status, data = self.screen_data(
-            self.model_class.deserialize(data), obj_params
-        )
+
+        try:
+            status, data = self.screen_data(
+                self.model_class.deserialize(data), obj_params
+            )
+        except Exception as err:
+            msg = f"malformed data: {err.args[0]}"
+            logger(msg)
+            return {"message": msg}, 400
 
         if status is False:
+            logger.info(data)
             return {"message": data}, 400
 
         key_names = self.get_key_names(formatted=False)
 
         item = None
 
         status, kdict = self._all_keys_found(key_names, data)
@@ -166,22 +170,22 @@
                 query = query.filter(
                     getattr(self.model_class, key_name) == value
                 )
             try:
                 item = query.first()
             except Exception as err:
                 msg = err.args[0]
-                return_msg = f"Internal Server Error: method {FUNC_NAME}: "
-                f"{url}"
-                logger.error(f"{url} method {FUNC_NAME}: {msg}")
-                return {"message": return_msg}, 500
+                logger.error(msg)
+                return {"message": msg}, 400
 
         if item:
+            msg = f"{kdict} for {self.model_name} already exists."
+            logger.info(msg)
             return (
-                {"message": f"{kdict} for {self.model_name} already exists."},
+                {"message": msg},
                 409,
             )
 
         non_rel_columns = dict(
             [
                 [key, value]
                 for key, value in obj_params.items()
@@ -231,14 +235,16 @@
                     # NOTE: needs further work
                     sub_status, sub_data = self.screen_data(
                         self.model_class.deserialize(subitem),
                         sub_obj_params,
                         skip_missing_data=True,
                     )
                     if sub_status is False:
+                        # NOTE: look at this further
+                        logger.info(sub_data)
                         return {"message": sub_data}, 400
 
                     getattr(item, key).append(sub_class(**sub_data))
 
         adjust_before = self.before_commit.get(FUNC_NAME)
 
         if adjust_before is not None:
@@ -248,20 +254,18 @@
             if status:
                 item = result
             else:
                 return result, status_code
 
         try:
             item.save()
-
         except Exception as err:
             msg = err.args[0]
-            return_msg = f"Internal Server Error: method {FUNC_NAME}: {url}"
-            logger.error(f"{url} method {FUNC_NAME}: {msg}")
-            return {"message": return_msg}, 500
+            logger.error(msg)
+            return {"message": msg}, 400
 
         adjust_after = self.after_commit.get(FUNC_NAME)
         if adjust_after:
             status, result, status_code = self._item_adjust(
                 adjust_after, item, status_code
             )
             if status:
@@ -288,65 +292,66 @@
         FUNC_NAME = "put"
         status_code = 200
 
         try:
             kdict = self._check_key(kwargs)
         except Exception as err:
             msg = err.args[0]
+            logger.info(msg)
             return {"message": msg}, 400
 
         if request.is_json:
             try:
                 data = request.json
             except Exception as err:
                 msg = err
-                return_msg = f"A JSON format problem:{msg}: {request.data}"
+                return_msg = f"A JSON format problem:{msg}"
+                logger.info(return_msg)
                 return {"message": return_msg}, 400
         else:
             return {"message": "JSON format is required"}, 415
 
         query = self.model_class.query
         if self.process_put_input is not None:
-            status, result = self.process_put_input(query, data, kwargs)
+            output = self.process_put_input(query, data, kwargs)
 
-            if status is False:
-                # exit the scene, data should be a
-                # tuple of message and status
-                if isinstance(result, tuple) and len(result) == 2:
-                    return result
-                else:
-                    func = self.process_put_input.__name__
-                    msg = f"malformed error in {func}: {result}"
-                    return {"message": msg}, 500
+            validate_process(output, true_keys=["query", "data"])
 
-            query, data = result
+            if output["status"]:
+                query = output["query"]
+                data = output["data"]
+            else:
+                message = output["message"]
+                status_code = output["status_code"]
 
-        status, kdict = self._all_keys_found(list(kdict.keys()), data)
+                return message, status_code
 
+        status, kdict = self._all_keys_found(list(kdict.keys()), data)
         if status:
             for key_name, value in kdict.items():
                 query = query.filter(
                     getattr(self.model_class, key_name) == value
                 )
         try:
             item = query.first()
+
         except Exception as err:
             msg = err.args[0]
-            return_msg = f"Internal Server Error: method {FUNC_NAME}: {url}"
-            logger.error(f"{url} method {FUNC_NAME}: {msg}")
-            return {"message": return_msg}, 500
+            logger.error(msg)
+            return {"message": msg}, 400
 
         data = self.model_class.deserialize(data)
 
         # use the key(s) from the url
         data.update(kdict)
         status, data = self.screen_data(
             self.model_class.deserialize(data), self.get_obj_params()
         )
         if status is False:
+            logger.info(f"{str(data)}: 400")
             return {"message": data}, 400
 
         if item is None:
             item = self.model_class(**data)
         else:
             for key, value in data.items():
                 setattr(item, key, value)
@@ -363,23 +368,17 @@
 
         try:
             item.save()
 
         except Exception as err:
             self.model_class.db.session.rollback()
             msg = err.args[0]
-            return_msg = f"Internal Server Error: method {FUNC_NAME}: {url}"
+            logger.info(msg)
             logger.error(f"{url} method {FUNC_NAME}: {msg}")
-            return (
-                {
-                    "message": "An error occurred updating the "
-                    f"{self.model_name}: {msg}."
-                },
-                500,
-            )
+            return {"message": msg}, 400
 
         adjust_after = self.after_commit.get(FUNC_NAME)
         if adjust_after:
             status, result, status_code = self._item_adjust(
                 adjust_after, item, status_code
             )
             if status:
@@ -420,38 +419,36 @@
                 return_msg = f"A JSON format problem:{msg}: {request.data}"
                 return {"message": return_msg}, 400
         else:
             return {"message": "JSON format is required"}, 415
 
         query = self.model_class.query
         if self.process_patch_input is not None:
-            status, result = self.process_patch_input(query, data, kwargs)
+            output = self.process_patch_input(query, data, kwargs)
 
-            if status is False:
-                # exit the scene, data should be a
-                # tuple of message and status
-                if isinstance(result, tuple) and len(result) == 2:
-                    return result
-                else:
-                    func = self.process_patch_input.__name__
-                    msg = f"malformed error in {func}: {result}"
-                    return {"message": msg}, 500
+            validate_process(output, true_keys=["query", "data"])
+
+            if output["status"]:
+                query = output["query"]
+                data = output["data"]
+            else:
+                message = output["message"]
+                status_code = output["status_code"]
 
-            query, data = result
+                return message, status_code
 
         for key_name, value in kdict.items():
             query = query.filter(getattr(self.model_class, key_name) == value)
 
         try:
             item = query.first()
         except Exception as err:
             msg = err.args[0]
-            return_msg = f"Internal Server Error: method {FUNC_NAME}: {url}"
-            logger.error(f"{url} method {FUNC_NAME}: {msg}")
-            return {"message": return_msg}, 500
+            logger.error(msg)
+            return {"message": msg}, 500
 
         data = self.model_class.deserialize(data)
 
         data.update(kdict)
         status, data = self.screen_data(
             data, self.get_obj_params(), skip_missing_data=True
         )
@@ -521,40 +518,33 @@
             kdict = self._check_key(kwargs)
         except Exception as err:
             msg = err.args[0]
             return {"message": msg}, 400
 
         query = self.model_class.query
         if self.process_delete_input is not None:
-            status, result = self.process_delete_input(query, kwargs)
+            output = self.process_delete_input(query, kwargs)
+            validate_process(output, true_keys=["query"])
 
-            if status is False:
-                # exit the scene, data should be a
-                # tuple of message and status
-                if isinstance(result, tuple) and len(result) == 2:
-                    return result
-                else:
-                    func = self.process_delete_input.__name__
-                    msg = f"malformed error in {func}: {result}"
-                    return {"message": msg}, 500
+            if output["status"]:
+                query = output["query"]
+            else:
+                message = output["message"]
+                status_code = output["status_code"]
 
-            query = result
+                return {"message": message}, status_code
 
         for key_name, value in kdict.items():
             query = query.filter(getattr(self.model_class, key_name) == value)
         try:
             item = query.first()
         except Exception as err:
             msg = err.args[0]
-            return_msg = (
-                f"Internal Server Error: method {FUNC_NAME}: {url}: {msg}"
-            )
-
-            logger.error(f"{url} method {FUNC_NAME}: {msg}")
-            return {"message": return_msg}, 500
+            logger.error(msg)
+            return {"message": msg}, 500
 
         if item is None:
             msg = f"{self.model_name} with {kdict} not found"
             logger.debug(msg)
             return {"message": msg}, 404
 
         adjust_before = self.before_commit.get(FUNC_NAME)
```

### Comparing `Flask-RESTful-DBBase-0.3.5/setup.py` & `Flask-RESTful-DBBase-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,35 +12,38 @@
 with open("README.md") as fobj:
     LONG_DESCRIPTION = fobj.read()
 
 PROJECT_URL = "https://sidorof.github.io/flask-restful-dbbase/"
 LICENSE = "MIT"
 AUTHOR = "Donald Smiley"
 AUTHOR_EMAIL = "dsmiley@sidorof.com"
-PYTHON_REQUIRES = ">=3.6"
+PYTHON_REQUIRES = ">=3.7"
 ZIP_SAFE = False
 INSTALL_REQUIRES = [
     "flask",
     "Flask-RESTful",
+    "SQLAlchemy < 1.4",
     "Flask-SQLAlchemy",
     "DBBase",
     "python-dateutil",
     "inflect",
 ]
 EXTRAS_REQUIRE = {"dev": ["unittest", "pytest"]}
 
 CLASSIFIERS = [
     "Framework :: Flask",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 __version__ = None
```

