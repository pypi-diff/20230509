# Comparing `tmp/sbmlcore-0.1.4.tar.gz` & `tmp/sbmlcore-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbmlcore-0.1.4.tar", last modified: Mon Jun 20 09:11:04 2022, max compression
+gzip compressed data, was "sbmlcore-0.2.0.tar", last modified: Tue May  9 13:33:56 2023, max compression
```

## Comparing `sbmlcore-0.1.4.tar` & `sbmlcore-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,44 @@
-drwxr-xr-x   0 fowler     (503) staff       (20)        0 2022-06-20 09:11:04.977790 sbmlcore-0.1.4/
--rw-r--r--   0 fowler     (503) staff       (20)     1072 2022-06-20 07:21:53.000000 sbmlcore-0.1.4/LICENSE
--rw-r--r--   0 fowler     (503) staff       (20)     3391 2022-06-20 09:11:04.977849 sbmlcore-0.1.4/PKG-INFO
--rw-r--r--   0 fowler     (503) staff       (20)     2420 2022-06-19 18:23:53.000000 sbmlcore-0.1.4/README.md
--rw-r--r--   0 fowler     (503) staff       (20)      116 2022-06-20 09:02:09.000000 sbmlcore-0.1.4/pyproject.toml
-drwxr-xr-x   0 fowler     (503) staff       (20)        0 2022-06-20 09:11:04.974286 sbmlcore-0.1.4/sbmlcore/
--rw-r--r--   0 fowler     (503) staff       (20)     6118 2022-06-19 18:23:53.000000 sbmlcore-0.1.4/sbmlcore/AminoAcidProperties.py
--rw-r--r--   0 fowler     (503) staff       (20)     3846 2022-06-19 18:23:53.000000 sbmlcore-0.1.4/sbmlcore/DeepDDG.py
--rw-r--r--   0 fowler     (503) staff       (20)    15119 2022-06-19 18:23:53.000000 sbmlcore-0.1.4/sbmlcore/ExternalCode.py
--rw-r--r--   0 fowler     (503) staff       (20)     2346 2022-06-19 18:23:53.000000 sbmlcore-0.1.4/sbmlcore/FeaturesDataFrame.py
--rw-r--r--   0 fowler     (503) staff       (20)     5335 2022-06-19 18:23:53.000000 sbmlcore-0.1.4/sbmlcore/StructuralDistances.py
--rw-r--r--   0 fowler     (503) staff       (20)    17217 2022-06-16 18:46:03.000000 sbmlcore-0.1.4/sbmlcore/TrajectoryDihedrals.py
--rw-r--r--   0 fowler     (503) staff       (20)    10293 2022-06-19 20:13:44.000000 sbmlcore-0.1.4/sbmlcore/TrajectoryDistances.py
--rw-r--r--   0 fowler     (503) staff       (20)      973 2022-06-16 18:46:03.000000 sbmlcore-0.1.4/sbmlcore/__init__.py
-drwxr-xr-x   0 fowler     (503) staff       (20)        0 2022-06-20 09:11:04.975030 sbmlcore-0.1.4/sbmlcore.egg-info/
--rw-r--r--   0 fowler     (503) staff       (20)     3391 2022-06-20 09:11:04.000000 sbmlcore-0.1.4/sbmlcore.egg-info/PKG-INFO
--rw-r--r--   0 fowler     (503) staff       (20)      802 2022-06-20 09:11:04.000000 sbmlcore-0.1.4/sbmlcore.egg-info/SOURCES.txt
--rw-r--r--   0 fowler     (503) staff       (20)        1 2022-06-20 09:11:04.000000 sbmlcore-0.1.4/sbmlcore.egg-info/dependency_links.txt
--rw-r--r--   0 fowler     (503) staff       (20)        1 2022-06-20 09:11:04.000000 sbmlcore-0.1.4/sbmlcore.egg-info/not-zip-safe
--rw-r--r--   0 fowler     (503) staff       (20)       45 2022-06-20 09:11:04.000000 sbmlcore-0.1.4/sbmlcore.egg-info/requires.txt
--rw-r--r--   0 fowler     (503) staff       (20)        9 2022-06-20 09:11:04.000000 sbmlcore-0.1.4/sbmlcore.egg-info/top_level.txt
--rw-r--r--   0 fowler     (503) staff       (20)     1117 2022-06-20 09:11:04.978109 sbmlcore-0.1.4/setup.cfg
-drwxr-xr-x   0 fowler     (503) staff       (20)        0 2022-06-20 09:11:04.977573 sbmlcore-0.1.4/tests/
--rw-r--r--   0 fowler     (503) staff       (20)       26 2022-06-16 18:46:03.000000 sbmlcore-0.1.4/tests/__init__.py
--rw-r--r--   0 fowler     (503) staff       (20)      234 2022-06-16 18:46:03.000000 sbmlcore-0.1.4/tests/test_MDAnalysis.py
--rw-r--r--   0 fowler     (503) staff       (20)      753 2022-06-16 18:46:03.000000 sbmlcore-0.1.4/tests/test_MW.py
--rw-r--r--   0 fowler     (503) staff       (20)      757 2022-06-16 18:46:03.000000 sbmlcore-0.1.4/tests/test_Pi.py
--rw-r--r--   0 fowler     (503) staff       (20)      786 2022-06-16 18:46:03.000000 sbmlcore-0.1.4/tests/test_aminoacidvolumechange.py
--rw-r--r--   0 fowler     (503) staff       (20)     3807 2022-06-16 18:46:03.000000 sbmlcore-0.1.4/tests/test_deep_ddg.py
--rw-r--r--   0 fowler     (503) staff       (20)     1201 2022-06-16 18:46:03.000000 sbmlcore-0.1.4/tests/test_dssp.py
--rw-r--r--   0 fowler     (503) staff       (20)     2412 2022-06-16 18:46:03.000000 sbmlcore-0.1.4/tests/test_freesasa.py
--rw-r--r--   0 fowler     (503) staff       (20)     1617 2022-06-16 18:46:03.000000 sbmlcore-0.1.4/tests/test_hydropathy.py
--rw-r--r--   0 fowler     (503) staff       (20)     1916 2022-06-16 18:46:03.000000 sbmlcore-0.1.4/tests/test_snap2.py
--rw-r--r--   0 fowler     (503) staff       (20)     1056 2022-06-16 18:46:03.000000 sbmlcore-0.1.4/tests/test_stride.py
--rw-r--r--   0 fowler     (503) staff       (20)     3019 2022-06-20 07:01:22.000000 sbmlcore-0.1.4/tests/test_structuraldistances.py
--rw-r--r--   0 fowler     (503) staff       (20)     9419 2022-06-20 06:58:05.000000 sbmlcore-0.1.4/tests/test_trajectorydihedrals.py
--rw-r--r--   0 fowler     (503) staff       (20)     6468 2022-06-20 06:44:06.000000 sbmlcore-0.1.4/tests/test_trajectorydistances.py
+drwxr-xr-x   0 fowler     (503) staff       (20)        0 2023-05-09 13:33:56.780476 sbmlcore-0.2.0/
+-rw-r--r--   0 fowler     (503) staff       (20)     1072 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/LICENSE
+-rw-r--r--   0 fowler     (503) staff       (20)     3911 2023-05-09 13:33:56.780562 sbmlcore-0.2.0/PKG-INFO
+-rw-r--r--   0 fowler     (503) staff       (20)     2939 2023-05-09 13:13:03.000000 sbmlcore-0.2.0/README.md
+-rw-r--r--   0 fowler     (503) staff       (20)        6 2023-05-09 13:30:29.000000 sbmlcore-0.2.0/VERSION
+-rw-r--r--   0 fowler     (503) staff       (20)      116 2023-05-09 13:29:27.000000 sbmlcore-0.2.0/pyproject.toml
+drwxr-xr-x   0 fowler     (503) staff       (20)        0 2023-05-09 13:33:56.774311 sbmlcore-0.2.0/sbmlcore/
+-rw-r--r--   0 fowler     (503) staff       (20)     6161 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/AminoAcidProperties.py
+-rw-r--r--   0 fowler     (503) staff       (20)     3915 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/DeepDDG.py
+-rw-r--r--   0 fowler     (503) staff       (20)    16192 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/ExternalCode.py
+-rw-r--r--   0 fowler     (503) staff       (20)     2282 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/FeaturesDataFrame.py
+-rw-r--r--   0 fowler     (503) staff       (20)      426 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/Misc.py
+-rw-r--r--   0 fowler     (503) staff       (20)     3238 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/RaSP.py
+-rw-r--r--   0 fowler     (503) staff       (20)     2840 2023-01-06 14:07:50.000000 sbmlcore-0.2.0/sbmlcore/ResidueDepth.py
+-rw-r--r--   0 fowler     (503) staff       (20)     6194 2022-10-05 09:39:59.000000 sbmlcore-0.2.0/sbmlcore/StructuralDistances.py
+-rw-r--r--   0 fowler     (503) staff       (20)     3791 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/TempFactors.py
+-rw-r--r--   0 fowler     (503) staff       (20)    17544 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/TrajectoryDihedrals.py
+-rw-r--r--   0 fowler     (503) staff       (20)     9895 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/TrajectoryDistances.py
+-rw-r--r--   0 fowler     (503) staff       (20)     1207 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/sbmlcore/__init__.py
+drwxr-xr-x   0 fowler     (503) staff       (20)        0 2023-05-09 13:33:56.775076 sbmlcore-0.2.0/sbmlcore.egg-info/
+-rw-r--r--   0 fowler     (503) staff       (20)     3911 2023-05-09 13:33:56.000000 sbmlcore-0.2.0/sbmlcore.egg-info/PKG-INFO
+-rw-r--r--   0 fowler     (503) staff       (20)      935 2023-05-09 13:33:56.000000 sbmlcore-0.2.0/sbmlcore.egg-info/SOURCES.txt
+-rw-r--r--   0 fowler     (503) staff       (20)        1 2023-05-09 13:33:56.000000 sbmlcore-0.2.0/sbmlcore.egg-info/dependency_links.txt
+-rw-r--r--   0 fowler     (503) staff       (20)       55 2023-05-09 13:33:56.000000 sbmlcore-0.2.0/sbmlcore.egg-info/requires.txt
+-rw-r--r--   0 fowler     (503) staff       (20)        9 2023-05-09 13:33:56.000000 sbmlcore-0.2.0/sbmlcore.egg-info/top_level.txt
+-rw-r--r--   0 fowler     (503) staff       (20)     1119 2023-05-09 13:33:56.780935 sbmlcore-0.2.0/setup.cfg
+drwxr-xr-x   0 fowler     (503) staff       (20)        0 2023-05-09 13:33:56.780327 sbmlcore-0.2.0/tests/
+-rw-r--r--   0 fowler     (503) staff       (20)      234 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_MDAnalysis.py
+-rw-r--r--   0 fowler     (503) staff       (20)      753 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_MW.py
+-rw-r--r--   0 fowler     (503) staff       (20)      757 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_Pi.py
+-rw-r--r--   0 fowler     (503) staff       (20)      786 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_aminoacidvolumechange.py
+-rw-r--r--   0 fowler     (503) staff       (20)     3807 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_deep_ddg.py
+-rw-r--r--   0 fowler     (503) staff       (20)     1201 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_dssp.py
+-rw-r--r--   0 fowler     (503) staff       (20)     2412 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_freesasa.py
+-rw-r--r--   0 fowler     (503) staff       (20)     1617 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_hydropathy.py
+-rw-r--r--   0 fowler     (503) staff       (20)      677 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_rasp.py
+-rw-r--r--   0 fowler     (503) staff       (20)      330 2023-01-06 15:36:46.000000 sbmlcore-0.2.0/tests/test_residuedepth.py
+-rw-r--r--   0 fowler     (503) staff       (20)      349 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_rogov.py
+-rw-r--r--   0 fowler     (503) staff       (20)     1916 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_snap2.py
+-rw-r--r--   0 fowler     (503) staff       (20)     1168 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_stride.py
+-rw-r--r--   0 fowler     (503) staff       (20)     2782 2023-05-09 13:20:53.000000 sbmlcore-0.2.0/tests/test_structuraldistances.py
+-rw-r--r--   0 fowler     (503) staff       (20)      665 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_tempfactor.py
+-rw-r--r--   0 fowler     (503) staff       (20)     9512 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_trajectorydihedrals.py
+-rw-r--r--   0 fowler     (503) staff       (20)     6544 2022-09-15 05:28:46.000000 sbmlcore-0.2.0/tests/test_trajectorydistances.py
```

### Comparing `sbmlcore-0.1.4/LICENSE` & `sbmlcore-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.1.4/README.md` & `sbmlcore-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-# sbml-core
-Collection of core classes and functions for structure-based machine learning to predict antimicrobial resistance.
+[![Tests](https://github.com/fowler-lab/sbmlcore/actions/workflows/tests.yaml/badge.svg)](https://github.com/fowler-lab/sbmlcore/actions/workflows/tests.yaml)
+[![codecov](https://codecov.io/gh/fowler-lab/sbmlcore/branch/main/graph/badge.svg?token=P44BPYQBFS)](https://codecov.io/gh/fowler-lab/sbmlcore)
+[![PyPI version](https://badge.fury.io/py/sbmlcore.svg)](https://badge.fury.io/py/sbmlcore)
+
+# sbmlcore
+Collection of core classes to help with building structure- and chemistry-based feature datasets to train machine learning models to predict antimicrobial resistance.
 
 This is a pre-release alpha version - it may not be fully functional for your requirements and it is also subject to change with no notice!
 
-See notebooks walkthrough.ipynb and addition_methods_walkthrough.ipynb for
-quick user tutorials.
+We will be making a series of jupyter-notebooks demonstrating how to use the classes available [here](https://github.com/fowler-lab/sbmlcore-tutorials).
 
 ## Included features
 
 ### Changes in Amino Acid Properties
 
 - Volume
 - Hydropathy scales: Kyte-Doolittle ([paper](https://www.sciencedirect.com/science/article/abs/pii/0022283682905150?via%3Dihub)) and WimleyWhite ([paper](https://www.nature.com/articles/nsb1096-842))
@@ -37,7 +40,9 @@
 - Distances between mutated residues and any atom/group of atoms of interest. Uses MDAnalysis ([paper1](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3144279/) and [paper2](https://conference.scipy.org/proceedings/scipy2016/oliver_beckstein.html)).
 
 ## To potentially include at a later stage
  - Secondary structure: DSSP (do not anticipate much difference to STRIDE)
  - Protein stability:
     1. StabilityPredict. Online metapredictor, single amino acid at a time. Josh used in the pncA paper but had to contact them directly to run the entirity of PncA. ([paper](https://www.jbc.org/article/S0021-9258(20)34176-4/fulltext))
     2. DynaMUT. Also claims to outperform DUET etc. ([paper](https://academic.oup.com/nar/article/46/W1/W350/4990022)). Can process a list of specified mutations in one job. ([server](http://biosig.unimelb.edu.au/dynamut/))
+
+PWF, 9 May 2023
```

### Comparing `sbmlcore-0.1.4/sbmlcore/AminoAcidProperties.py` & `sbmlcore-0.2.0/sbmlcore/AminoAcidProperties.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,30 @@
+import pkg_resources
+
 import pandas
 #N.B. All property scales have been checked! CIL
 
 def _make_table(data_dict):
     rows = []
     for i in data_dict.keys():
         for j in data_dict.keys():
             rows.append([i, j, data_dict[j] - data_dict[i]])
     return pandas.DataFrame(rows, columns=['ref_amino_acid', 'alt_amino_acid', 'value'])
 
 
 class AminoAcidProperty(object):
-    """Amino acid dataframe."""
+    """Base class for storing amino acid properties.
+    
+    Notes:
+        uses a pandas.DataFrame
+    """
 
     def __init__(self):
 
         pass
-        # assert isinstance(dataframe, pandas.DataFrame)
-        #
-        # self.dataframe = dataframe
-        #
-        # assert 'mutation' in self.dataframe.columns, 'passed dataframe must contain a column called mutations'
-        #
-        # def find_amino_acids(row):
-        #     return(row.mutation[0], row.mutation[-1])
-        #
-        # self.dataframe[['ref_amino_acid','alt_amino_acid']] = self.dataframe.apply(find_amino_acids,axis=1)
 
     def _add_feature(self, other):
 
         assert isinstance(other, pandas.DataFrame)
 
         assert self.lookup.columns[0] not in other.columns, 'trying to add a column that is already in the dataset!'
 
@@ -46,22 +42,37 @@
         other.reset_index(inplace=True)
 
         other.drop(columns = ['ref_amino_acid', 'alt_amino_acid'], inplace=True)
 
         return(other)
 
 
-class AminoAcidVolumeChange(AminoAcidProperty):
-    """
-    Change in volume (ang^3) of an amino acid site due to a mutation.
+class AminoAcidRogovChange(AminoAcidProperty):
+
+    def __init__(self):
+
+        filename = pkg_resources.resource_filename("sbmlcore", 'data/rogov.csv')
+        self.lookup = pandas.read_csv(filename)
+
+        def split_row(row):
+            if isinstance(row.MUTATION, str) and len(row.MUTATION)==2:
+                return(pandas.Series([row.MUTATION[0], row.MUTATION[-1]]))
+            else:
+                return(pandas.Series([None,None]))
+
 
-    Returns
-    -------
-    dataframe with additional column for d_volume
+        self.lookup[['ref_amino_acid', 'alt_amino_acid']] = self.lookup.apply(split_row, axis=1)
+        self.lookup.rename(columns={'SCORE': 'd_rogov'}, inplace=True)
+        self.lookup.drop(columns=['MUTATION'], inplace=True)
+        self.lookup.set_index(['ref_amino_acid', 'alt_amino_acid'], inplace=True)
 
+
+class AminoAcidVolumeChange(AminoAcidProperty):
+    """
+    Change in sidechain volume (ang^3) of an amino acid due to a mutation.
     """
 
     def __init__(self):
 
         aa_volume = {'A': 88.6, 'R': 173.4, 'N': 114.1, 'D': 111.1, 'C': 108.5,
                       'Q': 143.8, 'E': 138.4, 'G': 60.1, 'H': 153.2, 'I': 166.7,
                       'L': 166.7, 'K': 168.6, 'M': 162.9, 'F': 189.9, 'P': 112.7,
@@ -70,22 +81,19 @@
         self.lookup = _make_table(aa_volume)
         self.lookup.rename(columns = {'value': 'd_volume'}, inplace=True)
         self.lookup.set_index(['ref_amino_acid', 'alt_amino_acid'],inplace=True)
 
 
 class AminoAcidHydropathyChangeKyteDoolittle(AminoAcidProperty):
     """
-    Change in hydropathy of an amino acid site due to a mutation.
-
-    Different hydropathy/hydrophobicity scales can be used.
-    Kyte and Doolittle (1982) DOI 10.1016/0022-2836(82)90515-0
+    Change in hydropathy due to a mutation.
 
-    Returns
-    -------
-    dataframe with additional column for d_hydropathy_KD
+    Notes:
+        Kyte and Doolittle (1982) DOI 10.1016/0022-2836(82)90515-0
+        Wimley-White is also available.
     """
 
     def __init__(self):
 
         aa_hydropathy_KD = {'A': 1.8, 'R': -4.5, 'N': -3.5, 'D': -3.5,
                             'C': 2.5, 'E': -3.5, 'Q': -3.5, 'G': -0.4,
                             'H': -3.2, 'I': 4.5, 'L': 3.8, 'K': -3.9,
@@ -97,20 +105,17 @@
         self.lookup.set_index(['ref_amino_acid', 'alt_amino_acid'],inplace=True)
 
 
 class AminoAcidHydropathyChangeWimleyWhite(AminoAcidProperty):
     """
     Change in hydropathy of an amino acid site due to a mutation.
 
-    Different hydropathy/hydrophobicity scales can be used.
-    Wimley White (1996) DOI 10.1038/nsb1096-842, octanol-interface scale from https://blanco.biomol.uci.edu/hydrophobicity_scales.html, Asp- Glu- His+ used.
-
-    Returns
-    -------
-    dataframe with additional column for d_hydropathy_WW
+    Notes:
+        Wimley White (1996) DOI 10.1038/nsb1096-842, octanol-interface scale from https://blanco.biomol.uci.edu/hydrophobicity_scales.html, Asp- Glu- His+ used.
+        Kyte and Doolittle (1982) is also available.
     """
 
     def __init__(self):
 
         aa_hydropathy_WW = {'A': 0.33, 'R': 1.00, 'N': 0.43, 'D': 2.41,
                             'C': 0.22, 'Q': 0.19, 'E': 1.61, 'G': 1.14,
                             'H': 1.37, 'I': -0.81, 'L': -0.69, 'K': 1.81,
@@ -122,20 +127,16 @@
         self.lookup.set_index(['ref_amino_acid', 'alt_amino_acid'],inplace=True)
 
 
 class AminoAcidMWChange(AminoAcidProperty):
     """
     Change in molecular weight (g/mol) of an amino acid site due to a mutation.
 
-    From: https://www.thermofisher.com/uk/en/home/references/ambion-tech-support/rna-tools-and-calculators/proteins-and-amino-acids.html
-
-    Returns
-    -------
-    dataframe with additional column for d_MW
-
+    Notes:
+        From: https://www.thermofisher.com/uk/en/home/references/ambion-tech-support/rna-tools-and-calculators/proteins-and-amino-acids.html
     """
 
     def __init__(self):
 
         aa_MW = {'A': 89.1, 'R': 174.2, 'N': 132.1, 'D': 133.1, 'C': 121.2,
                  'E': 147.1, 'Q': 146.2, 'G':75.1, 'H': 155.2, 'I': 131.2,
                  'L': 131.2, 'K': 146.2, 'M': 149.2, 'F': 165.2, 'P': 115.1,
@@ -146,19 +147,16 @@
         self.lookup.set_index(['ref_amino_acid', 'alt_amino_acid'],inplace=True)
 
 
 class AminoAcidPiChange(AminoAcidProperty):
     """
     Change in isoelectric point of an amino acid site due to a mutation.
 
-    From https://www.sigmaaldrich.com/life-science/metabolomics/learning-center/amino-acid-reference-chart.html
-
-    Returns
-    -------
-    dataframe with additional column for d_Pi
+    Notes:
+        From https://www.sigmaaldrich.com/life-science/metabolomics/learning-center/amino-acid-reference-chart.html
     """
 
     def __init__(self):
 
         aa_Pi = {'A': 6.00, 'R': 10.76, 'N': 5.41, 'D': 2.77, 'C': 5.07, 'E': 3.22,
              'Q': 5.65, 'G': 5.97, 'H': 7.59, 'I': 6.02, 'L': 5.98, 'K': 9.74,
              'M': 5.74, 'F': 5.48, 'P': 6.30, 'S': 5.68, 'T': 5.60, 'W': 5.89,
```

### Comparing `sbmlcore-0.1.4/sbmlcore/DeepDDG.py` & `sbmlcore-0.2.0/sbmlcore/DeepDDG.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 import pathlib
-import copy
 
 import pandas
 
 class DeepDDG(object):
     """
-    Prediction of protein stability.
-
-    Parameters
-    ----------
-    .ddg file
-    offsets - as dictionary of form {segid (str): value (int)}
-
-    Returns
-    -------
-    Dataframe with protein stability as an extra column
+    Prediction of protein stability via the DeepDDG webserver.
 
+    Args:
+        DeepDDGFile (file): file written out by the DeepDDG webserver
+        offsets (dict): dictionary of form {segid (str): value (int)} where value is 
+                the numerical offset between the genetic sequence and the PDB
     """
 
     def __init__(self, DeepDDGFile, offsets=None):
 
         assert pathlib.Path(DeepDDGFile).is_file(), "specified file does not exist!"
 
         self.deep_ddg_file = DeepDDGFile
```

### Comparing `sbmlcore-0.1.4/sbmlcore/ExternalCode.py` & `sbmlcore-0.2.0/sbmlcore/ExternalCode.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,38 @@
 import pathlib
 import shutil
 import subprocess
 
 import pandas
 import freesasa
+import sbmlcore
+
 # unsure whether to try and do a base class
 
 # class ExternalCode(object):
 #
 #     def __init__(self, PBBFile):
 #
 
-amino_acid_3to1letter = {'CYS': 'C', 'ASP': 'D', 'SER': 'S', 'GLN': 'Q', 'LYS': 'K',
-     'ILE': 'I', 'PRO': 'P', 'THR': 'T', 'PHE': 'F', 'ASN': 'N',
-     'GLY': 'G', 'HIS': 'H', 'LEU': 'L', 'ARG': 'R', 'TRP': 'W',
-     'ALA': 'A', 'VAL':'V', 'GLU': 'E', 'TYR': 'Y', 'MET': 'M'}
 
 def wrap_angle(angle):
     angle =  angle % 360
     if angle > 180:
         angle -= 360;
     return(angle)
 
 
 class Stride(object):
     """
-    Secondary structure and SASA prediction
+    Prediction of secondary structure, SASA, backbone dihedral angles and numbers of hbond donor and acceptors using STRIDE
 
-    Parameters
-    ----------
-    .pdb file
-    offsets - as dictionary of form {segid (str): value (int)}
-
-    Returns
-    -------
-    dataframe with additional columns for:
-    secondary_structure
-    secondary_structure_long
-    phi
-    psi
-    residue_sasa
-    B
-    C
-    E
-    G
-    H
-    T
+    Args:
+        PDBFile (file): Protein Databank file containing protein coordinates
+        offsets (dict): dictionary of form {segid (str): value (int)} where value is 
+                the numerical offset between the genetic sequence and the PDB
     """
 
     def __init__(self, PDBFile, offsets=None):
 
         assert pathlib.Path(PDBFile).is_file(), "specified PDB file does not exist!"
 
         self.pdb_file = PDBFile
@@ -60,43 +43,63 @@
         # or if there is one in the $PATH use that one
         elif shutil.which('stride') is not None:
              stride = pathlib.Path(shutil.which('stride'))
 
         else:
             raise IOError("No stride installed!")
 
-        output = subprocess.getoutput(str(stride)+' ' + self.pdb_file)
+        output = subprocess.getoutput(str(stride)+' -h ' + self.pdb_file)
 
         rows=[]
+        hbond_acc=[]
+        hbond_dnr=[]
         for line in output.split('\n'):
             if line[:3] == 'ASG':
                 rows.append(line.split()[1:])
+            elif line[:3] == 'ACC':
+                cols = line.split()
+                hbond_acc.append([cols[1], cols[2], cols[3], cols[10]])
+            elif line[:3] == 'DNR':
+                cols = line.split()
+                hbond_dnr.append([cols[1], cols[2], cols[3], cols[10]])
 
         self.results = pandas.DataFrame(rows, columns=['resname', 'segid', 'resid',\
                                                        'ordinal_resid', 'secondary_structure',\
                                                        'secondary_structure_long', 'phi', 'psi',\
                                                        'residue_sasa', 'pdb_code'])
 
+        acceptors = pandas.DataFrame(hbond_acc, columns=['resname', 'segid', 'resid', 'n_hbond_acceptors'])
+        acceptors = acceptors.groupby(['resname', 'segid', 'resid']).count()
+
+        donors = pandas.DataFrame(hbond_dnr, columns=['resname', 'segid', 'resid', 'n_hbond_donors'])
+        donors = donors.groupby(['resname', 'segid', 'resid']).count()
+
+        self.results.set_index(['resname', 'segid', 'resid'], inplace=True)
+        self.results = self.results.join(acceptors, how='left')
+        self.results = self.results.join(donors, how='left')
+        self.results.fillna(0, inplace=True)
+        self.results.reset_index(inplace=True)
+
         def short_amino_acid(row):
-            return amino_acid_3to1letter[row.resname]
+            return sbmlcore.amino_acid_3to1letter[row.resname]
 
         self.results['amino_acid'] = self.results.apply(short_amino_acid, axis=1)
 
         self.results = self.results.astype({'resid': 'int',\
                                             'phi': 'float',\
                                             'psi': 'float',\
                                             'residue_sasa': 'float'})
         def correct_torsions(row):
             return pandas.Series([wrap_angle(row.phi), wrap_angle(row.psi)])
 
         self.results[['phi','psi']] = self.results.apply(correct_torsions, axis=1)
 
         self.results = self.results[['resid', 'amino_acid', 'segid',
                                      'secondary_structure', 'secondary_structure_long',
-                                     'phi', 'psi', 'residue_sasa']]
+                                     'phi', 'psi', 'residue_sasa', 'n_hbond_acceptors', 'n_hbond_donors']]
 
         tmp = pandas.get_dummies(self.results.secondary_structure)
         self.results = self.results.join(tmp, how='left')
 
         # apply any offsets to the residue numbering
         # as specified in the supplied offsets dict e.g. {'A': 3, 'B': -4}
         # Chain is segid i.e. A, B, C etc.
@@ -113,15 +116,14 @@
 
             for chain in offsets:
                 assert isinstance(offsets[chain], int), "Offsets for each segid must be an integer!"
 
             self.results['resid'] = self.results.apply(update_resid, args=(offsets,), axis=1)
 
 
-
     def _add_feature(self, other, feature_name='all'):
 
         assert isinstance(other, pandas.DataFrame)
 
         assert 'mutation' in other.columns, 'passed dataframe must contain a column called mutation'
 
         assert 'segid' in other.columns, 'passed dataframe must contain a column called segid containing chain information e.g. A'
@@ -150,26 +152,24 @@
         other.drop(columns = ['amino_acid', 'resid'], inplace=True)
 
         return(other)
 
 
 class FreeSASA(object):
     """
-    Uses external FreeSASA Python module to obtain the solvent accessible
-    surface areas of each residue in a user-specified pdb file.
-
-    Parameters
-    ----------
-    .pdb file
-    offsets - as dictionary of form {segid (str): value (int)}
-
-    Returns
-    -------
-    dataframe with additional column for SASA
+    The Solvent Accessible Surface Area (SASA) information for each amino acid in a protein. 
 
+    Notes:
+        Uses the external FreeSASA Python module to obtain the solvent accessible
+        surface areas of each residue in a user-specified pdb file.
+
+    Args:
+        PDBFile (file): path to a Protein Databank file containing protein coordinates
+        offsets (dict): dictionary of form {segid (str): value (int)} where value is 
+                        the numerical offset between the genetic sequence and the PDB
     """
 
     def __init__(self, PDBFile, offsets=None):
 
         if not pathlib.Path(PDBFile).is_file():
             raise IOError("Specified PDB file does not exist!")
 
@@ -189,14 +189,15 @@
 #        for key in area_classes:
 #            print(key, ": %.2f A2" % area_classes[key])
 
     def _add_feature(self, other):
         """
         Calculates and adds the SASA for each residue to the existing mutation dataframe (other).
         """
+
         assert isinstance(other, pandas.DataFrame), "You must be adding the extra feature to an existing dataframe!"
 
         assert 'mutation' in other.columns, "Passed dataframe must contain a column called mutation"
 
         assert 'segid' in other.columns, "Passed dataframe must contain a column called segid containing chain information e.g. A"
 
         # Checks on offset specification
@@ -204,87 +205,83 @@
             for chain in self.offsets:
                 assert chain in set(other.segid), "Must only specify the segids in the mutation dataframe! And these must also be present in the pdb."
                 assert isinstance(self.offsets[chain], int), "Offsets for each segid must be an integer!"
         else:
             pass
 
 
-    #Split mutation df to create new index in form of segid-resid from mutation
+        # Split mutation df to create new index in form of segid-resid from mutation
         def split_mutation(row):
             m=row.mutation
             return(int(m[1:-1]))
 
         other['resid'] = other.apply(split_mutation, axis=1)
         other['id'] = other['segid'] + other['resid'].astype(str)
         other.set_index('id', inplace=True)
 
-    #Create single letter resname column for mutation dataframe
+        # Create single letter resname column for mutation dataframe
         def resname_1(row):
             m=row.mutation
             return(str(m[0:1]))
 
         other['resname_1'] = other.apply(resname_1, axis=1)
 
-        #Adds offsets to mutation dataframe
+        # Adds offsets to mutation dataframe
         if self.offsets is not None:
             other["chain_offsets"] = [self.offsets[chain] for chain in other.segid]
         else:
             other["chain_offsets"] = 0
 
-        #Add three letter amino acid to mutation dataframe (needed for FreeSASA input)
-        amino_acid_onetothreeletter = {'C': 'CYS', 'D': 'ASP', 'S': 'SER', 'Q': 'GLN', 'K': 'LYS',
-        'I': 'ILE', 'P': 'PRO', 'T': 'THR', 'F': 'PHE', 'N': 'ASN',
-        'G': 'GLY', 'H': 'HIS', 'L': 'LEU', 'R': 'ARG', 'W': 'TRP',
-        'A': 'ALA', 'V': 'VAL', 'E': 'GLU', 'Y': 'TYR', 'M': 'MET'}
+        # Add three letter amino acid to mutation dataframe (needed for FreeSASA input)
 
-        other["resname_3"] = [amino_acid_onetothreeletter[resname] for resname in other.resname_1]
+        other["resname_3"] = [sbmlcore.amino_acid_1to3letter[resname] for resname in other.resname_1]
 
-        #Adds column for pdb resids (i.e. the resid as given in the pdb which may not be the same as in the mutation df)
-        #N.B. Specify the offsets in the same way as you did for structural features class!
+        # Adds column for pdb resids (i.e. the resid as given in the pdb which may not be the same as in the mutation df)
+        # N.B. Specify the offsets in the same way as you did for structural features class!
         other["pdb_resid"] = other["resid"] - other["chain_offsets"]
 
-        #Creates correct text input for FreeSASA - N.B. includes offsets in  pdb_resid i.e. these new resids should be the same as in the pdb (not the mutation dataframe)
+        # Creates correct text input for FreeSASA - N.B. includes offsets in  pdb_resid i.e. these new resids should be the same as in the pdb (not the mutation dataframe)
         sele_text = ["%s%i, resi %i and chain %s and resn %s" % (k,i,j,k,l) for i,j,k,l in zip(other.resid, other.pdb_resid, other.segid, other.resname_3)]
 
-        #sele_text = ["%s%i, resi %i and chain %s" % (j,i,i,j) for i,j in zip(other.resid, other.segid)]
+        # sele_text = ["%s%i, resi %i and chain %s" % (j,i,i,j) for i,j in zip(other.resid, other.segid)]
 
-        #Obtain SASAs for each residue
+        # Obtain SASAs for each residue
         structure = freesasa.Structure(self.pdb_file)
         values = freesasa.calc(structure)
         results = freesasa.selectArea(sele_text, structure, values)
         s = pandas.Series(results)
         b = pandas.DataFrame(s, columns=['SASA'])
-        #print(b)
+        # print(b)
 
-        #Join SASA df to original mutation df
+        # Join SASA df to original mutation df
         other = other.join(b, how='left')
         other.reset_index(drop=True, inplace=True)
 
         other.drop(columns = ['resname_1', 'chain_offsets', 'resname_3', 'pdb_resid', 'resid'], inplace=True)
 
         return(other)
 
+
 class SNAP2(object):
     """
-    Uses the .csv output file from Snap2 https://rostlab.org/services/snap2web/ which predicts the likelihood of each amino acid mutation affecting the function of the protein.
+    Likelihood of each amino acid mutation affecting the function of the protein.
 
-    Parameters
-    ----------
-     .csv output from the SNAP2 webserver
-             N.B. If structure contains multiple chains, each one needs to be loaded into the webserver individually, then the .csv files need to be concatenated using csv_segid_concat.ipynb and the segid for each chain correctly assigned. Only then can the SNAP2 class here be used.
-     offsets - as dictionary of form {segid (str): value (int)}
-
-    Returns
-    -------
-    dataframe with additional columns for:
-    Predicted Effect
-    Score
-    Expected Accuracy
-        N.B. Score is probably the only useful column so dropping the other two columns is advised.
+    Notes:
+        Uses the .csv output file from Snap2 https://rostlab.org/services/snap2web/
+        If structure contains multiple chains, each one needs to be loaded into the 
+        webserver individually, then the .csv files need to be concatenated using 
+        csv_segid_concat.ipynb and the segid for each chain correctly assigned. 
+        Only then can the SNAP2 class here be used.
+
+    Args:
+        CSVFile (.csv file): file output from the SNAP2 webserver
+        offsets (dict): dictionary of form {segid (str): value (int)} where value is 
+                        the numerical offset between the genetic sequence and the PDB
     """
+
     def __init__(self, CSVFile, offsets=None):
 
         if not pathlib.Path(CSVFile).is_file():
             raise IOError("Specified CSV file does not exist!")
 
         self.csv_file = CSVFile
 
@@ -294,85 +291,93 @@
         if offsets is not None:
             assert isinstance(offsets, dict), "Offsets should be specified as a dictionary e.g. offsets = {'A': 3, 'B': 4}"
             self.offsets = offsets
         else:
             print("Must supply offsets, and .csv must have segids")
             self.offsets = offsets
 
-        #Create dataframe from .csv file
+        # create dataframe from .csv file
         snap2_df = pandas.read_csv(self.csv_file)
-        #print(snap2_df)
 
-        #Check offsets are correctly specified or raise KeyError
+        # check offsets are correctly specified or raise KeyError
 
         for segid in snap2_df['segid']:
             if segid not in offsets:
                 raise KeyError('Need to specify an offset for ALL segids!')
 
-        #Remove entries with less than 80% accuracy
-        #N.B. 27/05/22 Removed this feature by changing to remove less than 0%
-        #Could make this into a user option instead?
-        #First need to change 'Expected Accuracy' from strings to floats
+        # remove entries with less than 80% accuracy
+        # N.B. 27/05/22 Removed this feature by changing to remove less than 0%
+        # could make this into a user option instead?
+        # first need to change 'Expected Accuracy' from strings to floats
         no_percentage = snap2_df['Expected Accuracy'].replace(to_replace='%', value='', regex=True)
 
-        #Turn str into int64 so that inequalities can be used
+        snap2_df['Expected Accuracy'].replace(to_replace='%', value='', regex=True, inplace=True)
+        snap2_df['Expected Accuracy'] = snap2_df['Expected Accuracy'].astype('int')
+
+        # turn str into int64 so that inequalities can be used
         series = pandas.to_numeric(no_percentage)
 
-        #no_percentage[ series < 80 ] #creates series with only those rows for which accuracy < 80%
-        #no_percentage[series < 80].index #extracts index for each of the rows for which accuracy < 80%
+        # no_percentage[ series < 80 ] #creates series with only those rows for which accuracy < 80%
+        # no_percentage[series < 80].index #extracts index for each of the rows for which accuracy < 80%
 
-        #Remove the entries for which the indices are specified above
+        # remove the entries for which the indices are specified above
         snap2_df.drop(no_percentage[series < 0].index, inplace=True)
 
-        #Add offsets column and correct mutation resid column and mutated resname (i.e. the residue change resulting from the mutation)
+        # add offsets column and correct mutation resid column and mutated resname (i.e. the residue change resulting from the mutation)
 
         def split_mutation_toresname(row):
             return pandas.Series([row.Variant[-1], int(row.Variant[1:-1])])
 
-        snap2_df[["mutated_to_resname", "resid"]] = snap2_df.apply(split_mutation_toresname, axis=1)
-
+        snap2_df[["alt_amino_acid", "resid"]] = snap2_df.apply(split_mutation_toresname, axis=1)
 
-        #Adds column for offsets
+        # adds column for offsets
         snap2_df["chain_offsets"] = [offsets[chain] for chain in snap2_df.segid]
 
-        #Applies offsets - adds them, as is also the case for Structural Features
-        snap2_df["mutation_resid"] = snap2_df["resid"] + snap2_df["chain_offsets"]
+        # applies offsets - adds them, as is also the case for Structural Features
+        snap2_df["resid"] = snap2_df["resid"] + snap2_df["chain_offsets"]
 
-        self.snap2_df = snap2_df
+        # snap2_df.drop(columns='resid', inplace=True)
+
+        snap2_df.rename(columns={'Predicted Effect':'snap2_effect',\
+                                 'Score':'snap2_score',\
+                                 'Expected Accuracy':'snap2_accuracy',\
+                                 'Variant': 'mutation'
+                                }, inplace=True)
+
+        self.results = snap2_df
 
 
     def _add_feature(self, other):
         """
-        Adds distances to existing mutation dataframe, and returns new joined dataframe.
+        Private method to add distances to existing mutation dataframe
         """
 
         assert isinstance(other, pandas.DataFrame), "You must be adding the extra feature to an existing dataframe!"
 
-        assert 'Score' not in other.columns, "You've already added that feature!"
+        assert 'snap2_score' not in other.columns, "You've already added that feature!"
 
         assert 'mutation' in other.columns, "Passed dataframe must contain a column called mutation"
 
         assert 'segid' in other.columns, "Passed dataframe must contain a column called segid containing chain information e.g. A"
 
-        # Identifies the original one letter resname and resid (consistent with offset) so that the new feature can be subsequently linked to these
+        # identifies the original one letter resname and resid (consistent with offset) so that the new feature can be subsequently linked to these
         #def split_mutation(row):
         #    return pandas.Series([row.mutation[0], int(row.mutation[1:-1])])
 
         #other[['amino_acid', 'mutation_resid']] = other.apply(split_mutation, axis=1)
 
-        #Add column for mutated_to_resname into original mutation df (i.e. the residue change as a result of the mutation) and the mutation resid so that the new feature can subsequently be linked to these
+        # add column for mutated_to_resname into original mutation df (i.e. the residue change as a result of the mutation) and the mutation resid so that the new feature can subsequently be linked to these
         def split_mutation_toresname(row):
             return pandas.Series([row.mutation[-1], int(row.mutation[1:-1])])
 
-        other[['mutated_to_resname', 'mutation_resid']] = other.apply(split_mutation_toresname, axis=1)
+        other[['alt_amino_acid', 'resid']] = other.apply(split_mutation_toresname, axis=1)
 
-        #Create MultiIndex using segid, resid and amino_acid
-        other.set_index(['segid', 'mutation_resid', 'mutated_to_resname'], inplace=True)
-        self.snap2_df.set_index(['segid', 'mutation_resid', 'mutated_to_resname'], inplace=True)
-
-        other = other.join(self.snap2_df, how='left')
+        # create MultiIndex using segid, resid and amino_acid
+        other.set_index(['segid', 'resid', 'alt_amino_acid'], inplace=True)
+        self.results.set_index(['segid', 'resid', 'alt_amino_acid'], inplace=True)
+        other = other.join(self.results[['snap2_score', 'snap2_accuracy']], how='left')
         other.reset_index(inplace=True) #Removes multi-index
 
-        #Remove superfluous columns
-        other.drop(columns = ['mutation_resid', 'mutated_to_resname', 'Variant', 'resid', 'chain_offsets'], inplace=True)
-        #print(other)
+        # remove superfluous columns
+        other.drop(columns = ['resid', 'alt_amino_acid'], inplace=True)
+
         return(other)
```

### Comparing `sbmlcore-0.1.4/sbmlcore/FeaturesDataFrame.py` & `sbmlcore-0.2.0/sbmlcore/FeaturesDataFrame.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 import pandas
 
+
 class FeatureDataset(object):
     '''
-    Class that contains the dataset of mutations and associated features for simple machine learning.
-
-    Parameters
-    ----------
-    existing dataframe
-
-    Optional:
-    protein (str)
-    gene (str)
-    species (str)
-    reference (str)
-
-    Returns
-    -------
-    dataframe with additional feature columns
+    Dataset of protein mutations and associated structural- and chemical-features for simple machine learning.
 
+    Args:
+        dataframe (pandas.DataFrame) 
+        protein (str, optional): protein name
+        gene (str, optional): gene name
+        species (str, optional): species
+        reference (str)
     '''
 
     def __init__(self, df, *args, **kwargs):
 
         assert isinstance(df, pandas.DataFrame), 'must supply a pandas.DataFrame'
 
         assert 'mutation' in df.columns, 'passed pandas.DataFrame must contain a column called mutation'
@@ -39,27 +32,26 @@
         for key in set(allowed_kwargs).difference(seen):
             # Default values to None if the kwarg has not been passed
             setattr(self, key, None)
 
 
     def __add__(self, other):
         ''''
-        Overload the addition operator.
+        Overload the addition operator to allow sbml Features to be added.
         '''
+
         self.df = other._add_feature(self.df)
 
         return self
 
     def __repr__(self):
         '''
-        Overload the print function to write a summary of this Features dataset.
-
-        Returns:
-            str: String describing the Features dataset
+        Print a summary of this Features dataset to STDOUT.
         '''
+
         output = ''
         if self.species is not None:
             output += 'species:          ' + self.species + '\n'
 
         if self.gene is not None:
             output += 'gene name:        ' + self.gene + '\n'
 
@@ -76,15 +68,16 @@
         return(output)
 
 
     def add_feature(self, other):
         '''
         Add the supplied sbmlcore Feature to this dataset.
 
-        Arguments:
+        Args:
             sbmlcore.Feature or list of sbmlcore.Features
         '''
+
         if isinstance(other,list):
             for i in other:
                 self.df = i._add_feature(self.df)
         else:
             self.df = other._add_feature(self.df)
```

### Comparing `sbmlcore-0.1.4/sbmlcore/StructuralDistances.py` & `sbmlcore-0.2.0/sbmlcore/StructuralDistances.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 import pandas
 import pathlib
 import MDAnalysis
-
-amino_acid_3to1letter = {'CYS': 'C', 'ASP': 'D', 'SER': 'S', 'GLN': 'Q', 'LYS': 'K',
-     'ILE': 'I', 'PRO': 'P', 'THR': 'T', 'PHE': 'F', 'ASN': 'N',
-     'GLY': 'G', 'HIS': 'H', 'LEU': 'L', 'ARG': 'R', 'TRP': 'W',
-     'ALA': 'A', 'VAL':'V', 'GLU': 'E', 'TYR': 'Y', 'MET': 'M'}
-
+import sbmlcore
+ 
 class StructuralDistances(object):
     """
-    Class for structural distances
+    Distances between a specified region (i.e. origin) and all amino acids in a protein.
+
+    Args:
+        pdb_file (file): path to the Protein DataBank file
+        distance_selection (str): the MDAnalysis style selection text that defines the origin
+                                  e.g. "resname MG"
+        distance_name (str): what you would like to call this distance
+        infer_masses (bool): whether to allow MDAnalysis to infer the masses of the atoms in the distance_selection, 
+                             allows the centre of mass to be calculated. This will generally work for residues, but 
+                             for small molecules the masses may not be able to be inferred, in which case set this to False
+                             and ensure only heavy atoms are in the supplied PDB and it will find the centre of geometry.
+        offsets (dict): dictionary of form {segid (str): value (int)} where value is 
+                        the numerical offset between the genetic sequence and the PDB
+
+    Examples:
+        The below will calculate the distance from the Magnesium ion in the M. tuberculosis
+        RNA polymerase structure to all amino acids in the protein. Since chain D (rpoB) in the
+        PDB file is numbered differently to the gene an offset dictionary is also supplied.
 
-    Parameters
-    ----------
-    1st - pdb file
-    2nd - group of atoms you want to calculate the distances to - uses MDAnalysis syntax, and distances are calculated from the centre of mass of this whole selection to each Ca in the structure
-    3rd - your choice of name for the resulting distance column in the dataframe
-    4th - resid offsets for the different chains - must be a dictionary in the form {'segid': int, ...}.
-
-    E.g. a = sbmlcore.StructuralDistances('tests/5uh6.pdb','resname MG', 'Mg_distance', offsets = {'A': 0, 'B': 0, 'C': -6})
-
-    Returns
-    -------
-    dataframe with structural distance columns (named by user)
+        >>> a = sbmlcore.StructuralDistances('tests/5uh6.pdb','resname MG', 'Mg_distance', offsets = {'A': 0, 'B': 0, 'C': -6})
     """
 
-    def __init__(self, pdb_file, distance_selection, distance_name, offsets=None):
+    def __init__(self, pdb_file, distance_selection, distance_name, infer_masses=True, offsets=None):
 
         # check file exists
         assert pathlib.Path(pdb_file).is_file(), "File does not exist!"
 
         u = MDAnalysis.Universe(pdb_file)
 
-        #Ensure distance selection is a string
+        # ensure distance selection is a string
         assert isinstance(distance_selection, str), "Distance selection must be a string!"
 
-        reference_com = u.select_atoms(distance_selection).center_of_mass()
-        #Check atom selection exists
+        # prefer to calculate the centre of mass, but the masses cannot always be inferred from the PDB file
+        if infer_masses:
+            reference_com = u.select_atoms(distance_selection).center_of_mass()
+        else:
+            reference_com = u.select_atoms(distance_selection).center_of_geometry()
+
+        # check atom selection exists
         assert u.select_atoms(distance_selection).n_atoms > 0, "Atom selection does not exist! Is your selection using the correct MDAnalysis syntax?"
 
         # apply any offsets to the residue numbering
         # as specified in the supplied offsets dict e.g. {'A': 3, 'B': -4}
         # Chain is segid i.e. A, B, C etc.
         if offsets is not None:
             assert isinstance(offsets, dict), "Offsets should be specified as a dictionary e.g. offsets = {'A': 3, 'B': -4}"
@@ -54,27 +61,26 @@
 
         distances = MDAnalysis.lib.distances.distance_array(reference_com, Ca_all.positions)
 
         Ca_data = {'segid': Ca_all.segids, 'resid': Ca_all.resids,
                    'resname': Ca_all.resnames, distance_name: distances[0]}
 
         def one_letter(row):
-            return(amino_acid_3to1letter[row.resname])
+            return(sbmlcore.amino_acid_3to1letter[row.resname])
 
         results = pandas.DataFrame(Ca_data)
         results['amino_acid'] = results.apply(one_letter, axis=1)
 
         self.results = results
         self.distance_name = distance_name
 
 
     def _add_feature(self, other):
         """
-        Adds distances to existing mutation dataframe, and returns new joined dataframe.
-        Arguments: existing dataframe
+        Private method to add distances to existing mutation dataframe
         """
 
         assert isinstance(other, pandas.DataFrame), "You must be adding the extra feature to an existing dataframe!"
 
         assert self.distance_name not in other.columns, "You've already added that feature!"
 
         assert 'mutation' in other.columns, "Passed dataframe must contain a column called mutation"
@@ -83,22 +89,22 @@
 
         # Identifies the original one letter resname and resid (consistent with offset) so that the new feature can be subsequently linked to these
         def split_mutation(row):
             return pandas.Series([row.mutation[0], int(row.mutation[1:-1])])
 
         other[['amino_acid', 'resid']] = other.apply(split_mutation, axis=1)
 
-        #Create MultiIndex using segid, resid and amino_acid
+        # create MultiIndex using segid, resid and amino_acid
         other.set_index(['segid', 'resid', 'amino_acid'], inplace=True)
         self.results.set_index(['segid', 'resid', 'amino_acid'], inplace=True)
 
         other = other.join(self.results, how='left')
 
-        #To check that the chain offsets have been correctly set
-        #and/or that structural data is of adequate quality -
+        # to check that the chain offsets have been correctly set
+        # and/or that structural data is of adequate quality -
         # defining this as the no NaNs should be less than half no rows
 
         #print("This is no rows:", len(other[self.distance_name])) #gives length of column 'Mg_distance'
 
         half_data = len(other[self.distance_name])//2 # // divides and rounds DOWN to nearest int
         #print("This is half the no rows, rounded down:", half_data)
 
@@ -114,10 +120,12 @@
         for i in other[self.distance_name]:
             assert isinstance(i, float), "Distances must be floats!"
 
 
         other.reset_index(inplace=True)
         self.results.reset_index(inplace=True)
 
-        other.drop(columns = ['amino_acid', 'resid', 'resname'], inplace=True)
+        other.drop(columns=['amino_acid', 'resid', 'resname'], inplace=True)
+
+        #other.drop(columns = ['amino_acid', 'resid', 'resname', 'resname_1', 'chain_offsets', 'resname_3', 'pdb_resid'], inplace=True)
 
         return(other)
```

### Comparing `sbmlcore-0.1.4/sbmlcore/TrajectoryDihedrals.py` & `sbmlcore-0.2.0/sbmlcore/TrajectoryDihedrals.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,77 +1,52 @@
 import pathlib
 
 import pandas
 import numpy
 import MDAnalysis
 from MDAnalysis.analysis.dihedrals import Dihedral
-
-amino_acid_3to1letter = {
-    "CYS": "C",
-    "ASP": "D",
-    "SER": "S",
-    "GLN": "Q",
-    "LYS": "K",
-    "ILE": "I",
-    "PRO": "P",
-    "THR": "T",
-    "PHE": "F",
-    "ASN": "N",
-    "GLY": "G",
-    "HIS": "H",
-    "LEU": "L",
-    "ARG": "R",
-    "TRP": "W",
-    "ALA": "A",
-    "VAL": "V",
-    "GLU": "E",
-    "TYR": "Y",
-    "MET": "M",
-}
+import sbmlcore
 
 
 class TrajectoryDihedrals(object):
-    """Calculate and add dihedral angles from a molecular dynamics trajectory.
-
-    Parameters
-    ----------
-    1st - path to structure file
-    2nd - list containing paths to trajectory files
-    3rd - path to pdb_file of static structure - used to pull segment ids as these are often lost in trajectory structure files
-    4th - the target angle (phi, psi, omega)
-    5th - your choice of name for the resulting distance column in the dataframe
-    6th - type of angle metic that is being calculated (mean, median, max, or min)(default=mean)
-    7th - if the structure file doesn't contain all bonds, one can set add_bonds=True to fire an MDAnalysis bond prediction algorithm
-    8th - resid offsets for the different chains - must be a dictionary in the form {'segid':int, ...}.
-    9th - desired starting time of the trajectory
-    10th - deisred end time of the trajectory
-    11th - if percentile_exclusion is set to True, only data between the 5th and 9th percentile is considered (default=False)
-
-    E.g. a = a = sbmlcore.TrajectoryDihedrals(
-        "./tests/rpob-5uh6-3-warm.gro.gz",
-        [
-            "./tests/rpob-5uh6-3-md-1-50ns-dt10ns-nojump.xtc",
-        ],
-        "./tests/5uh6.pdb",
-        "phi",
-        "mean_phi",
-        angle_type="mean",
-        add_bonds=True,
-        offsets = {'A': 0, 'B': 0, 'C': -6},
-        percentile_exclusion=True
-        )
-
-    Returns
-    ----------
-    Instantiating the class instantiates a df with segment ids, residue ids, residue names, and associated distances to the specified reference selection
-
-    add_feature adds distances to existing mutation dataframe, and returns new joined dataframed
-
+    """Average dihedrals between a specified region (i.e. origin) and all amino acids in a protein.
+    
+    Notes:
+        smblcore is using MDAnalysis to load and analyse the trajectories so any trajectory
+        it can parse (XTC, DCD) can be used, and also the MDAnalysis selection style text must
+        be used to identify the region/origin to measure the distances from.
+
+    Args:
+        pdb_file (file): 
+        trajectory_list (list of paths): list of paths to molecular dynamics trajectories
+        static_pdb (file): path to the Protein DataBank
+        dihedral (str): the target angle (phi, psi or omega)
+        angle_name (str): what you would like to call this angle
+        angle_type (str): one of mean, median, max or min (default is mean)
+        add_bonds (bool): if the structure file doesn't contain all bonds, then setting add_bonds=True 
+                          will run an MDAnalysis bond prediction algorithm
+        offsets (dict): dictionary of form {segid (str): value (int)} where value is 
+                        the numerical offset between the genetic sequence and the PDB
+        start_time (float): from what time to start using frames from the trajectory
+        end_time (float): before which time to stop using frames from the trajectory
+        percentile_exclusion (bool): if True, then the 0-5th and 5-100th percentile distances
+                                     are excluded. Default is False
+    Examples:
+        >>> a = sbmlcore.TrajectoryDihedrals("./tests/dhfr-3fre-tmp-1-1.gro",
+                                             ["./tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc"],
+                                            "./tests/dhfr-3fre-tmp-1-1.pdb",
+                                            "phi",
+                                            "mean_phi",
+                                            angle_type="mean",
+                                            add_bonds=True,
+                                            offsets = {'A': 0},
+                                            percentile_exclusion=True
+                                            )
     """
-
+    
     def __init__(
         self,
         pdb_file,
         trajectory_list,
         static_pdb,
         dihedral,
         angle_name,
@@ -183,24 +158,24 @@
 
         # calculate the specified metric for each residue (mean, max, min, median)
         angles = self.apply_angle_type(dihedral_array)
 
         # pull segment ids from the static pdb file
         segids = [i for i in u_static.select_atoms("protein").residues.segids]
 
-        # constructs the dictionary containing the distances and assocaited residue labels
+        # construct the dictionary containing the distances and assocaited residue labels
         data = {
             "segid": segids,
             "resid": residues_all.resids,
             "resname": residues_all.resnames,
             angle_name: angles,
         }
 
         def one_letter(row):
-            return amino_acid_3to1letter[row.resname]
+            return sbmlcore.amino_acid_3to1letter[row.resname]
 
         results = pandas.DataFrame(data)
         results["amino_acid"] = results.apply(one_letter, axis=1)
         results.drop(columns=["resname"], inplace=True)
         # otherwise column names post merge in add_feature are messy
 
         if offsets is not None:
@@ -263,29 +238,29 @@
                     ).run()
                     # add the segment of angles to the dihedral array
                     x = numpy.concatenate((x, y.results["angles"]), axis=1)
 
         return x
 
     def search_nonetypes(self, traj):
-        """searches for nonetype dihedral angles and returns a list of their indexes"""
+        """Searches for nonetype dihedral angles and returns a list of their indexes"""
 
         selection_call = "i." + self.dihedral + "_selection()"
 
         index = 0
         nonetype_list = []
         residues = traj.select_atoms("protein")
         for i in residues.residues:
             if not eval(selection_call):
                 nonetype_list.append(index)
             index += 1
         return nonetype_list
 
     def apply_angle_type(self, dihedral_array):
-        """calculates the specified angle for each residue across all frames"""
+        """Calculates the specified angle for each residue across all frames"""
 
         if self.angle_type == "mean":
             angles = numpy.mean(dihedral_array, axis=1)
         elif self.angle_type == "min":
             angles = numpy.min(dihedral_array, axis=1)
         elif self.angle_type == "max":
             angles = numpy.max(dihedral_array, axis=1)
@@ -363,15 +338,15 @@
 
     def return_angle_df(self):
         """returns the df generated by init method (useful for tests)"""
         return self.results
 
     @staticmethod
     def _filter_frames(pdb, traj, boundary, spec_time, dt):
-        """returns universe with frames greater and
+        """Returns MDAnalysis.Universe with frames greater and
         less than the specified start and end times"""
 
         # Becuase a new universe is essentially being created, every coordinate in the original is needed
         coordinates = (
             MDAnalysis.analysis.base.AnalysisFromFunction(
                 lambda ag: ag.positions.copy(), traj.atoms
             )
@@ -421,28 +396,28 @@
 
     @staticmethod
     def _exclude_percentiles(data):
         """return array without 5% tails"""
         data_list = []
         for resnum in range(len(data)):
             # calculate the expected length of an array after the tailes have been removed
-            len_no_tails = len(data[resnum]) - (0.1 * len(data[resnum]))
             if data[resnum].all() == numpy.zeros(len(data[resnum])).all():
+                dummy_arr = numpy.array([i for i in range(1, len(data[resnum])+1)])
                 # if the arrays is just an array of zeros, numpy can't calculate p5 nor p95 -
                 # //so we do it manually
-                arr = numpy.zeros(int(len_no_tails) - 1)
+                p5, p95 = numpy.percentile(dummy_arr, 5), numpy.percentile(dummy_arr, 95)
+                len_no_tails = len(dummy_arr[(dummy_arr > p5) & (dummy_arr <= p95)])
+                arr = numpy.zeros(int(len_no_tails))
                 data_list.append(arr)
             else:
                 arr = data[resnum]
                 p5 = numpy.percentile(arr, 5)
                 p95 = numpy.percentile(arr, 95)
                 data_list.append(arr[(arr > p5) & (arr <= p95)])
-
         data_arr = numpy.array(data_list)
-
         return data_arr
 
     @staticmethod
     def _apply_offsets(df, offsets):
         """returns dataframe with number offsets applied to the resids"""
         for chain in offsets:
             assert chain in set(
```

### Comparing `sbmlcore-0.1.4/sbmlcore/TrajectoryDistances.py` & `sbmlcore-0.2.0/sbmlcore/TrajectoryDistances.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,42 @@
 import pathlib
 
 import pandas
 import numpy
 import MDAnalysis
+import sbmlcore
 
-amino_acid_3to1letter = {
-    "CYS": "C",
-    "ASP": "D",
-    "SER": "S",
-    "GLN": "Q",
-    "LYS": "K",
-    "ILE": "I",
-    "PRO": "P",
-    "THR": "T",
-    "PHE": "F",
-    "ASN": "N",
-    "GLY": "G",
-    "HIS": "H",
-    "LEU": "L",
-    "ARG": "R",
-    "TRP": "W",
-    "ALA": "A",
-    "VAL": "V",
-    "GLU": "E",
-    "TYR": "Y",
-    "MET": "M",
-}
 
 
 class TrajectoryDistances(object):
     """
-    Calculate and add distances from a molecular dynamics trajectory.
-
-    Parameters
-    ----------
-    1st - path to structure file
-    2nd - list containing paths to trajectory files
-    3rd - path to pdb_file of static structure - used to pull segment ids as these are often lost in trajectory structure files
-    4th - group of atoms you want to calculate the distances to - uses MDAnalysis syntax, and distances are calculated from the centre of mass of this whole selection to each Ca in the structure
-    5th - your choice of name for the resulting distance column in the dataframe
-    6th - type of distance metric that is being calculated (mean, median, max or min) (default=mean)
-    7th - resid offsets for the different chains - must be a dictionary in the form {'segid': int, ...}.
-    8th - desired starting time of the trajectory
-    9th - desired end time of the trajectory
-    10th - if percentile_exlcusion is set to True, only data between the 5th and 9th percentile is considered (default=False)
-
-    E.g. a = sbmlcore.StructuralDistances('tests/5uh6.gro',['tests/5uh6.xtc'], '5hu6.pdb', 'resname RFP', 'RFP_distance', distance_type='median', offsets = {'A': 0, 'B': 0, 'C': -6}, 'start_time=1000', 'end_time=49000', percentile_exclusion=True)
-
-    Returns
-    -------
-    Instantiating the class instantiates a df with segment ids, residue ids, residue names, and associated distances to the specified reference selection
-
-    add_feature adds distances to existing mutation dataframe, and returns new joined dataframe
+    Average distances between a specified region (i.e. origin) and all amino acids in a protein.
+    
+    Notes:
+        smblcore is using MDAnalysis to load and analyse the trajectories so any trajectory
+        it can parse (XTC, DCD) can be used, and also the MDAnalysis selection style text must
+        be used to identify the region/origin to measure the distances from.
+
+    Args:
+        pdb_file (file): 
+        trajectory_list (list of paths): list of paths to molecular dynamics trajectories
+        static_pdb (file): path to the Protein DataBank
+        distance_selection (str): the MDAnalysis style selection text that defines the origin
+                                  e.g. "resname MG"
+        distance_name (str): what you would like to call this distance
+        distance_type (str): one of mean, median, max or min (default is mean)
+        offsets (dict): dictionary of form {segid (str): value (int)} where value is 
+                        the numerical offset between the genetic sequence and the PDB
+        start_time (float): from what time to start using frames from the trajectory
+        end_time (float): before which time to stop using frames from the trajectory
+        percentile_exclusion (bool): if True, then the 0-5th and 5-100th percentile distances
+                                     are excluded. Default is False
+    Examples:
 
+        >>> a = sbmlcore.StructuralDistances('tests/5uh6.gro',['tests/5uh6.xtc'], '5hu6.pdb', 'resname RFP', 'RFP_distance', distance_type='median', offsets = {'A': 0, 'B': 0, 'C': -6}, 'start_time=1000', 'end_time=49000', percentile_exclusion=True)
     """
 
     def __init__(
         self,
         pdb_file,
         trajectory_list,
         static_pdb,
@@ -81,18 +61,21 @@
         # ensure the distance type is legal, and the distance selection and name are strings
         assert distance_type in [
             "mean",
             "min",
             "max",
             "median",
         ], "provided distance_type not recognised!"
+
         assert isinstance(
             distance_selection, str
         ), "Distance selection must be a string!"
+
         assert isinstance(distance_name, str), "Distance name must be a string!"
+
         # checks whether percentile_exlcusion is True/False
         assert isinstance(
             percentile_exclusion, bool
         ), "Confidence interval must be True or False"
 
         if offsets is not None:
             # ensure the offsets are specified in a dictionary
@@ -171,15 +154,15 @@
             "segid": segids,
             "resid": Ca_all.resids,
             "resname": Ca_all.resnames,
             distance_name: distances,
         }
 
         def one_letter(row):
-            return amino_acid_3to1letter[row.resname]
+            return sbmlcore.amino_acid_3to1letter[row.resname]
 
         results = pandas.DataFrame(Ca_data)
         results["amino_acid"] = results.apply(one_letter, axis=1)
         results.drop(columns=["resname"], inplace=True)
         # otherwise column names post merge in add_feature are messy
 
         if offsets is not None:
@@ -188,25 +171,16 @@
         self.results = results
         self.distance_name = distance_name
 
     def _add_feature(self, existing_df):
         """
         Adds distances to existing mutation dataframe, and returns new joined dataframe.
 
-        Parameters
-        ---------
-        1st - existing dataframe
-
-        E.g. if a = sbmlcore.TrajectoryDistances(...),
-        use new_df = a.add_feature(existing_df)
-
-        Returns
-        --------
-        New, joined dataframe
-
+        Args:
+            existing_df (pandas.DataFrame): the FeaturesDataset
         """
 
         assert isinstance(
             existing_df, pandas.DataFrame
         ), "You must be adding the extra feature to an existing dataframe!"
 
         assert (
@@ -260,27 +234,27 @@
 
     def return_dist_df(self):
         """returns the df generated by init method (useful for tests)"""
         return self.results
 
     @staticmethod
     def _exclude_percentiles(data):
-        """returns array without 5% tails"""
+        """Returns array without 5% tails"""
         data_list = []
         for resnum in range(len(data)):
             arr = data[resnum]
             p5 = numpy.percentile(arr, 5)
             p95 = numpy.percentile(arr, 95)
             data_list.append(arr[(arr >= p5) & (arr <= p95)])
         data_arr = numpy.array(data_list)
         return data_arr
 
     @staticmethod
     def _apply_offsets(df, offsets):
-        """returns dataframe with numbering offsets applied to the resids"""
+        """Returns dataframe with numbering offsets applied to the resids"""
         for chain in offsets:
             assert chain in set(
                 df["segid"]
             ), "Need to specifify a segid that exists in the static pdb!"
             assert isinstance(
                 offsets[chain], int
             ), "Offsets for each segid must be an integer!"
```

### Comparing `sbmlcore-0.1.4/sbmlcore/__init__.py` & `sbmlcore-0.2.0/sbmlcore/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,29 @@
 # from .AminoAcidProperties import *
 from .AminoAcidProperties import AminoAcidProperty
 from .AminoAcidProperties import AminoAcidVolumeChange
 from .AminoAcidProperties import AminoAcidHydropathyChangeKyteDoolittle
 from .AminoAcidProperties import AminoAcidHydropathyChangeWimleyWhite
 from .AminoAcidProperties import AminoAcidMWChange
 from .AminoAcidProperties import AminoAcidPiChange
+from .AminoAcidProperties import AminoAcidRogovChange
+
+from .Misc import amino_acid_3to1letter
+from .Misc import amino_acid_1to3letter
 
 from .ExternalCode import Stride
 from .ExternalCode import FreeSASA
 from .ExternalCode import SNAP2
+from .TempFactors import TempFactors
 from .StructuralDistances import StructuralDistances
 from .TrajectoryDistances import TrajectoryDistances
 from .TrajectoryDihedrals import TrajectoryDihedrals
 from .DeepDDG import DeepDDG
+from .RaSP import RaSP
+from .ResidueDepth import ResidueDepth
 from .FeaturesDataFrame import FeatureDataset
 
 '''
 Use of semantic versioning, MAJOR.MINOR.MAINTAINANCE where
 MAJOR is not backwards compatible, but MINOR and MAINTAINANCE are
 '''
 __version__ = "0.0.1"
```

### Comparing `sbmlcore-0.1.4/sbmlcore.egg-info/SOURCES.txt` & `sbmlcore-0.2.0/sbmlcore.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 LICENSE
 README.md
+VERSION
 pyproject.toml
 setup.cfg
 sbmlcore/AminoAcidProperties.py
 sbmlcore/DeepDDG.py
 sbmlcore/ExternalCode.py
 sbmlcore/FeaturesDataFrame.py
+sbmlcore/Misc.py
+sbmlcore/RaSP.py
+sbmlcore/ResidueDepth.py
 sbmlcore/StructuralDistances.py
+sbmlcore/TempFactors.py
 sbmlcore/TrajectoryDihedrals.py
 sbmlcore/TrajectoryDistances.py
 sbmlcore/__init__.py
 sbmlcore.egg-info/PKG-INFO
 sbmlcore.egg-info/SOURCES.txt
 sbmlcore.egg-info/dependency_links.txt
-sbmlcore.egg-info/not-zip-safe
 sbmlcore.egg-info/requires.txt
 sbmlcore.egg-info/top_level.txt
-tests/__init__.py
 tests/test_MDAnalysis.py
 tests/test_MW.py
 tests/test_Pi.py
 tests/test_aminoacidvolumechange.py
 tests/test_deep_ddg.py
 tests/test_dssp.py
 tests/test_freesasa.py
 tests/test_hydropathy.py
+tests/test_rasp.py
+tests/test_residuedepth.py
+tests/test_rogov.py
 tests/test_snap2.py
 tests/test_stride.py
 tests/test_structuraldistances.py
+tests/test_tempfactor.py
 tests/test_trajectorydihedrals.py
 tests/test_trajectorydistances.py
```

### Comparing `sbmlcore-0.1.4/setup.cfg` & `sbmlcore-0.2.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sbmlcore
-version = 0.1.4
+version = file: VERSION
 author = Philip W Fowler and Charlotte I Lynch and Dylan Adlard
 author_email = philip.fowler@ndm.ox.ac.uk
 description = Constructs core features table for the application to machine learning models
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/fowler-lab/sbmlcore
 classifiers = 
@@ -23,20 +23,20 @@
 	Source = https://github.com/fowler-lab/sbmlcore
 	Tracker = https://github.com/fowler-lab/sbmlcore/issues
 
 [options]
 package_dir = 
 packages = sbmlcore
 python_requires = >=3.6
-zip_safe = False
 include_package_data = True
 install_requires = 
 	pandas
 	MDAnalysis
 	freesasa
 	pytest
 	pytest-cov
+	BioPython
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sbmlcore-0.1.4/tests/test_MW.py` & `sbmlcore-0.2.0/tests/test_MW.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.1.4/tests/test_Pi.py` & `sbmlcore-0.2.0/tests/test_Pi.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.1.4/tests/test_aminoacidvolumechange.py` & `sbmlcore-0.2.0/tests/test_aminoacidvolumechange.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.1.4/tests/test_deep_ddg.py` & `sbmlcore-0.2.0/tests/test_deep_ddg.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.1.4/tests/test_dssp.py` & `sbmlcore-0.2.0/tests/test_dssp.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.1.4/tests/test_freesasa.py` & `sbmlcore-0.2.0/tests/test_freesasa.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.1.4/tests/test_hydropathy.py` & `sbmlcore-0.2.0/tests/test_hydropathy.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.1.4/tests/test_snap2.py` & `sbmlcore-0.2.0/tests/test_snap2.py`

 * *Files identical despite different names*

### Comparing `sbmlcore-0.1.4/tests/test_stride.py` & `sbmlcore-0.2.0/tests/test_stride.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,17 @@
     a = sbmlcore.Stride('tests/3pl1.pdb')
 
     assert len(a.results) == 185
 
     # check that all the -180 < phi <= 180 (and also for psi)
     assert all((a.results.phi > -180) & (a.results.phi <= 180))
 
+    assert (a.results.n_hbond_acceptors>=0).sum() == 185
+    assert (a.results.n_hbond_donors>=0).sum() == 185
+
     # check that only these 1-letter codes are used for secondary structure
     assert set(a.results.secondary_structure).issubset({'H', 'I', 'G', 'E', 'B', 'T', 'C'})
 
     # these should all fail!
     with pytest.raises(AssertionError):
         a = sbmlcore.Stride('tests/3pl2.pdb')
```

### Comparing `sbmlcore-0.1.4/tests/test_structuraldistances.py` & `sbmlcore-0.2.0/tests/test_structuraldistances.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,18 +18,14 @@
     with pytest.raises(AssertionError):
         a = sbmlcore.StructuralDistances('tests/5uh7.pdb','resname ZN', 'Zn_distance', offsets = {'A': 0, 'B': 0, 'C': -6})
 
     # Distance selection is not a string
     with pytest.raises(AssertionError):
         a = sbmlcore.StructuralDistances('tests/5uh6.pdb', 5, 'Zn_distance', offsets = {'A': 0, 'B': 0, 'C': -6})
 
-    # Incorrectly naming a resname - i.e. atom selection does not exist
-    with pytest.raises(AssertionError):
-        a = sbmlcore.StructuralDistances('tests/5uh6.pdb','resname ZP', 'Zn_distance', offsets = {'A': 0, 'B': 0, 'C': -6})
-
     # Offsets is not a dictionary
     with pytest.raises(AssertionError):
         a = sbmlcore.StructuralDistances('tests/5uh6.pdb','resname ZN', 'Zn_distance', offsets = [0, 0, -6])
 
     # Incorrectly naming a segid offset with an incorrect letter
     with pytest.raises(AssertionError):
         a = sbmlcore.StructuralDistances('tests/5uh6.pdb','resname ZN', 'Zn_distance', offsets = {'A': 0, 'B': 0, 'Z': -6})
```

### Comparing `sbmlcore-0.1.4/tests/test_trajectorydihedrals.py` & `sbmlcore-0.2.0/tests/test_trajectorydihedrals.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 def test_missing_file():
 
     with pytest.raises(AssertionError):
         a = sbmlcore.TrajectoryDihedrals(
             "tests/dhfr-3fre-tmp-1-1.gro",
             "tests/missing.xtc",
             "tests/dhfr-3fre-tmp-1-1.pdb",
-            "psi", 
-            "mean_psi"
+            "psi",
+            "mean_psi",
         )
 
     with pytest.raises(AssertionError):
         a = sbmlcore.TrajectoryDihedrals(
             "tests/dhfr-3fre-tmp-1-1.gro",
             ["tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc"],
             "tests/missing.pdb",
-            "psi", 
-            "mean_psi"
+            "psi",
+            "mean_psi",
         )
 
     with pytest.raises(AssertionError):
         a = sbmlcore.TrajectoryDihedrals(
             "tests/missing.gro",
             ["tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc"],
             "tests/dhfr-3fre-tmp-1-1.pdb",
-            "psi", 
-            "mean_psi"
+            "psi",
+            "mean_psi",
         )
 
 
 def test_wrong_type():
 
     with pytest.raises(AssertionError):
         a = sbmlcore.TrajectoryDihedrals(
@@ -75,16 +75,16 @@
 
 def test_not_list():
     with pytest.raises(AssertionError):
         a = sbmlcore.TrajectoryDihedrals(
             "tests/dhfr-3fre-tmp-1-1.gro",
             "tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc",
             "tests/dhfr-3fre-tmp-1-1.pdb",
-            "psi", 
-            "mean_psi"
+            "psi",
+            "mean_psi",
         )
 
 
 def test_start_time():
     with pytest.raises(AssertionError):
         a = sbmlcore.TrajectoryDihedrals(
             "tests/dhfr-3fre-tmp-1-1.gro",
@@ -143,50 +143,50 @@
     input_df = pandas.DataFrame.from_dict(a)
     expected_output = pandas.DataFrame.from_dict(b)
     input_offsets = {"A": -3, "B": 0, "C": 7}
     output = sbmlcore.TrajectoryDistances._apply_offsets(input_df, input_offsets)
     pandas.testing.assert_frame_equal(output, expected_output)
 
 
-# def test_filter_frames():
+def test_filter_frames():
 
+    u = MDAnalysis.Universe(
+        "tests/dhfr-3fre-tmp-1-1.gro", "tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc"
+    )
+    dt = u.trajectory[1].time - u.trajectory[0].time
+    ut = sbmlcore.TrajectoryDihedrals._filter_frames(
+        "tests/dhfr-3fre-tmp-1-1.gro", u, "start", 2000, dt
+    )
+    test_coordinates = (
+        MDAnalysis.analysis.base.AnalysisFromFunction(
+            lambda ag: ag.positions.copy(), ut.atoms
+        )
+        .run()
+        .results
+    )
+    test_coordinates = pandas.DataFrame.from_dict(test_coordinates.timeseries[0])
+    expected_coordinates = pandas.read_csv(
+        "tests/test_start_coordinates_frame0.csv", index_col=0
+    )
+    expected_coordinates.rename(columns={"0": 0, "1": 1, "2": 2}, inplace=True)
+    pandas.testing.assert_frame_equal(
+        test_coordinates, expected_coordinates.astype("float32")
+    )
 
-#     u = MDAnalysis.Universe(
-#         "tests/rpob-5uh6-3-warm.gro.gz", 
-#         "tests/rpob-5uh6-3-md-1-50ns-dt10ns-nojump.xtc"
-#     )
-#     dt = u.trajectory[1].time - u.trajectory[0].time
-#     ut = sbmlcore.TrajectoryDihedrals._filter_frames(
-#         "tests/rpob-5uh6-3-warm.gro.gz", u, "start", 20000, dt
-#     )
-#     test_coordinates = (
-#         MDAnalysis.analysis.base.AnalysisFromFunction(
-#             lambda ag: ag.positions.copy(), ut.atoms
-#         )
-#         .run()
-#         .results
-#     )
-#     test_coordinates = pandas.DataFrame.from_dict(test_coordinates.timeseries[0])
-#     expected_coordinates = pandas.read_csv(
-#         "tests/test_start_coordinates_frame0.csv", index_col=0
-#     )
-#     expected_coordinates.rename(columns={'0':0, '1':1, "2":2}, inplace=True)
-#     pandas.testing.assert_frame_equal(test_coordinates, expected_coordinates.astype('float32'))
-
-#     ut = sbmlcore.TrajectoryDihedrals._filter_frames(
-#         "tests/rpob-5uh6-3-warm.gro.gz", u, "end", 30000, dt
-#     )
-#     test_coordinates = (
-#         MDAnalysis.analysis.base.AnalysisFromFunction(
-#             lambda ag: ag.positions.copy(), ut.atoms
-#         )
-#         .run()
-#         .results
-#     )
-#     assert len(test_coordinates.timeseries) == 3
+    ut = sbmlcore.TrajectoryDihedrals._filter_frames(
+        "tests/dhfr-3fre-tmp-1-1.gro", u, "end", 8000, dt
+    )
+    test_coordinates = (
+        MDAnalysis.analysis.base.AnalysisFromFunction(
+            lambda ag: ag.positions.copy(), ut.atoms
+        )
+        .run()
+        .results
+    )
+    assert len(test_coordinates.timeseries) == 8
 
 
 def test_apply_angle_type():
 
     instantiated_class = sbmlcore.TrajectoryDihedrals(
         "tests/dhfr-3fre-tmp-1-1.gro",
         ["tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc"],
@@ -197,102 +197,124 @@
     )
     input = numpy.array([[2, 4, 5, 6, 7, 8, 9], [6, 7, 8, 9, 0, 11, 12]])
     output = instantiated_class.apply_angle_type(input)
     expected_output = numpy.array([41 / 7, 53 / 7])
     numpy.testing.assert_array_equal(expected_output, output, verbose=True)
 
 
-# def test_search_nonetypes():
+def test_search_nonetypes():
+
+    u = MDAnalysis.Universe(
+        "tests/dhfr-3fre-tmp-1-1.gro", "tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc"
+    )
+    instantiated_class = sbmlcore.TrajectoryDihedrals(
+        "tests/dhfr-3fre-tmp-1-1.gro",
+        ["tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc"],
+        "tests/dhfr-3fre-tmp-1-1.pdb",
+        "psi",
+        "psi",
+    )
+    assert instantiated_class.search_nonetypes(u) == [156]
+
+
+def test_calculate_dihedrals():
+
+    u = MDAnalysis.Universe(
+        "tests/dhfr-3fre-tmp-1-1.gro", "tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc"
+    )
+    instantiated_class = sbmlcore.TrajectoryDihedrals(
+        "tests/dhfr-3fre-tmp-1-1.gro",
+        ["tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc"],
+        "tests/dhfr-3fre-tmp-1-1.pdb",
+        "phi",
+        "phi",
+    )
+    protein_res = u.select_atoms("protein")
+    output = instantiated_class.calculate_dihedrals(u, protein_res)
+    output = pandas.DataFrame(output)
+    expected_output = pandas.read_csv("tests/test_dihedrals.csv", index_col=0)
+    expected_output.columns = expected_output.columns.astype(int)
+
+    pandas.testing.assert_frame_equal(output, expected_output.astype("float64"))
+
+
+def test_init():
+    a = sbmlcore.TrajectoryDihedrals(
+        "tests/dhfr-3fre-tmp-1-1.gro",
+        [
+            "tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc",
+        ],
+        "tests/dhfr-3fre-tmp-1-1.pdb",
+        "phi",
+        "phi",
+        angle_type="max",
+        offsets={"A": 0},
+        percentile_exclusion=True,
+        start_time=2000.0,
+        end_time=8000.0,
+    ).return_angle_df()
+    b = pandas.read_csv("tests/3fre_traj_angles.csv", index_col=0)
+    pandas.testing.assert_frame_equal(a, b)
+
+
+def test_add_feature():
+
+    a = {
+        "segid": ["A", "A", "A", "A"],
+        "mutation": ["T1D", "L2K", "S3V", "S3F"],
+    }
+    df = pandas.DataFrame.from_dict(a)
+    features = sbmlcore.FeatureDataset(
+        df, species="S. aureus", gene="folA", protein="DHFR"
+    )
+    b = sbmlcore.TrajectoryDihedrals(
+        "tests/dhfr-3fre-tmp-1-1.gro",
+        [
+            "tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc",
+        ],
+        "tests/dhfr-3fre-tmp-1-1.pdb",
+        "psi",
+        "max psi",
+        angle_type="max",
+        offsets={"A": 0},
+        percentile_exclusion=True,
+        end_time=8000.0,
+    )
+    c = sbmlcore.TrajectoryDihedrals(
+        "tests/dhfr-3fre-tmp-1-1.gro",
+        [
+            "tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc",
+        ],
+        "tests/dhfr-3fre-tmp-1-1.pdb",
+        "omega",
+        "min omega",
+        angle_type="min",
+        offsets={"A": 0},
+        percentile_exclusion=True,
+        end_time=8000.0,
+    )
+
+    d = sbmlcore.TrajectoryDihedrals(
+        "tests/dhfr-3fre-tmp-1-1.gro",
+        [
+            "tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc",
+        ],
+        "tests/dhfr-3fre-tmp-1-1.pdb",
+        "phi",
+        "mean phi",
+        angle_type="mean",
+        offsets={"A": 0},
+        percentile_exclusion=True,
+        end_time=8000.0,
+    )
+
+    # method 1:
+    features.add_feature([b])
+
+    # method 2:
+    features_df = (features + c).df
+
+    # method 3:
+    features_df = d._add_feature(features_df)
 
-#     u = MDAnalysis.Universe(
-#         "tests/rpob-5uh6-3-warm.gro.gz", 
-#         "tests/rpob-5uh6-3-md-1-50ns-dt10ns-nojump.xtc"
-#     )
-#     instantiated_class = sbmlcore.TrajectoryDihedrals(
-#         "tests/dhfr-3fre-tmp-1-1.gro",
-#         ["tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc"],
-#         "tests/dhfr-3fre-tmp-1-1.pdb",
-#         "phi",
-#         "phi",
-#     )
-#     assert instantiated_class.search_nonetypes(u) == [0, 1575]
-
-
-# def test_calculate_dihedrals():
-
-#     u = MDAnalysis.Universe(
-#         "tests/rpob-5uh6-3-warm.gro.gz", "tests/rpob-5uh6-3-md-1-50ns-dt10ns-nojump.xtc"
-#     )
-#     instantiated_class = sbmlcore.TrajectoryDihedrals(
-#         "tests/rpob-5uh6-3-warm.gro.gz",
-#         ["tests/rpob-5uh6-3-md-1-50ns-dt10ns-nojump.xtc"],
-#         "tests/5uh6.pdb",
-#         "phi",
-#         "phi",
-#     )
-#     protein_res = u.select_atoms("protein")
-#     expected_output = pandas.read_csv("tests/test_dihedrals.csv", index_col=0)
-#     expected_output.columns = expected_output.columns.astype(int)
-#     output = instantiated_class.calculate_dihedrals(u, protein_res)
-#     output = pandas.DataFrame(output)
-#     pandas.testing.assert_frame_equal(output, expected_output.astype('float64'))
-
-
-# def test_init():
-#     a = sbmlcore.TrajectoryDihedrals(
-#         "tests/dhfr-3fre-tmp-1-1.gro",
-#         [
-#             "tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc",
-#             "tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc"
-#         ],
-#         "tests/dhfr-3fre-tmp-1-1.pdb",
-#         "phi",
-#         "phi",
-#         angle_type="max",
-#         offsets={"A": 0},
-#         percentile_exclusion=True,
-#         start_time=100.0,
-#         end_time=400.0,
-#     ).return_angle_df()
-#     b = pandas.read_csv("tests/5uh6_traj_angles.csv", index_col=0)
-#     pandas.testing.assert_frame_equal(a, b)
-
-
-# def test_add_feature():
-
-#     a = {
-#         "segid": ["A", "A", "A", "B", "C", "C"],
-#         "mutation": ["I3D", "S4K", "Q5V", "R6D", "S450F", "D435F"],
-#     }
-#     df = pandas.DataFrame.from_dict(a)
-#     b = sbmlcore.TrajectoryDihedrals(
-#         "tests/rpob-5uh6-3-warm.gro.gz",
-#         [
-#             "tests/rpob-5uh6-3-md-1-50ns-dt10ns-nojump.xtc",
-#             "tests/rpob-5uh6-3-md-2-50ns-dt10ns-nojump.xtc",
-#         ],
-#         "tests/5uh6.pdb",
-#         "psi",
-#         "max psi",
-#         angle_type="max",
-#         offsets={"A": 0, "B": 0, "C": -6},
-#         percentile_exclusion=True,
-#         end_time=40000.0,
-#     )
-#     c = sbmlcore.TrajectoryDihedrals(
-#         "tests/rpob-5uh6-3-warm.gro.gz",
-#         [
-#             "tests/rpob-5uh6-3-md-1-50ns-dt10ns-nojump.xtc",
-#             "tests/rpob-5uh6-3-md-2-50ns-dt10ns-nojump.xtc",
-#         ],
-#         "tests/5uh6.pdb",
-#         "omega",
-#         "min omega",
-#         angle_type="min",
-#         offsets={"A": 0, "B": 0, "C": -6},
-#         percentile_exclusion=True,
-#         end_time=40000.0,
-#     )
-#     df = b._add_feature(df)
-#     df = c._add_feature(df)
-#     test_df = pandas.read_csv('tests/5uh6_added_traj_angles.csv', index_col=0)
-#     pandas.testing.assert_frame_equal(test_df, df)
+    test_df = pandas.read_csv("tests/3fre_added_traj_angles.csv", index_col=0)
+    pandas.testing.assert_frame_equal(test_df, features_df)
```

### Comparing `sbmlcore-0.1.4/tests/test_trajectorydistances.py` & `sbmlcore-0.2.0/tests/test_trajectorydistances.py`

 * *Files 8% similar despite different names*

```diff
@@ -159,53 +159,69 @@
         "resname TMP",
         "max_TMP",
         distance_type="max",
         offsets={"A": 0},
         percentile_exclusion=True,
     ).return_dist_df()
 
-    # b = pandas.read_csv("tes/5uh6_traj_distances.csv", index_col=0)
-
     assert a.max_TMP.sum() == pytest.approx(5120.556)
-    # pandas.testing.assert_frame_equal(a, b)
 
 
-# def test_add_feature():
-#     # although this requires running the entire class to merge the dfs,
-#     # all other components of the class should have been individually tested by now
-#     a = {
-#         "segid": ["A", "A", "A", "B", "C", "C"],
-#         "mutation": ["I3D", "S4K", "Q5V", "R6D", "S450F", "D435F"],
-#     }
-#     df = pandas.DataFrame.from_dict(a)
-#     b = sbmlcore.TrajectoryDistances(
-#         "tests/rpob-5uh6-3-warm.gro",
-#         [
-#             "tests/rpob-5uh6-3-md-1-50ns-dt10ns-nojump.xtc",
-#             "tests/rpob-5uh6-3-md-2-50ns-dt10ns-nojump.xtc",
-#             "tests/rpob-5uh6-3-md-3-50ns-dt10ns-nojump.xtc",
-#         ],
-#         "tests/5uh6.pdb",
-#         "resname RFP",
-#         "max RFP",
-#         distance_type="max",
-#         offsets={"A": 0, "B": 0, "C": -6},
-#         percentile_exclusion=True,
-#     )
-#     c = sbmlcore.TrajectoryDistances(
-#         "tests/rpob-5uh6-3-warm.gro",
-#         [
-#             "tests/rpob-5uh6-3-md-1-50ns-dt10ns-nojump.xtc",
-#             "tests/rpob-5uh6-3-md-2-50ns-dt10ns-nojump.xtc",
-#             "tests/rpob-5uh6-3-md-3-50ns-dt10ns-nojump.xtc",
-#         ],
-#         "tests/5uh6.pdb",
-#         "resname RFP",
-#         "mean RFP",
-#         distance_type="mean",
-#         offsets={"A": 0, "B": 0, "C": -6},
-#         percentile_exclusion=True,
-#     )
-#     test_df = pandas.read_csv("tests/5uh6_added_traj_distances.csv", index_col=0)
-#     df = b._add_feature(df)
-#     df = c._add_feature(df)
-#     pandas.testing.assert_frame_equal(test_df, df)
+def test_add_feature():
+    # although this requires running the entire class to merge the dfs,
+    # all other components of the class should have been individually tested by now
+    a = {
+        "segid": ["A", "A", "A", "A"],
+        "mutation": ["T1D", "L2K", "S3V", "S3F"],
+    }
+    df = pandas.DataFrame.from_dict(a)
+    features = sbmlcore.FeatureDataset(
+        df, species="S. aureus", gene="folA", protein="DHFR"
+    )
+    b = sbmlcore.TrajectoryDistances(
+        "tests/dhfr-3fre-tmp-1-1.gro",
+        [
+            "tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc",
+        ],
+        "tests/dhfr-3fre-tmp-1-1.pdb",
+        "resname NDP",
+        "max NDP",
+        distance_type="max",
+        offsets={"A": 0},
+        percentile_exclusion=True,
+    )
+    c = sbmlcore.TrajectoryDistances(
+        "tests/dhfr-3fre-tmp-1-1.gro",
+        [
+            "tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc",
+        ],
+        "tests/dhfr-3fre-tmp-1-1.pdb",
+        "resname TMP",
+        "min TMP",
+        distance_type="min",
+        offsets={"A": 0},
+        percentile_exclusion=True,
+    )
+    d = sbmlcore.TrajectoryDistances(
+        "tests/dhfr-3fre-tmp-1-1.gro",
+        [
+            "tests/dhfr-3fre-tmp-1-2-nojump-skip100.xtc",
+        ],
+        "tests/dhfr-3fre-tmp-1-1.pdb",
+        "resname NDP",
+        "mean NDP",
+        distance_type="mean",
+        offsets={"A": 0},
+        percentile_exclusion=True,
+    )
+
+    # method 1:
+    features.add_feature([b])
+
+    # method 2:
+    features_df = (features + c).df
+
+    # method 3:
+    features_df = d._add_feature(features_df)
+
+    test_df = pandas.read_csv('tests/3fre_added_traj_distances.csv', index_col=0)
+    pandas.testing.assert_frame_equal(test_df, features_df)
```

