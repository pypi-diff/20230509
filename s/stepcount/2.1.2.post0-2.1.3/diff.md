# Comparing `tmp/stepcount-2.1.2.post0.tar.gz` & `tmp/stepcount-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepcount-2.1.2.post0.tar", last modified: Wed Apr 19 19:04:12 2023, max compression
+gzip compressed data, was "stepcount-2.1.3.tar", last modified: Tue May  9 18:38:31 2023, max compression
```

## Comparing `stepcount-2.1.2.post0.tar` & `stepcount-2.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:12.279609 stepcount-2.1.2.post0/
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-19 19:04:12.279609 stepcount-2.1.2.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:04:12.279609 stepcount-2.1.2.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:12.275609 stepcount-2.1.2.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:12.283609 stepcount-2.1.2.post0/src/stepcount/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/src/stepcount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 19:04:12.283609 stepcount-2.1.2.post0/src/stepcount/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/src/stepcount/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/src/stepcount/hmm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21708 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/src/stepcount/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/src/stepcount/sslmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/src/stepcount/stepcount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:12.279609 stepcount-2.1.2.post0/src/stepcount/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/src/stepcount/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/src/stepcount/utils/collate_outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:12.279609 stepcount-2.1.2.post0/src/stepcount.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-19 19:04:12.000000 stepcount-2.1.2.post0/src/stepcount.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-19 19:04:12.000000 stepcount-2.1.2.post0/src/stepcount.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:04:12.000000 stepcount-2.1.2.post0/src/stepcount.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-19 19:04:12.000000 stepcount-2.1.2.post0/src/stepcount.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-19 19:04:12.000000 stepcount-2.1.2.post0/src/stepcount.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 19:04:12.000000 stepcount-2.1.2.post0/src/stepcount.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:38:31.900541 stepcount-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-05-09 18:38:21.000000 stepcount-2.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-09 18:38:31.900541 stepcount-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-09 18:38:21.000000 stepcount-2.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-09 18:38:21.000000 stepcount-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 18:38:31.900541 stepcount-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-09 18:38:21.000000 stepcount-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:38:31.892541 stepcount-2.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:38:31.900541 stepcount-2.1.3/src/stepcount/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-09 18:38:21.000000 stepcount-2.1.3/src/stepcount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 18:38:31.900541 stepcount-2.1.3/src/stepcount/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-09 18:38:21.000000 stepcount-2.1.3/src/stepcount/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-05-09 18:38:21.000000 stepcount-2.1.3/src/stepcount/hmm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21831 2023-05-09 18:38:21.000000 stepcount-2.1.3/src/stepcount/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-05-09 18:38:21.000000 stepcount-2.1.3/src/stepcount/sslmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-05-09 18:38:21.000000 stepcount-2.1.3/src/stepcount/stepcount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:38:31.900541 stepcount-2.1.3/src/stepcount/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-09 18:38:21.000000 stepcount-2.1.3/src/stepcount/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-09 18:38:21.000000 stepcount-2.1.3/src/stepcount/utils/collate_outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:38:31.900541 stepcount-2.1.3/src/stepcount.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-09 18:38:31.000000 stepcount-2.1.3/src/stepcount.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-09 18:38:31.000000 stepcount-2.1.3/src/stepcount.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:38:31.000000 stepcount-2.1.3/src/stepcount.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-09 18:38:31.000000 stepcount-2.1.3/src/stepcount.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-09 18:38:31.000000 stepcount-2.1.3/src/stepcount.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 18:38:31.000000 stepcount-2.1.3/src/stepcount.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-09 18:38:21.000000 stepcount-2.1.3/versioneer.py
```

### Comparing `stepcount-2.1.2.post0/LICENSE.md` & `stepcount-2.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.2.post0/PKG-INFO` & `stepcount-2.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,203 +1,203 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 2.1.2.post0
+Version: 2.1.3
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
+Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
-Download-URL: https://github.com/OxWearables/stepcount
-Description: # stepcount
-        
-        A Python package to estimate step counts from accelerometer data.
-        
-        The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649). 
-        
-        Check out the 5-minute video tutorial to get started: [https://www.youtube.com/watch?v=FPb7H-jyRVQ](https://www.youtube.com/watch?v=FPb7H-jyRVQ).
-        
-        ## Getting started
-        
-        ### Prerequisite
-        
-        - Python 3.8 or greater
-            ```console
-            $ python --version  # or python3 --version
-            ```
-        
-        - Java 8 (1.8.0) or greater
-            ```console
-            $ java -version
-            ```
-        
-        ### Install (Windows)
-        For Windows users, we recommend running stepcount using the **Anaconda Prompt** from **Miniconda** via the following steps:
-        
-        1. Download [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (light-weight version of Anaconda). Choose **Miniconda3 Windows 64-bit**.
-        2. Install. Use the default recommended settings.
-        3. From the Start menu, search and open the **Anaconda Prompt**.
-        
-        ```console
-        $ pip install stepcount
-        ```
-        
-        For further information running Anaconda on Windows using virtual environments, see [this guide](anaconda_on_windows.md).
-        
-        ### Install (Linux)
-        
-        <!-- ```console
-        $ pip install git+https://github.com/OxWearables/stepcount.git@master#egg=stepcount
-        ``` -->
-        
-        <!-- ```console
-        $ pip install git+ssh://git@github.com/OxWearables/stepcount.git@master#egg=stepcount
-        ``` -->
-        
-        ```console
-        $ pip install stepcount
-        ```
-        
-        
-        
-        ## Usage
-        
-        ```bash
-        # Process an AX3 file
-        $ stepcount sample.cwa
-        
-        # Or an ActiGraph file
-        $ stepcount sample.gt3x
-        
-        # Or a GENEActiv file
-        $ stepcount sample.bin
-        
-        # Or a CSV file (see data format below)
-        $ stepcount sample.csv
-        ```
-        
-        Output:
-        ```console
-        Summary
-        -------
-        {
-            "Filename": "sample.cwa",
-            "Filesize(MB)": 65.1,
-            "Device": "Axivity",
-            "DeviceID": 2278,
-            "ReadErrors": 0,
-            "SampleRate": 100.0,
-            "ReadOK": 1,
-            "StartTime": "2013-10-21 10:00:07",
-            "EndTime": "2013-10-28 10:00:01",
-            "TotalWalking(min)": 655.75,
-            "TotalSteps": 43132,
-            ...
-        }
-        
-        Estimated Daily Steps
-        ---------------------
-                      steps
-        time
-        2013-10-21     5368
-        2013-10-22     7634
-        2013-10-23    10009
-        ...
-        
-        Output: outputs/sample/
-        ```
-        
-        ### Output files
-        By default, output files will be stored in a folder named after the input file, `outputs/{filename}/`, created in the current working directory. You can change the output path with the `-o` flag:
-        
-        ```console
-        $ stepcount sample.cwa -o /path/to/some/folder/
-        ```
-        
-        The following output files are created:
-        
-        - *Info.json* Summary info, as shown above.
-        - *Steps.csv* Raw time-series of step counts
-        - *HourlySteps.csv* Hourly step counts
-        - *DailySteps.csv* Daily step counts
-        - *HourlyStepsAdjusted.csv* Like HourlySteps but accounting for missing data (see section below).
-        - *DailyStepsAdjusted.csv* Like DailySteps but accounting for missing data (see section below).
-        
-        
-        ### Crude vs. Adjusted Estimates
-        Adjusted estimates are provided that account for missing data.
-        Missing values in the time-series are imputed with the mean of the same timepoint of other available days.
-        For adjusted totals and daily statistics, 24h multiples are needed and will be imputed if necessary.
-        Estimates will be NaN where data is still missing after imputation.
-        
-        
-        ### Processing CSV files
-        If a CSV file is provided, it must have the following header: `time`, `x`, `y`, `z`. 
-        
-        Example:
-        ```console
-        time,x,y,z
-        2013-10-21 10:00:08.000,-0.078923,0.396706,0.917759
-        2013-10-21 10:00:08.010,-0.094370,0.381479,0.933580
-        2013-10-21 10:00:08.020,-0.094370,0.366252,0.901938
-        2013-10-21 10:00:08.030,-0.078923,0.411933,0.901938
-        ...
-        ```
-        
-        ### Processing multiple files
-        #### Windows
-        To process multiple files you can create a text file in Notepad which includes one line for each file you wish to process, as shown below for *file1.cwa*, *file2.cwa*, and *file2.cwa*.
-        
-        Example text file *commands.txt*: 
-        ```console
-        stepcount file1.cwa &
-        stepcount file2.cwa &
-        stepcount file3.cwa 
-        :END
-        ````
-        Once this file is created, run `cmd < commands.txt` from the terminal.
-        
-        #### Linux
-        Create a file *command.sh* with:
-        ```console
-        stepcount file1.cwa
-        stepcount file2.cwa
-        stepcount file3.cwa
-        ```
-        Then, run `bash command.sh` from the terminal.
-        
-        #### Collating outputs
-        
-        A utility script is provided to collate outputs from multiple runs:
-        
-        ```console
-        stepcount-collate-outputs outputs/
-        ```
-        This will collate all *-Info.json files found in outputs/ and generate a CSV file.
-        
-        ## Validation
-        
-        Validation for this algorithm is presented in a preprint on medRxiv at: [https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1](https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1). 
-        
-        
-        ## Citing our work
-        
-        When using this tool, please consider citing the works listed in [CITATION.md](CITATION.md).
-        
-        
-        ## Licence
-        See [LICENSE.md](LICENSE.md).
-        
-        
-        ## Acknowledgements
-        We would like to thank all our code contributors, manuscript co-authors, and research participants for their help in making this work possible.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
+License-File: LICENSE.md
+
+# stepcount
+
+A Python package to estimate step counts from accelerometer data.
+
+The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649). 
+
+Check out the 5-minute video tutorial to get started: [https://www.youtube.com/watch?v=FPb7H-jyRVQ](https://www.youtube.com/watch?v=FPb7H-jyRVQ).
+
+## Getting started
+
+### Prerequisite
+
+- Python 3.8 or greater
+    ```console
+    $ python --version  # or python3 --version
+    ```
+
+- Java 8 (1.8.0) or greater
+    ```console
+    $ java -version
+    ```
+
+### Install (Windows)
+For Windows users, we recommend running stepcount using the **Anaconda Prompt** from **Miniconda** via the following steps:
+
+1. Download [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (light-weight version of Anaconda). Choose **Miniconda3 Windows 64-bit**.
+2. Install. Use the default recommended settings.
+3. From the Start menu, search and open the **Anaconda Prompt**.
+
+```console
+$ pip install stepcount
+```
+
+For further information running Anaconda on Windows using virtual environments, see [this guide](anaconda_on_windows.md).
+
+### Install (Linux)
+
+<!-- ```console
+$ pip install git+https://github.com/OxWearables/stepcount.git@master#egg=stepcount
+``` -->
+
+<!-- ```console
+$ pip install git+ssh://git@github.com/OxWearables/stepcount.git@master#egg=stepcount
+``` -->
+
+```console
+$ pip install stepcount
+```
+
+
+
+## Usage
+
+```bash
+# Process an AX3 file
+$ stepcount sample.cwa
+
+# Or an ActiGraph file
+$ stepcount sample.gt3x
+
+# Or a GENEActiv file
+$ stepcount sample.bin
+
+# Or a CSV file (see data format below)
+$ stepcount sample.csv
+```
+
+Output:
+```console
+Summary
+-------
+{
+    "Filename": "sample.cwa",
+    "Filesize(MB)": 65.1,
+    "Device": "Axivity",
+    "DeviceID": 2278,
+    "ReadErrors": 0,
+    "SampleRate": 100.0,
+    "ReadOK": 1,
+    "StartTime": "2013-10-21 10:00:07",
+    "EndTime": "2013-10-28 10:00:01",
+    "TotalWalking(min)": 655.75,
+    "TotalSteps": 43132,
+    ...
+}
+
+Estimated Daily Steps
+---------------------
+              steps
+time
+2013-10-21     5368
+2013-10-22     7634
+2013-10-23    10009
+...
+
+Output: outputs/sample/
+```
+
+### Output files
+By default, output files will be stored in a folder named after the input file, `outputs/{filename}/`, created in the current working directory. You can change the output path with the `-o` flag:
+
+```console
+$ stepcount sample.cwa -o /path/to/some/folder/
+```
+
+The following output files are created:
+
+- *Info.json* Summary info, as shown above.
+- *Steps.csv* Raw time-series of step counts
+- *HourlySteps.csv* Hourly step counts
+- *DailySteps.csv* Daily step counts
+- *HourlyStepsAdjusted.csv* Like HourlySteps but accounting for missing data (see section below).
+- *DailyStepsAdjusted.csv* Like DailySteps but accounting for missing data (see section below).
+
+
+### Crude vs. Adjusted Estimates
+Adjusted estimates are provided that account for missing data.
+Missing values in the time-series are imputed with the mean of the same timepoint of other available days.
+For adjusted totals and daily statistics, 24h multiples are needed and will be imputed if necessary.
+Estimates will be NaN where data is still missing after imputation.
+
+
+### Processing CSV files
+If a CSV file is provided, it must have the following header: `time`, `x`, `y`, `z`. 
+
+Example:
+```console
+time,x,y,z
+2013-10-21 10:00:08.000,-0.078923,0.396706,0.917759
+2013-10-21 10:00:08.010,-0.094370,0.381479,0.933580
+2013-10-21 10:00:08.020,-0.094370,0.366252,0.901938
+2013-10-21 10:00:08.030,-0.078923,0.411933,0.901938
+...
+```
+
+### Processing multiple files
+#### Windows
+To process multiple files you can create a text file in Notepad which includes one line for each file you wish to process, as shown below for *file1.cwa*, *file2.cwa*, and *file2.cwa*.
+
+Example text file *commands.txt*: 
+```console
+stepcount file1.cwa &
+stepcount file2.cwa &
+stepcount file3.cwa 
+:END
+````
+Once this file is created, run `cmd < commands.txt` from the terminal.
+
+#### Linux
+Create a file *command.sh* with:
+```console
+stepcount file1.cwa
+stepcount file2.cwa
+stepcount file3.cwa
+```
+Then, run `bash command.sh` from the terminal.
+
+#### Collating outputs
+
+A utility script is provided to collate outputs from multiple runs:
+
+```console
+stepcount-collate-outputs outputs/
+```
+This will collate all *-Info.json files found in outputs/ and generate a CSV file.
+
+## Validation
+
+Validation for this algorithm is presented in a preprint on medRxiv at: [https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1](https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1). 
+
+
+## Citing our work
+
+When using this tool, please consider citing the works listed in [CITATION.md](CITATION.md).
+
+
+## Licence
+See [LICENSE.md](LICENSE.md).
+
+
+## Acknowledgements
+We would like to thank all our code contributors, manuscript co-authors, and research participants for their help in making this work possible.
```

### Comparing `stepcount-2.1.2.post0/README.md` & `stepcount-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.2.post0/pyproject.toml` & `stepcount-2.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.2.post0/setup.py` & `stepcount-2.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         raise RuntimeError(f"Unable to find {string}.")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="stepcount",
-    python_requires=">=3.8",
+    python_requires=">=3.8,<3.11",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description="Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OxWearables/stepcount",
     download_url="https://github.com/OxWearables/stepcount",
```

### Comparing `stepcount-2.1.2.post0/src/stepcount/__init__.py` & `stepcount-2.1.3/src/stepcount/__init__.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.2.post0/src/stepcount/features.py` & `stepcount-2.1.3/src/stepcount/features.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.2.post0/src/stepcount/hmm_utils.py` & `stepcount-2.1.3/src/stepcount/hmm_utils.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.2.post0/src/stepcount/models.py` & `stepcount-2.1.3/src/stepcount/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,23 +208,26 @@
 
     def predict_from_frame(self, data, **kwargs):
 
         def fn(chunk):
             """ Process the chunk. Apply padding if length is not enough. """
             n = len(chunk)
             x = chunk[['x', 'y', 'z']].to_numpy()
-            if n > self.window_len:
+            if n == self.window_len:
+                x = x
+            elif n > self.window_len:
                 x = x[:self.window_len]
-            if n < self.window_len:
+            elif n < self.window_len and n > self.window_len / 2:
                 m = self.window_len - n
                 x = np.pad(x, ((0, m), (0, 0)), mode='wrap')
+            else:
+                x = np.full((self.window_len, 3), fill_value=np.nan)
             return x
 
         X, T = make_windows(data, self.window_sec, fn=fn, return_index=True)
-        X = np.asarray(X)
         Y = self.predict(X, **kwargs)
         Y = pd.Series(Y, index=T)
         return Y
 
 
 class WalkDetectorRF:
     def __init__(
@@ -440,23 +443,24 @@
 def make_windows(data, window_sec, fn=None, return_index=False):
     """ Split data into windows """
 
     if fn is None:
         def fn(x):
             return x
 
-    X = [fn(x) for _, x in data.resample(f"{window_sec}s", origin="start")]
+    X, T = [], []
+    for t, x in data.resample(f"{window_sec}s", origin="start"):
+        x = fn(x)
+        X.append(x)
+        T.append(t)
+
+    X = np.asarray(X)
 
     if return_index:
-        T = (
-            data.index
-            .to_series()
-            .resample(f"{window_sec}s", origin="start")
-            .first()
-        )
+        T = pd.DatetimeIndex(T)
         return X, T
 
     return X
 
 
 def cvp(
     model, X, Y, groups,
```

### Comparing `stepcount-2.1.2.post0/src/stepcount/sslmodel.py` & `stepcount-2.1.3/src/stepcount/sslmodel.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.2.post0/src/stepcount/stepcount.py` & `stepcount-2.1.3/src/stepcount/stepcount.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     before = time.time()
 
     # Load file
     if args.model_type == 'ssl':
         resample_hz = 30
     else:
-        resample_hz = 'uniform'
+        resample_hz = None
     data, info = read(args.filepath, resample_hz)
 
     # Output paths
     basename = resolve_path(args.filepath)[1]
     outdir = os.path.join(args.outdir, basename)
     os.makedirs(outdir, exist_ok=True)
 
@@ -139,28 +139,28 @@
     # there's a bug with .resample().sum(skipna)
     # https://github.com/pandas-dev/pandas/issues/29382
 
     # steps
     total = np.round(Y.agg(_sum))  # total steps
     hourly = Y.resample('H').agg(_sum).round()  # steps, hourly
     daily = Y.resample('D').agg(_sum).round()  # steps, daily
-    daily_avg = daily.mean().round()
-    daily_med = daily.median().round()
-    daily_min = daily.min().round()
-    daily_max = daily.max().round()
+    daily_avg = np.round(daily.mean())
+    daily_med = np.round(daily.median())
+    daily_min = np.round(daily.min())
+    daily_max = np.round(daily.max())
 
     # walking
     dt = pd.Timedelta(infer_freq(Y.index)).seconds
     W = Y.mask(~Y.isna(), Y >= steptol)
     total_walk = np.round(W.agg(_sum) * dt / 60)
     daily_walk = (W.resample('D').agg(_sum) * dt / 60).round()
-    daily_walk_avg = daily_walk.mean().round()
-    daily_walk_med = daily_walk.median().round()
-    daily_walk_min = daily_walk.min().round()
-    daily_walk_max = daily_walk.max().round()
+    daily_walk_avg = np.round(daily_walk.mean())
+    daily_walk_med = np.round(daily_walk.median())
+    daily_walk_min = np.round(daily_walk.min())
+    daily_walk_max = np.round(daily_walk.max())
 
     def _max(x, n=1):
         return x.nlargest(n, keep='all').mean()
 
     # cadence https://jamanetwork.com/journals/jama/fullarticle/2763292
     cadence = Y.resample('min').sum()
     cadence_peak1 = cadence.resample('D').agg(_max, n=1).mean()
```

### Comparing `stepcount-2.1.2.post0/src/stepcount/utils/collate_outputs.py` & `stepcount-2.1.3/src/stepcount/utils/collate_outputs.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.2.post0/src/stepcount.egg-info/PKG-INFO` & `stepcount-2.1.3/src/stepcount.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,203 +1,203 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 2.1.2.post0
+Version: 2.1.3
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
+Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
-Download-URL: https://github.com/OxWearables/stepcount
-Description: # stepcount
-        
-        A Python package to estimate step counts from accelerometer data.
-        
-        The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649). 
-        
-        Check out the 5-minute video tutorial to get started: [https://www.youtube.com/watch?v=FPb7H-jyRVQ](https://www.youtube.com/watch?v=FPb7H-jyRVQ).
-        
-        ## Getting started
-        
-        ### Prerequisite
-        
-        - Python 3.8 or greater
-            ```console
-            $ python --version  # or python3 --version
-            ```
-        
-        - Java 8 (1.8.0) or greater
-            ```console
-            $ java -version
-            ```
-        
-        ### Install (Windows)
-        For Windows users, we recommend running stepcount using the **Anaconda Prompt** from **Miniconda** via the following steps:
-        
-        1. Download [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (light-weight version of Anaconda). Choose **Miniconda3 Windows 64-bit**.
-        2. Install. Use the default recommended settings.
-        3. From the Start menu, search and open the **Anaconda Prompt**.
-        
-        ```console
-        $ pip install stepcount
-        ```
-        
-        For further information running Anaconda on Windows using virtual environments, see [this guide](anaconda_on_windows.md).
-        
-        ### Install (Linux)
-        
-        <!-- ```console
-        $ pip install git+https://github.com/OxWearables/stepcount.git@master#egg=stepcount
-        ``` -->
-        
-        <!-- ```console
-        $ pip install git+ssh://git@github.com/OxWearables/stepcount.git@master#egg=stepcount
-        ``` -->
-        
-        ```console
-        $ pip install stepcount
-        ```
-        
-        
-        
-        ## Usage
-        
-        ```bash
-        # Process an AX3 file
-        $ stepcount sample.cwa
-        
-        # Or an ActiGraph file
-        $ stepcount sample.gt3x
-        
-        # Or a GENEActiv file
-        $ stepcount sample.bin
-        
-        # Or a CSV file (see data format below)
-        $ stepcount sample.csv
-        ```
-        
-        Output:
-        ```console
-        Summary
-        -------
-        {
-            "Filename": "sample.cwa",
-            "Filesize(MB)": 65.1,
-            "Device": "Axivity",
-            "DeviceID": 2278,
-            "ReadErrors": 0,
-            "SampleRate": 100.0,
-            "ReadOK": 1,
-            "StartTime": "2013-10-21 10:00:07",
-            "EndTime": "2013-10-28 10:00:01",
-            "TotalWalking(min)": 655.75,
-            "TotalSteps": 43132,
-            ...
-        }
-        
-        Estimated Daily Steps
-        ---------------------
-                      steps
-        time
-        2013-10-21     5368
-        2013-10-22     7634
-        2013-10-23    10009
-        ...
-        
-        Output: outputs/sample/
-        ```
-        
-        ### Output files
-        By default, output files will be stored in a folder named after the input file, `outputs/{filename}/`, created in the current working directory. You can change the output path with the `-o` flag:
-        
-        ```console
-        $ stepcount sample.cwa -o /path/to/some/folder/
-        ```
-        
-        The following output files are created:
-        
-        - *Info.json* Summary info, as shown above.
-        - *Steps.csv* Raw time-series of step counts
-        - *HourlySteps.csv* Hourly step counts
-        - *DailySteps.csv* Daily step counts
-        - *HourlyStepsAdjusted.csv* Like HourlySteps but accounting for missing data (see section below).
-        - *DailyStepsAdjusted.csv* Like DailySteps but accounting for missing data (see section below).
-        
-        
-        ### Crude vs. Adjusted Estimates
-        Adjusted estimates are provided that account for missing data.
-        Missing values in the time-series are imputed with the mean of the same timepoint of other available days.
-        For adjusted totals and daily statistics, 24h multiples are needed and will be imputed if necessary.
-        Estimates will be NaN where data is still missing after imputation.
-        
-        
-        ### Processing CSV files
-        If a CSV file is provided, it must have the following header: `time`, `x`, `y`, `z`. 
-        
-        Example:
-        ```console
-        time,x,y,z
-        2013-10-21 10:00:08.000,-0.078923,0.396706,0.917759
-        2013-10-21 10:00:08.010,-0.094370,0.381479,0.933580
-        2013-10-21 10:00:08.020,-0.094370,0.366252,0.901938
-        2013-10-21 10:00:08.030,-0.078923,0.411933,0.901938
-        ...
-        ```
-        
-        ### Processing multiple files
-        #### Windows
-        To process multiple files you can create a text file in Notepad which includes one line for each file you wish to process, as shown below for *file1.cwa*, *file2.cwa*, and *file2.cwa*.
-        
-        Example text file *commands.txt*: 
-        ```console
-        stepcount file1.cwa &
-        stepcount file2.cwa &
-        stepcount file3.cwa 
-        :END
-        ````
-        Once this file is created, run `cmd < commands.txt` from the terminal.
-        
-        #### Linux
-        Create a file *command.sh* with:
-        ```console
-        stepcount file1.cwa
-        stepcount file2.cwa
-        stepcount file3.cwa
-        ```
-        Then, run `bash command.sh` from the terminal.
-        
-        #### Collating outputs
-        
-        A utility script is provided to collate outputs from multiple runs:
-        
-        ```console
-        stepcount-collate-outputs outputs/
-        ```
-        This will collate all *-Info.json files found in outputs/ and generate a CSV file.
-        
-        ## Validation
-        
-        Validation for this algorithm is presented in a preprint on medRxiv at: [https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1](https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1). 
-        
-        
-        ## Citing our work
-        
-        When using this tool, please consider citing the works listed in [CITATION.md](CITATION.md).
-        
-        
-        ## Licence
-        See [LICENSE.md](LICENSE.md).
-        
-        
-        ## Acknowledgements
-        We would like to thank all our code contributors, manuscript co-authors, and research participants for their help in making this work possible.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
+License-File: LICENSE.md
+
+# stepcount
+
+A Python package to estimate step counts from accelerometer data.
+
+The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649). 
+
+Check out the 5-minute video tutorial to get started: [https://www.youtube.com/watch?v=FPb7H-jyRVQ](https://www.youtube.com/watch?v=FPb7H-jyRVQ).
+
+## Getting started
+
+### Prerequisite
+
+- Python 3.8 or greater
+    ```console
+    $ python --version  # or python3 --version
+    ```
+
+- Java 8 (1.8.0) or greater
+    ```console
+    $ java -version
+    ```
+
+### Install (Windows)
+For Windows users, we recommend running stepcount using the **Anaconda Prompt** from **Miniconda** via the following steps:
+
+1. Download [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (light-weight version of Anaconda). Choose **Miniconda3 Windows 64-bit**.
+2. Install. Use the default recommended settings.
+3. From the Start menu, search and open the **Anaconda Prompt**.
+
+```console
+$ pip install stepcount
+```
+
+For further information running Anaconda on Windows using virtual environments, see [this guide](anaconda_on_windows.md).
+
+### Install (Linux)
+
+<!-- ```console
+$ pip install git+https://github.com/OxWearables/stepcount.git@master#egg=stepcount
+``` -->
+
+<!-- ```console
+$ pip install git+ssh://git@github.com/OxWearables/stepcount.git@master#egg=stepcount
+``` -->
+
+```console
+$ pip install stepcount
+```
+
+
+
+## Usage
+
+```bash
+# Process an AX3 file
+$ stepcount sample.cwa
+
+# Or an ActiGraph file
+$ stepcount sample.gt3x
+
+# Or a GENEActiv file
+$ stepcount sample.bin
+
+# Or a CSV file (see data format below)
+$ stepcount sample.csv
+```
+
+Output:
+```console
+Summary
+-------
+{
+    "Filename": "sample.cwa",
+    "Filesize(MB)": 65.1,
+    "Device": "Axivity",
+    "DeviceID": 2278,
+    "ReadErrors": 0,
+    "SampleRate": 100.0,
+    "ReadOK": 1,
+    "StartTime": "2013-10-21 10:00:07",
+    "EndTime": "2013-10-28 10:00:01",
+    "TotalWalking(min)": 655.75,
+    "TotalSteps": 43132,
+    ...
+}
+
+Estimated Daily Steps
+---------------------
+              steps
+time
+2013-10-21     5368
+2013-10-22     7634
+2013-10-23    10009
+...
+
+Output: outputs/sample/
+```
+
+### Output files
+By default, output files will be stored in a folder named after the input file, `outputs/{filename}/`, created in the current working directory. You can change the output path with the `-o` flag:
+
+```console
+$ stepcount sample.cwa -o /path/to/some/folder/
+```
+
+The following output files are created:
+
+- *Info.json* Summary info, as shown above.
+- *Steps.csv* Raw time-series of step counts
+- *HourlySteps.csv* Hourly step counts
+- *DailySteps.csv* Daily step counts
+- *HourlyStepsAdjusted.csv* Like HourlySteps but accounting for missing data (see section below).
+- *DailyStepsAdjusted.csv* Like DailySteps but accounting for missing data (see section below).
+
+
+### Crude vs. Adjusted Estimates
+Adjusted estimates are provided that account for missing data.
+Missing values in the time-series are imputed with the mean of the same timepoint of other available days.
+For adjusted totals and daily statistics, 24h multiples are needed and will be imputed if necessary.
+Estimates will be NaN where data is still missing after imputation.
+
+
+### Processing CSV files
+If a CSV file is provided, it must have the following header: `time`, `x`, `y`, `z`. 
+
+Example:
+```console
+time,x,y,z
+2013-10-21 10:00:08.000,-0.078923,0.396706,0.917759
+2013-10-21 10:00:08.010,-0.094370,0.381479,0.933580
+2013-10-21 10:00:08.020,-0.094370,0.366252,0.901938
+2013-10-21 10:00:08.030,-0.078923,0.411933,0.901938
+...
+```
+
+### Processing multiple files
+#### Windows
+To process multiple files you can create a text file in Notepad which includes one line for each file you wish to process, as shown below for *file1.cwa*, *file2.cwa*, and *file2.cwa*.
+
+Example text file *commands.txt*: 
+```console
+stepcount file1.cwa &
+stepcount file2.cwa &
+stepcount file3.cwa 
+:END
+````
+Once this file is created, run `cmd < commands.txt` from the terminal.
+
+#### Linux
+Create a file *command.sh* with:
+```console
+stepcount file1.cwa
+stepcount file2.cwa
+stepcount file3.cwa
+```
+Then, run `bash command.sh` from the terminal.
+
+#### Collating outputs
+
+A utility script is provided to collate outputs from multiple runs:
+
+```console
+stepcount-collate-outputs outputs/
+```
+This will collate all *-Info.json files found in outputs/ and generate a CSV file.
+
+## Validation
+
+Validation for this algorithm is presented in a preprint on medRxiv at: [https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1](https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1). 
+
+
+## Citing our work
+
+When using this tool, please consider citing the works listed in [CITATION.md](CITATION.md).
+
+
+## Licence
+See [LICENSE.md](LICENSE.md).
+
+
+## Acknowledgements
+We would like to thank all our code contributors, manuscript co-authors, and research participants for their help in making this work possible.
```

### Comparing `stepcount-2.1.2.post0/src/stepcount.egg-info/SOURCES.txt` & `stepcount-2.1.3/src/stepcount.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.2.post0/versioneer.py` & `stepcount-2.1.3/versioneer.py`

 * *Files identical despite different names*

