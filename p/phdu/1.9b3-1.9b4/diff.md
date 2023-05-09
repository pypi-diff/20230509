# Comparing `tmp/phdu-1.9b3.tar.gz` & `tmp/phdu-1.9b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-1.9b3.tar", last modified: Mon May  8 09:35:08 2023, max compression
+gzip compressed data, was "phdu-1.9b4.tar", last modified: Tue May  9 09:10:58 2023, max compression
```

## Comparing `phdu-1.9b3.tar` & `phdu-1.9b4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 09:35:08.701977 phdu-1.9b3/
--rw-r--r--   0 userx     (1000) wheel      (998)    35149 2023-01-19 11:17:18.000000 phdu-1.9b3/LICENSE.md
--rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-05-08 09:35:08.701977 phdu-1.9b3/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)     1771 2023-03-22 15:47:48.000000 phdu-1.9b3/README.md
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 09:35:08.698644 phdu-1.9b3/phdu/
--rw-r--r--   0 userx     (1000) wheel      (998)      486 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)      608 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2828 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/clustering.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3319 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/decomposition.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2628 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/np_utils.py
--rw-r--r--   0 userx     (1000) wheel      (998)     5912 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/pd_utils.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 09:35:08.698644 phdu-1.9b3/phdu/plots/
--rw-r--r--   0 userx     (1000) wheel      (998)       66 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/plots/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)        0 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/plots/_mpl.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3359 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/plots/base.py
--rw-r--r--   0 userx     (1000) wheel      (998)    14203 2023-04-28 14:30:33.000000 phdu-1.9b3/phdu/plots/plotly_utils.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3978 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/script_fmt.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 09:35:08.701977 phdu-1.9b3/phdu/stats/
--rw-r--r--   0 userx     (1000) wheel      (998)      157 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/stats/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2526 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/stats/_integration.py
--rw-r--r--   0 userx     (1000) wheel      (998)      842 2023-04-28 14:15:26.000000 phdu-1.9b3/phdu/stats/_plots.py
--rw-r--r--   0 userx     (1000) wheel      (998)      343 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/stats/_preprocess.py
--rw-r--r--   0 userx     (1000) wheel      (998)    31044 2023-05-08 09:34:15.000000 phdu-1.9b3/phdu/stats/bootstrap.py
--rw-r--r--   0 userx     (1000) wheel      (998)     9411 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/stats/conf_interval.py
--rw-r--r--   0 userx     (1000) wheel      (998)      643 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/stats/corr.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 09:35:08.701977 phdu-1.9b3/phdu/stats/rtopy/
--rw-r--r--   0 userx     (1000) wheel      (998)       22 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     1306 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4755 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 09:35:08.701977 phdu-1.9b3/phdu/stats/test/
--rw-r--r--   0 userx     (1000) wheel      (998)       25 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/stats/test/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)      279 2023-01-19 11:17:18.000000 phdu-1.9b3/phdu/stats/test/_adherence.py
--rw-r--r--   0 userx     (1000) wheel      (998)    16550 2023-03-22 15:47:48.000000 phdu-1.9b3/phdu/stats/test/permutation.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4179 2023-04-28 14:15:26.000000 phdu-1.9b3/phdu/storage.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-05-08 09:35:08.698644 phdu-1.9b3/phdu.egg-info/
--rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-05-08 09:35:08.000000 phdu-1.9b3/phdu.egg-info/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)      752 2023-05-08 09:35:08.000000 phdu-1.9b3/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 userx     (1000) wheel      (998)        1 2023-05-08 09:35:08.000000 phdu-1.9b3/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 userx     (1000) wheel      (998)      302 2023-05-08 09:35:08.000000 phdu-1.9b3/phdu.egg-info/requires.txt
--rw-r--r--   0 userx     (1000) wheel      (998)        5 2023-05-08 09:35:08.000000 phdu-1.9b3/phdu.egg-info/top_level.txt
--rw-r--r--   0 userx     (1000) wheel      (998)      106 2023-05-08 09:35:08.701977 phdu-1.9b3/setup.cfg
--rw-r--r--   0 userx     (1000) wheel      (998)     1660 2023-05-08 09:34:41.000000 phdu-1.9b3/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:10:58.535032 phdu-1.9b4/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-1.9b4/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-05-09 09:10:58.535032 phdu-1.9b4/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-1.9b4/README.md
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:10:58.427027 phdu-1.9b4/phdu/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-1.9b4/phdu/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-1.9b4/phdu/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-1.9b4/phdu/clustering.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-1.9b4/phdu/decomposition.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-1.9b4/phdu/np_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-1.9b4/phdu/pd_utils.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:10:58.471029 phdu-1.9b4/phdu/plots/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-1.9b4/phdu/plots/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-1.9b4/phdu/plots/_mpl.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-1.9b4/phdu/plots/base.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    14203 2023-05-04 17:25:49.000000 phdu-1.9b4/phdu/plots/plotly_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-1.9b4/phdu/script_fmt.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:10:58.499030 phdu-1.9b4/phdu/stats/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-1.9b4/phdu/stats/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-1.9b4/phdu/stats/_integration.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-1.9b4/phdu/stats/_plots.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-1.9b4/phdu/stats/_preprocess.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    31861 2023-05-09 09:10:20.000000 phdu-1.9b4/phdu/stats/bootstrap.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-1.9b4/phdu/stats/conf_interval.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-1.9b4/phdu/stats/corr.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:10:58.515031 phdu-1.9b4/phdu/stats/rtopy/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-1.9b4/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-1.9b4/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-1.9b4/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:10:58.531031 phdu-1.9b4/phdu/stats/test/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-1.9b4/phdu/stats/test/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-1.9b4/phdu/stats/test/_adherence.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-1.9b4/phdu/stats/test/permutation.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4179 2023-04-25 11:08:38.000000 phdu-1.9b4/phdu/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:10:58.455028 phdu-1.9b4/phdu.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-05-09 09:10:58.000000 phdu-1.9b4/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-05-09 09:10:58.000000 phdu-1.9b4/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-05-09 09:10:58.000000 phdu-1.9b4/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-05-09 09:10:58.000000 phdu-1.9b4/phdu.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-05-09 09:10:58.000000 phdu-1.9b4/phdu.egg-info/top_level.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-05-09 09:10:58.543032 phdu-1.9b4/setup.cfg
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-05-09 09:10:34.000000 phdu-1.9b4/setup.py
```

### Comparing `phdu-1.9b3/LICENSE.md` & `phdu-1.9b4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/PKG-INFO` & `phdu-1.9b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.9b3
+Version: 1.9b4
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.9b3/README.md` & `phdu-1.9b4/README.md`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu/_helper.py` & `phdu-1.9b4/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu/clustering.py` & `phdu-1.9b4/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu/decomposition.py` & `phdu-1.9b4/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu/np_utils.py` & `phdu-1.9b4/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu/pd_utils.py` & `phdu-1.9b4/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu/plots/base.py` & `phdu-1.9b4/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu/plots/plotly_utils.py` & `phdu-1.9b4/phdu/plots/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu/script_fmt.py` & `phdu-1.9b4/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu/stats/_integration.py` & `phdu-1.9b4/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu/stats/_plots.py` & `phdu-1.9b4/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu/stats/bootstrap.py` & `phdu-1.9b4/phdu/stats/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -629,54 +629,71 @@
         power = 1 - fail_low - fail_high
         results['violations-low'].append(fail_low)
         results['violations-high'].append(fail_high)
         results['power'].append(power)
     return pd.DataFrame(results, index=N_values)
 
 def power_analysis(data, statistic, low, high, output_len=1, N_values=np.array([5, 10, 25, 50, 100, 200]), recenter=False, seed=0, seed_N=int(1e9),
-                   R=int(1e4), R_se=int(1e5), R_se_nested=int(1e3), R_N=int(1e4), alpha_low=0.05, alpha_high=0.05):
+                   R=int(1e4), R_se=int(1e5), R_se_nested=int(1e3), R_N=int(1e3), alpha_low=0.05, alpha_high=0.05, method='percentile', exact_CI_p=None):
     """
-    Stable bootstrap power and sample-size calculation for accepting H0 with confidence (1 - alpha_low - alpha_high).
+    Stable bootstrap power and sample-size calculation for accepting
+        H0: stat in [low, high] with confidence (1 - alpha_low - alpha_high).
+
     Computes violations on the studentized equivalent for the low and high bound of H0.
-    Takes into account the variability in the original sample (size n):   bootstrap estimate, SE of the bootstrap estimate.
-                                     and in the future sample (size N):   bootstrap estimate.
+    Takes into account the variability in
+            the original sample (size n):        bootstrap estimate, SE of the bootstrap estimate.
+            and in the future sample (size N):   bootstrap quantile estimate.
     See Efron-Tshibirani: An introduction to the bootstrap,  p. 381-384.
 
     Returns: dataframe with index=N_values, columns=[low_fails, high_fails, power].
     """
+    seed_n = seed+1
+    seed_N = seed+2
+    seed_n_se = seed+3
+
     n = data.shape[0]
     if n not in N_values:
         N_values = np.sort(np.hstack((n, N_values)))
     base = statistic(data)
     se_estimate = np.sqrt(np.diag(cov(resample_nb(data, statistic, seed=seed, R=R_se, output_len=output_len),
                                       base,
                                       recenter=recenter)
                                  ))
     low_studentized = (base - low) / se_estimate
     high_studentized = (base - high) / se_estimate
 
     # Estimation of SE (datasize = n). This is the computational bottleneck.
-    data_n = resample_nb_X(data, R=R, seed=seed+1)
+    data_n = resample_nb_X(data, R=R, seed=seed_n)
     se_estimate_n = np.empty((R, output_len))
     estimate_n = np.empty((R, output_len))
     for i, d_n in enumerate(tqdm(data_n)):
         estimate_n_i = statistic(d_n)
-        nested_estimate_n = resample_nb(d_n, statistic, seed=seed+3+i, R=R_se_nested, output_len=output_len)
+        nested_estimate_n = resample_nb(d_n, statistic, seed=seed_n_se+i, R=R_se_nested, output_len=output_len)
         estimate_n[i] = estimate_n_i
         se_estimate_n[i] = np.sqrt(np.diag(cov(nested_estimate_n, estimate_n_i, recenter=recenter)))
 
     # Violations of studentized endpoints.
     results = defaultdict(list)
+    np.random.seed(seed_N)
     for N in N_values:
         estimate_N_low = np.empty((R, output_len))
         estimate_N_high = np.empty((R, output_len))
         for i in range(R):
-            estimate_N = resample_nb(data, statistic, N=N, R=R_N, seed=seed_N+i, output_len=output_len)
-            estimate_N_low[i] = np.percentile(estimate_N, 100*alpha_low, axis=0)
-            estimate_N_high[i] = np.percentile(estimate_N, 100*(1-alpha_high), axis=0)
+            data_N = data[np.random.randint(0, n, size=N)]
+            if method == 'exact':
+                if exact_CI_p is None:
+                    raise ValueError('exact_CI_p must be specified for exact method.')
+                estimate_N_low[i] = conf_interval.ci_percentile_equal_tailed(data_N, exact_CI_p, alpha=alpha_low, alternative='less')[0][1]
+                estimate_N_high[i] = conf_interval.ci_percentile_equal_tailed(data_N, exact_CI_p, alpha=1-alpha_high, alternative='less')[0][1]
+            elif method == 'percentile':
+                estimate_N = resample_nb(data_N, statistic, R=R_N, seed=seed_N+i, output_len=output_len)
+                estimate_N_low[i] = np.percentile(estimate_N, 100*alpha_low, axis=0)
+                estimate_N_high[i] = np.percentile(estimate_N, 100*(1-alpha_high), axis=0)
+            else:
+                raise ValueError('method must be either "exact" or "percentile".')
         T_l = (estimate_n - estimate_N_low) / se_estimate_n
         T_h = (estimate_n - estimate_N_high) / se_estimate_n
         low_violations = (T_l > low_studentized).mean()
         high_violations = (T_h < high_studentized).mean()
         # power = 1 - low_violations - high_violations. Wrong, there can be overlap
         power = 1 - ( (T_l > low_studentized) | (T_h < high_studentized) ).mean()
         results['violations-low'].append(low_violations)
```

### Comparing `phdu-1.9b3/phdu/stats/conf_interval.py` & `phdu-1.9b4/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu/stats/corr.py` & `phdu-1.9b4/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu/stats/rtopy/_helper.py` & `phdu-1.9b4/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu/stats/rtopy/resample.py` & `phdu-1.9b4/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu/stats/test/permutation.py` & `phdu-1.9b4/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu/storage.py` & `phdu-1.9b4/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/phdu.egg-info/PKG-INFO` & `phdu-1.9b4/phdu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.9b3
+Version: 1.9b4
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.9b3/phdu.egg-info/SOURCES.txt` & `phdu-1.9b4/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-1.9b3/setup.py` & `phdu-1.9b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='1.9.b3',
+    version='1.9.b4',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```

