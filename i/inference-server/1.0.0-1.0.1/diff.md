# Comparing `tmp/inference-server-1.0.0.tar.gz` & `tmp/inference-server-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inference-server-1.0.0.tar", last modified: Thu May  4 09:30:19 2023, max compression
+gzip compressed data, was "inference-server-1.0.1.tar", last modified: Tue May  9 11:26:38 2023, max compression
```

## Comparing `inference-server-1.0.0.tar` & `inference-server-1.0.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:19.578031 inference-server-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-04 09:30:01.000000 inference-server-1.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-04 09:30:01.000000 inference-server-1.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:19.574031 inference-server-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:19.574031 inference-server-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-04 09:30:01.000000 inference-server-1.0.0/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-04 09:30:01.000000 inference-server-1.0.0/.github/workflows/test-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-04 09:30:01.000000 inference-server-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-04 09:30:01.000000 inference-server-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-04 09:30:01.000000 inference-server-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-05-04 09:30:01.000000 inference-server-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-04 09:30:01.000000 inference-server-1.0.0/LICENSE_HEADER.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14171 2023-05-04 09:30:19.578031 inference-server-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-04 09:30:01.000000 inference-server-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:19.574031 inference-server-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-04 09:30:01.000000 inference-server-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-05-04 09:30:01.000000 inference-server-1.0.0/docs/deployment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-04 09:30:01.000000 inference-server-1.0.0/docs/hooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-04 09:30:01.000000 inference-server-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-04 09:30:01.000000 inference-server-1.0.0/docs/inference_server.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 09:30:01.000000 inference-server-1.0.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-04 09:30:01.000000 inference-server-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:19.578031 inference-server-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:19.574031 inference-server-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:19.578031 inference-server-1.0.0/src/inference_server/
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-04 09:30:01.000000 inference-server-1.0.0/src/inference_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-04 09:30:01.000000 inference-server-1.0.0/src/inference_server/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-04 09:30:01.000000 inference-server-1.0.0/src/inference_server/default_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 09:30:01.000000 inference-server-1.0.0/src/inference_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-04 09:30:01.000000 inference-server-1.0.0/src/inference_server/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:19.578031 inference-server-1.0.0/src/inference_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14171 2023-05-04 09:30:19.000000 inference-server-1.0.0/src/inference_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-04 09:30:19.000000 inference-server-1.0.0/src/inference_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:19.000000 inference-server-1.0.0/src/inference_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-04 09:30:19.000000 inference-server-1.0.0/src/inference_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 09:30:19.000000 inference-server-1.0.0/src/inference_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:19.578031 inference-server-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-04 09:30:01.000000 inference-server-1.0.0/tests/test_inference_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-04 09:30:01.000000 inference-server-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:38.767274 inference-server-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-09 11:26:23.000000 inference-server-1.0.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-09 11:26:23.000000 inference-server-1.0.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:38.759274 inference-server-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:38.763274 inference-server-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-09 11:26:23.000000 inference-server-1.0.1/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-09 11:26:23.000000 inference-server-1.0.1/.github/workflows/test-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-09 11:26:23.000000 inference-server-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-09 11:26:23.000000 inference-server-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-09 11:26:23.000000 inference-server-1.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-05-09 11:26:23.000000 inference-server-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-09 11:26:23.000000 inference-server-1.0.1/LICENSE_HEADER.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-05-09 11:26:38.767274 inference-server-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-09 11:26:23.000000 inference-server-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:38.763274 inference-server-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-09 11:26:23.000000 inference-server-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-05-09 11:26:23.000000 inference-server-1.0.1/docs/deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-09 11:26:23.000000 inference-server-1.0.1/docs/hooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-09 11:26:23.000000 inference-server-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-09 11:26:23.000000 inference-server-1.0.1/docs/inference_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-09 11:26:23.000000 inference-server-1.0.1/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 11:26:23.000000 inference-server-1.0.1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-09 11:26:23.000000 inference-server-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 11:26:38.767274 inference-server-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:38.759274 inference-server-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:38.767274 inference-server-1.0.1/src/inference_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-09 11:26:23.000000 inference-server-1.0.1/src/inference_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-09 11:26:23.000000 inference-server-1.0.1/src/inference_server/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-09 11:26:23.000000 inference-server-1.0.1/src/inference_server/default_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-09 11:26:23.000000 inference-server-1.0.1/src/inference_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-09 11:26:23.000000 inference-server-1.0.1/src/inference_server/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:38.767274 inference-server-1.0.1/src/inference_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-05-09 11:26:38.000000 inference-server-1.0.1/src/inference_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-09 11:26:38.000000 inference-server-1.0.1/src/inference_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:26:38.000000 inference-server-1.0.1/src/inference_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-09 11:26:38.000000 inference-server-1.0.1/src/inference_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-09 11:26:38.000000 inference-server-1.0.1/src/inference_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:38.767274 inference-server-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-09 11:26:23.000000 inference-server-1.0.1/tests/test_inference_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-09 11:26:23.000000 inference-server-1.0.1/tox.ini
```

### Comparing `inference-server-1.0.0/.flake8` & `inference-server-1.0.1/.flake8`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.0/.github/workflows/release-package.yml` & `inference-server-1.0.1/.github/workflows/release-package.yml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.0/.github/workflows/test-package.yml` & `inference-server-1.0.1/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.0/.gitignore` & `inference-server-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.0/.pre-commit-config.yaml` & `inference-server-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.0/LICENSE` & `inference-server-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.0/LICENSE_HEADER.txt` & `inference-server-1.0.1/LICENSE_HEADER.txt`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.0/PKG-INFO` & `inference-server-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: inference-server
-Version: 1.0.0
-Summary: Pluggable Python HTTP web service (WSGI) for real-time AI/ML model inference compatible with Amazon SageMaker.
+Version: 1.0.1
+Summary: Deploy your AI/ML model to Amazon SageMaker for real-time inference using your own Docker container image.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -179,15 +179,15 @@
               of your accepting any such warranty or additional liability.
         
 Project-URL: Homepage, https://github.com/jpmorganchase/inference-server
 Project-URL: Bug Tracker, https://github.com/jpmorganchase/inference-server/issues
 Project-URL: Documentation, https://inference-server.readthedocs.io
 Project-URL: Download, https://pypi.python.org/pypi/inference-server
 Project-URL: Source Code, https://github.com/jpmorganchase/inference-server
-Keywords: artificial-intelligence,http-server,inference,jpmorganchase,machine-learning,python,sagemaker,wsgi-server
+Keywords: artificial-intelligence,docker,http-server,inference,jpmorganchase,machine-learning,python,sagemaker,wsgi-server
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -195,15 +195,15 @@
 Provides-Extra: testing
 Provides-Extra: linting
 License-File: LICENSE
 License-File: LICENSE_HEADER.txt
 
 # inference-server
 
-Pluggable Python HTTP web service (WSGI) for real-time AI/ML model inference compatible with Amazon SageMaker.
+Deploy your AI/ML model to Amazon SageMaker for real-time inference using your own Docker container image.
 
 :blue_book: Documentation: https://inference-server.readthedocs.io
 
 
 ## Installing
 
 ```shell
```

### Comparing `inference-server-1.0.0/README.md` & `inference-server-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # inference-server
 
-Pluggable Python HTTP web service (WSGI) for real-time AI/ML model inference compatible with Amazon SageMaker.
+Deploy your AI/ML model to Amazon SageMaker for real-time inference using your own Docker container image.
 
 :blue_book: Documentation: https://inference-server.readthedocs.io
 
 
 ## Installing
 
 ```shell
```

### Comparing `inference-server-1.0.0/docs/conf.py` & `inference-server-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.0/docs/deployment.rst` & `inference-server-1.0.1/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.0/docs/hooks.rst` & `inference-server-1.0.1/docs/hooks.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.0/pyproject.toml` & `inference-server-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 
 name = "inference-server"
 dynamic = ["version"]
 
 authors = [
     { name = "J.P. Morgan Chase & Co.", email = "open_source@jpmorgan.com" }
 ]
-description = "Pluggable Python HTTP web service (WSGI) for real-time AI/ML model inference compatible with Amazon SageMaker."
+description = "Deploy your AI/ML model to Amazon SageMaker for real-time inference using your own Docker container image."
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Typing :: Typed",
 ]
 keywords = [
     "artificial-intelligence",
+    "docker",
     "http-server",
     "inference",
     "jpmorganchase",
     "machine-learning",
     "python",
     "sagemaker",
     "wsgi-server",
```

### Comparing `inference-server-1.0.0/src/inference_server/__init__.py` & `inference-server-1.0.1/src/inference_server/__init__.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.0/src/inference_server/_plugin.py` & `inference-server-1.0.1/src/inference_server/_plugin.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.0/src/inference_server/default_plugin.py` & `inference-server-1.0.1/src/inference_server/default_plugin.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.0/src/inference_server/testing.py` & `inference-server-1.0.1/src/inference_server/testing.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.0/src/inference_server.egg-info/PKG-INFO` & `inference-server-1.0.1/src/inference_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: inference-server
-Version: 1.0.0
-Summary: Pluggable Python HTTP web service (WSGI) for real-time AI/ML model inference compatible with Amazon SageMaker.
+Version: 1.0.1
+Summary: Deploy your AI/ML model to Amazon SageMaker for real-time inference using your own Docker container image.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -179,15 +179,15 @@
               of your accepting any such warranty or additional liability.
         
 Project-URL: Homepage, https://github.com/jpmorganchase/inference-server
 Project-URL: Bug Tracker, https://github.com/jpmorganchase/inference-server/issues
 Project-URL: Documentation, https://inference-server.readthedocs.io
 Project-URL: Download, https://pypi.python.org/pypi/inference-server
 Project-URL: Source Code, https://github.com/jpmorganchase/inference-server
-Keywords: artificial-intelligence,http-server,inference,jpmorganchase,machine-learning,python,sagemaker,wsgi-server
+Keywords: artificial-intelligence,docker,http-server,inference,jpmorganchase,machine-learning,python,sagemaker,wsgi-server
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -195,15 +195,15 @@
 Provides-Extra: testing
 Provides-Extra: linting
 License-File: LICENSE
 License-File: LICENSE_HEADER.txt
 
 # inference-server
 
-Pluggable Python HTTP web service (WSGI) for real-time AI/ML model inference compatible with Amazon SageMaker.
+Deploy your AI/ML model to Amazon SageMaker for real-time inference using your own Docker container image.
 
 :blue_book: Documentation: https://inference-server.readthedocs.io
 
 
 ## Installing
 
 ```shell
```

### Comparing `inference-server-1.0.0/src/inference_server.egg-info/SOURCES.txt` & `inference-server-1.0.1/src/inference_server.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 .github/workflows/release-package.yml
 .github/workflows/test-package.yml
 docs/conf.py
 docs/deployment.rst
 docs/hooks.rst
 docs/index.rst
 docs/inference_server.rst
+docs/introduction.rst
 docs/modules.rst
 src/inference_server/__init__.py
 src/inference_server/_plugin.py
 src/inference_server/default_plugin.py
 src/inference_server/py.typed
 src/inference_server/testing.py
 src/inference_server.egg-info/PKG-INFO
```

### Comparing `inference-server-1.0.0/tests/test_inference_server.py` & `inference-server-1.0.1/tests/test_inference_server.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.0/tox.ini` & `inference-server-1.0.1/tox.ini`

 * *Files identical despite different names*

