# Comparing `tmp/getMultiPrimerSet-1.0.1.tar.gz` & `tmp/getMultiPrimerSet-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getMultiPrimerSet-1.0.1.tar", last modified: Sun May  7 04:01:21 2023, max compression
+gzip compressed data, was "getMultiPrimerSet-1.0.2.tar", last modified: Mon May  8 23:29:22 2023, max compression
```

## Comparing `getMultiPrimerSet-1.0.1.tar` & `getMultiPrimerSet-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 04:01:21.406588 getMultiPrimerSet-1.0.1/
--rw-r--r--   0 semiquant   (502) staff       (20)     2423 2023-05-07 04:01:21.406432 getMultiPrimerSet-1.0.1/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)     2686 2023-05-07 03:54:39.000000 getMultiPrimerSet-1.0.1/README.md
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 04:01:21.405489 getMultiPrimerSet-1.0.1/getMultiPrimerSet/
--rw-r--r--   0 semiquant   (502) staff       (20)    11592 2023-05-07 03:59:38.000000 getMultiPrimerSet-1.0.1/getMultiPrimerSet/getMultiPrimerSet.py
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 04:01:21.406253 getMultiPrimerSet-1.0.1/getMultiPrimerSet.egg-info/
--rw-r--r--   0 semiquant   (502) staff       (20)     2423 2023-05-07 04:01:21.000000 getMultiPrimerSet-1.0.1/getMultiPrimerSet.egg-info/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)      305 2023-05-07 04:01:21.000000 getMultiPrimerSet-1.0.1/getMultiPrimerSet.egg-info/SOURCES.txt
--rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-07 04:01:21.000000 getMultiPrimerSet-1.0.1/getMultiPrimerSet.egg-info/dependency_links.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       79 2023-05-07 04:01:21.000000 getMultiPrimerSet-1.0.1/getMultiPrimerSet.egg-info/entry_points.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       34 2023-05-07 04:01:21.000000 getMultiPrimerSet-1.0.1/getMultiPrimerSet.egg-info/requires.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       18 2023-05-07 04:01:21.000000 getMultiPrimerSet-1.0.1/getMultiPrimerSet.egg-info/top_level.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-07 04:01:21.406637 getMultiPrimerSet-1.0.1/setup.cfg
--rw-r--r--   0 semiquant   (502) staff       (20)     2779 2023-05-07 03:59:47.000000 getMultiPrimerSet-1.0.1/setup.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-08 23:29:22.756068 getMultiPrimerSet-1.0.2/
+-rw-r--r--   0 semiquant   (502) staff       (20)     2423 2023-05-08 23:29:22.755905 getMultiPrimerSet-1.0.2/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)     2829 2023-05-07 07:23:30.000000 getMultiPrimerSet-1.0.2/README.md
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-08 23:29:22.754984 getMultiPrimerSet-1.0.2/getMultiPrimerSet/
+-rw-r--r--   0 semiquant   (502) staff       (20)    12550 2023-05-08 17:27:12.000000 getMultiPrimerSet-1.0.2/getMultiPrimerSet/getMultiPrimerSet.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-08 23:29:22.755730 getMultiPrimerSet-1.0.2/getMultiPrimerSet.egg-info/
+-rw-r--r--   0 semiquant   (502) staff       (20)     2423 2023-05-08 23:29:22.000000 getMultiPrimerSet-1.0.2/getMultiPrimerSet.egg-info/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)      305 2023-05-08 23:29:22.000000 getMultiPrimerSet-1.0.2/getMultiPrimerSet.egg-info/SOURCES.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-08 23:29:22.000000 getMultiPrimerSet-1.0.2/getMultiPrimerSet.egg-info/dependency_links.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       79 2023-05-08 23:29:22.000000 getMultiPrimerSet-1.0.2/getMultiPrimerSet.egg-info/entry_points.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       34 2023-05-08 23:29:22.000000 getMultiPrimerSet-1.0.2/getMultiPrimerSet.egg-info/requires.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       18 2023-05-08 23:29:22.000000 getMultiPrimerSet-1.0.2/getMultiPrimerSet.egg-info/top_level.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-08 23:29:22.756114 getMultiPrimerSet-1.0.2/setup.cfg
+-rw-r--r--   0 semiquant   (502) staff       (20)     2779 2023-05-08 23:28:24.000000 getMultiPrimerSet-1.0.2/setup.py
```

### Comparing `getMultiPrimerSet-1.0.1/PKG-INFO` & `getMultiPrimerSet-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getMultiPrimerSet
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for generating multiplex PCR primer sets
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `getMultiPrimerSet-1.0.1/README.md` & `getMultiPrimerSet-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 | product_size_max | The desired max size for the PCR product. Default is 800. |
 | ret | The maximum number of primer pairs to return. Default is 100. |
 | Q5 | A boolean indicating whether to use NEB Q5 hotstart polymerase settings for primer3. Default is True. |
 | background | The path to the mispriming library FASTA file. Default is an empty string. |
 | output | The name of the output file. Default is 'MultiPlexPrimerSet'. |
 | eval | The maximum number of primer sets to evaluate. Default is 10000. |
 
+
+<img src="https://user-images.githubusercontent.com/8179171/236663567-94d1f5dc-2ac6-49de-9fc1-a99c7a13945d.png"  width="20%" height="20%">
+
+
 The main function of the script is 'design_primers', which takes the input FASTA file, start and end positions of a target region, and the arguments specified using argparse, and returns the best primer set for that region as a list of dictionaries containing information about the primer pairs.
 
 The 'design_primers' function performs the following steps:
 
 -   Parses the input FASTA file and extracts the target region sequence.
 -   Sets up the primer3 input parameters based on the specified arguments.
 -   Runs primer3 to design the primers.
@@ -52,8 +56,8 @@
     --Q5 \
     --background "" \
     --output "example"
 ```
 
 
 ### TODO
--   Add pre and post check for overlapping amplicons and correct
+-   Add pre and post check for overlapping amplicons and correct
```

### Comparing `getMultiPrimerSet-1.0.1/getMultiPrimerSet/getMultiPrimerSet.py` & `getMultiPrimerSet-1.0.2/getMultiPrimerSet/getMultiPrimerSet.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 import pandas as pd
 import itertools
 import argparse
 import numpy as np
 import concurrent.futures
 import sys
 import random
-
+import requests
 parser = argparse.ArgumentParser(description='PCR primer design')
 
 # from getMultiPrimerSet.getMultiPrimerSet import main
 
 # Define input arguments
 # parser.add_argument('--cpus', type=int, help='number of threads (even though it says cpus)', default=1000)
 parser.add_argument('--region_file', type=str, help='The path to the primer design region file. Two columns, start position and end position (1-based). tsv or xlxs', required=True)
 parser.add_argument('--input_file', type=str, help='The path to the input FASTA file.', required=True)
 parser.add_argument('--target_tm', type=float, help='The desired melting temperature (Tm) for the primers.', default=65)
 parser.add_argument('--primer_len', type=int, help='The desired length of the primers.', default=20)
 parser.add_argument('--product_size_min', type=int, help='The desired min size for the PCR product. Default is 400.', default=400)
 parser.add_argument('--product_size_max', type=int, help='The desired max size for the PCR product. Default is 800.', default=800)
 parser.add_argument('--ret', type=int, help='The maximum number of primer pairs to return.', default=100)
-parser.add_argument('--Q5', action='store_true', help='Whether to use Q5 settings for primer3.', default=True)
+parser.add_argument('--Q5', action='store_true', help='Whether to use Q5 approximation settings for Tm calculations.', default=True)
 parser.add_argument('--background', type=str, help='The path to the mispriming library FASTA file.', default='')
 parser.add_argument('--output', type=str, help='Output name.', default='MultiPlexPrimerSet')
 parser.add_argument('--eval', type=int, help='The maximum number of primer sets to evaluate.', default=10000)
 args = parser.parse_args()
 
 product_size_range = (args.product_size_min, args.product_size_max)
 
@@ -128,36 +128,48 @@
                     'name' : name
                     })
     except Exception as e:
         print("An error occurred:", e)
 
     return primer_pairs
 
+def q5_melting_temp(seq1, seq2="", salt=0.5):
+    url = "https://tmapi.neb.com/tm/q5/%s/%s/%s?&fmt=short" % (salt, seq1, seq2)
+    response = requests.get(url)
+    json_string = response.json()
+    tm1 = json_string["data"]["tm1"]
+    # tm2 = json_string["data"]["tm2"]
+    return tm1 #[tm1, tm2]
+
 
 def is_valid_combination(combination, names):
     if set(entry['name'] for entry in combination) == names:
         return combination
     return []
 
-def evaluate_combination(comb):
+def evaluate_combination(comb, Q5=args.Q5):
     # Create a list of primer pairs
     primer_pairs = [(p1, p2) for p1, p2 in itertools.combinations(comb, 2)]
     # Extract the primer sequences from the primer pairs
     primer_pairs_sequences = [(p1['Forward Primer'], p2['Reverse Primer']) for p1, p2 in primer_pairs]
     # Calculate heterodimer formation energy
     heterodimer_scores = []
     for p in primer_pairs_sequences:
-        heterodimer_scores.append(primer3.calcHeterodimer(p[0], p[1], temp_c=args.target_tm).dg) #gibbs free energy
-        
+        if Q5:
+            heterodimer_scores.append(primer3.calcHeterodimer(p[0], p[1], temp_c=args.target_tm, dv_conc = 2, mv_conc = 80, dna_conc = 5800).dg) #gibbs free energy
+        else:
+            heterodimer_scores.append(primer3.calcHeterodimer(p[0], p[1], temp_c=args.target_tm).dg) #gibbs free energy
+    product_size_weight=0.2
+    heterodimer_score_weight =0.8
     score = {'size': product_size_range,
              'tmp': tm_range,
              'mean': np.mean(heterodimer_scores),
              'range': abs(np.min(heterodimer_scores)) - abs(np.max(heterodimer_scores))
-            }
-    
+             # 'weighted_score': product_size_weight * (1 - product_size_range) + heterodimer_score_weight * (1 - abs(np.mean(heterodimer_scores)) / 100)
+            }    
     return score, comb
 
 # Read the file into a pandas DataFrame
 file_path = args.region_file  # or 'file.xlsx'
 if file_path.endswith('.tsv'):
     df = pd.read_csv(file_path, sep='\t')
 else:
@@ -275,10 +287,14 @@
                     best_score = score
                     best_comb = comb
 
     print("")
     print("writing file: " + args.output + '.xlsx')
     # convert best_comb tuple to DataFrame object
     best_comb = pd.DataFrame(list(best_comb))
+    # add in NEB calc.
+    best_comb['Forward Primer TM NEB'] = best_comb['Forward Primer'].apply(q5_melting_temp)
+    best_comb['Reverse Primer TM NEB'] = best_comb['Reverse Primer'].apply(q5_melting_temp)
+
     best_comb.to_excel(args.output + '.xlsx', sheet_name='PrimerSet', index=False)
```

### Comparing `getMultiPrimerSet-1.0.1/getMultiPrimerSet.egg-info/PKG-INFO` & `getMultiPrimerSet-1.0.2/getMultiPrimerSet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getMultiPrimerSet
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for generating multiplex PCR primer sets
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `getMultiPrimerSet-1.0.1/setup.py` & `getMultiPrimerSet-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='getMultiPrimerSet',
-    version='1.0.1',
+    version='1.0.2',
     description='A package for generating multiplex PCR primer sets',
     author='Jason D Limberis',
     author_email='Jason.Limberis@ucsf.edu',
     long_description='''
 This program designs PCR primers for a multiplex of given target regions of a DNA sequence in a FASTA file.
 
 The script takes several arguments:
```

