# Comparing `tmp/phdu-1.9b6.tar.gz` & `tmp/phdu-1.9b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-1.9b6.tar", last modified: Tue May  9 09:28:15 2023, max compression
+gzip compressed data, was "phdu-1.9b7.tar", last modified: Tue May  9 09:35:22 2023, max compression
```

## Comparing `phdu-1.9b6.tar` & `phdu-1.9b7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:28:15.596774 phdu-1.9b6/
--rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-1.9b6/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-05-09 09:28:15.596774 phdu-1.9b6/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-1.9b6/README.md
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:28:15.516770 phdu-1.9b6/phdu/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-1.9b6/phdu/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-1.9b6/phdu/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-1.9b6/phdu/clustering.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-1.9b6/phdu/decomposition.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-1.9b6/phdu/np_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-1.9b6/phdu/pd_utils.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:28:15.548772 phdu-1.9b6/phdu/plots/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-1.9b6/phdu/plots/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-1.9b6/phdu/plots/_mpl.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-1.9b6/phdu/plots/base.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    14203 2023-05-04 17:25:49.000000 phdu-1.9b6/phdu/plots/plotly_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-1.9b6/phdu/script_fmt.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:28:15.572773 phdu-1.9b6/phdu/stats/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-1.9b6/phdu/stats/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-1.9b6/phdu/stats/_integration.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-1.9b6/phdu/stats/_plots.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-1.9b6/phdu/stats/_preprocess.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    31904 2023-05-09 09:27:43.000000 phdu-1.9b6/phdu/stats/bootstrap.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-1.9b6/phdu/stats/conf_interval.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-1.9b6/phdu/stats/corr.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:28:15.580773 phdu-1.9b6/phdu/stats/rtopy/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-1.9b6/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-1.9b6/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-1.9b6/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:28:15.592774 phdu-1.9b6/phdu/stats/test/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-1.9b6/phdu/stats/test/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-1.9b6/phdu/stats/test/_adherence.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-1.9b6/phdu/stats/test/permutation.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4179 2023-04-25 11:08:38.000000 phdu-1.9b6/phdu/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:28:15.532771 phdu-1.9b6/phdu.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-05-09 09:28:15.000000 phdu-1.9b6/phdu.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-05-09 09:28:15.000000 phdu-1.9b6/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-05-09 09:28:15.000000 phdu-1.9b6/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-05-09 09:28:15.000000 phdu-1.9b6/phdu.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-05-09 09:28:15.000000 phdu-1.9b6/phdu.egg-info/top_level.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-05-09 09:28:15.604775 phdu-1.9b6/setup.cfg
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-05-09 09:28:04.000000 phdu-1.9b6/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:35:22.577280 phdu-1.9b7/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-1.9b7/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-05-09 09:35:22.577280 phdu-1.9b7/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-1.9b7/README.md
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:35:22.529278 phdu-1.9b7/phdu/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-1.9b7/phdu/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-1.9b7/phdu/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-1.9b7/phdu/clustering.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-1.9b7/phdu/decomposition.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-1.9b7/phdu/np_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-1.9b7/phdu/pd_utils.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:35:22.549279 phdu-1.9b7/phdu/plots/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-1.9b7/phdu/plots/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-1.9b7/phdu/plots/_mpl.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-1.9b7/phdu/plots/base.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    14203 2023-05-04 17:25:49.000000 phdu-1.9b7/phdu/plots/plotly_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-1.9b7/phdu/script_fmt.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:35:22.565280 phdu-1.9b7/phdu/stats/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-1.9b7/phdu/stats/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-1.9b7/phdu/stats/_integration.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-1.9b7/phdu/stats/_plots.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-1.9b7/phdu/stats/_preprocess.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    31946 2023-05-09 09:32:43.000000 phdu-1.9b7/phdu/stats/bootstrap.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-1.9b7/phdu/stats/conf_interval.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-1.9b7/phdu/stats/corr.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:35:22.569280 phdu-1.9b7/phdu/stats/rtopy/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-1.9b7/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-1.9b7/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-1.9b7/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:35:22.573280 phdu-1.9b7/phdu/stats/test/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-1.9b7/phdu/stats/test/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-1.9b7/phdu/stats/test/_adherence.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-1.9b7/phdu/stats/test/permutation.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4179 2023-04-25 11:08:38.000000 phdu-1.9b7/phdu/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:35:22.545279 phdu-1.9b7/phdu.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-05-09 09:35:22.000000 phdu-1.9b7/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-05-09 09:35:22.000000 phdu-1.9b7/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-05-09 09:35:22.000000 phdu-1.9b7/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-05-09 09:35:22.000000 phdu-1.9b7/phdu.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-05-09 09:35:22.000000 phdu-1.9b7/phdu.egg-info/top_level.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-05-09 09:35:22.581281 phdu-1.9b7/setup.cfg
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-05-09 09:35:10.000000 phdu-1.9b7/setup.py
```

### Comparing `phdu-1.9b6/LICENSE.md` & `phdu-1.9b7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/PKG-INFO` & `phdu-1.9b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.9b6
+Version: 1.9b7
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.9b6/README.md` & `phdu-1.9b7/README.md`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu/_helper.py` & `phdu-1.9b7/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu/clustering.py` & `phdu-1.9b7/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu/decomposition.py` & `phdu-1.9b7/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu/np_utils.py` & `phdu-1.9b7/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu/pd_utils.py` & `phdu-1.9b7/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu/plots/base.py` & `phdu-1.9b7/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu/plots/plotly_utils.py` & `phdu-1.9b7/phdu/plots/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu/script_fmt.py` & `phdu-1.9b7/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu/stats/_integration.py` & `phdu-1.9b7/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu/stats/_plots.py` & `phdu-1.9b7/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu/stats/bootstrap.py` & `phdu-1.9b7/phdu/stats/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -629,15 +629,15 @@
         power = 1 - fail_low - fail_high
         results['violations-low'].append(fail_low)
         results['violations-high'].append(fail_high)
         results['power'].append(power)
     return pd.DataFrame(results, index=N_values)
 
 def power_analysis(data, statistic, low, high, output_len=1, N_values=np.array([5, 10, 25, 50, 100, 200]), recenter=False, seed=0, seed_N=int(1e9),
-                   R=int(1e4), R_se=int(1e5), R_se_nested=int(1e3), R_N=int(1e3), alpha_low=0.05, alpha_high=0.05, method='percentile', exact_CI_p=None):
+                   R=int(1e4), R_se=int(1e5), R_se_nested=int(1e3), R_N=int(1e3), alpha_low=0.05, alpha_high=0.05, method='percentile', exact_CI_p=None, tol=1e-8):
     """
     Stable bootstrap power and sample-size calculation for accepting
         H0: stat in [low, high] with confidence (1 - alpha_low - alpha_high).
 
     Computes violations on the studentized equivalent for the low and high bound of H0.
     Takes into account the variability in
             the original sample (size n):        bootstrap estimate, SE of the bootstrap estimate.
@@ -654,16 +654,16 @@
     if n not in N_values:
         N_values = np.sort(np.hstack((n, N_values)))
     base = statistic(data)
     se_estimate = np.sqrt(np.diag(cov(resample_nb(data, statistic, seed=seed, R=R_se, output_len=output_len),
                                       base,
                                       recenter=recenter)
                                  ))
-    low_studentized = (base - low) / se_estimate
-    high_studentized = (base - high) / se_estimate
+    low_studentized = (base - low) / (se_estimate + tol)
+    high_studentized = (base - high) / (se_estimate + tol)
 
     # Estimation of SE (datasize = n). This is the computational bottleneck.
     data_n = resample_nb_X(data, R=R, seed=seed_n)
     se_estimate_n = np.empty((R, output_len))
     estimate_n = np.empty((R, output_len))
     for i, d_n in enumerate(tqdm(data_n)):
         estimate_n_i = statistic(d_n)
@@ -687,16 +687,16 @@
                 estimate_N_high[i] = conf_interval.ci_percentile_equal_tailed(data_N, exact_CI_p, alpha=alpha_high, alternative='less')[0][1]
             elif method == 'percentile':
                 estimate_N = resample_nb(data_N, statistic, R=R_N, seed=seed_N+i, output_len=output_len)
                 estimate_N_low[i] = np.percentile(estimate_N, 100*alpha_low, axis=0)
                 estimate_N_high[i] = np.percentile(estimate_N, 100*(1-alpha_high), axis=0)
             else:
                 raise ValueError('method must be either "exact" or "percentile".')
-        T_l = (estimate_n - estimate_N_low) / se_estimate_n
-        T_h = (estimate_n - estimate_N_high) / se_estimate_n
+        T_l = (estimate_n - estimate_N_low) / (se_estimate_n + tol)
+        T_h = (estimate_n - estimate_N_high) / (se_estimate_n + tol)
         low_violations = (T_l > low_studentized).mean()
         high_violations = (T_h < high_studentized).mean()
         # power = 1 - low_violations - high_violations. Wrong, there can be overlap
         power = 1 - ( (T_l > low_studentized) | (T_h < high_studentized) ).mean()
         results['violations-low'].append(low_violations)
         results['violations-high'].append(high_violations)
         results['power'].append(power)
```

### Comparing `phdu-1.9b6/phdu/stats/conf_interval.py` & `phdu-1.9b7/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu/stats/corr.py` & `phdu-1.9b7/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu/stats/rtopy/_helper.py` & `phdu-1.9b7/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu/stats/rtopy/resample.py` & `phdu-1.9b7/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu/stats/test/permutation.py` & `phdu-1.9b7/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu/storage.py` & `phdu-1.9b7/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/phdu.egg-info/PKG-INFO` & `phdu-1.9b7/phdu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.9b6
+Version: 1.9b7
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.9b6/phdu.egg-info/SOURCES.txt` & `phdu-1.9b7/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-1.9b6/setup.py` & `phdu-1.9b7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='1.9.b6',
+    version='1.9.b7',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```

