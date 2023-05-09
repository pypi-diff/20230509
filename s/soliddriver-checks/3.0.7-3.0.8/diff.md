# Comparing `tmp/soliddriver-checks-3.0.7.tar.gz` & `tmp/soliddriver-checks-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soliddriver-checks-3.0.7.tar", last modified: Fri Apr 28 12:33:35 2023, max compression
+gzip compressed data, was "soliddriver-checks-3.0.8.tar", last modified: Tue May  9 06:36:42 2023, max compression
```

## Comparing `soliddriver-checks-3.0.7.tar` & `soliddriver-checks-3.0.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.143916 soliddriver-checks-3.0.7/
--rw-r--r--   0 hzzhao     (501) staff       (20)    18091 2022-03-31 07:35:30.000000 soliddriver-checks-3.0.7/LICENSE
--rw-r--r--   0 hzzhao     (501) staff       (20)      111 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.7/MANIFEST.in
--rw-r--r--   0 hzzhao     (501) staff       (20)     5174 2023-04-28 12:33:35.143803 soliddriver-checks-3.0.7/PKG-INFO
--rw-r--r--   0 hzzhao     (501) staff       (20)     4600 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.7/README.md
--rw-r--r--   0 hzzhao     (501) staff       (20)      107 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.7/pyproject.toml
--rw-r--r--   0 hzzhao     (501) staff       (20)       38 2023-04-28 12:33:35.143947 soliddriver-checks-3.0.7/setup.cfg
--rw-r--r--   0 hzzhao     (501) staff       (20)     1913 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/setup.py
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.139144 soliddriver-checks-3.0.7/src/
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.140586 soliddriver-checks-3.0.7/src/soliddriver_checks/
--rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-03 10:29:51.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/__init__.py
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.142042 soliddriver-checks-3.0.7/src/soliddriver_checks/api/
--rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/__init__.py
--rw-r--r--   0 hzzhao     (501) staff       (20)     1505 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/analysis.py
--rw-r--r--   0 hzzhao     (501) staff       (20)     9111 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/filter.py
--rw-r--r--   0 hzzhao     (501) staff       (20)     9805 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/km.py
--rw-r--r--   0 hzzhao     (501) staff       (20)    16773 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/kmp.py
--rw-r--r--   0 hzzhao     (501) staff       (20)      832 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/raw_data.py
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.142259 soliddriver-checks-3.0.7/src/soliddriver_checks/api/utils/
--rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/utils/__init__.py
--rw-r--r--   0 hzzhao     (501) staff       (20)     1795 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/utils/cmd.py
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.142365 soliddriver-checks-3.0.7/src/soliddriver_checks/api/utils/scripts/
--rwxr-xr-x   0 hzzhao     (501) staff       (20)      857 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/utils/scripts/check-links.sh
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.142999 soliddriver-checks-3.0.7/src/soliddriver_checks/cli/
--rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/cli/__init__.py
--rw-r--r--   0 hzzhao     (501) staff       (20)     6407 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/cli/cli.py
--rw-r--r--   0 hzzhao     (501) staff       (20)     6932 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/cli/km_report.py
--rw-r--r--   0 hzzhao     (501) staff       (20)    15074 2022-12-30 09:00:29.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/cli/kmp_report.py
--rw-r--r--   0 hzzhao     (501) staff       (20)      611 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/cli/terminal_logs.py
--rw-r--r--   0 hzzhao     (501) staff       (20)     7835 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/cli/xlsx_utils.py
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.143108 soliddriver-checks-3.0.7/src/soliddriver_checks/config/
--rw-r--r--   0 hzzhao     (501) staff       (20)     5884 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/config/soliddriver-checks.conf
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.143453 soliddriver-checks-3.0.7/src/soliddriver_checks/config/templates/
--rw-r--r--   0 hzzhao     (501) staff       (20)     3431 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/config/templates/km-report.html.jinja
--rw-r--r--   0 hzzhao     (501) staff       (20)     4675 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/config/templates/kmp-report.html.jinja
--rw-r--r--   0 hzzhao     (501) staff       (20)    13833 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/config/templates/templates.xlsx
--rw-r--r--   0 hzzhao     (501) staff       (20)     3720 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/config.py
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.143652 soliddriver-checks-3.0.7/src/soliddriver_checks/service/
--rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-18 08:10:10.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/service/__init__.py
--rw-r--r--   0 hzzhao     (501) staff       (20)     1646 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/service/service.py
--rw-r--r--   0 hzzhao     (501) staff       (20)      101 2023-04-28 12:30:59.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/version.py
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.141371 soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/
--rw-r--r--   0 hzzhao     (501) staff       (20)     5174 2023-04-28 12:33:35.000000 soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/PKG-INFO
--rw-r--r--   0 hzzhao     (501) staff       (20)     1351 2023-04-28 12:33:35.000000 soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/SOURCES.txt
--rw-r--r--   0 hzzhao     (501) staff       (20)        1 2023-04-28 12:33:35.000000 soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/dependency_links.txt
--rw-r--r--   0 hzzhao     (501) staff       (20)      149 2023-04-28 12:33:35.000000 soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/entry_points.txt
--rw-r--r--   0 hzzhao     (501) staff       (20)      139 2023-04-28 12:33:35.000000 soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/requires.txt
--rw-r--r--   0 hzzhao     (501) staff       (20)       19 2023-04-28 12:33:35.000000 soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/top_level.txt
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-05-09 06:36:42.857736 soliddriver-checks-3.0.8/
+-rw-r--r--   0 hzzhao     (501) staff       (20)    18091 2022-03-31 07:35:30.000000 soliddriver-checks-3.0.8/LICENSE
+-rw-r--r--   0 hzzhao     (501) staff       (20)      111 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.8/MANIFEST.in
+-rw-r--r--   0 hzzhao     (501) staff       (20)     5174 2023-05-09 06:36:42.857627 soliddriver-checks-3.0.8/PKG-INFO
+-rw-r--r--   0 hzzhao     (501) staff       (20)     4600 2023-05-04 11:53:40.000000 soliddriver-checks-3.0.8/README.md
+-rw-r--r--   0 hzzhao     (501) staff       (20)      107 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.8/pyproject.toml
+-rw-r--r--   0 hzzhao     (501) staff       (20)       38 2023-05-09 06:36:42.857765 soliddriver-checks-3.0.8/setup.cfg
+-rw-r--r--   0 hzzhao     (501) staff       (20)     1913 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.8/setup.py
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-05-09 06:36:42.852867 soliddriver-checks-3.0.8/src/
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-05-09 06:36:42.854274 soliddriver-checks-3.0.8/src/soliddriver_checks/
+-rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-03 10:29:51.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/__init__.py
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-05-09 06:36:42.855646 soliddriver-checks-3.0.8/src/soliddriver_checks/api/
+-rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/api/__init__.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)     1505 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/api/analysis.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)     9111 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/api/filter.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)     9805 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/api/km.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)    16773 2023-05-09 06:15:29.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/api/kmp.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)      832 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/api/raw_data.py
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-05-09 06:36:42.855978 soliddriver-checks-3.0.8/src/soliddriver_checks/api/utils/
+-rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/api/utils/__init__.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)     1795 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/api/utils/cmd.py
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-05-09 06:36:42.856085 soliddriver-checks-3.0.8/src/soliddriver_checks/api/utils/scripts/
+-rwxr-xr-x   0 hzzhao     (501) staff       (20)      857 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/api/utils/scripts/check-links.sh
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-05-09 06:36:42.856744 soliddriver-checks-3.0.8/src/soliddriver_checks/cli/
+-rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/cli/__init__.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)     6407 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/cli/cli.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)     6932 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/cli/km_report.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)    15074 2022-12-30 09:00:29.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/cli/kmp_report.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)      611 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/cli/terminal_logs.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)     7835 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/cli/xlsx_utils.py
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-05-09 06:36:42.856879 soliddriver-checks-3.0.8/src/soliddriver_checks/config/
+-rw-r--r--   0 hzzhao     (501) staff       (20)     5884 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/config/soliddriver-checks.conf
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-05-09 06:36:42.857224 soliddriver-checks-3.0.8/src/soliddriver_checks/config/templates/
+-rw-r--r--   0 hzzhao     (501) staff       (20)     3431 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/config/templates/km-report.html.jinja
+-rw-r--r--   0 hzzhao     (501) staff       (20)     4675 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/config/templates/kmp-report.html.jinja
+-rw-r--r--   0 hzzhao     (501) staff       (20)    13833 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/config/templates/templates.xlsx
+-rw-r--r--   0 hzzhao     (501) staff       (20)     3720 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/config.py
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-05-09 06:36:42.857455 soliddriver-checks-3.0.8/src/soliddriver_checks/service/
+-rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-18 08:10:10.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/service/__init__.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)     1646 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/service/service.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)      101 2023-05-09 06:20:41.000000 soliddriver-checks-3.0.8/src/soliddriver_checks/version.py
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-05-09 06:36:42.854962 soliddriver-checks-3.0.8/src/soliddriver_checks.egg-info/
+-rw-r--r--   0 hzzhao     (501) staff       (20)     5174 2023-05-09 06:36:42.000000 soliddriver-checks-3.0.8/src/soliddriver_checks.egg-info/PKG-INFO
+-rw-r--r--   0 hzzhao     (501) staff       (20)     1351 2023-05-09 06:36:42.000000 soliddriver-checks-3.0.8/src/soliddriver_checks.egg-info/SOURCES.txt
+-rw-r--r--   0 hzzhao     (501) staff       (20)        1 2023-05-09 06:36:42.000000 soliddriver-checks-3.0.8/src/soliddriver_checks.egg-info/dependency_links.txt
+-rw-r--r--   0 hzzhao     (501) staff       (20)      149 2023-05-09 06:36:42.000000 soliddriver-checks-3.0.8/src/soliddriver_checks.egg-info/entry_points.txt
+-rw-r--r--   0 hzzhao     (501) staff       (20)      139 2023-05-09 06:36:42.000000 soliddriver-checks-3.0.8/src/soliddriver_checks.egg-info/requires.txt
+-rw-r--r--   0 hzzhao     (501) staff       (20)       19 2023-05-09 06:36:42.000000 soliddriver-checks-3.0.8/src/soliddriver_checks.egg-info/top_level.txt
```

### Comparing `soliddriver-checks-3.0.7/LICENSE` & `soliddriver-checks-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/PKG-INFO` & `soliddriver-checks-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: soliddriver-checks
-Version: 3.0.7
+Version: 3.0.8
 Summary: Check Kernel Module Package and Kernel Module information
 Home-page: https://github.com/SUSE/soliddriver-checks
 Author: Hui-Zhi Zhao
 Author-email: hui.zhi.zhao@suse.com
 Project-URL: Bug Tracker, https://github.com/SUSE/soliddriver-checks/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # soliddriver-checks
 
-```soliddriver-checks is``` A tool for ```KMP(Kernel Module Package)``` and ```installed/running kernel module``` checking, with this tool, users can have an report of their KMP(s) and KM status (the report can be formatted in ```html```, ```excel``` and ```json```), the tool can be run as command line tool or service:
+```soliddriver-checks is``` a tool for ```KMP(Kernel Module Package)``` and ```installed/running kernel module``` checking, with this tool, users can have an report of their KMP(s) and KM status (the report can be formatted in ```html```, ```excel``` and ```json```), the tool can be run as command line tool or service:
 
 ##### Note: This tool only check the KMP and KM are built meet SUSE’s requirement, don’t look into the code perspective. So any bugs or security related issues inside the kernel module can not be found.
 
 - KM: kernel module
 - KMP: kernel module package
 
 ## Installation:
```

### Comparing `soliddriver-checks-3.0.7/README.md` & `soliddriver-checks-3.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # soliddriver-checks
 
-```soliddriver-checks is``` A tool for ```KMP(Kernel Module Package)``` and ```installed/running kernel module``` checking, with this tool, users can have an report of their KMP(s) and KM status (the report can be formatted in ```html```, ```excel``` and ```json```), the tool can be run as command line tool or service:
+```soliddriver-checks is``` a tool for ```KMP(Kernel Module Package)``` and ```installed/running kernel module``` checking, with this tool, users can have an report of their KMP(s) and KM status (the report can be formatted in ```html```, ```excel``` and ```json```), the tool can be run as command line tool or service:
 
 ##### Note: This tool only check the KMP and KM are built meet SUSE’s requirement, don’t look into the code perspective. So any bugs or security related issues inside the kernel module can not be found.
 
 - KM: kernel module
 - KMP: kernel module package
 
 ## Installation:
```

### Comparing `soliddriver-checks-3.0.7/setup.py` & `soliddriver-checks-3.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/api/analysis.py` & `soliddriver-checks-3.0.8/src/soliddriver_checks/api/analysis.py`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/api/filter.py` & `soliddriver-checks-3.0.8/src/soliddriver_checks/api/filter.py`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/api/km.py` & `soliddriver-checks-3.0.8/src/soliddriver_checks/api/km.py`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/api/kmp.py` & `soliddriver-checks-3.0.8/src/soliddriver_checks/api/kmp.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,16 +191,16 @@
         eval, alaias_msg = self._kms_modalias_analysis(kmp_modalias, km_info)
         ana_level.append(eval["value"])
 
         ana_summary = {
             "license": self._kmp_km_ana_summary(km_analysis, "license"),
             "supported": self._kmp_km_ana_summary(km_analysis, "supported"),
             "signature": self._kmp_km_ana_summary(km_analysis, "signature"),
-            "symbols": {"level": eval, "value": alaias_msg},
-            "alias": self._kmp_km_ana_summary(km_analysis, "symbols"),
+            "symbols": self._kmp_km_ana_summary(km_analysis, "symbols"),
+            "alias": {"level": eval, "value": alaias_msg},
         }
 
         return KMPEvaluation(max(ana_level)).to_json(), ana_summary
 
     def _kms_symbols_analysis(self, kmp_reqs, km_syms):
         syms = {}
         syms["unfound"] = []
```

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/api/raw_data.py` & `soliddriver-checks-3.0.8/src/soliddriver_checks/api/raw_data.py`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/api/utils/cmd.py` & `soliddriver-checks-3.0.8/src/soliddriver_checks/api/utils/cmd.py`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/api/utils/scripts/check-links.sh` & `soliddriver-checks-3.0.8/src/soliddriver_checks/api/utils/scripts/check-links.sh`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/cli/cli.py` & `soliddriver-checks-3.0.8/src/soliddriver_checks/cli/cli.py`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/cli/km_report.py` & `soliddriver-checks-3.0.8/src/soliddriver_checks/cli/km_report.py`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/cli/kmp_report.py` & `soliddriver-checks-3.0.8/src/soliddriver_checks/cli/kmp_report.py`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/cli/terminal_logs.py` & `soliddriver-checks-3.0.8/src/soliddriver_checks/cli/terminal_logs.py`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/cli/xlsx_utils.py` & `soliddriver-checks-3.0.8/src/soliddriver_checks/cli/xlsx_utils.py`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/config/soliddriver-checks.conf` & `soliddriver-checks-3.0.8/src/soliddriver_checks/config/soliddriver-checks.conf`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/config/templates/km-report.html.jinja` & `soliddriver-checks-3.0.8/src/soliddriver_checks/config/templates/km-report.html.jinja`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/config/templates/kmp-report.html.jinja` & `soliddriver-checks-3.0.8/src/soliddriver_checks/config/templates/kmp-report.html.jinja`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/config/templates/templates.xlsx` & `soliddriver-checks-3.0.8/src/soliddriver_checks/config/templates/templates.xlsx`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/config.py` & `soliddriver-checks-3.0.8/src/soliddriver_checks/config.py`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks/service/service.py` & `soliddriver-checks-3.0.8/src/soliddriver_checks/service/service.py`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/PKG-INFO` & `soliddriver-checks-3.0.8/src/soliddriver_checks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: soliddriver-checks
-Version: 3.0.7
+Version: 3.0.8
 Summary: Check Kernel Module Package and Kernel Module information
 Home-page: https://github.com/SUSE/soliddriver-checks
 Author: Hui-Zhi Zhao
 Author-email: hui.zhi.zhao@suse.com
 Project-URL: Bug Tracker, https://github.com/SUSE/soliddriver-checks/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # soliddriver-checks
 
-```soliddriver-checks is``` A tool for ```KMP(Kernel Module Package)``` and ```installed/running kernel module``` checking, with this tool, users can have an report of their KMP(s) and KM status (the report can be formatted in ```html```, ```excel``` and ```json```), the tool can be run as command line tool or service:
+```soliddriver-checks is``` a tool for ```KMP(Kernel Module Package)``` and ```installed/running kernel module``` checking, with this tool, users can have an report of their KMP(s) and KM status (the report can be formatted in ```html```, ```excel``` and ```json```), the tool can be run as command line tool or service:
 
 ##### Note: This tool only check the KMP and KM are built meet SUSE’s requirement, don’t look into the code perspective. So any bugs or security related issues inside the kernel module can not be found.
 
 - KM: kernel module
 - KMP: kernel module package
 
 ## Installation:
```

### Comparing `soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/SOURCES.txt` & `soliddriver-checks-3.0.8/src/soliddriver_checks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

