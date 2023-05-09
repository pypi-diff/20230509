# Comparing `tmp/scutls-0.1.7.tar.gz` & `tmp/scutls-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scutls-0.1.7.tar", max compression
+gzip compressed data, was "scutls-0.1.8.tar", max compression
```

## Comparing `scutls-0.1.7.tar` & `scutls-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0      563 2023-01-06 05:03:05.145749 scutls-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       22 2023-01-06 05:03:16.476307 scutls-0.1.7/scutls/__init__.py
--rw-r--r--   0        0        0     4155 2023-01-06 03:56:33.414976 scutls-0.1.7/scutls/arguments.py
--rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.1.7/scutls/assets/genome_ensembl_107_54_54_54.json
--rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.1.7/scutls/assets/genome_ensembl_release_all.txt
--rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.1.7/scutls/assets/genome_ensembl_release_use.txt
--rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.1.7/scutls/assets/genome_ucsc.json
--rw-r--r--   0        0        0      683 2023-01-06 03:26:34.585406 scutls-0.1.7/scutls/cli.py
--rw-r--r--   0        0        0     7697 2022-12-04 03:13:17.278874 scutls-0.1.7/scutls/download.py
--rw-r--r--   0        0        0     3587 2023-01-06 04:59:39.007377 scutls-0.1.7/scutls/fastq.py
--rw-r--r--   0        0        0     5988 2022-12-04 03:55:34.933756 scutls-0.1.7/scutls/util.py
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 scutls-0.1.7/setup.py
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 scutls-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-05-09 02:54:26.962623 scutls-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6148 2022-06-21 02:55:28.045509 scutls-0.1.8/scutls/.DS_Store
+-rw-r--r--   0        0        0       22 2023-01-06 05:03:16.476307 scutls-0.1.8/scutls/__init__.py
+-rw-r--r--   0        0        0     5682 2023-05-09 02:41:06.226561 scutls-0.1.8/scutls/arguments.py
+-rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.1.8/scutls/assets/genome_ensembl_107_54_54_54.json
+-rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.1.8/scutls/assets/genome_ensembl_release_all.txt
+-rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.1.8/scutls/assets/genome_ensembl_release_use.txt
+-rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.1.8/scutls/assets/genome_ucsc.json
+-rw-r--r--   0        0        0     3891 2023-05-09 02:52:35.471573 scutls-0.1.8/scutls/barcode.py
+-rw-r--r--   0        0        0     1023 2023-05-09 02:41:24.391377 scutls-0.1.8/scutls/cli.py
+-rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.1.8/scutls/download.py
+-rw-r--r--   0        0        0     3603 2023-05-08 14:34:45.400997 scutls-0.1.8/scutls/fastq.py
+-rw-r--r--   0        0        0     7624 2023-05-09 02:33:14.600203 scutls-0.1.8/scutls/util.py
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 scutls-0.1.8/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 scutls-0.1.8/PKG-INFO
```

### Comparing `scutls-0.1.7/pyproject.toml` & `scutls-0.1.8/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "scutls"
-version = "0.1.7"
+version = "0.1.8"
 description = "Single-cell data processing utility tools"
 authors = ["Kai Hu <kai.hu@umassmed.edu>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 importlib-resources = "^5.8.0"
 wget = "^3.2"
 bs4 = "^0.0.1"
 urllib3 = "^1.26.10"
 GEOparse = "^2.0.3"
 biopython = "^1.80"
+regex = "^2023.5.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `scutls-0.1.7/scutls/arguments.py` & `scutls-0.1.8/scutls/arguments.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sys
-import pkg_resources
 from argparse import ArgumentParser
 from scutls import cli
 from scutls.__init__ import __version__
 
 parser = ArgumentParser(description = "Single-cell sequencing utility tools")
 parser.add_argument("-v", "--version", action="version", version="%(prog)s " + str(__version__))
 
@@ -16,112 +15,154 @@
     "-o", "--outdir",
     help = "output directory, default to ./",
     required = False, type = str, default = "./"
 )
 parser_download.add_argument(
     "-lgu",
     "--list_genome_ucsc",
-    help="list all available UCSC genome names",
+    help = "list all available UCSC genome names",
     required = False,
     default = False,
     action='store_true' # quick hack to skip requred input: https://stackoverflow.com/questions/59363298/argparse-expected-one-argument
 )
 parser_download.add_argument(
     "-gu",
     "--genome_ucsc",
-    help="a UCSC genome name to download",
+    help = "a UCSC genome name to download",
     required = False,
     default = None,
     type = str
 )
 parser_download.add_argument(
     "-lge",
     "--list_genome_ensembl",
-    help="list all available ENSEMBL genome names",
+    help = "list all available ENSEMBL genome names",
     required = False,
     default = False,
     action='store_true' # quick hack to skip requred input: https://stackoverflow.com/questions/59363298/argparse-expected-one-argument
 )
 parser_download.add_argument(
     "-ge",
     "--genome_ensembl",
-    help="an ENSEMBL genome name to download",
+    help = "an ENSEMBL genome name to download",
     required = False,
     default = None,
     type = str
 )
 parser_download.add_argument(
     "-au",
     "--annotation_ucsc",
-    help="an UCSC genome name to download annotation file",
+    help = "an UCSC genome name to download annotation file",
     required = False,
     default = None,
     type = str
 )
 parser_download.add_argument(
     "-ae",
     "--annotation_ensembl",
-    help="an ENSEMBL genome name to download annotation file",
+    help = "an ENSEMBL genome name to download annotation file",
     required = False,
     default = None,
     type = str
 )
 parser_download.add_argument(
     "-er",
     "--ensembl_release",
-    help="list all ENSEMBL releases and the one in use",
+    help = "list all ENSEMBL releases and the one in use",
     required = False,
     default = False,
     action='store_true' # quick hack to skip requred input: https://stackoverflow.com/questions/59363298/argparse-expected-one-argument
 )
 parser_download.add_argument(
     "-eru",
     "--ensembl_release_use",
-    help="update ENSEMBL release in use, input 4 release numbers separated by comma (vetebrate, plants, fungi, metazoa), e.g. -eru '104, 51, 51, 51'",
+    help = "update ENSEMBL release in use, input 4 release numbers separated by comma (vetebrate, plants, fungi, metazoa), e.g. -eru '104, 51, 51, 51'",
     required = False,
     default = None,
     type = str
 )
 parser_download.add_argument(
     "-erup",
     "--ensembl_release_update",
-    help="update ENSEMBL releases",
+    help = "update ENSEMBL releases",
     required = False,
     default = False,
     action='store_true' # quick hack to skip requred input: https://stackoverflow.com/questions/59363298/argparse-expected-one-argument
 )
-parser_download.set_defaults(func=cli.run_download)
+parser_download.set_defaults(func = cli.run_download)
 
-# subcommand: fastq
+# sub-command: fastq
 parser_fastq = subparsers.add_parser(
     "fastq", description = "process fastq files")
 parser_fastq.add_argument(
     "-i", "--input",
     help = "input fastq, can end with .gz",
     required = True, type = str, default = None
 )
 parser_fastq.add_argument(
     "-o", "--output",
     help = "output fastq name, can end with .gz",
     required = True, type = str, default = None
 )
-# add mutually exclusive groups
+## add mutually exclusive groups
 parser_fastq_group = parser_fastq.add_mutually_exclusive_group()
 parser_fastq_group.add_argument(
     "-u", "--unique",
     help = "keep unique records (by sequence ID) in fastq file",
     required = False, default = False, action='store_true'
 )
 parser_fastq_group.add_argument(
     "-j", "--join",
     help = "append each read from --join fastq to corresponding line in --input fastq, not 'cat'; the read count and id must be the same in the two fastq files",
     required = False, type = str, default = None
 )
+## set default values
+parser_fastq.set_defaults(func = cli.run_fastq)
 
-parser_fastq.set_defaults(func=cli.run_fastq)
+# sub-command: barcode
+parser_barcode = subparsers.add_parser(
+    "barcode", description = "handle barcode file")
+parser_barcode.add_argument(
+    "-i", "--input",
+    help = "input fastq, can end with .gz",
+    required = True, type = str, default = None)
+parser_barcode.add_argument(
+    "-o", "--output",
+    help = "output fastq name, can end with .gz",
+    required = True, type = str, default = None
+)
+parser_barcode.add_argument(
+    "-o2", "--output2",
+    help = "output fastq name for non-hit reads, can end with .gz",
+    required = False, type = str, default = None
+)
+parser_barcode.add_argument(
+    "-c", "--contain",
+    help = "barcode string to search against the fastq, seperate by comma if multiple. e.g. 'AACCC,GTCCC,CAAA'",
+    required = True, type = str, default = None
+)
+parser_barcode.add_argument(
+    "-e", "--error",
+    help = "allowed mismatchs (including INDELs) when searching for barcode string",
+    required = False, type = int, default = 1
+)
+parser_barcode.add_argument(
+    "-rcb", "--rc_barcode", 
+    help = "reverse complement the barcode before searching",
+    required = False,
+    default = False,
+    action='store_true' # quick hack to skip requred input: https://stackoverflow.com/questions/59363298/argparse-expected-one-argument
+)
+parser_barcode.add_argument(
+    "-nproc", "--num_processor",
+    help = "number of parallel jobs",
+    required = False, type = int, default = 1
+)
+## set default values
+parser_barcode.set_defaults(func = cli.run_barcode)
 
 def main():
     if len(sys.argv[1:]) == 0:
         parser.print_help()
         parser.exit()
     else:
         args = parser.parse_args()
```

### Comparing `scutls-0.1.7/scutls/assets/genome_ensembl_107_54_54_54.json` & `scutls-0.1.8/scutls/assets/genome_ensembl_107_54_54_54.json`

 * *Files identical despite different names*

### Comparing `scutls-0.1.7/scutls/assets/genome_ensembl_release_all.txt` & `scutls-0.1.8/scutls/assets/genome_ensembl_release_all.txt`

 * *Files identical despite different names*

### Comparing `scutls-0.1.7/scutls/assets/genome_ucsc.json` & `scutls-0.1.8/scutls/assets/genome_ucsc.json`

 * *Files identical despite different names*

### Comparing `scutls-0.1.7/scutls/cli.py` & `scutls-0.1.8/scutls/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from scutls import download, fastq
+from scutls import download, fastq, barcode
+
+# the default values are specified via the arguments.py file
 
 def run_download(args):
     download.download(
     list_genome_ucsc = args.list_genome_ucsc,
     genome_ucsc = args.genome_ucsc,
     list_genome_ensembl = args.list_genome_ensembl,
     genome_ensembl = args.genome_ensembl,
@@ -17,7 +19,18 @@
 def run_fastq(args):
     fastq.fastq(
     input  = args.input,
     output = args.output,
     unique = args.unique,
     join   = args.join
     )
+
+def run_barcode(args):
+    barcode.barcode(
+    input  = args.input,
+    output = args.output,
+    output2 = args.output2,
+    contain = args.contain,
+    error   = args.error,
+    rc_barcode = args.rc_barcode,
+    nproc = args.num_processor # must use full name
+    )
```

### Comparing `scutls-0.1.7/scutls/download.py` & `scutls-0.1.8/scutls/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 import importlib_resources
 import wget
 import os
 from os import path
 import cmd
-import inspect
 import argparse
 from .util import update_ensembl_release, get_ensembl_url_json
 
 def download(list_genome_ucsc = False, list_genome_ensembl = False, genome_ucsc = None, genome_ensembl = None, annotation_ucsc = None, annotation_ensembl = None, ensembl_release = False, ensembl_release_use = None, ensembl_release_update = False, outdir = "./"):
     """download subcommand
     Paramters
     ---------
```

### Comparing `scutls-0.1.7/scutls/fastq.py` & `scutls-0.1.8/scutls/fastq.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import argparse
 from Bio import SeqIO, bgzf
 from Bio.Seq import Seq
 from .util import _open
 import os
 
 def fastq(input = None, output = None, unique = None, join = None):
     """fastq subcommand
```

### Comparing `scutls-0.1.7/setup.py` & `scutls-0.1.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 {'': ['*'], 'scutls': ['assets/*']}
 
 install_requires = \
 ['GEOparse>=2.0.3,<3.0.0',
  'biopython>=1.80,<2.0',
  'bs4>=0.0.1,<0.0.2',
  'importlib-resources>=5.8.0,<6.0.0',
+ 'regex>=2023.5.5,<2024.0.0',
  'urllib3>=1.26.10,<2.0.0',
  'wget>=3.2,<4.0']
 
 entry_points = \
 {'console_scripts': ['scutls = scutls.arguments:main']}
 
 setup_kwargs = {
     'name': 'scutls',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Single-cell data processing utility tools',
     'long_description': 'None',
     'author': 'Kai Hu',
     'author_email': 'kai.hu@umassmed.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scutls-0.1.7/PKG-INFO` & `scutls-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: scutls
-Version: 0.1.7
+Version: 0.1.8
 Summary: Single-cell data processing utility tools
 Author: Kai Hu
 Author-email: kai.hu@umassmed.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GEOparse (>=2.0.3,<3.0.0)
 Requires-Dist: biopython (>=1.80,<2.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: importlib-resources (>=5.8.0,<6.0.0)
+Requires-Dist: regex (>=2023.5.5,<2024.0.0)
 Requires-Dist: urllib3 (>=1.26.10,<2.0.0)
 Requires-Dist: wget (>=3.2,<4.0)
```

