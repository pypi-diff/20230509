# Comparing `tmp/antspymm-0.9.4.tar.gz` & `tmp/antspymm-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antspymm-0.9.4.tar", last modified: Tue May  9 12:40:49 2023, max compression
+gzip compressed data, was "antspymm-0.9.5.tar", last modified: Tue May  9 16:05:48 2023, max compression
```

## Comparing `antspymm-0.9.4.tar` & `antspymm-0.9.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 12:40:49.683468 antspymm-0.9.4/
--rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-01 09:20:32.000000 antspymm-0.9.4/LICENSE
--rw-r--r--   0 stnava     (501) staff       (20)       33 2023-01-29 13:38:57.000000 antspymm-0.9.4/MANIFEST.in
--rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-05-09 12:40:49.683170 antspymm-0.9.4/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)     9827 2023-04-12 13:23:21.000000 antspymm-0.9.4/README.md
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 12:40:49.668983 antspymm-0.9.4/antspymm/
--rw-r--r--   0 stnava     (501) staff       (20)     2690 2023-03-20 11:54:16.000000 antspymm-0.9.4/antspymm/__init__.py
--rw-r--r--   0 stnava     (501) staff       (20)   284838 2023-05-09 12:38:11.000000 antspymm-0.9.4/antspymm/mm.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 12:40:49.670648 antspymm-0.9.4/antspymm.egg-info/
--rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-05-09 12:40:49.000000 antspymm-0.9.4/antspymm.egg-info/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)      789 2023-05-09 12:40:49.000000 antspymm-0.9.4/antspymm.egg-info/SOURCES.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-05-09 12:40:49.000000 antspymm-0.9.4/antspymm.egg-info/dependency_links.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-05-09 12:40:49.000000 antspymm-0.9.4/antspymm.egg-info/not-zip-safe
--rw-r--r--   0 stnava     (501) staff       (20)      112 2023-05-09 12:40:49.000000 antspymm-0.9.4/antspymm.egg-info/requires.txt
--rw-r--r--   0 stnava     (501) staff       (20)        9 2023-05-09 12:40:49.000000 antspymm-0.9.4/antspymm.egg-info/top_level.txt
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 12:40:49.677100 antspymm-0.9.4/docs/
--rw-r--r--   0 stnava     (501) staff       (20)  1939802 2023-01-29 13:48:53.000000 antspymm-0.9.4/docs/antspymm_data_dictionary.csv
--rw-r--r--   0 stnava     (501) staff       (20)      567 2023-04-12 13:06:30.000000 antspymm-0.9.4/docs/bids_cohort_example.py
--rw-r--r--   0 stnava     (501) staff       (20)     1296 2023-04-08 18:52:17.000000 antspymm-0.9.4/docs/example_run_from_directory.py
--rw-r--r--   0 stnava     (501) staff       (20)      478 2023-02-19 10:57:50.000000 antspymm-0.9.4/docs/make_dict_table.Rmd
--rw-r--r--   0 stnava     (501) staff       (20)      632 2023-04-12 13:06:30.000000 antspymm-0.9.4/docs/nrg_cohort_example.py
--rw-r--r--   0 stnava     (501) staff       (20)     2082 2023-03-20 13:00:28.000000 antspymm-0.9.4/docs/outlierness.py
--rw-r--r--   0 stnava     (501) staff       (20)     3643 2023-04-15 22:47:31.000000 antspymm-0.9.4/docs/ukbb_to_nrg_processing.py
--rw-r--r--   0 stnava     (501) staff       (20)     4546 2023-04-16 12:24:12.000000 antspymm-0.9.4/docs/ukbb_to_nrg_processing2.py
--rw-r--r--   0 stnava     (501) staff       (20)       38 2023-05-09 12:40:49.683534 antspymm-0.9.4/setup.cfg
--rw-r--r--   0 stnava     (501) staff       (20)      681 2023-05-09 12:40:22.000000 antspymm-0.9.4/setup.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 12:40:49.682579 antspymm-0.9.4/tests/
--rw-r--r--   0 stnava     (501) staff       (20)     5589 2022-10-21 12:35:02.000000 antspymm-0.9.4/tests/mm.py
--rw-r--r--   0 stnava     (501) staff       (20)     2087 2022-12-17 20:51:01.000000 antspymm-0.9.4/tests/mm_nrg.py
--rw-r--r--   0 stnava     (501) staff       (20)      440 2023-03-15 12:39:26.000000 antspymm-0.9.4/tests/test_bids_2_nrg.py
--rw-r--r--   0 stnava     (501) staff       (20)      394 2022-06-09 14:57:05.000000 antspymm-0.9.4/tests/test_dti_recon.py
--rw-r--r--   0 stnava     (501) staff       (20)     1500 2023-05-01 14:47:40.000000 antspymm-0.9.4/tests/test_dti_reg.py
--rw-r--r--   0 stnava     (501) staff       (20)     2507 2023-02-05 20:18:30.000000 antspymm-0.9.4/tests/test_dwi_run.py
--rw-r--r--   0 stnava     (501) staff       (20)      445 2023-02-05 00:06:28.000000 antspymm-0.9.4/tests/test_flair_run.py
--rw-r--r--   0 stnava     (501) staff       (20)     3368 2023-05-02 12:19:49.000000 antspymm-0.9.4/tests/test_joint_dti_recon.py
--rw-r--r--   0 stnava     (501) staff       (20)     1497 2023-03-15 12:44:41.000000 antspymm-0.9.4/tests/test_mm_csv.py
--rw-r--r--   0 stnava     (501) staff       (20)     2101 2022-11-16 16:52:51.000000 antspymm-0.9.4/tests/test_rsfmri_run.py
--rw-r--r--   0 stnava     (501) staff       (20)      762 2023-05-05 18:29:30.000000 antspymm-0.9.4/tests/test_ukbb_rsfmri.py
--rw-r--r--   0 stnava     (501) staff       (20)      597 2021-11-02 19:50:00.000000 antspymm-0.9.4/tests/testsr.py
--rw-r--r--   0 stnava     (501) staff       (20)     1439 2023-03-02 15:01:53.000000 antspymm-0.9.4/tests/visualize_tractogram.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 16:05:48.613791 antspymm-0.9.5/
+-rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-01 09:20:32.000000 antspymm-0.9.5/LICENSE
+-rw-r--r--   0 stnava     (501) staff       (20)       33 2023-01-29 13:38:57.000000 antspymm-0.9.5/MANIFEST.in
+-rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-05-09 16:05:48.613547 antspymm-0.9.5/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)     9827 2023-04-12 13:23:21.000000 antspymm-0.9.5/README.md
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 16:05:48.600387 antspymm-0.9.5/antspymm/
+-rw-r--r--   0 stnava     (501) staff       (20)     2690 2023-03-20 11:54:16.000000 antspymm-0.9.5/antspymm/__init__.py
+-rw-r--r--   0 stnava     (501) staff       (20)   284817 2023-05-09 16:03:22.000000 antspymm-0.9.5/antspymm/mm.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 16:05:48.601873 antspymm-0.9.5/antspymm.egg-info/
+-rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-05-09 16:05:48.000000 antspymm-0.9.5/antspymm.egg-info/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)      789 2023-05-09 16:05:48.000000 antspymm-0.9.5/antspymm.egg-info/SOURCES.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-05-09 16:05:48.000000 antspymm-0.9.5/antspymm.egg-info/dependency_links.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-05-09 16:05:48.000000 antspymm-0.9.5/antspymm.egg-info/not-zip-safe
+-rw-r--r--   0 stnava     (501) staff       (20)      112 2023-05-09 16:05:48.000000 antspymm-0.9.5/antspymm.egg-info/requires.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        9 2023-05-09 16:05:48.000000 antspymm-0.9.5/antspymm.egg-info/top_level.txt
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 16:05:48.608234 antspymm-0.9.5/docs/
+-rw-r--r--   0 stnava     (501) staff       (20)  1939802 2023-01-29 13:48:53.000000 antspymm-0.9.5/docs/antspymm_data_dictionary.csv
+-rw-r--r--   0 stnava     (501) staff       (20)      567 2023-04-12 13:06:30.000000 antspymm-0.9.5/docs/bids_cohort_example.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1296 2023-04-08 18:52:17.000000 antspymm-0.9.5/docs/example_run_from_directory.py
+-rw-r--r--   0 stnava     (501) staff       (20)      478 2023-02-19 10:57:50.000000 antspymm-0.9.5/docs/make_dict_table.Rmd
+-rw-r--r--   0 stnava     (501) staff       (20)      632 2023-04-12 13:06:30.000000 antspymm-0.9.5/docs/nrg_cohort_example.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2082 2023-03-20 13:00:28.000000 antspymm-0.9.5/docs/outlierness.py
+-rw-r--r--   0 stnava     (501) staff       (20)     3643 2023-04-15 22:47:31.000000 antspymm-0.9.5/docs/ukbb_to_nrg_processing.py
+-rw-r--r--   0 stnava     (501) staff       (20)     4546 2023-04-16 12:24:12.000000 antspymm-0.9.5/docs/ukbb_to_nrg_processing2.py
+-rw-r--r--   0 stnava     (501) staff       (20)       38 2023-05-09 16:05:48.613856 antspymm-0.9.5/setup.cfg
+-rw-r--r--   0 stnava     (501) staff       (20)      681 2023-05-09 16:04:53.000000 antspymm-0.9.5/setup.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 16:05:48.613024 antspymm-0.9.5/tests/
+-rw-r--r--   0 stnava     (501) staff       (20)     5589 2022-10-21 12:35:02.000000 antspymm-0.9.5/tests/mm.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2087 2022-12-17 20:51:01.000000 antspymm-0.9.5/tests/mm_nrg.py
+-rw-r--r--   0 stnava     (501) staff       (20)      440 2023-03-15 12:39:26.000000 antspymm-0.9.5/tests/test_bids_2_nrg.py
+-rw-r--r--   0 stnava     (501) staff       (20)      394 2022-06-09 14:57:05.000000 antspymm-0.9.5/tests/test_dti_recon.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1500 2023-05-01 14:47:40.000000 antspymm-0.9.5/tests/test_dti_reg.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2507 2023-02-05 20:18:30.000000 antspymm-0.9.5/tests/test_dwi_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)      445 2023-02-05 00:06:28.000000 antspymm-0.9.5/tests/test_flair_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)     3368 2023-05-02 12:19:49.000000 antspymm-0.9.5/tests/test_joint_dti_recon.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1497 2023-03-15 12:44:41.000000 antspymm-0.9.5/tests/test_mm_csv.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2101 2022-11-16 16:52:51.000000 antspymm-0.9.5/tests/test_rsfmri_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)      762 2023-05-05 18:29:30.000000 antspymm-0.9.5/tests/test_ukbb_rsfmri.py
+-rw-r--r--   0 stnava     (501) staff       (20)      597 2021-11-02 19:50:00.000000 antspymm-0.9.5/tests/testsr.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1439 2023-03-02 15:01:53.000000 antspymm-0.9.5/tests/visualize_tractogram.py
```

### Comparing `antspymm-0.9.4/LICENSE` & `antspymm-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/PKG-INFO` & `antspymm-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspymm
-Version: 0.9.4
+Version: 0.9.5
 Summary: multi-channel/time-series medical image processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyMM
 Author: Avants, Gosselin, Tustison, Reardon
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
```

### Comparing `antspymm-0.9.4/README.md` & `antspymm-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/antspymm/__init__.py` & `antspymm-0.9.5/antspymm/__init__.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/antspymm/mm.py` & `antspymm-0.9.5/antspymm/mm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1254,21 +1254,21 @@
 
     if verbose:
         print("begin global distortion correction")
     # initrig = tra_initializer(avg_b0, ab0, max_rotation=60, transform=['rigid'], verbose=verbose)
     if mask_csf:
         bcsf = ants.threshold_image( avg_b0,"Otsu",2).threshold_image(1,1).morphology("open",1).iMath("GetLargestComponent")
     else:
-        bcsf = avg_b0[0] * 0 + 1
+        bcsf = ab0 * 0 + 1
 
-    initrig = ants.registration( avg_b0, ab0*bcsf,'BOLDRigid',outprefix=ofnG)
-    deftx = ants.registration( avg_dwi, adw*bcsf, 'SyNOnly',
+    initrig = ants.registration( avg_b0, ab0,'BOLDRigid',outprefix=ofnG)
+    deftx = ants.registration( avg_dwi, adw, 'SyNOnly',
         syn_metric='CC', syn_sampling=2,
         reg_iterations=[50,50,20],
-        multivariate_extras=[ [ "CC", avg_b0, ab0*bcsf, 1, 2 ]],
+        multivariate_extras=[ [ "CC", avg_b0, ab0, 1, 2 ]],
         initial_transform=initrig['fwdtransforms'][0],
         outprefix=ofnG
         )['fwdtransforms']
     if verbose:
         print("end global distortion correction")
 
     if verbose:
```

### Comparing `antspymm-0.9.4/antspymm.egg-info/PKG-INFO` & `antspymm-0.9.5/antspymm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspymm
-Version: 0.9.4
+Version: 0.9.5
 Summary: multi-channel/time-series medical image processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyMM
 Author: Avants, Gosselin, Tustison, Reardon
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
```

### Comparing `antspymm-0.9.4/antspymm.egg-info/SOURCES.txt` & `antspymm-0.9.5/antspymm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/docs/antspymm_data_dictionary.csv` & `antspymm-0.9.5/docs/antspymm_data_dictionary.csv`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/docs/bids_cohort_example.py` & `antspymm-0.9.5/docs/bids_cohort_example.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/docs/example_run_from_directory.py` & `antspymm-0.9.5/docs/example_run_from_directory.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/docs/nrg_cohort_example.py` & `antspymm-0.9.5/docs/nrg_cohort_example.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/docs/outlierness.py` & `antspymm-0.9.5/docs/outlierness.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/docs/ukbb_to_nrg_processing.py` & `antspymm-0.9.5/docs/ukbb_to_nrg_processing.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/docs/ukbb_to_nrg_processing2.py` & `antspymm-0.9.5/docs/ukbb_to_nrg_processing2.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/setup.py` & `antspymm-0.9.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = open("README.md").read()
 
 with open("./requirements.txt") as f:
       requirements = f.read().splitlines()
 
 setup(name='antspymm',
-      version='0.9.4',
+      version='0.9.5',
       description='multi-channel/time-series medical image processing with antspyx',
       long_description=long_description,
       long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
       url='https://github.com/stnava/ANTsPyMM',
       author='Avants, Gosselin, Tustison, Reardon',
       author_email='stnava@gmail.com',
       license='Apache 2.0',
```

### Comparing `antspymm-0.9.4/tests/mm.py` & `antspymm-0.9.5/tests/mm.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/tests/mm_nrg.py` & `antspymm-0.9.5/tests/mm_nrg.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/tests/test_dti_reg.py` & `antspymm-0.9.5/tests/test_dti_reg.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/tests/test_dwi_run.py` & `antspymm-0.9.5/tests/test_dwi_run.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/tests/test_joint_dti_recon.py` & `antspymm-0.9.5/tests/test_joint_dti_recon.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/tests/test_mm_csv.py` & `antspymm-0.9.5/tests/test_mm_csv.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/tests/test_rsfmri_run.py` & `antspymm-0.9.5/tests/test_rsfmri_run.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/tests/test_ukbb_rsfmri.py` & `antspymm-0.9.5/tests/test_ukbb_rsfmri.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/tests/testsr.py` & `antspymm-0.9.5/tests/testsr.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.4/tests/visualize_tractogram.py` & `antspymm-0.9.5/tests/visualize_tractogram.py`

 * *Files identical despite different names*

