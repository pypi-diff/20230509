# Comparing `tmp/pdcscore-1.1.3.tar.gz` & `tmp/pdcscore-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdcscore-1.1.3.tar", last modified: Sun May  7 01:42:35 2023, max compression
+gzip compressed data, was "pdcscore-1.1.4.tar", last modified: Tue May  9 02:46:58 2023, max compression
```

## Comparing `pdcscore-1.1.3.tar` & `pdcscore-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 01:42:35.635275 pdcscore-1.1.3/
--rw-rw-rw-   0        0        0     1099 2023-05-04 02:23:33.000000 pdcscore-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     5604 2023-05-07 01:42:35.635275 pdcscore-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4321 2023-05-07 01:22:27.000000 pdcscore-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 01:42:35.617275 pdcscore-1.1.3/pdcscore/
--rw-rw-rw-   0        0        0       79 2023-05-07 01:41:34.000000 pdcscore-1.1.3/pdcscore/__init__.py
--rw-rw-rw-   0        0        0     3523 2023-05-07 01:22:49.000000 pdcscore-1.1.3/pdcscore/pdcscore.py
-drwxrwxrwx   0        0        0        0 2023-05-07 01:42:35.633275 pdcscore-1.1.3/pdcscore.egg-info/
--rw-rw-rw-   0        0        0     5604 2023-05-07 01:42:35.000000 pdcscore-1.1.3/pdcscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-07 01:42:35.000000 pdcscore-1.1.3/pdcscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 01:42:35.000000 pdcscore-1.1.3/pdcscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-07 01:42:35.000000 pdcscore-1.1.3/pdcscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-07 01:42:35.000000 pdcscore-1.1.3/pdcscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 01:42:35.635275 pdcscore-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1602 2023-05-07 01:41:49.000000 pdcscore-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:46:58.076979 pdcscore-1.1.4/
+-rw-rw-rw-   0        0        0     1099 2023-05-09 02:44:59.000000 pdcscore-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     5621 2023-05-09 02:46:58.076979 pdcscore-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4419 2023-05-09 02:44:59.000000 pdcscore-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 02:46:58.054356 pdcscore-1.1.4/pdcscore/
+-rw-rw-rw-   0        0        0       81 2023-05-09 02:44:59.000000 pdcscore-1.1.4/pdcscore/__init__.py
+-rw-rw-rw-   0        0        0     4336 2023-05-09 02:44:59.000000 pdcscore-1.1.4/pdcscore/pdcscore.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:46:58.075980 pdcscore-1.1.4/pdcscore.egg-info/
+-rw-rw-rw-   0        0        0     5621 2023-05-09 02:46:57.000000 pdcscore-1.1.4/pdcscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-09 02:46:57.000000 pdcscore-1.1.4/pdcscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 02:46:57.000000 pdcscore-1.1.4/pdcscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-09 02:46:57.000000 pdcscore-1.1.4/pdcscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-09 02:46:57.000000 pdcscore-1.1.4/pdcscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 02:46:58.077978 pdcscore-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1646 2023-05-09 02:44:59.000000 pdcscore-1.1.4/setup.py
```

### Comparing `pdcscore-1.1.3/LICENSE` & `pdcscore-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pdcscore-1.1.3/PKG-INFO` & `pdcscore-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdcscore
-Version: 1.1.3
+Version: 1.1.4
 Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: https://github.com/famutimine/pdcscore
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
@@ -20,17 +20,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+## README.md
+
 The objective of this package is to offer a Python-based solution for computing the Proportion of Days Covered (PDC), a widely used metric in the healthcare industry to evaluate medication adherence. As the healthcare analytics sector shifts away from SAS, there is a growing need to recreate key metrics in alternative platforms. This package aims to simplify the process and reduce the workload for business analysts in the healthcare ecosystem by providing a readily available PDC calculation tool, thereby eliminating the need to build it from scratch.
 
-I followed the original implementation logic of PDC in SAS, this can be found at https://support.sas.com/resources/papers/proceedings13/167-2013.pdf 
+I followed the original implementation logic of PDC in SAS, this can be found at https://support.sas.com/resources/papers/proceedings13/167-2013.pdf
 
 This paper offers a gentle, yet detailed introduction to the topic, and will serve as a reference to anyone new to the subject.
 
 
 Current update accounts for 6 months washout period and is optimized for multiprocessing large datasets.
 
 Please use as described below:
@@ -103,7 +105,8 @@
 calcfunc = pdcCalc(dataframe=df,patient_id_col='patient_id', drugname_col='drugname', filldate_col='filldate'
                    , supply_days_col='supply_days', msr_start_dt_col='msr_start_dt', msr_end_dt_col='msr_end_dt')
 pdc_scores_df = calcfunc.calculate_pdc()
 
 # Inspect output
 pdc_scores_df.head()
 
+
```

### Comparing `pdcscore-1.1.3/README.md` & `pdcscore-1.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,84 @@
-The objective of this package is to offer a Python-based solution for computing the Proportion of Days Covered (PDC), a widely used metric in the healthcare industry to evaluate medication adherence. As the healthcare analytics sector shifts away from SAS, there is a growing need to recreate key metrics in alternative platforms. This package aims to simplify the process and reduce the workload for business analysts in the healthcare ecosystem by providing a readily available PDC calculation tool, thereby eliminating the need to build it from scratch.
-
-I followed the original implementation logic of PDC in SAS, this can be found at https://support.sas.com/resources/papers/proceedings13/167-2013.pdf 
-
-This paper offers a gentle, yet detailed introduction to the topic, and will serve as a reference to anyone new to the subject.
-
-
-Current update accounts for 6 months washout period and is optimized for multiprocessing large datasets.
-
-Please use as described below:
-
-**INPUT PARAMETERS:**
-
-**dataframe** - *A pandas dataframe containing the required columns described below.*
-
-**patient_id_col** - *A unique patient identifier. Format = STRING or INTEGER*
-
-**drugname_col** - *The name of the drug being filled or drug class or Generic name, per usual PDC requirements. Format = STRING*
-
-**filldate_col** - *The date of the fill being dispensed. Format = DATE*
-
-**supply_days_col** - *Days of supply being dispensed at fill. Format = INTEGER*
-
-**msr_start_dt_col** - *start date of measurement period for the patient or a reference START DATE. Format = DATE*
-
-**msr_end_dt_col** - *end date of measurement period for the patient or a reference END DATE. Format = DATE*
-
-
-
-**OUTPUT DATAFRAME** - *A Pandas dataframe containing the following columns*
-
-**patient_id_col** - *This will return a column name representing a unique patient identifier as provided in original input dataframe. FORMAT = STRING*
-
-**drugname_col** - *The name of the drug being filled or drug class or Generic name, as provided in original input dataframe.*
-
-**dayscovered**- *The number of unique days of drug coverage, after shifting coverage to accommodate early refills. FORMAT = INTEGER*
-
-**totaldays** - *The total number of days in patient analysis window. Set to 0 if days of coverage is 0. FORMAT = INTEGER*
-
-**pdc_score** - *The patient's PDC score, calculated as dayscovered / totaldays. Set to 0 if days of coverage is 0. FORMAT = FLOAT*
-
-
-
-## USAGE EXAMPLE
-```python
-
-#  Import required libraries
-import pandas as pd
-import numpy as np
-from datetime import datetime
-from pdcscore import pdcCalc
-
-# Create a sample dataframe
-df = pd.DataFrame({
-    'patient_id': ['A001', 'A001', 'A001', 'B001', 'B001', 'B001', 'C001', 'C001', 'C001','C001', 'C001', 'C001'],
-    'drugname': ['DRUG_X', 'DRUG_X', 'DRUG_X', 'DRUG_Y', 'DRUG_Y', 'DRUG_Y', 'DRUG_Y', 'DRUG_Y', 'DRUG_Y',
-                    'DRUG_Z', 'DRUG_Z', 'DRUG_Z'],
-    'filldate': pd.to_datetime(['2021-10-21', '2022-01-21', '2022-03-20',
-                                '2022-01-01', '2022-02-01', '2022-03-01',
-                                   '2022-02-18', '2022-03-01', '2022-03-22',
-                                   '2021-06-18', '2022-02-11', '2022-03-05']),
-    'supply_days': [90, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30],
-    'msr_start_dt': pd.to_datetime(['2022-01-01', '2022-01-01', '2022-01-01',
-                                         '2022-01-01', '2022-01-01', '2022-01-01',
-                                       '2022-01-01', '2022-01-01', '2022-01-01',
-                                       '2022-01-01', '2022-01-01', '2022-01-01']),
-    'msr_end_dt': pd.to_datetime(['2022-03-31', '2022-03-31', '2022-03-31',
-                                       '2022-03-31', '2022-03-31', '2022-03-31',
-                                     '2022-03-31', '2022-03-31', '2022-03-31',
-                                     '2022-03-31', '2022-03-31', '2022-03-31'])
-})
-
-# Inspect sample data
-df.head(n=len(df))
-
-# calculate PDC scores on the input DataFrame
-calcfunc = pdcCalc(dataframe=df,patient_id_col='patient_id', drugname_col='drugname', filldate_col='filldate'
-                   , supply_days_col='supply_days', msr_start_dt_col='msr_start_dt', msr_end_dt_col='msr_end_dt')
-pdc_scores_df = calcfunc.calculate_pdc()
-
-# Inspect output
-pdc_scores_df.head()
+## README.md
+
+The objective of this package is to offer a Python-based solution for computing the Proportion of Days Covered (PDC), a widely used metric in the healthcare industry to evaluate medication adherence. As the healthcare analytics sector shifts away from SAS, there is a growing need to recreate key metrics in alternative platforms. This package aims to simplify the process and reduce the workload for business analysts in the healthcare ecosystem by providing a readily available PDC calculation tool, thereby eliminating the need to build it from scratch.
+
+I followed the original implementation logic of PDC in SAS, this can be found at https://support.sas.com/resources/papers/proceedings13/167-2013.pdf
+
+This paper offers a gentle, yet detailed introduction to the topic, and will serve as a reference to anyone new to the subject.
+
+
+Current update accounts for 6 months washout period and is optimized for multiprocessing large datasets.
+
+Please use as described below:
+
+**INPUT PARAMETERS:**
+
+**dataframe** - *A pandas dataframe containing the required columns described below.*
+
+**patient_id_col** - *A unique patient identifier. Format = STRING or INTEGER*
+
+**drugname_col** - *The name of the drug being filled or drug class or Generic name, per usual PDC requirements. Format = STRING*
+
+**filldate_col** - *The date of the fill being dispensed. Format = DATE*
+
+**supply_days_col** - *Days of supply being dispensed at fill. Format = INTEGER*
+
+**msr_start_dt_col** - *start date of measurement period for the patient or a reference START DATE. Format = DATE*
+
+**msr_end_dt_col** - *end date of measurement period for the patient or a reference END DATE. Format = DATE*
+
+
+
+**OUTPUT DATAFRAME** - *A Pandas dataframe containing the following columns*
+
+**patient_id_col** - *This will return a column name representing a unique patient identifier as provided in original input dataframe. FORMAT = STRING*
+
+**drugname_col** - *The name of the drug being filled or drug class or Generic name, as provided in original input dataframe.*
+
+**dayscovered**- *The number of unique days of drug coverage, after shifting coverage to accommodate early refills. FORMAT = INTEGER*
+
+**totaldays** - *The total number of days in patient analysis window. Set to 0 if days of coverage is 0. FORMAT = INTEGER*
+
+**pdc_score** - *The patient's PDC score, calculated as dayscovered / totaldays. Set to 0 if days of coverage is 0. FORMAT = FLOAT*
+
+
+
+## USAGE EXAMPLE
+```python
+
+#  Import required libraries
+import pandas as pd
+import numpy as np
+from datetime import datetime
+from pdcscore import pdcCalc
+
+# Create a sample dataframe
+df = pd.DataFrame({
+    'patient_id': ['A001', 'A001', 'A001', 'B001', 'B001', 'B001', 'C001', 'C001', 'C001','C001', 'C001', 'C001'],
+    'drugname': ['DRUG_X', 'DRUG_X', 'DRUG_X', 'DRUG_Y', 'DRUG_Y', 'DRUG_Y', 'DRUG_Y', 'DRUG_Y', 'DRUG_Y',
+                    'DRUG_Z', 'DRUG_Z', 'DRUG_Z'],
+    'filldate': pd.to_datetime(['2021-10-21', '2022-01-21', '2022-03-20',
+                                '2022-01-01', '2022-02-01', '2022-03-01',
+                                   '2022-02-18', '2022-03-01', '2022-03-22',
+                                   '2021-06-18', '2022-02-11', '2022-03-05']),
+    'supply_days': [90, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30, 30],
+    'msr_start_dt': pd.to_datetime(['2022-01-01', '2022-01-01', '2022-01-01',
+                                         '2022-01-01', '2022-01-01', '2022-01-01',
+                                       '2022-01-01', '2022-01-01', '2022-01-01',
+                                       '2022-01-01', '2022-01-01', '2022-01-01']),
+    'msr_end_dt': pd.to_datetime(['2022-03-31', '2022-03-31', '2022-03-31',
+                                       '2022-03-31', '2022-03-31', '2022-03-31',
+                                     '2022-03-31', '2022-03-31', '2022-03-31',
+                                     '2022-03-31', '2022-03-31', '2022-03-31'])
+})
+
+# Inspect sample data
+df.head(n=len(df))
+
+# calculate PDC scores on the input DataFrame
+calcfunc = pdcCalc(dataframe=df,patient_id_col='patient_id', drugname_col='drugname', filldate_col='filldate'
+                   , supply_days_col='supply_days', msr_start_dt_col='msr_start_dt', msr_end_dt_col='msr_end_dt')
+pdc_scores_df = calcfunc.calculate_pdc()
+
+# Inspect output
+pdc_scores_df.head()
```

### Comparing `pdcscore-1.1.3/pdcscore.egg-info/PKG-INFO` & `pdcscore-1.1.4/pdcscore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdcscore
-Version: 1.1.3
+Version: 1.1.4
 Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: https://github.com/famutimine/pdcscore
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
@@ -20,17 +20,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+## README.md
+
 The objective of this package is to offer a Python-based solution for computing the Proportion of Days Covered (PDC), a widely used metric in the healthcare industry to evaluate medication adherence. As the healthcare analytics sector shifts away from SAS, there is a growing need to recreate key metrics in alternative platforms. This package aims to simplify the process and reduce the workload for business analysts in the healthcare ecosystem by providing a readily available PDC calculation tool, thereby eliminating the need to build it from scratch.
 
-I followed the original implementation logic of PDC in SAS, this can be found at https://support.sas.com/resources/papers/proceedings13/167-2013.pdf 
+I followed the original implementation logic of PDC in SAS, this can be found at https://support.sas.com/resources/papers/proceedings13/167-2013.pdf
 
 This paper offers a gentle, yet detailed introduction to the topic, and will serve as a reference to anyone new to the subject.
 
 
 Current update accounts for 6 months washout period and is optimized for multiprocessing large datasets.
 
 Please use as described below:
@@ -103,7 +105,8 @@
 calcfunc = pdcCalc(dataframe=df,patient_id_col='patient_id', drugname_col='drugname', filldate_col='filldate'
                    , supply_days_col='supply_days', msr_start_dt_col='msr_start_dt', msr_end_dt_col='msr_end_dt')
 pdc_scores_df = calcfunc.calculate_pdc()
 
 # Inspect output
 pdc_scores_df.head()
 
+
```

### Comparing `pdcscore-1.1.3/setup.py` & `pdcscore-1.1.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from setuptools import setup, find_packages
-import os
-
-dir_path = r'C:\Users\famut\pdc_base_folder'
-file_name = 'README.md'
-
-file_path = os.path.join(dir_path, file_name)
-
-with open(file_path, encoding='utf-8') as f:
-    long_description = f.read()
-
-setup(
-    name='pdcscore',
-    version='1.1.3',
-    description='A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/famutimine/pdcscore',
-    author='Daniel Famutimi MD, MPH',
-    author_email='danielfamutimi@gmail.com',
-    license='MIT',
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Intended Audience :: Healthcare Industry',
-        'Intended Audience :: System Administrators',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: Scientific/Engineering :: Medical Science Apps.',
-        'Topic :: Scientific/Engineering :: Information Analysis',
-    ],
-    keywords='pdc calculator medication adherence',
-    packages=find_packages(),
-    include_package_data=True,
-    install_requires=[
-        'numpy',
-        'pandas',
-    ],
-)
+from setuptools import setup, find_packages
+import os
+
+dir_path = r'C:\Users\famut\pdc_base_folder'
+file_name = 'README.md'
+
+file_path = os.path.join(dir_path, file_name)
+
+with open(file_path, encoding='utf-8') as f:
+    long_description = f.read()
+
+setup(
+    name='pdcscore',
+    version='1.1.4',
+    description='A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/famutimine/pdcscore',
+    author='Daniel Famutimi MD, MPH',
+    author_email='danielfamutimi@gmail.com',
+    license='MIT',
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'Intended Audience :: Healthcare Industry',
+        'Intended Audience :: System Administrators',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: Scientific/Engineering :: Medical Science Apps.',
+        'Topic :: Scientific/Engineering :: Information Analysis',
+    ],
+    keywords='pdc calculator medication adherence',
+    packages=find_packages(),
+    include_package_data=True,
+    install_requires=[
+        'numpy',
+        'pandas',
+    ],
+)
```

