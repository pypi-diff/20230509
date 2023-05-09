# Comparing `tmp/FakeNewsClassifier-0.0.20.tar.gz` & `tmp/FakeNewsClassifier-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FakeNewsClassifier-0.0.20.tar", last modified: Mon May  8 11:43:42 2023, max compression
+gzip compressed data, was "FakeNewsClassifier-0.0.21.tar", last modified: Tue May  9 08:34:58 2023, max compression
```

## Comparing `FakeNewsClassifier-0.0.20.tar` & `FakeNewsClassifier-0.0.21.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 xkoren10  (1001) xkoren10  (1001)        0 2023-05-08 11:43:42.156105 FakeNewsClassifier-0.0.20/
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     1073 2023-05-01 19:59:28.000000 FakeNewsClassifier-0.0.20/LICENSE
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)      131 2023-05-05 13:45:29.000000 FakeNewsClassifier-0.0.20/MANIFEST.in
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     5096 2023-05-08 11:43:42.156105 FakeNewsClassifier-0.0.20/PKG-INFO
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     4558 2023-05-06 16:13:30.000000 FakeNewsClassifier-0.0.20/README.md
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)      756 2023-05-08 11:43:09.000000 FakeNewsClassifier-0.0.20/pyproject.toml
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)       38 2023-05-08 11:43:42.156105 FakeNewsClassifier-0.0.20/setup.cfg
-drwxrwxr-x   0 xkoren10  (1001) xkoren10  (1001)        0 2023-05-08 11:43:42.142104 FakeNewsClassifier-0.0.20/src/
-drwxrwxr-x   0 xkoren10  (1001) xkoren10  (1001)        0 2023-05-08 11:43:42.143105 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)       32 2023-05-02 18:47:16.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/__init__.py
-drwxrwxr-x   0 xkoren10  (1001) xkoren10  (1001)        0 2023-05-08 11:43:42.145105 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/datasets/
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)   351716 2023-05-02 22:58:52.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/datasets/dezinfo_sk.csv
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     2963 2023-03-05 18:12:21.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/datasets/stopwords.txt
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     2904 2023-05-07 21:04:34.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/dt.py
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     4380 2023-05-08 11:42:51.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/models.py
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     2531 2023-05-05 21:53:44.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/nb.py
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     1635 2023-05-05 21:42:11.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/process_text.py
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     5598 2023-05-06 13:40:43.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/saved_model.py
-drwxrwxr-x   0 xkoren10  (1001) xkoren10  (1001)        0 2023-05-08 11:43:42.155104 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/saved_models/
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)   319857 2023-05-06 13:39:24.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/saved_models/model_dt.pk
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)   649580 2023-05-06 13:38:48.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/saved_models/model_nb.pk
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001) 16020024 2023-05-06 13:38:39.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/saved_models/model_snn.hdf5
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)   317973 2023-05-06 13:38:39.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/saved_models/model_snn.pk
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)   560889 2023-05-06 13:39:06.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/saved_models/model_svm.pk
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)      616 2023-05-05 21:38:26.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/scraper.py
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     3682 2023-05-05 21:57:38.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/snn.py
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     2627 2023-05-05 21:54:58.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/svm.py
-drwxrwxr-x   0 xkoren10  (1001) xkoren10  (1001)        0 2023-05-08 11:43:42.144105 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier.egg-info/
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     5096 2023-05-08 11:43:42.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier.egg-info/PKG-INFO
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)      936 2023-05-08 11:43:42.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier.egg-info/SOURCES.txt
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)        1 2023-05-08 11:43:42.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier.egg-info/dependency_links.txt
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)       92 2023-05-08 11:43:42.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier.egg-info/requires.txt
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)       33 2023-05-08 11:43:42.000000 FakeNewsClassifier-0.0.20/src/FakeNewsClassifier.egg-info/top_level.txt
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)        0 2023-05-06 12:30:59.000000 FakeNewsClassifier-0.0.20/src/__init__.py
--rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     1481 2023-05-06 12:30:19.000000 FakeNewsClassifier-0.0.20/src/main.py
+drwxrwxr-x   0 xkoren10  (1001) xkoren10  (1001)        0 2023-05-09 08:34:58.530605 FakeNewsClassifier-0.0.21/
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     1073 2023-05-01 19:59:28.000000 FakeNewsClassifier-0.0.21/LICENSE
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)      131 2023-05-05 13:45:29.000000 FakeNewsClassifier-0.0.21/MANIFEST.in
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     5096 2023-05-09 08:34:58.529605 FakeNewsClassifier-0.0.21/PKG-INFO
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     4558 2023-05-06 16:13:30.000000 FakeNewsClassifier-0.0.21/README.md
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)      756 2023-05-09 08:34:41.000000 FakeNewsClassifier-0.0.21/pyproject.toml
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)       38 2023-05-09 08:34:58.530605 FakeNewsClassifier-0.0.21/setup.cfg
+drwxrwxr-x   0 xkoren10  (1001) xkoren10  (1001)        0 2023-05-09 08:34:58.513605 FakeNewsClassifier-0.0.21/src/
+drwxrwxr-x   0 xkoren10  (1001) xkoren10  (1001)        0 2023-05-09 08:34:58.514605 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)       32 2023-05-02 18:47:16.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/__init__.py
+drwxrwxr-x   0 xkoren10  (1001) xkoren10  (1001)        0 2023-05-09 08:34:58.516605 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/datasets/
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)   351716 2023-05-02 22:58:52.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/datasets/dezinfo_sk.csv
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     2963 2023-03-05 18:12:21.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/datasets/stopwords.txt
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     3055 2023-05-09 08:32:17.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/dt.py
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     4380 2023-05-08 11:42:51.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/models.py
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     2680 2023-05-09 08:33:39.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/nb.py
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     1635 2023-05-05 21:42:11.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/process_text.py
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     5598 2023-05-06 13:40:43.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/saved_model.py
+drwxrwxr-x   0 xkoren10  (1001) xkoren10  (1001)        0 2023-05-09 08:34:58.529605 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/saved_models/
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)   319857 2023-05-06 13:39:24.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/saved_models/model_dt.pk
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)   649580 2023-05-06 13:38:48.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/saved_models/model_nb.pk
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001) 16020024 2023-05-06 13:38:39.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/saved_models/model_snn.hdf5
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)   317973 2023-05-06 13:38:39.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/saved_models/model_snn.pk
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)   560889 2023-05-06 13:39:06.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/saved_models/model_svm.pk
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)      616 2023-05-05 21:38:26.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/scraper.py
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     3831 2023-05-09 08:33:49.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/snn.py
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     2774 2023-05-09 08:33:55.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/svm.py
+drwxrwxr-x   0 xkoren10  (1001) xkoren10  (1001)        0 2023-05-09 08:34:58.515605 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier.egg-info/
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     5096 2023-05-09 08:34:58.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier.egg-info/PKG-INFO
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)      936 2023-05-09 08:34:58.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)        1 2023-05-09 08:34:58.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)       92 2023-05-09 08:34:58.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier.egg-info/requires.txt
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)       33 2023-05-09 08:34:58.000000 FakeNewsClassifier-0.0.21/src/FakeNewsClassifier.egg-info/top_level.txt
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)        0 2023-05-06 12:30:59.000000 FakeNewsClassifier-0.0.21/src/__init__.py
+-rw-rw-r--   0 xkoren10  (1001) xkoren10  (1001)     1481 2023-05-06 12:30:19.000000 FakeNewsClassifier-0.0.21/src/main.py
```

### Comparing `FakeNewsClassifier-0.0.20/LICENSE` & `FakeNewsClassifier-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `FakeNewsClassifier-0.0.20/PKG-INFO` & `FakeNewsClassifier-0.0.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FakeNewsClassifier
-Version: 0.0.20
+Version: 0.0.21
 Summary: Simple fake news classifier package created for bachelor's thesis 'Detection of Fake News Using Machine Learning'.
 Author-email: Matej Koreň <xkoren10@stud.fit.vutbr.cz>
 Project-URL: Homepage, https://github.com/xkoren10/BP-2022-23
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `FakeNewsClassifier-0.0.20/README.md` & `FakeNewsClassifier-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `FakeNewsClassifier-0.0.20/pyproject.toml` & `FakeNewsClassifier-0.0.21/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FakeNewsClassifier"
-version = "0.0.20"
+version = "0.0.21"
 authors = [
   { name="Matej Koreň", email="xkoren10@stud.fit.vutbr.cz" },
 ]
 description = "Simple fake news classifier package created for bachelor's thesis 'Detection of Fake News Using Machine Learning'."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/datasets/dezinfo_sk.csv` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/datasets/dezinfo_sk.csv`

 * *Files identical despite different names*

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/datasets/stopwords.txt` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/datasets/stopwords.txt`

 * *Files identical despite different names*

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/dt.py` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/dt.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         ('bow', CountVectorizer(analyzer=pt.process_text)),
         # integer counts to weighted TF-IDF scores
         ('tfidf', TfidfTransformer()),
         # train on TF-IDF vectors w/ Decision Tree classifier
         ('classifier', DecisionTreeClassifier(min_samples_leaf=10)),
     ])
     # training
+    print("Training in progress...")
     pipeline_dt.fit(X_train, y_train)
 
     # testing
     predictions_DT = pipeline_dt.predict(X_test)
 
     # results
     print('DT - test')
@@ -52,14 +53,15 @@
         user_input = input(
             'New model was trained, would you like to save it? (Y/N): ')
 
         if user_input.lower() == 'y' or 'yes':
             filename = 'model_dt.pk'
             with open(os.path.join(saved_model_dir, filename), 'wb') as file:
                 pickle.dump(pipeline_dt, file)
+            print("Model saved successfully.")
             break
         elif user_input.lower() == 'n' or 'no':
             break
         else:
             print('Invalid option, please, type yes or no.')
 
     # additional statistics
@@ -79,7 +81,8 @@
         df_cm = pd.DataFrame(cm, index=class_label, columns=class_label)
         sns.heatmap(df_cm, annot=True, fmt='d', cmap="crest")
         plt.title("Confusion Matrix - Decision Tree")
         plt.xlabel("Predicted Label")
         plt.ylabel("True Label")
         plt.savefig('figures/dt_' +
                     str(datetime.now().strftime("%Y-%m-%d_%H-%M-%S")) + '.png')
+        print("Statistics saved into figures/.. and html/.. .")
```

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/models.py` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/models.py`

 * *Files identical despite different names*

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/nb.py` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/nb.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         # integer counts to weighted TF-IDF scores
         ('tfidf', TfidfTransformer()),
         # train on TF-IDF vectors w/ Naive Bayes classifier
         ('classifier', MultinomialNB()),
     ])
 
     # training
+    print("Training in progress...")
     pipeline_nb.fit(X_train, y_train)
 
     # testing
     predictions_NB = pipeline_nb.predict(X_test)
 
     # results
     print('NB - test')
@@ -52,14 +53,15 @@
         user_input = input(
             'New model was trained, would you like to save it? (Y/N): ')
 
         if user_input.lower() == 'y' or 'yes':
             filename = 'model_nb.pk'
             with open(os.path.join(saved_model_dir, filename), 'wb') as file:
                 pickle.dump(pipeline_nb, file)
+            print("Model saved successfully.")
             break
         elif user_input.lower() == 'n' or 'no':
             break
         else:
             print('Invalid option, please, type yes or no.')
 
     # additional statistics
@@ -71,7 +73,8 @@
         df_cm = pd.DataFrame(cm, index=class_label, columns=class_label)
         sns.heatmap(df_cm, annot=True, fmt='d', cmap="crest")
         plt.title("Confusion Matrix - Naive Bayes")
         plt.xlabel("Predicted Label")
         plt.ylabel("True Label")
         plt.savefig('figures/nb_' +
                     str(datetime.now().strftime("%Y-%m-%d_%H-%M-%S")) + '.png')
+        print("Statistics saved into figures/.. and html/.. .")
```

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/process_text.py` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/process_text.py`

 * *Files identical despite different names*

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/saved_model.py` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/saved_model.py`

 * *Files identical despite different names*

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/saved_models/model_dt.pk` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/saved_models/model_dt.pk`

 * *Files identical despite different names*

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/saved_models/model_nb.pk` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/saved_models/model_nb.pk`

 * *Files identical despite different names*

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/saved_models/model_snn.hdf5` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/saved_models/model_snn.hdf5`

 * *Files identical despite different names*

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/saved_models/model_snn.pk` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/saved_models/model_snn.pk`

 * *Files identical despite different names*

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/saved_models/model_svm.pk` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/saved_models/model_svm.pk`

 * *Files identical despite different names*

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/scraper.py` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/scraper.py`

 * *Files identical despite different names*

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/snn.py` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/snn.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     tfidf_var = pipeline_snn.transform(X_train)
 
     # model initializing
     snn_model = KerasClassifier(model=make_model(tfidf_var.shape[1:], verbose), verbose=1,
                                 epochs=10, batch_size=10, callbacks=EarlyStopping(monitor='loss', mode='min', verbose=1))
 
     # model training
+    print("Training in progress...")
     snn_model.fit(tfidf_var, y_train)
 
     # test text transforming
     test_var = pipeline_snn.transform(X_test)
 
     # model testing
     predictions_snn = snn_model.predict(test_var)
@@ -83,14 +84,15 @@
             'New model was trained, would you like to save it? (Y/N): ')
 
         if user_input.lower() == 'y' or 'yes':
             filename = 'model_snn.pk'
             with open(os.path.join(saved_model_dir,filename), 'wb') as file:
                 pickle.dump(pipeline_snn, file)
             snn_model.model.save(os.path.join(saved_model_dir,'model_snn.hdf5'))
+            print("Model saved successfully.")
             break
         elif user_input.lower() == 'n' or 'no':
             break
         else:
             print('Invalid option, please, type yes or no.')
 
     # additional statistics
@@ -101,7 +103,8 @@
         df_cm = pd.DataFrame(cm, index=class_label, columns=class_label)
         sns.heatmap(df_cm, annot=True, fmt='d', cmap="crest")
         plt.title("Confusion Matrix - Sequential NN")
         plt.xlabel("Predicted Label")
         plt.ylabel("True Label")
         plt.savefig('figures/snn_' +
                     str(datetime.now().strftime("%Y-%m-%d_%H-%M-%S")) + '.png')
+        print("Statistics saved into figures/.. and html/.. .")
```

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier/svm.py` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier/svm.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         # integer counts to weighted TF-IDF scores
         ('tfidf', TfidfTransformer()),
         # train w/ Support Vectors classifier
         ('classifier', SVC(C=1.0, kernel='linear', gamma='auto', probability=True)),
     ])
 
     #training
+    print("Training in progress...")
     pipeline_sv.fit(X_train, y_train)
 
     #testing
     predictions_SVM = pipeline_sv.predict(X_test)
 
     #results
     print('SVM - test')
@@ -54,14 +55,15 @@
     while True:
         user_input = input('New model was trained, would you like to save it? (Y/N): ')
 
         if user_input.lower() == 'y' or 'yes':
             filename = 'model_svm.pk'
             with open(os.path.join(saved_model_dir,filename), 'wb') as file:
                 pickle.dump(pipeline_sv, file)
+            print("Model saved successfully.")
             break
         elif user_input.lower() == 'n' or 'no':
             break
         else:
             print('Invalid option, please, type yes or no.')
 
     # additional statistics
@@ -73,8 +75,8 @@
         df_cm = pd.DataFrame(cm, index=class_label, columns=class_label)
         sns.heatmap(df_cm, annot=True, fmt='d', cmap="crest")
         plt.title("Confusion Matrix - Support vectors")
         plt.xlabel("Predicted Label")
         plt.ylabel("True Label")
         plt.savefig('figures/svm' +
                     str(datetime.now().strftime("%Y-%m-%d_%H-%M-%S")) + '.png')
-
+        print("Statistics saved into figures/.. and html/.. .")
```

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier.egg-info/PKG-INFO` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FakeNewsClassifier
-Version: 0.0.20
+Version: 0.0.21
 Summary: Simple fake news classifier package created for bachelor's thesis 'Detection of Fake News Using Machine Learning'.
 Author-email: Matej Koreň <xkoren10@stud.fit.vutbr.cz>
 Project-URL: Homepage, https://github.com/xkoren10/BP-2022-23
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `FakeNewsClassifier-0.0.20/src/FakeNewsClassifier.egg-info/SOURCES.txt` & `FakeNewsClassifier-0.0.21/src/FakeNewsClassifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FakeNewsClassifier-0.0.20/src/main.py` & `FakeNewsClassifier-0.0.21/src/main.py`

 * *Files identical despite different names*

