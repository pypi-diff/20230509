# Comparing `tmp/vcftoolz-1.2.0.tar.gz` & `tmp/vcftoolz-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vcftoolz-1.2.0.tar", last modified: Thu Apr  4 15:11:50 2019, max compression
+gzip compressed data, was "vcftoolz-1.2.1.tar", last modified: Tue May  9 03:14:53 2023, max compression
```

## Comparing `vcftoolz-1.2.0.tar` & `vcftoolz-1.2.1.tar`

### file list

```diff
@@ -1,42 +1,38 @@
-drwx------   0 steven.davis (2052855671) domainus (10000)        0 2019-04-04 15:11:50.000000 vcftoolz-1.2.0/
--rw-------   0 steven.davis (2052855671) domainus (10000)     1556 2018-11-15 13:47:39.000000 vcftoolz-1.2.0/LICENSE
--rw-------   0 steven.davis (2052855671) domainus (10000)      891 2019-04-04 14:23:01.000000 vcftoolz-1.2.0/HISTORY.rst
-drwx------   0 steven.davis (2052855671) domainus (10000)        0 2019-04-04 15:11:50.000000 vcftoolz-1.2.0/pyvenn/
--rw-------   0 steven.davis (2052855671) domainus (10000)     1184 2018-01-03 19:57:54.000000 vcftoolz-1.2.0/pyvenn/demo.py
--rw-------   0 steven.davis (2052855671) domainus (10000)        0 2018-01-03 19:57:54.000000 vcftoolz-1.2.0/pyvenn/__init__.py
--rw-------   0 steven.davis (2052855671) domainus (10000)    22120 2018-01-04 21:43:17.000000 vcftoolz-1.2.0/pyvenn/venn.py
--rwx------   0 steven.davis (2052855671) domainus (10000)     1857 2019-04-04 14:28:32.000000 vcftoolz-1.2.0/setup.py
--rw-------   0 steven.davis (2052855671) domainus (10000)      159 2019-04-04 15:11:50.000000 vcftoolz-1.2.0/setup.cfg
--rw-------   0 steven.davis (2052855671) domainus (10000)     3327 2019-04-01 15:18:59.000000 vcftoolz-1.2.0/CONTRIBUTING.rst
-drwx------   0 steven.davis (2052855671) domainus (10000)        0 2019-04-04 15:11:50.000000 vcftoolz-1.2.0/docs/
--rw-------   0 steven.davis (2052855671) domainus (10000)      451 2018-11-15 13:47:39.000000 vcftoolz-1.2.0/docs/index.rst
--rw-------   0 steven.davis (2052855671) domainus (10000)     8624 2019-04-04 15:06:16.000000 vcftoolz-1.2.0/docs/usage.rst
--rw-------   0 steven.davis (2052855671) domainus (10000)     6463 2018-11-15 13:47:39.000000 vcftoolz-1.2.0/docs/make.bat
--rw-------   0 steven.davis (2052855671) domainus (10000)       28 2018-11-15 13:47:39.000000 vcftoolz-1.2.0/docs/authors.rst
--rw-------   0 steven.davis (2052855671) domainus (10000)       33 2018-11-15 13:47:39.000000 vcftoolz-1.2.0/docs/contributing.rst
--rw-------   0 steven.davis (2052855671) domainus (10000)     6770 2018-11-15 13:47:39.000000 vcftoolz-1.2.0/docs/Makefile
--rw-------   0 steven.davis (2052855671) domainus (10000)      713 2018-11-15 13:47:39.000000 vcftoolz-1.2.0/docs/installation.rst
--rw-------   0 steven.davis (2052855671) domainus (10000)       27 2018-11-15 13:47:39.000000 vcftoolz-1.2.0/docs/readme.rst
--rwx------   0 steven.davis (2052855671) domainus (10000)     9411 2018-11-15 15:00:45.000000 vcftoolz-1.2.0/docs/conf.py
--rw-------   0 steven.davis (2052855671) domainus (10000)       28 2018-11-15 13:47:39.000000 vcftoolz-1.2.0/docs/history.rst
--rw-------   0 steven.davis (2052855671) domainus (10000)     1954 2019-04-04 14:56:12.000000 vcftoolz-1.2.0/README.rst
-drwx------   0 steven.davis (2052855671) domainus (10000)        0 2019-04-04 15:11:50.000000 vcftoolz-1.2.0/tests/
--rwx------   0 steven.davis (2052855671) domainus (10000)       24 2018-11-15 13:47:39.000000 vcftoolz-1.2.0/tests/__init__.py
--rwx------   0 steven.davis (2052855671) domainus (10000)     3198 2018-11-19 21:14:42.000000 vcftoolz-1.2.0/tests/test_vcftoolz.py
--rw-------   0 steven.davis (2052855671) domainus (10000)      299 2018-11-15 13:47:39.000000 vcftoolz-1.2.0/tests/test_cli.py
--rw-------   0 steven.davis (2052855671) domainus (10000)      220 2018-11-15 16:10:21.000000 vcftoolz-1.2.0/AUTHORS.rst
-drwx------   0 steven.davis (2052855671) domainus (10000)        0 2019-04-04 15:11:50.000000 vcftoolz-1.2.0/vcftoolz/
--rwx------   0 steven.davis (2052855671) domainus (10000)    45814 2019-04-03 21:03:03.000000 vcftoolz-1.2.0/vcftoolz/vcftoolz.py
--rwx------   0 steven.davis (2052855671) domainus (10000)    28430 2019-02-04 15:39:52.000000 vcftoolz-1.2.0/vcftoolz/vcf_call_parser.py
--rw-------   0 steven.davis (2052855671) domainus (10000)    13994 2019-04-04 14:38:56.000000 vcftoolz-1.2.0/vcftoolz/cli.py
--rwx------   0 steven.davis (2052855671) domainus (10000)      113 2019-04-04 14:28:51.000000 vcftoolz-1.2.0/vcftoolz/__init__.py
--rw-------   0 steven.davis (2052855671) domainus (10000)     4484 2019-04-04 15:11:50.000000 vcftoolz-1.2.0/PKG-INFO
--rw-------   0 steven.davis (2052855671) domainus (10000)      244 2018-11-15 13:47:39.000000 vcftoolz-1.2.0/MANIFEST.in
-drwx------   0 steven.davis (2052855671) domainus (10000)        0 2019-04-04 15:11:50.000000 vcftoolz-1.2.0/vcftoolz.egg-info/
--rw-------   0 steven.davis (2052855671) domainus (10000)      674 2019-04-04 15:11:50.000000 vcftoolz-1.2.0/vcftoolz.egg-info/SOURCES.txt
--rw-------   0 steven.davis (2052855671) domainus (10000)       16 2019-04-04 15:11:50.000000 vcftoolz-1.2.0/vcftoolz.egg-info/top_level.txt
--rw-------   0 steven.davis (2052855671) domainus (10000)       56 2019-04-04 15:11:50.000000 vcftoolz-1.2.0/vcftoolz.egg-info/requires.txt
--rw-------   0 steven.davis (2052855671) domainus (10000)     4484 2019-04-04 15:11:50.000000 vcftoolz-1.2.0/vcftoolz.egg-info/PKG-INFO
--rw-------   0 steven.davis (2052855671) domainus (10000)        1 2019-04-04 14:29:32.000000 vcftoolz-1.2.0/vcftoolz.egg-info/not-zip-safe
--rw-------   0 steven.davis (2052855671) domainus (10000)       48 2019-04-04 15:11:50.000000 vcftoolz-1.2.0/vcftoolz.egg-info/entry_points.txt
--rw-------   0 steven.davis (2052855671) domainus (10000)        1 2019-04-04 15:11:50.000000 vcftoolz-1.2.0/vcftoolz.egg-info/dependency_links.txt
+drwxrwxrwx   0 chet      (1000) chet      (1000)        0 2023-05-09 03:14:53.914941 vcftoolz-1.2.1/
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      220 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/AUTHORS.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     3327 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/CONTRIBUTING.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      891 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/HISTORY.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     1556 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/LICENSE
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      244 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/MANIFEST.in
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     3825 2023-05-09 03:14:53.915941 vcftoolz-1.2.1/PKG-INFO
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     1954 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/README.rst
+drwxrwxrwx   0 chet      (1000) chet      (1000)        0 2023-05-09 03:14:53.558073 vcftoolz-1.2.1/docs/
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     6770 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/Makefile
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       28 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/authors.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     9411 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/conf.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       33 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/contributing.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       28 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/history.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      451 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/index.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      713 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/installation.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     6463 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/make.bat
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       27 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/readme.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     8624 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/usage.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      159 2023-05-09 03:14:53.922938 vcftoolz-1.2.1/setup.cfg
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     1858 2023-05-09 03:11:12.000000 vcftoolz-1.2.1/setup.py
+drwxrwxrwx   0 chet      (1000) chet      (1000)        0 2023-05-09 03:14:53.632073 vcftoolz-1.2.1/tests/
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       24 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/tests/__init__.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      299 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/tests/test_cli.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     3198 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/tests/test_vcftoolz.py
+drwxrwxrwx   0 chet      (1000) chet      (1000)        0 2023-05-09 03:14:53.727075 vcftoolz-1.2.1/vcftoolz/
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      113 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/vcftoolz/__init__.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)    13994 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/vcftoolz/cli.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)    28430 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/vcftoolz/vcf_call_parser.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)    45814 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/vcftoolz/vcftoolz.py
+drwxrwxrwx   0 chet      (1000) chet      (1000)        0 2023-05-09 03:14:53.889942 vcftoolz-1.2.1/vcftoolz.egg-info/
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     3825 2023-05-09 03:14:50.000000 vcftoolz-1.2.1/vcftoolz.egg-info/PKG-INFO
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      625 2023-05-09 03:14:50.000000 vcftoolz-1.2.1/vcftoolz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 chet      (1000) chet      (1000)        1 2023-05-09 03:14:50.000000 vcftoolz-1.2.1/vcftoolz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       48 2023-05-09 03:14:50.000000 vcftoolz-1.2.1/vcftoolz.egg-info/entry_points.txt
+-rwxrwxrwx   0 chet      (1000) chet      (1000)        1 2023-05-09 03:14:50.000000 vcftoolz-1.2.1/vcftoolz.egg-info/not-zip-safe
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       57 2023-05-09 03:14:50.000000 vcftoolz-1.2.1/vcftoolz.egg-info/requires.txt
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       16 2023-05-09 03:14:50.000000 vcftoolz-1.2.1/vcftoolz.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vcftoolz-1.2.0/LICENSE` & `vcftoolz-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.0/HISTORY.rst` & `vcftoolz-1.2.1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.0/setup.py` & `vcftoolz-1.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 with open('HISTORY.rst') as history_file:
     history = history_file.read().replace('.. :changelog:', '')
 
 requirements = [
     'biopython',
     'numpy',
     'pandas',
-    'PyVCF',
+    'PyVCF3',
     'matplotlib',
     'matplotlib_venn',
 ]
 
 test_requirements = [
     "pytest",
 ]
 
 setup(
     name='vcftoolz',
-    version='1.2.0',
+    version='1.2.1',
     description="Tools for working with Variant Call Format files.",
     long_description=readme + '\n\n' + history,
     author="Steve Davis",
     author_email='steven.davis@fda.hhs.gov',
     url='https://github.com/CFSAN-Biostatistics/vcftoolz',
     packages=[
         'pyvenn',
```

### Comparing `vcftoolz-1.2.0/CONTRIBUTING.rst` & `vcftoolz-1.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.0/docs/usage.rst` & `vcftoolz-1.2.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.0/docs/make.bat` & `vcftoolz-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.0/docs/Makefile` & `vcftoolz-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.0/docs/installation.rst` & `vcftoolz-1.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.0/docs/conf.py` & `vcftoolz-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.0/README.rst` & `vcftoolz-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.0/tests/test_vcftoolz.py` & `vcftoolz-1.2.1/tests/test_vcftoolz.py`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.0/vcftoolz/vcftoolz.py` & `vcftoolz-1.2.1/vcftoolz/vcftoolz.py`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.0/vcftoolz/vcf_call_parser.py` & `vcftoolz-1.2.1/vcftoolz/vcf_call_parser.py`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.0/vcftoolz/cli.py` & `vcftoolz-1.2.1/vcftoolz/cli.py`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.0/PKG-INFO` & `vcftoolz-1.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: vcftoolz
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tools for working with Variant Call Format files.
 Home-page: https://github.com/CFSAN-Biostatistics/vcftoolz
 Author: Steve Davis
 Author-email: steven.davis@fda.hhs.gov
 License: BSD
-Description: ===============================
-        VCF Toolz
-        ===============================
-        
-        
-        .. Image showing the PyPI version badge - links to PyPI
-        .. image:: https://img.shields.io/pypi/v/vcftoolz.svg
-                :target: https://pypi.python.org/pypi/vcftoolz
-        
-        .. Image showing the Travis Continuous Integration test status, commented out for now
-        .. .. image:: https://img.shields.io/travis/CFSAN-Biostatistics/vcftoolz.svg
-        ..        :target: https://travis-ci.org/CFSAN-Biostatistics/vcftoolz
-        
-        .. Image showing the JOSS paper badge
-        .. image:: http://joss.theoj.org/papers/10.21105/joss.01144/status.svg
-           :target: https://doi.org/10.21105/joss.01144
-        
-        Tools for working with Variant Call Format files.
-        
-        VCF Toolz was developed by the United States Food
-        and Drug Administration, Center for Food Safety and Applied Nutrition.
-        
-        * Free software
-        * Documentation: https://vcftoolz.readthedocs.io
-        * Source Code: https://github.com/CFSAN-Biostatistics/vcftoolz
-        * PyPI Distribution: https://pypi.python.org/pypi/vcftoolz
-        
-        
-        Features
-        --------
-        
-        * Compares the snps in two or more VCF files.
-        * Lists the snps that are unique to each VCF file with full genotype information per snp.
-        * Lists the snps that are missing from each VCF file if present in at least two other VCF files.
-        * Generates Venn diagrams of positions and snps in the VCF files.
-        * Reports precision, recall, and F1 score when the truth is known.
-        * Reports the effectiveness of filtered variants when the truth is known.
-        * Reformat the VCF file in a tall-narrow format for easy viewing and diffs.
-        * Count samples, positions, calls, snps, indels, other variants, missing calls, and filter reasons.
-        * Plot calls along the length of the genome and show the location of filtered calls.
-        
-        
-        Citing VCF Toolz
-        --------------------------------------
-        
-        To cite VCF Toolz, please reference the VCF Toolz paper:
-        
-            https://doi.org/10.21105/joss.01144
-        
-        
-        License
-        -------
-        
-        See the LICENSE file included in the VCF Toolz distribution.
-        
-        
-        
-        
-        
-        History
-        =======
-        
-        1.2.0 (2019-04-04)
-        ---------------------
-        * Fix defect in narrow command wrongly printing ALT=. when GT=.
-        * Add the ``count`` command to count samples, positions, calls, snps, indels,
-          other variants, filtered calls, missing calls, and filter reasons.
-        * Add the ``plot`` command to plot calls along the length of the genome and show
-          the location of filtered calls.
-        * Change the text of the compare report to refer to "Calls", not "Sample snps".
-        * Drop support for Python 3.4, which is not supported by matplotlib.
-        * Add support for Python 3.7.
-        
-        1.1.1 (2019-03-26)
-        ---------------------
-        * Replace None with '.' when printing call data.
-        * Support VCF files with multiple alternate alleles per position.
-        
-        1.1.0 (2019-02-06)
-        ---------------------
-        * Support reading gzip compressed vcf files.
-        
-        
-        1.0.0 (2018-11-20)
-        ---------------------
-        
-        * First public release.
-        
 Keywords: bioinformatics,NGS,vcftoolz
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Freely Distributable
 Classifier: Natural Language :: English
@@ -105,7 +17,99 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+===============================
+VCF Toolz
+===============================
+
+
+.. Image showing the PyPI version badge - links to PyPI
+.. image:: https://img.shields.io/pypi/v/vcftoolz.svg
+        :target: https://pypi.python.org/pypi/vcftoolz
+
+.. Image showing the Travis Continuous Integration test status, commented out for now
+.. .. image:: https://img.shields.io/travis/CFSAN-Biostatistics/vcftoolz.svg
+..        :target: https://travis-ci.org/CFSAN-Biostatistics/vcftoolz
+
+.. Image showing the JOSS paper badge
+.. image:: http://joss.theoj.org/papers/10.21105/joss.01144/status.svg
+   :target: https://doi.org/10.21105/joss.01144
+
+Tools for working with Variant Call Format files.
+
+VCF Toolz was developed by the United States Food
+and Drug Administration, Center for Food Safety and Applied Nutrition.
+
+* Free software
+* Documentation: https://vcftoolz.readthedocs.io
+* Source Code: https://github.com/CFSAN-Biostatistics/vcftoolz
+* PyPI Distribution: https://pypi.python.org/pypi/vcftoolz
+
+
+Features
+--------
+
+* Compares the snps in two or more VCF files.
+* Lists the snps that are unique to each VCF file with full genotype information per snp.
+* Lists the snps that are missing from each VCF file if present in at least two other VCF files.
+* Generates Venn diagrams of positions and snps in the VCF files.
+* Reports precision, recall, and F1 score when the truth is known.
+* Reports the effectiveness of filtered variants when the truth is known.
+* Reformat the VCF file in a tall-narrow format for easy viewing and diffs.
+* Count samples, positions, calls, snps, indels, other variants, missing calls, and filter reasons.
+* Plot calls along the length of the genome and show the location of filtered calls.
+
+
+Citing VCF Toolz
+--------------------------------------
+
+To cite VCF Toolz, please reference the VCF Toolz paper:
+
+    https://doi.org/10.21105/joss.01144
+
+
+License
+-------
+
+See the LICENSE file included in the VCF Toolz distribution.
+
+
+
+
+
+History
+=======
+
+1.2.0 (2019-04-04)
+---------------------
+* Fix defect in narrow command wrongly printing ALT=. when GT=.
+* Add the ``count`` command to count samples, positions, calls, snps, indels,
+  other variants, filtered calls, missing calls, and filter reasons.
+* Add the ``plot`` command to plot calls along the length of the genome and show
+  the location of filtered calls.
+* Change the text of the compare report to refer to "Calls", not "Sample snps".
+* Drop support for Python 3.4, which is not supported by matplotlib.
+* Add support for Python 3.7.
+
+1.1.1 (2019-03-26)
+---------------------
+* Replace None with '.' when printing call data.
+* Support VCF files with multiple alternate alleles per position.
+
+1.1.0 (2019-02-06)
+---------------------
+* Support reading gzip compressed vcf files.
+
+
+1.0.0 (2018-11-20)
+---------------------
+
+* First public release.
+
+
```

### Comparing `vcftoolz-1.2.0/vcftoolz.egg-info/SOURCES.txt` & `vcftoolz-1.2.1/vcftoolz.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,17 +12,14 @@
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
-pyvenn/__init__.py
-pyvenn/demo.py
-pyvenn/venn.py
 tests/__init__.py
 tests/test_cli.py
 tests/test_vcftoolz.py
 vcftoolz/__init__.py
 vcftoolz/cli.py
 vcftoolz/vcf_call_parser.py
 vcftoolz/vcftoolz.py
```

### Comparing `vcftoolz-1.2.0/vcftoolz.egg-info/PKG-INFO` & `vcftoolz-1.2.1/vcftoolz.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: vcftoolz
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tools for working with Variant Call Format files.
 Home-page: https://github.com/CFSAN-Biostatistics/vcftoolz
 Author: Steve Davis
 Author-email: steven.davis@fda.hhs.gov
 License: BSD
-Description: ===============================
-        VCF Toolz
-        ===============================
-        
-        
-        .. Image showing the PyPI version badge - links to PyPI
-        .. image:: https://img.shields.io/pypi/v/vcftoolz.svg
-                :target: https://pypi.python.org/pypi/vcftoolz
-        
-        .. Image showing the Travis Continuous Integration test status, commented out for now
-        .. .. image:: https://img.shields.io/travis/CFSAN-Biostatistics/vcftoolz.svg
-        ..        :target: https://travis-ci.org/CFSAN-Biostatistics/vcftoolz
-        
-        .. Image showing the JOSS paper badge
-        .. image:: http://joss.theoj.org/papers/10.21105/joss.01144/status.svg
-           :target: https://doi.org/10.21105/joss.01144
-        
-        Tools for working with Variant Call Format files.
-        
-        VCF Toolz was developed by the United States Food
-        and Drug Administration, Center for Food Safety and Applied Nutrition.
-        
-        * Free software
-        * Documentation: https://vcftoolz.readthedocs.io
-        * Source Code: https://github.com/CFSAN-Biostatistics/vcftoolz
-        * PyPI Distribution: https://pypi.python.org/pypi/vcftoolz
-        
-        
-        Features
-        --------
-        
-        * Compares the snps in two or more VCF files.
-        * Lists the snps that are unique to each VCF file with full genotype information per snp.
-        * Lists the snps that are missing from each VCF file if present in at least two other VCF files.
-        * Generates Venn diagrams of positions and snps in the VCF files.
-        * Reports precision, recall, and F1 score when the truth is known.
-        * Reports the effectiveness of filtered variants when the truth is known.
-        * Reformat the VCF file in a tall-narrow format for easy viewing and diffs.
-        * Count samples, positions, calls, snps, indels, other variants, missing calls, and filter reasons.
-        * Plot calls along the length of the genome and show the location of filtered calls.
-        
-        
-        Citing VCF Toolz
-        --------------------------------------
-        
-        To cite VCF Toolz, please reference the VCF Toolz paper:
-        
-            https://doi.org/10.21105/joss.01144
-        
-        
-        License
-        -------
-        
-        See the LICENSE file included in the VCF Toolz distribution.
-        
-        
-        
-        
-        
-        History
-        =======
-        
-        1.2.0 (2019-04-04)
-        ---------------------
-        * Fix defect in narrow command wrongly printing ALT=. when GT=.
-        * Add the ``count`` command to count samples, positions, calls, snps, indels,
-          other variants, filtered calls, missing calls, and filter reasons.
-        * Add the ``plot`` command to plot calls along the length of the genome and show
-          the location of filtered calls.
-        * Change the text of the compare report to refer to "Calls", not "Sample snps".
-        * Drop support for Python 3.4, which is not supported by matplotlib.
-        * Add support for Python 3.7.
-        
-        1.1.1 (2019-03-26)
-        ---------------------
-        * Replace None with '.' when printing call data.
-        * Support VCF files with multiple alternate alleles per position.
-        
-        1.1.0 (2019-02-06)
-        ---------------------
-        * Support reading gzip compressed vcf files.
-        
-        
-        1.0.0 (2018-11-20)
-        ---------------------
-        
-        * First public release.
-        
 Keywords: bioinformatics,NGS,vcftoolz
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Freely Distributable
 Classifier: Natural Language :: English
@@ -105,7 +17,99 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+===============================
+VCF Toolz
+===============================
+
+
+.. Image showing the PyPI version badge - links to PyPI
+.. image:: https://img.shields.io/pypi/v/vcftoolz.svg
+        :target: https://pypi.python.org/pypi/vcftoolz
+
+.. Image showing the Travis Continuous Integration test status, commented out for now
+.. .. image:: https://img.shields.io/travis/CFSAN-Biostatistics/vcftoolz.svg
+..        :target: https://travis-ci.org/CFSAN-Biostatistics/vcftoolz
+
+.. Image showing the JOSS paper badge
+.. image:: http://joss.theoj.org/papers/10.21105/joss.01144/status.svg
+   :target: https://doi.org/10.21105/joss.01144
+
+Tools for working with Variant Call Format files.
+
+VCF Toolz was developed by the United States Food
+and Drug Administration, Center for Food Safety and Applied Nutrition.
+
+* Free software
+* Documentation: https://vcftoolz.readthedocs.io
+* Source Code: https://github.com/CFSAN-Biostatistics/vcftoolz
+* PyPI Distribution: https://pypi.python.org/pypi/vcftoolz
+
+
+Features
+--------
+
+* Compares the snps in two or more VCF files.
+* Lists the snps that are unique to each VCF file with full genotype information per snp.
+* Lists the snps that are missing from each VCF file if present in at least two other VCF files.
+* Generates Venn diagrams of positions and snps in the VCF files.
+* Reports precision, recall, and F1 score when the truth is known.
+* Reports the effectiveness of filtered variants when the truth is known.
+* Reformat the VCF file in a tall-narrow format for easy viewing and diffs.
+* Count samples, positions, calls, snps, indels, other variants, missing calls, and filter reasons.
+* Plot calls along the length of the genome and show the location of filtered calls.
+
+
+Citing VCF Toolz
+--------------------------------------
+
+To cite VCF Toolz, please reference the VCF Toolz paper:
+
+    https://doi.org/10.21105/joss.01144
+
+
+License
+-------
+
+See the LICENSE file included in the VCF Toolz distribution.
+
+
+
+
+
+History
+=======
+
+1.2.0 (2019-04-04)
+---------------------
+* Fix defect in narrow command wrongly printing ALT=. when GT=.
+* Add the ``count`` command to count samples, positions, calls, snps, indels,
+  other variants, filtered calls, missing calls, and filter reasons.
+* Add the ``plot`` command to plot calls along the length of the genome and show
+  the location of filtered calls.
+* Change the text of the compare report to refer to "Calls", not "Sample snps".
+* Drop support for Python 3.4, which is not supported by matplotlib.
+* Add support for Python 3.7.
+
+1.1.1 (2019-03-26)
+---------------------
+* Replace None with '.' when printing call data.
+* Support VCF files with multiple alternate alleles per position.
+
+1.1.0 (2019-02-06)
+---------------------
+* Support reading gzip compressed vcf files.
+
+
+1.0.0 (2018-11-20)
+---------------------
+
+* First public release.
+
+
```

