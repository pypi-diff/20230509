# Comparing `tmp/nanomonsv-0.5.0b2.tar.gz` & `tmp/nanomonsv-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomonsv-0.5.0b2.tar", last modified: Fri Jun 24 10:10:50 2022, max compression
+gzip compressed data, was "nanomonsv-0.5.1.tar", last modified: Tue May  9 05:35:22 2023, max compression
```

## Comparing `nanomonsv-0.5.0b2.tar` & `nanomonsv-0.5.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 10:10:50.266979 nanomonsv-0.5.0b2/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14222 2022-06-24 10:10:50.266979 nanomonsv-0.5.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13504 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 10:10:50.262979 nanomonsv-0.5.0b2/nanomonsv/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9482 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    19901 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     8065 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/cluster_sbnd.py
--rw-r--r--   0 runner    (1001) docker     (121)    20284 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/count_sread_by_alignment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 10:10:50.266979 nanomonsv-0.5.0b2/nanomonsv/data/
--rw-r--r--   0 runner    (1001) docker     (121)   147053 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/data/LINE1.hg19.bed.gz
--rw-r--r--   0 runner    (1001) docker     (121)    79292 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/data/LINE1.hg19.bed.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (121)   152156 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/data/LINE1.hg38.bed.gz
--rw-r--r--   0 runner    (1001) docker     (121)    82867 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/data/LINE1.hg38.bed.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (121)    18301 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/filt.py
--rw-r--r--   0 runner    (1001) docker     (121)     7115 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/gather_support_read_seq.py
--rw-r--r--   0 runner    (1001) docker     (121)    15341 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/generate_consensus.py
--rw-r--r--   0 runner    (1001) docker     (121)    19718 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/identify.py
--rw-r--r--   0 runner    (1001) docker     (121)    27433 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/insert_classify.py
--rw-r--r--   0 runner    (1001) docker     (121)     4211 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/locate_bp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2420 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/locate_bp_sbnd.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)    23057 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/long_read_validate.py
--rw-r--r--   0 runner    (1001) docker     (121)     6921 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/merge_control.py
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/my_seq.py
--rw-r--r--   0 runner    (1001) docker     (121)    13279 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/parse.py
--rw-r--r--   0 runner    (1001) docker     (121)    16166 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/post_proc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15065 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/pyssw.py
--rw-r--r--   0 runner    (1001) docker     (121)    28149 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/smith_waterman.py
--rw-r--r--   0 runner    (1001) docker     (121)    11992 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/ssw_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)    19498 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/swalign.py
--rw-r--r--   0 runner    (1001) docker     (121)     3118 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7571 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/vcf_convert.py
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/nanomonsv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 10:10:50.262979 nanomonsv-0.5.0b2/nanomonsv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14222 2022-06-24 10:10:50.000000 nanomonsv-0.5.0b2/nanomonsv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-06-24 10:10:50.000000 nanomonsv-0.5.0b2/nanomonsv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 10:10:50.000000 nanomonsv-0.5.0b2/nanomonsv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-24 10:10:50.000000 nanomonsv-0.5.0b2/nanomonsv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-06-24 10:10:50.000000 nanomonsv-0.5.0b2/nanomonsv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-24 10:10:50.266979 nanomonsv-0.5.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-06-24 10:10:42.000000 nanomonsv-0.5.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:35:22.138529 nanomonsv-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-05-09 05:35:22.138529 nanomonsv-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:35:22.134528 nanomonsv-0.5.1/nanomonsv/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19901 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/cluster_sbnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20284 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/count_sread_by_alignment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:35:22.138529 nanomonsv-0.5.1/nanomonsv/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   147053 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/data/LINE1.hg19.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    79292 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/data/LINE1.hg19.bed.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (123)   152156 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/data/LINE1.hg38.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    82867 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/data/LINE1.hg38.bed.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/filt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/gather_support_read_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/generate_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/identify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27769 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/insert_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/locate_bp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/locate_bp_sbnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23057 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/long_read_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/merge_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/my_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16166 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/post_proc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15065 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/pyssw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28947 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/smith_waterman.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/ssw_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/swalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/vcf_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:35:22.138529 nanomonsv-0.5.1/nanomonsv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-05-09 05:35:22.000000 nanomonsv-0.5.1/nanomonsv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-09 05:35:22.000000 nanomonsv-0.5.1/nanomonsv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 05:35:22.000000 nanomonsv-0.5.1/nanomonsv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-09 05:35:22.000000 nanomonsv-0.5.1/nanomonsv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 05:35:22.000000 nanomonsv-0.5.1/nanomonsv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 05:35:22.138529 nanomonsv-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/setup.py
```

### Comparing `nanomonsv-0.5.0b2/LICENSE` & `nanomonsv-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/PKG-INFO` & `nanomonsv-0.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,57 @@
-Metadata-Version: 2.1
-Name: nanomonsv
-Version: 0.5.0b2
-Summary: Python tools for detecting structural variation from nanopore sequence data
-Home-page: https://github.com/friend1ws/nanomonsv
-Author: Yuichi Shiraishi
-Author-email: friend1ws@gamil.com
-License: GPLv3
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # nanomonsv
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Build Status](https://travis-ci.com/friend1ws/nanomonsv.svg?branch=master)](https://travis-ci.com/friend1ws/nanomonsv.svg?branch=master&status=started)
 
 ## Introduction
 
-nanomonsv is a software for detecting somatic structural variations　 from paired (tumor and matched control) cancer genome sequence data. nanomonsv is presented in the following preprint. **When you use nanomonsv or any resource of this repository, please kindly site this preprint**.
+nanomonsv is a software for detecting somatic structural variations from paired (tumor and matched control) cancer genome sequence data. nanomonsv is presented in the following preprint. **When you use nanomonsv or any resource of this repository, please kindly site this preprint**.
+
+Precise characterization of somatic complex structural variations from paired long-read sequencing data with nanomonsv, Shiraishi et al., bioRxiv, 2020, [[link]](https://www.biorxiv.org/content/10.1101/2020.07.22.214262v3).
 
-Precise characterization of somatic structural variations and mobile element insertions from paired long-read sequencing data with nanomonsv, Shiraishi et al., bioRxiv, 2020, [[link]](https://www.biorxiv.org/content/10.1101/2020.07.22.214262v1)
+The current version of nanomonsv includes two detection modules, Canonical SV module, and [Single breakend SV module](https://github.com/friend1ws/nanomonsv/wiki/Single-breakend-SV). Canonical SV module can identify somatic SVs that can be captured by short-read technologies with higher precision and recall than existing methods. Furthermore, Single breakend SV module enables the detection of complex SVs that can only be identified by long-reads, such as SVs involving highly-repetitive centromeric sequences, and LINE1- and virus-mediated rearrangements. 
+
+Please see the [wiki page](https://github.com/friend1ws/nanomonsv/wiki/Single-breakend-SV) for Single breakend SV module.
 
 ## Dependency
 
 ### For basic use (`parse`, `get` command)
 
 ### Binary programs
 
 [htslib](http://www.htslib.org/), [mafft](https://mafft.cbrc.jp/alignment/software/), [racon](https://github.com/isovic/racon)(optional from ver. 0.3.0. However, we recommend to use this option. Add --use_racon option when you perfrom get command.)
 
 ### Python
-Pytnon (tested with >=3.6), pysam, numpy, parasail
+Python (tested with >=3.6), pysam, numpy, parasail
 
 > [SSW Library](https://github.com/mengyao/Complete-Striped-Smith-Waterman-Library) (This became optional since version 0.2.0. We have changed the main engine of Smith-Waterman algorithm to parasail.)
 
 
 ### For advanced use (`insert_classify` command)
 [bwa](https://github.com/lh3/bwa), [minimap2](https://github.com/lh3/minimap2), [bedtools](https://bedtools.readthedocs.io/en/latest/), [RepeatMasker](http://www.repeatmasker.org/)
 
 ## Preparation
 
 ### For basic use (`parse`, `get` command)
 
 #### Install software and add them to the PATH
 
-nanomonsv uses, `tabix`, `bgzip` (which ar part of HTSlib projects) and `mafft` inside the program,
+nanomonsv uses, `tabix`, `bgzip` (which are part of HTSlib projects) and `mafft` inside the program,
 assuming those are installed, and the paths are already added to the running environment.
 
 > ##### For use of SSW Library
 > Since version 0.2.0, nanomonsv can be executed without SSW Library. When users want to use SSW Library, create the libssw.so and add the path to the LD_LIBRARY_PATH environment variable. Please refer the **How to use the Python wrapper ssw_lib.py** section in the [SSW Library](https://github.com/mengyao/Complete-Striped-Smith-Waterman-Library) repository page.
 
 ###### For use of racon
 Since version 0.3.0, we support racon for the step where generating consensus sequence and get single-base resolution breakpoints. racon may become the default instead of mafft in the future.
 
 
 ### For advanced use (`insert_classify` command)
-`bwa`, `minimap2`, `bedtools` and `RepeatMasker` are required to be installed and these pathese are added to the running environment.
+`bwa`, `minimap2`, `bedtools` and `RepeatMasker` are required to be installed and these paths are added to the running environment.
 
 
 ### Input file
 
 nanomonsv accept the BAM file aligned by `minimap2`. 
 
 
@@ -74,32 +59,33 @@
 Starting with version 0.5.0, the use of the control panel is supported. 
 In this software, supporting reads for SVs are collected for multiple samples other than the target sample, 
 and such reads are removed as common noise (or those derived from common SVs) in the `get` stage. 
 This strategy is expected to exclude many false positives as well as improve computational cost.
 
 We have prepared the command to create control panels from the user's own sequencing data.
 In addition, for users who do not have sufficient sequencing data that can serve as a control panel (or just do not have time for processing), 
-we prepared a control panel that has been created using the 30 Nanopore sequencing data from the [Human Pangenome Reference Consortium](https://humanpangenome.org/),
-which you can download by the following command:
-
-```
-wget https://ncc-gap-pub.s3.ap-northeast-1.amazonaws.com/nanomonsv/control_panel/hprc_year1_data_freeze_nanopore_minimap2_2_24_merge_control.tar.gz
-```
+we prepared a control panel that has been created using the 30 Nanopore sequencing data from the [Human Pangenome Reference Consortium](https://humanpangenome.org/), which is available at [zenodo](https://zenodo.org/record/7017953).
 
 This control panel is made by aligning 30 Nanopore sequencing data to the GRCh38 reference genome (obtained from [here](https://console.cloud.google.com/storage/browser/genomics-public-data/resources/broad/hg38/v0;tab=objects)) with minimap2 version 2.24. 
 **When you use these control panels and publish, do not forget to credit to [HPRC](https://github.com/human-pangenomics/HG002_Data_Freeze_v1.0#citations)!**
 
 
 ## Quickstart
 
 1. Install all the prerequisite software and install nanomonsv.
 ```
 pip install nanomonsv (--user)
 ```
 
+You can also install nanomonsv via conda (bioconda channel).
+```
+conda create -n nanomonsv -c conda-forge -c bioconda nanomonsv
+```
+Occasionally the conda releases lag behind the source code and PyPI releases.
+
 2. Prepare the reference genome for the test data (here, we show the path to Genomic Data Commons reference genome).
 ```
 wget https://api.gdc.cancer.gov/data/254f697d-310d-4d7d-a27b-27fbf767a834 -O GRCh38.d1.vd1.fa.tar.gz
 tar xvf GRCh38.d1.vd1.fa.tar.gz
 ```
 
 3. Parse the putative structural variation supporting reads of the test data.
@@ -122,14 +108,16 @@
 - H2009: [tumor](https://www.ncbi.nlm.nih.gov/sra/DRX248308[accn]), [control](https://www.ncbi.nlm.nih.gov/sra/DRX248309[accn])
 - HCC1954: [tumor](https://www.ncbi.nlm.nih.gov/sra/DRX248306[accn]), [control](https://www.ncbi.nlm.nih.gov/sra/DRX248307[accn])
 
 The results of nanomonsv for the above data are available [here](https://github.com/friend1ws/nanomonsv/tree/master/misc/example).
 When you perform nanomonsv to the above data and have experienced errors, please report to us.
 Also, please kindly cite the [bioRxiv paper](https://www.biorxiv.org/content/10.1101/2020.07.22.214262v1) when you use these data.
 
+See tutorial [wiki page](https://github.com/friend1ws/nanomonsv/wiki/Tutorial) for an example workflow on analyzing COLO829 sample.
+
 ## Commands
 
 ### parse
 
 This step parses all the supporting reads of putative somatic SVs.
 
 ```
@@ -158,16 +146,16 @@
               [--min_tumor_VAF MIN_TUMOR_VAF]
               [--max_control_variant_read_num MAX_CONTROL_VARIANT_READ_NUM]
               [--max_control_VAF MAX_CONTROL_VAF]
               [--cluster_margin_size CLUSTER_MARGIN_SIZE]
               [--median_mapQ_thres MEDIAN_MAPQ_THRES]
               [--max_overhang_size_thres MAX_OVERHANG_SIZE_THRES]
               [--var_read_min_mapq VAR_READ_MIN_MAPQ] [--use_ssw_lib] [--use_racon]
-              [--threads THREADS] [--processes PROCESSES] 
-              [--sort_option SORT_OPTION] [--debug]
+              [--single_bnd] [--threads THREADS] [--processes PROCESSES] 
+              [--sort_option SORT_OPTION] [--max_memory_minimap2] [--debug]
               tumor_prefix tumor_bam reference.fa
  ```
  - **tumor_prefix**: Prefix to the tumor data set in the parse step
  - **tumor_bam**: Path to input indexed BAM file
  - **reference.fa**: Path to reference genome used for the alignment
  
 This software can generate a list of SVs without specifying the matched control.
@@ -175,26 +163,32 @@
 Even when only tumor sample is available, we still recommend using dummy control sample (collected from other person's tissue).
 - **control_prefix**: Prefix to the matched control data set in the parse step
 - **control_bam**: Path to the matched control BAM file
 
 When you use the control panel (recommended!), use the following argument.
 - **control_panel_prefix**: Prefix of non-matched control panel data processed in merge_control step.
 
+You can also use **--process** to use multi-processing mode. Currently, we do not recommend using **--thread** option.
+
 After successful execution, you will be able to find the result file names as {tumor_prefix}.nanomonsv.result.txt.
 See the help (`nanomonsv get -h`) for other options. 
 
 When you want to change the engine of Smith-Waterman algorithm to SSW Library, specify `--use_ssw_lib` option,
 though we do not generally recommend this.
 
 Also, we basically recommend using `--use_racon` option. This will slightly improve the identification of single-base resolution breakpoint, 
 and polishing of inserted sequences. 
 
+For detection of single breakend SVs, please use `--single_bnd` option as well as `--use_racon`. 
+Please see [wiki page](https://github.com/friend1ws/nanomonsv/wiki/Single-breakend-SV).
+
 Also, we have prepared the script (misc/post_fileter.py) for filtering the result.
 Please see the [wiki page](https://github.com/friend1ws/nanomonsv/wiki/How-to-filter-nanomonsv-result).
 For output files of the version 0.4.0 and later, some filtering has already been performed (see the [wiki page](https://github.com/friend1ws/nanomonsv/wiki/How-to-understand-nanomonsv-result-filtering)). 
+However, we strongly recommed to perform additional processing; removing indels within simple repeat regions (see the [wiki page](https://github.com/friend1ws/nanomonsv/wiki/An-example-on-removing-indels-within-simple-repeat)).
 
 From the version 0.4.0, we will also provide the VCF format result files.
 
 #### result
 
 * **Chr_1**: Chromosome for the 1st breakpoint
 * **Pos_1**: Coordinate for the 1st breakpoint
@@ -269,9 +263,7 @@
                    [--var_read_min_mapq VAR_READ_MIN_MAPQ] [--debug]
                    sv_list_file tumor_bam output reference.fa
 ```
 - **sv_list_file**: SV candidate list file (similar format with the result file by `get` command. 
 But only from **Chr_1** to **Inserted_Seq** columns are necessary.
 - **output_file**: Path to the output file
 - **reference.fa**: Path to the reference genome                          
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nanomonsv-0.5.0b2/README.md` & `nanomonsv-0.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,75 @@
+Metadata-Version: 2.1
+Name: nanomonsv
+Version: 0.5.1
+Summary: Python tools for detecting structural variation from nanopore sequence data
+Home-page: https://github.com/friend1ws/nanomonsv
+Author: Yuichi Shiraishi
+Author-email: friend1ws@gamil.com
+License: GPLv3
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # nanomonsv
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Build Status](https://travis-ci.com/friend1ws/nanomonsv.svg?branch=master)](https://travis-ci.com/friend1ws/nanomonsv.svg?branch=master&status=started)
 
 ## Introduction
 
-nanomonsv is a software for detecting somatic structural variations　 from paired (tumor and matched control) cancer genome sequence data. nanomonsv is presented in the following preprint. **When you use nanomonsv or any resource of this repository, please kindly site this preprint**.
+nanomonsv is a software for detecting somatic structural variations from paired (tumor and matched control) cancer genome sequence data. nanomonsv is presented in the following preprint. **When you use nanomonsv or any resource of this repository, please kindly site this preprint**.
+
+Precise characterization of somatic complex structural variations from paired long-read sequencing data with nanomonsv, Shiraishi et al., bioRxiv, 2020, [[link]](https://www.biorxiv.org/content/10.1101/2020.07.22.214262v3).
+
+The current version of nanomonsv includes two detection modules, Canonical SV module, and [Single breakend SV module](https://github.com/friend1ws/nanomonsv/wiki/Single-breakend-SV). Canonical SV module can identify somatic SVs that can be captured by short-read technologies with higher precision and recall than existing methods. Furthermore, Single breakend SV module enables the detection of complex SVs that can only be identified by long-reads, such as SVs involving highly-repetitive centromeric sequences, and LINE1- and virus-mediated rearrangements. 
 
-Precise characterization of somatic structural variations and mobile element insertions from paired long-read sequencing data with nanomonsv, Shiraishi et al., bioRxiv, 2020, [[link]](https://www.biorxiv.org/content/10.1101/2020.07.22.214262v1)
+Please see the [wiki page](https://github.com/friend1ws/nanomonsv/wiki/Single-breakend-SV) for Single breakend SV module.
 
 ## Dependency
 
 ### For basic use (`parse`, `get` command)
 
 ### Binary programs
 
 [htslib](http://www.htslib.org/), [mafft](https://mafft.cbrc.jp/alignment/software/), [racon](https://github.com/isovic/racon)(optional from ver. 0.3.0. However, we recommend to use this option. Add --use_racon option when you perfrom get command.)
 
 ### Python
-Pytnon (tested with >=3.6), pysam, numpy, parasail
+Python (tested with >=3.6), pysam, numpy, parasail
 
 > [SSW Library](https://github.com/mengyao/Complete-Striped-Smith-Waterman-Library) (This became optional since version 0.2.0. We have changed the main engine of Smith-Waterman algorithm to parasail.)
 
 
 ### For advanced use (`insert_classify` command)
 [bwa](https://github.com/lh3/bwa), [minimap2](https://github.com/lh3/minimap2), [bedtools](https://bedtools.readthedocs.io/en/latest/), [RepeatMasker](http://www.repeatmasker.org/)
 
 ## Preparation
 
 ### For basic use (`parse`, `get` command)
 
 #### Install software and add them to the PATH
 
-nanomonsv uses, `tabix`, `bgzip` (which ar part of HTSlib projects) and `mafft` inside the program,
+nanomonsv uses, `tabix`, `bgzip` (which are part of HTSlib projects) and `mafft` inside the program,
 assuming those are installed, and the paths are already added to the running environment.
 
 > ##### For use of SSW Library
 > Since version 0.2.0, nanomonsv can be executed without SSW Library. When users want to use SSW Library, create the libssw.so and add the path to the LD_LIBRARY_PATH environment variable. Please refer the **How to use the Python wrapper ssw_lib.py** section in the [SSW Library](https://github.com/mengyao/Complete-Striped-Smith-Waterman-Library) repository page.
 
 ###### For use of racon
 Since version 0.3.0, we support racon for the step where generating consensus sequence and get single-base resolution breakpoints. racon may become the default instead of mafft in the future.
 
 
 ### For advanced use (`insert_classify` command)
-`bwa`, `minimap2`, `bedtools` and `RepeatMasker` are required to be installed and these pathese are added to the running environment.
+`bwa`, `minimap2`, `bedtools` and `RepeatMasker` are required to be installed and these paths are added to the running environment.
 
 
 ### Input file
 
 nanomonsv accept the BAM file aligned by `minimap2`. 
 
 
@@ -55,32 +77,33 @@
 Starting with version 0.5.0, the use of the control panel is supported. 
 In this software, supporting reads for SVs are collected for multiple samples other than the target sample, 
 and such reads are removed as common noise (or those derived from common SVs) in the `get` stage. 
 This strategy is expected to exclude many false positives as well as improve computational cost.
 
 We have prepared the command to create control panels from the user's own sequencing data.
 In addition, for users who do not have sufficient sequencing data that can serve as a control panel (or just do not have time for processing), 
-we prepared a control panel that has been created using the 30 Nanopore sequencing data from the [Human Pangenome Reference Consortium](https://humanpangenome.org/),
-which you can download by the following command:
-
-```
-wget https://ncc-gap-pub.s3.ap-northeast-1.amazonaws.com/nanomonsv/control_panel/hprc_year1_data_freeze_nanopore_minimap2_2_24_merge_control.tar.gz
-```
+we prepared a control panel that has been created using the 30 Nanopore sequencing data from the [Human Pangenome Reference Consortium](https://humanpangenome.org/), which is available at [zenodo](https://zenodo.org/record/7017953).
 
 This control panel is made by aligning 30 Nanopore sequencing data to the GRCh38 reference genome (obtained from [here](https://console.cloud.google.com/storage/browser/genomics-public-data/resources/broad/hg38/v0;tab=objects)) with minimap2 version 2.24. 
 **When you use these control panels and publish, do not forget to credit to [HPRC](https://github.com/human-pangenomics/HG002_Data_Freeze_v1.0#citations)!**
 
 
 ## Quickstart
 
 1. Install all the prerequisite software and install nanomonsv.
 ```
 pip install nanomonsv (--user)
 ```
 
+You can also install nanomonsv via conda (bioconda channel).
+```
+conda create -n nanomonsv -c conda-forge -c bioconda nanomonsv
+```
+Occasionally the conda releases lag behind the source code and PyPI releases.
+
 2. Prepare the reference genome for the test data (here, we show the path to Genomic Data Commons reference genome).
 ```
 wget https://api.gdc.cancer.gov/data/254f697d-310d-4d7d-a27b-27fbf767a834 -O GRCh38.d1.vd1.fa.tar.gz
 tar xvf GRCh38.d1.vd1.fa.tar.gz
 ```
 
 3. Parse the putative structural variation supporting reads of the test data.
@@ -103,14 +126,16 @@
 - H2009: [tumor](https://www.ncbi.nlm.nih.gov/sra/DRX248308[accn]), [control](https://www.ncbi.nlm.nih.gov/sra/DRX248309[accn])
 - HCC1954: [tumor](https://www.ncbi.nlm.nih.gov/sra/DRX248306[accn]), [control](https://www.ncbi.nlm.nih.gov/sra/DRX248307[accn])
 
 The results of nanomonsv for the above data are available [here](https://github.com/friend1ws/nanomonsv/tree/master/misc/example).
 When you perform nanomonsv to the above data and have experienced errors, please report to us.
 Also, please kindly cite the [bioRxiv paper](https://www.biorxiv.org/content/10.1101/2020.07.22.214262v1) when you use these data.
 
+See tutorial [wiki page](https://github.com/friend1ws/nanomonsv/wiki/Tutorial) for an example workflow on analyzing COLO829 sample.
+
 ## Commands
 
 ### parse
 
 This step parses all the supporting reads of putative somatic SVs.
 
 ```
@@ -139,16 +164,16 @@
               [--min_tumor_VAF MIN_TUMOR_VAF]
               [--max_control_variant_read_num MAX_CONTROL_VARIANT_READ_NUM]
               [--max_control_VAF MAX_CONTROL_VAF]
               [--cluster_margin_size CLUSTER_MARGIN_SIZE]
               [--median_mapQ_thres MEDIAN_MAPQ_THRES]
               [--max_overhang_size_thres MAX_OVERHANG_SIZE_THRES]
               [--var_read_min_mapq VAR_READ_MIN_MAPQ] [--use_ssw_lib] [--use_racon]
-              [--threads THREADS] [--processes PROCESSES] 
-              [--sort_option SORT_OPTION] [--debug]
+              [--single_bnd] [--threads THREADS] [--processes PROCESSES] 
+              [--sort_option SORT_OPTION] [--max_memory_minimap2] [--debug]
               tumor_prefix tumor_bam reference.fa
  ```
  - **tumor_prefix**: Prefix to the tumor data set in the parse step
  - **tumor_bam**: Path to input indexed BAM file
  - **reference.fa**: Path to reference genome used for the alignment
  
 This software can generate a list of SVs without specifying the matched control.
@@ -156,26 +181,32 @@
 Even when only tumor sample is available, we still recommend using dummy control sample (collected from other person's tissue).
 - **control_prefix**: Prefix to the matched control data set in the parse step
 - **control_bam**: Path to the matched control BAM file
 
 When you use the control panel (recommended!), use the following argument.
 - **control_panel_prefix**: Prefix of non-matched control panel data processed in merge_control step.
 
+You can also use **--process** to use multi-processing mode. Currently, we do not recommend using **--thread** option.
+
 After successful execution, you will be able to find the result file names as {tumor_prefix}.nanomonsv.result.txt.
 See the help (`nanomonsv get -h`) for other options. 
 
 When you want to change the engine of Smith-Waterman algorithm to SSW Library, specify `--use_ssw_lib` option,
 though we do not generally recommend this.
 
 Also, we basically recommend using `--use_racon` option. This will slightly improve the identification of single-base resolution breakpoint, 
 and polishing of inserted sequences. 
 
+For detection of single breakend SVs, please use `--single_bnd` option as well as `--use_racon`. 
+Please see [wiki page](https://github.com/friend1ws/nanomonsv/wiki/Single-breakend-SV).
+
 Also, we have prepared the script (misc/post_fileter.py) for filtering the result.
 Please see the [wiki page](https://github.com/friend1ws/nanomonsv/wiki/How-to-filter-nanomonsv-result).
 For output files of the version 0.4.0 and later, some filtering has already been performed (see the [wiki page](https://github.com/friend1ws/nanomonsv/wiki/How-to-understand-nanomonsv-result-filtering)). 
+However, we strongly recommed to perform additional processing; removing indels within simple repeat regions (see the [wiki page](https://github.com/friend1ws/nanomonsv/wiki/An-example-on-removing-indels-within-simple-repeat)).
 
 From the version 0.4.0, we will also provide the VCF format result files.
 
 #### result
 
 * **Chr_1**: Chromosome for the 1st breakpoint
 * **Pos_1**: Coordinate for the 1st breakpoint
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nanomonsv-0.5.0b2/nanomonsv/arg_parser.py` & `nanomonsv-0.5.1/nanomonsv/arg_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,17 @@
 
     get.add_argument("--processes", default = 1, type = int,
                      help = "Number of parallel processes to use (default: 1)")
 
     get.add_argument("--sort_option", metavar = "-S 1G", type = str, default = "-S 1G", 
                      help = "Options for Linux sort command (default: '-S 1G')")
 
+    get.add_argument("--max_memory_minimap2", metavar = 1, type = int, default = 1, 
+                     help = "Maximum memory size (Gbyte) for minimap2 (default: 1)")
+
     get.add_argument("--debug", default = False, action = 'store_true', help = "keep intermediate files (default: False)")
 
     get.set_defaults(func = get_main)
     ##########
 
     ##########
     # validate
```

### Comparing `nanomonsv-0.5.0b2/nanomonsv/cluster.py` & `nanomonsv-0.5.1/nanomonsv/cluster.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/cluster_sbnd.py` & `nanomonsv-0.5.1/nanomonsv/cluster_sbnd.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/count_sread_by_alignment.py` & `nanomonsv-0.5.1/nanomonsv/count_sread_by_alignment.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/data/LINE1.hg19.bed.gz` & `nanomonsv-0.5.1/nanomonsv/data/LINE1.hg19.bed.gz`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/data/LINE1.hg19.bed.gz.tbi` & `nanomonsv-0.5.1/nanomonsv/data/LINE1.hg19.bed.gz.tbi`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/data/LINE1.hg38.bed.gz` & `nanomonsv-0.5.1/nanomonsv/data/LINE1.hg38.bed.gz`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/data/LINE1.hg38.bed.gz.tbi` & `nanomonsv-0.5.1/nanomonsv/data/LINE1.hg38.bed.gz.tbi`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/filt.py` & `nanomonsv-0.5.1/nanomonsv/filt.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/gather_support_read_seq.py` & `nanomonsv-0.5.1/nanomonsv/gather_support_read_seq.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/generate_consensus.py` & `nanomonsv-0.5.1/nanomonsv/generate_consensus.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #! /usr/bin/env python3
 
 import sys, os, subprocess, shutil, statistics, logging
 from collections import Counter
 import pysam
 import parasail
+import resource
 
 from .logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class Consensus_generator(object):
 
-    def __init__(self, output_file, use_racon, debug):
+    def __init__(self, output_file, use_racon, debug, max_memory_minimap2):
 
         self.tmp_dir = output_file + ".tmp_dir"
         os.makedirs(self.tmp_dir, exist_ok = True)
 
         self.hout = open(output_file, 'w')
         self.temp_key = None 
         self.readid2is_bp = {}
@@ -24,14 +25,15 @@
         self.use_racon = False if use_racon == False else True
         self.debug = debug
         self.parasail_error = []
 
         self.start_margin = 120
         self.min_inclusion_ratio = 0.9
         self.min_inclusion_count = 3
+        self.max_memory_minimap2 = max_memory_minimap2
 
     def __del__(self):
         self.hout.close()
         if len(self.parasail_error) > 0:
             logger.debug(f"Alignment by parasail failed in {self.parasail_error}")
 
         if not self.debug:
@@ -198,24 +200,30 @@
 
         if self.temp_support_read_file_h is not None: self.temp_support_read_file_h.close()
         if self.use_racon:
             self.print_consensus_racon()
         else:
             self.print_consensus_mafft()
 
+    def preexec_fn(self):
+        limit = self.max_memory_minimap2 * 1024 ** 3
+        if "RLIMIT_AS" in resource.__dict__:
+            resource.setrlimit(resource.RLIMIT_AS, (limit, limit))
+        elif "RLIMIT_VMEM" in resource.__dict__:
+            resource.setrlimit(resource.RLIMIT_VMEM, (limit, limit))
 
     def print_consensus_sbnd(self):
 
         if self.temp_support_read_file_h is not None: self.temp_support_read_file_h.close()
 
         with open(self.tmp_dir + '/' + self.temp_key + "_ava_minimap2.paf", 'w') as hout:
             subprocess.check_call(["minimap2", "-x", "ava-ont", 
                 self.tmp_dir + '/' + self.temp_key + ".supporting_read.fa",
                 self.tmp_dir + '/' + self.temp_key + ".supporting_read.fa"],
-                stderr = subprocess.DEVNULL, stdout = hout)
+                stderr = subprocess.DEVNULL, stdout = hout, preexec_fn = self.preexec_fn)
 
         readid2inclusion_count = {}
         with open(self.tmp_dir + '/' + self.temp_key + "_ava_minimap2.paf") as hin:
             for line in hin:
                 row = line.rstrip('\n').split('\t')
                 if int(row[2]) <= self.start_margin and (float(row[3]) - float(row[2])) / float(row[1]) >= self.min_inclusion_ratio:
                     if row[5] not in readid2inclusion_count: readid2inclusion_count[row[5]] = 0
@@ -242,15 +250,15 @@
                 if tid == '' or seq_read_count > 10000: 
                     logger.warning(f"Something inconsistent happend when choosing template reads for {self.temp_key}")
                     return
 
         with open(self.tmp_dir + '/' + self.temp_key + "_ova_minimap2.paf", 'w') as hout:
             subprocess.check_call(["minimap2", "-x", "map-ont", self.tmp_dir + '/' + self.temp_key + "_ref.fa",
                 self.tmp_dir + '/' + self.temp_key + ".supporting_read.fa"], 
-                stderr = subprocess.DEVNULL, stdout = hout)
+                stderr = subprocess.DEVNULL, stdout = hout, preexec_fn = self.preexec_fn)
 
         paf_rec_count = 0
         with open(self.tmp_dir + '/' + self.temp_key + "_ova_minimap2.paf", 'r') as hin:
             for line in hin:
                 paf_rec_count = paf_rec_count + 1
 
         if paf_rec_count < 3:
@@ -278,15 +286,15 @@
         # second round racon
         with open(self.tmp_dir + '/' + self.temp_key + "_ref_2nd.fa", 'w') as hout:
             print(f">{self.temp_key}_1st_polished_seq\n{consensus}", file = hout)
 
         with open(self.tmp_dir + '/' + self.temp_key + "_ova_minimap2_2nd.paf", 'w') as hout:
             subprocess.check_call(["minimap2", "-x", "map-ont", self.tmp_dir + '/' + self.temp_key + "_ref_2nd.fa",
                 self.tmp_dir + '/' + self.temp_key + ".supporting_read.fa"],
-                stderr = subprocess.DEVNULL, stdout = hout)
+                stderr = subprocess.DEVNULL, stdout = hout, preexec_fn = self.preexec_fn)
 
         paf_rec_count = 0
         with open(self.tmp_dir + '/' + self.temp_key + "_ova_minimap2_2nd.paf", 'r') as hin:
             for line in hin:
                 paf_rec_count = paf_rec_count + 1
             
         if paf_rec_count < 3:
@@ -309,19 +317,19 @@
                 if line.startswith('>'): continue
                 consensus = consensus + line.rstrip('\n')
 
         print(f"{self.temp_key}\t{consensus}", file = self.hout)
 
 
 
-def generate_consensus(input_file, output_file, use_racon = False, debug = False): 
+def generate_consensus(input_file, output_file, use_racon = False, debug = False, max_memory_minimap2 = 1): 
 
     if debug: logger.setLevel(logging.DEBUG)
 
-    consensus_generator = Consensus_generator(output_file, use_racon, debug)
+    consensus_generator = Consensus_generator(output_file, use_racon, debug, max_memory_minimap2)
         
     with open(input_file, 'r') as hin:
         for line in hin:
             tkey, treadid, tsize, tseq = line.rstrip('\n').split('\t')
             # when new key appears transaction            
             if tkey != consensus_generator.temp_key:
                 if consensus_generator.temp_key is not None:
@@ -332,20 +340,20 @@
 
         if consensus_generator.temp_key is not None:
             consensus_generator.print_consensus()
 
     del consensus_generator 
 
 
-def generate_consensus_sbnd(input_file, output_file, use_racon = False, debug = False):
+def generate_consensus_sbnd(input_file, output_file, use_racon = False, debug = False, max_memory_minimap2 = 1):
 
     if debug: logger.setLevel(logging.DEBUG)
 
     # generate contig for single breakend
-    consensus_generator_sbnd = Consensus_generator(output_file, use_racon, debug)
+    consensus_generator_sbnd = Consensus_generator(output_file, use_racon, debug, max_memory_minimap2)
     with open(input_file, 'r') as hin:
         for line in hin:
             tkey, treadid, tsize, tseq = line.rstrip('\n').split('\t')
             # when new key appears transaction            
             if tkey != consensus_generator_sbnd.temp_key:
                 if consensus_generator_sbnd.temp_key is not None:
                     consensus_generator_sbnd.print_consensus_sbnd()
```

### Comparing `nanomonsv-0.5.0b2/nanomonsv/identify.py` & `nanomonsv-0.5.1/nanomonsv/identify.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/insert_classify.py` & `nanomonsv-0.5.1/nanomonsv/insert_classify.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,22 +298,22 @@
             if seq.startswith('TTTTTTTTTT') or match1 is not None: is_polyT = True
             if seq.endswith('AAAAAAAAAA') or match2 is not None: is_polyA = True
 
 
             tsd_cand1 = seq[:20]
             local_seq1 = get_seq(reference, tchr, int(tpos2), int(tpos2) + len(tsd_cand1))
             alignment1 = sw.align(tsd_cand1, local_seq1)
-            if alignment1.q_pos <= 2 and alignment1.matches >= 5 and alignment1.identity >= 0.8: 
+            if alignment1.q_pos <= 2 and alignment1.r_pos <= 2 and alignment1.matches >= 5 and alignment1.identity >= 0.8: 
                 tsd1 = alignment1.query[(alignment1.q_pos):(alignment1.q_pos + alignment1.matches)]  
 
 
             tsd_cand2 = reverse_complement(seq[-20:])
             local_seq2 = reverse_complement(get_seq(reference, tchr, int(tpos1) - len(tsd_cand2), int(tpos1)))
             alignment2 = sw.align(tsd_cand2, local_seq2)
-            if alignment2.q_pos <= 2 and alignment2.matches >= 5 and alignment2.identity >= 0.8: 
+            if alignment2.q_pos <= 2 and alignment2.r_pos <= 2 and alignment2.matches >= 5 and alignment2.identity >= 0.8: 
                 tsd2 = reverse_complement(alignment2.query[(alignment2.q_pos):(alignment2.q_pos + alignment2.matches)])
 
             if tsd1 is not None and tsd2 is None: 
                 tsd = tsd1
             elif tsd1 is None and tsd2 is not None:
                 tsd = tsd2
             elif tsd1 is not None and tsd2 is not None:
@@ -321,15 +321,16 @@
             else:
                 tsd = None
 
             polyAT = None
             if is_polyT: polyAT = "polyT"
             if is_polyA: polyAT = "polyA"
 
-            print(sid + '\t' + str(polyAT) + '\t' + str(tsd) + '\t' + tsd_cand1 + '\t' + local_seq1 + '\t' + tsd_cand2 + '\t' + local_seq2, file = hout) 
+            # print(sid + '\t' + str(polyAT) + '\t' + str(tsd) + '\t' + tsd_cand1 + '\t' + local_seq1 + '\t' + tsd_cand2 + '\t' + local_seq2, file = hout) 
+            print(f'{sid}\t{polyAT}\t{tsd}\t{tsd_cand1}\t{local_seq1}\t{alignment1.q_pos}\t{alignment1.r_pos}\t{alignment1.matches}\t{alignment1.identity}\t{tsd_cand2}\t{local_seq2}\t{alignment2.q_pos}\t{alignment2.r_pos}\t{alignment2.matches}\t{alignment2.identity}', file = hout)
 
 
 
 def summarize_bwa_alignment(input_sam, seq_list, output_file):
 
     samfile = pysam.AlignmentFile(input_sam, 'r')
```

### Comparing `nanomonsv-0.5.0b2/nanomonsv/locate_bp.py` & `nanomonsv-0.5.1/nanomonsv/locate_bp.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/locate_bp_sbnd.py` & `nanomonsv-0.5.1/nanomonsv/locate_bp_sbnd.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/long_read_validate.py` & `nanomonsv-0.5.1/nanomonsv/long_read_validate.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/merge_control.py` & `nanomonsv-0.5.1/nanomonsv/merge_control.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/my_seq.py` & `nanomonsv-0.5.1/nanomonsv/my_seq.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/parse.py` & `nanomonsv-0.5.1/nanomonsv/parse.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/post_proc.py` & `nanomonsv-0.5.1/nanomonsv/post_proc.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/pyssw.py` & `nanomonsv-0.5.1/nanomonsv/pyssw.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/run.py` & `nanomonsv-0.5.1/nanomonsv/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,61 +118,70 @@
 
 def merge_control_main(args):
 
     merge_control_from_parse_files(args.prefix_list_file, args.output_prefix)
 
 
 def call_slow_request(args, index):
-    logger.info("Generate consensus sequences (%d)" % (index))
-    generate_consensus(args.tumor_prefix + ".support_read_seq.%d.txt" % (index),
-        args.tumor_prefix + ".consensus_seq.%d.txt" % (index),
-        use_racon = args.use_racon, debug = args.debug)
-    generate_consensus_sbnd(args.tumor_prefix + ".support_read_seq.sbnd.%d.txt" % (index),
-        args.tumor_prefix + ".consensus_seq.sbnd.%d.txt" % (index),
-        use_racon = args.use_racon, debug = args.debug)
-
-    logger.info("Locating single-base resolution break points for candidate SVs (%d)" % (index))
-    locate_bp(args.tumor_prefix + ".consensus_seq.%d.txt" % (index),
-        args.tumor_prefix + ".refined_bp.%d.txt" % (index),
-        args.reference_fasta, args.debug)
-    locate_bp_sbnd(args.tumor_prefix + ".consensus_seq.sbnd.%d.txt" % (index),
-        args.tumor_prefix + ".refined_bp.sbnd.%d.txt" % (index),
-        args.reference_fasta, args.debug)
-
-    logger.info("Counting the number of supprting read for the tumor by realignment of SV candidate segments (%d)" % (index))
-    count_sread_by_alignment(
-        args.tumor_prefix + ".refined_bp.%d.txt" % (index), 
-        args.tumor_bam, 
-        args.tumor_prefix + ".realignment.tumor.sread_count.%d.txt" % (index), 
-        args.tumor_prefix + ".realignment.tumor.sread_info.%d.txt" % (index), 
-        args.reference_fasta,
-        sbnd_file = args.tumor_prefix + ".refined_bp.sbnd.%d.txt" % (index), 
-        output_count_file_sbnd = args.tumor_prefix + ".realignment.tumor.sread_count.sbnd.%d.txt" % (index),
-        output_alignment_info_file_sbnd = args.tumor_prefix + ".realignment.tumor.sread_info.sbnd.%d.txt" % (index),
-        check_read_max_num = args.check_read_max_num, 
-        var_read_min_mapq = args.var_read_min_mapq, use_ssw_lib = args.use_ssw_lib, 
-        sort_option = args.sort_option, debug = args.debug
-    )
- 
-    if args.control_bam is not None:
-        logger.info("Counting the number of supprting read for the control by realignment of SV candidate segments (%d)" % (index))
+    ret_code = 1
+    err_message = ""
+    try:
+        logger.info("Generate consensus sequences (%d)" % (index))
+        generate_consensus(args.tumor_prefix + ".support_read_seq.%d.txt" % (index),
+            args.tumor_prefix + ".consensus_seq.%d.txt" % (index),
+            use_racon = args.use_racon, debug = args.debug)
+        generate_consensus_sbnd(args.tumor_prefix + ".support_read_seq.sbnd.%d.txt" % (index),
+            args.tumor_prefix + ".consensus_seq.sbnd.%d.txt" % (index),
+            use_racon = args.use_racon, debug = args.debug, max_memory_minimap2 = args.max_memory_minimap2)
+
+        logger.info("Locating single-base resolution break points for candidate SVs (%d)" % (index))
+        locate_bp(args.tumor_prefix + ".consensus_seq.%d.txt" % (index),
+            args.tumor_prefix + ".refined_bp.%d.txt" % (index),
+            args.reference_fasta, args.debug)
+        locate_bp_sbnd(args.tumor_prefix + ".consensus_seq.sbnd.%d.txt" % (index),
+            args.tumor_prefix + ".refined_bp.sbnd.%d.txt" % (index),
+            args.reference_fasta, args.debug)
+
+        logger.info("Counting the number of supporting read for the tumor by realignment of SV candidate segments (%d)" % (index))
         count_sread_by_alignment(
             args.tumor_prefix + ".refined_bp.%d.txt" % (index), 
-            args.control_bam, 
-            args.tumor_prefix + ".realignment.control.sread_count.%d.txt" % (index), 
-            args.tumor_prefix + ".realignment.control.sread_info.%d.txt" % (index), 
+            args.tumor_bam, 
+            args.tumor_prefix + ".realignment.tumor.sread_count.%d.txt" % (index), 
+            args.tumor_prefix + ".realignment.tumor.sread_info.%d.txt" % (index), 
             args.reference_fasta,
             sbnd_file = args.tumor_prefix + ".refined_bp.sbnd.%d.txt" % (index), 
-            output_count_file_sbnd = args.tumor_prefix + ".realignment.control.sread_count.sbnd.%d.txt" % (index),
-            output_alignment_info_file_sbnd = args.tumor_prefix + ".realignment.control.sread_info.sbnd.%d.txt" % (index),
+            output_count_file_sbnd = args.tumor_prefix + ".realignment.tumor.sread_count.sbnd.%d.txt" % (index),
+            output_alignment_info_file_sbnd = args.tumor_prefix + ".realignment.tumor.sread_info.sbnd.%d.txt" % (index),
             check_read_max_num = args.check_read_max_num, 
             var_read_min_mapq = args.var_read_min_mapq, use_ssw_lib = args.use_ssw_lib, 
             sort_option = args.sort_option, debug = args.debug
         )
-    return 0
+     
+        if args.control_bam is not None:
+            logger.info("Counting the number of supporting read for the control by realignment of SV candidate segments (%d)" % (index))
+            count_sread_by_alignment(
+                args.tumor_prefix + ".refined_bp.%d.txt" % (index), 
+                args.control_bam, 
+                args.tumor_prefix + ".realignment.control.sread_count.%d.txt" % (index), 
+                args.tumor_prefix + ".realignment.control.sread_info.%d.txt" % (index), 
+                args.reference_fasta,
+                sbnd_file = args.tumor_prefix + ".refined_bp.sbnd.%d.txt" % (index), 
+                output_count_file_sbnd = args.tumor_prefix + ".realignment.control.sread_count.sbnd.%d.txt" % (index),
+                output_alignment_info_file_sbnd = args.tumor_prefix + ".realignment.control.sread_info.sbnd.%d.txt" % (index),
+                check_read_max_num = args.check_read_max_num, 
+                var_read_min_mapq = args.var_read_min_mapq, use_ssw_lib = args.use_ssw_lib, 
+                sort_option = args.sort_option, debug = args.debug
+            )
+        ret_code = 0
+    except Exception as e:
+        err_message = str(e)
+    
+    logger.info("End Process (%d): ret_code=%d" % (index, ret_code))
+    return (ret_code, err_message)
+
 def get_main(args):
 
     # check if the executables exist
     if args.use_racon: 
         is_tool("racon")
     else:
         is_tool("mafft")
@@ -290,55 +299,61 @@
     fw_support_read_seq_sbnds = []
     for i in range(parallel_num):
         fw_support_read_seqs.append(open(args.tumor_prefix + ".support_read_seq.%d.txt" % (i), "w"))
         fw_support_read_seq_sbnds.append(open(args.tumor_prefix + ".support_read_seq.sbnd.%d.txt" % (i), "w"))
 
     last_key = ""
     last_tpos = -1
-    for row in open(args.tumor_prefix + ".support_read_seq.txt"):
-        if row.rstrip() == "": continue
-        key = row.split("\t")[0]
-        if last_key != key:
-            last_key = key
-            last_tpos += 1
-            if last_tpos == parallel_num:
-                last_tpos = 0
-        fw_support_read_seqs[last_tpos].write(row)
+    with open(args.tumor_prefix + ".support_read_seq.txt") as hin:
+        for row in hin:
+            if row.rstrip() == "": continue
+            key = row.split("\t")[0]
+            if last_key != key:
+                last_key = key
+                last_tpos += 1
+                if last_tpos == parallel_num:
+                    last_tpos = 0
+            fw_support_read_seqs[last_tpos].write(row)
     
     last_key = ""
     last_tpos = -1
-    for row in open(args.tumor_prefix + ".support_read_seq.sbnd.txt"):
-        if row.rstrip() == "": continue
-        key = row.split("\t")[0]
-        if last_key != key:
-            last_key = key
-            last_tpos += 1
-            if last_tpos == parallel_num:
-                last_tpos = 0
-        fw_support_read_seq_sbnds[last_tpos].write(row)
+    with open(args.tumor_prefix + ".support_read_seq.sbnd.txt") as hin:
+        for row in hin:
+            if row.rstrip() == "": continue
+            key = row.split("\t")[0]
+            if last_key != key:
+                last_key = key
+                last_tpos += 1
+                if last_tpos == parallel_num:
+                    last_tpos = 0
+            fw_support_read_seq_sbnds[last_tpos].write(row)
 
     for i in range(parallel_num):
         fw_support_read_seqs[i].close()
         fw_support_read_seq_sbnds[i].close()
 
     if parallel_num == 1:
         call_slow_request(args, 0)
     else:
         import concurrent.futures
 
         if args.processes > 1:
             with concurrent.futures.ProcessPoolExecutor(max_workers=parallel_num) as executor:
                 features = [executor.submit(call_slow_request, args, i) for i in range(parallel_num)]
-                #for feature in features:
-                #    print(feature.result())
+                for feature in features:
+                    (ret_code, err_message) = feature.result()
+                    if ret_code != 0:
+                        raise Exception(err_message)
         else:
             with concurrent.futures.ThreadPoolExecutor() as executor:
                 features = [executor.submit(call_slow_request, args, i) for i in range(parallel_num)]
-                #for feature in features:
-                #    print(feature.result())
+                for feature in features:
+                    (ret_code, err_message) = feature.result()
+                    if ret_code != 0:
+                        raise Exception(err_message)
 
     logger.info("Merge parallel execution")
     def merge_txt(prefix):
         with open(prefix + ".txt", 'w') as hout:
             for i in range(parallel_num):
                 for l in open(prefix + ".%d.txt" % (i)):
                     hout.write(l)
@@ -351,29 +366,28 @@
         merge_txt(args.tumor_prefix + ".realignment.control.sread_count")
         merge_txt(args.tumor_prefix + ".realignment.control.sread_info")
         merge_txt(args.tumor_prefix + ".realignment.control.sread_count.sbnd")
         merge_txt(args.tumor_prefix + ".realignment.control.sread_info.sbnd")
     if not args.debug:
         for i in range(parallel_num):
             os.remove(args.tumor_prefix + ".support_read_seq.%d.txt" % (i))
+            os.remove(args.tumor_prefix + ".support_read_seq.sbnd.%d.txt" % (i))
             os.remove(args.tumor_prefix + ".consensus_seq.%d.txt" % (i))
             os.remove(args.tumor_prefix + ".consensus_seq.sbnd.%d.txt" % (i))
             os.remove(args.tumor_prefix + ".refined_bp.%d.txt" % (i))
             os.remove(args.tumor_prefix + ".refined_bp.sbnd.%d.txt" % (i))
             os.remove(args.tumor_prefix + ".realignment.tumor.sread_count.%d.txt" % (i))
             os.remove(args.tumor_prefix + ".realignment.tumor.sread_count.sbnd.%d.txt" % (i))
             os.remove(args.tumor_prefix + ".realignment.tumor.sread_info.%d.txt" % (i))
             os.remove(args.tumor_prefix + ".realignment.tumor.sread_info.sbnd.%d.txt" % (i))
             if args.control_bam is not None:
                 os.remove(args.tumor_prefix + ".realignment.control.sread_count.%d.txt" % (i))
                 os.remove(args.tumor_prefix + ".realignment.control.sread_count.sbnd.%d.txt" % (i))
                 os.remove(args.tumor_prefix + ".realignment.control.sread_info.%d.txt" % (i))
                 os.remove(args.tumor_prefix + ".realignment.control.sread_info.sbnd.%d.txt" % (i))
-            if not args.single_bnd:
-                os.remove(args.tumor_prefix + ".support_read_seq.sbnd.%d.txt" % (i))
 
     logger.info("Final processing") 
     control_sread_count_file = args.tumor_prefix + ".realignment.control.sread_count.txt" if args.control_bam is not None else None
     integrate_realignment_result(args.tumor_prefix + ".realignment.tumor.sread_count.txt", control_sread_count_file,
         args.tumor_prefix + ".nanomonsv.result.txt", args.reference_fasta, min_indel_size = args.min_indel_size,
         min_tumor_variant_read_num = args.min_tumor_variant_read_num, min_tumor_VAF = args.min_tumor_VAF, 
         max_control_variant_read_num = args.max_control_variant_read_num, max_control_VAF = args.max_control_VAF)
@@ -391,14 +405,16 @@
         args.tumor_prefix + ".nanomonsv.result.txt", args.tumor_prefix + ".refined_bp.sbnd.txt")
  
     if not args.debug:
         os.remove(args.tumor_prefix + ".rearrangement.sorted.clustered.bedpe")
         os.remove(args.tumor_prefix + ".insertion.sorted.clustered.bedpe")
         os.remove(args.tumor_prefix + ".deletion.sorted.clustered.bedpe")
         os.remove(args.tumor_prefix + ".singlebreakend.sorted.clustered.bed")
+        os.remove(args.tumor_prefix + ".support_read_seq.txt")
+        os.remove(args.tumor_prefix + ".support_read_seq.sbnd.txt")
         #os.remove(args.tumor_prefix + ".consensus_seq.txt")
         #os.remove(args.tumor_prefix + ".consensus_seq.sbnd.txt")
         #os.remove(args.tumor_prefix + ".refined_bp.txt")
         os.remove(args.tumor_prefix + ".refined_bp.sbnd.txt")
         os.remove(args.tumor_prefix + ".realignment.tumor.sread_count.txt")
         os.remove(args.tumor_prefix + ".realignment.tumor.sread_count.sbnd.txt")
         os.remove(args.tumor_prefix + ".realignment.tumor.sread_info.txt")  
@@ -407,30 +423,30 @@
             os.remove(args.tumor_prefix + ".realignment.control.sread_count.txt")
             os.remove(args.tumor_prefix + ".realignment.control.sread_count.sbnd.txt")
             os.remove(args.tumor_prefix + ".realignment.control.sread_info.txt")
             os.remove(args.tumor_prefix + ".realignment.control.sread_info.sbnd.txt")
 
         if not args.single_bnd:
             os.remove(args.tumor_prefix + ".nanomonsv.sbnd.result.txt")   
-            #os.remove(args.tumor_prefix + ".support_read_seq.sbnd.txt")
+
 
 def validate_main(args):
    
     # executable check
     if args.use_ssw_lib: libssw_check()
 
     
-    logger.info("Counting the number of supprting read for the tumor by realignment of SV candidate segments")
+    logger.info("Counting the number of supporting read for the tumor by realignment of SV candidate segments")
     count_sread_by_alignment(args.sv_list_file, args.tumor_bam,
         args.output + ".realignment.tumor.sread_count.txt", args.output + ".realignment.tumor.sread_info.txt",
         args.reference_fasta, var_read_min_mapq = args.var_read_min_mapq, use_ssw_lib = args.use_ssw_lib, 
         sort_option = args.sort_option, debug = args.debug)
 
     if args.control_bam is not None:
-        logger.info("Counting the number of supprting read for the control by realignment of SV candidate segments")
+        logger.info("Counting the number of supporting read for the control by realignment of SV candidate segments")
         count_sread_by_alignment(args.sv_list_file, args.control_bam,
             args.output + ".realignment.control.sread_count.txt", args.output + ".realignment.control.sread_info.txt",
             args.reference_fasta, var_read_min_mapq = args.var_read_min_mapq, use_ssw_lib = args.use_ssw_lib, 
             sort_option = args.sort_option, debug = args.debug)
 
     logger.info("Final processing")
     control_sread_count_file = args.output + ".realignment.control.sread_count.txt" if args.control_bam is not None else None
```

### Comparing `nanomonsv-0.5.0b2/nanomonsv/smith_waterman.py` & `nanomonsv-0.5.1/nanomonsv/smith_waterman.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/ssw_lib.py` & `nanomonsv-0.5.1/nanomonsv/ssw_lib.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/swalign.py` & `nanomonsv-0.5.1/nanomonsv/swalign.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,16 @@
                 elif cell_val == del_val:
                     val = (cell_val, 'd', 1)
                 elif cell_val == ins_val:
                     val = (cell_val, 'i', 1)
                 else:
                     val = (0, 'x', 0)
 
-                if val[0] >= max_val:
+                # if val[0] >= max_val:
+                if val[0] > max_val: # prefer matches with small coordinate (modified by Y.S. on 2022/10/17)
                     max_val = val[0]
                     max_row = row
                     max_col = col
 
                 matrix.set(row, col, val)
 
         # backtrack
```

### Comparing `nanomonsv-0.5.0b2/nanomonsv/utils.py` & `nanomonsv-0.5.1/nanomonsv/utils.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv/vcf_convert.py` & `nanomonsv-0.5.1/nanomonsv/vcf_convert.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/nanomonsv.egg-info/PKG-INFO` & `nanomonsv-0.5.1/nanomonsv.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: nanomonsv
-Version: 0.5.0b2
+Version: 0.5.1
 Summary: Python tools for detecting structural variation from nanopore sequence data
 Home-page: https://github.com/friend1ws/nanomonsv
 Author: Yuichi Shiraishi
 Author-email: friend1ws@gamil.com
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -20,53 +19,57 @@
 # nanomonsv
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Build Status](https://travis-ci.com/friend1ws/nanomonsv.svg?branch=master)](https://travis-ci.com/friend1ws/nanomonsv.svg?branch=master&status=started)
 
 ## Introduction
 
-nanomonsv is a software for detecting somatic structural variations　 from paired (tumor and matched control) cancer genome sequence data. nanomonsv is presented in the following preprint. **When you use nanomonsv or any resource of this repository, please kindly site this preprint**.
+nanomonsv is a software for detecting somatic structural variations from paired (tumor and matched control) cancer genome sequence data. nanomonsv is presented in the following preprint. **When you use nanomonsv or any resource of this repository, please kindly site this preprint**.
 
-Precise characterization of somatic structural variations and mobile element insertions from paired long-read sequencing data with nanomonsv, Shiraishi et al., bioRxiv, 2020, [[link]](https://www.biorxiv.org/content/10.1101/2020.07.22.214262v1)
+Precise characterization of somatic complex structural variations from paired long-read sequencing data with nanomonsv, Shiraishi et al., bioRxiv, 2020, [[link]](https://www.biorxiv.org/content/10.1101/2020.07.22.214262v3).
+
+The current version of nanomonsv includes two detection modules, Canonical SV module, and [Single breakend SV module](https://github.com/friend1ws/nanomonsv/wiki/Single-breakend-SV). Canonical SV module can identify somatic SVs that can be captured by short-read technologies with higher precision and recall than existing methods. Furthermore, Single breakend SV module enables the detection of complex SVs that can only be identified by long-reads, such as SVs involving highly-repetitive centromeric sequences, and LINE1- and virus-mediated rearrangements. 
+
+Please see the [wiki page](https://github.com/friend1ws/nanomonsv/wiki/Single-breakend-SV) for Single breakend SV module.
 
 ## Dependency
 
 ### For basic use (`parse`, `get` command)
 
 ### Binary programs
 
 [htslib](http://www.htslib.org/), [mafft](https://mafft.cbrc.jp/alignment/software/), [racon](https://github.com/isovic/racon)(optional from ver. 0.3.0. However, we recommend to use this option. Add --use_racon option when you perfrom get command.)
 
 ### Python
-Pytnon (tested with >=3.6), pysam, numpy, parasail
+Python (tested with >=3.6), pysam, numpy, parasail
 
 > [SSW Library](https://github.com/mengyao/Complete-Striped-Smith-Waterman-Library) (This became optional since version 0.2.0. We have changed the main engine of Smith-Waterman algorithm to parasail.)
 
 
 ### For advanced use (`insert_classify` command)
 [bwa](https://github.com/lh3/bwa), [minimap2](https://github.com/lh3/minimap2), [bedtools](https://bedtools.readthedocs.io/en/latest/), [RepeatMasker](http://www.repeatmasker.org/)
 
 ## Preparation
 
 ### For basic use (`parse`, `get` command)
 
 #### Install software and add them to the PATH
 
-nanomonsv uses, `tabix`, `bgzip` (which ar part of HTSlib projects) and `mafft` inside the program,
+nanomonsv uses, `tabix`, `bgzip` (which are part of HTSlib projects) and `mafft` inside the program,
 assuming those are installed, and the paths are already added to the running environment.
 
 > ##### For use of SSW Library
 > Since version 0.2.0, nanomonsv can be executed without SSW Library. When users want to use SSW Library, create the libssw.so and add the path to the LD_LIBRARY_PATH environment variable. Please refer the **How to use the Python wrapper ssw_lib.py** section in the [SSW Library](https://github.com/mengyao/Complete-Striped-Smith-Waterman-Library) repository page.
 
 ###### For use of racon
 Since version 0.3.0, we support racon for the step where generating consensus sequence and get single-base resolution breakpoints. racon may become the default instead of mafft in the future.
 
 
 ### For advanced use (`insert_classify` command)
-`bwa`, `minimap2`, `bedtools` and `RepeatMasker` are required to be installed and these pathese are added to the running environment.
+`bwa`, `minimap2`, `bedtools` and `RepeatMasker` are required to be installed and these paths are added to the running environment.
 
 
 ### Input file
 
 nanomonsv accept the BAM file aligned by `minimap2`. 
 
 
@@ -74,32 +77,33 @@
 Starting with version 0.5.0, the use of the control panel is supported. 
 In this software, supporting reads for SVs are collected for multiple samples other than the target sample, 
 and such reads are removed as common noise (or those derived from common SVs) in the `get` stage. 
 This strategy is expected to exclude many false positives as well as improve computational cost.
 
 We have prepared the command to create control panels from the user's own sequencing data.
 In addition, for users who do not have sufficient sequencing data that can serve as a control panel (or just do not have time for processing), 
-we prepared a control panel that has been created using the 30 Nanopore sequencing data from the [Human Pangenome Reference Consortium](https://humanpangenome.org/),
-which you can download by the following command:
-
-```
-wget https://ncc-gap-pub.s3.ap-northeast-1.amazonaws.com/nanomonsv/control_panel/hprc_year1_data_freeze_nanopore_minimap2_2_24_merge_control.tar.gz
-```
+we prepared a control panel that has been created using the 30 Nanopore sequencing data from the [Human Pangenome Reference Consortium](https://humanpangenome.org/), which is available at [zenodo](https://zenodo.org/record/7017953).
 
 This control panel is made by aligning 30 Nanopore sequencing data to the GRCh38 reference genome (obtained from [here](https://console.cloud.google.com/storage/browser/genomics-public-data/resources/broad/hg38/v0;tab=objects)) with minimap2 version 2.24. 
 **When you use these control panels and publish, do not forget to credit to [HPRC](https://github.com/human-pangenomics/HG002_Data_Freeze_v1.0#citations)!**
 
 
 ## Quickstart
 
 1. Install all the prerequisite software and install nanomonsv.
 ```
 pip install nanomonsv (--user)
 ```
 
+You can also install nanomonsv via conda (bioconda channel).
+```
+conda create -n nanomonsv -c conda-forge -c bioconda nanomonsv
+```
+Occasionally the conda releases lag behind the source code and PyPI releases.
+
 2. Prepare the reference genome for the test data (here, we show the path to Genomic Data Commons reference genome).
 ```
 wget https://api.gdc.cancer.gov/data/254f697d-310d-4d7d-a27b-27fbf767a834 -O GRCh38.d1.vd1.fa.tar.gz
 tar xvf GRCh38.d1.vd1.fa.tar.gz
 ```
 
 3. Parse the putative structural variation supporting reads of the test data.
@@ -122,14 +126,16 @@
 - H2009: [tumor](https://www.ncbi.nlm.nih.gov/sra/DRX248308[accn]), [control](https://www.ncbi.nlm.nih.gov/sra/DRX248309[accn])
 - HCC1954: [tumor](https://www.ncbi.nlm.nih.gov/sra/DRX248306[accn]), [control](https://www.ncbi.nlm.nih.gov/sra/DRX248307[accn])
 
 The results of nanomonsv for the above data are available [here](https://github.com/friend1ws/nanomonsv/tree/master/misc/example).
 When you perform nanomonsv to the above data and have experienced errors, please report to us.
 Also, please kindly cite the [bioRxiv paper](https://www.biorxiv.org/content/10.1101/2020.07.22.214262v1) when you use these data.
 
+See tutorial [wiki page](https://github.com/friend1ws/nanomonsv/wiki/Tutorial) for an example workflow on analyzing COLO829 sample.
+
 ## Commands
 
 ### parse
 
 This step parses all the supporting reads of putative somatic SVs.
 
 ```
@@ -158,16 +164,16 @@
               [--min_tumor_VAF MIN_TUMOR_VAF]
               [--max_control_variant_read_num MAX_CONTROL_VARIANT_READ_NUM]
               [--max_control_VAF MAX_CONTROL_VAF]
               [--cluster_margin_size CLUSTER_MARGIN_SIZE]
               [--median_mapQ_thres MEDIAN_MAPQ_THRES]
               [--max_overhang_size_thres MAX_OVERHANG_SIZE_THRES]
               [--var_read_min_mapq VAR_READ_MIN_MAPQ] [--use_ssw_lib] [--use_racon]
-              [--threads THREADS] [--processes PROCESSES] 
-              [--sort_option SORT_OPTION] [--debug]
+              [--single_bnd] [--threads THREADS] [--processes PROCESSES] 
+              [--sort_option SORT_OPTION] [--max_memory_minimap2] [--debug]
               tumor_prefix tumor_bam reference.fa
  ```
  - **tumor_prefix**: Prefix to the tumor data set in the parse step
  - **tumor_bam**: Path to input indexed BAM file
  - **reference.fa**: Path to reference genome used for the alignment
  
 This software can generate a list of SVs without specifying the matched control.
@@ -175,26 +181,32 @@
 Even when only tumor sample is available, we still recommend using dummy control sample (collected from other person's tissue).
 - **control_prefix**: Prefix to the matched control data set in the parse step
 - **control_bam**: Path to the matched control BAM file
 
 When you use the control panel (recommended!), use the following argument.
 - **control_panel_prefix**: Prefix of non-matched control panel data processed in merge_control step.
 
+You can also use **--process** to use multi-processing mode. Currently, we do not recommend using **--thread** option.
+
 After successful execution, you will be able to find the result file names as {tumor_prefix}.nanomonsv.result.txt.
 See the help (`nanomonsv get -h`) for other options. 
 
 When you want to change the engine of Smith-Waterman algorithm to SSW Library, specify `--use_ssw_lib` option,
 though we do not generally recommend this.
 
 Also, we basically recommend using `--use_racon` option. This will slightly improve the identification of single-base resolution breakpoint, 
 and polishing of inserted sequences. 
 
+For detection of single breakend SVs, please use `--single_bnd` option as well as `--use_racon`. 
+Please see [wiki page](https://github.com/friend1ws/nanomonsv/wiki/Single-breakend-SV).
+
 Also, we have prepared the script (misc/post_fileter.py) for filtering the result.
 Please see the [wiki page](https://github.com/friend1ws/nanomonsv/wiki/How-to-filter-nanomonsv-result).
 For output files of the version 0.4.0 and later, some filtering has already been performed (see the [wiki page](https://github.com/friend1ws/nanomonsv/wiki/How-to-understand-nanomonsv-result-filtering)). 
+However, we strongly recommed to perform additional processing; removing indels within simple repeat regions (see the [wiki page](https://github.com/friend1ws/nanomonsv/wiki/An-example-on-removing-indels-within-simple-repeat)).
 
 From the version 0.4.0, we will also provide the VCF format result files.
 
 #### result
 
 * **Chr_1**: Chromosome for the 1st breakpoint
 * **Pos_1**: Coordinate for the 1st breakpoint
@@ -269,9 +281,7 @@
                    [--var_read_min_mapq VAR_READ_MIN_MAPQ] [--debug]
                    sv_list_file tumor_bam output reference.fa
 ```
 - **sv_list_file**: SV candidate list file (similar format with the result file by `get` command. 
 But only from **Chr_1** to **Inserted_Seq** columns are necessary.
 - **output_file**: Path to the output file
 - **reference.fa**: Path to the reference genome                          
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nanomonsv-0.5.0b2/nanomonsv.egg-info/SOURCES.txt` & `nanomonsv-0.5.1/nanomonsv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.0b2/setup.py` & `nanomonsv-0.5.1/setup.py`

 * *Files identical despite different names*

