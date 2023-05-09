# Comparing `tmp/antspymm-0.9.2.tar.gz` & `tmp/antspymm-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antspymm-0.9.2.tar", last modified: Fri May  5 18:32:37 2023, max compression
+gzip compressed data, was "antspymm-0.9.3.tar", last modified: Tue May  9 10:41:05 2023, max compression
```

## Comparing `antspymm-0.9.2.tar` & `antspymm-0.9.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-05 18:32:37.005564 antspymm-0.9.2/
--rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-01 09:20:32.000000 antspymm-0.9.2/LICENSE
--rw-r--r--   0 stnava     (501) staff       (20)       33 2023-01-29 13:38:57.000000 antspymm-0.9.2/MANIFEST.in
--rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-05-05 18:32:37.005158 antspymm-0.9.2/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)     9827 2023-04-12 13:23:21.000000 antspymm-0.9.2/README.md
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-05 18:32:36.986983 antspymm-0.9.2/antspymm/
--rw-r--r--   0 stnava     (501) staff       (20)     2690 2023-03-20 11:54:16.000000 antspymm-0.9.2/antspymm/__init__.py
--rw-r--r--   0 stnava     (501) staff       (20)   284852 2023-05-05 18:23:38.000000 antspymm-0.9.2/antspymm/mm.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-05 18:32:36.989465 antspymm-0.9.2/antspymm.egg-info/
--rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-05-05 18:32:36.000000 antspymm-0.9.2/antspymm.egg-info/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)      789 2023-05-05 18:32:36.000000 antspymm-0.9.2/antspymm.egg-info/SOURCES.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-05-05 18:32:36.000000 antspymm-0.9.2/antspymm.egg-info/dependency_links.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-05-05 18:32:36.000000 antspymm-0.9.2/antspymm.egg-info/not-zip-safe
--rw-r--r--   0 stnava     (501) staff       (20)      112 2023-05-05 18:32:36.000000 antspymm-0.9.2/antspymm.egg-info/requires.txt
--rw-r--r--   0 stnava     (501) staff       (20)        9 2023-05-05 18:32:36.000000 antspymm-0.9.2/antspymm.egg-info/top_level.txt
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-05 18:32:36.997387 antspymm-0.9.2/docs/
--rw-r--r--   0 stnava     (501) staff       (20)  1939802 2023-01-29 13:48:53.000000 antspymm-0.9.2/docs/antspymm_data_dictionary.csv
--rw-r--r--   0 stnava     (501) staff       (20)      567 2023-04-12 13:06:30.000000 antspymm-0.9.2/docs/bids_cohort_example.py
--rw-r--r--   0 stnava     (501) staff       (20)     1296 2023-04-08 18:52:17.000000 antspymm-0.9.2/docs/example_run_from_directory.py
--rw-r--r--   0 stnava     (501) staff       (20)      478 2023-02-19 10:57:50.000000 antspymm-0.9.2/docs/make_dict_table.Rmd
--rw-r--r--   0 stnava     (501) staff       (20)      632 2023-04-12 13:06:30.000000 antspymm-0.9.2/docs/nrg_cohort_example.py
--rw-r--r--   0 stnava     (501) staff       (20)     2082 2023-03-20 13:00:28.000000 antspymm-0.9.2/docs/outlierness.py
--rw-r--r--   0 stnava     (501) staff       (20)     3643 2023-04-15 22:47:31.000000 antspymm-0.9.2/docs/ukbb_to_nrg_processing.py
--rw-r--r--   0 stnava     (501) staff       (20)     4546 2023-04-16 12:24:12.000000 antspymm-0.9.2/docs/ukbb_to_nrg_processing2.py
--rw-r--r--   0 stnava     (501) staff       (20)       38 2023-05-05 18:32:37.005651 antspymm-0.9.2/setup.cfg
--rw-r--r--   0 stnava     (501) staff       (20)      681 2023-05-05 18:19:33.000000 antspymm-0.9.2/setup.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-05 18:32:37.004406 antspymm-0.9.2/tests/
--rw-r--r--   0 stnava     (501) staff       (20)     5589 2022-10-21 12:35:02.000000 antspymm-0.9.2/tests/mm.py
--rw-r--r--   0 stnava     (501) staff       (20)     2087 2022-12-17 20:51:01.000000 antspymm-0.9.2/tests/mm_nrg.py
--rw-r--r--   0 stnava     (501) staff       (20)      440 2023-03-15 12:39:26.000000 antspymm-0.9.2/tests/test_bids_2_nrg.py
--rw-r--r--   0 stnava     (501) staff       (20)      394 2022-06-09 14:57:05.000000 antspymm-0.9.2/tests/test_dti_recon.py
--rw-r--r--   0 stnava     (501) staff       (20)     1500 2023-05-01 14:47:40.000000 antspymm-0.9.2/tests/test_dti_reg.py
--rw-r--r--   0 stnava     (501) staff       (20)     2507 2023-02-05 20:18:30.000000 antspymm-0.9.2/tests/test_dwi_run.py
--rw-r--r--   0 stnava     (501) staff       (20)      445 2023-02-05 00:06:28.000000 antspymm-0.9.2/tests/test_flair_run.py
--rw-r--r--   0 stnava     (501) staff       (20)     3368 2023-05-02 12:19:49.000000 antspymm-0.9.2/tests/test_joint_dti_recon.py
--rw-r--r--   0 stnava     (501) staff       (20)     1497 2023-03-15 12:44:41.000000 antspymm-0.9.2/tests/test_mm_csv.py
--rw-r--r--   0 stnava     (501) staff       (20)     2101 2022-11-16 16:52:51.000000 antspymm-0.9.2/tests/test_rsfmri_run.py
--rw-r--r--   0 stnava     (501) staff       (20)      762 2023-05-05 18:29:30.000000 antspymm-0.9.2/tests/test_ukbb_rsfmri.py
--rw-r--r--   0 stnava     (501) staff       (20)      597 2021-11-02 19:50:00.000000 antspymm-0.9.2/tests/testsr.py
--rw-r--r--   0 stnava     (501) staff       (20)     1439 2023-03-02 15:01:53.000000 antspymm-0.9.2/tests/visualize_tractogram.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 10:41:05.524414 antspymm-0.9.3/
+-rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-01 09:20:32.000000 antspymm-0.9.3/LICENSE
+-rw-r--r--   0 stnava     (501) staff       (20)       33 2023-01-29 13:38:57.000000 antspymm-0.9.3/MANIFEST.in
+-rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-05-09 10:41:05.524166 antspymm-0.9.3/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)     9827 2023-04-12 13:23:21.000000 antspymm-0.9.3/README.md
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 10:41:05.512287 antspymm-0.9.3/antspymm/
+-rw-r--r--   0 stnava     (501) staff       (20)     2690 2023-03-20 11:54:16.000000 antspymm-0.9.3/antspymm/__init__.py
+-rw-r--r--   0 stnava     (501) staff       (20)   284834 2023-05-09 10:38:20.000000 antspymm-0.9.3/antspymm/mm.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 10:41:05.513729 antspymm-0.9.3/antspymm.egg-info/
+-rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-05-09 10:41:05.000000 antspymm-0.9.3/antspymm.egg-info/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)      789 2023-05-09 10:41:05.000000 antspymm-0.9.3/antspymm.egg-info/SOURCES.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-05-09 10:41:05.000000 antspymm-0.9.3/antspymm.egg-info/dependency_links.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-05-09 10:41:05.000000 antspymm-0.9.3/antspymm.egg-info/not-zip-safe
+-rw-r--r--   0 stnava     (501) staff       (20)      112 2023-05-09 10:41:05.000000 antspymm-0.9.3/antspymm.egg-info/requires.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        9 2023-05-09 10:41:05.000000 antspymm-0.9.3/antspymm.egg-info/top_level.txt
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 10:41:05.519111 antspymm-0.9.3/docs/
+-rw-r--r--   0 stnava     (501) staff       (20)  1939802 2023-01-29 13:48:53.000000 antspymm-0.9.3/docs/antspymm_data_dictionary.csv
+-rw-r--r--   0 stnava     (501) staff       (20)      567 2023-04-12 13:06:30.000000 antspymm-0.9.3/docs/bids_cohort_example.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1296 2023-04-08 18:52:17.000000 antspymm-0.9.3/docs/example_run_from_directory.py
+-rw-r--r--   0 stnava     (501) staff       (20)      478 2023-02-19 10:57:50.000000 antspymm-0.9.3/docs/make_dict_table.Rmd
+-rw-r--r--   0 stnava     (501) staff       (20)      632 2023-04-12 13:06:30.000000 antspymm-0.9.3/docs/nrg_cohort_example.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2082 2023-03-20 13:00:28.000000 antspymm-0.9.3/docs/outlierness.py
+-rw-r--r--   0 stnava     (501) staff       (20)     3643 2023-04-15 22:47:31.000000 antspymm-0.9.3/docs/ukbb_to_nrg_processing.py
+-rw-r--r--   0 stnava     (501) staff       (20)     4546 2023-04-16 12:24:12.000000 antspymm-0.9.3/docs/ukbb_to_nrg_processing2.py
+-rw-r--r--   0 stnava     (501) staff       (20)       38 2023-05-09 10:41:05.524475 antspymm-0.9.3/setup.cfg
+-rw-r--r--   0 stnava     (501) staff       (20)      681 2023-05-09 10:39:26.000000 antspymm-0.9.3/setup.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-09 10:41:05.523770 antspymm-0.9.3/tests/
+-rw-r--r--   0 stnava     (501) staff       (20)     5589 2022-10-21 12:35:02.000000 antspymm-0.9.3/tests/mm.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2087 2022-12-17 20:51:01.000000 antspymm-0.9.3/tests/mm_nrg.py
+-rw-r--r--   0 stnava     (501) staff       (20)      440 2023-03-15 12:39:26.000000 antspymm-0.9.3/tests/test_bids_2_nrg.py
+-rw-r--r--   0 stnava     (501) staff       (20)      394 2022-06-09 14:57:05.000000 antspymm-0.9.3/tests/test_dti_recon.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1500 2023-05-01 14:47:40.000000 antspymm-0.9.3/tests/test_dti_reg.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2507 2023-02-05 20:18:30.000000 antspymm-0.9.3/tests/test_dwi_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)      445 2023-02-05 00:06:28.000000 antspymm-0.9.3/tests/test_flair_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)     3368 2023-05-02 12:19:49.000000 antspymm-0.9.3/tests/test_joint_dti_recon.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1497 2023-03-15 12:44:41.000000 antspymm-0.9.3/tests/test_mm_csv.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2101 2022-11-16 16:52:51.000000 antspymm-0.9.3/tests/test_rsfmri_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)      762 2023-05-05 18:29:30.000000 antspymm-0.9.3/tests/test_ukbb_rsfmri.py
+-rw-r--r--   0 stnava     (501) staff       (20)      597 2021-11-02 19:50:00.000000 antspymm-0.9.3/tests/testsr.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1439 2023-03-02 15:01:53.000000 antspymm-0.9.3/tests/visualize_tractogram.py
```

### Comparing `antspymm-0.9.2/LICENSE` & `antspymm-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/PKG-INFO` & `antspymm-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspymm
-Version: 0.9.2
+Version: 0.9.3
 Summary: multi-channel/time-series medical image processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyMM
 Author: Avants, Gosselin, Tustison, Reardon
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
```

### Comparing `antspymm-0.9.2/README.md` & `antspymm-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/antspymm/__init__.py` & `antspymm-0.9.3/antspymm/__init__.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/antspymm/mm.py` & `antspymm-0.9.3/antspymm/mm.py`

 * *Files 0% similar despite different names*

```diff
@@ -4349,16 +4349,16 @@
                 srmodel=srmodel,
                 motion_correct=dti_motion_correct, # set to False if using input from qsiprep
                 denoise=dti_denoise,
                 verbose = verbose)
         else :  # use phase encoding acquisitions for distortion correction and T1 for brain extraction
             if verbose:
                 print("We have both DTI_LR and DTI_RL: " + str(len(dw_image)))
-            a1b,a1w=antspymm.get_average_dwi_b0(dw_image[0])
-            a2b,a2w=antspymm.get_average_dwi_b0(dw_image[1],fixed_b0=a1b,fixed_dwi=a1w)
+            a1b,a1w=get_average_dwi_b0(dw_image[0])
+            a2b,a2w=get_average_dwi_b0(dw_image[1],fixed_b0=a1b,fixed_dwi=a1w)
             btpB0, btpDW = dti_template(
                 b_image_list=[a1b,a2b],
                 w_image_list=[a1w,a2w],
                 iterations=7, verbose=verbose )
             initrig = ants.registration( btpDW, hier['brain_n4_dnz'], 'BOLDRigid' )['fwdtransforms'][0]
             tempreg = ants.registration( btpDW, hier['brain_n4_dnz'], 'SyNOnly',
                 syn_metric='mattes', syn_sampling=32,
```

### Comparing `antspymm-0.9.2/antspymm.egg-info/PKG-INFO` & `antspymm-0.9.3/antspymm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspymm
-Version: 0.9.2
+Version: 0.9.3
 Summary: multi-channel/time-series medical image processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyMM
 Author: Avants, Gosselin, Tustison, Reardon
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
```

### Comparing `antspymm-0.9.2/antspymm.egg-info/SOURCES.txt` & `antspymm-0.9.3/antspymm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/docs/antspymm_data_dictionary.csv` & `antspymm-0.9.3/docs/antspymm_data_dictionary.csv`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/docs/bids_cohort_example.py` & `antspymm-0.9.3/docs/bids_cohort_example.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/docs/example_run_from_directory.py` & `antspymm-0.9.3/docs/example_run_from_directory.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/docs/nrg_cohort_example.py` & `antspymm-0.9.3/docs/nrg_cohort_example.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/docs/outlierness.py` & `antspymm-0.9.3/docs/outlierness.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/docs/ukbb_to_nrg_processing.py` & `antspymm-0.9.3/docs/ukbb_to_nrg_processing.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/docs/ukbb_to_nrg_processing2.py` & `antspymm-0.9.3/docs/ukbb_to_nrg_processing2.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/setup.py` & `antspymm-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = open("README.md").read()
 
 with open("./requirements.txt") as f:
       requirements = f.read().splitlines()
 
 setup(name='antspymm',
-      version='0.9.2',
+      version='0.9.3',
       description='multi-channel/time-series medical image processing with antspyx',
       long_description=long_description,
       long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
       url='https://github.com/stnava/ANTsPyMM',
       author='Avants, Gosselin, Tustison, Reardon',
       author_email='stnava@gmail.com',
       license='Apache 2.0',
```

### Comparing `antspymm-0.9.2/tests/mm.py` & `antspymm-0.9.3/tests/mm.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/tests/mm_nrg.py` & `antspymm-0.9.3/tests/mm_nrg.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/tests/test_dti_reg.py` & `antspymm-0.9.3/tests/test_dti_reg.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/tests/test_dwi_run.py` & `antspymm-0.9.3/tests/test_dwi_run.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/tests/test_joint_dti_recon.py` & `antspymm-0.9.3/tests/test_joint_dti_recon.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/tests/test_mm_csv.py` & `antspymm-0.9.3/tests/test_mm_csv.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/tests/test_rsfmri_run.py` & `antspymm-0.9.3/tests/test_rsfmri_run.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/tests/test_ukbb_rsfmri.py` & `antspymm-0.9.3/tests/test_ukbb_rsfmri.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/tests/testsr.py` & `antspymm-0.9.3/tests/testsr.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.2/tests/visualize_tractogram.py` & `antspymm-0.9.3/tests/visualize_tractogram.py`

 * *Files identical despite different names*

