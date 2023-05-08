# Comparing `tmp/cohere-sagemaker-0.5.0.tar.gz` & `tmp/cohere-sagemaker-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-sagemaker-0.5.0.tar", last modified: Tue Mar 14 16:51:54 2023, max compression
+gzip compressed data, was "cohere-sagemaker-0.6.0.tar", last modified: Mon May  8 23:53:12 2023, max compression
```

## Comparing `cohere-sagemaker-0.5.0.tar` & `cohere-sagemaker-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 1vn        (502) staff       (20)        0 2023-03-14 16:51:54.190202 cohere-sagemaker-0.5.0/
--rw-r--r--   0 1vn        (502) staff       (20)     1066 2023-03-13 22:08:03.000000 cohere-sagemaker-0.5.0/LICENSE
--rw-r--r--   0 1vn        (502) staff       (20)     1795 2023-03-14 16:51:54.190085 cohere-sagemaker-0.5.0/PKG-INFO
--rw-r--r--   0 1vn        (502) staff       (20)     1294 2023-03-13 22:08:03.000000 cohere-sagemaker-0.5.0/README.md
-drwxr-xr-x   0 1vn        (502) staff       (20)        0 2023-03-14 16:51:54.189397 cohere-sagemaker-0.5.0/cohere_sagemaker/
--rw-r--r--   0 1vn        (502) staff       (20)       57 2023-03-13 22:08:03.000000 cohere-sagemaker-0.5.0/cohere_sagemaker/__init__.py
--rw-r--r--   0 1vn        (502) staff       (20)     6227 2023-03-14 14:39:10.000000 cohere-sagemaker-0.5.0/cohere_sagemaker/client.py
--rw-r--r--   0 1vn        (502) staff       (20)      623 2023-03-13 22:08:03.000000 cohere-sagemaker-0.5.0/cohere_sagemaker/embeddings.py
--rw-r--r--   0 1vn        (502) staff       (20)      591 2023-03-13 22:08:03.000000 cohere-sagemaker-0.5.0/cohere_sagemaker/error.py
--rw-r--r--   0 1vn        (502) staff       (20)      796 2023-03-13 22:08:03.000000 cohere-sagemaker-0.5.0/cohere_sagemaker/generation.py
--rw-r--r--   0 1vn        (502) staff       (20)     2069 2023-03-14 14:39:10.000000 cohere-sagemaker-0.5.0/cohere_sagemaker/rerank.py
--rw-r--r--   0 1vn        (502) staff       (20)      337 2023-03-13 22:08:03.000000 cohere-sagemaker-0.5.0/cohere_sagemaker/response.py
-drwxr-xr-x   0 1vn        (502) staff       (20)        0 2023-03-14 16:51:54.189943 cohere-sagemaker-0.5.0/cohere_sagemaker.egg-info/
--rw-r--r--   0 1vn        (502) staff       (20)     1795 2023-03-14 16:51:54.000000 cohere-sagemaker-0.5.0/cohere_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 1vn        (502) staff       (20)      425 2023-03-14 16:51:54.000000 cohere-sagemaker-0.5.0/cohere_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 1vn        (502) staff       (20)        1 2023-03-14 16:51:54.000000 cohere-sagemaker-0.5.0/cohere_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 1vn        (502) staff       (20)        6 2023-03-14 16:51:54.000000 cohere-sagemaker-0.5.0/cohere_sagemaker.egg-info/requires.txt
--rw-r--r--   0 1vn        (502) staff       (20)       17 2023-03-14 16:51:54.000000 cohere-sagemaker-0.5.0/cohere_sagemaker.egg-info/top_level.txt
--rw-r--r--   0 1vn        (502) staff       (20)       38 2023-03-14 16:51:54.190245 cohere-sagemaker-0.5.0/setup.cfg
--rw-r--r--   0 1vn        (502) staff       (20)     1512 2023-03-14 14:39:10.000000 cohere-sagemaker-0.5.0/setup.py
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-08 23:53:12.137115 cohere-sagemaker-0.6.0/
+-rw-r--r--   0 alexandre   (502) staff       (20)     1066 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/LICENSE
+-rw-r--r--   0 alexandre   (502) staff       (20)     1409 2023-05-08 23:53:12.136981 cohere-sagemaker-0.6.0/PKG-INFO
+-rw-r--r--   0 alexandre   (502) staff       (20)      945 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/README.md
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-08 23:53:12.136122 cohere-sagemaker-0.6.0/cohere_sagemaker/
+-rw-r--r--   0 alexandre   (502) staff       (20)       57 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/cohere_sagemaker/__init__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     1222 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/cohere_sagemaker/classification.py
+-rw-r--r--   0 alexandre   (502) staff       (20)    17536 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/cohere_sagemaker/client.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      623 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/cohere_sagemaker/embeddings.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      591 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/cohere_sagemaker/error.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      796 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/cohere_sagemaker/generation.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     2069 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/cohere_sagemaker/rerank.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      337 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/cohere_sagemaker/response.py
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-08 23:53:12.136807 cohere-sagemaker-0.6.0/cohere_sagemaker.egg-info/
+-rw-r--r--   0 alexandre   (502) staff       (20)     1409 2023-05-08 23:53:12.000000 cohere-sagemaker-0.6.0/cohere_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 alexandre   (502) staff       (20)      460 2023-05-08 23:53:12.000000 cohere-sagemaker-0.6.0/cohere_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)        1 2023-05-08 23:53:12.000000 cohere-sagemaker-0.6.0/cohere_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)        6 2023-05-08 23:53:12.000000 cohere-sagemaker-0.6.0/cohere_sagemaker.egg-info/requires.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)       17 2023-05-08 23:53:12.000000 cohere-sagemaker-0.6.0/cohere_sagemaker.egg-info/top_level.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)       38 2023-05-08 23:53:12.137157 cohere-sagemaker-0.6.0/setup.cfg
+-rw-r--r--   0 alexandre   (502) staff       (20)     1512 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/setup.py
```

### Comparing `cohere-sagemaker-0.5.0/LICENSE` & `cohere-sagemaker-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.5.0/README.md` & `cohere-sagemaker-0.6.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -12,27 +12,14 @@
 Install from source:
 ```bash
 python setup.py install
 ```
 
 ## Quick Start
 
-To use this library, you need to configure your AWS credentials. You can do this by running `aws configure`. Once that's set up, you can use the library like this:
-```python
-from cohere_sagemaker import Client
-
-client = Client(endpoint_name='my-cohere-endpoint')
+To use this library, you need to configure your AWS credentials. You can do this by running `aws configure`. Once that's set up, please refer to one of the Jupyter notebooks to get started. Here is the one for our [medium command model](https://github.com/cohere-ai/cohere-sagemaker/blob/main/notebooks/Deploy%20command%20medium.ipynb)
 
-# generate prediction for a prompt
-response = client.generate(
-    prompt="Tell me a story about",
-    max_tokens=20)
 
-print(response.generations[0].text)
-# a time when you had to make a difficult decision. What did you do
-```
 Note: by default we assume region configured in AWS CLI (`aws configure get region`), to override use `region_name` parameter, e.g.
 ```python
-client = Client(endpoint_name='my-cohere-endpoint', region_name='us-east-1')
+client = Client(region_name='us-east-1')
 ```
-
-More detailed examples can be found in the [Jupyter notebook](https://github.com/cohere-ai/cohere-sagemaker/blob/main/notebooks/Deploy%20cohere%20model.ipynb).
```

### Comparing `cohere-sagemaker-0.5.0/cohere_sagemaker/embeddings.py` & `cohere-sagemaker-0.6.0/cohere_sagemaker/embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.5.0/cohere_sagemaker/error.py` & `cohere-sagemaker-0.6.0/cohere_sagemaker/error.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.5.0/cohere_sagemaker/generation.py` & `cohere-sagemaker-0.6.0/cohere_sagemaker/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.5.0/cohere_sagemaker/rerank.py` & `cohere-sagemaker-0.6.0/cohere_sagemaker/rerank.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.5.0/setup.py` & `cohere-sagemaker-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         return False
 
     def has_ext_modules(foo) -> bool:
         return True
 
 
 setuptools.setup(name='cohere-sagemaker',
-                 version='0.5.0',
+                 version='0.6.0',
                  author='Cohere',
                  author_email='support@cohere.ai',
                  description='A Python library for the Cohere endpoints in AWS Sagemaker',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://github.com/cohere-ai/cohere-sagemaker',
                  packages=setuptools.find_packages(),
```

