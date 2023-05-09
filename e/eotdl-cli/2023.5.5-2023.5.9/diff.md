# Comparing `tmp/eotdl_cli-2023.5.5.tar.gz` & `tmp/eotdl-cli-2023.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl_cli-2023.5.5.tar", max compression
+gzip compressed data, was "eotdl-cli-2023.5.9.tar", max compression
```

## Comparing `eotdl_cli-2023.5.5.tar` & `eotdl-cli-2023.5.9.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl_cli-2023.5.5/README.md
--rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl_cli-2023.5.5/eotdl_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-2023.5.5/eotdl_cli/commands/__init__.py
--rw-r--r--   0        0        0      920 2023-04-26 16:16:15.561454 eotdl_cli-2023.5.5/eotdl_cli/commands/auth.py
--rw-r--r--   0        0        0     1158 2023-04-26 16:16:15.561454 eotdl_cli-2023.5.5/eotdl_cli/commands/datasets.py
--rw-r--r--   0        0        0      479 2023-04-26 16:16:15.561454 eotdl_cli-2023.5.5/eotdl_cli/main.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-2023.5.5/eotdl_cli/src/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-2023.5.5/eotdl_cli/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl_cli-2023.5.5/eotdl_cli/src/errors/auth.py
--rw-r--r--   0        0        0     3471 2023-05-04 14:24:22.158984 eotdl_cli-2023.5.5/eotdl_cli/src/repos/APIRepo.py
--rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl_cli-2023.5.5/eotdl_cli/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl_cli-2023.5.5/eotdl_cli/src/repos/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/auth/main.py
--rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/datasets/DownloadDataset.py
--rw-r--r--   0        0        0      973 2023-04-26 16:16:15.561454 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/datasets/IngestDataset.py
--rw-r--r--   0        0        0      489 2023-04-11 08:30:40.657793 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
--rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
--rw-r--r--   0        0        0       69 2023-04-11 08:30:40.657793 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/datasets/__init__.py
--rw-r--r--   0        0        0     1088 2023-04-26 16:16:15.561454 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/datasets/main.py
--rw-r--r--   0        0        0      602 2023-05-05 07:50:42.076183 eotdl_cli-2023.5.5/pyproject.toml
--rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 eotdl_cli-2023.5.5/PKG-INFO
+-rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl-cli-2023.5.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl-cli-2023.5.9/eotdl_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9/eotdl_cli/commands/__init__.py
+-rw-r--r--   0        0        0      920 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9/eotdl_cli/commands/auth.py
+-rw-r--r--   0        0        0     1722 2023-05-09 10:08:45.819972 eotdl-cli-2023.5.9/eotdl_cli/commands/datasets.py
+-rw-r--r--   0        0        0      479 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9/eotdl_cli/main.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9/eotdl_cli/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9/eotdl_cli/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9/eotdl_cli/src/errors/auth.py
+-rw-r--r--   0        0        0     3953 2023-05-09 10:08:20.688084 eotdl-cli-2023.5.9/eotdl_cli/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9/eotdl_cli/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9/eotdl_cli/src/repos/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/__init__.py
+-rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      973 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0      861 2023-05-09 08:01:49.700457 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py
+-rw-r--r--   0        0        0      489 2023-04-11 08:30:40.657793 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0       91 2023-05-09 08:01:31.412351 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0     1406 2023-05-09 08:01:32.976360 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/main.py
+-rw-r--r--   0        0        0      602 2023-05-09 10:08:57.803922 eotdl-cli-2023.5.9/pyproject.toml
+-rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 eotdl-cli-2023.5.9/setup.py
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 eotdl-cli-2023.5.9/PKG-INFO
```

### Comparing `eotdl_cli-2023.5.5/eotdl_cli/commands/auth.py` & `eotdl-cli-2023.5.9/eotdl_cli/commands/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-2023.5.5/eotdl_cli/commands/datasets.py` & `eotdl-cli-2023.5.9/eotdl_cli/commands/datasets.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import typer
-from src.usecases.datasets import retrieve_datasets, download_dataset, ingest_dataset
+from src.usecases.datasets import (
+    retrieve_datasets,
+    download_dataset,
+    ingest_dataset,
+    ingest_large_dataset,
+)
 from src.usecases.auth import auth
 
 app = typer.Typer()
 
+
 @app.command()
 def list():
     """
     List all datasets
     """
     datasets = retrieve_datasets()
     typer.echo(datasets)
 
+
 @app.command()
 def get(name: str, path: str = None):
     """
     Download a dataset
 
     name: Name of the dataset
     path: Path to download the dataset to
@@ -23,27 +30,48 @@
     try:
         user = auth()
         dst_path = download_dataset(name, path, user)
         typer.echo(f"Dataset {name} downloaded to {dst_path}")
     except Exception as e:
         typer.echo(e)
 
+
+# @app.command()
+# def ingest(path: str):
+#     """
+#     Ingest a dataset
+
+#     path: Path to dataset to ingest
+#     """
+#     try:
+#         user = auth()
+#         name = typer.prompt("Dataset name")
+#         description = typer.prompt("Description")
+#         # confirm
+#         typer.confirm(f"Is the data correct?", abort=True)
+#         ingest_dataset(name, description, path, user, typer.echo)
+#         typer.echo(f"Dataset {name} ingested")
+#     except Exception as e:
+#         typer.echo(e)
+
+
 @app.command()
 def ingest(path: str):
     """
     Ingest a dataset
 
     path: Path to dataset to ingest
     """
     try:
         user = auth()
         name = typer.prompt("Dataset name")
         description = typer.prompt("Description")
         # confirm
         typer.confirm(f"Is the data correct?", abort=True)
-        ingest_dataset(name, description, path, user, typer.echo)
+        ingest_large_dataset(name, description, path, user, typer.echo)
         typer.echo(f"Dataset {name} ingested")
     except Exception as e:
         typer.echo(e)
 
+
 if __name__ == "__main__":
-    app()
+    app()
```

### Comparing `eotdl_cli-2023.5.5/eotdl_cli/src/repos/APIRepo.py` & `eotdl-cli-2023.5.9/eotdl_cli/src/repos/APIRepo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,105 @@
 import requests
 from tqdm import tqdm
 from pathlib import Path
-import os 
+import os
 
-class APIRepo():
-    def __init__(self, url=os.getenv('EOTDL_API_URL', 'https://api.eotdl.com/')):
+
+class APIRepo:
+    def __init__(self, url=os.getenv("EOTDL_API_URL", "https://api.eotdl.com/")):
         self.url = url
 
     def login(self):
-        return requests.get(self.url + 'auth/login')
-    
+        return requests.get(self.url + "auth/login")
+
     def token(self, code):
-        return requests.get(self.url + 'auth/token?code=' + code)
+        return requests.get(self.url + "auth/token?code=" + code)
 
     def logout_url(self):
-        response = requests.get(self.url + 'auth/logout')
-        return response.json()['logout_url']
-    
+        response = requests.get(self.url + "auth/logout")
+        return response.json()["logout_url"]
+
     def retrieve_datasets(self):
-        return requests.get(self.url + 'datasets').json()
+        return requests.get(self.url + "datasets").json()
 
     def retrieve_dataset(self, name):
-        return requests.get(self.url + 'datasets?name=' + name)
-    
+        return requests.get(self.url + "datasets?name=" + name)
+
     def download_dataset(self, dataset_id, id_token, path):
-        url = self.url + 'datasets/' + dataset_id + '/download'
-        headers={'Authorization': 'Bearer ' + id_token}
+        url = self.url + "datasets/" + dataset_id + "/download"
+        headers = {"Authorization": "Bearer " + id_token}
         if path is None:
-            path = str(Path.home()) + '/.etodl/datasets'
+            path = str(Path.home()) + "/.etodl/datasets"
             os.makedirs(path, exist_ok=True)
         with requests.get(url, headers=headers, stream=True) as r:
             r.raise_for_status()
-            total_size = int(r.headers.get('content-length', 0))
+            total_size = int(r.headers.get("content-length", 0))
             block_size = 1024  # 1 Kibibyte
-            progress_bar = tqdm(total=total_size, unit='iB', unit_scale=True)
-            filename = r.headers.get('content-disposition').split('filename=')[1][1:-1]
-            path = f'{path}/{filename}'
-            with open(path, 'wb') as f:
+            progress_bar = tqdm(total=total_size, unit="iB", unit_scale=True)
+            filename = r.headers.get("content-disposition").split("filename=")[1][1:-1]
+            path = f"{path}/{filename}"
+            with open(path, "wb") as f:
                 for chunk in r.iter_content(block_size):
                     progress_bar.update(len(chunk))
                     f.write(chunk)
             progress_bar.close()
             return path
-        
+
     def ingest_dataset(self, name, description, path, id_token):
         # Not sure this will work with large datasets, need to test
-        url = self.url + 'datasets'
-        headers={'Authorization': 'Bearer ' + id_token}
-        files = {'file': open(path, 'rb')}
-        data = {'name': name, 'description': description}
+        url = self.url + "datasets"
+        headers = {"Authorization": "Bearer " + id_token}
+        files = {"file": open(path, "rb")}
+        data = {"name": name, "description": description}
         response = requests.post(url, headers=headers, files=files, data=data)
         return response
 
     def read_in_chunks(self, file_object, CHUNK_SIZE):
         while True:
             data = file_object.read(CHUNK_SIZE)
             if not data:
                 break
             yield data
-    
+
     def ingest_large_dataset(self, name, description, path, id_token):
-        content_name = str(path)
         content_path = os.path.abspath(path)
-        content_size = os.stat(content_path).st_size 
+        content_size = os.stat(content_path).st_size
         file_object = open(content_path, "rb")
         index = 0
         offset = 0
         headers = {}
-        url = self.url + 'datasets/chunk'
-        data = {'name': name, 'description': description}
-        id = None
+        url = self.url + "datasets/chunk"
+        id, upload_id = None, None
         calls = 0
-        for chunk in self.read_in_chunks(file_object, 1024*1024*5):
+        data = {"name": name, "description": description}
+        chunk_size = 1024 * 1024 * 5  # 5 MiB
+        total_chunks = content_size // chunk_size
+        pbar = tqdm(self.read_in_chunks(file_object, chunk_size), total=total_chunks)
+        for chunk in pbar:
             offset = index + len(chunk)
-            headers['Content-Range'] = 'bytes %s-%s/%s' % (index, offset - 1, content_size) 
-            headers['Authorization'] = 'Bearer ' + id_token
-            index = offset 
+            headers["Content-Range"] = "bytes %s-%s/%s" % (
+                index,
+                offset - 1,
+                content_size,
+            )
+            headers["Authorization"] = "Bearer " + id_token
+            headers["Part-Number"] = str(index // chunk_size + 1)
+            if upload_id is not None:
+                headers["Upload-Id"] = upload_id
+            if id is not None:
+                headers["Dataset-Id"] = id
+            index = offset
             file = {"file": chunk}
-            if id is not None: data['id'] = id
             r = requests.post(url, files=file, headers=headers, data=data)
             if r.status_code == 200:
-                id = r.json()['id']
-                print("r: %s, Content-Range: %s" % (r, headers['Content-Range'])) 
+                r_data = r.json()
+                id, upload_id = r_data["id"], r_data["upload_id"]
             else:
                 break
             calls += 1
-            # if calls >= 3: break
+            pbar.set_description(
+                "{:.2f}/{:.2f} MB".format(
+                    offset / 1024 / 1024, content_size / 1024 / 1024
+                )
+            )
+        pbar.close()
         return r
-
-
-
```

### Comparing `eotdl_cli-2023.5.5/eotdl_cli/src/repos/AuthRepo.py` & `eotdl-cli-2023.5.9/eotdl_cli/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-2023.5.5/eotdl_cli/src/usecases/auth/Auth.py` & `eotdl-cli-2023.5.9/eotdl_cli/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-2023.5.5/eotdl_cli/src/usecases/auth/main.py` & `eotdl-cli-2023.5.9/eotdl_cli/src/usecases/auth/main.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-2023.5.5/eotdl_cli/src/usecases/datasets/IngestDataset.py` & `eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/IngestDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-2023.5.5/eotdl_cli/src/usecases/datasets/main.py` & `eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ...repos import APIRepo
 from .RetrieveDatasets import RetrieveDatasets
 from .RetrieveDataset import RetrieveDataset
 from .DownloadDataset import DownloadDataset
 from .IngestDataset import IngestDataset
+from .IngestLargeDataset import IngestLargeDataset
 
 def retrieve_datasets():
     api_repo = APIRepo()
     retrieve = RetrieveDatasets(api_repo)
     inputs = retrieve.Inputs()
     outputs = retrieve(inputs)
     return outputs.datasets
@@ -27,8 +28,15 @@
 	return outputs.dst_path
 
 def ingest_dataset(name, description, path, user, logger):
 	api_repo = APIRepo()
 	ingest = IngestDataset(api_repo, logger)
 	inputs = ingest.Inputs(name=name, description=description, path=path, user=user)
 	outputs = ingest(inputs)
+	return outputs.dataset
+
+def ingest_large_dataset(name, description, path, user, logger):
+	api_repo = APIRepo()
+	ingest = IngestLargeDataset(api_repo, logger)
+	inputs = ingest.Inputs(name=name, description=description, path=path, user=user)
+	outputs = ingest(inputs)
 	return outputs.dataset
```

### Comparing `eotdl_cli-2023.5.5/pyproject.toml` & `eotdl-cli-2023.5.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl-cli"
-version = "2023.05.05"
+version = "2023.05.09"
 description = ""
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl_cli"}]
 
 [tool.poetry.scripts]
```

### Comparing `eotdl_cli-2023.5.5/PKG-INFO` & `eotdl-cli-2023.5.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: eotdl-cli
-Version: 2023.5.5
+Version: 2023.5.9
 Summary: 
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
```

