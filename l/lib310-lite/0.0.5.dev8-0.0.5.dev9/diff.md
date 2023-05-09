# Comparing `tmp/lib310_lite-0.0.5.dev8.tar.gz` & `tmp/lib310_lite-0.0.5.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.0.5.dev8.tar", max compression
+gzip compressed data, was "lib310_lite-0.0.5.dev9.tar", max compression
```

## Comparing `lib310_lite-0.0.5.dev8.tar` & `lib310_lite-0.0.5.dev9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.5.dev8/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.5.dev8/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7467 2023-05-08 08:51:40.656605 lib310_lite-0.0.5.dev8/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.5.dev8/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.5.dev8/lib310_lite/fucntion.py
--rw-r--r--   0        0        0     8950 2023-05-09 09:53:04.351939 lib310_lite-0.0.5.dev8/lib310_lite/mldl/mldl.py
--rw-r--r--   0        0        0      843 2023-05-08 09:08:49.952690 lib310_lite-0.0.5.dev8/lib310_lite/mldl/models/InteractionModel.py
--rw-r--r--   0        0        0     2102 2023-05-08 09:07:24.596219 lib310_lite-0.0.5.dev8/lib310_lite/mldl/models/SeqLangModel.py
--rw-r--r--   0        0        0      804 2023-05-09 09:53:27.494691 lib310_lite-0.0.5.dev8/pyproject.toml
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev8/setup.py
--rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev8/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.5.dev9/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.5.dev9/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7467 2023-05-08 08:51:40.656605 lib310_lite-0.0.5.dev9/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.5.dev9/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.5.dev9/lib310_lite/fucntion.py
+-rw-r--r--   0        0        0     8811 2023-05-09 09:58:45.500468 lib310_lite-0.0.5.dev9/lib310_lite/mldl/mldl.py
+-rw-r--r--   0        0        0      843 2023-05-08 09:08:49.952690 lib310_lite-0.0.5.dev9/lib310_lite/mldl/models/InteractionModel.py
+-rw-r--r--   0        0        0     2102 2023-05-08 09:07:24.596219 lib310_lite-0.0.5.dev9/lib310_lite/mldl/models/SeqLangModel.py
+-rw-r--r--   0        0        0      804 2023-05-09 09:58:59.887220 lib310_lite-0.0.5.dev9/pyproject.toml
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev9/setup.py
+-rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev9/PKG-INFO
```

### Comparing `lib310_lite-0.0.5.dev8/lib310_lite/bigquery/client.py` & `lib310_lite-0.0.5.dev9/lib310_lite/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5.dev8/lib310_lite/bigquery/constants.py` & `lib310_lite-0.0.5.dev9/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5.dev8/lib310_lite/mldl/mldl.py` & `lib310_lite-0.0.5.dev9/lib310_lite/mldl/mldl.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     __VAL = 'VAL'
     __MAIN = 'MAIN'
     __INTERACTION = 'INTERACTION'
     __PARTS = {__INTERACTION: 1}
 
     def __init__(self, db_url: str, cache_size: int = 50, num_threads: int = 10, random_seed: int = time.time()):
         random.seed(random_seed)
-        self.engine = create_engine(db_url, pool_size=2 * num_threads + 1, max_overflow=num_threads * 3 + 1)
+        self.engine = create_engine(db_url, pool_size=3 * (num_threads + 1), max_overflow=4 * (num_threads + 1))
         self.Session = sessionmaker(bind=self.engine)
 
         self.bq_client = BigQueryClient()
 
         # this is the pool of samples row_id
         self.sample_cache = []
         # this is the maximum number of requests we fetch sooner from the database
@@ -138,15 +138,15 @@
         if parts is None:
             parts = MLDL.__PARTS
         try:
             # get random row_id from the pool
             index_list = random.sample(self.sample_cache, min(num, len(self.sample_cache)))
 
             with concurrent.futures.ThreadPoolExecutor() as executor:
-                main_thread = executor.submit(self.fetch_sample_main, index_list, stage, parts)
+                main_thread = executor.submit(self.fetch_sample_main, index_list, parts)
                 if parts[MLDL.__INTERACTION] and parts[MLDL.__INTERACTION] == 1:
                     interaction_thread = executor.submit(self.fetch_sample_interaction, index_list)
 
                 main_df = main_thread.result()
 
                 interaction_df = pd.DataFrame()
                 if parts[MLDL.__INTERACTION] and parts[MLDL.__INTERACTION] == 1:
@@ -168,19 +168,18 @@
                 time.sleep(retry * 10)
             retry += 1
             print(f'Cannot fetch data from database, retry number {retry} times')
             if retry > 7:
                 raise Exception('Cannot fetch data from database')
             return self.fetch_sample(num, stage, parts, retry)
 
-    def fetch_sample_main(self, index_list: list, stage: str, parts: dict = None):
+    def fetch_sample_main(self, index_list: list, parts: dict = None):
         """
         This function is used to fetch the main data from the database
         :param index_list: list of row_ids
-        :param stage: stage of the data
         :param parts: parts of the data
         :return: dataframe of main data
         """
         session = self.Session()
         if parts is None:
             parts = MLDL.__PARTS
         try:
@@ -189,19 +188,18 @@
         except Exception as e:
             print(e)
             raise Exception('Cannot fetch data from database <SeqLang>')
         finally:
             session.close()
         return df
 
-    def fetch_sample_interaction(self, index_list: list, session):
+    def fetch_sample_interaction(self, index_list: list):
         """
         This function is used to fetch the interaction data from the database
         :param index_list: list of row_ids
-        :param session: the session that we use to connect to the database
         :return: dataframe of interaction data
         """
         session = self.Session()
         try:
             results = session.query(InteractionModel).filter(InteractionModel.row_id.in_(index_list)).all()
             df = pd.DataFrame([r.to_dict() for r in results])
         except Exception as e:
```

### Comparing `lib310_lite-0.0.5.dev8/lib310_lite/mldl/models/InteractionModel.py` & `lib310_lite-0.0.5.dev9/lib310_lite/mldl/models/InteractionModel.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5.dev8/lib310_lite/mldl/models/SeqLangModel.py` & `lib310_lite-0.0.5.dev9/lib310_lite/mldl/models/SeqLangModel.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5.dev8/pyproject.toml` & `lib310_lite-0.0.5.dev9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.0.5.dev8"
+version = "0.0.5.dev9"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
```

### Comparing `lib310_lite-0.0.5.dev8/setup.py` & `lib310_lite-0.0.5.dev9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
  'numpy<1.23.0',
  'psycopg2-binary>=2.9.0']
 
 setup_kwargs = {
     'name': 'lib310-lite',
-    'version': '0.0.5.dev8',
+    'version': '0.0.5.dev9',
     'description': 'lib310 Lite Python Package',
     'long_description': 'None',
     'author': '310',
     'author_email': 'info@310.ai',
     'maintainer': 'Saman Fekri',
     'maintainer_email': 'saman@310.ai',
     'url': 'None',
```

### Comparing `lib310_lite-0.0.5.dev8/PKG-INFO` & `lib310_lite-0.0.5.dev9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.0.5.dev8
+Version: 0.0.5.dev9
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
```

