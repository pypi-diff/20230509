# Comparing `tmp/crabpy_pyramid-1.3.0.tar.gz` & `tmp/crabpy_pyramid-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crabpy_pyramid-1.3.0.tar", last modified: Fri May  5 13:21:56 2023, max compression
+gzip compressed data, was "crabpy_pyramid-1.4.0.tar", last modified: Tue May  9 05:35:56 2023, max compression
```

## Comparing `crabpy_pyramid-1.3.0.tar` & `crabpy_pyramid-1.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-05 13:21:56.532286 crabpy_pyramid-1.3.0/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4460 2023-05-05 13:21:30.000000 crabpy_pyramid-1.3.0/CHANGES.rst
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/LICENSE
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/MANIFEST.in
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6490 2023-05-05 13:21:56.532286 crabpy_pyramid-1.3.0/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1326 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/README.rst
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-05 13:21:56.528286 crabpy_pyramid-1.3.0/crabpy_pyramid/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    11605 2023-05-05 13:21:30.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/__init__.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-05 13:21:56.532286 crabpy_pyramid-1.3.0/crabpy_pyramid/renderers/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/renderers/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6711 2023-05-05 13:21:30.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/renderers/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3726 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/renderers/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    15765 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/renderers/crab.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-05 13:21:56.532286 crabpy_pyramid-1.3.0/crabpy_pyramid/routes/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/routes/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3498 2023-05-05 13:21:30.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/routes/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1901 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/routes/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4825 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/routes/crab.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2735 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/utils.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-05 13:21:56.532286 crabpy_pyramid-1.3.0/crabpy_pyramid/views/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/views/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    11435 2023-05-05 13:21:30.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/views/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     5610 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/views/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    13969 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/views/crab.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      599 2023-05-05 13:21:30.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/views/exceptions.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-05 13:21:56.532286 crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6490 2023-05-05 13:21:56.000000 crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      839 2023-05-05 13:21:56.000000 crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/SOURCES.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-05-05 13:21:56.000000 crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/dependency_links.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       47 2023-05-05 13:21:56.000000 crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/entry_points.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 13:30:20.000000 crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/not-zip-safe
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       42 2023-05-05 13:21:56.000000 crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/requires.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       15 2023-05-05 13:21:56.000000 crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/top_level.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      173 2023-05-05 13:21:56.532286 crabpy_pyramid-1.3.0/setup.cfg
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1484 2023-05-05 13:21:30.000000 crabpy_pyramid-1.3.0/setup.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:35:56.965313 crabpy_pyramid-1.4.0/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4606 2023-05-09 05:35:34.000000 crabpy_pyramid-1.4.0/CHANGES.rst
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/LICENSE
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/MANIFEST.in
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6636 2023-05-09 05:35:56.969313 crabpy_pyramid-1.4.0/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1326 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/README.rst
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:35:56.965313 crabpy_pyramid-1.4.0/crabpy_pyramid/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    11605 2023-05-05 13:21:30.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/__init__.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:35:56.965313 crabpy_pyramid-1.4.0/crabpy_pyramid/renderers/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/renderers/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6935 2023-05-09 05:35:34.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/renderers/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3726 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/renderers/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    15765 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/renderers/crab.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:35:56.965313 crabpy_pyramid-1.4.0/crabpy_pyramid/routes/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/routes/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3498 2023-05-05 13:21:30.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/routes/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1901 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/routes/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4825 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/routes/crab.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2735 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/utils.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:35:56.965313 crabpy_pyramid-1.4.0/crabpy_pyramid/views/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/views/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    11433 2023-05-09 05:35:34.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/views/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     5610 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/views/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    13969 2023-04-13 13:30:11.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/views/crab.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      599 2023-05-05 13:21:30.000000 crabpy_pyramid-1.4.0/crabpy_pyramid/views/exceptions.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-09 05:35:56.965313 crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6636 2023-05-09 05:35:56.000000 crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      839 2023-05-09 05:35:56.000000 crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/SOURCES.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-05-09 05:35:56.000000 crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/dependency_links.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       47 2023-05-09 05:35:56.000000 crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/entry_points.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 13:30:20.000000 crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/not-zip-safe
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       42 2023-05-09 05:35:56.000000 crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/requires.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       15 2023-05-09 05:35:56.000000 crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/top_level.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      173 2023-05-09 05:35:56.969313 crabpy_pyramid-1.4.0/setup.cfg
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1484 2023-05-09 05:35:34.000000 crabpy_pyramid-1.4.0/setup.py
```

### Comparing `crabpy_pyramid-1.3.0/CHANGES.rst` & `crabpy_pyramid-1.4.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+1.4.0 (09-05-2023)
+------------------
+
+- Adressenregister fixes (#179)
+- Verschil tss return HttpNotfound en raise HttpNotfound wegwerken (#178)
+
 1.3.0 (05-05-2023)
 ------------------
 
 - Lijst gemeenten statisch maken (#173)
 - Exception handlig aanpassen (#175)
 
 1.2.0 (13-04-2023)
```

### Comparing `crabpy_pyramid-1.3.0/LICENSE` & `crabpy_pyramid-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.3.0/PKG-INFO` & `crabpy_pyramid-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crabpy_pyramid
-Version: 1.3.0
+Version: 1.4.0
 Summary: Bindings for the CRABpy webservices and the Pyramid framework.
 Home-page: http://github.com/OnroerendErfgoed/crabpy_pyramid
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Keywords: web wsgi pyramid CRAB CAPAKEY AGIV
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,20 @@
     # activate your virtual env
     $ pip install sphinx sphinxcontrib-httpdomain
     $ python setup.py develop
     $ cd docs
     $ make html
 
 
+1.4.0 (09-05-2023)
+------------------
+
+- Adressenregister fixes (#179)
+- Verschil tss return HttpNotfound en raise HttpNotfound wegwerken (#178)
+
 1.3.0 (05-05-2023)
 ------------------
 
 - Lijst gemeenten statisch maken (#173)
 - Exception handlig aanpassen (#175)
 
 1.2.0 (13-04-2023)
```

### Comparing `crabpy_pyramid-1.3.0/README.rst` & `crabpy_pyramid-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.3.0/crabpy_pyramid/__init__.py` & `crabpy_pyramid-1.4.0/crabpy_pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.3.0/crabpy_pyramid/renderers/adressenregister.py` & `crabpy_pyramid-1.4.0/crabpy_pyramid/renderers/adressenregister.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,61 +7,73 @@
 
 
 def list_gewesten_adapter(obj, request):
     """
     Adapter for rendering a list of
     :class:`crabpy.gateway.adressenregister.Gewest` to json.
     """
-    return {"id": obj.id, "naam": obj.naam, "niscode": obj.niscode}
+    return {
+        "naam": obj.naam,
+        "niscode": obj.niscode
+    }
 
 
 def list_provincie_adapter(obj, request):
     """
     Adapter for rendering a list of
     :class:`crabpy.gateway.adressenregister.Provincie` to json.
     """
     return {
         "niscode": obj.niscode,
         "naam": obj.naam,
         "gewest": {
-            "id": obj.gewest_niscode,
+            "niscode": obj.gewest_niscode,
         },
     }
 
 
 def list_deelgemeente_adapter(obj, request):
     """
     Adapter for rendering a list of
     :class:`crabpy.gateway.adressenregister.Deelgemeente` to json.
     """
     return {
-        "id": obj.id,
+        "niscode": obj.id,
         "naam": obj.naam,
-        "gemeente_niscode": obj.gemeente_niscode,
+        "gemeente": {
+            "niscode": obj.gemeente_niscode
+        },
     }
 
 
 def list_gemeente_adapter(obj, request):
     """
     Adapter for rendering a list of
     :class:`crabpy.gateway.adressenregister.Gemeenten` to json.
     """
     return {
         "niscode": obj.niscode,
         "naam": obj.naam(),
-        "provincie": {"niscode": obj.provincie_niscode}
+        "provincie": {
+            "niscode": obj.provincie_niscode
+        }
     }
 
 
 def list_straten_adapter(obj, request):
     """
     Adapter for rendering a list of
     :class:`crabpy.gateway.adresregister.Straat` to json.
     """
-    return {"id": obj.id, "naam": obj.naam, "status": obj.status, "uri": obj.uri}
+    return {
+        "id": obj.id,
+        "naam": obj.naam,
+        "status": obj.status,
+        "uri": obj.uri
+    }
 
 
 def list_adressen_adapter(obj, request):
     """
     Adapter for rendering a list of
     :class:`crabpy.gateway.adresregister.Adres` to json.
     """
@@ -76,15 +88,19 @@
 
 
 def list_percelen_adapter(obj, request):
     """
     Adapter for rendering a list of
     :class:`crabpy.gateway.adressenregister.Perceel` to json.
     """
-    return {"id": obj.id, "uri": obj.uri, "status": obj.status}
+    return {
+        "id": obj.id,
+        "uri": obj.uri,
+        "status": obj.status
+    }
 
 
 def list_postinfo_adapter(obj, request):
     """
     Adapter for rendering a list of
     :class:`crabpy.gateway.adressenregister.Postinfo` to json.
     """
@@ -96,15 +112,18 @@
     }
 
 
 def list_landen_adapter(obj, request):
     """
     Adapter for rendering a list of landen to json.
     """
-    return {"id": obj.alpha_2, "naam": _(obj.name)}
+    return {
+        "id": obj.alpha_2,
+        "naam": _(obj.name)
+    }
 
 
 json_list_renderer.add_adapter(adressenregister.Gewest, list_gewesten_adapter)
 json_list_renderer.add_adapter(adressenregister.Provincie, list_provincie_adapter)
 json_list_renderer.add_adapter(adressenregister.Deelgemeente, list_deelgemeente_adapter)
 json_list_renderer.add_adapter(adressenregister.Gemeente, list_gemeente_adapter)
 json_list_renderer.add_adapter(adressenregister.Straat, list_straten_adapter)
@@ -116,15 +135,14 @@
 
 def item_gewest_adapter(obj, request):
     """
     Adapter for rendering an object of
     :class:`crabpy.gateway.adressenregister.Gewest` to json.
     """
     return {
-        "id": obj.id,
         "niscode": obj.niscode,
         "naam": obj.naam,
         "centroid": obj.centroid,
         "bounding_box": obj.bounding_box,
     }
 
 
@@ -157,26 +175,34 @@
 
 def item_deelgemeente_adapter(obj, request):
     """
     Adapter for rendering a object of
     :class:`crabpy.gateway.adressenregister.Deelgemeente` to json.
     """
     return {
-        "id": obj.id,
+        "niscode": obj.id,
         "naam": obj.naam,
-        "gemeente": {"id": obj.gemeente.id, "naam": obj.gemeente.naam},
+        "gemeente": {
+            "niscode": obj.gemeente.niscode,
+            "naam": obj.gemeente.naam()
+        },
     }
 
 
 def item_straat_adapter(obj, request):
     """
     Adapter for rendering an object of
     :class:`crabpy.gateway.adressenregister.Straat` to json.
     """
-    return {"id": obj.id, "naam": obj.naam(), "status": obj.status, "uri": obj.uri}
+    return {
+        "id": obj.id,
+        "naam": obj.naam(),
+        "status": obj.status,
+        "uri": obj.uri
+    }
 
 
 def item_adres_adapter(obj, request):
     """
     Adapter for rendering a list of
     :class:`crabpy.gateway.adresregister.Adres` to json.
     """
```

### Comparing `crabpy_pyramid-1.3.0/crabpy_pyramid/renderers/capakey.py` & `crabpy_pyramid-1.4.0/crabpy_pyramid/renderers/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.3.0/crabpy_pyramid/renderers/crab.py` & `crabpy_pyramid-1.4.0/crabpy_pyramid/renderers/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.3.0/crabpy_pyramid/routes/adressenregister.py` & `crabpy_pyramid-1.4.0/crabpy_pyramid/routes/adressenregister.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.3.0/crabpy_pyramid/routes/capakey.py` & `crabpy_pyramid-1.4.0/crabpy_pyramid/routes/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.3.0/crabpy_pyramid/routes/crab.py` & `crabpy_pyramid-1.4.0/crabpy_pyramid/routes/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.3.0/crabpy_pyramid/utils.py` & `crabpy_pyramid-1.4.0/crabpy_pyramid/utils.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.3.0/crabpy_pyramid/views/adressenregister.py` & `crabpy_pyramid-1.4.0/crabpy_pyramid/views/adressenregister.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     accept="application/json",
 )
 def list_deelgemeenten(request):
     request = set_http_caching(request, "adressenregister", "permanent")
     Gateway = request.adressenregister_gateway()
     gewest_niscode = request.matchdict.get("gewest_niscode")
     if gewest_niscode != "2000":
-        return HTTPNotFound()
+        raise HTTPNotFound()
     deelgemeenten = handle_gateway_response(Gateway.list_deelgemeenten, gewest_niscode)
 
     return range_return(request, deelgemeenten)
 
 
 @view_config(
     route_name="adressenregister_list_deelgemeenten_by_gemeente",
@@ -336,9 +336,9 @@
     accept="application/json",
 )
 def get_land_by_id(request):
     request = set_http_caching(request, "adressenregister", "permanent")
     land_id = request.matchdict.get("land_id")
     land = pycountry.countries.get(alpha_2=land_id)
     if land is None:
-        return HTTPNotFound()
+        raise HTTPNotFound()
     return land
```

### Comparing `crabpy_pyramid-1.3.0/crabpy_pyramid/views/capakey.py` & `crabpy_pyramid-1.4.0/crabpy_pyramid/views/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.3.0/crabpy_pyramid/views/crab.py` & `crabpy_pyramid-1.4.0/crabpy_pyramid/views/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.3.0/crabpy_pyramid/views/exceptions.py` & `crabpy_pyramid-1.4.0/crabpy_pyramid/views/exceptions.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/PKG-INFO` & `crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crabpy-pyramid
-Version: 1.3.0
+Version: 1.4.0
 Summary: Bindings for the CRABpy webservices and the Pyramid framework.
 Home-page: http://github.com/OnroerendErfgoed/crabpy_pyramid
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Keywords: web wsgi pyramid CRAB CAPAKEY AGIV
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,20 @@
     # activate your virtual env
     $ pip install sphinx sphinxcontrib-httpdomain
     $ python setup.py develop
     $ cd docs
     $ make html
 
 
+1.4.0 (09-05-2023)
+------------------
+
+- Adressenregister fixes (#179)
+- Verschil tss return HttpNotfound en raise HttpNotfound wegwerken (#178)
+
 1.3.0 (05-05-2023)
 ------------------
 
 - Lijst gemeenten statisch maken (#173)
 - Exception handlig aanpassen (#175)
 
 1.2.0 (13-04-2023)
```

### Comparing `crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/SOURCES.txt` & `crabpy_pyramid-1.4.0/crabpy_pyramid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.3.0/setup.py` & `crabpy_pyramid-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'coverage',
     'webtest'
 ]
 
 testing_extras = tests_requires + []
 
 setup(name='crabpy_pyramid',
-      version='1.3.0',
+      version='1.4.0',
       description='Bindings for the CRABpy webservices and the Pyramid framework.',
       long_description=README + '\n\n' + CHANGES,
       classifiers=[
         'Development Status :: 5 - Production/Stable',
         "Programming Language :: Python",
         'Programming Language :: Python :: 3.8',
         "Framework :: Pyramid",
```

