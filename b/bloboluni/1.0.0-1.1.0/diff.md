# Comparing `tmp/bloboluni-1.0.0.tar.gz` & `tmp/bloboluni-1.1.0.tar.gz`

## Comparing `bloboluni-1.0.0.tar` & `bloboluni-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bloboluni-1.0.0/GitVersion.yml
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 bloboluni-1.0.0/test.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 bloboluni-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloboluni-1.0.0/bloboluni/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 bloboluni-1.0.0/bloboluni/serializers.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 bloboluni-1.0.0/bloboluni/storage.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 bloboluni-1.0.0/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 bloboluni-1.0.0/LICENSE
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bloboluni-1.0.0/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bloboluni-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 bloboluni-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bloboluni-1.1.0/GitVersion.yml
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 bloboluni-1.1.0/test.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 bloboluni-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloboluni-1.1.0/bloboluni/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 bloboluni-1.1.0/bloboluni/serializers.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 bloboluni-1.1.0/bloboluni/storage.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 bloboluni-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 bloboluni-1.1.0/LICENSE
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 bloboluni-1.1.0/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bloboluni-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 bloboluni-1.1.0/PKG-INFO
```

### Comparing `bloboluni-1.0.0/.github/workflows/python-publish.yml` & `bloboluni-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bloboluni-1.0.0/bloboluni/serializers.py` & `bloboluni-1.1.0/bloboluni/serializers.py`

 * *Files identical despite different names*

### Comparing `bloboluni-1.0.0/bloboluni/storage.py` & `bloboluni-1.1.0/bloboluni/storage.py`

 * *Files identical despite different names*

### Comparing `bloboluni-1.0.0/.gitignore` & `bloboluni-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bloboluni-1.0.0/LICENSE` & `bloboluni-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bloboluni-1.0.0/pyproject.toml` & `bloboluni-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bloboluni"
-version = "1.0.0"
+version = "1.1.0"
 description = "A simple package for storing and retrieving blobs of data from Azure Blob Storage"
 authors = [
   { name = "Martin Moan", email = "martin.moan1@gmail.com" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
```

### Comparing `bloboluni-1.0.0/PKG-INFO` & `bloboluni-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bloboluni
-Version: 1.0.0
+Version: 1.1.0
 Summary: A simple package for storing and retrieving blobs of data from Azure Blob Storage
 Project-URL: Homepage, https://github.com/MartinMoan/blobstorage
 Project-URL: Bug Tracker, https://github.com/MartinMoan/blobstorage/issues
 Author-email: Martin Moan <martin.moan1@gmail.com>
 License: Copyright (c) 2023 Martin Hoff Moan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,19 +31,41 @@
 Requires-Python: >=3.7
 Requires-Dist: azure-identity>=1
 Requires-Dist: azure-storage-blob>=1
 Requires-Dist: python-dotenv>=1
 Requires-Dist: requests>2
 Description-Content-Type: text/markdown
 
-# BlobStorage
-A simple python package for storing and retrieving blobs of data from Azure Blob Storage.
+# bloboluni: Azure blob storage wrapper
+`bloboluni` is a simple python module for interacting with Azure blob storage.
 
-Installation:
+## Installation
 ````
 pip install bloboluni
 ````
 
-Usage
+## Usage
+````python
+from bloboluni.storage import JsonPickleBlobStorage
+from mymodels import Person, Profession
+
+if __name__ == "__main__":
+    alex = Person("Alex", 27, Profession("Developer", "A developer"))
+
+    # Create a storage client
+    storage = JsonPickleBlobStorage(connectionstring="...", container="mycontainer")
+
+    # Store some data
+    storage.upsert(key="Alex", alex)
+
+    # Read some data
+    sam = storage.get(key="Sam") # Returns instance of Person or None
+
+    # Delete some data
+    storage.delete(key="Sam")
 ````
-test
-````
+
+`bloboluni` provides storage clients using several different serialization implementations. 
+Currently, these are:
+- `BlobStorage`
+- `JsonBlobStorage` 
+- `JsonPickleBlobStorage`
```

