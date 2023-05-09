# Comparing `tmp/lib310_lite-0.0.5.dev3.tar.gz` & `tmp/lib310_lite-0.0.5.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.0.5.dev3.tar", max compression
+gzip compressed data, was "lib310_lite-0.0.5.dev4.tar", max compression
```

## Comparing `lib310_lite-0.0.5.dev3.tar` & `lib310_lite-0.0.5.dev4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.5.dev3/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.5.dev3/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7467 2023-05-08 08:51:40.656605 lib310_lite-0.0.5.dev3/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.5.dev3/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.5.dev3/lib310_lite/fucntion.py
--rw-r--r--   0        0        0     9850 2023-05-08 16:05:00.621832 lib310_lite-0.0.5.dev3/lib310_lite/mldl/mldl.py
--rw-r--r--   0        0        0      843 2023-05-08 09:08:49.952690 lib310_lite-0.0.5.dev3/lib310_lite/mldl/models/InteractionModel.py
--rw-r--r--   0        0        0     2102 2023-05-08 09:07:24.596219 lib310_lite-0.0.5.dev3/lib310_lite/mldl/models/SeqLangModel.py
--rw-r--r--   0        0        0      804 2023-05-08 16:05:20.583342 lib310_lite-0.0.5.dev3/pyproject.toml
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev3/setup.py
--rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev3/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.5.dev4/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.5.dev4/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7467 2023-05-08 08:51:40.656605 lib310_lite-0.0.5.dev4/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.5.dev4/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.5.dev4/lib310_lite/fucntion.py
+-rw-r--r--   0        0        0     9142 2023-05-09 09:04:57.558068 lib310_lite-0.0.5.dev4/lib310_lite/mldl/mldl.py
+-rw-r--r--   0        0        0      843 2023-05-08 09:08:49.952690 lib310_lite-0.0.5.dev4/lib310_lite/mldl/models/InteractionModel.py
+-rw-r--r--   0        0        0     2102 2023-05-08 09:07:24.596219 lib310_lite-0.0.5.dev4/lib310_lite/mldl/models/SeqLangModel.py
+-rw-r--r--   0        0        0      804 2023-05-09 09:04:57.550549 lib310_lite-0.0.5.dev4/pyproject.toml
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev4/setup.py
+-rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev4/PKG-INFO
```

### Comparing `lib310_lite-0.0.5.dev3/lib310_lite/bigquery/client.py` & `lib310_lite-0.0.5.dev4/lib310_lite/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5.dev3/lib310_lite/bigquery/constants.py` & `lib310_lite-0.0.5.dev4/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5.dev3/lib310_lite/mldl/mldl.py` & `lib310_lite-0.0.5.dev4/lib310_lite/mldl/mldl.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,29 +24,20 @@
     __VAL = 'VAL'
     __MAIN = 'MAIN'
     __INTERACTION = 'INTERACTION'
     __PARTS = {__INTERACTION: 1}
 
     def __init__(self, db_url: str, cache_size: int = 50, num_threads: int = 10, random_seed: int = time.time()):
         random.seed(random_seed)
-        self.engine = create_engine(db_url, pool_size=num_threads + 1, max_overflow=num_threads*2)
+        self.engine = create_engine(db_url, pool_size=2 * num_threads + 1, max_overflow=num_threads * 3 + 1)
         self.Session = sessionmaker(bind=self.engine)
 
         self.bq_client = BigQueryClient()
 
-        # self.collections = {
-        #     MLDL.__TRAIN: {
-        #         MLDL.__MAIN: self.db['seq_lang5_copy'],
-        #         MLDL.__INTERACTION: self.db['interactions_lang5_train'],
-        #     },
-        #     MLDL.__TEST: {
-        #         MLDL.__MAIN: self.db['seq_lang5_copy'],
-        #         MLDL.__INTERACTION: self.db['interactions_lang5_test'],
-        #     }
-        # }
+        self.session = self.Session()
 
         # this is the pool of samples row_id
         self.sample_cache = []
         # this is the maximum number of requests we fetch sooner from the database
         self.max_queue_size = cache_size
         # this is the number of threads we use to fetch data from the database
         self.num_threads = num_threads
@@ -71,20 +62,14 @@
         :param max_length: maximum length of the sequence
         :param min_num_feature: minimum number of features
         :param stage: TRAIN or TEST
         :param parts: the parts of the data that we want to fetch
         :return: a pandas dataframe
         """
         stage = stage.upper()
-        # if stage == MLDL.__TRAIN:
-        #     col = self.collections[MLDL.__TRAIN]
-        # elif stage == MLDL.__TEST:
-        #     col = self.collections[MLDL.__TEST]
-        # else:
-        #     raise ValueError('Stage must be either TRAIN or TEST')
 
         if parts is None:
             parts = MLDL.__PARTS
 
         hit = self.queue_key == f'{num}_{max_length}_{min_num_feature}_{stage}'
         if hit:
             # HIT
@@ -113,18 +98,18 @@
 
         # generate new key
         self.queue_key = f'{num}_{max_length}_{min_num_feature}_{stage}'
 
         # start new thread
         self.filler_thread = Thread(target=self.filler, args=(num, stage, parts))
         self.filler_thread.start()
-        time.sleep(3)
-        session = self.Session()
-        r = self.fetch_sample(num, stage, session, parts)
-        session.close()
+
+        # session = self.Session()
+        r = self.fetch_sample(num, stage, self.session, parts)
+        # session.close()
         return r
 
     def filler(self, num: int, stage: str, parts: dict = None):
         """
         This function is used to fill the queue with data then get batch read data from the queue
         :param num: number of samples
         :param stage: TRAIN or TEST
@@ -136,20 +121,20 @@
             while not self.kill_event.is_set():
                 executor.submit(self.filler_worker, num, stage, parts)
             while not self.queue.empty():
                 self.queue.get()
             executor.shutdown(wait=True)
 
     def filler_worker(self, num: int, stage: str, parts: dict = None):
-        session = self.Session()
+
         if parts is None:
             parts = MLDL.__PARTS
-        df = self.fetch_sample(num, stage, session, parts)
+        df = self.fetch_sample(num, stage, self.session, parts)
         self.queue.put(df)
-        session.close()
+
         return
 
     def fetch_sample(self, num: int, stage: str, session, parts: dict = None):
         """
         This function is used to fetch the data from the database
         Run two threads to fetch the data from the database
         :param num: number of samples
@@ -216,15 +201,14 @@
     def fetch_sample_interaction(self, index_list: list, session):
         """
         This function is used to fetch the interaction data from the database
         :param index_list: list of row_ids
         :param session: the session that we use to connect to the database
         :return: dataframe of interaction data
         """
-        # session = self.Session()
         try:
             results = session.query(InteractionModel).filter(InteractionModel.row_id.in_(index_list)).all()
             df = pd.DataFrame([r.to_dict() for r in results])
         except Exception as e:
             print(e)
             raise Exception('Cannot fetch data from database <Interaction>')
         return df
```

### Comparing `lib310_lite-0.0.5.dev3/lib310_lite/mldl/models/InteractionModel.py` & `lib310_lite-0.0.5.dev4/lib310_lite/mldl/models/InteractionModel.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5.dev3/lib310_lite/mldl/models/SeqLangModel.py` & `lib310_lite-0.0.5.dev4/lib310_lite/mldl/models/SeqLangModel.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5.dev3/pyproject.toml` & `lib310_lite-0.0.5.dev4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.0.5.dev3"
+version = "0.0.5.dev4"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
```

### Comparing `lib310_lite-0.0.5.dev3/setup.py` & `lib310_lite-0.0.5.dev4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
  'numpy<1.23.0',
  'psycopg2-binary>=2.9.0']
 
 setup_kwargs = {
     'name': 'lib310-lite',
-    'version': '0.0.5.dev3',
+    'version': '0.0.5.dev4',
     'description': 'lib310 Lite Python Package',
     'long_description': 'None',
     'author': '310',
     'author_email': 'info@310.ai',
     'maintainer': 'Saman Fekri',
     'maintainer_email': 'saman@310.ai',
     'url': 'None',
```

### Comparing `lib310_lite-0.0.5.dev3/PKG-INFO` & `lib310_lite-0.0.5.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.0.5.dev3
+Version: 0.0.5.dev4
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
```

