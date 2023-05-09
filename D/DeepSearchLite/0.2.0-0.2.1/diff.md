# Comparing `tmp/DeepSearchLite-0.2.0.tar.gz` & `tmp/DeepSearchLite-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepSearchLite-0.2.0.tar", last modified: Mon May  8 16:17:17 2023, max compression
+gzip compressed data, was "DeepSearchLite-0.2.1.tar", last modified: Tue May  9 16:02:52 2023, max compression
```

## Comparing `DeepSearchLite-0.2.0.tar` & `DeepSearchLite-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ibad      (1000) ibad      (1000)        0 2023-05-08 16:17:17.500680 DeepSearchLite-0.2.0/
-drwxrwxr-x   0 ibad      (1000) ibad      (1000)        0 2023-05-08 16:17:17.500680 DeepSearchLite-0.2.0/DeepSearchLite/
--rw-rw-r--   0 ibad      (1000) ibad      (1000)    16114 2023-05-08 16:14:43.000000 DeepSearchLite-0.2.0/DeepSearchLite/DeepSearchLite.py
--rw-rw-r--   0 ibad      (1000) ibad      (1000)       65 2023-05-07 01:07:56.000000 DeepSearchLite-0.2.0/DeepSearchLite/__init__.py
-drwxrwxr-x   0 ibad      (1000) ibad      (1000)        0 2023-05-08 16:17:17.500680 DeepSearchLite-0.2.0/DeepSearchLite.egg-info/
--rw-rw-r--   0 ibad      (1000) ibad      (1000)     6346 2023-05-08 16:17:17.000000 DeepSearchLite-0.2.0/DeepSearchLite.egg-info/PKG-INFO
--rw-rw-r--   0 ibad      (1000) ibad      (1000)      275 2023-05-08 16:17:17.000000 DeepSearchLite-0.2.0/DeepSearchLite.egg-info/SOURCES.txt
--rw-rw-r--   0 ibad      (1000) ibad      (1000)        1 2023-05-08 16:17:17.000000 DeepSearchLite-0.2.0/DeepSearchLite.egg-info/dependency_links.txt
--rw-rw-r--   0 ibad      (1000) ibad      (1000)       35 2023-05-08 16:17:17.000000 DeepSearchLite-0.2.0/DeepSearchLite.egg-info/requires.txt
--rw-rw-r--   0 ibad      (1000) ibad      (1000)       15 2023-05-08 16:17:17.000000 DeepSearchLite-0.2.0/DeepSearchLite.egg-info/top_level.txt
--rw-rw-r--   0 ibad      (1000) ibad      (1000)     1068 2023-05-07 01:06:14.000000 DeepSearchLite-0.2.0/LICENSE
--rw-rw-r--   0 ibad      (1000) ibad      (1000)     6346 2023-05-08 16:17:17.500680 DeepSearchLite-0.2.0/PKG-INFO
--rw-rw-r--   0 ibad      (1000) ibad      (1000)     5655 2023-05-08 16:14:43.000000 DeepSearchLite-0.2.0/README.md
--rw-rw-r--   0 ibad      (1000) ibad      (1000)       38 2023-05-08 16:17:17.500680 DeepSearchLite-0.2.0/setup.cfg
--rw-rw-r--   0 ibad      (1000) ibad      (1000)     1044 2023-05-08 16:14:43.000000 DeepSearchLite-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:02:52.902332 DeepSearchLite-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:02:52.902332 DeepSearchLite-0.2.1/DeepSearchLite/
+-rw-r--r--   0 runner    (1001) docker     (123)    16114 2023-05-09 16:02:39.000000 DeepSearchLite-0.2.1/DeepSearchLite/DeepSearchLite.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-09 16:02:39.000000 DeepSearchLite-0.2.1/DeepSearchLite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:02:52.902332 DeepSearchLite-0.2.1/DeepSearchLite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-09 16:02:52.000000 DeepSearchLite-0.2.1/DeepSearchLite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-09 16:02:52.000000 DeepSearchLite-0.2.1/DeepSearchLite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:02:52.000000 DeepSearchLite-0.2.1/DeepSearchLite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-09 16:02:52.000000 DeepSearchLite-0.2.1/DeepSearchLite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 16:02:52.000000 DeepSearchLite-0.2.1/DeepSearchLite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-09 16:02:39.000000 DeepSearchLite-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-09 16:02:52.902332 DeepSearchLite-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-09 16:02:39.000000 DeepSearchLite-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 16:02:52.902332 DeepSearchLite-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-09 16:02:39.000000 DeepSearchLite-0.2.1/setup.py
```

### Comparing `DeepSearchLite-0.2.0/DeepSearchLite/DeepSearchLite.py` & `DeepSearchLite-0.2.1/DeepSearchLite/DeepSearchLite.py`

 * *Files identical despite different names*

### Comparing `DeepSearchLite-0.2.0/DeepSearchLite.egg-info/PKG-INFO` & `DeepSearchLite-0.2.1/DeepSearchLite.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: DeepSearchLite
-Version: 0.2.0
-Summary: A package for image similarity search
+Version: 0.2.1
+Summary: A package for similarity search for any type of data. Use your own feature extractor and data loader and use this package to perform similarity search.
 Home-page: https://github.com/ibadrather/DeepSearchLite
 Author: Ibad Rather
 Author-email: ibad.rather.ir@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DeepSearchLite-0.2.0/LICENSE` & `DeepSearchLite-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepSearchLite-0.2.0/PKG-INFO` & `DeepSearchLite-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: DeepSearchLite
-Version: 0.2.0
-Summary: A package for image similarity search
+Version: 0.2.1
+Summary: A package for similarity search for any type of data. Use your own feature extractor and data loader and use this package to perform similarity search.
 Home-page: https://github.com/ibadrather/DeepSearchLite
 Author: Ibad Rather
 Author-email: ibad.rather.ir@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DeepSearchLite-0.2.0/README.md` & `DeepSearchLite-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `DeepSearchLite-0.2.0/setup.py` & `DeepSearchLite-0.2.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DeepSearchLite",
-    version="0.2.0",
+    version="0.2.1",
     author="Ibad Rather",
     author_email="ibad.rather.ir@gmail.com",
-    description="A package for image similarity search",
+    description="A package for similarity search for any type of data. Use your own feature extractor and data loader and use this package to perform similarity search.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ibadrather/DeepSearchLite",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

