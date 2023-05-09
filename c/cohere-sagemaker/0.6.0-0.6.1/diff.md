# Comparing `tmp/cohere-sagemaker-0.6.0.tar.gz` & `tmp/cohere-sagemaker-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-sagemaker-0.6.0.tar", last modified: Mon May  8 23:53:12 2023, max compression
+gzip compressed data, was "cohere-sagemaker-0.6.1.tar", last modified: Tue May  9 15:22:22 2023, max compression
```

## Comparing `cohere-sagemaker-0.6.0.tar` & `cohere-sagemaker-0.6.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-08 23:53:12.137115 cohere-sagemaker-0.6.0/
--rw-r--r--   0 alexandre   (502) staff       (20)     1066 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/LICENSE
--rw-r--r--   0 alexandre   (502) staff       (20)     1409 2023-05-08 23:53:12.136981 cohere-sagemaker-0.6.0/PKG-INFO
--rw-r--r--   0 alexandre   (502) staff       (20)      945 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/README.md
-drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-08 23:53:12.136122 cohere-sagemaker-0.6.0/cohere_sagemaker/
--rw-r--r--   0 alexandre   (502) staff       (20)       57 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/cohere_sagemaker/__init__.py
--rw-r--r--   0 alexandre   (502) staff       (20)     1222 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/cohere_sagemaker/classification.py
--rw-r--r--   0 alexandre   (502) staff       (20)    17536 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/cohere_sagemaker/client.py
--rw-r--r--   0 alexandre   (502) staff       (20)      623 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/cohere_sagemaker/embeddings.py
--rw-r--r--   0 alexandre   (502) staff       (20)      591 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/cohere_sagemaker/error.py
--rw-r--r--   0 alexandre   (502) staff       (20)      796 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/cohere_sagemaker/generation.py
--rw-r--r--   0 alexandre   (502) staff       (20)     2069 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/cohere_sagemaker/rerank.py
--rw-r--r--   0 alexandre   (502) staff       (20)      337 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/cohere_sagemaker/response.py
-drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-08 23:53:12.136807 cohere-sagemaker-0.6.0/cohere_sagemaker.egg-info/
--rw-r--r--   0 alexandre   (502) staff       (20)     1409 2023-05-08 23:53:12.000000 cohere-sagemaker-0.6.0/cohere_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 alexandre   (502) staff       (20)      460 2023-05-08 23:53:12.000000 cohere-sagemaker-0.6.0/cohere_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 alexandre   (502) staff       (20)        1 2023-05-08 23:53:12.000000 cohere-sagemaker-0.6.0/cohere_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 alexandre   (502) staff       (20)        6 2023-05-08 23:53:12.000000 cohere-sagemaker-0.6.0/cohere_sagemaker.egg-info/requires.txt
--rw-r--r--   0 alexandre   (502) staff       (20)       17 2023-05-08 23:53:12.000000 cohere-sagemaker-0.6.0/cohere_sagemaker.egg-info/top_level.txt
--rw-r--r--   0 alexandre   (502) staff       (20)       38 2023-05-08 23:53:12.137157 cohere-sagemaker-0.6.0/setup.cfg
--rw-r--r--   0 alexandre   (502) staff       (20)     1512 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.0/setup.py
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-09 15:22:22.416019 cohere-sagemaker-0.6.1/
+-rw-r--r--   0 alexandre   (502) staff       (20)     1066 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.1/LICENSE
+-rw-r--r--   0 alexandre   (502) staff       (20)     1412 2023-05-09 15:22:22.415895 cohere-sagemaker-0.6.1/PKG-INFO
+-rw-r--r--   0 alexandre   (502) staff       (20)      948 2023-05-09 15:22:05.000000 cohere-sagemaker-0.6.1/README.md
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-09 15:22:22.415132 cohere-sagemaker-0.6.1/cohere_sagemaker/
+-rw-r--r--   0 alexandre   (502) staff       (20)       57 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.1/cohere_sagemaker/__init__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     1222 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.1/cohere_sagemaker/classification.py
+-rw-r--r--   0 alexandre   (502) staff       (20)    18103 2023-05-09 15:22:05.000000 cohere-sagemaker-0.6.1/cohere_sagemaker/client.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      623 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.1/cohere_sagemaker/embeddings.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      591 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.1/cohere_sagemaker/error.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      796 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.1/cohere_sagemaker/generation.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     2069 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.1/cohere_sagemaker/rerank.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      337 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.1/cohere_sagemaker/response.py
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-09 15:22:22.415717 cohere-sagemaker-0.6.1/cohere_sagemaker.egg-info/
+-rw-r--r--   0 alexandre   (502) staff       (20)     1412 2023-05-09 15:22:22.000000 cohere-sagemaker-0.6.1/cohere_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 alexandre   (502) staff       (20)      460 2023-05-09 15:22:22.000000 cohere-sagemaker-0.6.1/cohere_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)        1 2023-05-09 15:22:22.000000 cohere-sagemaker-0.6.1/cohere_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)       16 2023-05-09 15:22:22.000000 cohere-sagemaker-0.6.1/cohere_sagemaker.egg-info/requires.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)       17 2023-05-09 15:22:22.000000 cohere-sagemaker-0.6.1/cohere_sagemaker.egg-info/top_level.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)       38 2023-05-09 15:22:22.416058 cohere-sagemaker-0.6.1/setup.cfg
+-rw-r--r--   0 alexandre   (502) staff       (20)     1525 2023-05-09 15:22:05.000000 cohere-sagemaker-0.6.1/setup.py
```

### Comparing `cohere-sagemaker-0.6.0/LICENSE` & `cohere-sagemaker-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.0/PKG-INFO` & `cohere-sagemaker-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cohere-sagemaker
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Python library for the Cohere endpoints in AWS Sagemaker
 Home-page: https://github.com/cohere-ai/cohere-sagemaker
 Author: Cohere
 Author-email: support@cohere.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Cohere Python SDK (AWS SageMaker)
 
-This package provides functionality developed to simplify interfacing with the [Cohere models via AWS SageMaker Marketplace](https://aws.amazon.com/marketplace/pp/prodview-6dmzzso5vu5my) in Python 3.
+This package provides functionality developed to simplify interfacing with the [Cohere models via AWS SageMaker Marketplace](https://aws.amazon.com/marketplace/pp/prodview-6dmzzso5vu5my) in Python >=3.6
 
 ## Installation
 
 The package can be installed with pip:
 ```bash
 pip install --upgrade cohere-sagemaker
 ```
```

### Comparing `cohere-sagemaker-0.6.0/README.md` & `cohere-sagemaker-0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Cohere Python SDK (AWS SageMaker)
 
-This package provides functionality developed to simplify interfacing with the [Cohere models via AWS SageMaker Marketplace](https://aws.amazon.com/marketplace/pp/prodview-6dmzzso5vu5my) in Python 3.
+This package provides functionality developed to simplify interfacing with the [Cohere models via AWS SageMaker Marketplace](https://aws.amazon.com/marketplace/pp/prodview-6dmzzso5vu5my) in Python >=3.6
 
 ## Installation
 
 The package can be installed with pip:
 ```bash
 pip install --upgrade cohere-sagemaker
 ```
```

### Comparing `cohere-sagemaker-0.6.0/cohere_sagemaker/classification.py` & `cohere-sagemaker-0.6.1/cohere_sagemaker/classification.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.0/cohere_sagemaker/client.py` & `cohere-sagemaker-0.6.1/cohere_sagemaker/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 import tarfile
 import tempfile
 import sagemaker as sage
 from sagemaker.s3 import parse_s3_url, S3Downloader, S3Uploader
 
 import boto3
-from botocore.exceptions import ClientError, EndpointConnectionError
+from botocore.exceptions import ClientError, EndpointConnectionError, ParamValidationError
 from cohere_sagemaker.classification import Classification, Classifications
 
 from cohere_sagemaker.embeddings import Embeddings
 from cohere_sagemaker.error import CohereError
 from cohere_sagemaker.generation import (Generation, Generations,
                                          TokenLikelihood)
 from cohere_sagemaker.rerank import Reranking
@@ -116,15 +116,15 @@
         """
         # First, check if endpoint already exists
         if self._does_endpoint_exist(endpoint_name):
             if recreate:
                 self.connect_to_endpoint(endpoint_name)
                 self.delete_endpoint()
             else:
-                raise CohereError(f"Endpoint {endpoint_name} already exists and {recreate=}.")
+                raise CohereError(f"Endpoint {endpoint_name} already exists and recreate={recreate}.")
 
         kwargs = {}
         model_data = None
         if s3_models_dir is not None:
             # If s3_models_dir is given, we assume to have custom fine-tuned models -> Algorithm
             kwargs["algorithm_arn"] = arn
             model_data = self._s3_models_dir_to_tarfile(s3_models_dir)
@@ -142,21 +142,29 @@
         model = sage.ModelPackage(
             role="ServiceRoleSagemaker", 
             model_data=model_data, 
             sagemaker_session=self._sess,  # makes sure the right region is used
             **kwargs
         )
 
-        model.deploy(
-            n_instances, 
-            instance_type, 
-            endpoint_name=endpoint_name, 
+        validation_params = dict(
             model_data_download_timeout=2400, 
             container_startup_health_check_timeout=2400
         )
+
+        try:
+            model.deploy(
+                n_instances, 
+                instance_type, 
+                endpoint_name=endpoint_name, 
+                **validation_params
+            )
+        except ParamValidationError:
+            # For at least some versions of python 3.6, SageMaker SDK does not support the validation_params
+            model.deploy(n_instances, instance_type, endpoint_name=endpoint_name)
         self.connect_to_endpoint(endpoint_name)
 
         if model_data is not None:
             # Delete the uploaded models.tar.gz it after deployment has completed
             s3_resource = boto3.resource("s3")
             bucket, key = parse_s3_url(model_data)
             s3_resource.Object(bucket, key).delete()
@@ -425,9 +433,14 @@
         
         try:
             self._service_client.delete_endpoint_config(EndpointConfigName=self._endpoint_name)
         except:
             print("Endpoint config not found, skipping deletion.")
 
     def close(self) -> None:
-        self._client.close()
-        self._service_client.close()
+        try:
+            self._client.close()
+            self._service_client.close()
+        except AttributeError:
+            print("SageMaker client could not be closed. This might be because you are using an old version of SageMaker.")
+            raise
+
```

### Comparing `cohere-sagemaker-0.6.0/cohere_sagemaker/embeddings.py` & `cohere-sagemaker-0.6.1/cohere_sagemaker/embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.0/cohere_sagemaker/error.py` & `cohere-sagemaker-0.6.1/cohere_sagemaker/error.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.0/cohere_sagemaker/generation.py` & `cohere-sagemaker-0.6.1/cohere_sagemaker/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.0/cohere_sagemaker/rerank.py` & `cohere-sagemaker-0.6.1/cohere_sagemaker/rerank.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.0/cohere_sagemaker.egg-info/PKG-INFO` & `cohere-sagemaker-0.6.1/cohere_sagemaker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cohere-sagemaker
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Python library for the Cohere endpoints in AWS Sagemaker
 Home-page: https://github.com/cohere-ai/cohere-sagemaker
 Author: Cohere
 Author-email: support@cohere.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Cohere Python SDK (AWS SageMaker)
 
-This package provides functionality developed to simplify interfacing with the [Cohere models via AWS SageMaker Marketplace](https://aws.amazon.com/marketplace/pp/prodview-6dmzzso5vu5my) in Python 3.
+This package provides functionality developed to simplify interfacing with the [Cohere models via AWS SageMaker Marketplace](https://aws.amazon.com/marketplace/pp/prodview-6dmzzso5vu5my) in Python >=3.6
 
 ## Installation
 
 The package can be installed with pip:
 ```bash
 pip install --upgrade cohere-sagemaker
 ```
```

### Comparing `cohere-sagemaker-0.6.0/setup.py` & `cohere-sagemaker-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,23 @@
         return False
 
     def has_ext_modules(foo) -> bool:
         return True
 
 
 setuptools.setup(name='cohere-sagemaker',
-                 version='0.6.0',
+                 version='0.6.1',
                  author='Cohere',
                  author_email='support@cohere.ai',
                  description='A Python library for the Cohere endpoints in AWS Sagemaker',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://github.com/cohere-ai/cohere-sagemaker',
                  packages=setuptools.find_packages(),
-                 install_requires=['boto3'],
+                 install_requires=['boto3', 'sagemaker'],
                  include_package_data=True,
                  classifiers=[
                      'Programming Language :: Python :: 3',
                      'License :: OSI Approved :: MIT License',
                      'Operating System :: OS Independent',
                  ],
                  python_requires='>=3.6',
```

