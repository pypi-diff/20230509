# Comparing `tmp/sportydatagen-0.2.0.tar.gz` & `tmp/sportydatagen-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sportydatagen-0.2.0.tar", max compression
+gzip compressed data, was "sportydatagen-0.2.1.tar", max compression
```

## Comparing `sportydatagen-0.2.0.tar` & `sportydatagen-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1073 2023-04-27 15:01:59.848205 sportydatagen-0.2.0/LICENSE
--rw-r--r--   0        0        0     1576 2023-04-27 15:01:59.848205 sportydatagen-0.2.0/README.md
--rw-r--r--   0        0        0     1800 2023-04-27 15:02:00.019205 sportydatagen-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      271 2023-04-27 15:02:00.019205 sportydatagen-0.2.0/sportydatagen/__init__.py
--rw-r--r--   0        0        0     5358 2023-04-27 15:02:00.019205 sportydatagen-0.2.0/sportydatagen/activity.py
--rw-r--r--   0        0        0     2878 2023-04-27 15:02:00.019205 sportydatagen-0.2.0/sportydatagen/banister_trimp_v2.py
--rw-r--r--   0        0        0     7186 2023-04-27 15:02:00.019205 sportydatagen-0.2.0/sportydatagen/convert_to_csv.py
--rw-r--r--   0        0        0     5020 2023-04-27 15:02:00.019205 sportydatagen-0.2.0/sportydatagen/csv_utils.py
--rw-r--r--   0        0        0     8784 2023-04-27 15:02:00.020205 sportydatagen-0.2.0/sportydatagen/feature_extraction_utils.py
--rw-r--r--   0        0        0      142 2023-04-27 15:02:00.020205 sportydatagen-0.2.0/sportydatagen/filetype.py
--rw-r--r--   0        0        0     7148 2023-04-27 15:02:00.020205 sportydatagen-0.2.0/sportydatagen/return_random_data.py
--rw-r--r--   0        0        0     2895 2023-04-27 15:02:00.020205 sportydatagen-0.2.0/sportydatagen/saf_extract_features_to_csv.py
--rw-r--r--   0        0        0      459 2023-04-27 15:02:00.020205 sportydatagen-0.2.0/sportydatagen/sportfile_utils.py
--rw-r--r--   0        0        0     2514 2023-04-27 15:02:00.020205 sportydatagen-0.2.0/sportydatagen/utils.py
--rw-r--r--   0        0        0     2358 2023-04-27 15:02:06.761357 sportydatagen-0.2.0/setup.py
--rw-r--r--   0        0        0     2298 2023-04-27 15:02:06.761613 sportydatagen-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-09 12:00:11.363491 sportydatagen-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1576 2023-05-09 12:00:11.363491 sportydatagen-0.2.1/README.md
+-rw-r--r--   0        0        0     1800 2023-05-09 12:00:11.537493 sportydatagen-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      372 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/__init__.py
+-rw-r--r--   0        0        0     5358 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/activity.py
+-rw-r--r--   0        0        0     7186 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/convert_to_csv.py
+-rw-r--r--   0        0        0     5419 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/csv_utils.py
+-rw-r--r--   0        0        0     9004 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/feature_extraction_utils.py
+-rw-r--r--   0        0        0      142 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/filetype.py
+-rw-r--r--   0        0        0     8126 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/return_random_data.py
+-rw-r--r--   0        0        0     2895 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/saf_extract_features_to_csv.py
+-rw-r--r--   0        0        0      477 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/sportfile_utils.py
+-rw-r--r--   0        0        0     2514 2023-05-09 12:00:11.538493 sportydatagen-0.2.1/sportydatagen/utils.py
+-rw-r--r--   0        0        0     2358 2023-05-09 12:00:23.577822 sportydatagen-0.2.1/setup.py
+-rw-r--r--   0        0        0     2298 2023-05-09 12:00:23.578082 sportydatagen-0.2.1/PKG-INFO
```

### Comparing `sportydatagen-0.2.0/LICENSE` & `sportydatagen-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sportydatagen-0.2.0/README.md` & `sportydatagen-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sportydatagen-0.2.0/pyproject.toml` & `sportydatagen-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "sportydatagen"
-version = "0.2.0"
+version = "0.2.1"
 description = "Sports activity generator module"
 license="MIT"
 readme = "README.md"
 keywords = ['artificial sport trainer', 'computational intelligence', 'data mining', 'sport activities', 'tcx']
 authors = ["Rok Kukovec <rok.kukovec1@student.um.si>", "Iztok Fister Jr. <iztok@iztok-jr-fister.eu>"]
 homepage = "https://gitlab.com/firefly-cpp/sportydatagen"
 repository = "https://gitlab.com/firefly-cpp/sportydatagen"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 niapy = "^2.0.5"
-sport-activities-features = "^0.3.11"
+sport-activities-features = "^0.3.12"
 numpy = "^1.24.2"
 pandas = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 black = "^23.1.0"
 isort = "^5.12.0"
-ruff = "^0.0.261"
+ruff = "^0.0.265"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 line_length = 79
```

### Comparing `sportydatagen-0.2.0/sportydatagen/activity.py` & `sportydatagen-0.2.1/sportydatagen/activity.py`

 * *Files identical despite different names*

### Comparing `sportydatagen-0.2.0/sportydatagen/convert_to_csv.py` & `sportydatagen-0.2.1/sportydatagen/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `sportydatagen-0.2.0/sportydatagen/csv_utils.py` & `sportydatagen-0.2.1/sportydatagen/csv_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,23 @@
 from sportydatagen.filetype import Filetype
 
 # Class for reading TCX files
 tcx_file = TCXFile()
 
 
 def create_list_of_all_possible_files(number_of_files: int) -> list:
-    """Create a list of all possible files."""
+    """Create a list of all possible files.
+
+    Args:
+    ----------------
+        number_of_files (int): Number of files.
+
+    Returns:
+    ----------------
+        all_possible_csv_files (list): List of all possible files."""
     all_possible_csv_files = []
     for i in range(1, number_of_files + 1):
         all_possible_csv_files.append(f'{i}.csv')
     return all_possible_csv_files
 
 
 def missing_csv_files(directory_path: str, number_of_files: int) -> list:
@@ -25,20 +33,20 @@
 
     Prints missing files from all possible numbered
     sequence of tcx/gpx files converted to csv files. Csv files are stored in
     tcx_csv directory. The script will print a list of missing files.
     Files are missing if they have not been correctly converted to csv format.
 
     Args:
-    ----
+    ----------------
     directory_path (str): Path to directory with csv files.
     number_of_files (int): Number of files.
 
     Returns:
-    -------
+    ----------------
     str: List of missing files.
     """
     csv_files_in_directory = os.listdir(Path(directory_path))
 
     all_possible_files = create_list_of_all_possible_files(number_of_files)
 
     set_of_actual_csv_files = set(csv_files_in_directory)
@@ -73,15 +81,25 @@
 
 
 # Function to check if heartrate exists
 def check_file_delete_csv_if_columns_are_nan(
         csv_directory: str,
         columns_to_check: list = None,
 ) -> None:
-    """Check if columns are nan in df and delete corresponding csv file."""
+    """Check if columns are nan in df and delete corresponding csv file.
+
+    Args:
+    ----------------
+        csv_directory (str): Path to csv directory.
+        columns_to_check (list): List of columns to check.
+
+    Returns:
+    ----------------
+        None
+    """
     if columns_to_check is None:
         columns_to_check = [
             'heartrates',
             'latitude',
             'longitude',
             'altitudes',
             'distances',
```

### Comparing `sportydatagen-0.2.0/sportydatagen/feature_extraction_utils.py` & `sportydatagen-0.2.1/sportydatagen/feature_extraction_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,35 @@
 
 import datetime as dt
 import os
 from pathlib import Path
 
 import pandas as pd
 from sport_activities_features import (
-    BanisterTRIMP,
+    BanisterTRIMPv1,
+    BanisterTRIMPv2,
     EdwardsTRIMP,
     GPXFile,
     LuciaTRIMP,
     TCXFile,
 )
 
-from sportydatagen.banister_trimp_v2 import BanisterTrimpV2
 from sportydatagen.filetype import Filetype
 
 
 def calculate_duration(read_df_tcx_csv: pd.DataFrame) -> int:
-    """Calculate duration of activity in seconds."""
+    """Calculate duration of activity in seconds.
+
+    Args:
+    ----------------
+        read_df_tcx_csv (pd.DataFrame): Dataframe with timestamps.
+    Returns:
+    ----------------
+        total_seconds (int): Duration of activity in seconds.
+    """
     try:
         start_time = dt.datetime.strptime(
             read_df_tcx_csv['timestamps'][0],
             '%Y-%m-%d %H:%M:%S',
         ).astimezone()
         end_time = dt.datetime.strptime(
             read_df_tcx_csv['timestamps'][len(read_df_tcx_csv) - 1],
@@ -101,20 +109,22 @@
     altitude_min = read_df_csv['altitudes'].min()
     duration = calculate_duration(read_df_csv)
     ascent, descent = calculate_ascent_descent(read_df_csv)
     # speed_min has been removed since it is always 0
     speed_max = read_df_csv['speeds'].max()
     speed_avg = read_df_csv['speeds'].mean()
 
-    # TRIMP
-    banister = BanisterTRIMP(duration, hr_avg)
-    banister_trimp = banister.calculate_TRIMP()
+    # Banister's simple TRIMP
+    banister = BanisterTRIMPv1(duration, hr_avg)
+    banister_trimp_v1 = banister.calculate_TRIMP()
+
+    # Banister's TRIMP V2
+    banister_v2 = BanisterTRIMPv2(duration, hr_avg, hr_min, hr_max)
 
-    banister_v2 = BanisterTrimpV2(duration, hr_avg, hr_min, hr_max)
-    banister_v2_trimp = banister_v2.calculate_trimp()
+    banister_trimp_v2 = banister_v2.calculate_TRIMP()
 
     # If sport_file is not None and path to original file is known,
     # extract calories, else set calories to 'NULL'
     if sport_file is not None and sportfile_directory is not None:
         if original_filename is None:
             original_filename = 'NULL'
             relative_path_of_original_file = None
@@ -155,16 +165,16 @@
         'altitude_avg': round(altitude_avg, 2),
         'altitude_min': altitude_min,
         'altitude_max': altitude_max,
         'ascent': ascent,
         'descent': descent,
         'speed_max': speed_max,
         'speed_avg': speed_avg,
-        'banister_TRIMP': banister_trimp,
-        'banister_V2_TRIMP': banister_v2_trimp,
+        'banister_simple_TRIMP': banister_trimp_v1,
+        'banister_TRIMP': banister_trimp_v2,
         'edwards_TRIMP': edwards_trimp,
         'lucia_TRIMP': lucia_trimp,
         'file_name': original_filename,
     }
```

### Comparing `sportydatagen-0.2.0/sportydatagen/return_random_data.py` & `sportydatagen-0.2.1/sportydatagen/return_random_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """Return random data from extracted features."""
-
-
 import pandas as pd
 
 
 def return_number_random_data(
         filepath: str,
         random_size: int,
         random_state: int = 1,
 ) -> pd.DataFrame:
     """Return a number of random data from extracted features.
 
     Args:
-    ----
+    ----------------
     filepath (str): Path where the extracted features are stored.
     random_size (int): Number of random data to return.
     random_state (int): Random state for reproducibility.
 
     Returns:
-    -------
+    ----------------
     pd.DataFrame: Random data from extracted features.
     """
     # Pandas read csv
     read_df_tcx_csv = pd.read_csv(
         filepath_or_buffer=filepath,
         sep=';',
         index_col='index',
@@ -40,21 +38,21 @@
         filepath: str,
         random_percent: float,
         random_state: int = 1,
 ) -> pd.DataFrame:
     """Return a percent of random data from extracted features.
 
     Args:
-    ----
+    ----------------
     filepath (str): Path where the extracted features are stored.
     random_percent (float): Percent of random data to return.
     random_state (int): Random state for reproducibility.
 
     Returns:
-    -------
+    ----------------
     pd.DataFrame: Random data from extracted features.
     """
     # Pandas read csv
     read_df_tcx_csv = pd.read_csv(
         filepath_or_buffer=filepath,
         sep=';',
         index_col='index',
@@ -102,15 +100,15 @@
         max_speed_max: float = 9999,
         min_speed_avg: float = 0,
         max_speed_avg: float = 9999,
 ) -> pd.DataFrame:
     """Return a number of rows based on conditions.
 
     Args:
-    ----
+    ----------------
     filepath (str): Path where the extracted features are stored.
     random_size (int): Number of random data to return.
     random_state (int): Random state for reproducibility.
     activity_type (str): Activity type to return.
     min_total_distance (float): Minimum total distance in column to return.
     max_total_distance (float): Maximum total distance in column to return.
     min_duration (float): Minimum duration in column to return.
@@ -135,15 +133,15 @@
     max_descent (float): Maximum descent in column to return.
     min_speed_max (float): Minimum maximum speed in column to return.
     max_speed_max (float): Maximum maximum speed in column to return.
     min_speed_avg (float): Minimum average speed in column to return.
     max_speed_avg (float): Maximum average speed in column to return.
 
     Returns:
-    -------
+    ----------------
     pd.DataFrame: Random data from extracted features.
     """
     # Pandas read csv
     read_df_tcx_csv = pd.read_csv(
         filepath_or_buffer=filepath,
         sep=';',
         index_col='index',
@@ -181,7 +179,36 @@
         return read_df_tcx_csv.sample(
             n=random_size,
             random_state=random_state)
     except ValueError:
         error_message = (f'Not enough data left to return {random_size} '
                          f'random data. Ease the conditions.')
         raise ValueError from ValueError(error_message)
+
+
+def filter_returned_columns(
+        columns_to_return: list,
+        df_to_filter: pd.DataFrame,
+) -> pd.DataFrame:
+    """Filter returned columns and their order.
+
+    Args:
+    ----------------
+    columns_to_return (list): Specific columns to return.
+    df_to_filter (pd.DataFrame): Any dataframe.
+
+    Returns:
+    ----------------
+    pd.DataFrame: Random data from extracted features.
+    """
+    all_possible_columns = df_to_filter.columns
+
+    # Check if columns to return are in dataframe
+    error_cols = list(set(columns_to_return) - set(all_possible_columns))
+    if error_cols:
+        # Raise error if columns are not in dataframe
+        # and show possible columns
+        error_message = (f'Columns {error_cols} not found in dataframe. '
+                         f'Possible columns are {all_possible_columns}.')
+        raise ValueError(error_message)
+
+    return df_to_filter[columns_to_return]
```

### Comparing `sportydatagen-0.2.0/sportydatagen/saf_extract_features_to_csv.py` & `sportydatagen-0.2.1/sportydatagen/saf_extract_features_to_csv.py`

 * *Files identical despite different names*

### Comparing `sportydatagen-0.2.0/sportydatagen/utils.py` & `sportydatagen-0.2.1/sportydatagen/utils.py`

 * *Files identical despite different names*

### Comparing `sportydatagen-0.2.0/setup.py` & `sportydatagen-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['niapy>=2.0.5,<3.0.0',
  'numpy>=1.24.2,<2.0.0',
  'pandas',
- 'sport-activities-features>=0.3.11,<0.4.0']
+ 'sport-activities-features>=0.3.12,<0.4.0']
 
 setup_kwargs = {
     'name': 'sportydatagen',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Sports activity generator module',
     'long_description': '# SportyDataGen -- Generator of Endurance Sports Activity Collections (datasets)\n\n## About\n\nSportyDataGen Library is a Python library designed to work with sport GPX and TCX files. It allows users to easily convert these file types into CSV format, extract feature data, and return random data based on specified conditions.\n\nIt aims to help researchers to create datasets for machine learning and data mining applications.\n\n## Features\n* Conversion of GPX and TCX files to CSV format\n* Extraction of feature data from sport files, including GPS coordinates, ascent, heart rate, distance and more\n* Merge of multiple csv files into a single dataset\n* Random selection of data based on the number of rows, percentage of rows in a file or custom conditions\n* Integration with Python scripts to provide an efficient data processing pipeline\n\n## Reference Papers:\n\nIdeas are based on the following research papers:\n\n[1] Fister, I., Jr.; Vrbančič, G.; Brezočnik, L.; Podgorelec, V.; Fister, I. [SportyDataGen: An Online Generator of Endurance Sports Activity Collections](https://www.iztok-jr-fister.eu/static/publications/225.pdf). In Proceedings of the Central European Conference on Information and Intelligent Systems, Varaždin, Croatia, 19–21 September 2018; pp. 171–178.\n\n## License\n\nThis package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.\n\n## Disclaimer\n\nThis framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!\n',
     'author': 'Rok Kukovec',
     'author_email': 'rok.kukovec1@student.um.si',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/firefly-cpp/sportydatagen',
```

### Comparing `sportydatagen-0.2.0/PKG-INFO` & `sportydatagen-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: sportydatagen
-Version: 0.2.0
+Version: 0.2.1
 Summary: Sports activity generator module
 Home-page: https://gitlab.com/firefly-cpp/sportydatagen
 License: MIT
 Keywords: artificial sport trainer,computational intelligence,data mining,sport activities,tcx
 Author: Rok Kukovec
 Author-email: rok.kukovec1@student.um.si
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: niapy (>=2.0.5,<3.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas
-Requires-Dist: sport-activities-features (>=0.3.11,<0.4.0)
+Requires-Dist: sport-activities-features (>=0.3.12,<0.4.0)
 Project-URL: Repository, https://gitlab.com/firefly-cpp/sportydatagen
 Description-Content-Type: text/markdown
 
 # SportyDataGen -- Generator of Endurance Sports Activity Collections (datasets)
 
 ## About
```

