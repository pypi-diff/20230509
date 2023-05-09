# Comparing `tmp/eotdl-cli-2023.5.9.tar.gz` & `tmp/eotdl-cli-2023.5.9.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl-cli-2023.5.9.tar", max compression
+gzip compressed data, was "eotdl-cli-2023.5.9.post2.tar", max compression
```

## Comparing `eotdl-cli-2023.5.9.tar` & `eotdl-cli-2023.5.9.post2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl-cli-2023.5.9/README.md
--rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl-cli-2023.5.9/eotdl_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9/eotdl_cli/commands/__init__.py
--rw-r--r--   0        0        0      920 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9/eotdl_cli/commands/auth.py
--rw-r--r--   0        0        0     1722 2023-05-09 10:08:45.819972 eotdl-cli-2023.5.9/eotdl_cli/commands/datasets.py
--rw-r--r--   0        0        0      479 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9/eotdl_cli/main.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9/eotdl_cli/src/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9/eotdl_cli/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9/eotdl_cli/src/errors/auth.py
--rw-r--r--   0        0        0     3953 2023-05-09 10:08:20.688084 eotdl-cli-2023.5.9/eotdl_cli/src/repos/APIRepo.py
--rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9/eotdl_cli/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9/eotdl_cli/src/repos/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/auth/main.py
--rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/DownloadDataset.py
--rw-r--r--   0        0        0      973 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/IngestDataset.py
--rw-r--r--   0        0        0      861 2023-05-09 08:01:49.700457 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py
--rw-r--r--   0        0        0      489 2023-04-11 08:30:40.657793 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
--rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
--rw-r--r--   0        0        0       91 2023-05-09 08:01:31.412351 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/__init__.py
--rw-r--r--   0        0        0     1406 2023-05-09 08:01:32.976360 eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/main.py
--rw-r--r--   0        0        0      602 2023-05-09 10:08:57.803922 eotdl-cli-2023.5.9/pyproject.toml
--rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 eotdl-cli-2023.5.9/setup.py
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 eotdl-cli-2023.5.9/PKG-INFO
+-rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl-cli-2023.5.9.post2/README.md
+-rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl-cli-2023.5.9.post2/eotdl_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post2/eotdl_cli/commands/__init__.py
+-rw-r--r--   0        0        0      920 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9.post2/eotdl_cli/commands/auth.py
+-rw-r--r--   0        0        0     1878 2023-05-09 13:11:13.605365 eotdl-cli-2023.5.9.post2/eotdl_cli/commands/datasets.py
+-rw-r--r--   0        0        0      479 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9.post2/eotdl_cli/main.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post2/eotdl_cli/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post2/eotdl_cli/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post2/eotdl_cli/src/errors/auth.py
+-rw-r--r--   0        0        0     5860 2023-05-09 13:06:29.128630 eotdl-cli-2023.5.9.post2/eotdl_cli/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post2/eotdl_cli/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post2/eotdl_cli/src/repos/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/__init__.py
+-rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      973 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0      861 2023-05-09 08:01:49.700457 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py
+-rw-r--r--   0        0        0      489 2023-04-11 08:30:40.657793 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0       91 2023-05-09 08:01:31.412351 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0     1406 2023-05-09 08:01:32.976360 eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/main.py
+-rw-r--r--   0        0        0      604 2023-05-09 13:13:17.081716 eotdl-cli-2023.5.9.post2/pyproject.toml
+-rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 eotdl-cli-2023.5.9.post2/setup.py
+-rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 eotdl-cli-2023.5.9.post2/PKG-INFO
```

### Comparing `eotdl-cli-2023.5.9/eotdl_cli/commands/auth.py` & `eotdl-cli-2023.5.9.post2/eotdl_cli/commands/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9/eotdl_cli/commands/datasets.py` & `eotdl-cli-2023.5.9.post2/eotdl_cli/commands/datasets.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from src.usecases.datasets import (
     retrieve_datasets,
     download_dataset,
     ingest_dataset,
     ingest_large_dataset,
 )
 from src.usecases.auth import auth
+from typing import Optional
 
 app = typer.Typer()
 
 
 @app.command()
 def list():
     """
@@ -51,26 +52,32 @@
 #         ingest_dataset(name, description, path, user, typer.echo)
 #         typer.echo(f"Dataset {name} ingested")
 #     except Exception as e:
 #         typer.echo(e)
 
 
 @app.command()
-def ingest(path: str):
+def ingest(
+    path: str,
+    n: Optional[str] = None,
+    d: Optional[str] = None,
+    y: Optional[bool] = False,
+):
     """
     Ingest a dataset
 
     path: Path to dataset to ingest
     """
     try:
         user = auth()
-        name = typer.prompt("Dataset name")
-        description = typer.prompt("Description")
+        name = n or typer.prompt("Dataset name")
+        description = d or typer.prompt("Description")
         # confirm
-        typer.confirm(f"Is the data correct?", abort=True)
+        if not y:
+            typer.confirm(f"Is the data correct?", abort=True)
         ingest_large_dataset(name, description, path, user, typer.echo)
         typer.echo(f"Dataset {name} ingested")
     except Exception as e:
         typer.echo(e)
 
 
 if __name__ == "__main__":
```

### Comparing `eotdl-cli-2023.5.9/eotdl_cli/src/repos/APIRepo.py` & `eotdl-cli-2023.5.9.post2/eotdl_cli/src/repos/APIRepo.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import requests
 from tqdm import tqdm
 from pathlib import Path
 import os
+from concurrent.futures import ThreadPoolExecutor
+import time
 
 
 class APIRepo:
     def __init__(self, url=os.getenv("EOTDL_API_URL", "https://api.eotdl.com/")):
         self.url = url
 
     def login(self):
@@ -56,50 +58,96 @@
     def read_in_chunks(self, file_object, CHUNK_SIZE):
         while True:
             data = file_object.read(CHUNK_SIZE)
             if not data:
                 break
             yield data
 
+    def parallel_upload(
+        self, content_size, chunk_size, content_path, url, headers, total_chunks
+    ):
+        # Create thread pool executor
+        executor = ThreadPoolExecutor(max_workers=4)
+
+        # Divide file into chunks and create tasks for each chunk
+        offset = 0
+        tasks = []
+        while offset < content_size:
+            chunk_end = min(offset + chunk_size, content_size)
+            tasks.append((offset, chunk_end, str(offset // chunk_size + 1)))
+            offset = chunk_end
+
+        # Define the function that will upload each chunk
+        def upload_chunk(start, end, part):
+            # print(f"Uploading chunk {start} - {end}", part)
+            with open(content_path, "rb") as f:
+                f.seek(start)
+                chunk = f.read(end - start)
+            headers["Part-Number"] = part
+            response = requests.post(url, files={"file": chunk}, headers=headers)
+            if response.status_code != 200:
+                print(f"Failed to upload chunk {start} - {end}")
+            return response
+
+        # Submit each task to the executor
+        with tqdm(total=total_chunks) as pbar:
+            futures = []
+            for task in tasks:
+                future = executor.submit(upload_chunk, *task)
+                future.add_done_callback(lambda p: pbar.update())
+                futures.append(future)
+
+            # Wait for all tasks to complete
+            for future in futures:
+                future.result()
+
     def ingest_large_dataset(self, name, description, path, id_token):
+        # first call to get upload id
+        url = self.url + "datasets/chunk?name=" + name + "&description=" + description
+        headers = {"Authorization": "Bearer " + id_token}
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            return response
+        data = response.json()
+        dataset_id, upload_id = data["dataset_id"], data["upload_id"]
+
+        # upload chunks in parallel
         content_path = os.path.abspath(path)
         content_size = os.stat(content_path).st_size
         file_object = open(content_path, "rb")
         index = 0
         offset = 0
-        headers = {}
+        headers["Upload-Id"] = upload_id
+        headers["Dataset-Id"] = dataset_id
         url = self.url + "datasets/chunk"
-        id, upload_id = None, None
-        calls = 0
-        data = {"name": name, "description": description}
         chunk_size = 1024 * 1024 * 5  # 5 MiB
         total_chunks = content_size // chunk_size
+
+        # parallel upload not working so well, the api cannot handle it...
+        # self.parallel_upload(
+        #     content_size, chunk_size, content_path, url, headers, total_chunks
+        # )
+
+        # upload chunks sequentially
         pbar = tqdm(self.read_in_chunks(file_object, chunk_size), total=total_chunks)
         for chunk in pbar:
             offset = index + len(chunk)
-            headers["Content-Range"] = "bytes %s-%s/%s" % (
-                index,
-                offset - 1,
-                content_size,
-            )
-            headers["Authorization"] = "Bearer " + id_token
             headers["Part-Number"] = str(index // chunk_size + 1)
-            if upload_id is not None:
-                headers["Upload-Id"] = upload_id
-            if id is not None:
-                headers["Dataset-Id"] = id
             index = offset
             file = {"file": chunk}
-            r = requests.post(url, files=file, headers=headers, data=data)
-            if r.status_code == 200:
-                r_data = r.json()
-                id, upload_id = r_data["id"], r_data["upload_id"]
-            else:
-                break
-            calls += 1
+            r = requests.post(url, files=file, headers=headers)
+            if r.status_code != 200:
+                return r.json()["detail"]
             pbar.set_description(
                 "{:.2f}/{:.2f} MB".format(
                     offset / 1024 / 1024, content_size / 1024 / 1024
                 )
             )
         pbar.close()
+
+        # complete upload
+        url = self.url + "datasets/complete"
+        del headers["Part-Number"]
+        r = requests.post(
+            url, json={"name": name, "description": description}, headers=headers
+        )
         return r
```

### Comparing `eotdl-cli-2023.5.9/eotdl_cli/src/repos/AuthRepo.py` & `eotdl-cli-2023.5.9.post2/eotdl_cli/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9/eotdl_cli/src/usecases/auth/Auth.py` & `eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9/eotdl_cli/src/usecases/auth/main.py` & `eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/auth/main.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/IngestDataset.py` & `eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/IngestDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py` & `eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9/eotdl_cli/src/usecases/datasets/main.py` & `eotdl-cli-2023.5.9.post2/eotdl_cli/src/usecases/datasets/main.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9/pyproject.toml` & `eotdl-cli-2023.5.9.post2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl-cli"
-version = "2023.05.09"
+version = "2023.05.09-2"
 description = ""
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl_cli"}]
 
 [tool.poetry.scripts]
```

### Comparing `eotdl-cli-2023.5.9/setup.py` & `eotdl-cli-2023.5.9.post2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['eotdl-cli = eotdl_cli.main:app']}
 
 setup_kwargs = {
     'name': 'eotdl-cli',
-    'version': '2023.5.9',
+    'version': '2023.5.9.post2',
     'description': '',
     'long_description': '# eotdl-cli\n\nThis is the CLI for EOTDL.\n\n',
     'author': 'EarthPulse',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `eotdl-cli-2023.5.9/PKG-INFO` & `eotdl-cli-2023.5.9.post2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotdl-cli
-Version: 2023.5.9
+Version: 2023.5.9.post2
 Summary: 
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

