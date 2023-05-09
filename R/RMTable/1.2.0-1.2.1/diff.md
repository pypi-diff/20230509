# Comparing `tmp/RMTable-1.2.0.tar.gz` & `tmp/RMTable-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/RMTable-1.2.0.tar", last modified: Thu May  4 09:01:00 2023, max compression
+gzip compressed data, was "dist/RMTable-1.2.1.tar", last modified: Tue May  9 00:50:04 2023, max compression
```

## Comparing `RMTable-1.2.0.tar` & `RMTable-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-05-04 09:01:00.443506 RMTable-1.2.0/
--rw-r--r--   0 cvaneck    (503) staff       (20)     1072 2019-04-22 15:49:25.000000 RMTable-1.2.0/LICENSE
--rw-r--r--   0 cvaneck    (503) staff       (20)     5151 2023-05-04 09:01:00.443159 RMTable-1.2.0/PKG-INFO
--rw-r--r--   0 cvaneck    (503) staff       (20)     4421 2022-07-26 14:25:27.000000 RMTable-1.2.0/README.md
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-05-04 09:01:00.428815 RMTable-1.2.0/RMTable.egg-info/
--rw-r--r--   0 cvaneck    (503) staff       (20)     5151 2023-05-04 09:01:00.000000 RMTable-1.2.0/RMTable.egg-info/PKG-INFO
--rw-r--r--   0 cvaneck    (503) staff       (20)      442 2023-05-04 09:01:00.000000 RMTable-1.2.0/RMTable.egg-info/SOURCES.txt
--rw-r--r--   0 cvaneck    (503) staff       (20)        1 2023-05-04 09:01:00.000000 RMTable-1.2.0/RMTable.egg-info/dependency_links.txt
--rw-r--r--   0 cvaneck    (503) staff       (20)       14 2023-05-04 09:01:00.000000 RMTable-1.2.0/RMTable.egg-info/requires.txt
--rw-r--r--   0 cvaneck    (503) staff       (20)        8 2023-05-04 09:01:00.000000 RMTable-1.2.0/RMTable.egg-info/top_level.txt
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-05-04 09:01:00.442377 RMTable-1.2.0/rmtable/
--rw-r--r--   0 cvaneck    (503) staff       (20)       22 2022-05-27 14:57:42.000000 RMTable-1.2.0/rmtable/__init__.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    13769 2023-05-04 00:13:29.000000 RMTable-1.2.0/rmtable/column_standard_v1.3.json
--rw-r--r--   0 cvaneck    (503) staff       (20)     1748 2023-05-04 00:13:48.000000 RMTable-1.2.0/rmtable/entries_standard_v1.3.json
--rw-r--r--   0 cvaneck    (503) staff       (20)    25444 2023-03-20 05:27:35.000000 RMTable-1.2.0/rmtable/rmtable.py
--rw-r--r--   0 cvaneck    (503) staff       (20)       38 2023-05-04 09:01:00.443567 RMTable-1.2.0/setup.cfg
--rw-r--r--   0 cvaneck    (503) staff       (20)     1548 2023-05-03 23:14:10.000000 RMTable-1.2.0/setup.py
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-05-09 00:50:04.847907 RMTable-1.2.1/
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1072 2019-04-22 15:49:25.000000 RMTable-1.2.1/LICENSE
+-rw-r--r--   0 cvaneck    (503) staff       (20)     4969 2023-05-09 00:50:04.847464 RMTable-1.2.1/PKG-INFO
+-rw-r--r--   0 cvaneck    (503) staff       (20)     4239 2023-05-04 09:02:12.000000 RMTable-1.2.1/README.md
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-05-09 00:50:04.833578 RMTable-1.2.1/RMTable.egg-info/
+-rw-r--r--   0 cvaneck    (503) staff       (20)     4969 2023-05-09 00:50:04.000000 RMTable-1.2.1/RMTable.egg-info/PKG-INFO
+-rw-r--r--   0 cvaneck    (503) staff       (20)      442 2023-05-09 00:50:04.000000 RMTable-1.2.1/RMTable.egg-info/SOURCES.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)        1 2023-05-09 00:50:04.000000 RMTable-1.2.1/RMTable.egg-info/dependency_links.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)       14 2023-05-09 00:50:04.000000 RMTable-1.2.1/RMTable.egg-info/requires.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)        8 2023-05-09 00:50:04.000000 RMTable-1.2.1/RMTable.egg-info/top_level.txt
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-05-09 00:50:04.846318 RMTable-1.2.1/rmtable/
+-rw-r--r--   0 cvaneck    (503) staff       (20)       22 2022-05-27 14:57:42.000000 RMTable-1.2.1/rmtable/__init__.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)    13682 2023-05-09 00:40:59.000000 RMTable-1.2.1/rmtable/column_standard_v1.3.json
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1664 2023-05-09 00:47:13.000000 RMTable-1.2.1/rmtable/entries_standard_v1.3.json
+-rw-r--r--   0 cvaneck    (503) staff       (20)    25444 2023-03-20 05:27:35.000000 RMTable-1.2.1/rmtable/rmtable.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)       38 2023-05-09 00:50:04.847980 RMTable-1.2.1/setup.cfg
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1548 2023-05-09 00:48:35.000000 RMTable-1.2.1/setup.py
```

### Comparing `RMTable-1.2.0/LICENSE` & `RMTable-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RMTable-1.2.0/PKG-INFO` & `RMTable-1.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RMTable
-Version: 1.2.0
+Version: 1.2.1
 Summary: Reading, writing, and manipulating RMTables (radio astronomy Faraday rotation catalogs)
 Home-page: https://github.com/CIRADA-Tools/RMTable
 Maintainer: Cameron Van Eck
 Maintainer-email: cameron.van.eck@utoronto.ca
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,15 @@
 
 ### [Documentation](https://github.com/CIRADA-Tools/RMTable/wiki)
 Detailed documentation, including installation instructions and example code, is available on the wiki linked above.  
 
 ***
 
 The paper describing the RMTable standard and the consolidated catalog is currently being refereed. The current draft, with a description of the RMTable standard, can be found [here](https://www.dropbox.com/s/ebdnhad8vypx4cc/RMTable.pdf?dl=0).  
-If that link dies, a slightly older working document for the RM Standard definition is [here](https://docs.google.com/document/d/1lo-W89G1X7xGoMOPHYS5japxJKPDamjEJ9uIGnRPnpo/edit).
+
 
 The main code is in rmtable.py, which contains the class definition for an 
 RMTable, which contains all the columns in the RM Standard and automatically
 fills in blank columns with default values.
 
 Some code demonstrating the use of RMTables can be found in examples.py.
 
@@ -43,25 +43,25 @@
 
 
 
 ***
 
 ### Catalog
 
-The consolidated catalog, which currently contains 55 819 RMs from 42 catalogs, is available in the consolidated_catalog_* files above or these links: [FITS format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.0.1.fits.zip) [TSV format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.0.1.tsv.zip) and [VOTable format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.0.1.xml.zip)  
+The consolidated catalog, which currently contains 55 819 RMs from 42 catalogs, is available in the consolidated_catalog_* files above or these links: [FITS format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.1.0.fits.zip) [TSV format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.1.0.tsv.zip) and [VOTable format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.1.0.xml.zip)  
 This catalog is provided on an as-is basis; there may be uncaught transcription errors in adapting the published catalogs into the RMTable catalog format. It's also known that some of the published values/sources are unphysical (negative Stokes I, fractional polarizations outside of \[0,1), unrealistic spectral indices, etc). Users should use their discretion when selecting sources in the catalog to use. Please see Section 3.2 of the [paper](https://www.dropbox.com/s/ebdnhad8vypx4cc/RMTable.pdf?dl=0) for more suggestions on catalog usage.
 
-The DOI for the current version of the catalog (ver1.0.1) is [10.5281/zenodo.6907975](https://zenodo.org/record/6907975/). The DOI for all versions of the catalog is [10.5281/zenodo.6702842](https://zenodo.org/record/6702842).
+The DOI for the current version of the catalog (ver1.1.0) is [10.5281/zenodo.7894467](https://zenodo.org/record/7894467/). The DOI for all versions of the catalog is [10.5281/zenodo.6702842](https://zenodo.org/record/6702842).
 
 
 The list of individual catalogs/papers that have been incorporated into the consolidated catalog, with some notes on how they were adapted, can be found [here](https://github.com/CIRADA-Tools/RMTable/raw/master/docs/Catalog_notes.pdf).
 
 ***
 
 ### Suggestions for catalog authors (or those converting older catalogs)
 Given the large number of columns in the standard, it may seem to potential RM catalog authors that the process of generating a catalog in RMTable format could be more effort than is merited. The majority of the columns defined in the standard are optional and can be omitted or left blank without creating problems, although every column that is included increases the value of the catalog to future users. The key minimum elements that must be adhered to follow the RMTable standard are twofold: first, the standard columns that **are** included must use the naming convention and units of the standard (to avoid users being unable to combine catalogs, or combining catalogs with inconsistent units); second, any columns added that are outside the RMTable standard must not have a name conflict with any of the defined standard columns (e.g., a column labelled ``b'' would conflict with the Galactic Latitude column in RMTable). As long as those two conditions are satisfied, catalog authors have the freedom to choose how much effort they invest into including more of the standard columns. Using this package will automatically ensure both conditions are satisfied.
 
 
 Conversions of new catalogs into the RMTable format for inclusion into the consolidated catalog are very welcome. If you are interested in contributing a catalog to the consolidated catalog, or find any errors with the catalogs already included, please contact me.
 
-Cameron Van Eck (cameron.van.eck (at) utoronto.ca)
+Cameron Van Eck (cameron.vaneck (at) anu.edu.au)
```

### Comparing `RMTable-1.2.0/README.md` & `RMTable-1.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 ### [Documentation](https://github.com/CIRADA-Tools/RMTable/wiki)
 Detailed documentation, including installation instructions and example code, is available on the wiki linked above.  
 
 ***
 
 The paper describing the RMTable standard and the consolidated catalog is currently being refereed. The current draft, with a description of the RMTable standard, can be found [here](https://www.dropbox.com/s/ebdnhad8vypx4cc/RMTable.pdf?dl=0).  
-If that link dies, a slightly older working document for the RM Standard definition is [here](https://docs.google.com/document/d/1lo-W89G1X7xGoMOPHYS5japxJKPDamjEJ9uIGnRPnpo/edit).
+
 
 The main code is in rmtable.py, which contains the class definition for an 
 RMTable, which contains all the columns in the RM Standard and automatically
 fills in blank columns with default values.
 
 Some code demonstrating the use of RMTables can be found in examples.py.
 
@@ -23,25 +23,25 @@
 
 
 
 ***
 
 ### Catalog
 
-The consolidated catalog, which currently contains 55 819 RMs from 42 catalogs, is available in the consolidated_catalog_* files above or these links: [FITS format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.0.1.fits.zip) [TSV format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.0.1.tsv.zip) and [VOTable format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.0.1.xml.zip)  
+The consolidated catalog, which currently contains 55 819 RMs from 42 catalogs, is available in the consolidated_catalog_* files above or these links: [FITS format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.1.0.fits.zip) [TSV format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.1.0.tsv.zip) and [VOTable format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.1.0.xml.zip)  
 This catalog is provided on an as-is basis; there may be uncaught transcription errors in adapting the published catalogs into the RMTable catalog format. It's also known that some of the published values/sources are unphysical (negative Stokes I, fractional polarizations outside of \[0,1), unrealistic spectral indices, etc). Users should use their discretion when selecting sources in the catalog to use. Please see Section 3.2 of the [paper](https://www.dropbox.com/s/ebdnhad8vypx4cc/RMTable.pdf?dl=0) for more suggestions on catalog usage.
 
-The DOI for the current version of the catalog (ver1.0.1) is [10.5281/zenodo.6907975](https://zenodo.org/record/6907975/). The DOI for all versions of the catalog is [10.5281/zenodo.6702842](https://zenodo.org/record/6702842).
+The DOI for the current version of the catalog (ver1.1.0) is [10.5281/zenodo.7894467](https://zenodo.org/record/7894467/). The DOI for all versions of the catalog is [10.5281/zenodo.6702842](https://zenodo.org/record/6702842).
 
 
 The list of individual catalogs/papers that have been incorporated into the consolidated catalog, with some notes on how they were adapted, can be found [here](https://github.com/CIRADA-Tools/RMTable/raw/master/docs/Catalog_notes.pdf).
 
 ***
 
 ### Suggestions for catalog authors (or those converting older catalogs)
 Given the large number of columns in the standard, it may seem to potential RM catalog authors that the process of generating a catalog in RMTable format could be more effort than is merited. The majority of the columns defined in the standard are optional and can be omitted or left blank without creating problems, although every column that is included increases the value of the catalog to future users. The key minimum elements that must be adhered to follow the RMTable standard are twofold: first, the standard columns that **are** included must use the naming convention and units of the standard (to avoid users being unable to combine catalogs, or combining catalogs with inconsistent units); second, any columns added that are outside the RMTable standard must not have a name conflict with any of the defined standard columns (e.g., a column labelled ``b'' would conflict with the Galactic Latitude column in RMTable). As long as those two conditions are satisfied, catalog authors have the freedom to choose how much effort they invest into including more of the standard columns. Using this package will automatically ensure both conditions are satisfied.
 
 
 Conversions of new catalogs into the RMTable format for inclusion into the consolidated catalog are very welcome. If you are interested in contributing a catalog to the consolidated catalog, or find any errors with the catalogs already included, please contact me.
 
-Cameron Van Eck (cameron.van.eck (at) utoronto.ca)
+Cameron Van Eck (cameron.vaneck (at) anu.edu.au)
```

### Comparing `RMTable-1.2.0/RMTable.egg-info/PKG-INFO` & `RMTable-1.2.1/RMTable.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RMTable
-Version: 1.2.0
+Version: 1.2.1
 Summary: Reading, writing, and manipulating RMTables (radio astronomy Faraday rotation catalogs)
 Home-page: https://github.com/CIRADA-Tools/RMTable
 Maintainer: Cameron Van Eck
 Maintainer-email: cameron.van.eck@utoronto.ca
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,15 @@
 
 ### [Documentation](https://github.com/CIRADA-Tools/RMTable/wiki)
 Detailed documentation, including installation instructions and example code, is available on the wiki linked above.  
 
 ***
 
 The paper describing the RMTable standard and the consolidated catalog is currently being refereed. The current draft, with a description of the RMTable standard, can be found [here](https://www.dropbox.com/s/ebdnhad8vypx4cc/RMTable.pdf?dl=0).  
-If that link dies, a slightly older working document for the RM Standard definition is [here](https://docs.google.com/document/d/1lo-W89G1X7xGoMOPHYS5japxJKPDamjEJ9uIGnRPnpo/edit).
+
 
 The main code is in rmtable.py, which contains the class definition for an 
 RMTable, which contains all the columns in the RM Standard and automatically
 fills in blank columns with default values.
 
 Some code demonstrating the use of RMTables can be found in examples.py.
 
@@ -43,25 +43,25 @@
 
 
 
 ***
 
 ### Catalog
 
-The consolidated catalog, which currently contains 55 819 RMs from 42 catalogs, is available in the consolidated_catalog_* files above or these links: [FITS format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.0.1.fits.zip) [TSV format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.0.1.tsv.zip) and [VOTable format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.0.1.xml.zip)  
+The consolidated catalog, which currently contains 55 819 RMs from 42 catalogs, is available in the consolidated_catalog_* files above or these links: [FITS format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.1.0.fits.zip) [TSV format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.1.0.tsv.zip) and [VOTable format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.1.0.xml.zip)  
 This catalog is provided on an as-is basis; there may be uncaught transcription errors in adapting the published catalogs into the RMTable catalog format. It's also known that some of the published values/sources are unphysical (negative Stokes I, fractional polarizations outside of \[0,1), unrealistic spectral indices, etc). Users should use their discretion when selecting sources in the catalog to use. Please see Section 3.2 of the [paper](https://www.dropbox.com/s/ebdnhad8vypx4cc/RMTable.pdf?dl=0) for more suggestions on catalog usage.
 
-The DOI for the current version of the catalog (ver1.0.1) is [10.5281/zenodo.6907975](https://zenodo.org/record/6907975/). The DOI for all versions of the catalog is [10.5281/zenodo.6702842](https://zenodo.org/record/6702842).
+The DOI for the current version of the catalog (ver1.1.0) is [10.5281/zenodo.7894467](https://zenodo.org/record/7894467/). The DOI for all versions of the catalog is [10.5281/zenodo.6702842](https://zenodo.org/record/6702842).
 
 
 The list of individual catalogs/papers that have been incorporated into the consolidated catalog, with some notes on how they were adapted, can be found [here](https://github.com/CIRADA-Tools/RMTable/raw/master/docs/Catalog_notes.pdf).
 
 ***
 
 ### Suggestions for catalog authors (or those converting older catalogs)
 Given the large number of columns in the standard, it may seem to potential RM catalog authors that the process of generating a catalog in RMTable format could be more effort than is merited. The majority of the columns defined in the standard are optional and can be omitted or left blank without creating problems, although every column that is included increases the value of the catalog to future users. The key minimum elements that must be adhered to follow the RMTable standard are twofold: first, the standard columns that **are** included must use the naming convention and units of the standard (to avoid users being unable to combine catalogs, or combining catalogs with inconsistent units); second, any columns added that are outside the RMTable standard must not have a name conflict with any of the defined standard columns (e.g., a column labelled ``b'' would conflict with the Galactic Latitude column in RMTable). As long as those two conditions are satisfied, catalog authors have the freedom to choose how much effort they invest into including more of the standard columns. Using this package will automatically ensure both conditions are satisfied.
 
 
 Conversions of new catalogs into the RMTable format for inclusion into the consolidated catalog are very welcome. If you are interested in contributing a catalog to the consolidated catalog, or find any errors with the catalogs already included, please contact me.
 
-Cameron Van Eck (cameron.van.eck (at) utoronto.ca)
+Cameron Van Eck (cameron.vaneck (at) anu.edu.au)
```

### Comparing `RMTable-1.2.0/rmtable/column_standard_v1.3.json` & `RMTable-1.2.1/rmtable/column_standard_v1.3.json`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#Note that any changes to this file should be reflected in the documentation as well.
-
 {
     "ra": {
         "dtype": "f8",
         "limits": [
             0,
             360
         ],
```

### Comparing `RMTable-1.2.0/rmtable/entries_standard_v1.3.json` & `RMTable-1.2.1/rmtable/entries_standard_v1.3.json`

 * *Files 10% similar despite different names*

```diff
@@ -1,110 +1,104 @@
-00000000: 234e 6f74 6520 7468 6174 2061 6e79 2075  #Note that any u
-00000010: 7064 6174 6573 2074 6f20 7468 6973 2066  pdates to this f
-00000020: 696c 6520 7368 6f75 6c64 2061 6c73 6f20  ile should also 
-00000030: 6265 2072 6566 6c65 6374 6564 2069 6e20  be reflected in 
-00000040: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
-00000050: 6e2e 0a0a 7b0a 2020 2020 2272 6d5f 6d65  n...{.    "rm_me
-00000060: 7468 6f64 223a 205b 0a20 2020 2020 2020  thod": [.       
-00000070: 2022 4556 5041 2d6c 696e 6561 7220 6669   "EVPA-linear fi
-00000080: 7422 2c0a 2020 2020 2020 2020 2252 4d20  t",.        "RM 
-00000090: 5379 6e74 6865 7369 7320 2d20 506f 6c2e  Synthesis - Pol.
-000000a0: 2049 6e74 222c 0a20 2020 2020 2020 2022   Int",.        "
-000000b0: 524d 2053 796e 7468 6573 6973 202d 2046  RM Synthesis - F
-000000c0: 7261 6374 696f 6e61 6c20 706f 6c61 7269  ractional polari
-000000d0: 7a61 7469 6f6e 222c 0a20 2020 2020 2020  zation",.       
-000000e0: 2022 524d 2053 796e 7468 6573 6973 222c   "RM Synthesis",
-000000f0: 0a20 2020 2020 2020 2022 4661 7261 6461  .        "Farada
-00000100: 7920 5379 6e74 6865 7369 7322 2c0a 2020  y Synthesis",.  
-00000110: 2020 2020 2020 2251 5566 6974 222c 0a20        "QUfit",. 
-00000120: 2020 2020 2020 2022 5155 6669 7420 2d20         "QUfit - 
-00000130: 4465 6c74 6120 6675 6e63 7469 6f6e 222c  Delta function",
-00000140: 0a20 2020 2020 2020 2022 5155 6669 7420  .        "QUfit 
-00000150: 2d20 4761 7573 7369 616e 2078 2042 7572  - Gaussian x Bur
-00000160: 6e20 536c 6162 222c 0a20 2020 2020 2020  n Slab",.       
-00000170: 2022 5155 6669 7420 2d20 4275 726e 2073   "QUfit - Burn s
-00000180: 6c61 6222 2c0a 2020 2020 2020 2020 2251  lab",.        "Q
-00000190: 5566 6974 202d 2047 6175 7373 6961 6e22  Ufit - Gaussian"
-000001a0: 2c0a 2020 2020 2020 2020 2251 5566 6974  ,.        "QUfit
-000001b0: 202d 204d 756c 7469 706c 6522 2c0a 2020   - Multiple",.  
-000001c0: 2020 2020 2020 2255 6e6b 6e6f 776e 220a        "Unknown".
-000001d0: 2020 2020 5d2c 0a20 2020 2022 706f 6c5f      ],.    "pol_
-000001e0: 6269 6173 223a 205b 0a20 2020 2020 2020  bias": [.       
-000001f0: 2022 3139 3734 4170 4a2e 2e2e 3139 342e   "1974ApJ...194.
-00000200: 2e32 3439 5722 2c0a 2020 2020 2020 2020  .249W",.        
-00000210: 2231 3938 3541 2641 2e2e 2e31 3432 2e2e  "1985A&A...142..
-00000220: 3130 3053 222c 0a20 2020 2020 2020 2022  100S",.        "
-00000230: 3230 3132 5041 5341 2e2e 2e32 392e 2e32  2012PASA...29..2
-00000240: 3134 4722 2c0a 2020 2020 2020 2020 2231  14G",.        "1
-00000250: 3938 3641 704a 2e2e 2e33 3032 2e2e 3330  986ApJ...302..30
-00000260: 364b 222c 0a20 2020 2020 2020 2022 556e  6K",.        "Un
-00000270: 6b6e 6f77 6e22 2c0a 2020 2020 2020 2020  known",.        
-00000280: 224e 6f6e 6522 2c0a 2020 2020 2020 2020  "None",.        
-00000290: 224e 6f74 2064 6573 6372 6962 6564 220a  "Not described".
-000002a0: 2020 2020 5d2c 0a20 2020 2022 7465 6c65      ],.    "tele
-000002b0: 7363 6f70 6522 3a20 5b0a 2020 2020 2020  scope": [.      
-000002c0: 2020 2256 4c41 222c 0a20 2020 2020 2020    "VLA",.       
-000002d0: 2022 4c4f 4641 5222 2c0a 2020 2020 2020   "LOFAR",.      
-000002e0: 2020 2241 5443 4122 2c0a 2020 2020 2020    "ATCA",.      
-000002f0: 2020 2244 5241 4f2d 5354 222c 0a20 2020    "DRAO-ST",.   
-00000300: 2020 2020 2022 4d57 4122 2c0a 2020 2020       "MWA",.    
-00000310: 2020 2020 2257 5352 5422 2c0a 2020 2020      "WSRT",.    
-00000320: 2020 2020 2245 6666 656c 7362 6572 6722      "Effelsberg"
-00000330: 2c0a 2020 2020 2020 2020 2241 5441 222c  ,.        "ATA",
-00000340: 0a20 2020 2020 2020 2022 4153 4b41 5022  .        "ASKAP"
-00000350: 2c0a 2020 2020 2020 2020 2241 524f 222c  ,.        "ARO",
-00000360: 0a20 2020 2020 2020 2022 4172 6563 6962  .        "Arecib
-00000370: 6f22 2c0a 2020 2020 2020 2020 2250 6172  o",.        "Par
-00000380: 6b65 7322 2c0a 2020 2020 2020 2020 2243  kes",.        "C
-00000390: 4849 4d45 222c 0a20 2020 2020 2020 2022  HIME",.        "
-000003a0: 4641 5354 222c 0a20 2020 2020 2020 2022  FAST",.        "
-000003b0: 556e 6b6e 6f77 6e22 0a20 2020 205d 2c0a  Unknown".    ],.
-000003c0: 2020 2020 2263 6c61 7373 6966 6963 6174      "classificat
-000003d0: 696f 6e22 3a20 5b0a 2020 2020 2020 2020  ion": [.        
-000003e0: 2222 2c0a 2020 2020 2020 2020 2250 756c  "",.        "Pul
-000003f0: 7361 7222 2c0a 2020 2020 2020 2020 2246  sar",.        "F
-00000400: 5249 4920 686f 7473 706f 7422 2c0a 2020  RII hotspot",.  
-00000410: 2020 2020 2020 2241 474e 222c 0a20 2020        "AGN",.   
-00000420: 2020 2020 2022 5261 6469 6f20 6761 6c61       "Radio gala
-00000430: 7879 222c 0a20 2020 2020 2020 2022 4869  xy",.        "Hi
-00000440: 6768 2d72 6564 7368 6966 7420 7261 6469  gh-redshift radi
-00000450: 6f20 6761 6c61 7879 222c 0a20 2020 2020  o galaxy",.     
-00000460: 2020 2022 4652 4222 2c0a 2020 2020 2020     "FRB",.      
-00000470: 2020 2255 6e6b 6e6f 776e 220a 2020 2020    "Unknown".    
-00000480: 5d2c 0a20 2020 2022 666c 7578 5f74 7970  ],.    "flux_typ
-00000490: 6522 3a20 5b0a 2020 2020 2020 2020 2255  e": [.        "U
-000004a0: 6e6b 6e6f 776e 222c 0a20 2020 2020 2020  nknown",.       
-000004b0: 2022 496e 7465 6772 6174 6564 222c 0a20   "Integrated",. 
-000004c0: 2020 2020 2020 2022 5065 616b 222c 0a20         "Peak",. 
-000004d0: 2020 2020 2020 2022 426f 7822 2c0a 2020         "Box",.  
-000004e0: 2020 2020 2020 2256 6973 6962 696c 6974        "Visibilit
-000004f0: 6965 7322 2c0a 2020 2020 2020 2020 2247  ies",.        "G
-00000500: 6175 7373 6961 6e20 6669 7420 2d20 5065  aussian fit - Pe
-00000510: 616b 220a 2020 2020 5d2c 0a20 2020 2022  ak".    ],.    "
-00000520: 636f 6d70 6c65 7869 7479 5f74 6573 7422  complexity_test"
-00000530: 3a20 5b0a 2020 2020 2020 2020 2222 2c0a  : [.        "",.
-00000540: 2020 2020 2020 2020 224e 6f6e 6522 2c0a          "None",.
-00000550: 2020 2020 2020 2020 2253 6967 6d61 5f61          "Sigma_a
-00000560: 6464 222c 0a20 2020 2020 2020 2022 5365  dd",.        "Se
-00000570: 636f 6e64 206d 6f6d 656e 7422 2c0a 2020  cond moment",.  
-00000580: 2020 2020 2020 2251 552d 6669 7474 696e        "QU-fittin
-00000590: 6722 2c0a 2020 2020 2020 2020 2249 6e73  g",.        "Ins
-000005a0: 7065 6374 696f 6e22 2c0a 2020 2020 2020  pection",.      
-000005b0: 2020 224d 6163 6869 6e65 206c 6561 726e    "Machine learn
-000005c0: 696e 6720 2d20 416c 6765 7220 3230 3231  ing - Alger 2021
-000005d0: 222c 0a20 2020 2020 2020 2022 436f 6e76  ",.        "Conv
-000005e0: 6f6c 7574 696f 6e61 6c20 6e65 7572 616c  olutional neural
-000005f0: 206e 6574 776f 726b 7320 2d20 4272 6f77   networks - Brow
-00000600: 6e20 3230 3139 222c 0a20 2020 2020 2020  n 2019",.       
-00000610: 2022 5155 2d66 6974 2026 2042 4943 220a   "QU-fit & BIC".
-00000620: 2020 2020 5d2c 0a20 2020 2022 696f 6e6f      ],.    "iono
-00000630: 7370 6865 7265 223a 205b 0a20 2020 2020  sphere": [.     
-00000640: 2020 2022 556e 6b6e 6f77 6e22 2c0a 2020     "Unknown",.  
-00000650: 2020 2020 2020 224e 6f6e 6522 2c0a 2020        "None",.  
-00000660: 2020 2020 2020 2252 4d65 7874 7261 6374        "RMextract
-00000670: 222c 0a20 2020 2020 2020 2022 696f 6e46  ",.        "ionF
-00000680: 5222 2c0a 2020 2020 2020 2020 2246 4152  R",.        "FAR
-00000690: 4144 222c 0a20 2020 2020 2020 2022 414c  AD",.        "AL
-000006a0: 4255 5322 2c0a 2020 2020 2020 2020 2246  BUS",.        "F
-000006b0: 5269 6f6e 220a 2020 2020 5d2c 0a20 2020  Rion".    ],.   
-000006c0: 2022 7665 7273 696f 6e22 3a20 2231 2e33   "version": "1.3
-000006d0: 220a 7d0a                                ".}.
+00000000: 7b0a 2020 2020 2272 6d5f 6d65 7468 6f64  {.    "rm_method
+00000010: 223a 205b 0a20 2020 2020 2020 2022 4556  ": [.        "EV
+00000020: 5041 2d6c 696e 6561 7220 6669 7422 2c0a  PA-linear fit",.
+00000030: 2020 2020 2020 2020 2252 4d20 5379 6e74          "RM Synt
+00000040: 6865 7369 7320 2d20 506f 6c2e 2049 6e74  hesis - Pol. Int
+00000050: 222c 0a20 2020 2020 2020 2022 524d 2053  ",.        "RM S
+00000060: 796e 7468 6573 6973 202d 2046 7261 6374  ynthesis - Fract
+00000070: 696f 6e61 6c20 706f 6c61 7269 7a61 7469  ional polarizati
+00000080: 6f6e 222c 0a20 2020 2020 2020 2022 524d  on",.        "RM
+00000090: 2053 796e 7468 6573 6973 222c 0a20 2020   Synthesis",.   
+000000a0: 2020 2020 2022 4661 7261 6461 7920 5379       "Faraday Sy
+000000b0: 6e74 6865 7369 7322 2c0a 2020 2020 2020  nthesis",.      
+000000c0: 2020 2251 5566 6974 222c 0a20 2020 2020    "QUfit",.     
+000000d0: 2020 2022 5155 6669 7420 2d20 4465 6c74     "QUfit - Delt
+000000e0: 6120 6675 6e63 7469 6f6e 222c 0a20 2020  a function",.   
+000000f0: 2020 2020 2022 5155 6669 7420 2d20 4761       "QUfit - Ga
+00000100: 7573 7369 616e 2078 2042 7572 6e20 536c  ussian x Burn Sl
+00000110: 6162 222c 0a20 2020 2020 2020 2022 5155  ab",.        "QU
+00000120: 6669 7420 2d20 4275 726e 2073 6c61 6222  fit - Burn slab"
+00000130: 2c0a 2020 2020 2020 2020 2251 5566 6974  ,.        "QUfit
+00000140: 202d 2047 6175 7373 6961 6e22 2c0a 2020   - Gaussian",.  
+00000150: 2020 2020 2020 2251 5566 6974 202d 204d        "QUfit - M
+00000160: 756c 7469 706c 6522 2c0a 2020 2020 2020  ultiple",.      
+00000170: 2020 2255 6e6b 6e6f 776e 220a 2020 2020    "Unknown".    
+00000180: 5d2c 0a20 2020 2022 706f 6c5f 6269 6173  ],.    "pol_bias
+00000190: 223a 205b 0a20 2020 2020 2020 2022 3139  ": [.        "19
+000001a0: 3734 4170 4a2e 2e2e 3139 342e 2e32 3439  74ApJ...194..249
+000001b0: 5722 2c0a 2020 2020 2020 2020 2231 3938  W",.        "198
+000001c0: 3541 2641 2e2e 2e31 3432 2e2e 3130 3053  5A&A...142..100S
+000001d0: 222c 0a20 2020 2020 2020 2022 3230 3132  ",.        "2012
+000001e0: 5041 5341 2e2e 2e32 392e 2e32 3134 4722  PASA...29..214G"
+000001f0: 2c0a 2020 2020 2020 2020 2231 3938 3641  ,.        "1986A
+00000200: 704a 2e2e 2e33 3032 2e2e 3330 364b 222c  pJ...302..306K",
+00000210: 0a20 2020 2020 2020 2022 556e 6b6e 6f77  .        "Unknow
+00000220: 6e22 2c0a 2020 2020 2020 2020 224e 6f6e  n",.        "Non
+00000230: 6522 2c0a 2020 2020 2020 2020 224e 6f74  e",.        "Not
+00000240: 2064 6573 6372 6962 6564 220a 2020 2020   described".    
+00000250: 5d2c 0a20 2020 2022 7465 6c65 7363 6f70  ],.    "telescop
+00000260: 6522 3a20 5b0a 2020 2020 2020 2020 2256  e": [.        "V
+00000270: 4c41 222c 0a20 2020 2020 2020 2022 4c4f  LA",.        "LO
+00000280: 4641 5222 2c0a 2020 2020 2020 2020 2241  FAR",.        "A
+00000290: 5443 4122 2c0a 2020 2020 2020 2020 2244  TCA",.        "D
+000002a0: 5241 4f2d 5354 222c 0a20 2020 2020 2020  RAO-ST",.       
+000002b0: 2022 4d57 4122 2c0a 2020 2020 2020 2020   "MWA",.        
+000002c0: 2257 5352 5422 2c0a 2020 2020 2020 2020  "WSRT",.        
+000002d0: 2245 6666 656c 7362 6572 6722 2c0a 2020  "Effelsberg",.  
+000002e0: 2020 2020 2020 2241 5441 222c 0a20 2020        "ATA",.   
+000002f0: 2020 2020 2022 4153 4b41 5022 2c0a 2020       "ASKAP",.  
+00000300: 2020 2020 2020 2241 524f 222c 0a20 2020        "ARO",.   
+00000310: 2020 2020 2022 4172 6563 6962 6f22 2c0a       "Arecibo",.
+00000320: 2020 2020 2020 2020 2250 6172 6b65 7322          "Parkes"
+00000330: 2c0a 2020 2020 2020 2020 2243 4849 4d45  ,.        "CHIME
+00000340: 222c 0a20 2020 2020 2020 2022 4641 5354  ",.        "FAST
+00000350: 222c 0a20 2020 2020 2020 2022 556e 6b6e  ",.        "Unkn
+00000360: 6f77 6e22 0a20 2020 205d 2c0a 2020 2020  own".    ],.    
+00000370: 2263 6c61 7373 6966 6963 6174 696f 6e22  "classification"
+00000380: 3a20 5b0a 2020 2020 2020 2020 2222 2c0a  : [.        "",.
+00000390: 2020 2020 2020 2020 2250 756c 7361 7222          "Pulsar"
+000003a0: 2c0a 2020 2020 2020 2020 2246 5249 4920  ,.        "FRII 
+000003b0: 686f 7473 706f 7422 2c0a 2020 2020 2020  hotspot",.      
+000003c0: 2020 2241 474e 222c 0a20 2020 2020 2020    "AGN",.       
+000003d0: 2022 5261 6469 6f20 6761 6c61 7879 222c   "Radio galaxy",
+000003e0: 0a20 2020 2020 2020 2022 4869 6768 2d72  .        "High-r
+000003f0: 6564 7368 6966 7420 7261 6469 6f20 6761  edshift radio ga
+00000400: 6c61 7879 222c 0a20 2020 2020 2020 2022  laxy",.        "
+00000410: 4652 4222 2c0a 2020 2020 2020 2020 2255  FRB",.        "U
+00000420: 6e6b 6e6f 776e 220a 2020 2020 5d2c 0a20  nknown".    ],. 
+00000430: 2020 2022 666c 7578 5f74 7970 6522 3a20     "flux_type": 
+00000440: 5b0a 2020 2020 2020 2020 2255 6e6b 6e6f  [.        "Unkno
+00000450: 776e 222c 0a20 2020 2020 2020 2022 496e  wn",.        "In
+00000460: 7465 6772 6174 6564 222c 0a20 2020 2020  tegrated",.     
+00000470: 2020 2022 5065 616b 222c 0a20 2020 2020     "Peak",.     
+00000480: 2020 2022 426f 7822 2c0a 2020 2020 2020     "Box",.      
+00000490: 2020 2256 6973 6962 696c 6974 6965 7322    "Visibilities"
+000004a0: 2c0a 2020 2020 2020 2020 2247 6175 7373  ,.        "Gauss
+000004b0: 6961 6e20 6669 7420 2d20 5065 616b 220a  ian fit - Peak".
+000004c0: 2020 2020 5d2c 0a20 2020 2022 636f 6d70      ],.    "comp
+000004d0: 6c65 7869 7479 5f74 6573 7422 3a20 5b0a  lexity_test": [.
+000004e0: 2020 2020 2020 2020 2222 2c0a 2020 2020          "",.    
+000004f0: 2020 2020 224e 6f6e 6522 2c0a 2020 2020      "None",.    
+00000500: 2020 2020 2253 6967 6d61 5f61 6464 222c      "Sigma_add",
+00000510: 0a20 2020 2020 2020 2022 5365 636f 6e64  .        "Second
+00000520: 206d 6f6d 656e 7422 2c0a 2020 2020 2020   moment",.      
+00000530: 2020 2251 552d 6669 7474 696e 6722 2c0a    "QU-fitting",.
+00000540: 2020 2020 2020 2020 2249 6e73 7065 6374          "Inspect
+00000550: 696f 6e22 2c0a 2020 2020 2020 2020 224d  ion",.        "M
+00000560: 6163 6869 6e65 206c 6561 726e 696e 6720  achine learning 
+00000570: 2d20 416c 6765 7220 3230 3231 222c 0a20  - Alger 2021",. 
+00000580: 2020 2020 2020 2022 436f 6e76 6f6c 7574         "Convolut
+00000590: 696f 6e61 6c20 6e65 7572 616c 206e 6574  ional neural net
+000005a0: 776f 726b 7320 2d20 4272 6f77 6e20 3230  works - Brown 20
+000005b0: 3139 222c 0a20 2020 2020 2020 2022 5155  19",.        "QU
+000005c0: 2d66 6974 2026 2042 4943 220a 2020 2020  -fit & BIC".    
+000005d0: 5d2c 0a20 2020 2022 696f 6e6f 7370 6865  ],.    "ionosphe
+000005e0: 7265 223a 205b 0a20 2020 2020 2020 2022  re": [.        "
+000005f0: 556e 6b6e 6f77 6e22 2c0a 2020 2020 2020  Unknown",.      
+00000600: 2020 224e 6f6e 6522 2c0a 2020 2020 2020    "None",.      
+00000610: 2020 2252 4d65 7874 7261 6374 222c 0a20    "RMextract",. 
+00000620: 2020 2020 2020 2022 696f 6e46 5222 2c0a         "ionFR",.
+00000630: 2020 2020 2020 2020 2246 4152 4144 222c          "FARAD",
+00000640: 0a20 2020 2020 2020 2022 414c 4255 5322  .        "ALBUS"
+00000650: 2c0a 2020 2020 2020 2020 2246 5269 6f6e  ,.        "FRion
+00000660: 220a 2020 2020 5d2c 0a20 2020 2022 7665  ".    ],.    "ve
+00000670: 7273 696f 6e22 3a20 2231 2e33 220a 7d0a  rsion": "1.3".}.
```

### Comparing `RMTable-1.2.0/rmtable/rmtable.py` & `RMTable-1.2.1/rmtable/rmtable.py`

 * *Files identical despite different names*

### Comparing `RMTable-1.2.0/setup.py` & `RMTable-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from setuptools import find_packages, setup, Command
 
 NAME = 'RMTable'
 DESCRIPTION = 'Reading, writing, and manipulating RMTables (radio astronomy Faraday rotation catalogs)'
 URL = 'https://github.com/CIRADA-Tools/RMTable'
 REQUIRES_PYTHON = '>=3.5.0'
-VERSION = '1.2.0'
+VERSION = '1.2.1'
 
 REQUIRED = [
     'numpy', 'astropy',
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
```

