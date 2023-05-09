# Comparing `tmp/bloboluni-0.2.2.tar.gz` & `tmp/bloboluni-1.0.0.tar.gz`

## Comparing `bloboluni-0.2.2.tar` & `bloboluni-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 bloboluni-0.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloboluni-0.2.2/bloboluni/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 bloboluni-0.2.2/bloboluni/serializers.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 bloboluni-0.2.2/bloboluni/storage.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 bloboluni-0.2.2/bloboluni/test.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 bloboluni-0.2.2/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 bloboluni-0.2.2/LICENSE
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 bloboluni-0.2.2/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bloboluni-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 bloboluni-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bloboluni-1.0.0/GitVersion.yml
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 bloboluni-1.0.0/test.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 bloboluni-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloboluni-1.0.0/bloboluni/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 bloboluni-1.0.0/bloboluni/serializers.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 bloboluni-1.0.0/bloboluni/storage.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 bloboluni-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 bloboluni-1.0.0/LICENSE
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bloboluni-1.0.0/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bloboluni-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 bloboluni-1.0.0/PKG-INFO
```

### Comparing `bloboluni-0.2.2/.github/workflows/python-publish.yml` & `bloboluni-1.0.0/.github/workflows/python-publish.yml`

 * *Files 16% similar despite different names*

```diff
@@ -6,48 +6,56 @@
 # separate terms of service, privacy policy, and support
 # documentation.
 
 name: Upload Python Package
 
 on:
   push:
-    tags:
-      - '*'
+    branches: ["main"]
 
 permissions:
   contents: read
 
 jobs:
   deploy:
     name: Build and publish Python distributions to PyPI and TestPyPI
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
+      with:
+        fetch-depth: 0
+    - name: Install GitVersion
+      uses: gittools/actions/gitversion/setup@v0
+      with:
+        versionSpec: '5.x'
+    - name: Determine Version
+      id: gitversion
+      uses: gittools/actions/gitversion/execute@v0
+      with:
+        useConfigFile: true
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
-    - name: Extract tag name
-      id: tag
-      run: echo ::set-output name=TAG_NAME::$(echo $GITHUB_REF | cut -d / -f 3)
-    - name: Update version in setup.py
+    - name: Show current version
+      run: echo ${{ steps.gitversion.outputs.semVer }}
+    - name: Update version in pyproject.yml
       run: >-
-        sed -i "s/{{VERSION_PLACEHOLDER}}/${{ steps.tag.outputs.TAG_NAME }}/g" pyproject.toml
+        sed -i "s/{{VERSION_PLACEHOLDER}}/${{ steps.gitversion.outputs.semVer }}/g" pyproject.toml
     - name: Build package
       run: python -m build
     - name: Publish package to TestPyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.TEST_PYPI_API_TOKEN }}
         repository_url: https://test.pypi.org/legacy/
     - name: Publish package to PyPI
-      if: startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `bloboluni-0.2.2/bloboluni/serializers.py` & `bloboluni-1.0.0/bloboluni/serializers.py`

 * *Files identical despite different names*

### Comparing `bloboluni-0.2.2/bloboluni/test.py` & `bloboluni-1.0.0/test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
-from storage import JsonPickleBlobStorage
-import os
+from bloboluni.storage import JsonPickleBlobStorage
+import os, uuid
 from dotenv import load_dotenv
 load_dotenv()
 
 @dataclass
 class MyProfession:
     name: str
     description: str
@@ -12,15 +12,21 @@
 @dataclass
 class MyClass:
     name: str
     age: int
     profession: MyProfession
 
 if __name__ == "__main__":
-    data = MyClass("John", 30, MyProfession("Developer", "A developer"))
+    data = MyClass("blob", 30, MyProfession("Developer", "A developer"))
 
     connectionstring = os.environ["AZURE_STORAGE_CONNECTION_STRING"]
     storage = JsonPickleBlobStorage(connectionstring, "langchain")
     
-    storage.upsert("john", data)
-    john = storage.get("john")
-    storage.delete("john")
+    key = uuid.uuid4().hex
+    blob = storage.get(key)
+    assert blob is None
+    storage.upsert(key, data)
+    blob = storage.get(key)
+    assert blob is not None
+    storage.delete(key)
+    blob = storage.get(key)
+    assert blob is None
```

### Comparing `bloboluni-0.2.2/.gitignore` & `bloboluni-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bloboluni-0.2.2/LICENSE` & `bloboluni-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bloboluni-0.2.2/pyproject.toml` & `bloboluni-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bloboluni"
-version = "0.2.2"
+version = "1.0.0"
 description = "A simple package for storing and retrieving blobs of data from Azure Blob Storage"
 authors = [
   { name = "Martin Moan", email = "martin.moan1@gmail.com" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
```

### Comparing `bloboluni-0.2.2/PKG-INFO` & `bloboluni-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bloboluni
-Version: 0.2.2
+Version: 1.0.0
 Summary: A simple package for storing and retrieving blobs of data from Azure Blob Storage
 Project-URL: Homepage, https://github.com/MartinMoan/blobstorage
 Project-URL: Bug Tracker, https://github.com/MartinMoan/blobstorage/issues
 Author-email: Martin Moan <martin.moan1@gmail.com>
 License: Copyright (c) 2023 Martin Hoff Moan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,10 +34,16 @@
 Requires-Dist: python-dotenv>=1
 Requires-Dist: requests>2
 Description-Content-Type: text/markdown
 
 # BlobStorage
 A simple python package for storing and retrieving blobs of data from Azure Blob Storage.
 
+Installation:
+````
+pip install bloboluni
+````
+
+Usage
 ````
 test
 ````
```

