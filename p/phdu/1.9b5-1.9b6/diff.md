# Comparing `tmp/phdu-1.9b5.tar.gz` & `tmp/phdu-1.9b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-1.9b5.tar", last modified: Tue May  9 09:16:46 2023, max compression
+gzip compressed data, was "phdu-1.9b6.tar", last modified: Tue May  9 09:28:15 2023, max compression
```

## Comparing `phdu-1.9b5.tar` & `phdu-1.9b6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:16:46.935725 phdu-1.9b5/
--rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-1.9b5/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-05-09 09:16:46.939725 phdu-1.9b5/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-1.9b5/README.md
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:16:46.803718 phdu-1.9b5/phdu/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-1.9b5/phdu/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-1.9b5/phdu/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-1.9b5/phdu/clustering.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-1.9b5/phdu/decomposition.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-1.9b5/phdu/np_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-1.9b5/phdu/pd_utils.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:16:46.859721 phdu-1.9b5/phdu/plots/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-1.9b5/phdu/plots/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-1.9b5/phdu/plots/_mpl.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-1.9b5/phdu/plots/base.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    14203 2023-05-04 17:25:49.000000 phdu-1.9b5/phdu/plots/plotly_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-1.9b5/phdu/script_fmt.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:16:46.895723 phdu-1.9b5/phdu/stats/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-1.9b5/phdu/stats/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-1.9b5/phdu/stats/_integration.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-1.9b5/phdu/stats/_plots.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-1.9b5/phdu/stats/_preprocess.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    31903 2023-05-09 09:16:26.000000 phdu-1.9b5/phdu/stats/bootstrap.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-1.9b5/phdu/stats/conf_interval.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-1.9b5/phdu/stats/corr.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:16:46.919724 phdu-1.9b5/phdu/stats/rtopy/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-1.9b5/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-1.9b5/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-1.9b5/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:16:46.935725 phdu-1.9b5/phdu/stats/test/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-1.9b5/phdu/stats/test/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-1.9b5/phdu/stats/test/_adherence.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-1.9b5/phdu/stats/test/permutation.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4179 2023-04-25 11:08:38.000000 phdu-1.9b5/phdu/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:16:46.839720 phdu-1.9b5/phdu.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-05-09 09:16:46.000000 phdu-1.9b5/phdu.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-05-09 09:16:46.000000 phdu-1.9b5/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-05-09 09:16:46.000000 phdu-1.9b5/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-05-09 09:16:46.000000 phdu-1.9b5/phdu.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-05-09 09:16:46.000000 phdu-1.9b5/phdu.egg-info/top_level.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-05-09 09:16:46.943725 phdu-1.9b5/setup.cfg
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-05-09 09:16:36.000000 phdu-1.9b5/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:28:15.596774 phdu-1.9b6/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-1.9b6/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-05-09 09:28:15.596774 phdu-1.9b6/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-1.9b6/README.md
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:28:15.516770 phdu-1.9b6/phdu/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-1.9b6/phdu/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-1.9b6/phdu/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-1.9b6/phdu/clustering.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-1.9b6/phdu/decomposition.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-1.9b6/phdu/np_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-1.9b6/phdu/pd_utils.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:28:15.548772 phdu-1.9b6/phdu/plots/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-1.9b6/phdu/plots/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-1.9b6/phdu/plots/_mpl.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-1.9b6/phdu/plots/base.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    14203 2023-05-04 17:25:49.000000 phdu-1.9b6/phdu/plots/plotly_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-1.9b6/phdu/script_fmt.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:28:15.572773 phdu-1.9b6/phdu/stats/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-1.9b6/phdu/stats/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-1.9b6/phdu/stats/_integration.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-1.9b6/phdu/stats/_plots.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-1.9b6/phdu/stats/_preprocess.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    31904 2023-05-09 09:27:43.000000 phdu-1.9b6/phdu/stats/bootstrap.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-1.9b6/phdu/stats/conf_interval.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-1.9b6/phdu/stats/corr.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:28:15.580773 phdu-1.9b6/phdu/stats/rtopy/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-1.9b6/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-1.9b6/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-1.9b6/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:28:15.592774 phdu-1.9b6/phdu/stats/test/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-1.9b6/phdu/stats/test/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-1.9b6/phdu/stats/test/_adherence.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-1.9b6/phdu/stats/test/permutation.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4179 2023-04-25 11:08:38.000000 phdu-1.9b6/phdu/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-09 09:28:15.532771 phdu-1.9b6/phdu.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-05-09 09:28:15.000000 phdu-1.9b6/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-05-09 09:28:15.000000 phdu-1.9b6/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-05-09 09:28:15.000000 phdu-1.9b6/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-05-09 09:28:15.000000 phdu-1.9b6/phdu.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-05-09 09:28:15.000000 phdu-1.9b6/phdu.egg-info/top_level.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-05-09 09:28:15.604775 phdu-1.9b6/setup.cfg
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-05-09 09:28:04.000000 phdu-1.9b6/setup.py
```

### Comparing `phdu-1.9b5/LICENSE.md` & `phdu-1.9b6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/PKG-INFO` & `phdu-1.9b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.9b5
+Version: 1.9b6
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.9b5/README.md` & `phdu-1.9b6/README.md`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu/_helper.py` & `phdu-1.9b6/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu/clustering.py` & `phdu-1.9b6/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu/decomposition.py` & `phdu-1.9b6/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu/np_utils.py` & `phdu-1.9b6/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu/pd_utils.py` & `phdu-1.9b6/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu/plots/base.py` & `phdu-1.9b6/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu/plots/plotly_utils.py` & `phdu-1.9b6/phdu/plots/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu/script_fmt.py` & `phdu-1.9b6/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu/stats/_integration.py` & `phdu-1.9b6/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu/stats/_plots.py` & `phdu-1.9b6/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu/stats/bootstrap.py` & `phdu-1.9b6/phdu/stats/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -679,16 +679,16 @@
         estimate_N_high = np.empty((R, output_len))
         for i in range(R):
             data_N = data[np.random.randint(0, n, size=N)]
             if method == 'exact':
                 data_N = data_N.squeeze()
                 if exact_CI_p is None:
                     raise ValueError('exact_CI_p must be specified for exact method.')
-                estimate_N_low[i] = conf_interval.ci_percentile_equal_tailed(data_N, exact_CI_p, alpha=alpha_low, alternative='less')[0][1]
-                estimate_N_high[i] = conf_interval.ci_percentile_equal_tailed(data_N, exact_CI_p, alpha=1-alpha_high, alternative='less')[0][1]
+                estimate_N_low[i] = conf_interval.ci_percentile_equal_tailed(data_N, exact_CI_p, alpha=alpha_low, alternative='greater')[0][0]
+                estimate_N_high[i] = conf_interval.ci_percentile_equal_tailed(data_N, exact_CI_p, alpha=alpha_high, alternative='less')[0][1]
             elif method == 'percentile':
                 estimate_N = resample_nb(data_N, statistic, R=R_N, seed=seed_N+i, output_len=output_len)
                 estimate_N_low[i] = np.percentile(estimate_N, 100*alpha_low, axis=0)
                 estimate_N_high[i] = np.percentile(estimate_N, 100*(1-alpha_high), axis=0)
             else:
                 raise ValueError('method must be either "exact" or "percentile".')
         T_l = (estimate_n - estimate_N_low) / se_estimate_n
```

### Comparing `phdu-1.9b5/phdu/stats/conf_interval.py` & `phdu-1.9b6/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu/stats/corr.py` & `phdu-1.9b6/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu/stats/rtopy/_helper.py` & `phdu-1.9b6/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu/stats/rtopy/resample.py` & `phdu-1.9b6/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu/stats/test/permutation.py` & `phdu-1.9b6/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu/storage.py` & `phdu-1.9b6/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/phdu.egg-info/PKG-INFO` & `phdu-1.9b6/phdu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.9b5
+Version: 1.9b6
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.9b5/phdu.egg-info/SOURCES.txt` & `phdu-1.9b6/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-1.9b5/setup.py` & `phdu-1.9b6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='1.9.b5',
+    version='1.9.b6',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```

