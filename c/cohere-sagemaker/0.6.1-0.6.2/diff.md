# Comparing `tmp/cohere-sagemaker-0.6.1.tar.gz` & `tmp/cohere-sagemaker-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-sagemaker-0.6.1.tar", last modified: Tue May  9 15:22:22 2023, max compression
+gzip compressed data, was "cohere-sagemaker-0.6.2.tar", last modified: Tue May  9 20:53:50 2023, max compression
```

## Comparing `cohere-sagemaker-0.6.1.tar` & `cohere-sagemaker-0.6.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-09 15:22:22.416019 cohere-sagemaker-0.6.1/
--rw-r--r--   0 alexandre   (502) staff       (20)     1066 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.1/LICENSE
--rw-r--r--   0 alexandre   (502) staff       (20)     1412 2023-05-09 15:22:22.415895 cohere-sagemaker-0.6.1/PKG-INFO
--rw-r--r--   0 alexandre   (502) staff       (20)      948 2023-05-09 15:22:05.000000 cohere-sagemaker-0.6.1/README.md
-drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-09 15:22:22.415132 cohere-sagemaker-0.6.1/cohere_sagemaker/
--rw-r--r--   0 alexandre   (502) staff       (20)       57 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.1/cohere_sagemaker/__init__.py
--rw-r--r--   0 alexandre   (502) staff       (20)     1222 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.1/cohere_sagemaker/classification.py
--rw-r--r--   0 alexandre   (502) staff       (20)    18103 2023-05-09 15:22:05.000000 cohere-sagemaker-0.6.1/cohere_sagemaker/client.py
--rw-r--r--   0 alexandre   (502) staff       (20)      623 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.1/cohere_sagemaker/embeddings.py
--rw-r--r--   0 alexandre   (502) staff       (20)      591 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.1/cohere_sagemaker/error.py
--rw-r--r--   0 alexandre   (502) staff       (20)      796 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.1/cohere_sagemaker/generation.py
--rw-r--r--   0 alexandre   (502) staff       (20)     2069 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.1/cohere_sagemaker/rerank.py
--rw-r--r--   0 alexandre   (502) staff       (20)      337 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.1/cohere_sagemaker/response.py
-drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-09 15:22:22.415717 cohere-sagemaker-0.6.1/cohere_sagemaker.egg-info/
--rw-r--r--   0 alexandre   (502) staff       (20)     1412 2023-05-09 15:22:22.000000 cohere-sagemaker-0.6.1/cohere_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 alexandre   (502) staff       (20)      460 2023-05-09 15:22:22.000000 cohere-sagemaker-0.6.1/cohere_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 alexandre   (502) staff       (20)        1 2023-05-09 15:22:22.000000 cohere-sagemaker-0.6.1/cohere_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 alexandre   (502) staff       (20)       16 2023-05-09 15:22:22.000000 cohere-sagemaker-0.6.1/cohere_sagemaker.egg-info/requires.txt
--rw-r--r--   0 alexandre   (502) staff       (20)       17 2023-05-09 15:22:22.000000 cohere-sagemaker-0.6.1/cohere_sagemaker.egg-info/top_level.txt
--rw-r--r--   0 alexandre   (502) staff       (20)       38 2023-05-09 15:22:22.416058 cohere-sagemaker-0.6.1/setup.cfg
--rw-r--r--   0 alexandre   (502) staff       (20)     1525 2023-05-09 15:22:05.000000 cohere-sagemaker-0.6.1/setup.py
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-09 20:53:50.072662 cohere-sagemaker-0.6.2/
+-rw-r--r--   0 alexandre   (502) staff       (20)     1066 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.2/LICENSE
+-rw-r--r--   0 alexandre   (502) staff       (20)     1412 2023-05-09 20:53:50.072533 cohere-sagemaker-0.6.2/PKG-INFO
+-rw-r--r--   0 alexandre   (502) staff       (20)      948 2023-05-09 15:22:05.000000 cohere-sagemaker-0.6.2/README.md
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-09 20:53:50.071780 cohere-sagemaker-0.6.2/cohere_sagemaker/
+-rw-r--r--   0 alexandre   (502) staff       (20)       57 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.2/cohere_sagemaker/__init__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     1222 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.2/cohere_sagemaker/classification.py
+-rw-r--r--   0 alexandre   (502) staff       (20)    19336 2023-05-09 20:02:06.000000 cohere-sagemaker-0.6.2/cohere_sagemaker/client.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      623 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.2/cohere_sagemaker/embeddings.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      591 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.2/cohere_sagemaker/error.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      796 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.2/cohere_sagemaker/generation.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     2069 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.2/cohere_sagemaker/rerank.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      337 2023-05-08 23:46:08.000000 cohere-sagemaker-0.6.2/cohere_sagemaker/response.py
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2023-05-09 20:53:50.072348 cohere-sagemaker-0.6.2/cohere_sagemaker.egg-info/
+-rw-r--r--   0 alexandre   (502) staff       (20)     1412 2023-05-09 20:53:50.000000 cohere-sagemaker-0.6.2/cohere_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 alexandre   (502) staff       (20)      460 2023-05-09 20:53:50.000000 cohere-sagemaker-0.6.2/cohere_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)        1 2023-05-09 20:53:50.000000 cohere-sagemaker-0.6.2/cohere_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)       16 2023-05-09 20:53:50.000000 cohere-sagemaker-0.6.2/cohere_sagemaker.egg-info/requires.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)       17 2023-05-09 20:53:50.000000 cohere-sagemaker-0.6.2/cohere_sagemaker.egg-info/top_level.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)       38 2023-05-09 20:53:50.072704 cohere-sagemaker-0.6.2/setup.cfg
+-rw-r--r--   0 alexandre   (502) staff       (20)     1525 2023-05-09 20:46:51.000000 cohere-sagemaker-0.6.2/setup.py
```

### Comparing `cohere-sagemaker-0.6.1/LICENSE` & `cohere-sagemaker-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.1/PKG-INFO` & `cohere-sagemaker-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere-sagemaker
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Python library for the Cohere endpoints in AWS Sagemaker
 Home-page: https://github.com/cohere-ai/cohere-sagemaker
 Author: Cohere
 Author-email: support@cohere.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cohere-sagemaker-0.6.1/README.md` & `cohere-sagemaker-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.1/cohere_sagemaker/classification.py` & `cohere-sagemaker-0.6.2/cohere_sagemaker/classification.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.1/cohere_sagemaker/client.py` & `cohere-sagemaker-0.6.2/cohere_sagemaker/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,25 +98,29 @@
         self,
         arn: str,
         endpoint_name: str,
         s3_models_dir: Optional[str] = None,
         instance_type: str = "ml.g4dn.xlarge",
         n_instances: int = 1,
         recreate: bool = False,
+        role: Optional[str] = None,
     ) -> None:
         """Creates and deploys a SageMaker endpoint.
 
         Args:
             arn (str): The product ARN. Refers to a ready-to-use model (model package) or a fine-tuned model
                 (algorithm).
             endpoint_name (str): The name of the endpoint.
             s3_models_dir (str, optional): S3 URI pointing to the folder containing fine-tuned models. Defaults to None.
             instance_type (str, optional): The EC2 instance type to deploy the endpoint to. Defaults to "ml.g4dn.xlarge".
             n_instances (int, optional): Number of endpoint instances. Defaults to 1.
             recreate (bool, optional): Force re-creation of endpoint if it already exists. Defaults to False.
+            rool (str, optional): The IAM role to use for the endpoint. If not provided, sagemaker.get_execution_role()
+                will be used to get the role. This should work when one uses the client inside SageMaker. If this errors 
+                out, the default role "ServiceRoleSagemaker" will be used, which generally works outside of SageMaker.
         """
         # First, check if endpoint already exists
         if self._does_endpoint_exist(endpoint_name):
             if recreate:
                 self.connect_to_endpoint(endpoint_name)
                 self.delete_endpoint()
             else:
@@ -135,16 +139,23 @@
         # Out of precaution, check if there is an endpoint config and delete it if that's the case
         # Otherwise it might block deployment
         try:
             self._service_client.delete_endpoint_config(EndpointConfigName=endpoint_name)
         except ClientError:
             pass
 
+        if role is None:
+            try:
+                role = sage.get_execution_role()
+            except ValueError:
+                print("Using default role: 'ServiceRoleSagemaker'.")
+                role = "ServiceRoleSagemaker"
+
         model = sage.ModelPackage(
-            role="ServiceRoleSagemaker", 
+            role=role,
             model_data=model_data, 
             sagemaker_session=self._sess,  # makes sure the right region is used
             **kwargs
         )
 
         validation_params = dict(
             model_data_download_timeout=2400, 
@@ -369,33 +380,44 @@
         arn: str,
         name: str,
         train_data: str,
         s3_models_dir: str,
         eval_data: Optional[str] = None,
         instance_type: str = "ml.g4dn.xlarge",
         training_parameters: Dict[str, Any] = {},  # Optional, training algorithm specific hyper-parameters
+        role: Optional[str] = None,
     ) -> None:
         """Creates a fine-tuning job.
 
         Args:
             arn (str): The product ARN of the fine-tuning package.
             name (str): The name to give to the fine-tuned model.
             train_data (str): An S3 path pointing to the training data.
             s3_models_dir (str): An S3 path pointing to the directory where the fine-tuned model will be saved.
             eval_data (str, optional): An S3 path pointing to the eval data. Defaults to None.
             instance_type (str, optional): The EC2 instance type to use for training. Defaults to "ml.g4dn.xlarge".
             training_parameters (Dict[str, Any], optional): Additional training parameters. Defaults to {}.
+            rool (str, optional): The IAM role to use for the endpoint. If not provided, sagemaker.get_execution_role()
+                will be used to get the role. This should work when one uses the client inside SageMaker. If this errors 
+                out, the default role "ServiceRoleSagemaker" will be used, which generally works outside of SageMaker.
         """
         assert len(training_parameters) == 0, "training_parameters not yet supported."
         assert name != "model", "name cannot be 'model'"
         s3_models_dir = s3_models_dir + ("/" if not s3_models_dir.endswith("/") else "")
 
+        if role is None:
+            try:
+                role = sage.get_execution_role()
+            except ValueError:
+                print("Using default role: 'ServiceRoleSagemaker'.")
+                role = "ServiceRoleSagemaker"
+
         estimator = sage.algorithm.AlgorithmEstimator(
             algorithm_arn=arn,
-            role="ServiceRoleSagemaker",
+            role=role,
             instance_count=1,
             instance_type=instance_type,
             sagemaker_session=self._sess,
             output_path=s3_models_dir,
             hyperparameters={"name": name},
         )
```

### Comparing `cohere-sagemaker-0.6.1/cohere_sagemaker/embeddings.py` & `cohere-sagemaker-0.6.2/cohere_sagemaker/embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.1/cohere_sagemaker/error.py` & `cohere-sagemaker-0.6.2/cohere_sagemaker/error.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.1/cohere_sagemaker/generation.py` & `cohere-sagemaker-0.6.2/cohere_sagemaker/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.1/cohere_sagemaker/rerank.py` & `cohere-sagemaker-0.6.2/cohere_sagemaker/rerank.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.6.1/cohere_sagemaker.egg-info/PKG-INFO` & `cohere-sagemaker-0.6.2/cohere_sagemaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere-sagemaker
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Python library for the Cohere endpoints in AWS Sagemaker
 Home-page: https://github.com/cohere-ai/cohere-sagemaker
 Author: Cohere
 Author-email: support@cohere.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cohere-sagemaker-0.6.1/setup.py` & `cohere-sagemaker-0.6.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         return False
 
     def has_ext_modules(foo) -> bool:
         return True
 
 
 setuptools.setup(name='cohere-sagemaker',
-                 version='0.6.1',
+                 version='0.6.2',
                  author='Cohere',
                  author_email='support@cohere.ai',
                  description='A Python library for the Cohere endpoints in AWS Sagemaker',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://github.com/cohere-ai/cohere-sagemaker',
                  packages=setuptools.find_packages(),
```

