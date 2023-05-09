# Comparing `tmp/aphos_openapi-2.4.0.tar.gz` & `tmp/aphos_openapi-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aphos_openapi-2.4.0.tar", last modified: Fri Apr 28 23:12:07 2023, max compression
+gzip compressed data, was "aphos_openapi-2.5.0.tar", last modified: Tue May  9 13:48:33 2023, max compression
```

## Comparing `aphos_openapi-2.4.0.tar` & `aphos_openapi-2.5.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:12:07.576025 aphos_openapi-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15593 2023-04-28 23:12:07.576025 aphos_openapi-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:12:07.572024 aphos_openapi-2.4.0/aphos_openapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/aphos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:12:07.572024 aphos_openapi-2.4.0/aphos_openapi/api/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/api/catalog_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/api/flux_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25235 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/api/space_object_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39091 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:12:07.576025 aphos_openapi-2.4.0/aphos_openapi/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:12:07.576025 aphos_openapi-2.4.0/aphos_openapi/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/comparison_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/flux.py
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/flux_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/night.py
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/photo_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/space_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/space_object_with_fluxes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    82630 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:12:07.576025 aphos_openapi-2.4.0/aphos_openapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/models/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    14718 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/models/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/aphos_openapi/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:12:07.572024 aphos_openapi-2.4.0/aphos_openapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15593 2023-04-28 23:12:07.000000 aphos_openapi-2.4.0/aphos_openapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-28 23:12:07.000000 aphos_openapi-2.4.0/aphos_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:12:07.000000 aphos_openapi-2.4.0/aphos_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 23:12:07.000000 aphos_openapi-2.4.0/aphos_openapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 23:12:07.000000 aphos_openapi-2.4.0/aphos_openapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:12:07.576025 aphos_openapi-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-28 23:11:53.000000 aphos_openapi-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:48:33.157122 aphos_openapi-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-05-09 13:48:33.157122 aphos_openapi-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:48:33.153122 aphos_openapi-2.5.0/aphos_openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/aphos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:48:33.153122 aphos_openapi-2.5.0/aphos_openapi/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/api/catalog_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/api/flux_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25235 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/api/space_object_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39091 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:48:33.153122 aphos_openapi-2.5.0/aphos_openapi/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:48:33.157122 aphos_openapi-2.5.0/aphos_openapi/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/comparison_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/flux_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/night.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/photo_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/space_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/space_object_with_fluxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82630 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:48:33.157122 aphos_openapi-2.5.0/aphos_openapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/models/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/models/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:48:33.153122 aphos_openapi-2.5.0/aphos_openapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-05-09 13:48:33.000000 aphos_openapi-2.5.0/aphos_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-09 13:48:33.000000 aphos_openapi-2.5.0/aphos_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:48:33.000000 aphos_openapi-2.5.0/aphos_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-09 13:48:33.000000 aphos_openapi-2.5.0/aphos_openapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 13:48:33.000000 aphos_openapi-2.5.0/aphos_openapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:48:33.157122 aphos_openapi-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/setup.py
```

### Comparing `aphos_openapi-2.4.0/LICENSE` & `aphos_openapi-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/PKG-INFO` & `aphos_openapi-2.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: aphos_openapi
-Version: 2.4.0
+Version: 2.5.0
 Summary: APhoS Python library for data representation
 Author: Pavel Kinc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # APhoS client for retrieving data in Python
 
 This is Amateur Photometric Survey (APhoS) client for web application.  
 Contains documentation about modules, models and functions for working with astronomical data from APhoS database.  
-Server is accessible from: https://ip-147-251-21-104.flt.cloud.muni.cz/  
-Swagger UI (Interface for api of the server): https://ip-147-251-21-104.flt.cloud.muni.cz/swagger-ui/index.html  
-Openapi json or yaml file (documentation of api): https://ip-147-251-21-104.flt.cloud.muni.cz/api-docs
+Server is accessible from: https://aphos.cerit-sc.cz/  
+Swagger UI (Interface for api of the server): https://aphos.cerit-sc.cz/swagger-ui/index.html
+Openapi json or yaml file (documentation of api): https://aphos.cerit-sc.cz/openapi
 
 ## Installation
-### Package: `aphos_openapi`
+### Package: `aphos-openapi`
 
 Install: `pip install aphos-openapi`  
-Upgrade: `pip install aphos_openapi --upgrade`
+Upgrade: `pip install aphos-openapi --upgrade`
+
 (If you have pip3 instead of pip, just use pip3)
 
 ## Contents
 References work only in github: https://github.com/pavel-kinc/aphos-client/blob/main/README.md
 * [Basic info](README.md#aphos-client-for-retrieving-data-in-python)
 * [Installation](README.md#installation)
 * [Requirements](README.md#requirements)
@@ -210,15 +211,17 @@
 Resolve name based on astropy name resolver and tries to find equal potential objects in APhoS database (Cross-identification).  
 Returns: List of space objects which are potentially equal to given name, from all catalogs.  
 Params:  
 &emsp;name - any name by which a space object can be resolved
 <br/><br/>
 
 #### upload_files(<br/>path: str) <br/>-> list[tuple[str, bool, str]]
-Upload files as Anounymous user. Files are in format csv, with delimiter ';', generated from SIPS software. For authenticated upload use website -> info().  
+!!! HIDDEN FOR NOW !!!
+
+Upload files as Anonymous user. Files are in format csv, with delimiter ';', generated from SIPS software. For authenticated upload use website -> info().  
 Returns: List of tuple (file, success of upload of the given file, info about upload).  
 Params:  
 &emsp;path - path to file or directory with files
 <br/><br/>
 
 #### info() -> None
 Prints useful documentation and info about this package.
```

### Comparing `aphos_openapi-2.4.0/README.md` & `aphos_openapi-2.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # APhoS client for retrieving data in Python
 
 This is Amateur Photometric Survey (APhoS) client for web application.  
 Contains documentation about modules, models and functions for working with astronomical data from APhoS database.  
-Server is accessible from: https://ip-147-251-21-104.flt.cloud.muni.cz/  
-Swagger UI (Interface for api of the server): https://ip-147-251-21-104.flt.cloud.muni.cz/swagger-ui/index.html  
-Openapi json or yaml file (documentation of api): https://ip-147-251-21-104.flt.cloud.muni.cz/api-docs
+Server is accessible from: https://aphos.cerit-sc.cz/  
+Swagger UI (Interface for api of the server): https://aphos.cerit-sc.cz/swagger-ui/index.html
+Openapi json or yaml file (documentation of api): https://aphos.cerit-sc.cz/openapi
 
 ## Installation
-### Package: `aphos_openapi`
+### Package: `aphos-openapi`
 
 Install: `pip install aphos-openapi`  
-Upgrade: `pip install aphos_openapi --upgrade`
+Upgrade: `pip install aphos-openapi --upgrade`
+
 (If you have pip3 instead of pip, just use pip3)
 
 ## Contents
 References work only in github: https://github.com/pavel-kinc/aphos-client/blob/main/README.md
 * [Basic info](README.md#aphos-client-for-retrieving-data-in-python)
 * [Installation](README.md#installation)
 * [Requirements](README.md#requirements)
@@ -198,15 +199,17 @@
 Resolve name based on astropy name resolver and tries to find equal potential objects in APhoS database (Cross-identification).  
 Returns: List of space objects which are potentially equal to given name, from all catalogs.  
 Params:  
 &emsp;name - any name by which a space object can be resolved
 <br/><br/>
 
 #### upload_files(<br/>path: str) <br/>-> list[tuple[str, bool, str]]
-Upload files as Anounymous user. Files are in format csv, with delimiter ';', generated from SIPS software. For authenticated upload use website -> info().  
+!!! HIDDEN FOR NOW !!!
+
+Upload files as Anonymous user. Files are in format csv, with delimiter ';', generated from SIPS software. For authenticated upload use website -> info().  
 Returns: List of tuple (file, success of upload of the given file, info about upload).  
 Params:  
 &emsp;path - path to file or directory with files
 <br/><br/>
 
 #### info() -> None
 Prints useful documentation and info about this package.
```

### Comparing `aphos_openapi-2.4.0/aphos_openapi/__init__.py` & `aphos_openapi-2.5.0/aphos_openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/aphos.py` & `aphos_openapi-2.5.0/aphos_openapi/aphos.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ALL_CATALOGS = "All catalogues"
 
 _DEV_CONSTANT = 2.5/aphos_openapi.math.log(10)
 
 _READ_ME = "https://test.pypi.org/project/aphos-openapi/"
 
-_WEBSITE = "https://ip-147-251-21-104.flt.cloud.muni.cz/"
+_WEBSITE = "https://aphos.cerit-sc.cz/"
 
 
 def get_catalogs() -> _Optional[_List[str]]:
     """
     Get all available catalogs from APhoS.
 
     Returns: List of available catalogs (strings).
```

### Comparing `aphos_openapi-2.4.0/aphos_openapi/api/catalog_api.py` & `aphos_openapi-2.5.0/aphos_openapi/api/catalog_api.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/api/flux_api.py` & `aphos_openapi-2.5.0/aphos_openapi/api/flux_api.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/api/space_object_api.py` & `aphos_openapi-2.5.0/aphos_openapi/api/space_object_api.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/api/user_api.py` & `aphos_openapi-2.5.0/aphos_openapi/api/user_api.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/api_client.py` & `aphos_openapi-2.5.0/aphos_openapi/api_client.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/apis/__init__.py` & `aphos_openapi-2.5.0/aphos_openapi/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/configuration.py` & `aphos_openapi-2.5.0/aphos_openapi/configuration.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -388,22 +388,22 @@
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                'url': "https://ip-147-251-21-104.flt.cloud.muni.cz",
-                'description': "Test server (virtual machine) - CURRENT",
-            },
-            {
                 'url': "https://aphos.cerit-sc.cz",
                 'description': "Main server APhoS",
             },
             {
+                'url': "https://ip-147-251-21-104.flt.cloud.muni.cz",
+                'description': "Test server (virtual machine) - CURRENT",
+            },
+            {
                 'url': "http://localhost:8009",
                 'description': "Developer server",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
```

### Comparing `aphos_openapi-2.4.0/aphos_openapi/exceptions.py` & `aphos_openapi-2.5.0/aphos_openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/model/comparison_object.py` & `aphos_openapi-2.5.0/aphos_openapi/model/comparison_object.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/model/error_message.py` & `aphos_openapi-2.5.0/aphos_openapi/model/error_message.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/model/flux.py` & `aphos_openapi-2.5.0/aphos_openapi/model/flux.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/model/flux_data.py` & `aphos_openapi-2.5.0/aphos_openapi/model/flux_data.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/model/night.py` & `aphos_openapi-2.5.0/aphos_openapi/model/night.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/model/photo_properties.py` & `aphos_openapi-2.5.0/aphos_openapi/model/photo_properties.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/model/space_object.py` & `aphos_openapi-2.5.0/aphos_openapi/model/space_object.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/model/space_object_with_fluxes.py` & `aphos_openapi-2.5.0/aphos_openapi/model/space_object_with_fluxes.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/model/user.py` & `aphos_openapi-2.5.0/aphos_openapi/model/user.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/model_utils.py` & `aphos_openapi-2.5.0/aphos_openapi/model_utils.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/models/__init__.py` & `aphos_openapi-2.5.0/aphos_openapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/models/coordinates.py` & `aphos_openapi-2.5.0/aphos_openapi/models/coordinates.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi/models/graph_data.py` & `aphos_openapi-2.5.0/aphos_openapi/models/graph_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,33 +85,33 @@
     def graph(self) -> Any:
         """
         Graph representation of GraphData object (Light curve in time).
         This representation uses matplotlib to create a graph.
 
         x-axis: Julian date (normal format)
 
-        y-axis: Magnitude
+        y-axis: Brightness [mag]
 
         Graph has also togglable error bars (deviations) and user filtering based on legend.
         """
-        self._create_graph()
+        _, box = self._create_graph()
         _plt.show()
 
-    def _create_graph(self) -> List[Any]:
+    def _create_graph(self, ylabel: str = "Brightness [mag]") -> Tuple[List[Any], Optional[CheckButtons]]:
         """
         Create pyplot graph from data.
         Returns: Figure of given graph
 
         """
         d: Dict[str, List[Tuple[float, float, float]]] = dict()
         fig, ax = _plt.subplots(figsize=(11, 7))
         fig.subplots_adjust(right=0.8, bottom=0.15)
         _plt.title(f"Light curve of {self._info_str()}")
         _plt.xlabel("Julian Date (JD)")
-        _plt.ylabel("Magnitude")
+        _plt.ylabel(ylabel)
         for a, b, c, u in self.data_list:
             key = u[0:15]
             d.setdefault(key, []).append((a, b, c))
         errs = []
         plts = []
         for key, val in d.items():
             a, b, c = zip(*val)
@@ -125,48 +125,48 @@
         if len(errs) > 10:
             scroll(fig, legend)
         toggle_legend(legend, plts, errs)
 
         ax.invert_yaxis()
         ax.ticklabel_format(useOffset=False, style='plain')
         _plt.setp(ax.get_xticklabels(), rotation=10, horizontalalignment='right')
-        return plts
+        return plts, box
 
     def composite_graph(self) -> None:
         """
         Composite (compressed) graph representation of light curve in time.
 
         Similar to graph() but biggest "jump" between two measurements is defined by
         constant (currently 0.06 JD -> ~1.5 hour).
 
         User can see light curve of multiple measurements without too much of zooming,
         date is compromised, but relative time between values in 1 measurement is same.
 
         Every measurement is seperated by 2 lines, distance is given by the given constant.
         """
 
-        self._create_composite_graph()
+        box = self._create_composite_graph()
         _plt.show()
 
-    def _create_composite_graph(self) -> None:
+    def _create_composite_graph(self) -> Optional[CheckButtons]:
         """
         Create compressed graph.
 
         Returns: None
 
         """
         fig, ax = _plt.subplots(figsize=(11, 7))
         _plt.title(f"Composed night light curve of {self._info_str()}")
         _plt.xlabel("Days")
-        _plt.ylabel("Magnitude")
+        _plt.ylabel("Brightness [mag]")
         fig.subplots_adjust(right=0.8)
         errs = []
         my_list = sorted(self.data_list, key=lambda x: x.date)
         if len(my_list) == 0:
-            return
+            return None
         # start from 0
         curr_min: float = 0
         # start from 1. measurement and keep with real
         curr = my_list[0].date
         a = []
         b = []
         c = []
@@ -184,53 +184,55 @@
             b.append(y)
             c.append(z)
 
         plt, = ax.plot(a, b, "o")
         errs.append(ax.errorbar(a, b, yerr=c, fmt=" ", color="#1f77b4", visible=False))
         box = deviations(_plt, errs, [plt], None)
         ax.invert_yaxis()
+        return box
 
     def phase_graph(self, moment: float, period: float) -> None:
         """
         Phase graph representation.
 
         Creates phase curve for given data.
 
         Args:
             moment: start of epoch, julian date
             period: time period in days
         """
-        self._create_phase_graph(moment, period)
+        box = self._create_phase_graph(moment, period)
         _plt.show()
 
-    def _create_phase_graph(self, moment: float, period: float) -> None:
+    def _create_phase_graph(self, moment: float, period: float) -> Optional[CheckButtons]:
         """
         Creates phase graph.
 
         Args:
             moment: start of epoch, julian date
             period: time period in days
         """
         fig, ax = _plt.subplots(figsize=(11, 7))
         _plt.title(f"Phase graph of {self._info_str()}")
         _plt.xlabel("Phase")
-        _plt.ylabel("Magnitude")
+        _plt.ylabel("Brightness [mag]")
         fig.subplots_adjust(right=0.8)
         a = []
         b = []
         c = []
         errs = []
         for x, y, z, _ in self.data_list:
             a.append(((x - moment) / period) % 1)
             b.append(y)
             c.append(z)
         plt, = ax.plot(a, b, "o")
         errs.append(ax.errorbar(a, b, yerr=c, fmt=" ", color="#1f77b4", visible=False))
         box = deviations(_plt, errs, [plt], None)
         ax.invert_yaxis()
+        return box
 
 
 class DMDU:
     """
     Class for representation of astronomical data.
 
     Attributes:
@@ -325,15 +327,14 @@
                         continue
                 elif not exclude:
                     continue
             res.append(DMDU(float(row[0]), float(row[1]), float(row[2]), row[3]))
     return info, res
 
 
-
 """
 Graph handling and event handlers for matplotlib graph helper functions.
 """
 
 
 def deviations(plot: _matplotlib.pyplot, errors: List[Any],
                plts: List[_matplotlib.lines.Line2D],
```

### Comparing `aphos_openapi-2.4.0/aphos_openapi/rest.py` & `aphos_openapi-2.5.0/aphos_openapi/rest.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/aphos_openapi.egg-info/PKG-INFO` & `aphos_openapi-2.5.0/aphos_openapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: aphos-openapi
-Version: 2.4.0
+Version: 2.5.0
 Summary: APhoS Python library for data representation
 Author: Pavel Kinc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # APhoS client for retrieving data in Python
 
 This is Amateur Photometric Survey (APhoS) client for web application.  
 Contains documentation about modules, models and functions for working with astronomical data from APhoS database.  
-Server is accessible from: https://ip-147-251-21-104.flt.cloud.muni.cz/  
-Swagger UI (Interface for api of the server): https://ip-147-251-21-104.flt.cloud.muni.cz/swagger-ui/index.html  
-Openapi json or yaml file (documentation of api): https://ip-147-251-21-104.flt.cloud.muni.cz/api-docs
+Server is accessible from: https://aphos.cerit-sc.cz/  
+Swagger UI (Interface for api of the server): https://aphos.cerit-sc.cz/swagger-ui/index.html
+Openapi json or yaml file (documentation of api): https://aphos.cerit-sc.cz/openapi
 
 ## Installation
-### Package: `aphos_openapi`
+### Package: `aphos-openapi`
 
 Install: `pip install aphos-openapi`  
-Upgrade: `pip install aphos_openapi --upgrade`
+Upgrade: `pip install aphos-openapi --upgrade`
+
 (If you have pip3 instead of pip, just use pip3)
 
 ## Contents
 References work only in github: https://github.com/pavel-kinc/aphos-client/blob/main/README.md
 * [Basic info](README.md#aphos-client-for-retrieving-data-in-python)
 * [Installation](README.md#installation)
 * [Requirements](README.md#requirements)
@@ -210,15 +211,17 @@
 Resolve name based on astropy name resolver and tries to find equal potential objects in APhoS database (Cross-identification).  
 Returns: List of space objects which are potentially equal to given name, from all catalogs.  
 Params:  
 &emsp;name - any name by which a space object can be resolved
 <br/><br/>
 
 #### upload_files(<br/>path: str) <br/>-> list[tuple[str, bool, str]]
-Upload files as Anounymous user. Files are in format csv, with delimiter ';', generated from SIPS software. For authenticated upload use website -> info().  
+!!! HIDDEN FOR NOW !!!
+
+Upload files as Anonymous user. Files are in format csv, with delimiter ';', generated from SIPS software. For authenticated upload use website -> info().  
 Returns: List of tuple (file, success of upload of the given file, info about upload).  
 Params:  
 &emsp;path - path to file or directory with files
 <br/><br/>
 
 #### info() -> None
 Prints useful documentation and info about this package.
```

### Comparing `aphos_openapi-2.4.0/aphos_openapi.egg-info/SOURCES.txt` & `aphos_openapi-2.5.0/aphos_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.4.0/setup.py` & `aphos_openapi-2.5.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aphos_openapi",
-    version="2.4.0",
+    version="2.5.0",
     author="Pavel Kinc",
     description="APhoS Python library for data representation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
     license_files=('LICENSE',),
     classifiers=[
@@ -18,10 +18,10 @@
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
     install_requires=[
         'urllib3>=1.25.3,<2.0',
         'python-dateutil',
         'matplotlib',
-        'astropy'
+        'astropy<=5.2.2'
     ]
 )
```

