# Comparing `tmp/cubed-xarray-0.0.0.tar.gz` & `tmp/cubed-xarray-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubed-xarray-0.0.0.tar", last modified: Mon May  8 19:55:23 2023, max compression
+gzip compressed data, was "cubed-xarray-0.0.1.tar", last modified: Tue May  9 15:39:01 2023, max compression
```

## Comparing `cubed-xarray-0.0.0.tar` & `cubed-xarray-0.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-05-08 19:55:23.501523 cubed-xarray-0.0.0/
--rw-rw-r--   0 tom       (1001) tom       (1001)     1799 2023-03-24 16:03:06.000000 cubed-xarray-0.0.0/.gitignore
--rw-rw-r--   0 tom       (1001) tom       (1001)    11357 2023-03-24 16:03:06.000000 cubed-xarray-0.0.0/LICENSE
--rw-rw-r--   0 tom       (1001) tom       (1001)     2258 2023-05-08 19:55:23.501523 cubed-xarray-0.0.0/PKG-INFO
--rw-rw-r--   0 tom       (1001) tom       (1001)     1342 2023-05-05 20:01:03.000000 cubed-xarray-0.0.0/README.md
-drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-05-08 19:55:23.501523 cubed-xarray-0.0.0/cubed_xarray/
--rw-rw-r--   0 tom       (1001) tom       (1001)      243 2023-04-06 18:08:26.000000 cubed-xarray-0.0.0/cubed_xarray/__init__.py
--rw-rw-r--   0 tom       (1001) tom       (1001)     5724 2023-05-05 20:06:01.000000 cubed-xarray-0.0.0/cubed_xarray/cubedmanager.py
-drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-05-08 19:55:23.501523 cubed-xarray-0.0.0/cubed_xarray/tests/
--rw-rw-r--   0 tom       (1001) tom       (1001)        0 2023-04-06 18:08:26.000000 cubed-xarray-0.0.0/cubed_xarray/tests/__init__.py
--rw-rw-r--   0 tom       (1001) tom       (1001)        0 2023-05-05 21:02:48.000000 cubed-xarray-0.0.0/cubed_xarray/tests/test_wrapping.py
-drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-05-08 19:55:23.501523 cubed-xarray-0.0.0/cubed_xarray.egg-info/
--rw-rw-r--   0 tom       (1001) tom       (1001)     2258 2023-05-08 19:55:23.000000 cubed-xarray-0.0.0/cubed_xarray.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1001) tom       (1001)      418 2023-05-08 19:55:23.000000 cubed-xarray-0.0.0/cubed_xarray.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)        1 2023-05-08 19:55:23.000000 cubed-xarray-0.0.0/cubed_xarray.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)       70 2023-05-08 19:55:23.000000 cubed-xarray-0.0.0/cubed_xarray.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)       40 2023-05-08 19:55:23.000000 cubed-xarray-0.0.0/cubed_xarray.egg-info/requires.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)       13 2023-05-08 19:55:23.000000 cubed-xarray-0.0.0/cubed_xarray.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)     1417 2023-04-06 18:08:26.000000 cubed-xarray-0.0.0/pyproject.toml
--rw-rw-r--   0 tom       (1001) tom       (1001)       44 2023-05-04 22:39:07.000000 cubed-xarray-0.0.0/requirements.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)      134 2023-05-08 19:55:23.501523 cubed-xarray-0.0.0/setup.cfg
--rw-rw-r--   0 tom       (1001) tom       (1001)       93 2023-04-06 18:08:26.000000 cubed-xarray-0.0.0/setup.py
+drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-05-09 15:39:01.067148 cubed-xarray-0.0.1/
+-rw-rw-r--   0 tom       (1001) tom       (1001)     1799 2023-03-24 16:03:06.000000 cubed-xarray-0.0.1/.gitignore
+-rw-rw-r--   0 tom       (1001) tom       (1001)    11357 2023-03-24 16:03:06.000000 cubed-xarray-0.0.1/LICENSE
+-rw-rw-r--   0 tom       (1001) tom       (1001)     2334 2023-05-09 15:39:01.067148 cubed-xarray-0.0.1/PKG-INFO
+-rw-rw-r--   0 tom       (1001) tom       (1001)     1342 2023-05-05 20:01:03.000000 cubed-xarray-0.0.1/README.md
+drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-05-09 15:39:01.067148 cubed-xarray-0.0.1/cubed_xarray/
+-rw-rw-r--   0 tom       (1001) tom       (1001)      243 2023-04-06 18:08:26.000000 cubed-xarray-0.0.1/cubed_xarray/__init__.py
+-rw-rw-r--   0 tom       (1001) tom       (1001)     5641 2023-05-08 19:56:58.000000 cubed-xarray-0.0.1/cubed_xarray/cubedmanager.py
+drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-05-09 15:39:01.067148 cubed-xarray-0.0.1/cubed_xarray/tests/
+-rw-rw-r--   0 tom       (1001) tom       (1001)        0 2023-04-06 18:08:26.000000 cubed-xarray-0.0.1/cubed_xarray/tests/__init__.py
+-rw-rw-r--   0 tom       (1001) tom       (1001)        0 2023-05-05 21:02:48.000000 cubed-xarray-0.0.1/cubed_xarray/tests/test_wrapping.py
+drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-05-09 15:39:01.067148 cubed-xarray-0.0.1/cubed_xarray.egg-info/
+-rw-rw-r--   0 tom       (1001) tom       (1001)     2334 2023-05-09 15:39:01.000000 cubed-xarray-0.0.1/cubed_xarray.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1001) tom       (1001)      418 2023-05-09 15:39:01.000000 cubed-xarray-0.0.1/cubed_xarray.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)        1 2023-05-09 15:39:01.000000 cubed-xarray-0.0.1/cubed_xarray.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)       70 2023-05-09 15:39:01.000000 cubed-xarray-0.0.1/cubed_xarray.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)       40 2023-05-09 15:39:01.000000 cubed-xarray-0.0.1/cubed_xarray.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)       13 2023-05-09 15:39:01.000000 cubed-xarray-0.0.1/cubed_xarray.egg-info/top_level.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)     1575 2023-05-09 15:36:05.000000 cubed-xarray-0.0.1/pyproject.toml
+-rw-rw-r--   0 tom       (1001) tom       (1001)       44 2023-05-04 22:39:07.000000 cubed-xarray-0.0.1/requirements.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)       38 2023-05-09 15:39:01.067148 cubed-xarray-0.0.1/setup.cfg
+-rw-rw-r--   0 tom       (1001) tom       (1001)       93 2023-04-06 18:08:26.000000 cubed-xarray-0.0.1/setup.py
```

### Comparing `cubed-xarray-0.0.0/.gitignore` & `cubed-xarray-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cubed-xarray-0.0.0/LICENSE` & `cubed-xarray-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cubed-xarray-0.0.0/PKG-INFO` & `cubed-xarray-0.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cubed-xarray
-Version: 0.0.0
+Version: 0.0.1
 Summary: Interface for using cubed with xarray for parallel computation.
 Author-email: Tom Nicholas <tomnicholas1@googlemail.com>
 License: Apache-2
-Project-URL: Home, https://github.com/xarray-contrib/cubed-xarray
-Project-URL: Documentation, https://github.com/xarray-contrib/cubed-xarray#readme
+Project-URL: homepage, https://github.com/xarray-contrib/cubed-xarray
+Project-URL: documentation, https://github.com/xarray-contrib/cubed-xarray#readme
+Project-URL: repository, https://github.com/xarray-contrib/cubed-xarray
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `cubed-xarray-0.0.0/README.md` & `cubed-xarray-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cubed-xarray-0.0.0/cubed_xarray/cubedmanager.py` & `cubed-xarray-0.0.1/cubed_xarray/cubedmanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,21 +47,18 @@
         from cubed import from_array
 
         # Extract cubed-specific kwargs.
         # Also ignores dask-specific kwargs that are passed in.
         # The passing of dask-specific kwargs to cubed should be eventually removed by deprecating them
         # as explicit arguments to xarray methods
         spec = kwargs.pop("spec", None)
-        name = kwargs.pop("name", None)
-        print(name)
 
         return from_array(
             data,
             chunks,
-            name=name,
             spec=spec,
         )
 
     def rechunk(self, data: "CubedArray", chunks, **kwargs) -> "CubedArray":
         return data.rechunk(chunks, **kwargs)
 
     def compute(self, *data: "CubedArray", **kwargs) -> np.ndarray:
```

### Comparing `cubed-xarray-0.0.0/cubed_xarray.egg-info/PKG-INFO` & `cubed-xarray-0.0.1/cubed_xarray.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cubed-xarray
-Version: 0.0.0
+Version: 0.0.1
 Summary: Interface for using cubed with xarray for parallel computation.
 Author-email: Tom Nicholas <tomnicholas1@googlemail.com>
 License: Apache-2
-Project-URL: Home, https://github.com/xarray-contrib/cubed-xarray
-Project-URL: Documentation, https://github.com/xarray-contrib/cubed-xarray#readme
+Project-URL: homepage, https://github.com/xarray-contrib/cubed-xarray
+Project-URL: documentation, https://github.com/xarray-contrib/cubed-xarray#readme
+Project-URL: repository, https://github.com/xarray-contrib/cubed-xarray
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `cubed-xarray-0.0.0/pyproject.toml` & `cubed-xarray-0.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [project]
 name = "cubed-xarray"
+version = "0.0.1"
 authors = [
     {name = "Tom Nicholas", email = "tomnicholas1@googlemail.com"}
 ]
 description = "Interface for using cubed with xarray for parallel computation."
 license = {text = "Apache-2"}
 readme = "README.md"
 classifiers = [
@@ -20,26 +21,29 @@
 ]
 requires-python = ">=3.9"
 dependencies = [
     "numpy >= 1.17",
     "xarray >= 0.16.1",
     "cubed >= 0.6.0",
 ]
-dynamic = ["version"]
 
 [project.urls]
-Home = "https://github.com/xarray-contrib/cubed-xarray"
-Documentation = "https://github.com/xarray-contrib/cubed-xarray#readme"
+homepage = "https://github.com/xarray-contrib/cubed-xarray"
+documentation = "https://github.com/xarray-contrib/cubed-xarray#readme"
+repository = "https://github.com/xarray-contrib/cubed-xarray"
 
 [tool.setuptools.packages.find]
 include = [
     "cubed_xarray",
     "cubed_xarray.tests",
 ]
 
+[project.entry-points."xarray.chunkmanagers"]
+cubed = "cubed_xarray.cubedmanager:CubedManager"
+
 [build-system]
 requires = ["setuptools >= 64", "setuptools_scm >= 7.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 fallback_version = "999"
```

