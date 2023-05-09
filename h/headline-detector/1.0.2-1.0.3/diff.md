# Comparing `tmp/headline_detector-1.0.2.tar.gz` & `tmp/headline_detector-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headline_detector-1.0.2.tar", last modified: Thu May  4 08:25:52 2023, max compression
+gzip compressed data, was "headline_detector-1.0.3.tar", last modified: Tue May  9 10:18:05 2023, max compression
```

## Comparing `headline_detector-1.0.2.tar` & `headline_detector-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 08:25:52.850201 headline_detector-1.0.2/
--rw-rw-rw-   0        0        0     2729 2023-05-04 08:25:52.849202 headline_detector-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2418 2023-05-02 12:37:59.000000 headline_detector-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-04 08:25:52.850201 headline_detector-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      781 2023-05-04 08:25:35.000000 headline_detector-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 08:25:52.821200 headline_detector-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-04 08:25:52.830201 headline_detector-1.0.2/src/headline_detector/
--rw-rw-rw-   0        0        0       93 2023-05-02 12:00:22.000000 headline_detector-1.0.2/src/headline_detector/__init__.py
--rw-rw-rw-   0        0        0     7773 2023-05-02 12:00:50.000000 headline_detector-1.0.2/src/headline_detector/detector.py
--rw-rw-rw-   0        0        0      498 2023-05-02 09:35:48.000000 headline_detector-1.0.2/src/headline_detector/hyper_params.py
--rw-rw-rw-   0        0        0     5241 2023-05-02 11:58:36.000000 headline_detector-1.0.2/src/headline_detector/model.py
--rw-rw-rw-   0        0        0     1407 2023-05-02 09:47:20.000000 headline_detector-1.0.2/src/headline_detector/model_checkpoint.py
--rw-rw-rw-   0        0        0     1395 2023-05-04 08:22:17.000000 headline_detector-1.0.2/src/headline_detector/preprocessing_scenario.py
-drwxrwxrwx   0        0        0        0 2023-05-04 08:25:52.848200 headline_detector-1.0.2/src/headline_detector/processing_pipeline/
--rw-rw-rw-   0        0        0      142 2023-05-02 11:08:45.000000 headline_detector-1.0.2/src/headline_detector/processing_pipeline/__init__.py
--rw-rw-rw-   0        0        0     1758 2023-05-02 11:32:18.000000 headline_detector-1.0.2/src/headline_detector/processing_pipeline/pipeline.py
--rw-rw-rw-   0        0        0     2256 2023-05-02 11:07:28.000000 headline_detector-1.0.2/src/headline_detector/processing_pipeline/processing_func.py
--rw-rw-rw-   0        0        0     2821 2023-05-02 11:07:12.000000 headline_detector-1.0.2/src/headline_detector/processing_pipeline/stemmer.py
--rw-rw-rw-   0        0        0      202 2023-05-02 10:42:33.000000 headline_detector-1.0.2/src/headline_detector/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-04 08:25:52.843200 headline_detector-1.0.2/src/headline_detector.egg-info/
--rw-rw-rw-   0        0        0     2729 2023-05-04 08:25:52.000000 headline_detector-1.0.2/src/headline_detector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      722 2023-05-04 08:25:52.000000 headline_detector-1.0.2/src/headline_detector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 08:25:52.000000 headline_detector-1.0.2/src/headline_detector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-05-04 08:25:52.000000 headline_detector-1.0.2/src/headline_detector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-04 08:25:52.000000 headline_detector-1.0.2/src/headline_detector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 10:18:05.135979 headline_detector-1.0.3/
+-rw-rw-rw-   0        0        0     1103 2023-05-04 08:26:37.000000 headline_detector-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2751 2023-05-09 10:18:05.134979 headline_detector-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2417 2023-05-04 08:26:37.000000 headline_detector-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 10:18:05.135979 headline_detector-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      781 2023-05-09 10:17:42.000000 headline_detector-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 10:18:05.101978 headline_detector-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 10:18:05.114980 headline_detector-1.0.3/src/headline_detector/
+-rw-rw-rw-   0        0        0       93 2023-05-02 12:00:22.000000 headline_detector-1.0.3/src/headline_detector/__init__.py
+-rw-rw-rw-   0        0        0     7757 2023-05-09 10:17:12.000000 headline_detector-1.0.3/src/headline_detector/detector.py
+-rw-rw-rw-   0        0        0      498 2023-05-02 09:35:48.000000 headline_detector-1.0.3/src/headline_detector/hyper_params.py
+-rw-rw-rw-   0        0        0     5241 2023-05-02 11:58:36.000000 headline_detector-1.0.3/src/headline_detector/model.py
+-rw-rw-rw-   0        0        0     1407 2023-05-02 09:47:20.000000 headline_detector-1.0.3/src/headline_detector/model_checkpoint.py
+-rw-rw-rw-   0        0        0     1395 2023-05-04 08:22:17.000000 headline_detector-1.0.3/src/headline_detector/preprocessing_scenario.py
+drwxrwxrwx   0        0        0        0 2023-05-09 10:18:05.132979 headline_detector-1.0.3/src/headline_detector/processing_pipeline/
+-rw-rw-rw-   0        0        0      142 2023-05-02 11:08:45.000000 headline_detector-1.0.3/src/headline_detector/processing_pipeline/__init__.py
+-rw-rw-rw-   0        0        0     1758 2023-05-02 11:32:18.000000 headline_detector-1.0.3/src/headline_detector/processing_pipeline/pipeline.py
+-rw-rw-rw-   0        0        0     2256 2023-05-02 11:07:28.000000 headline_detector-1.0.3/src/headline_detector/processing_pipeline/processing_func.py
+-rw-rw-rw-   0        0        0     2821 2023-05-02 11:07:12.000000 headline_detector-1.0.3/src/headline_detector/processing_pipeline/stemmer.py
+-rw-rw-rw-   0        0        0      202 2023-05-02 10:42:33.000000 headline_detector-1.0.3/src/headline_detector/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 10:18:05.128979 headline_detector-1.0.3/src/headline_detector.egg-info/
+-rw-rw-rw-   0        0        0     2751 2023-05-09 10:18:04.000000 headline_detector-1.0.3/src/headline_detector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      730 2023-05-09 10:18:04.000000 headline_detector-1.0.3/src/headline_detector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 10:18:04.000000 headline_detector-1.0.3/src/headline_detector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-05-09 10:18:04.000000 headline_detector-1.0.3/src/headline_detector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-09 10:18:04.000000 headline_detector-1.0.3/src/headline_detector.egg-info/top_level.txt
```

### Comparing `headline_detector-1.0.2/PKG-INFO` & `headline_detector-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: headline_detector
-Version: 1.0.2
+Version: 1.0.3
 Summary: An Indonesian Headline Detection Python API.
 Author: Kaenova Mahendra Auditama
 Author-email: kaenova@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # [headline_detector](https://github.com/kaenova/headline_detector)
 
 _Indonesian Headline Detection Python API_
 
 This is a Python library that provides APIs for detecting headlines in textual data, especially on social media platforms such as Twitter. The library utilizes a model that has been developed and trained on a dataset of Twitter posts containing both headline and non-headline texts, with the assistance of journalism professionals to ensure the data quality.
 
@@ -24,15 +25,15 @@
 | ------------ | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
 | Fasttext     | 0.8766     | 0.8714     | 0.8793     | 0.8714     | 0.8714     | 0.8661     |
 | CNN          | 0.9081     | 0.9081     | 0.8950     | 0.8898     | 0.8950     | 0.8898     |
 | IndoBERTweet | 0.9895     | 0.9921     | 0.9738     | 0.9580     | 0.9843     | 0.9685     |
 
 All meassured in accuracy
 
-### Model Throughput
+## Model Throughput
 
 | Model        | Throughput (Â± Text/seconds) |
 | ------------ | --------------------------- |
 | IndoBERTweet | Â±1.3                        |
 | CNN          | Â±281.60                     |
 | Fasttext     | Â±2048.41                    |
```

### Comparing `headline_detector-1.0.2/README.md` & `headline_detector-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 | ------------ | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
 | Fasttext     | 0.8766     | 0.8714     | 0.8793     | 0.8714     | 0.8714     | 0.8661     |
 | CNN          | 0.9081     | 0.9081     | 0.8950     | 0.8898     | 0.8950     | 0.8898     |
 | IndoBERTweet | 0.9895     | 0.9921     | 0.9738     | 0.9580     | 0.9843     | 0.9685     |
 
 All meassured in accuracy
 
-### Model Throughput
+## Model Throughput
 
 | Model        | Throughput (± Text/seconds) |
 | ------------ | --------------------------- |
 | IndoBERTweet | ±1.3                        |
 | CNN          | ±281.60                     |
 | Fasttext     | ±2048.41                    |
```

### Comparing `headline_detector-1.0.2/setup.py` & `headline_detector-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 requirements = (this_directory / "requirements.txt").read_text().split("\n")
 
 setuptools.setup(
     name = "headline_detector",
-    version = "1.0.2",
+    version = "1.0.3",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = "Kaenova Mahendra Auditama",
     author_email = "kaenova@gmail.com",
     description = "An Indonesian Headline Detection Python API.",
     classifiers = [
         "Programming Language :: Python :: 3",
```

### Comparing `headline_detector-1.0.2/src/headline_detector/detector.py` & `headline_detector-1.0.3/src/headline_detector/detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,22 +32,22 @@
         with torch.no_grad():
             for text in tqdm(texts):
                 if self.preprocessor is not None:
                     text = self.preprocessor.process_text(text)
                 logits = self.active_model.forward([text])
                 prediction.append(logits)
         prediction = torch.cat(prediction, 0)
-        prediction = F.softmax(prediction, dim=0)
+        prediction = F.softmax(prediction, dim=1)
         prediction = torch.argmax(prediction, 1)
         prediction = prediction.cpu().numpy()
         prediction = prediction.tolist()
         return prediction
 
     @staticmethod
-    def load_from_scenario(scenario_num: "int") -> "model.FastTextClassifier":
+    def load_from_scenario(scenario_num: "int") -> "FasttextDetector":
         # Load model
         scenario_num = int(scenario_num)
         if scenario_num not in m_checkpoint.fasttext_checkpoints.keys():
             raise ValueError("Not a valid scenario number")
         model_path = hf_hub.hf_hub_download(
             repo_id=m_checkpoint.repo_id,
             filename=m_checkpoint.fasttext_checkpoints[scenario_num],
@@ -92,22 +92,22 @@
         with torch.no_grad():
             for text in tqdm(texts):
                 if self.preprocessor is not None:
                     text = self.preprocessor.process_text(text)
                 logits = self.active_model.forward([text])
                 prediction.append(logits)
         prediction = torch.cat(prediction, 0)
-        prediction = F.softmax(prediction, dim=0)
+        prediction = F.softmax(prediction, dim=1)
         prediction = torch.argmax(prediction, 1)
         prediction = prediction.cpu().numpy()
         prediction = prediction.tolist()
         return prediction
 
     @staticmethod
-    def load_from_scenario(scenario_num: "int") -> "model.CNNClassifier":
+    def load_from_scenario(scenario_num: "int") -> "CNNDetector":
         scenario_num = int(scenario_num)
         if scenario_num not in m_checkpoint.cnn_checkpoints.keys():
             raise ValueError("Not a valid scenario number")
         model_path = hf_hub.hf_hub_download(
             repo_id=m_checkpoint.repo_id,
             filename=m_checkpoint.cnn_checkpoints[scenario_num],
             cache_dir=".headline_detector_model",
@@ -153,22 +153,22 @@
         with torch.no_grad():
             for text in tqdm(texts):
                 if self.preprocessor is not None:
                     text = self.preprocessor.process_text(text)
                 logits = self.active_model.forward([text])
                 prediction.append(logits)
         prediction = torch.cat(prediction, 0)
-        prediction = F.softmax(prediction, dim=0)
+        prediction = F.softmax(prediction, dim=1)
         prediction = torch.argmax(prediction, 1)
         prediction = prediction.cpu().numpy()
         prediction = prediction.tolist()
         return prediction
 
     @staticmethod
-    def load_from_scenario(scenario_num: "int") -> "model.BERTClassifier":
+    def load_from_scenario(scenario_num: "int") -> "IndoBERTweetDetector":
         scenario_num = int(scenario_num)
         if scenario_num not in m_checkpoint.indobertweet_checkpoints.keys():
             raise ValueError("Not a valid scenario number")
         model_path = hf_hub.hf_hub_download(
             repo_id=m_checkpoint.repo_id,
             filename=m_checkpoint.indobertweet_checkpoints[scenario_num],
             cache_dir=".headline_detector_model",
```

### Comparing `headline_detector-1.0.2/src/headline_detector/model.py` & `headline_detector-1.0.3/src/headline_detector/model.py`

 * *Files identical despite different names*

### Comparing `headline_detector-1.0.2/src/headline_detector/model_checkpoint.py` & `headline_detector-1.0.3/src/headline_detector/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `headline_detector-1.0.2/src/headline_detector/preprocessing_scenario.py` & `headline_detector-1.0.3/src/headline_detector/preprocessing_scenario.py`

 * *Files identical despite different names*

### Comparing `headline_detector-1.0.2/src/headline_detector/processing_pipeline/pipeline.py` & `headline_detector-1.0.3/src/headline_detector/processing_pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `headline_detector-1.0.2/src/headline_detector/processing_pipeline/processing_func.py` & `headline_detector-1.0.3/src/headline_detector/processing_pipeline/processing_func.py`

 * *Files identical despite different names*

### Comparing `headline_detector-1.0.2/src/headline_detector/processing_pipeline/stemmer.py` & `headline_detector-1.0.3/src/headline_detector/processing_pipeline/stemmer.py`

 * *Files identical despite different names*

### Comparing `headline_detector-1.0.2/src/headline_detector.egg-info/PKG-INFO` & `headline_detector-1.0.3/src/headline_detector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: headline-detector
-Version: 1.0.2
+Version: 1.0.3
 Summary: An Indonesian Headline Detection Python API.
 Author: Kaenova Mahendra Auditama
 Author-email: kaenova@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # [headline_detector](https://github.com/kaenova/headline_detector)
 
 _Indonesian Headline Detection Python API_
 
 This is a Python library that provides APIs for detecting headlines in textual data, especially on social media platforms such as Twitter. The library utilizes a model that has been developed and trained on a dataset of Twitter posts containing both headline and non-headline texts, with the assistance of journalism professionals to ensure the data quality.
 
@@ -24,15 +25,15 @@
 | ------------ | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
 | Fasttext     | 0.8766     | 0.8714     | 0.8793     | 0.8714     | 0.8714     | 0.8661     |
 | CNN          | 0.9081     | 0.9081     | 0.8950     | 0.8898     | 0.8950     | 0.8898     |
 | IndoBERTweet | 0.9895     | 0.9921     | 0.9738     | 0.9580     | 0.9843     | 0.9685     |
 
 All meassured in accuracy
 
-### Model Throughput
+## Model Throughput
 
 | Model        | Throughput (Â± Text/seconds) |
 | ------------ | --------------------------- |
 | IndoBERTweet | Â±1.3                        |
 | CNN          | Â±281.60                     |
 | Fasttext     | Â±2048.41                    |
```

### Comparing `headline_detector-1.0.2/src/headline_detector.egg-info/SOURCES.txt` & `headline_detector-1.0.3/src/headline_detector.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 src/headline_detector/__init__.py
 src/headline_detector/detector.py
 src/headline_detector/hyper_params.py
 src/headline_detector/model.py
 src/headline_detector/model_checkpoint.py
```

