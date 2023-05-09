# Comparing `tmp/lib310_lite-0.0.5.dev7.tar.gz` & `tmp/lib310_lite-0.0.5.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.0.5.dev7.tar", max compression
+gzip compressed data, was "lib310_lite-0.0.5.dev8.tar", max compression
```

## Comparing `lib310_lite-0.0.5.dev7.tar` & `lib310_lite-0.0.5.dev8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.5.dev7/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.5.dev7/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7467 2023-05-08 08:51:40.656605 lib310_lite-0.0.5.dev7/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.5.dev7/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.5.dev7/lib310_lite/fucntion.py
--rw-r--r--   0        0        0     9032 2023-05-09 09:50:52.151901 lib310_lite-0.0.5.dev7/lib310_lite/mldl/mldl.py
--rw-r--r--   0        0        0      843 2023-05-08 09:08:49.952690 lib310_lite-0.0.5.dev7/lib310_lite/mldl/models/InteractionModel.py
--rw-r--r--   0        0        0     2102 2023-05-08 09:07:24.596219 lib310_lite-0.0.5.dev7/lib310_lite/mldl/models/SeqLangModel.py
--rw-r--r--   0        0        0      804 2023-05-09 09:50:52.149397 lib310_lite-0.0.5.dev7/pyproject.toml
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev7/setup.py
--rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev7/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.5.dev8/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.5.dev8/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7467 2023-05-08 08:51:40.656605 lib310_lite-0.0.5.dev8/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.5.dev8/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.5.dev8/lib310_lite/fucntion.py
+-rw-r--r--   0        0        0     8950 2023-05-09 09:53:04.351939 lib310_lite-0.0.5.dev8/lib310_lite/mldl/mldl.py
+-rw-r--r--   0        0        0      843 2023-05-08 09:08:49.952690 lib310_lite-0.0.5.dev8/lib310_lite/mldl/models/InteractionModel.py
+-rw-r--r--   0        0        0     2102 2023-05-08 09:07:24.596219 lib310_lite-0.0.5.dev8/lib310_lite/mldl/models/SeqLangModel.py
+-rw-r--r--   0        0        0      804 2023-05-09 09:53:27.494691 lib310_lite-0.0.5.dev8/pyproject.toml
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev8/setup.py
+-rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 lib310_lite-0.0.5.dev8/PKG-INFO
```

### Comparing `lib310_lite-0.0.5.dev7/lib310_lite/bigquery/client.py` & `lib310_lite-0.0.5.dev8/lib310_lite/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5.dev7/lib310_lite/bigquery/constants.py` & `lib310_lite-0.0.5.dev8/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5.dev7/lib310_lite/mldl/mldl.py` & `lib310_lite-0.0.5.dev8/lib310_lite/mldl/mldl.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,26 +130,25 @@
         Run two threads to fetch the data from the database
         :param num: number of samples
         :param stage: TRAIN or TEST or VAL or any other stage
         :param parts: the parts of the data that we want to fetch
         :param retry: number of retries max is constant 7
         :return: dataframe of the data
         """
-        session = self.Session()
 
         if parts is None:
             parts = MLDL.__PARTS
         try:
             # get random row_id from the pool
             index_list = random.sample(self.sample_cache, min(num, len(self.sample_cache)))
 
             with concurrent.futures.ThreadPoolExecutor() as executor:
-                main_thread = executor.submit(self.fetch_sample_main, index_list, stage, session, parts)
+                main_thread = executor.submit(self.fetch_sample_main, index_list, stage, parts)
                 if parts[MLDL.__INTERACTION] and parts[MLDL.__INTERACTION] == 1:
-                    interaction_thread = executor.submit(self.fetch_sample_interaction, index_list, session)
+                    interaction_thread = executor.submit(self.fetch_sample_interaction, index_list)
 
                 main_df = main_thread.result()
 
                 interaction_df = pd.DataFrame()
                 if parts[MLDL.__INTERACTION] and parts[MLDL.__INTERACTION] == 1:
                     interaction_df = interaction_thread.result()
 
@@ -168,51 +167,52 @@
             else:
                 time.sleep(retry * 10)
             retry += 1
             print(f'Cannot fetch data from database, retry number {retry} times')
             if retry > 7:
                 raise Exception('Cannot fetch data from database')
             return self.fetch_sample(num, stage, parts, retry)
-        finally:
-            print('2')
-            session.close()
 
-    def fetch_sample_main(self, index_list: list, stage: str, session, parts: dict = None):
+    def fetch_sample_main(self, index_list: list, stage: str, parts: dict = None):
         """
         This function is used to fetch the main data from the database
         :param index_list: list of row_ids
         :param stage: stage of the data
-        :param session: the session that we use to connect to the database
         :param parts: parts of the data
         :return: dataframe of main data
         """
-        # session = self.Session()
+        session = self.Session()
         if parts is None:
             parts = MLDL.__PARTS
         try:
             results = session.query(SeqLangModel).filter(SeqLangModel.row_id.in_(index_list)).all()
             df = pd.DataFrame([r.to_dict() for r in results])
         except Exception as e:
             print(e)
             raise Exception('Cannot fetch data from database <SeqLang>')
+        finally:
+            session.close()
         return df
 
     def fetch_sample_interaction(self, index_list: list, session):
         """
         This function is used to fetch the interaction data from the database
         :param index_list: list of row_ids
         :param session: the session that we use to connect to the database
         :return: dataframe of interaction data
         """
+        session = self.Session()
         try:
             results = session.query(InteractionModel).filter(InteractionModel.row_id.in_(index_list)).all()
             df = pd.DataFrame([r.to_dict() for r in results])
         except Exception as e:
             print(e)
             raise Exception('Cannot fetch data from database <Interaction>')
+        finally:
+            session.close()
         return df
 
     def terminate(self):
         """
         Terminate the filler threads and clear the queue
         """
         # Terminate the filler thread
```

### Comparing `lib310_lite-0.0.5.dev7/lib310_lite/mldl/models/InteractionModel.py` & `lib310_lite-0.0.5.dev8/lib310_lite/mldl/models/InteractionModel.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5.dev7/lib310_lite/mldl/models/SeqLangModel.py` & `lib310_lite-0.0.5.dev8/lib310_lite/mldl/models/SeqLangModel.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.5.dev7/pyproject.toml` & `lib310_lite-0.0.5.dev8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.0.5.dev7"
+version = "0.0.5.dev8"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
```

### Comparing `lib310_lite-0.0.5.dev7/setup.py` & `lib310_lite-0.0.5.dev8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
  'numpy<1.23.0',
  'psycopg2-binary>=2.9.0']
 
 setup_kwargs = {
     'name': 'lib310-lite',
-    'version': '0.0.5.dev7',
+    'version': '0.0.5.dev8',
     'description': 'lib310 Lite Python Package',
     'long_description': 'None',
     'author': '310',
     'author_email': 'info@310.ai',
     'maintainer': 'Saman Fekri',
     'maintainer_email': 'saman@310.ai',
     'url': 'None',
```

### Comparing `lib310_lite-0.0.5.dev7/PKG-INFO` & `lib310_lite-0.0.5.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.0.5.dev7
+Version: 0.0.5.dev8
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
```

