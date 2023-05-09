# Comparing `tmp/aiosolr-4.2.7.tar.gz` & `tmp/aiosolr-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosolr-4.2.7.tar", last modified: Wed Feb  1 21:17:35 2023, max compression
+gzip compressed data, was "aiosolr-4.3.0.tar", last modified: Tue May  9 17:49:16 2023, max compression
```

## Comparing `aiosolr-4.2.7.tar` & `aiosolr-4.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 brad.belyeu   (501) staff       (20)        0 2023-02-01 21:17:35.514402 aiosolr-4.2.7/
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     5027 2023-02-01 21:17:35.514581 aiosolr-4.2.7/PKG-INFO
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     3456 2022-02-08 22:46:58.000000 aiosolr-4.2.7/README.md
-drwxrwxrwx   0 brad.belyeu   (501) staff       (20)        0 2023-02-01 21:17:35.514135 aiosolr-4.2.7/aiosolr.egg-info/
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     5027 2023-02-01 21:17:35.000000 aiosolr-4.2.7/aiosolr.egg-info/PKG-INFO
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)      208 2023-02-01 21:17:35.000000 aiosolr-4.2.7/aiosolr.egg-info/SOURCES.txt
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)        1 2023-02-01 21:17:35.000000 aiosolr-4.2.7/aiosolr.egg-info/dependency_links.txt
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)       15 2023-02-01 21:17:35.000000 aiosolr-4.2.7/aiosolr.egg-info/requires.txt
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)        8 2023-02-01 21:17:35.000000 aiosolr-4.2.7/aiosolr.egg-info/top_level.txt
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)    21514 2023-02-01 21:15:45.000000 aiosolr-4.2.7/aiosolr.py
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)      537 2021-06-10 19:49:07.000000 aiosolr-4.2.7/pyproject.toml
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)      282 2023-02-01 21:17:35.515158 aiosolr-4.2.7/setup.cfg
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     1138 2023-02-01 21:15:03.000000 aiosolr-4.2.7/setup.py
+drwxrwxrwx   0 brad.belyeu   (501) staff       (20)        0 2023-05-09 17:49:16.265564 aiosolr-4.3.0/
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     5027 2023-05-09 17:49:16.265856 aiosolr-4.3.0/PKG-INFO
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     3456 2022-02-08 22:46:58.000000 aiosolr-4.3.0/README.md
+drwxrwxrwx   0 brad.belyeu   (501) staff       (20)        0 2023-05-09 17:49:16.265154 aiosolr-4.3.0/aiosolr.egg-info/
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     5027 2023-05-09 17:49:16.000000 aiosolr-4.3.0/aiosolr.egg-info/PKG-INFO
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)      208 2023-05-09 17:49:16.000000 aiosolr-4.3.0/aiosolr.egg-info/SOURCES.txt
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)        1 2023-05-09 17:49:16.000000 aiosolr-4.3.0/aiosolr.egg-info/dependency_links.txt
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)       15 2023-05-09 17:49:16.000000 aiosolr-4.3.0/aiosolr.egg-info/requires.txt
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)        8 2023-05-09 17:49:16.000000 aiosolr-4.3.0/aiosolr.egg-info/top_level.txt
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)    21590 2023-05-09 17:46:29.000000 aiosolr-4.3.0/aiosolr.py
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)      537 2021-06-10 19:49:07.000000 aiosolr-4.3.0/pyproject.toml
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)      282 2023-05-09 17:49:16.266764 aiosolr-4.3.0/setup.cfg
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     1138 2023-05-09 17:46:29.000000 aiosolr-4.3.0/setup.py
```

### Comparing `aiosolr-4.2.7/PKG-INFO` & `aiosolr-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: aiosolr
-Version: 4.2.7
+Version: 4.3.0
 Summary: Lightweight Python client for Apache Solr.
 Home-page: https://github.com/bbelyeu/aiosolr/
 Author: Brad Belyeu
 Author-email: bradley.belyeu@life.church
 License: MIT
-Download-URL: https://github.com/bbelyeu/aiosolr/archive/4.2.7.zip
+Download-URL: https://github.com/bbelyeu/aiosolr/archive/4.3.0.zip
 Description: # aiosolr
         
         AsyncIO Python client for Apache Solr
         
         ## Requirements
         
         This project requires Python 3.6+
```

### Comparing `aiosolr-4.2.7/README.md` & `aiosolr-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aiosolr-4.2.7/aiosolr.egg-info/PKG-INFO` & `aiosolr-4.3.0/aiosolr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: aiosolr
-Version: 4.2.7
+Version: 4.3.0
 Summary: Lightweight Python client for Apache Solr.
 Home-page: https://github.com/bbelyeu/aiosolr/
 Author: Brad Belyeu
 Author-email: bradley.belyeu@life.church
 License: MIT
-Download-URL: https://github.com/bbelyeu/aiosolr/archive/4.2.7.zip
+Download-URL: https://github.com/bbelyeu/aiosolr/archive/4.3.0.zip
 Description: # aiosolr
         
         AsyncIO Python client for Apache Solr
         
         ## Requirements
         
         This project requires Python 3.6+
```

### Comparing `aiosolr-4.2.7/aiosolr.py` & `aiosolr-4.3.0/aiosolr.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,23 +33,25 @@
 class Response:
     """Response class."""
 
     def __init__(self, data, status):
         self.data = data
         self.doc = {}
         self.docs = []
+        self.grouped = []
         self.more_like_this = []
         self.status = status
         self.spelling_suggestions = []
 
         if isinstance(data, dict):
             self.doc = data.get("doc", {})
             response = data.get("response", {})
             if response:
                 self.docs = response.get("docs", [])
+            self.grouped = data.get("grouped", {})
             mlt_data = data.get("moreLikeThis", {})
 
             if mlt_data:
                 mlt_data_key = list(mlt_data.keys())[0]
                 self.more_like_this = mlt_data[mlt_data_key].get("docs", [])
 
             spellcheck = data.get("spellcheck", {})
@@ -457,15 +459,14 @@
         suggestions = []
 
         if query:
             if "+" in query:
                 query = query.replace("+", " ")
 
             for name in response.data["suggest"].keys():
-
                 try:
                     suggestions += [
                         {"match": s["term"], "payload": s["payload"]}
                         for s in response.data["suggest"][name][query]["suggestions"]
                     ]
                 except KeyError:
                     pass
```

### Comparing `aiosolr-4.2.7/pyproject.toml` & `aiosolr-4.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiosolr-4.2.7/setup.py` & `aiosolr-4.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 
 from setuptools import setup
 
 if sys.version_info < (3, 7):
     sys.exit("Sorry, Python < 3.7 is not supported")
 
-__version__ = "4.2.7"
+__version__ = "4.3.0"
 
 setup(
     name="aiosolr",
     version=__version__,
     description=__doc__,
     author="Brad Belyeu",
     author_email="bradley.belyeu@life.church",
```

