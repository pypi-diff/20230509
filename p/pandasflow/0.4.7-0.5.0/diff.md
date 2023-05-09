# Comparing `tmp/pandasflow-0.4.7.tar.gz` & `tmp/pandasflow-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.4.7.tar", last modified: Fri May  5 12:26:32 2023, max compression
+gzip compressed data, was "pandasflow-0.5.0.tar", last modified: Tue May  9 15:34:30 2023, max compression
```

## Comparing `pandasflow-0.4.7.tar` & `pandasflow-0.5.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 12:26:32.724717 pandasflow-0.4.7/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.4.7/LICENCE
--rw-rw-rw-   0        0        0      694 2023-05-05 12:26:32.724717 pandasflow-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.4.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 12:26:32.707961 pandasflow-0.4.7/pandasflow/
--rw-rw-rw-   0        0        0      302 2023-05-05 12:26:28.000000 pandasflow-0.4.7/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:26:32.711571 pandasflow-0.4.7/pandasflow/dev/
--rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.4.7/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.4.7/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      371 2023-05-02 10:20:49.000000 pandasflow-0.4.7/pandasflow/get_import.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:26:32.716189 pandasflow-0.4.7/pandasflow/metrics/
--rw-rw-rw-   0        0        0      324 2023-05-05 12:24:58.000000 pandasflow-0.4.7/pandasflow/metrics/__init__.py
--rw-rw-rw-   0        0        0      687 2023-05-02 14:28:16.000000 pandasflow-0.4.7/pandasflow/metrics/best_f1.py
--rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.4.7/pandasflow/metrics/conf_mat.py
--rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.4.7/pandasflow/metrics/lloss_up.py
--rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.4.7/pandasflow/metrics/mean_error.py
--rw-rw-rw-   0        0        0     1129 2023-05-05 12:20:37.000000 pandasflow-0.4.7/pandasflow/metrics/precision_recall.py
--rw-rw-rw-   0        0        0      984 2023-05-05 12:25:59.000000 pandasflow-0.4.7/pandasflow/metrics/roc.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:26:32.716189 pandasflow-0.4.7/pandasflow/model/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.4.7/pandasflow/model/__init__.py
--rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.4.7/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:26:32.716189 pandasflow-0.4.7/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.4.7/pandasflow/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:26:32.718899 pandasflow-0.4.7/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.4.7/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     3016 2023-05-04 13:48:42.000000 pandasflow-0.4.7/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3719 2023-05-04 13:48:33.000000 pandasflow-0.4.7/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:26:32.710543 pandasflow-0.4.7/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      694 2023-05-05 12:26:32.000000 pandasflow-0.4.7/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      912 2023-05-05 12:26:32.000000 pandasflow-0.4.7/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 12:26:32.000000 pandasflow-0.4.7/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-05 12:26:32.000000 pandasflow-0.4.7/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-05 12:26:32.000000 pandasflow-0.4.7/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 12:26:32.724717 pandasflow-0.4.7/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:26:32.723305 pandasflow-0.4.7/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.4.7/test/__init__.py
--rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.4.7/test/best_f1_test.py
--rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.4.7/test/conf_mat_test.py
--rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.4.7/test/lloss_up_test.py
--rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.4.7/test/mean_error_test.py
--rw-rw-rw-   0        0        0     1285 2023-05-05 12:03:43.000000 pandasflow-0.4.7/test/precision_recall_test.py
--rw-rw-rw-   0        0        0     1272 2023-05-05 12:25:08.000000 pandasflow-0.4.7/test/roc_test.py
--rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.4.7/test/split_tt_test.py
--rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.4.7/test/split_tvt_test.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.021614 pandasflow-0.5.0/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.5.0/LICENCE
+-rw-rw-rw-   0        0        0      694 2023-05-09 15:34:30.021614 pandasflow-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.002664 pandasflow-0.5.0/pandasflow/
+-rw-rw-rw-   0        0        0      346 2023-05-09 15:34:20.000000 pandasflow-0.5.0/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.006654 pandasflow-0.5.0/pandasflow/dev/
+-rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.5.0/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.5.0/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      387 2023-05-09 15:27:01.000000 pandasflow-0.5.0/pandasflow/get_import.py
+-rw-rw-rw-   0        0        0      206 2023-05-09 15:33:32.000000 pandasflow-0.5.0/pandasflow/get_sqlt.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.011641 pandasflow-0.5.0/pandasflow/metrics/
+-rw-rw-rw-   0        0        0      324 2023-05-05 12:24:58.000000 pandasflow-0.5.0/pandasflow/metrics/__init__.py
+-rw-rw-rw-   0        0        0      718 2023-05-08 11:42:43.000000 pandasflow-0.5.0/pandasflow/metrics/best_f1.py
+-rw-rw-rw-   0        0        0     1132 2023-05-02 12:00:22.000000 pandasflow-0.5.0/pandasflow/metrics/conf_mat.py
+-rw-rw-rw-   0        0        0     2263 2023-04-26 15:20:14.000000 pandasflow-0.5.0/pandasflow/metrics/lloss_up.py
+-rw-rw-rw-   0        0        0      400 2023-04-26 15:19:05.000000 pandasflow-0.5.0/pandasflow/metrics/mean_error.py
+-rw-rw-rw-   0        0        0      721 2023-05-07 08:19:28.000000 pandasflow-0.5.0/pandasflow/metrics/precision_recall.py
+-rw-rw-rw-   0        0        0      654 2023-05-07 08:18:25.000000 pandasflow-0.5.0/pandasflow/metrics/roc.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.012637 pandasflow-0.5.0/pandasflow/model/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:16:13.000000 pandasflow-0.5.0/pandasflow/model/__init__.py
+-rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.5.0/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.012637 pandasflow-0.5.0/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.5.0/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.014632 pandasflow-0.5.0/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.5.0/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     3016 2023-05-04 13:48:42.000000 pandasflow-0.5.0/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3719 2023-05-04 13:48:33.000000 pandasflow-0.5.0/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.005655 pandasflow-0.5.0/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-05-09 15:34:29.000000 pandasflow-0.5.0/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      935 2023-05-09 15:34:29.000000 pandasflow-0.5.0/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 15:34:29.000000 pandasflow-0.5.0/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-09 15:34:29.000000 pandasflow-0.5.0/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-09 15:34:29.000000 pandasflow-0.5.0/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 15:34:30.021614 pandasflow-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-04-26 15:06:07.000000 pandasflow-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:34:30.020620 pandasflow-0.5.0/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.5.0/test/__init__.py
+-rw-rw-rw-   0        0        0      760 2023-05-02 12:24:07.000000 pandasflow-0.5.0/test/best_f1_test.py
+-rw-rw-rw-   0        0        0      740 2023-05-02 12:00:40.000000 pandasflow-0.5.0/test/conf_mat_test.py
+-rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.5.0/test/lloss_up_test.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.5.0/test/mean_error_test.py
+-rw-rw-rw-   0        0        0     1296 2023-05-07 08:19:28.000000 pandasflow-0.5.0/test/precision_recall_test.py
+-rw-rw-rw-   0        0        0     1249 2023-05-07 08:18:25.000000 pandasflow-0.5.0/test/roc_test.py
+-rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.5.0/test/split_tt_test.py
+-rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.5.0/test/split_tvt_test.py
```

### Comparing `pandasflow-0.4.7/LICENCE` & `pandasflow-0.5.0/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.7/PKG-INFO` & `pandasflow-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.4.7
+Version: 0.5.0
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.4.7/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.5.0/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.7/pandasflow/metrics/best_f1.py` & `pandasflow-0.5.0/pandasflow/metrics/best_f1.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,12 +22,15 @@
 				f1_score(df[y_true.name], df['y_pred_thr'])
 			)
 		)
 	
 	result = pd.DataFrame(result, columns=['thr', 'f1'])
 	result = result.sort_values(by='f1', ascending=False)
 	
-	print(result.head(min(out, len(result))))
+	result = result.head(min(out, len(result)))
+	
+	print()
+	print(result)
```

### Comparing `pandasflow-0.4.7/pandasflow/metrics/conf_mat.py` & `pandasflow-0.5.0/pandasflow/metrics/conf_mat.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.7/pandasflow/metrics/lloss_up.py` & `pandasflow-0.5.0/pandasflow/metrics/lloss_up.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.7/pandasflow/metrics/precision_recall.py` & `pandasflow-0.5.0/pandasflow/metrics/precision_recall.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 import pandasflow as pdf
 import pandas as pd
 from sklearn.metrics import precision_recall_curve, average_precision_score
 from matplotlib import pyplot
 
 
 def precision_recall(target, score, plot=False, marker='', round_=2):
+	if type(score) == pd.Series:
+		score_ = []
+		score_.append(score)
+	else:
+		score_ = score
 	
-	if type(score) == pd.Series or type(score) == list and len(score) == 1:
-		score_ = score if type(score) == pd.Series else score[0]
-		score_name = score_.name
+	for sc in score_:
+		precision, recall, _ = precision_recall_curve(target, sc)
+		pyplot.plot(recall, precision, marker=marker, label=sc.name)
 		
-		precision, recall, _ = precision_recall_curve(target, score_)
-		pyplot.plot(recall, precision, marker=marker, label=score_name)
-		
-		average = average_precision_score(target, score_)
+		average = average_precision_score(target, sc)
 		average = round(average, round_)
-		print(f"{score_name} average precision: ", average)
-	
-	
-	if type(score) == list and len(score) > 1:
-		for sc in score:
-			precision, recall, _ = precision_recall_curve(target, sc)
-			pyplot.plot(recall, precision, marker=marker, label=sc.name)
-			
-			average = average_precision_score(target, sc)
-			average = round(average, round_)
-			print(f"{sc.name} average precision: ", average)
-			
+		print(f"{sc.name} average precision: ", average)
+		
 	pyplot.xlabel('Recall')
 	pyplot.ylabel('Precision')
 	pyplot.legend()
 	
 	if plot:
 		pyplot.show()
```

### Comparing `pandasflow-0.4.7/pandasflow/reset_mi.py` & `pandasflow-0.5.0/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.7/pandasflow/split/train_test.py` & `pandasflow-0.5.0/pandasflow/split/train_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.7/pandasflow/split/train_valid_test.py` & `pandasflow-0.5.0/pandasflow/split/train_valid_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.7/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.5.0/pandasflow.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.4.7
+Version: 0.5.0
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.4.7/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.5.0/pandasflow.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENCE
 README.md
 setup.cfg
 setup.py
 pandasflow/__init__.py
 pandasflow/get_import.py
+pandasflow/get_sqlt.py
 pandasflow/reset_mi.py
 pandasflow.egg-info/PKG-INFO
 pandasflow.egg-info/SOURCES.txt
 pandasflow.egg-info/dependency_links.txt
 pandasflow.egg-info/requires.txt
 pandasflow.egg-info/top_level.txt
 pandasflow/dev/__init__.py
```

### Comparing `pandasflow-0.4.7/setup.py` & `pandasflow-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.7/test/best_f1_test.py` & `pandasflow-0.5.0/test/best_f1_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.7/test/conf_mat_test.py` & `pandasflow-0.5.0/test/conf_mat_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.7/test/lloss_up_test.py` & `pandasflow-0.5.0/test/lloss_up_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.7/test/precision_recall_test.py` & `pandasflow-0.5.0/test/precision_recall_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,12 +23,12 @@
 t['y_score3'] = np.concatenate([np.random.uniform(0, 0.2, size=850), #TN
                                 np.random.uniform(0.8, 1, size=140), #FP
                                 np.random.uniform(0, 0.2, size=2),   #FN
                                 np.random.uniform(0.8, 1, size=8)])  #TP
 
 
 
-# pdf.metrics.precision_recall(t['y_true'], score=t['y_score1'])
+pdf.metrics.precision_recall(t['y_true'], score=t['y_score1'], plot=True)
 
 # pdf.metrics.precision_recall(t['y_true'], score=[t['y_score1'], t['y_score2']])
 
-pdf.metrics.precision_recall(t['y_true'], score=[t['y_score1'], t['y_score2'], t['y_score3']], plot=True)
+# pdf.metrics.precision_recall(t['y_true'], score=[t['y_score1'], t['y_score2'], t['y_score3']], plot=True)
```

### Comparing `pandasflow-0.4.7/test/roc_test.py` & `pandasflow-0.5.0/test/roc_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import pandasflow as pdf
 import pandas as pd
 import numpy as np
 
-
-
-
-
 t = pd.DataFrame({'y_true': [0]*990 + [1]*10})
 
 np.random.seed(42)
 
 t['y_score1'] = np.concatenate([np.random.uniform(0, 0.2, size=970),
                                 np.random.uniform(0.8, 1, size=20),
                                 np.random.uniform(0, 0.2, size=5),
@@ -23,12 +19,12 @@
 t['y_score3'] = np.concatenate([np.random.uniform(0, 0.2, size=850), #TN
                                 np.random.uniform(0.8, 1, size=140), #FP
                                 np.random.uniform(0, 0.2, size=2),   #FN
                                 np.random.uniform(0.8, 1, size=8)])  #TP
 
 
 
-# pdf.metrics.precision_recall(t['y_true'], score=t['y_score1'])
+pdf.metrics.roc(t['y_true'], score=t['y_score1'], plot=True)
 
-# pdf.metrics.precision_recall(t['y_true'], score=[t['y_score1'], t['y_score2']])
+# pdf.metrics.roc(t['y_true'], score=[t['y_score1'], t['y_score2']])
 
-pdf.metrics.roc(t['y_true'], score=[t['y_score1'], t['y_score2'], t['y_score3']], plot=True)
+# pdf.metrics.roc(t['y_true'], score=[t['y_score1'], t['y_score2'], t['y_score3']], plot=True)
```

### Comparing `pandasflow-0.4.7/test/split_tvt_test.py` & `pandasflow-0.5.0/test/split_tvt_test.py`

 * *Files identical despite different names*

