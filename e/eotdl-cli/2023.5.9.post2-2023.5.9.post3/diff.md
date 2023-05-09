# Comparing `tmp/eotdl-cli-2023.5.9.post2.tar.gz` & `tmp/eotdl-cli-2023.5.9.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl-cli-2023.5.9.post2.tar", max compression
+gzip compressed data, was "eotdl-cli-2023.5.9.post3.tar", max compression
```

## Comparing `eotdl-cli-2023.5.9.post2.tar` & `eotdl-cli-2023.5.9.post3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl-cli-2023.5.9.post2/README.md
--rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl-cli-2023.5.9.post2/eotdl_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post2/eotdl_cli/commands/__init__.py
--rw-r--r--   0        0        0      920 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9.post2/eotdl_cli/commands/auth.py
--rw-r--r--   0        0        0     1878 2023-05-09 13:11:13.605365 eotdl-cli-2023.5.9.post2/eotdl_cli/commands/datasets.py
--rw-r--r--   0        0        0      479 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9.post2/eotdl_cli/main.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post2/eotdl_cli/src/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post2/eotdl_cli/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post2/eotdl_cli/src/errors/auth.py
--rw-r--r--   0        0        0     5860 2023-05-09 13:06:29.128630 eotdl-cli-2023.5.9.post2/eotdl_cli/src/repos/APIRepo.py
--rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post2/eotdl_cli/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post2/eotdl_cli/src/repos/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/auth/main.py
--rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/DownloadDataset.py
--rw-r--r--   0        0        0      973 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/IngestDataset.py
--rw-r--r--   0        0        0      861 2023-05-09 08:01:49.700457 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py
--rw-r--r--   0        0        0      489 2023-04-11 08:30:40.657793 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
--rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
--rw-r--r--   0        0        0       91 2023-05-09 08:01:31.412351 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/__init__.py
--rw-r--r--   0        0        0     1406 2023-05-09 08:01:32.976360 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/main.py
--rw-r--r--   0        0        0      604 2023-05-09 13:13:17.081716 eotdl-cli-2023.5.9.post2/pyproject.toml
--rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 eotdl-cli-2023.5.9.post2/setup.py
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 eotdl-cli-2023.5.9.post2/PKG-INFO
+-rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl-cli-2023.5.9.post3/README.md
+-rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl-cli-2023.5.9.post3/eotdl_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post3/eotdl_cli/commands/__init__.py
+-rw-r--r--   0        0        0      920 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9.post3/eotdl_cli/commands/auth.py
+-rw-r--r--   0        0        0     2537 2023-05-09 14:49:28.320318 eotdl-cli-2023.5.9.post3/eotdl_cli/commands/datasets.py
+-rw-r--r--   0        0        0      479 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9.post3/eotdl_cli/main.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post3/eotdl_cli/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post3/eotdl_cli/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post3/eotdl_cli/src/errors/auth.py
+-rw-r--r--   0        0        0     7709 2023-05-09 15:00:49.243575 eotdl-cli-2023.5.9.post3/eotdl_cli/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post3/eotdl_cli/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post3/eotdl_cli/src/repos/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/__init__.py
+-rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      932 2023-05-09 14:32:14.727109 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0      820 2023-05-09 14:38:59.864610 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py
+-rw-r--r--   0        0        0      837 2023-05-09 14:50:06.056518 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/IngestLargeDatasetParallel.py
+-rw-r--r--   0        0        0      421 2023-05-09 14:26:26.021798 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0      148 2023-05-09 14:56:32.370413 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0     1842 2023-05-09 14:50:08.224530 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/main.py
+-rw-r--r--   0        0        0      604 2023-05-09 15:04:18.048486 eotdl-cli-2023.5.9.post3/pyproject.toml
+-rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 eotdl-cli-2023.5.9.post3/setup.py
+-rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 eotdl-cli-2023.5.9.post3/PKG-INFO
```

### Comparing `eotdl-cli-2023.5.9.post2/eotdl_cli/commands/auth.py` & `eotdl-cli-2023.5.9.post3/eotdl_cli/commands/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post2/eotdl_cli/commands/datasets.py` & `eotdl-cli-2023.5.9.post3/eotdl_cli/commands/datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typer
 from src.usecases.datasets import (
     retrieve_datasets,
     download_dataset,
-    ingest_dataset,
+    # ingest_dataset,
     ingest_large_dataset,
+    ingest_large_dataset_parallel,
 )
 from src.usecases.auth import auth
 from typing import Optional
 
 app = typer.Typer()
 
 
@@ -76,9 +77,34 @@
             typer.confirm(f"Is the data correct?", abort=True)
         ingest_large_dataset(name, description, path, user, typer.echo)
         typer.echo(f"Dataset {name} ingested")
     except Exception as e:
         typer.echo(e)
 
 
+@app.command()
+def pingest(
+    path: str,
+    n: Optional[str] = None,
+    d: Optional[str] = None,
+    y: Optional[bool] = False,
+):
+    """
+    Ingest a dataset
+
+    path: Path to dataset to ingest
+    """
+    try:
+        user = auth()
+        name = n or typer.prompt("Dataset name")
+        description = d or typer.prompt("Description")
+        # confirm
+        if not y:
+            typer.confirm(f"Is the data correct?", abort=True)
+        ingest_large_dataset_parallel(name, description, path, user, typer.echo)
+        typer.echo(f"Dataset {name} ingested")
+    except Exception as e:
+        typer.echo(e)
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `eotdl-cli-2023.5.9.post2/eotdl_cli/src/repos/AuthRepo.py` & `eotdl-cli-2023.5.9.post3/eotdl_cli/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/auth/Auth.py` & `eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/auth/main.py` & `eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/auth/main.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/IngestDataset.py` & `eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/IngestLargeDatasetParallel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pydantic import BaseModel
 
-class IngestDataset():
+
+class IngestLargeDatasetParallel:
     def __init__(self, repo, logger):
         self.repo = repo
         self.logger = logger
 
     class Inputs(BaseModel):
         name: str
         description: str
@@ -12,17 +13,17 @@
         user: dict
 
     class Outputs(BaseModel):
         dataset: dict
 
     def __call__(self, inputs: Inputs) -> Outputs:
         # allow only zip files
-        if not inputs.path.endswith('.zip'):
-            raise Exception('Only zip files are allowed')
+        if not inputs.path.endswith(".zip"):
+            raise Exception("Only zip files are allowed")
         self.logger("Ingesting dataset...")
-        response = self.repo.ingest_dataset(inputs.name, inputs.description, inputs.path, inputs.user['id_token'])
-        # response = self.repo.ingest_large_dataset(inputs.name, inputs.description, inputs.path, inputs.user['id_token'])
-        data = response.json()
-        if response.status_code == 200:
-            self.logger("Done")
-            return self.Outputs(dataset=data)
-        raise Exception(data['detail'])
+        data, error = self.repo.ingest_large_dataset_parallel(
+            inputs.name, inputs.description, inputs.path, inputs.user["id_token"]
+        )
+        if error:
+            raise Exception(error)
+        self.logger("Done")
+        return self.Outputs(dataset=data)
```

### Comparing `eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py` & `eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/IngestDataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pydantic import BaseModel
 
-class IngestLargeDataset():
+
+class IngestDataset:
     def __init__(self, repo, logger):
         self.repo = repo
         self.logger = logger
 
     class Inputs(BaseModel):
         name: str
         description: str
@@ -12,16 +13,18 @@
         user: dict
 
     class Outputs(BaseModel):
         dataset: dict
 
     def __call__(self, inputs: Inputs) -> Outputs:
         # allow only zip files
-        if not inputs.path.endswith('.zip'):
-            raise Exception('Only zip files are allowed')
+        if not inputs.path.endswith(".zip"):
+            raise Exception("Only zip files are allowed")
         self.logger("Ingesting dataset...")
-        response = self.repo.ingest_large_dataset(inputs.name, inputs.description, inputs.path, inputs.user['id_token'])
-        data = response.json()
-        if response.status_code == 200:
-            self.logger("Done")
-            return self.Outputs(dataset=data)
-        raise Exception(data['detail'])
+        data, error = self.repo.ingest_dataset(
+            inputs.name, inputs.description, inputs.path, inputs.user["id_token"]
+        )
+        # response = self.repo.ingest_large_dataset(inputs.name, inputs.description, inputs.path, inputs.user['id_token'])
+        if error:
+            raise Exception(error)
+        self.logger("Done")
+        return self.Outputs(dataset=data)
```

### Comparing `eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/main.py` & `eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,56 @@
 from ...repos import APIRepo
 from .RetrieveDatasets import RetrieveDatasets
 from .RetrieveDataset import RetrieveDataset
 from .DownloadDataset import DownloadDataset
 from .IngestDataset import IngestDataset
 from .IngestLargeDataset import IngestLargeDataset
+from .IngestLargeDatasetParallel import IngestLargeDatasetParallel
+
 
 def retrieve_datasets():
     api_repo = APIRepo()
     retrieve = RetrieveDatasets(api_repo)
     inputs = retrieve.Inputs()
     outputs = retrieve(inputs)
     return outputs.datasets
 
+
 def retrieve_dataset(name):
-	api_repo = APIRepo()
-	retrieve = RetrieveDataset(api_repo)
-	inputs = retrieve.Inputs(name=name)
-	outputs = retrieve(inputs)
-	return outputs.dataset
+    api_repo = APIRepo()
+    retrieve = RetrieveDataset(api_repo)
+    inputs = retrieve.Inputs(name=name)
+    outputs = retrieve(inputs)
+    return outputs.dataset
+
 
 def download_dataset(name, path, user):
-	dataset_id = retrieve_dataset(name)['id']
-	api_repo = APIRepo()
-	download = DownloadDataset(api_repo)
-	inputs = download.Inputs(dataset=dataset_id, path=path, user=user)
-	outputs = download(inputs)
-	return outputs.dst_path
+    dataset_id = retrieve_dataset(name)["id"]
+    api_repo = APIRepo()
+    download = DownloadDataset(api_repo)
+    inputs = download.Inputs(dataset=dataset_id, path=path, user=user)
+    outputs = download(inputs)
+    return outputs.dst_path
+
 
 def ingest_dataset(name, description, path, user, logger):
-	api_repo = APIRepo()
-	ingest = IngestDataset(api_repo, logger)
-	inputs = ingest.Inputs(name=name, description=description, path=path, user=user)
-	outputs = ingest(inputs)
-	return outputs.dataset
+    api_repo = APIRepo()
+    ingest = IngestDataset(api_repo, logger)
+    inputs = ingest.Inputs(name=name, description=description, path=path, user=user)
+    outputs = ingest(inputs)
+    return outputs.dataset
+
 
 def ingest_large_dataset(name, description, path, user, logger):
-	api_repo = APIRepo()
-	ingest = IngestLargeDataset(api_repo, logger)
-	inputs = ingest.Inputs(name=name, description=description, path=path, user=user)
-	outputs = ingest(inputs)
-	return outputs.dataset
+    api_repo = APIRepo()
+    ingest = IngestLargeDataset(api_repo, logger)
+    inputs = ingest.Inputs(name=name, description=description, path=path, user=user)
+    outputs = ingest(inputs)
+    return outputs.dataset
+
+
+def ingest_large_dataset_parallel(name, description, path, user, logger):
+    api_repo = APIRepo()
+    ingest = IngestLargeDatasetParallel(api_repo, logger)
+    inputs = ingest.Inputs(name=name, description=description, path=path, user=user)
+    outputs = ingest(inputs)
+    return outputs.dataset
```

### Comparing `eotdl-cli-2023.5.9.post2/pyproject.toml` & `eotdl-cli-2023.5.9.post3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl-cli"
-version = "2023.05.09-2"
+version = "2023.05.09-3"
 description = ""
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl_cli"}]
 
 [tool.poetry.scripts]
```

### Comparing `eotdl-cli-2023.5.9.post2/setup.py` & `eotdl-cli-2023.5.9.post3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['eotdl-cli = eotdl_cli.main:app']}
 
 setup_kwargs = {
     'name': 'eotdl-cli',
-    'version': '2023.5.9.post2',
+    'version': '2023.5.9.post3',
     'description': '',
     'long_description': '# eotdl-cli\n\nThis is the CLI for EOTDL.\n\n',
     'author': 'EarthPulse',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `eotdl-cli-2023.5.9.post2/PKG-INFO` & `eotdl-cli-2023.5.9.post3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotdl-cli
-Version: 2023.5.9.post2
+Version: 2023.5.9.post3
 Summary: 
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

