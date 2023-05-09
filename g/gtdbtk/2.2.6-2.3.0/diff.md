# Comparing `tmp/gtdbtk-2.2.6.tar.gz` & `tmp/gtdbtk-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtdbtk-2.2.6.tar", last modified: Thu Mar 23 03:49:14 2023, max compression
+gzip compressed data, was "gtdbtk-2.3.0.tar", last modified: Tue May  9 00:11:54 2023, max compression
```

## Comparing `gtdbtk-2.2.6.tar` & `gtdbtk-2.3.0.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.072359 gtdbtk-2.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35122 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-03-23 03:49:14.072359 gtdbtk-2.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.056359 gtdbtk-2.2.6/gtdbtk/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/ani_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/ani_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.060359 gtdbtk-2.2.6/gtdbtk/biolib_lite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/biolib_lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/biolib_lite/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/biolib_lite/custom_help_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/biolib_lite/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/biolib_lite/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/biolib_lite/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/biolib_lite/newick.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/biolib_lite/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    16327 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/biolib_lite/prodigal_biolib.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/biolib_lite/seq_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    30846 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/biolib_lite/taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)   116129 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.060359 gtdbtk-2.2.6/gtdbtk/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/config/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    16476 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/decorate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.060359 gtdbtk-2.2.6/gtdbtk/external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/fastani.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/fasttree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/hmm_aligner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/mash.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/pfam_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/pplacer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/prodigal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.060359 gtdbtk-2.2.6/gtdbtk/external/pypfam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.060359 gtdbtk-2.2.6/gtdbtk/external/pypfam/HMM/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1812 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/pypfam/HMM/HMMMatch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4876 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/pypfam/HMM/HMMResults.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21015 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/pypfam/HMM/HMMResultsIO.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2241 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/pypfam/HMM/HMMSequence.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2066 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/pypfam/HMM/HMMUnit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/pypfam/HMM/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.060359 gtdbtk-2.2.6/gtdbtk/external/pypfam/Scan/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22327 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/pypfam/Scan/PfamScan.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/pypfam/Scan/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/pypfam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/external/tigrfam_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.064359 gtdbtk-2.2.6/gtdbtk/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/files/batchfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/files/classify_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/files/gtdb_radii.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.064359 gtdbtk-2.2.6/gtdbtk/files/marker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/files/marker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/files/marker/copy_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/files/marker/tophit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/files/marker_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/files/missing_genomes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/files/pplacer_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.064359 gtdbtk-2.2.6/gtdbtk/files/prodigal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/files/prodigal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/files/prodigal/tln_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/files/prodigal/tln_table_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/files/red_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/files/stage_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/files/tree_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/infer_ranks.py
--rw-r--r--   0 runner    (1001) docker     (123)    53648 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    34858 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.064359 gtdbtk-2.2.6/gtdbtk/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/model/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.064359 gtdbtk-2.2.6/gtdbtk/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/pipeline/align.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/pipeline/export_msa.py
--rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/relative_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/reroot_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    21475 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.052359 gtdbtk-2.2.6/gtdbtk/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.052359 gtdbtk-2.2.6/gtdbtk/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.068359 gtdbtk-2.2.6/gtdbtk/tests/data/genomes/
--rw-r--r--   0 runner    (1001) docker     (123)  2973983 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/tests/data/genomes/genome_1.fna
--rw-r--r--   0 runner    (1001) docker     (123)  1292421 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/tests/data/genomes/genome_2.fna
--rw-r--r--   0 runner    (1001) docker     (123)  1210030 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/tests/data/genomes/genome_3.fna
--rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/tools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12742 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/gtdbtk/trim_msa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.056359 gtdbtk-2.2.6/gtdbtk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-03-23 03:49:14.000000 gtdbtk-2.2.6/gtdbtk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-03-23 03:49:14.000000 gtdbtk-2.2.6/gtdbtk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 03:49:14.000000 gtdbtk-2.2.6/gtdbtk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-23 03:49:14.000000 gtdbtk-2.2.6/gtdbtk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-23 03:49:14.000000 gtdbtk-2.2.6/gtdbtk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-23 03:49:14.000000 gtdbtk-2.2.6/gtdbtk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 03:49:14.072359 gtdbtk-2.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.068359 gtdbtk-2.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.072359 gtdbtk-2.2.6/tests/test_gtdbtk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.072359 gtdbtk-2.2.6/tests/test_gtdbtk/test_biolib_lite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_biolib_lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_biolib_lite/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_biolib_lite/test_newick.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_biolib_lite/test_seq_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_biolib_lite/test_taxonomy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.072359 gtdbtk-2.2.6/tests/test_gtdbtk/test_external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_external/test_fastani.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_external/test_fasttree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.072359 gtdbtk-2.2.6/tests/test_gtdbtk/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.072359 gtdbtk-2.2.6/tests/test_gtdbtk/test_files/test_marker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_files/test_marker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_files/test_marker/test_copy_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_files/test_marker/test_tophit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:14.072359 gtdbtk-2.2.6/tests/test_gtdbtk/test_files/test_prodigal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_files/test_prodigal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_files/test_prodigal/test_tln_table_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-23 03:49:05.000000 gtdbtk-2.2.6/tests/test_gtdbtk/test_trim_msa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.421002 gtdbtk-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35122 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-09 00:11:54.421002 gtdbtk-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.405002 gtdbtk-2.3.0/gtdbtk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/ani_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/ani_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.405002 gtdbtk-2.3.0/gtdbtk/biolib_lite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/custom_help_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/newick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16327 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/prodigal_biolib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/seq_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30846 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/biolib_lite/taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117674 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24439 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.409002 gtdbtk-2.3.0/gtdbtk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/config/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/config/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16476 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/decorate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.409002 gtdbtk-2.3.0/gtdbtk/external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/fastani.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/fasttree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/hmm_aligner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/mash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pfam_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pplacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/prodigal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.409002 gtdbtk-2.3.0/gtdbtk/external/pypfam/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.409002 gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1812 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMMatch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4876 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMResults.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21015 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMResultsIO.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2241 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMSequence.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2066 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMUnit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.409002 gtdbtk-2.3.0/gtdbtk/external/pypfam/Scan/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22327 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/Scan/PfamScan.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/Scan/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/pypfam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/external/tigrfam_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.409002 gtdbtk-2.3.0/gtdbtk/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/batchfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/classify_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/gtdb_radii.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.409002 gtdbtk-2.3.0/gtdbtk/files/marker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/marker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/marker/copy_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/marker/tophit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/marker_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/missing_genomes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/pplacer_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.413002 gtdbtk-2.3.0/gtdbtk/files/prodigal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/prodigal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/prodigal/tln_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/prodigal/tln_table_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/red_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/stage_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/files/tree_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/infer_ranks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54256 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34860 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.413002 gtdbtk-2.3.0/gtdbtk/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/model/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.413002 gtdbtk-2.3.0/gtdbtk/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/pipeline/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/pipeline/export_msa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/relative_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/reroot_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21477 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.401002 gtdbtk-2.3.0/gtdbtk/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.401002 gtdbtk-2.3.0/gtdbtk/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.417002 gtdbtk-2.3.0/gtdbtk/tests/data/genomes/
+-rw-r--r--   0 runner    (1001) docker     (123)  2973983 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/tests/data/genomes/genome_1.fna
+-rw-r--r--   0 runner    (1001) docker     (123)  1292421 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/tests/data/genomes/genome_2.fna
+-rw-r--r--   0 runner    (1001) docker     (123)  1210030 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/tests/data/genomes/genome_3.fna
+-rw-r--r--   0 runner    (1001) docker     (123)    15764 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12742 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/gtdbtk/trim_msa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.405002 gtdbtk-2.3.0/gtdbtk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-09 00:11:54.000000 gtdbtk-2.3.0/gtdbtk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-09 00:11:54.000000 gtdbtk-2.3.0/gtdbtk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:11:54.000000 gtdbtk-2.3.0/gtdbtk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-09 00:11:54.000000 gtdbtk-2.3.0/gtdbtk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-09 00:11:54.000000 gtdbtk-2.3.0/gtdbtk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 00:11:54.000000 gtdbtk-2.3.0/gtdbtk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:11:54.421002 gtdbtk-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.417002 gtdbtk-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-09 00:11:39.000000 gtdbtk-2.3.0/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.417002 gtdbtk-2.3.0/tests/test_gtdbtk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14323 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.421002 gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/test_newick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/test_seq_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/test_taxonomy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.421002 gtdbtk-2.3.0/tests/test_gtdbtk/test_external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_external/test_fastani.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_external/test_fasttree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.421002 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.421002 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_marker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_marker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_marker/test_copy_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_marker/test_tophit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:54.421002 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_prodigal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_prodigal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_prodigal/test_tln_table_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-09 00:11:40.000000 gtdbtk-2.3.0/tests/test_gtdbtk/test_trim_msa.py
```

### Comparing `gtdbtk-2.2.6/LICENSE` & `gtdbtk-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/PKG-INFO` & `gtdbtk-2.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtdbtk
-Version: 2.2.6
+Version: 2.3.0
 Summary: A toolkit for assigning objective taxonomic classifications to bacterial and archaeal genomes.
 Home-page: https://github.com/Ecogenomics/GTDBTk
 Author: Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks
 Author-email: p.chaumeil@uq.edu.au
 Maintainer: Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks
 Maintainer-email: donovan.parks@gmail.com
 License: GPL3
@@ -56,21 +56,17 @@
 ## 📖 Documentation
 
 Documentation for GTDB-Tk can be found [here](https://ecogenomics.github.io/GTDBTk/).
 
 
 ## ✨ New Features
 
-GTDB-Tk v2.2.0+ includes the following new features:
-- GTDB-TK `classify` and `classify_wf` have changed in version 2.2.0+. There is now an ANI classification stage (`ANI screen`) that precedes classification by placement in a reference tree.
-  - **This is now the default behavior for `classify` and `classify_wf`.**
-  - In `classify`, user genomes are first compared against a Mash database comprised of all GTDB representative genomes and genome pairs of sufficient similarity processed by FastANI. User genomes classified to a GTDB representative based on FastANI results are not run through pplacer. 
-  - In the `classify_wf` workflow, genomes are classified using Mash and FastANI before executing the identify step. User genomes classified with FastANI are not run through the remainder of the pipeline (identify, align, classify).
-  - `classify_wf` and `classify` have now **an extra mutually exclusive required argument**: You can either pick `--skip_ani_screen` (to skip the ani_screening step to classify genomes using mash and FastANI) or `--mash_db` path to save/read (if exists) the Mash reference sketch database.
-  - To classify genomes without the additional `ani_screen` step, use the `--skip_ani_screen` flag.
+GTDB-Tk v2.3.0+ includes the following new features:
+- New functionality ``convert_to_species`` function to convert GTDB genome IDs to GTDB species names
+
 
 ## 📈 Performance
 Using ANI screen "can" reduce computation by >50%, although it depends on the set of input genomes. A set of input genomes consisting primarily of new species will not benefit from ANI screen as much as a set of genomes that are largely assigned to GTDB species clusters. In the latter case, the ANI screen will reduce the number of genomes that need to be classified by pplacer which reduces computation time substantially (between 25% and 60% in our testing).
 
 ## 📚 References
 
 GTDB-Tk is described in:
```

### Comparing `gtdbtk-2.2.6/README.md` & `gtdbtk-2.3.0/gtdbtk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: gtdbtk
+Version: 2.3.0
+Summary: A toolkit for assigning objective taxonomic classifications to bacterial and archaeal genomes.
+Home-page: https://github.com/Ecogenomics/GTDBTk
+Author: Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks
+Author-email: p.chaumeil@uq.edu.au
+Maintainer: Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks
+Maintainer-email: donovan.parks@gmail.com
+License: GPL3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # GTDB-Tk
 
 [![PyPI](https://img.shields.io/pypi/v/gtdbtk.svg)](https://pypi.python.org/pypi/gtdbtk)
 [![PyPI Downloads](https://pepy.tech/badge/gtdbtk)](https://pepy.tech/project/gtdbtk)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/gtdbtk.svg?color=43b02a)](https://anaconda.org/bioconda/gtdbtk)
 [![BioConda Downloads](https://img.shields.io/conda/dn/bioconda/gtdbtk.svg?style=flag&label=downloads&color=43b02a)](https://anaconda.org/bioconda/gtdbtk)
 [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/ecogenomic/gtdbtk?sort=date&color=299bec&label=docker)](https://hub.docker.com/r/ecogenomic/gtdbtk)
@@ -33,21 +56,17 @@
 ## 📖 Documentation
 
 Documentation for GTDB-Tk can be found [here](https://ecogenomics.github.io/GTDBTk/).
 
 
 ## ✨ New Features
 
-GTDB-Tk v2.2.0+ includes the following new features:
-- GTDB-TK `classify` and `classify_wf` have changed in version 2.2.0+. There is now an ANI classification stage (`ANI screen`) that precedes classification by placement in a reference tree.
-  - **This is now the default behavior for `classify` and `classify_wf`.**
-  - In `classify`, user genomes are first compared against a Mash database comprised of all GTDB representative genomes and genome pairs of sufficient similarity processed by FastANI. User genomes classified to a GTDB representative based on FastANI results are not run through pplacer. 
-  - In the `classify_wf` workflow, genomes are classified using Mash and FastANI before executing the identify step. User genomes classified with FastANI are not run through the remainder of the pipeline (identify, align, classify).
-  - `classify_wf` and `classify` have now **an extra mutually exclusive required argument**: You can either pick `--skip_ani_screen` (to skip the ani_screening step to classify genomes using mash and FastANI) or `--mash_db` path to save/read (if exists) the Mash reference sketch database.
-  - To classify genomes without the additional `ani_screen` step, use the `--skip_ani_screen` flag.
+GTDB-Tk v2.3.0+ includes the following new features:
+- New functionality ``convert_to_species`` function to convert GTDB genome IDs to GTDB species names
+
 
 ## 📈 Performance
 Using ANI screen "can" reduce computation by >50%, although it depends on the set of input genomes. A set of input genomes consisting primarily of new species will not benefit from ANI screen as much as a set of genomes that are largely assigned to GTDB species clusters. In the latter case, the ANI screen will reduce the number of genomes that need to be classified by pplacer which reduces computation time substantially (between 25% and 60% in our testing).
 
 ## 📚 References
 
 GTDB-Tk is described in:
```

### Comparing `gtdbtk-2.2.6/gtdbtk/__init__.py` & `gtdbtk-2.3.0/gtdbtk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 __maintainer__ = 'Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks'
 __maintainer_email__ = 'donovan.parks@gmail.com'
 __name__ = 'gtdbtk'
 __python_requires__ = '>=3.6'
 __status__ = 'Production'
 __title__ = 'GTDB-Tk'
 __url__ = 'https://github.com/Ecogenomics/GTDBTk'
-__version__ = '2.2.6'
+__version__ = '2.3.0'
```

### Comparing `gtdbtk-2.2.6/gtdbtk/__main__.py` & `gtdbtk-2.3.0/gtdbtk/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,20 +45,21 @@
     align    -> Create multiple sequence alignment
     classify -> Determine taxonomic classification of genomes
     infer    -> Infer tree from multiple sequence alignment
     root     -> Root tree using an outgroup
     decorate -> Decorate tree with GTDB taxonomy
 
   Tools:
-    infer_ranks     -> Establish taxonomic ranks of internal nodes using RED
-    ani_rep         -> Calculates ANI to GTDB representative genomes
-    trim_msa        -> Trim an untrimmed MSA file based on a mask
-    export_msa      -> Export the untrimmed archaeal or bacterial MSA file
-    remove_labels   -> Remove labels (bootstrap values, node labels) from an Newick tree
-    convert_to_itol -> Convert a GTDB-Tk Newick tree to an iTOL tree
+    infer_ranks        -> Establish taxonomic ranks of internal nodes using RED
+    ani_rep            -> Calculates ANI to GTDB representative genomes
+    trim_msa           -> Trim an untrimmed MSA file based on a mask
+    export_msa         -> Export the untrimmed archaeal or bacterial MSA file
+    remove_labels      -> Remove labels (bootstrap values, node labels) from an Newick tree
+    convert_to_itol    -> Convert a GTDB-Tk Newick tree to an iTOL tree
+    convert_to_species -> Convert GTDB genome IDs to GTDB species names
  
 
   Testing:
     test          -> Validate the classify_wf pipeline with 3 archaeal genomes 
     check_install -> Verify third party programs and GTDB reference package
 
   Use: gtdbtk <command> -h for command specific help
```

### Comparing `gtdbtk-2.2.6/gtdbtk/ani_rep.py` & `gtdbtk-2.3.0/gtdbtk/ani_rep.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import os
 from collections import defaultdict
 from typing import List
 
 from gtdbtk.biolib_lite.common import canonical_gid
 from gtdbtk.biolib_lite.execute import check_dependencies
 from gtdbtk.biolib_lite.taxonomy import Taxonomy
-from gtdbtk.config.config import (TAXONOMY_FILE,
-                                  AF_THRESHOLD)
+from gtdbtk.config.common import CONFIG
 from gtdbtk.config.output import DIR_ANI_REP_INT_MASH
 from gtdbtk.exceptions import GTDBTkExit
 from gtdbtk.external.fastani import FastANI
 from gtdbtk.external.mash import Mash
 from gtdbtk.files.gtdb_radii import GTDBRadiiFile
 from gtdbtk.tools import get_ref_genomes
 
@@ -72,15 +71,15 @@
             The path to read/write the pre-computed Mash reference sketch database.
         """
         max_mash_dist = mash_d
         fastani_results = self.run_mash_fastani(genomes, no_mash, mash_d, out_dir,
                                                 prefix, mash_k, mash_v,
                                                 mash_s, max_mash_dist, mash_db=mash_db)
 
-        taxonomy = Taxonomy().read(TAXONOMY_FILE, canonical_ids=True)
+        taxonomy = Taxonomy().read(CONFIG.TAXONOMY_FILE, canonical_ids=True)
         ani_summary_file = ANISummaryFile(out_dir, prefix, fastani_results, taxonomy)
         ani_summary_file.write()
         ANIClosestFile(out_dir,
                        prefix,
                        fastani_results,
                        genomes,
                        min_af,
@@ -265,13 +264,13 @@
                         gtdb_ani_radius = self.gtdb_radii.get_rep_ani(canonical_rid)
                         closest_ani = closest[0][1]["ani"]
                         closest_af = closest[0][1]["af"]
 
                         fh.write(f'{gid}\t{ref_gid}')
                         fh.write(f'\t{closest_ani}\t{closest_af}')
                         fh.write(f'\t{taxonomy_str}')
-                        fh.write(f'\t{closest_ani >= gtdb_ani_radius and closest_af >= AF_THRESHOLD}\n')
+                        fh.write(f'\t{closest_ani >= gtdb_ani_radius and closest_af >= CONFIG.AF_THRESHOLD}\n')
                     else:
                         fh.write(f'{gid}\tno result\tno result\tno result\tno result\tno result\n')
                 else:
                     fh.write(f'{gid}\tno result\tno result\tno result\tno result\n')
         self.logger.info(f'Closest representative hits saved to: {self.path}')
```

### Comparing `gtdbtk-2.2.6/gtdbtk/ani_screen.py` & `gtdbtk-2.3.0/gtdbtk/ani_screen.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 from gtdbtk.ani_rep import ANIRep, ANISummaryFile
 from gtdbtk.biolib_lite.common import make_sure_path_exists, canonical_gid
 
 from gtdbtk.biolib_lite.taxonomy import Taxonomy
 from gtdbtk.classify import Classify
 from gtdbtk.config.output import DIR_ANISCREEN
 
-from gtdbtk.config.config import (TAXONOMY_FILE, MASH_SKETCH_FILE, AF_THRESHOLD)
 from gtdbtk.files.gtdb_radii import GTDBRadiiFile
-
+from gtdbtk.config.common import CONFIG
 
 class ANIScreener(object):
     """Computes a list of genomes to a list of representatives."""
 
     def __init__(self, cpus):
         """Instantiate the ANI rep class.
 
@@ -35,25 +34,25 @@
         # All genomes classified with FastANI will be removed from the input genomes list for the
         # rest of the pipeline.
         mash_classified_user_genomes = {}
         #if mash_db finishes with a backslash, it should be considered a directory
         if mash_db.endswith('/'):
             make_sure_path_exists(mash_db)
         if os.path.isdir(mash_db):
-            mash_db = os.path.join(mash_db, MASH_SKETCH_FILE)
+            mash_db = os.path.join(mash_db, CONFIG.MASH_SKETCH_FILE)
 
         #we set mash_d == mash_max_dist to avoid user to run mash with impossible values
         mash_d = mash_max_dist
 
         ani_rep = ANIRep(self.cpus)
         # we store all the mash information in the classify directory
         fastani_results = ani_rep.run_mash_fastani(genomes, no_mash, mash_d, os.path.join(out_dir, DIR_ANISCREEN),
                                                     prefix, mash_k, mash_v, mash_s, mash_max_dist, mash_db)
 
-        taxonomy = Taxonomy().read(TAXONOMY_FILE, canonical_ids=True)
+        taxonomy = Taxonomy().read(CONFIG.TAXONOMY_FILE, canonical_ids=True)
 
         mash_classified_user_genomes = self.sort_fastani_ani_screen(
              fastani_results,taxonomy)
 
         #We write the results in 2 different files for each domain
         reports = {}
         if mash_classified_user_genomes:
@@ -84,15 +83,15 @@
             The taxonomy of the reference genomes
         """
         classified_user_genomes = {}
 
         # sort the dictionary by ani then af
         for gid in fastani_results.keys():
             thresh_results = [(ref_gid, hit) for (ref_gid, hit) in fastani_results[gid].items() if
-                              hit['af'] >= AF_THRESHOLD and hit['ani'] >= self.gtdb_radii.get_rep_ani(
+                              hit['af'] >= CONFIG.AF_THRESHOLD and hit['ani'] >= self.gtdb_radii.get_rep_ani(
                                   canonical_gid(ref_gid))]
             all_results = [(ref_gid, hit) for (ref_gid, hit) in fastani_results[gid].items()]
             closest = sorted(thresh_results, key=lambda x: (-x[1]['ani'], -x[1]['af']))
             all_closest = sorted(all_results, key=lambda x: (-x[1]['ani'], -x[1]['af']))
             if len(closest) > 0:
                 ref_gid, hit = closest[0]
                 hit_taxonomy = taxonomy[canonical_gid(ref_gid)]
```

### Comparing `gtdbtk-2.2.6/gtdbtk/biolib_lite/common.py` & `gtdbtk-2.3.0/gtdbtk/biolib_lite/common.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/biolib_lite/custom_help_formatter.py` & `gtdbtk-2.3.0/gtdbtk/biolib_lite/custom_help_formatter.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/biolib_lite/exceptions.py` & `gtdbtk-2.3.0/gtdbtk/biolib_lite/exceptions.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/biolib_lite/execute.py` & `gtdbtk-2.3.0/gtdbtk/biolib_lite/execute.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/biolib_lite/logger.py` & `gtdbtk-2.3.0/gtdbtk/biolib_lite/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import ntpath
 import os
 import re
 import sys
 
 from tqdm import tqdm
 
-from gtdbtk.config.config import LOG_TASK
+from gtdbtk.config.common import CONFIG
 from .common import make_sure_path_exists
 
 
 def supports_colour():
     """Check that the current terminal supports colour.
 
     Returns
@@ -124,15 +124,15 @@
                                     format(colour('ERROR:', ['bright'], 'red')),
                                     datefmt="%Y-%m-%d %H:%M:%S")
         task_fmt = logging.Formatter(fmt="[%(asctime)s] {} %(message)s".
                                      format(colour('TASK:', ['bright'])),
                                      datefmt="%Y-%m-%d %H:%M:%S")
 
         def format(self, record):
-            if record.levelno == LOG_TASK:
+            if record.levelno == CONFIG.LOG_TASK:
                 return self.task_fmt.format(record)
             if record.levelno >= logging.ERROR:
                 return self.err_fmt.format(record)
             elif record.levelno >= logging.WARNING:
                 return self.warn_fmt.format(record)
             elif record.levelno >= logging.INFO:
                 return self.info_fmt.format(record)
@@ -158,15 +158,15 @@
         err_fmt = logging.Formatter(fmt="[%(asctime)s] ERROR: %(message)s",
                                     datefmt="%Y-%m-%d %H:%M:%S")
         task_fmt = logging.Formatter(fmt="[%(asctime)s] TASK: %(message)s",
                                      datefmt="%Y-%m-%d %H:%M:%S")
 
         def format(self, record):
             record.msg = self.ansi_escape.sub('', record.msg)
-            if record.levelno == LOG_TASK:
+            if record.levelno == CONFIG.LOG_TASK:
                 return self.task_fmt.format(record)
             if record.levelno >= logging.ERROR:
                 return self.err_fmt.format(record)
             elif record.levelno >= logging.WARNING:
                 return self.warn_fmt.format(record)
             elif record.levelno >= logging.INFO:
                 return self.info_fmt.format(record)
```

### Comparing `gtdbtk-2.2.6/gtdbtk/biolib_lite/newick.py` & `gtdbtk-2.3.0/gtdbtk/biolib_lite/newick.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/biolib_lite/parallel.py` & `gtdbtk-2.3.0/gtdbtk/biolib_lite/parallel.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/biolib_lite/prodigal_biolib.py` & `gtdbtk-2.3.0/gtdbtk/biolib_lite/prodigal_biolib.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/biolib_lite/seq_io.py` & `gtdbtk-2.3.0/gtdbtk/biolib_lite/seq_io.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/biolib_lite/taxonomy.py` & `gtdbtk-2.3.0/gtdbtk/biolib_lite/taxonomy.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/classify.py` & `gtdbtk-2.3.0/gtdbtk/classify.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from collections import defaultdict
 from operator import itemgetter
 
 import dendropy
 
 from numpy import median as np_median
 
-import gtdbtk.config.config as Config
+from gtdbtk.config.common import CONFIG
 from gtdbtk.ani_rep import ANIRep, ANISummaryFile
 from gtdbtk.biolib_lite.common import make_sure_path_exists,canonical_gid
 from gtdbtk.biolib_lite.execute import check_dependencies
 from gtdbtk.biolib_lite.newick import parse_label
 from gtdbtk.biolib_lite.seq_io import read_seq, read_fasta
 from gtdbtk.biolib_lite.taxonomy import Taxonomy
 from gtdbtk.config.output import *
@@ -65,16 +65,16 @@
     def __init__(self, cpus=1, pplacer_cpus=None, af_threshold=None,skip_pplacer=False):
         """Initialize."""
 
         check_dependencies(['pplacer', 'guppy', 'fastANI'])
 
         self.skip_pplacer = skip_pplacer
 
-        self.taxonomy_file = Config.TAXONOMY_FILE
-        self.af_threshold = af_threshold if af_threshold else Config.AF_THRESHOLD
+        self.taxonomy_file = CONFIG.TAXONOMY_FILE
+        self.af_threshold = af_threshold if af_threshold else CONFIG.AF_THRESHOLD
         self.gtdb_taxonomy = Taxonomy().read(self.taxonomy_file)
 
         self.order_rank = ["d__", "p__", "c__", "o__", 'f__', 'g__', 's__']
 
         self.DOMAIN_IDX = 0
         self.PHYLUM_IDX = 1
         self.CLASS_IDX = 2
@@ -106,15 +106,15 @@
         # rank_of_interest determine the rank in the tree_mapping file for
         # lower classification
         self.rank_of_interest = "c__"
 
     @staticmethod
     def parse_radius_file():
         results = {}
-        with open(Config.RADII_FILE) as f:
+        with open(CONFIG.RADII_FILE) as f:
             for line in f:
                 infos = line.strip().split('\t')
                 gid = infos[1]
                 if infos[1].startswith('GB_') or infos[1].startswith('RS_'):
                     gid = gid[3:]
                 results[gid] = float(infos[2])
         return results
@@ -155,24 +155,24 @@
         mem_warning = 'pplacer requires ~{req_gb} GB of RAM to fully load the ' \
                       '{domain} tree into memory. However, {cur_gb:,} GB was ' \
                       'detected. This may affect pplacer performance, or fail' \
                       ' if there is insufficient swap space.'
         mem_gb = get_memory_gb()
         if mem_gb is not None:
             mem_total = mem_gb['MemTotal']
-            if marker_set_id == 'bac120' and levelopt is None and mem_total < Config.PPLACER_MIN_RAM_BAC_FULL:
-                self.logger.warning(mem_warning.format(req_gb=Config.PPLACER_MIN_RAM_BAC_FULL,
+            if marker_set_id == 'bac120' and levelopt is None and mem_total < CONFIG.PPLACER_MIN_RAM_BAC_FULL:
+                self.logger.warning(mem_warning.format(req_gb=CONFIG.PPLACER_MIN_RAM_BAC_FULL,
                                                        domain='bacterial',
                                                        cur_gb=mem_total))
-            if marker_set_id == 'bac120' and levelopt == 'high' and mem_total < Config.PPLACER_MIN_RAM_BAC_SPLIT:
-                self.logger.warning(mem_warning.format(req_gb=Config.PPLACER_MIN_RAM_BAC_SPLIT,
+            if marker_set_id == 'bac120' and levelopt == 'high' and mem_total < CONFIG.PPLACER_MIN_RAM_BAC_SPLIT:
+                self.logger.warning(mem_warning.format(req_gb=CONFIG.PPLACER_MIN_RAM_BAC_SPLIT,
                                                        domain='bacterial',
                                                        cur_gb=mem_total))
-            elif marker_set_id == 'ar53' and mem_total < Config.PPLACER_MIN_RAM_ARC:
-                self.logger.warning(mem_warning.format(req_gb=Config.PPLACER_MIN_RAM_ARC,
+            elif marker_set_id == 'ar53' and mem_total < CONFIG.PPLACER_MIN_RAM_ARC:
+                self.logger.warning(mem_warning.format(req_gb=CONFIG.PPLACER_MIN_RAM_ARC,
                                                        domain='archaeal',
                                                        cur_gb=mem_total))
 
         # rename user MSA file for compatibility with pplacer
         if not user_msa_file.endswith('.fasta') and not user_msa_file.endswith('.gz'):
             if marker_set_id == 'bac120':
                 t = PATH_BAC120_USER_MSA.format(prefix=prefix)
@@ -196,43 +196,43 @@
                 scratch_dir, prefix + ".pplacer.scratch")
             make_sure_path_exists(scratch_dir)
 
         # get path to pplacer reference package
         pplacer_ref_pkg = None
         if marker_set_id == 'bac120':
             if levelopt is None:
-                self.logger.log(Config.LOG_TASK,
+                self.logger.log(CONFIG.LOG_TASK,
                                 f'Placing {num_genomes:,} bacterial genomes '
                                 f'into reference tree with pplacer using '
                                 f'{self.pplacer_cpus} CPUs (be patient).')
-                pplacer_ref_pkg = os.path.join(Config.PPLACER_DIR,
-                                               Config.PPLACER_BAC120_REF_PKG)
+                pplacer_ref_pkg = os.path.join(CONFIG.PPLACER_DIR,
+                                               CONFIG.PPLACER_BAC120_REF_PKG)
 
             elif levelopt == 'high':
-                self.logger.log(Config.LOG_TASK,
+                self.logger.log(CONFIG.LOG_TASK,
                                 f'Placing {num_genomes:,} bacterial genomes '
                                 f'into backbone reference tree with pplacer using '
                                 f'{self.pplacer_cpus} CPUs (be patient).')
-                pplacer_ref_pkg = os.path.join(Config.BACKBONE_PPLACER_DIR,
-                                               Config.BACKBONE_PPLACER_REF_PKG)
+                pplacer_ref_pkg = os.path.join(CONFIG.BACKBONE_PPLACER_DIR,
+                                               CONFIG.BACKBONE_PPLACER_REF_PKG)
             elif levelopt == 'low':
-                self.logger.log(Config.LOG_TASK,
+                self.logger.log(CONFIG.LOG_TASK,
                                 f'Placing {num_genomes:,} bacterial genomes '
                                 f'into class-level reference tree {tree_iter} ({idx_tree}/{number_low_trees}) with '
                                 f'pplacer using {self.pplacer_cpus} CPUs '
                                 f'(be patient).')
-                pplacer_ref_pkg = os.path.join(Config.CLASS_LEVEL_PPLACER_DIR,
-                                               Config.CLASS_LEVEL_PPLACER_REF_PKG.format(iter=tree_iter))
+                pplacer_ref_pkg = os.path.join(CONFIG.CLASS_LEVEL_PPLACER_DIR,
+                                               CONFIG.CLASS_LEVEL_PPLACER_REF_PKG.format(iter=tree_iter))
         elif marker_set_id == 'ar53':
-            self.logger.log(Config.LOG_TASK,
+            self.logger.log(CONFIG.LOG_TASK,
                             f'Placing {num_genomes:,} archaeal genomes into '
                             f'reference tree with pplacer using '
                             f'{self.pplacer_cpus} CPUs (be patient).')
-            pplacer_ref_pkg = os.path.join(Config.PPLACER_DIR,
-                                           Config.PPLACER_AR53_REF_PKG)
+            pplacer_ref_pkg = os.path.join(CONFIG.PPLACER_DIR,
+                                           CONFIG.PPLACER_AR53_REF_PKG)
         else:
             raise GenomeMarkerSetUnknown(f'Unknown marker set: {marker_set_id}')
 
         # create pplacer output directory
         pplacer_out_dir = os.path.join(out_dir, DIR_PPLACER)
         if not os.path.exists(pplacer_out_dir):
             os.makedirs(pplacer_out_dir)
@@ -314,33 +314,33 @@
         return results
 
     def parser_marker_summary_file(self, marker_summary_fh):
         results = dict()
         for gid, marker_dict in marker_summary_fh.genomes.items():
             multi_hits_percent = (100 * len(marker_dict['mul'])) / \
                                  len(marker_summary_fh.marker_names)
-            if multi_hits_percent >= Config.DEFAULT_MULTIHIT_THRESHOLD:
+            if multi_hits_percent >= CONFIG.DEFAULT_MULTIHIT_THRESHOLD:
                 results[gid] = round(multi_hits_percent, 1)
         return results
 
     def run(self,
             genomes,
             align_dir,
             out_dir,
             prefix,
             scratch_dir=None,
             debugopt=False,
             fulltreeopt=False,
             skip_ani_screen=False,
             genes=False,
             no_mash=False,
-            mash_k=Config.MASH_K_VALUE,
-            mash_v=Config.MASH_V_VALUE,
-            mash_s=Config.MASH_S_VALUE,
-            mash_max_dist=Config.MASH_MAX_DISTANCE,
+            mash_k=CONFIG.MASH_K_VALUE,
+            mash_v=CONFIG.MASH_V_VALUE,
+            mash_s=CONFIG.MASH_S_VALUE,
+            mash_max_dist=CONFIG.MASH_MAX_DISTANCE,
             mash_db=None,
             ani_summary_files=None,
             all_classified_ani=False):
         """Classify genomes based on position in reference tree."""
         if not all_classified_ani:
             _bac_gids, _ar_gids, bac_ar_diff = Markers().genome_domain(align_dir, prefix)
 
@@ -356,15 +356,15 @@
                 self.logger.warning('The --genes flag is set to True. The ANI screening steps will be skipped.')
                 skip_ani_screen = True
             elif not no_mash:
                 # if mash_db finishes with a backslash, it should be considered a directory
                 if mash_db.endswith('/'):
                     make_sure_path_exists(mash_db)
                 if os.path.isdir(mash_db):
-                    mash_db = os.path.join(mash_db, Config.MASH_SKETCH_FILE)
+                    mash_db = os.path.join(mash_db, CONFIG.MASH_SKETCH_FILE)
 
             # we set mash_d == mash_max_dist to avoid user to run mash with impossible values
             mash_d = mash_max_dist
 
             ani_rep = ANIRep(self.cpus)
             # we store all the mash information in the classify directory
             fastani_results = ani_rep.run_mash_fastani(genomes, no_mash, mash_d, os.path.join(out_dir, DIR_ANISCREEN), prefix, mash_k, mash_v, mash_s,mash_max_dist, mash_db )
@@ -451,31 +451,53 @@
                         tree_mapping_file = GenomeMappingFile(out_dir, prefix)
                 else:
                     raise GenomeMarkerSetUnknown('There was an error determining the marker set.')
 
                 if (not os.path.exists(user_msa_file)) or (os.path.getsize(user_msa_file) < 30):
                     # file will not exist if there are no User genomes from a given domain
                     #
+                    if marker_set_id == 'ar53':
+                        # we still add the filtered genomes to the summary file
+                        # add filtered genomes to the summary file
+                        warning_counter = self.add_filtered_genomes_to_summary(align_dir, warning_counter, summary_file,
+                                                                               marker_set_id, prefix)
+
                     # But if there is Unclassified genomes without domain,
                     # they still have to be written in the bac120 summary file:
-                    if marker_set_id == 'bac120':
+                    elif marker_set_id == 'bac120':
                         # Add failed genomes from prodigal and genomes with no markers in the bac120 summary file
                         # This is an executive direction: failed prodigal and genomes with no markers are not bacterial or archaeal
                         # but they need to be included in one of the summary file
                         prodigal_failed_counter = self.add_failed_genomes_to_summary(align_dir, summary_file, prefix)
-                        if summary_file.has_row():
-                            summary_file.write()
-                            output_files.setdefault(marker_set_id, []).append(summary_file.path)
-                            # Symlink to the summary file from the root
+                        # we also add the filtered genomes to the summary file
+                        # add filtered genomes to the summary file
+                        warning_counter = self.add_filtered_genomes_to_summary(align_dir, warning_counter, summary_file,
+                                                                               marker_set_id, prefix)
+
+                    # we add all genomes classified with ANI
+                    if mash_classified_user_genomes and marker_set_id in mash_classified_user_genomes:
+                        list_summary_rows = mash_classified_user_genomes.get(marker_set_id)
+                        for row in list_summary_rows:
+                            summary_file.add_row(row)
+
+                    if summary_file.has_row():
+                        summary_file.write()
+                        output_files.setdefault(marker_set_id, []).append(summary_file.path)
+                        # Symlink to the summary file from the root
+                        if marker_set_id == 'ar53':
+                            symlink_f(PATH_AR53_SUMMARY_OUT.format(prefix=prefix),
+                                      os.path.join(out_dir, os.path.basename(PATH_AR53_SUMMARY_OUT.format(prefix=prefix))))
+                        elif marker_set_id == 'bac120':
                             symlink_f(PATH_BAC120_SUMMARY_OUT.format(prefix=prefix),
                                       os.path.join(out_dir, os.path.basename(PATH_BAC120_SUMMARY_OUT.format(prefix=prefix))))
-                            if prodigal_failed_counter > 0:
-                                self.logger.warning(f"{prodigal_failed_counter} of {len(genomes)} "
-                                                    f"genome{'' if prodigal_failed_counter == 1 else 's'} "
-                                                    f"ha{'s' if prodigal_failed_counter == 1 else 've'} been labeled as 'Unclassified'.")
+                        if prodigal_failed_counter > 0:
+                            self.logger.warning(f"{prodigal_failed_counter} of {len(genomes)} "
+                                                f"genome{'' if prodigal_failed_counter == 1 else 's'} "
+                                                f"ha{'s' if prodigal_failed_counter == 1 else 've'} been labeled as 'Unclassified'.")
+
 
                     continue
 
                 msa_dict = read_fasta(user_msa_file)
 
                 # Read the translation table summary file (identify).
                 tln_table_summary_file = TlnTableSummaryFile(align_dir, prefix)
@@ -556,15 +578,15 @@
                     disappearing_genomes = [seq_id for seq_id in genomes_to_process if seq_id not in high_classification]
                     if disappearing_genomes:
                         for disappearing_genome in disappearing_genomes:
                             disappearing_genomes_file.add_genome(disappearing_genome, 'Backbone')
 
                     tree_mapping_dict = {}
                     tree_mapping_dict_reverse = {}
-                    with open(Config.CLASS_LEVEL_TREE_MAPPING_FILE) as ltmf:
+                    with open(CONFIG.CLASS_LEVEL_TREE_MAPPING_FILE) as ltmf:
                         for line in ltmf:
                             k, v = line.strip().split()
                             tree_mapping_dict[k] = v
                             tree_mapping_dict_reverse.setdefault(v, []).append(k)
 
                     splitter = Split(self.order_rank, self.gtdb_taxonomy, self.reference_ids)
                     sorted_high_taxonomy,warning_counter, len_sorted_genomes, high_taxonomy_used = splitter.map_high_taxonomy(
@@ -1159,15 +1181,15 @@
         # We go through all leaves of the tree. if the leaf is a user
         # genome we take its parent node and look at all the leaves
         # for this node.
 
         # Persist descendant information for efficient traversal.
         tt = TreeTraversal()
 
-        self.logger.log(Config.LOG_TASK, 'Traversing tree to determine classification method.')
+        self.logger.log(CONFIG.LOG_TASK, 'Traversing tree to determine classification method.')
         if genes:
             fastani_verification = {}
         else:
             fastani_verification, qury_nodes = self._get_fastani_verification(tree, self.reference_ids, tt)
 
         #DEBUG: Skip FastANI step
         #fastani_verification = {}
@@ -1175,15 +1197,15 @@
         # we run a fastani comparison for each user genomes against the
         # selected genomes in the same genus
         ##if not prescreening and len(fastani_verification) > 0:
         if len(fastani_verification) > 0:
             fastani = FastANI(cpus=self.cpus, force_single=True)
             d_ani_compare, d_paths = self._get_fastani_genome_path(
                 fastani_verification, genomes)
-            self.logger.log(Config.LOG_TASK,
+            self.logger.log(CONFIG.LOG_TASK,
                             f'Calculating average nucleotide identity using '
                             f'FastANI (v{fastani.version}).')
             all_fastani_dict = fastani.run(d_ani_compare, d_paths)
         else:
             all_fastani_dict = {}
 
         classified_user_genomes, unclassified_user_genomes,warning_counter = self._sort_fastani_results(
@@ -1243,21 +1265,21 @@
                                            rooting='force-rooted',
                                            preserve_underscores=True)
 
         # Persist descendant information for efficient traversal.
         tt = TreeTraversal()
 
         if levelopt is None:
-            red_file = Config.MRCA_RED_BAC120
+            red_file = CONFIG.MRCA_RED_BAC120
         elif levelopt == 'high':
-            red_file = Config.BACKBONE_RED_FILE
+            red_file = CONFIG.BACKBONE_RED_FILE
         elif levelopt == 'low':
-            red_file = Config.CLASS_LEVEL_RED_FILE.format(iter=tree_iter)
+            red_file = CONFIG.CLASS_LEVEL_RED_FILE.format(iter=tree_iter)
         if marker_set_id == 'ar53':
-            red_file = Config.MRCA_RED_AR53
+            red_file = CONFIG.MRCA_RED_AR53
 
         # create map from leave labels to tree nodes
         leaf_node_map = {}
         for leaf in tree.leaf_node_iter():
             leaf_node_map[leaf.taxon.label] = leaf
 
         # parse RED file and associate reference RED value to reference node in
@@ -1363,24 +1385,25 @@
     def add_filtered_genomes_to_summary(self, align_dir,warning_counter, summary_file, marker_set_id,prefix):
         if marker_set_id == 'bac120':
             filtered_file = os.path.join(align_dir,PATH_BAC120_FILTERED_GENOMES.format(prefix=prefix))
             domain = 'Bacteria'
         else:
             filtered_file = os.path.join(align_dir,PATH_AR53_FILTERED_GENOMES.format(prefix=prefix))
             domain = 'Archaea'
-
-        with open(filtered_file) as fin:
-            for line in fin:
-                infos = line.strip().split('\t')
-                summary_row = ClassifySummaryFileRow()
-                summary_row.gid = infos[0]
-                summary_row.classification = f'Unclassified {domain}'
-                summary_row.warnings = infos[1]
-                summary_file.add_row(summary_row)
-                warning_counter += 1
+        # if file exists:
+        if os.path.exists(filtered_file):
+            with open(filtered_file) as fin:
+                for line in fin:
+                    infos = line.strip().split('\t')
+                    summary_row = ClassifySummaryFileRow()
+                    summary_row.gid = infos[0]
+                    summary_row.classification = f'Unclassified {domain}'
+                    summary_row.warnings = infos[1]
+                    summary_file.add_row(summary_row)
+                    warning_counter += 1
         return warning_counter
 
     def add_failed_genomes_to_summary(self, align_dir, summary_file, prefix):
         warning_counter = 0
         prodigal_failed_file = os.path.join(align_dir, PATH_FAILS.format(prefix=prefix))
         align_failed_file = os.path.join(align_dir, PATH_FAILED_ALIGN_GENOMES.format(prefix=prefix))
         for failfile in (prodigal_failed_file, align_failed_file):
@@ -1438,15 +1461,15 @@
 
         """
         classified_user_genomes = {}
 
         # sort the dictionary by ani then af
         for gid in fastani_results.keys():
             thresh_results = [(ref_gid, hit) for (ref_gid, hit) in fastani_results[gid].items() if
-                              hit['af'] >= Config.AF_THRESHOLD and hit['ani'] >= self.gtdb_radii.get_rep_ani(
+                              hit['af'] >= CONFIG.AF_THRESHOLD and hit['ani'] >= self.gtdb_radii.get_rep_ani(
                                   canonical_gid(ref_gid))]
             closest = sorted(thresh_results, key=lambda x: (-x[1]['ani'], -x[1]['af']))
             if len(closest) > 0:
                 summary_row = ClassifySummaryFileRow()
                 summary_row.gid = gid
                 summary_row.classification_method = 'ani_screen'
                 if len(closest) > 1:
@@ -1803,23 +1826,23 @@
         self.logger.info('Reading tree.')
         tree = dendropy.Tree.get_from_path(input_tree,
                                            schema='newick',
                                            rooting='force-rooted',
                                            preserve_underscores=True)
 
         self.logger.info('Reading taxonomy from file.')
-        taxonomy = Taxonomy().read(Config.TAXONOMY_FILE)
+        taxonomy = Taxonomy().read(CONFIG.TAXONOMY_FILE)
 
         # determine taxa to be used for inferring distribution
         trusted_taxa = None
         taxa_for_dist_inference = self._filter_taxa_for_dist_inference(tree,
                                                                        taxonomy,
                                                                        trusted_taxa,
-                                                                       Config.RED_MIN_CHILDREN,
-                                                                       Config.RED_MIN_SUPPORT)
+                                                                       CONFIG.RED_MIN_CHILDREN,
+                                                                       CONFIG.RED_MIN_SUPPORT)
 
         phylum_rel_dists, rel_node_dists = self.median_rd_over_phyla(tree,
                                                                      taxa_for_dist_inference,
                                                                      taxonomy)
 
         # set edge lengths to median value over all rootings
         tree.seed_node.rel_dist = 0.0
@@ -2149,22 +2172,22 @@
                 leafnode = node[0]
                 shortleaf = leafnode.taxon.label
                 if leafnode.taxon.label.startswith('GB_') or leafnode.taxon.label.startswith('RS_'):
                     shortleaf = leafnode.taxon.label[3:]
                 # TODEL UBA genomes
                 if shortleaf.startswith("UBA"):
                     ref_path = os.path.join(
-                        Config.FASTANI_GENOMES,
+                        CONFIG.FASTANI_GENOMES,
                         'UBA',
-                        shortleaf + Config.FASTANI_GENOMES_EXT)
+                        shortleaf + CONFIG.FASTANI_GENOMES_EXT)
                 else:
                     ref_path = os.path.join(
-                        Config.FASTANI_GENOMES,
+                        CONFIG.FASTANI_GENOMES,
                         self.parse_leaf_to_dir_path(shortleaf),
-                        shortleaf + Config.FASTANI_GENOMES_EXT)
+                        shortleaf + CONFIG.FASTANI_GENOMES_EXT)
 
                 if not os.path.isfile(ref_path):
                     raise GTDBTkExit(f'Reference genome missing from FastANI database: {ref_path}')
 
                 dict_compare[user_label].add(shortleaf)
                 dict_paths[shortleaf] = ref_path
```

### Comparing `gtdbtk-2.2.6/gtdbtk/cli.py` & `gtdbtk-2.3.0/gtdbtk/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import argparse
 import tempfile
 from contextlib import contextmanager
 
 from gtdbtk.biolib_lite.custom_help_formatter import ChangeTempAction
 from gtdbtk.biolib_lite.custom_help_formatter import CustomHelpFormatter
-from gtdbtk.config.config import AF_THRESHOLD, PPLACER_MIN_RAM_BAC_FULL, MASH_K_VALUE, MASH_S_VALUE, MASH_D_VALUE, \
-    MASH_V_VALUE, MASH_MAX_DISTANCE
+from gtdbtk.config.common import CONFIG
 
 
 @contextmanager
 def subparser(parser, name, desc):
     yield parser.add_parser(name, conflict_handler='resolve', help=desc,
                             formatter_class=CustomHelpFormatter)
 
@@ -59,15 +58,15 @@
     group.add_argument('--bacteria', action='store_true', default=False,
                        help='process bacterial genomes')
 
 
 def __outgroup_taxon(group, required):
     group.add_argument('--outgroup_taxon', type=str, default=None, required=required,
                        help="taxon to use as outgroup (e.g., "
-                            "``p__Patescibacteria`` or ``p__Altarchaeota``)")
+                            "``p__Patescibacteria`` or ``p__Altiarchaeota``)")
 
 
 def __out_dir(group, required):
     group.add_argument('--out_dir', type=str, default=None, required=required,
                        help="directory to output files")
 
 
@@ -201,15 +200,15 @@
 #     group.add_argument('-r', '--recalculate_red', default=False, action='store_true',
 #                        help='recalculate RED values based on the reference tree and all added user genomes')
 
 
 def __full_tree(group):
     group.add_argument('-f', '--full_tree', default=False, action='store_true',
                        help='use the unsplit bacterial tree for the classify step; this is the original GTDB-Tk '
-                            f'approach (version < 2) and requires more than {PPLACER_MIN_RAM_BAC_FULL} GB of RAM to load the reference tree')
+                            f'approach (version < 2) and requires more than {CONFIG.PPLACER_MIN_RAM_BAC_FULL} GB of RAM to load the reference tree')
 
 
 def __identify_dir(group, required):
     group.add_argument('--identify_dir', type=str, default=None, required=required,
                        help="output directory of 'identify' command")
 
 
@@ -251,44 +250,44 @@
 
 def __no_mash(group):
     group.add_argument('--no_mash', default=False, action='store_true',
                        help='skip pre-filtering of genomes using Mash')
 
 
 def __mash_k(group):
-    group.add_argument('--mash_k', default=MASH_K_VALUE, type=int,
+    group.add_argument('--mash_k', default=CONFIG.MASH_K_VALUE, type=int,
                        help='k-mer size [1-32]')
 
 
 def __mash_s(group):
-    group.add_argument('--mash_s', default=MASH_S_VALUE, type=int,
+    group.add_argument('--mash_s', default=CONFIG.MASH_S_VALUE, type=int,
                        help='maximum number of non-redundant hashes')
 
 
 def __mash_d(group):
-    group.add_argument('--mash_d', default=MASH_D_VALUE, type=float,
+    group.add_argument('--mash_d', default=CONFIG.MASH_D_VALUE, type=float,
                        help='maximum distance to keep [0-1]')
 
 
 def __mash_v(group):
-    group.add_argument('--mash_v', default=MASH_V_VALUE, type=float,
+    group.add_argument('--mash_v', default=CONFIG.MASH_V_VALUE, type=float,
                        help='maximum p-value to keep [0-1]')
 
 def __mash_max_distance(group):
-    group.add_argument('--mash_max_distance', default=MASH_MAX_DISTANCE, type=float,
+    group.add_argument('--mash_max_distance', default=CONFIG.MASH_MAX_DISTANCE, type=float,
                        help='Maximum Mash distance to select a potential GTDB genome as representative '
                             'of a user genome.')
 
 def __mash_db(group):
     group.add_argument('--mash_db', default=None, type=str,
                        help='path to save/read (if exists) the Mash reference sketch database (.msh)')
 
 
 def __min_af(group):
-    group.add_argument('--min_af', type=float, default=AF_THRESHOLD,
+    group.add_argument('--min_af', type=float, default=CONFIG.AF_THRESHOLD,
                        help='minimum alignment fraction to assign genome to a species cluster')
 
 
 def __untrimmed_msa(group, required):
     group.add_argument('--untrimmed_msa', type=str, default=None, required=required,
                        help="path to the untrimmed MSA file")
 
@@ -314,14 +313,22 @@
                        help="reference mask already present in GTDB-Tk")
 
 
 def __domain(group, required):
     group.add_argument('--domain', required=required, choices=['arc', 'bac'],
                        help="domain to export")
 
+def __all_ranks(group):
+    group.add_argument('--all_ranks', default=False, action='store_true',
+                       help='add all missing ranks to the leaf nodes if they are present in the reference tree.')
+
+def __db_version(group):
+    group.add_argument('--db_version', type = int, default = None,
+                       help="GTDB-Tk version package to test for compatibility.")
+
 
 def __write_single_copy_genes(group):
     group.add_argument('--write_single_copy_genes', default=False, action='store_true',
                        help='output unaligned single-copy marker genes')
 
 def get_main_parser():
     # Setup the main, and sub parsers.
@@ -582,24 +589,36 @@
         with arg_group(parser, 'required named arguments') as grp:
             __input_tree(grp, required=True)
             __output_tree(grp, required=True)
         with arg_group(parser, 'optional arguments') as grp:
             __debug(grp)
             __help(grp)
 
+    # Convert genome ids to species names.
+    with subparser(sub_parsers, 'convert_to_species', 'Replace GTDB genomes ids with GTDB Species name.') as parser:
+        with arg_group(parser, 'required named arguments') as grp:
+            __input_tree(grp, required=True)
+            __output_tree(grp, required=True)
+        with arg_group(parser, 'optional arguments') as grp:
+            __custom_taxonomy_file(grp)
+            __all_ranks(grp)
+            __debug(grp)
+            __help(grp)
+
     # Export MSA.
     with subparser(sub_parsers, 'export_msa', 'Export the untrimmed archaeal or bacterial MSA file.') as parser:
         with arg_group(parser, 'required named arguments') as grp:
             __domain(grp, required=True)
             __output(grp, required=True)
         with arg_group(parser, 'optional arguments') as grp:
             __debug(grp)
             __help(grp)
 
     # Verify install.
     with subparser(sub_parsers, 'check_install', 'Verify third party programs and '
                                                  'GTDB reference package.') as parser:
         with arg_group(parser, 'optional arguments') as grp:
+            __db_version(grp)
             __debug(grp)
             __help(grp)
 
     return main_parser
```

### Comparing `gtdbtk-2.2.6/gtdbtk/config/output.py` & `gtdbtk-2.3.0/gtdbtk/config/output.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/decorate.py` & `gtdbtk-2.3.0/gtdbtk/decorate.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/exceptions.py` & `gtdbtk-2.3.0/gtdbtk/exceptions.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/external/fastani.py` & `gtdbtk-2.3.0/gtdbtk/external/fastani.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/external/fasttree.py` & `gtdbtk-2.3.0/gtdbtk/external/fasttree.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/external/hmm_aligner.py` & `gtdbtk-2.3.0/gtdbtk/external/hmm_aligner.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/external/mash.py` & `gtdbtk-2.3.0/gtdbtk/external/mash.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import subprocess
 import tempfile
 from collections import defaultdict
 from typing import Tuple, Dict
 from gtdbtk.biolib_lite.common import make_sure_path_exists
 from gtdbtk.exceptions import GTDBTkExit
 from gtdbtk.tools import tqdm_log
-import gtdbtk.config.config as Config
+from gtdbtk.config.common import CONFIG
 
 
 class Mash(object):
     """Runs Mash against genomes."""
 
     def __init__(self, cpus, out_dir, prefix):
         """Instantiate the Mash class.
@@ -267,15 +267,15 @@
         """
         path = os.path.join(root, f'{prefix}.{self.name}')
 
         super().__init__(genomes, path, cpus, k, s)
 
 
 class RefSketchFile(SketchFile):
-    name = Config.MASH_SKETCH_FILE
+    name = CONFIG.MASH_SKETCH_FILE
 
     def __init__(self, genomes, root, prefix, cpus, k, s, mash_db=None):
         """Create a query file for a given set of genomes.
 
         Parameters
         ----------
         genomes : dict[str, str]
```

### Comparing `gtdbtk-2.2.6/gtdbtk/external/pfam_search.py` & `gtdbtk-2.3.0/gtdbtk/external/pfam_search.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/external/pplacer.py` & `gtdbtk-2.3.0/gtdbtk/external/pplacer.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/external/prodigal.py` & `gtdbtk-2.3.0/gtdbtk/external/prodigal.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/external/pypfam/HMM/HMMMatch.py` & `gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMMatch.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/external/pypfam/HMM/HMMResults.py` & `gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMResults.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/external/pypfam/HMM/HMMResultsIO.py` & `gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMResultsIO.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/external/pypfam/HMM/HMMSequence.py` & `gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMSequence.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/external/pypfam/HMM/HMMUnit.py` & `gtdbtk-2.3.0/gtdbtk/external/pypfam/HMM/HMMUnit.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/external/pypfam/Scan/PfamScan.py` & `gtdbtk-2.3.0/gtdbtk/external/pypfam/Scan/PfamScan.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/external/tigrfam_search.py` & `gtdbtk-2.3.0/gtdbtk/external/tigrfam_search.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/files/batchfile.py` & `gtdbtk-2.3.0/gtdbtk/files/batchfile.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/files/classify_summary.py` & `gtdbtk-2.3.0/gtdbtk/files/classify_summary.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/files/gtdb_radii.py` & `gtdbtk-2.3.0/gtdbtk/files/gtdb_radii.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from gtdbtk.biolib_lite.common import canonical_gid
-from gtdbtk.config.config import RADII_FILE
-
+from gtdbtk.config.common import CONFIG
 
 class GTDBRadiiFile(object):
     """A wrapper for the gtdb_radii.tsv file included in the reference data."""
-    path = RADII_FILE
 
     def __init__(self):
         self._rep_idx = None
         self._species_idx = None
         self._read()
 
+    @property
+    def path(self):
+        return CONFIG.RADII_FILE
+
     def _read(self):
         """Read the file and create any data."""
         self._rep_idx, self._species_idx = dict(), dict()
         with open(self.path) as fh:
             for line in fh.readlines():
                 species, genome, ani = line.strip().split('\t')
                 genome = canonical_gid(genome)
```

### Comparing `gtdbtk-2.2.6/gtdbtk/files/marker/copy_number.py` & `gtdbtk-2.3.0/gtdbtk/files/marker/copy_number.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import logging
 import os
 from typing import Set, Dict, List, Union
 
 from gtdbtk.biolib_lite.common import make_sure_path_exists
 from gtdbtk.biolib_lite.seq_io import read_fasta
-from gtdbtk.config.config import BAC120_MARKERS, AR53_MARKERS
+from gtdbtk.config.common import CONFIG
 from gtdbtk.config.output import PATH_BAC120_MARKER_SUMMARY, PATH_AR53_MARKER_SUMMARY
 from gtdbtk.exceptions import GTDBTkExit
 from gtdbtk.files.marker.tophit import TopHitPfamFile, TopHitTigrFile, Hit
 
 
 class CopyNumberFile(object):
     """Store copy number information for a specific marker set. Records the
@@ -155,16 +155,16 @@
 
 
 class CopyNumberFileAR53(CopyNumberFile):
     """Store hmm copy number information for AR53 markers."""
 
     def __init__(self, out_dir: str, prefix: str):
         path = os.path.join(out_dir, PATH_AR53_MARKER_SUMMARY.format(prefix=prefix))
-        super().__init__(path, 'ar53', AR53_MARKERS)
+        super().__init__(path, 'ar53', CONFIG.AR53_MARKERS)
 
 
 class CopyNumberFileBAC120(CopyNumberFile):
     """Store hmm copy number information for BAC120 markers."""
 
     def __init__(self, out_dir: str, prefix: str):
         path = os.path.join(out_dir, PATH_BAC120_MARKER_SUMMARY.format(prefix=prefix))
-        super().__init__(path, 'bac120', BAC120_MARKERS)
+        super().__init__(path, 'bac120', CONFIG.BAC120_MARKERS)
```

### Comparing `gtdbtk-2.2.6/gtdbtk/files/marker/tophit.py` & `gtdbtk-2.3.0/gtdbtk/files/marker/tophit.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/files/marker_info.py` & `gtdbtk-2.3.0/gtdbtk/files/marker_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,28 +14,32 @@
 #    along with this program. If not, see <http://www.gnu.org/licenses/>.     #
 #                                                                             #
 ###############################################################################
 
 import os
 
 from gtdbtk.biolib_lite.common import make_sure_path_exists
-from gtdbtk.config.config import AR53_MARKERS, BAC120_MARKERS, TIGRFAM_HMMS, PFAM_HMM_DIR
+from gtdbtk.config.common import CONFIG
 from gtdbtk.config.output import PATH_AR53_MARKER_INFO, PATH_BAC120_MARKER_INFO
 
 
 class MarkerInfoFile(object):
     """Store the GTDB-Tk RED dictionary."""
 
-    marker_paths = {"PFAM": os.path.join(PFAM_HMM_DIR, 'individual_hmms'),
-                    "TIGRFAM": os.path.join(os.path.dirname(TIGRFAM_HMMS), 'individual_hmms')}
-
     def __init__(self, path: str, markers: dict):
         self.path = path
         self.markers = self._parse_markers(markers)
 
+    @property
+    def marker_paths(self):
+        return {
+            "PFAM": os.path.join(CONFIG.PFAM_HMM_DIR, 'individual_hmms'),
+            "TIGRFAM": os.path.join(os.path.dirname(CONFIG.TIGRFAM_HMMS), 'individual_hmms')
+        }
+
     def _parse_markers(self, markers):
         out = dict()
         for db_marker in sorted(markers):
             for marker in markers[db_marker]:
                 marker_id = marker[0:marker.rfind('.')]
                 marker_path = os.path.join(self.marker_paths[db_marker], marker)
 
@@ -67,16 +71,16 @@
 
 
 class MarkerInfoFileAR53(MarkerInfoFile):
     """Marker information for the AR53 marker set."""
 
     def __init__(self, out_dir: str, prefix: str):
         path = os.path.join(out_dir, PATH_AR53_MARKER_INFO.format(prefix=prefix))
-        super().__init__(path, AR53_MARKERS)
+        super().__init__(path, CONFIG.AR53_MARKERS)
 
 
 class MarkerInfoFileBAC120(MarkerInfoFile):
     """Marker information for the BAC120 marker set."""
 
     def __init__(self, out_dir: str, prefix: str):
         path = os.path.join(out_dir, PATH_BAC120_MARKER_INFO.format(prefix=prefix))
-        super().__init__(path, BAC120_MARKERS)
+        super().__init__(path, CONFIG.BAC120_MARKERS)
```

### Comparing `gtdbtk-2.2.6/gtdbtk/files/missing_genomes.py` & `gtdbtk-2.3.0/gtdbtk/files/missing_genomes.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/files/pplacer_classification.py` & `gtdbtk-2.3.0/gtdbtk/files/pplacer_classification.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/files/prodigal/tln_table.py` & `gtdbtk-2.3.0/gtdbtk/files/prodigal/tln_table.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/files/prodigal/tln_table_summary.py` & `gtdbtk-2.3.0/gtdbtk/files/prodigal/tln_table_summary.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/files/red_dict.py` & `gtdbtk-2.3.0/gtdbtk/files/red_dict.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #                                                                             #
 ###############################################################################
 
 import os
 from typing import Dict
 
 from gtdbtk.biolib_lite.common import make_sure_path_exists
-from gtdbtk.config.config import RED_DIST_ARC_DICT, RED_DIST_BAC_DICT
+from gtdbtk.config.common import CONFIG
 from gtdbtk.config.output import PATH_AR53_RED_DICT, PATH_BAC120_RED_DICT
 
 
 class REDDictFile(object):
     """Store the GTDB-Tk RED dictionary."""
 
     def __init__(self, path: str, red_dict: Dict[str, float]):
@@ -42,16 +42,16 @@
 
 
 class REDDictFileAR53(REDDictFile):
     """Store the RED dictionary for the AR53 marker set."""
 
     def __init__(self, out_dir: str, prefix: str):
         path = os.path.join(out_dir, PATH_AR53_RED_DICT.format(prefix=prefix))
-        super().__init__(path, RED_DIST_ARC_DICT)
+        super().__init__(path, CONFIG.RED_DIST_ARC_DICT)
 
 
 class REDDictFileBAC120(REDDictFile):
     """Store the RED dictionary for the BAC120 marker set."""
 
     def __init__(self, out_dir: str, prefix: str):
         path = os.path.join(out_dir, PATH_BAC120_RED_DICT.format(prefix=prefix))
-        super().__init__(path, RED_DIST_BAC_DICT)
+        super().__init__(path, CONFIG.RED_DIST_BAC_DICT)
```

### Comparing `gtdbtk-2.2.6/gtdbtk/files/stage_logger.py` & `gtdbtk-2.3.0/gtdbtk/files/stage_logger.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/files/tree_mapping.py` & `gtdbtk-2.3.0/gtdbtk/files/tree_mapping.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/infer_ranks.py` & `gtdbtk-2.3.0/gtdbtk/infer_ranks.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,15 @@
 
 import logging
 
 import dendropy
 
 from gtdbtk.biolib_lite.newick import parse_label, create_label
 from gtdbtk.biolib_lite.taxonomy import Taxonomy
-from gtdbtk.config.config import (TAXONOMY_FILE,
-                                  RED_DIST_BAC_DICT,
-                                  RED_DIST_ARC_DICT,
-                                  MRCA_RED_BAC120,
-                                  MRCA_RED_AR53,
-                                  RED_INTERVAL)
+from gtdbtk.config.common import CONFIG
 from gtdbtk.exceptions import GTDBTkExit
 from gtdbtk.relative_distance import RelativeDistance
 
 
 class InferRanks(object):
     """Establish taxonomic ranks of internal nodes using RED."""
 
@@ -39,15 +34,15 @@
 
         self.logger = logging.getLogger('timestamp')
 
     def _get_ingroup_domain(self, ingroup_taxon) -> str:
         """Get domain on ingroup taxon."""
 
         # read GTDB taxonomy in order to establish domain on ingroup taxon
-        gtdb_taxonomy = Taxonomy().read(TAXONOMY_FILE)
+        gtdb_taxonomy = Taxonomy().read(CONFIG.TAXONOMY_FILE)
         ingroup_domain = None
         for taxa in gtdb_taxonomy.values():
             if ingroup_taxon in taxa:
                 ingroup_domain = taxa[Taxonomy.DOMAIN_IDX]
 
         if ingroup_domain is None:
             raise GTDBTkExit(f'Ingroup taxon {ingroup_taxon} was not found in '
@@ -56,17 +51,17 @@
         return ingroup_domain
 
     def _get_median_reds(self, ingroup_domain: str):
         """Get median RED values for domain of ingroup taxon."""
 
         # get median RED values for domain
         if ingroup_domain == 'd__Bacteria':
-            median_reds = RED_DIST_BAC_DICT
+            median_reds = CONFIG.RED_DIST_BAC_DICT
         elif ingroup_domain == 'd__Archaea':
-            median_reds = RED_DIST_ARC_DICT
+            median_reds = CONFIG.RED_DIST_ARC_DICT
         else:
             raise GTDBTkExit(f'Unrecognized GTDB domain: {ingroup_domain}.')
 
         # report median values
         domain = ingroup_domain.replace('d__', '')
         self.logger.info('Median RED values for {}:'.format(domain))
         for idx, rank_prefix in enumerate(Taxonomy.rank_prefixes):
@@ -96,17 +91,17 @@
             raise GTDBTkExit(f'Ingroup taxon {ingroup_taxon} not found in tree.')
 
         return ingroup_node
 
     def _find_ingroup_red(self, ingroup_node, ingroup_domain, tree):
         """Find RED of the ingroup taxon."""
 
-        red_file = MRCA_RED_BAC120
+        red_file = CONFIG.MRCA_RED_BAC120
         if ingroup_domain == 'd__Archaea':
-            red_file = MRCA_RED_AR53
+            red_file = CONFIG.MRCA_RED_AR53
 
         # create map from leave labels to tree nodes
         leaf_node_map = {}
         for leaf in tree.leaf_node_iter():
             leaf_node_map[leaf.taxon.label] = leaf
 
         # find RED value of ingroup node
@@ -128,15 +123,15 @@
 
         red_ranks = {}
         for rank_prefix, median_red in median_reds.items():
             rank_idx = Taxonomy.rank_index[rank_prefix]
             rank_label = Taxonomy.rank_labels[rank_idx]
 
             abs_red_diff = abs(node_red - median_red)
-            if abs_red_diff <= RED_INTERVAL:
+            if abs_red_diff <= CONFIG.RED_INTERVAL:
                 red_ranks[rank_label] = abs_red_diff
 
         red_ranks_label = []
         for rank_label, abs_red_diff in sorted(red_ranks.items(), key=lambda kv: kv[1]):
             red_ranks_label.append(rank_label)
 
         return '&'.join(red_ranks_label)
```

### Comparing `gtdbtk-2.2.6/gtdbtk/main.py` & `gtdbtk-2.3.0/gtdbtk/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import sys
 import tempfile
 from datetime import datetime, timedelta
 from typing import Dict, Tuple
 
 from tqdm import tqdm
 
-import gtdbtk.config.config as Config
+from gtdbtk.config.common import CONFIG
 from gtdbtk.ani_rep import ANIRep
 from gtdbtk.ani_screen import ANIScreener
 from gtdbtk.biolib_lite.common import (check_dir_exists,
                                        check_file_exists,
                                        make_sure_path_exists,
                                        remove_extension)
 from gtdbtk.biolib_lite.execute import check_dependencies
@@ -82,28 +82,28 @@
             #timestamp_logger.info(f'{prog_name} {" ".join(sys.argv[1:])}')
 
         #setup the stage logger
         if output_dir is not None:
             self.stage_logger = StageLogger()
             self.stage_logger.version=self.version
             self.stage_logger.command_line=f'{prog_name} {" ".join(sys.argv[1:])}'
-            self.stage_logger.database_version = Config.VERSION_DATA
-            self.stage_logger.database_path=Config.GENERIC_PATH
+            self.stage_logger.database_version = CONFIG.VERSION_DATA
+            self.stage_logger.database_path=CONFIG.GENERIC_PATH
             self.stage_logger.output_dir=output_dir
             self.stage_logger.path = os.path.join(output_dir, "gtdbtk.json")
 
     def _check_package_compatibility(self):
         """Check that GTDB-Tk is using the most up-to-date reference package."""
-        pkg_ver = float(Config.VERSION_DATA.replace('r', ''))
-        min_ver = float(Config.MIN_REF_DATA_VERSION.replace('r', ''))
+        pkg_ver = float(CONFIG.VERSION_DATA.replace('r', ''))
+        min_ver = float(CONFIG.MIN_REF_DATA_VERSION.replace('r', ''))
         self.logger.info(f'Using GTDB-Tk reference data version '
-                         f'{Config.VERSION_DATA}: {Config.GENERIC_PATH}')
+                         f'{CONFIG.VERSION_DATA}: {CONFIG.GENERIC_PATH}')
         if pkg_ver < min_ver:
             self.logger.warning(colour(f'You are not using the reference data '
-                                       f'intended for this release: {Config.MIN_REF_DATA_VERSION}',
+                                       f'intended for this release: {CONFIG.MIN_REF_DATA_VERSION}',
                                        ['bright'], fg='yellow'))
 
     def _verify_genome_id(self, genome_id: str) -> bool:
         """Ensure genome ID will be valid in Newick tree.
 
         Parameters
         ----------
@@ -216,15 +216,15 @@
 
         return genomic_files, tln_tables
 
     def _read_taxonomy_files(self, options) -> Dict[str, Tuple[str, str, str, str, str, str, str]]:
         """Read and merge taxonomy files."""
 
         self.logger.info('Reading GTDB taxonomy for representative genomes.')
-        taxonomy = Taxonomy().read(Config.TAXONOMY_FILE)
+        taxonomy = Taxonomy().read(CONFIG.TAXONOMY_FILE)
 
         if options.gtdbtk_classification_file:
             # add and overwrite taxonomy for genomes specified in the
             # GTDB-Tk classification file
             check_file_exists(options.gtdbtk_classification_file)
 
             self.logger.info('Reading GTDB-Tk classification file.')
@@ -848,25 +848,25 @@
         decorate_step.output_files=reports
 
         if hasattr(self, 'stage_logger'):
             self.stage_logger.steps.append(decorate_step)
 
         self.logger.info('Done.')
 
-    def check_install(self):
+    def check_install(self,options):
         """ Verify all GTDB-Tk data files are present.
 
         Raises
         ------
         ReferenceFileMalformed
             If one or more reference files are malformed.
         """
         self.logger.info("Running install verification")
         misc = Misc()
-        misc.check_install()
+        misc.check_install(options.db_version)
         self.logger.info('Done.')
 
     def infer_ranks(self, options):
         """Establish taxonomic ranks of internal nodes using RED."""
 
         check_file_exists(options.input_tree)
 
@@ -907,14 +907,28 @@
         """
         check_file_exists(options.input_tree)
 
         r = Misc()
         r.convert_to_itol(options.input_tree, options.output_tree)
         self.logger.info('Done.')
 
+    def convert_to_species(self, options):
+        """Change GTDB genomes ids to GTDb species name in the tree.
+
+        Parameters
+        ----------
+        options : argparse.Namespace
+            The CLI arguments input by the user.
+        """
+        check_file_exists(options.input_tree)
+
+        r = Misc()
+        r.convert_to_species(options.input_tree, options.output_tree,options.custom_taxonomy_file,options.all_ranks)
+        self.logger.info('Done.')
+
     def remove_labels(self, options):
         """Remove labels from tree.
 
         Parameters
         ----------
         options : argparse.Namespace
             The CLI arguments input by the user.
@@ -1197,24 +1211,26 @@
             self.infer_ranks(options)
         elif options.subparser_name == 'ani_rep':
             self.ani_rep(options)
         elif options.subparser_name == 'remove_labels':
             self.remove_labels(options)
         elif options.subparser_name == 'convert_to_itol':
             self.convert_to_itol(options)
+        elif options.subparser_name == 'convert_to_species':
+            self.convert_to_species(options)
         elif options.subparser_name == 'trim_msa':
             self.trim_msa(options)
         elif options.subparser_name == 'export_msa':
             self.export_msa(options)
         elif options.subparser_name == 'test':
             check_dependencies(['prodigal', 'hmmalign', 'pplacer', 'guppy',
                                 'fastANI'])
             self.run_test(options)
         elif options.subparser_name == 'check_install':
-            self.check_install()
+            self.check_install(options)
         else:
             self.logger.error('Unknown GTDB-Tk command: "' +
                               options.subparser_name + '"\n')
             sys.exit(1)
 
 
         return 0
```

### Comparing `gtdbtk-2.2.6/gtdbtk/markers.py` & `gtdbtk-2.3.0/gtdbtk/markers.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from collections import defaultdict
 from shutil import copy
 from typing import Dict, Tuple, Optional
 
 import gzip
 import numpy as np
 
-import gtdbtk.config.config as Config
+from gtdbtk.config.common import CONFIG
 from gtdbtk.biolib_lite.common import make_sure_path_exists
 from gtdbtk.biolib_lite.execute import check_dependencies
 from gtdbtk.biolib_lite.seq_io import read_fasta
 from gtdbtk.biolib_lite.taxonomy import Taxonomy
 from gtdbtk.config.output import *
 from gtdbtk.exceptions import GenomeMarkerSetUnknown, MSAMaskLengthMismatch, InconsistentGenomeBatch, GTDBTkExit
 from gtdbtk.external.pfam_search import PfamSearch
@@ -61,21 +61,21 @@
 
         self.genome_file_suffix = GENOME_FILE_SUFFIX
         self.protein_file_suffix = PROTEIN_FILE_SUFFIX
         self.nt_gene_file_suffix = NT_GENE_FILE_SUFFIX
         self.gff_file_suffix = GFF_FILE_SUFFIX
         self.checksum_suffix = CHECKSUM_SUFFIX
 
-        self.taxonomy_file = Config.TAXONOMY_FILE
+        self.taxonomy_file = CONFIG.TAXONOMY_FILE
 
-        self.pfam_hmm_dir = Config.PFAM_HMM_DIR
+        self.pfam_hmm_dir = CONFIG.PFAM_HMM_DIR
         self.pfam_suffix = PFAM_SUFFIX
         self.pfam_top_hit_suffix = PFAM_TOP_HIT_SUFFIX
 
-        self.tigrfam_hmms = Config.TIGRFAM_HMMS
+        self.tigrfam_hmms = CONFIG.TIGRFAM_HMMS
         self.tigrfam_suffix = TIGRFAM_SUFFIX
         self.tigrfam_top_hit_suffix = TIGRFAM_TOP_HIT_SUFFIX
 
     def _report_identified_marker_genes(self, gene_dict, outdir, prefix,
                                         write_single_copy_genes,reports):
         """Report statistics for identified marker genes."""
 
@@ -119,19 +119,19 @@
         if write_single_copy_genes:
             fasta_dir = os.path.join(outdir, DIR_IDENTIFY_FASTA)
             self.logger.info(
                 f'Writing unaligned single-copy genes to: {fasta_dir}')
 
             # Iterate over each domain.
             marker_doms = list()
-            marker_doms.append((Config.AR53_MARKERS['PFAM'] +
-                                Config.AR53_MARKERS['TIGRFAM'],
+            marker_doms.append((CONFIG.AR53_MARKERS['PFAM'] +
+                                CONFIG.AR53_MARKERS['TIGRFAM'],
                                 ar53_copy_number_file, 'ar53'))
-            marker_doms.append((Config.BAC120_MARKERS['PFAM'] +
-                                Config.BAC120_MARKERS['TIGRFAM'],
+            marker_doms.append((CONFIG.BAC120_MARKERS['PFAM'] +
+                                CONFIG.BAC120_MARKERS['TIGRFAM'],
                                 bac120_copy_number_file, 'bac120'))
             for marker_names, marker_file, marker_d in marker_doms:
 
                 # Create the domain-specific subdirectory.
                 fasta_d_dir = os.path.join(fasta_dir, marker_d)
                 make_sure_path_exists(fasta_d_dir)
 
@@ -197,15 +197,15 @@
                                 self.failed_genomes,
                                 self.marker_gene_dir,
                                 self.protein_file_suffix,
                                 self.nt_gene_file_suffix,
                                 self.gff_file_suffix,
                                 force)
             self.logger.log(
-                Config.LOG_TASK, f'Running Prodigal {prodigal.version} to identify genes.')
+                CONFIG.LOG_TASK, f'Running Prodigal {prodigal.version} to identify genes.')
             genome_dictionary = prodigal.run(genomes, tln_tables)
 
         else:
             self.logger.info(
                 'Using supplied genomes as called genes, skipping Prodigal.')
             genome_dictionary = dict()
             for gid, gpath in genomes.items():
@@ -218,40 +218,40 @@
                 # we create a symlink to the genome file in the marker gene directory
                 # so we can use this symlink in the align step
                 symlink_protein_dir = os.path.join(self.marker_gene_dir, gid)
                 make_sure_path_exists(symlink_protein_dir)
                 symlink_f(os.path.abspath(gpath), os.path.join(symlink_protein_dir,gid+self.protein_file_suffix))
 
         # annotated genes against TIGRFAM and Pfam databases
-        self.logger.log(Config.LOG_TASK,
+        self.logger.log(CONFIG.LOG_TASK,
                         'Identifying TIGRFAM protein families.')
         gene_files = [(db_genome_id, genome_dictionary[db_genome_id]['aa_gene_path'])
                       for db_genome_id in genome_dictionary.keys()]
         tigr_search = TigrfamSearch(self.cpus,
                                     self.tigrfam_hmms,
                                     self.protein_file_suffix,
                                     self.tigrfam_suffix,
                                     self.tigrfam_top_hit_suffix,
                                     self.checksum_suffix,
                                     self.marker_gene_dir)
         tigr_search.run(gene_files)
 
-        self.logger.log(Config.LOG_TASK, 'Identifying Pfam protein families.')
+        self.logger.log(CONFIG.LOG_TASK, 'Identifying Pfam protein families.')
         pfam_search = PfamSearch(self.cpus,
                                  self.pfam_hmm_dir,
                                  self.protein_file_suffix,
                                  self.pfam_suffix,
                                  self.pfam_top_hit_suffix,
                                  self.checksum_suffix,
                                  self.marker_gene_dir)
         pfam_search.run(gene_files)
         self.logger.info(
             f'Annotations done using HMMER {tigr_search.version}.')
 
-        self.logger.log(Config.LOG_TASK,
+        self.logger.log(CONFIG.LOG_TASK,
                         'Summarising identified marker genes.')
         reports = self._report_identified_marker_genes(genome_dictionary, out_dir, prefix,
                                              write_single_copy_genes,reports)
 
         return reports
 
     def _path_to_identify_data(self, identity_dir, warn=True):
@@ -410,16 +410,16 @@
                 out_d[genome_id] = len(
                     marker_summary.get_single_copy_hits(genome_id))
 
         bac_gids = set()
         ar_gids = set()
         bac_ar_diff = {}
         for gid in bac_count:
-            arc_aa_per = (ar_count[gid] * 100.0 / Config.AR_MARKER_COUNT)
-            bac_aa_per = (bac_count[gid] * 100.0 / Config.BAC_MARKER_COUNT)
+            arc_aa_per = (ar_count[gid] * 100.0 / CONFIG.AR_MARKER_COUNT)
+            bac_aa_per = (bac_count[gid] * 100.0 / CONFIG.BAC_MARKER_COUNT)
             if bac_aa_per >= arc_aa_per:
                 bac_gids.add(gid)
             else:
                 ar_gids.add(gid)
             if abs(bac_aa_per - arc_aa_per) <= 10:
                 bac_ar_diff[gid] = {'bac120': round(
                     bac_aa_per, 1), 'ar53': round(arc_aa_per, 1)}
@@ -530,16 +530,16 @@
         #     align.concat_single_copy_hits(dir_tmp_arc,
         #                                   cur_gid_dict,
         #                                   ar53_marker_info_file)
         #
 
         self.logger.info(
             f'Aligning markers in {len(genomic_files):,} genomes with {self.cpus} CPUs.')
-        dom_iter = ((bac_gids, Config.CONCAT_BAC120, Config.MASK_BAC120, "bac120", 'bacterial', CopyNumberFileBAC120),
-                    (ar_gids, Config.CONCAT_AR53, Config.MASK_AR53, "ar53", 'archaeal', CopyNumberFileAR53))
+        dom_iter = ((bac_gids, CONFIG.CONCAT_BAC120, CONFIG.MASK_BAC120, "bac120", 'bacterial', CopyNumberFileBAC120),
+                    (ar_gids, CONFIG.CONCAT_AR53, CONFIG.MASK_AR53, "ar53", 'archaeal', CopyNumberFileAR53))
 
         # For some genomes, it is possible to have no markers.
         no_marker_gids = bac_gids.union(ar_gids)
 
         gtdb_taxonomy = Taxonomy().read(self.taxonomy_file)
         for gids, msa_file, mask_file, marker_set_id, domain_str, copy_number_f in dom_iter:
 
@@ -572,15 +572,15 @@
             if skip_gtdb_refs:
                 gtdb_msa = {}
             else:
                 gtdb_msa = self._msa_filter_by_taxa(msa_file,
                                                     gtdb_taxonomy,
                                                     taxa_filter,
                                                     outgroup_taxon)
-            gtdb_msa_mask = os.path.join(Config.MASK_DIR, mask_file)
+            gtdb_msa_mask = os.path.join(CONFIG.MASK_DIR, mask_file)
 
             # Generate the user MSA.
             user_msa = align.align_marker_set(
                 cur_genome_files, marker_info_file, copy_number_f, self.cpus)
 
 
             # tmp_gids = bac_gids.difference(set(user_msa.keys()))
@@ -637,15 +637,15 @@
 
                 filtered_user_genomes = set(
                     pruned_seqs).intersection(user_msa)
                 if len(filtered_user_genomes):
                     self.logger.info(
                         f'Filtered genomes include {len(filtered_user_genomes)} user submitted genomes.')
             else:
-                self.logger.log(Config.LOG_TASK,
+                self.logger.log(CONFIG.LOG_TASK,
                                 f'Masking columns of {domain_str} multiple sequence alignment using canonical mask.')
                 trimmed_seqs, pruned_seqs = self._apply_mask(gtdb_msa,
                                                             user_msa,
                                                            gtdb_msa_mask,
                                                             min_perc_aa / 100.0)
                 self.logger.info('Masked {} alignment from {:,} to {:,} AAs.'.format(
                     domain_str,
```

### Comparing `gtdbtk-2.2.6/gtdbtk/misc.py` & `gtdbtk-2.3.0/gtdbtk/misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 import logging
 import os
 
 import shutil
 
 import dendropy
 
-import gtdbtk.config.config as Config
+from gtdbtk.biolib_lite.taxonomy import Taxonomy
+from gtdbtk.config.common import CONFIG
 from gtdbtk.biolib_lite.execute import check_dependencies
 from gtdbtk.biolib_lite.logger import colour
 from gtdbtk.biolib_lite.newick import parse_label
 from gtdbtk.biolib_lite.seq_io import read_fasta
 from gtdbtk.config.output import DIR_CLASSIFY_INTERMEDIATE, DIR_ALIGN_INTERMEDIATE, DIR_IDENTIFY_INTERMEDIATE
 from gtdbtk.exceptions import GTDBTkException, GTDBTkExit
 from gtdbtk.tools import sha1_dir
@@ -49,17 +50,17 @@
             Which mask should be used, reference or user specified.
         maskid : str
             The path to the mask used for trimming.
         output_file : str
             The path to the output trimmed MSA.
         """
         if maskid == 'bac' and mask_type == 'reference':
-            mask = os.path.join(Config.MASK_DIR, Config.MASK_BAC120)
+            mask = os.path.join(CONFIG.MASK_DIR, CONFIG.MASK_BAC120)
         elif maskid == 'arc' and mask_type == 'reference':
-            mask = os.path.join(Config.MASK_DIR, Config.MASK_AR53)
+            mask = os.path.join(CONFIG.MASK_DIR, CONFIG.MASK_AR53)
         elif mask_type == 'file':
             mask = maskid
         else:
             self.logger.error('Command not understood.')
             raise GTDBTkException('Command not understood.')
 
         with open(mask, 'r') as f:
@@ -154,14 +155,60 @@
                     label = label.replace('; ',';').replace(';','|').replace("'","").lstrip('')
                 node.label = label
                 if node.edge.length:
                     node.edge.length = f'{node.edge.length}[{bootstrap}]'
 
         intree.write_to_path(output_file, schema='newick', suppress_rooting=True,unquoted_underscores=True)
 
+    def convert_to_species(self, input_file, output_file,custom_taxonomy_file=None,all_ranks=False):
+        """Change GTDB genomes ids to GTDb species name in the tree.
+
+        Parameters
+        ----------
+        input_file : str
+            The path to the input Newick tree.
+        output_file : str
+            The path to the output Newick tree.
+        """
+
+        self.logger.info("Convert GTDB-Tk tree...")
+        intree= dendropy.Tree.get_from_path(input_file,
+                                           schema='newick',
+                                           rooting='force-rooted',
+                                           preserve_underscores=True)
+
+        # get all leaves from the tree
+        leaves = intree.leaf_nodes()
+        #load the taxonomy file
+        taxonomy = Taxonomy().read(CONFIG.TAXONOMY_FILE)
+        #load the custom taxonomy file
+        if custom_taxonomy_file:
+            self.logger.info("Loading custom taxonomy file...")
+            custom_taxonomy = Taxonomy().read(custom_taxonomy_file)
+            #check intersection between custom taxonomy and taxonomy
+            intersection = set(custom_taxonomy.keys()).intersection(set(taxonomy.keys()))
+            if len(intersection) > 0:
+                self.logger.warning("{} genomes are present in both custom taxonomy and taxonomy file. The custom taxonomy will be used.".format(len(intersection)))
+            #update taxonomy with custom taxonomy
+            taxonomy.update(custom_taxonomy)
+
+
+        #get the species name for each genome
+        for leaf in leaves:
+            if leaf.taxon.label in taxonomy:
+                # get the label from parent node
+                if all_ranks:
+                    leaf.taxon.label = ';'.join(taxonomy[leaf.taxon.label])
+                else:
+                    leaf.taxon.label = taxonomy[leaf.taxon.label][-1]
+
+        #write the tree
+        intree.write_to_path(output_file, schema='newick', suppress_rooting=True,unquoted_underscores=True)
+
+
 
     def remove_intermediate_files(self,output_dir,wf_name):
         """Remove intermediate files.
 
         Parameters
         ----------
         output_dir : str
@@ -186,15 +233,15 @@
         elif wf_name == 'de_novo_wf':
             #Remove classify step intermediate files
             intermediate_infer = os.path.join(output_dir, DIR_ALIGN_INTERMEDIATE)
             if os.path.exists(intermediate_infer) and os.path.isdir(intermediate_infer):
                 shutil.rmtree(intermediate_infer)
         self.logger.info('Intermediate files removed.')
 
-    def check_install(self):
+    def check_install(self,db_version):
         """Check that all reference files exist.
 
         Returns
         -------
         bool
             True if the installation is complete, False otherwise.
         """
@@ -216,16 +263,18 @@
                 self.logger.info("         |-- {:16} {}".format(
                     name, colour('NOT FOUND', ['bright'], fg='yellow')))
 
         # Assume this was successful unless otherwise observed.
         ok = True
 
         # Compute the hash for each directory
-        self.logger.info(f'Checking integrity of reference package: {Config.GENERIC_PATH}')
-        for obj_path, expected_hash in Config.REF_HASHES.items():
+        self.logger.info(f'Checking integrity of reference package: {CONFIG.GENERIC_PATH}')
+        ref_hashes = CONFIG.get_REF_HASHES(db_version)
+
+        for obj_path, expected_hash in ref_hashes.items():
             base_name = obj_path[:-1] if obj_path.endswith('/') else obj_path
             base_name = base_name.split('/')[-1]
             user_hash = sha1_dir(obj_path, progress=True)
 
             if user_hash != expected_hash:
                 self.logger.info("         |-- {:16} {}".format(
                     base_name, colour(f'HASH MISMATCH {user_hash}', ['bright'], fg='yellow')))
```

### Comparing `gtdbtk-2.2.6/gtdbtk/pipeline/align.py` & `gtdbtk-2.3.0/gtdbtk/pipeline/align.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import multiprocessing as mp
 import os
 import subprocess
 import tempfile
 from collections import defaultdict
 
-from gtdbtk.config.config import LOG_TASK
+from gtdbtk.config.common import CONFIG
 from gtdbtk.exceptions import GTDBTkExit
 from gtdbtk.external.hmm_aligner import HmmAligner
 from gtdbtk.files.marker.copy_number import CopyNumberFile
 from gtdbtk.files.marker.tophit import TopHitPfamFile, TopHitTigrFile
 from gtdbtk.files.marker_info import MarkerInfoFile
 from gtdbtk.tools import tqdm_log
 
@@ -211,30 +211,30 @@
     Returns
     -------
     Dict[str, str]
         dict[gid] = sequence
     """
     logger = logging.getLogger('timestamp')
 
-    logger.log(LOG_TASK, f'Generating concatenated alignment for each marker.')
+    logger.log(CONFIG.LOG_TASK, f'Generating concatenated alignment for each marker.')
     single_copy_hits = get_single_copy_hits(gid_dict, copy_number_file, cpus)
 
     with tempfile.TemporaryDirectory(prefix='gtdbtk_tmp_') as dir_tmp:
         # Write each of the markers to disk.
         marker_paths = dict()
         for marker_id, marker_d in single_copy_hits.items():
             cur_path = os.path.join(dir_tmp, f'{marker_id}.fa')
             marker_paths[marker_id] = cur_path
             with open(cur_path, 'w') as fh:
                 for cur_gid, cur_seq in marker_d.items():
                     fh.write(f'>{cur_gid}\n{cur_seq}\n')
 
         # Run hmmalign on all of the markers (in order of largest)
         hmmer_v = HmmAligner.get_version()
-        logger.log(LOG_TASK, f'Aligning {len(marker_paths)} identified markers using hmmalign {hmmer_v}.')
+        logger.log(CONFIG.LOG_TASK, f'Aligning {len(marker_paths)} identified markers using hmmalign {hmmer_v}.')
         queue = list()
         for marker_id, marker_path in sorted(marker_paths.items(),
                                              key=lambda z: -marker_info_file.markers[z[0]]['size']):
             queue.append((marker_id,
                           marker_info_file.markers[marker_id]['path'],
                           marker_path,
                           frozenset(single_copy_hits[marker_id])))
```

### Comparing `gtdbtk-2.2.6/gtdbtk/pipeline/export_msa.py` & `gtdbtk-2.3.0/gtdbtk/pipeline/export_msa.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 from shutil import copyfile
 
 from gtdbtk.biolib_lite.common import make_sure_path_exists
-from gtdbtk.config.config import CONCAT_AR53, CONCAT_BAC120
+from gtdbtk.config.common import CONFIG
 from gtdbtk.exceptions import GTDBTkExit
 from gtdbtk.model.enum import Domain
 
 
 def export_msa(domain: Domain, output_file: str):
     """Exports the GTDB MSA to the specified path.
 
     :param domain: The domain used to determine the marker set.
     :param output_file: The path to write the MSA.
     """
     if domain is Domain.ARCHAEA:
-        file_to_export = CONCAT_AR53
+        file_to_export = CONFIG.CONCAT_AR53
     elif domain is Domain.BACTERIA:
-        file_to_export = CONCAT_BAC120
+        file_to_export = CONFIG.CONCAT_BAC120
     else:
         raise GTDBTkExit(f'Unknown domain: "{domain}"')
 
     make_sure_path_exists(os.path.dirname(output_file))
     copyfile(file_to_export, output_file)
```

### Comparing `gtdbtk-2.2.6/gtdbtk/relative_distance.py` & `gtdbtk-2.3.0/gtdbtk/relative_distance.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/reroot_tree.py` & `gtdbtk-2.3.0/gtdbtk/reroot_tree.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/split.py` & `gtdbtk-2.3.0/gtdbtk/split.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #    along with this program. If not, see <http://www.gnu.org/licenses/>.     #
 #                                                                             #
 ###############################################################################
 import os
 
 import logging
 
-import gtdbtk.config.config as Config
+from gtdbtk.config.common import CONFIG
 from gtdbtk.biolib_lite.common import make_sure_path_exists
 from gtdbtk.biolib_lite.newick import parse_label
 from gtdbtk.biolib_lite.seq_io import read_fasta
 from gtdbtk.config.output import *
 from gtdbtk.exceptions import GenomeMarkerSetUnknown, GTDBTkExit
 from gtdbtk.files.classify_summary import ClassifySummaryFileRow
 from gtdbtk.files.pplacer_classification import PplacerHighClassifyRow, PplacerHighClassifyFile
@@ -65,15 +65,15 @@
 
         if marker_set_id == 'bac120':
             out_pplacer = PplacerHighClassifyFile(out_dir,prefix)
         else:
             self.logger.error('There was an error determining the marker set.')
             raise GenomeMarkerSetUnknown
 
-        red_bac_dict = Config.RED_DIST_BAC_DICT
+        red_bac_dict = CONFIG.RED_DIST_BAC_DICT
 
         # We get the pplacer taxonomy for comparison
         user_genome_ids = set(read_fasta(user_msa_file).keys())
         for leaf in tree.leaf_node_iter():
 
             is_on_terminal_branch = False
             terminal_branch_test = False
```

### Comparing `gtdbtk-2.2.6/gtdbtk/tests/data/genomes/genome_1.fna` & `gtdbtk-2.3.0/gtdbtk/tests/data/genomes/genome_1.fna`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/tests/data/genomes/genome_2.fna` & `gtdbtk-2.3.0/gtdbtk/tests/data/genomes/genome_2.fna`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/tests/data/genomes/genome_3.fna` & `gtdbtk-2.3.0/gtdbtk/tests/data/genomes/genome_3.fna`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk/tools.py` & `gtdbtk-2.3.0/gtdbtk/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import time
 import urllib.request
 from itertools import islice
 
 import dendropy
 from tqdm import tqdm
 
-import gtdbtk.config.config as Config
+from gtdbtk.config.common import CONFIG
 from gtdbtk.config.output import CHECKSUM_SUFFIX
 from gtdbtk.exceptions import GTDBTkExit
 
 order_rank = ["d__", "p__", "c__", "o__", 'f__', 'g__', 's__']
 ##################################################
 ############MISC UTILITIES########################
 ##################################################
@@ -30,15 +30,15 @@
 
     Returns
     -------
     frozenset
         An immutable set with short and long accessions (e.g. GB_GCA_ and GCA_).
     """
     results = set()
-    with open(Config.TAXONOMY_FILE) as tf:
+    with open(CONFIG.TAXONOMY_FILE) as tf:
         for line in tf:
             raw_id = line.split('\t')[0]
             results.add(raw_id)
             if raw_id[0:4] in ['GCF_', 'GCA_']:
                 results.add(add_ncbi_prefix(raw_id))
             elif raw_id[0:3] in ['RS_', 'GB_']:
                 results.add(raw_id[3:])
@@ -49,20 +49,20 @@
 
     Returns
     -------
     dict[str, str]
         Dict[genome_id] = fasta_path
     """
     ref_genomes = dict()
-    with open(Config.FASTANI_GENOME_LIST) as g_path_file:
+    with open(CONFIG.FASTANI_GENOME_LIST) as g_path_file:
         for line in g_path_file:
             (full_name, path) = line.strip().split()
-            if full_name.endswith(Config.FASTANI_GENOMES_EXT):
-                accession = full_name.split(Config.FASTANI_GENOMES_EXT)[0]
-            ref_genomes[accession] = os.path.join(Config.FASTANI_DIR, path, full_name)
+            if full_name.endswith(CONFIG.FASTANI_GENOMES_EXT):
+                accession = full_name.split(CONFIG.FASTANI_GENOMES_EXT)[0]
+            ref_genomes[accession] = os.path.join(CONFIG.FASTANI_DIR, path, full_name)
     return ref_genomes
 
 def aa_percent_msa(aa_string):
         aa_len = sum([1 for c in aa_string if c.isalpha()])
         aa_perc = float(aa_len) / len(aa_string)
         return round(aa_perc * 100, 2)
 
@@ -286,19 +286,19 @@
         virt = int(re.search(r'VmSize:[^\d]+(\d+)', contents).group(1)) / 1e6
         res = int(re.search(r'VmRSS:[^\d]+(\d+)', contents).group(1)) / 1e6
     finally:
         return virt, res
 
 
 def get_gtdbtk_latest_version():
-    if not Config.GTDBTK_VER_CHECK:
+    if not CONFIG.GTDBTK_VER_CHECK:
         return None
     try:
         resp = json.loads(urllib.request.urlopen('https://pypi.org/pypi/gtdbtk/json',
-                                                 timeout=Config.GTDBTK_VER_TIMEOUT).read().decode('utf-8'))
+                                                 timeout=CONFIG.GTDBTK_VER_TIMEOUT).read().decode('utf-8'))
         return resp['info']['version']
     except Exception:
         return None
 
 
 class TreeTraversal(object):
     """Efficiently calculates leaf nodes of a given node without re-computing
```

### Comparing `gtdbtk-2.2.6/gtdbtk/trim_msa.py` & `gtdbtk-2.3.0/gtdbtk/trim_msa.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/gtdbtk.egg-info/PKG-INFO` & `gtdbtk-2.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: gtdbtk
-Version: 2.2.6
-Summary: A toolkit for assigning objective taxonomic classifications to bacterial and archaeal genomes.
-Home-page: https://github.com/Ecogenomics/GTDBTk
-Author: Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks
-Author-email: p.chaumeil@uq.edu.au
-Maintainer: Pierre-Alain Chaumeil, Aaron Mussig and Donovan Parks
-Maintainer-email: donovan.parks@gmail.com
-License: GPL3
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # GTDB-Tk
 
 [![PyPI](https://img.shields.io/pypi/v/gtdbtk.svg)](https://pypi.python.org/pypi/gtdbtk)
 [![PyPI Downloads](https://pepy.tech/badge/gtdbtk)](https://pepy.tech/project/gtdbtk)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/gtdbtk.svg?color=43b02a)](https://anaconda.org/bioconda/gtdbtk)
 [![BioConda Downloads](https://img.shields.io/conda/dn/bioconda/gtdbtk.svg?style=flag&label=downloads&color=43b02a)](https://anaconda.org/bioconda/gtdbtk)
 [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/ecogenomic/gtdbtk?sort=date&color=299bec&label=docker)](https://hub.docker.com/r/ecogenomic/gtdbtk)
@@ -56,21 +33,17 @@
 ## 📖 Documentation
 
 Documentation for GTDB-Tk can be found [here](https://ecogenomics.github.io/GTDBTk/).
 
 
 ## ✨ New Features
 
-GTDB-Tk v2.2.0+ includes the following new features:
-- GTDB-TK `classify` and `classify_wf` have changed in version 2.2.0+. There is now an ANI classification stage (`ANI screen`) that precedes classification by placement in a reference tree.
-  - **This is now the default behavior for `classify` and `classify_wf`.**
-  - In `classify`, user genomes are first compared against a Mash database comprised of all GTDB representative genomes and genome pairs of sufficient similarity processed by FastANI. User genomes classified to a GTDB representative based on FastANI results are not run through pplacer. 
-  - In the `classify_wf` workflow, genomes are classified using Mash and FastANI before executing the identify step. User genomes classified with FastANI are not run through the remainder of the pipeline (identify, align, classify).
-  - `classify_wf` and `classify` have now **an extra mutually exclusive required argument**: You can either pick `--skip_ani_screen` (to skip the ani_screening step to classify genomes using mash and FastANI) or `--mash_db` path to save/read (if exists) the Mash reference sketch database.
-  - To classify genomes without the additional `ani_screen` step, use the `--skip_ani_screen` flag.
+GTDB-Tk v2.3.0+ includes the following new features:
+- New functionality ``convert_to_species`` function to convert GTDB genome IDs to GTDB species names
+
 
 ## 📈 Performance
 Using ANI screen "can" reduce computation by >50%, although it depends on the set of input genomes. A set of input genomes consisting primarily of new species will not benefit from ANI screen as much as a set of genomes that are largely assigned to GTDB species clusters. In the latter case, the ANI screen will reduce the number of genomes that need to be classified by pplacer which reduces computation time substantially (between 25% and 60% in our testing).
 
 ## 📚 References
 
 GTDB-Tk is described in:
```

### Comparing `gtdbtk-2.2.6/gtdbtk.egg-info/SOURCES.txt` & `gtdbtk-2.3.0/gtdbtk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 gtdbtk/biolib_lite/logger.py
 gtdbtk/biolib_lite/newick.py
 gtdbtk/biolib_lite/parallel.py
 gtdbtk/biolib_lite/prodigal_biolib.py
 gtdbtk/biolib_lite/seq_io.py
 gtdbtk/biolib_lite/taxonomy.py
 gtdbtk/config/__init__.py
-gtdbtk/config/config.py
+gtdbtk/config/common.py
 gtdbtk/config/output.py
 gtdbtk/external/__init__.py
 gtdbtk/external/fastani.py
 gtdbtk/external/fasttree.py
 gtdbtk/external/hmm_aligner.py
 gtdbtk/external/mash.py
 gtdbtk/external/pfam_search.py
```

### Comparing `gtdbtk-2.2.6/setup.py` & `gtdbtk-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/tests/common.py` & `gtdbtk-2.3.0/tests/common.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/tests/test_classify.py` & `gtdbtk-2.3.0/tests/test_classify.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import os
 import shutil
 import tempfile
 import unittest
 
 import dendropy
 
-import gtdbtk.config.config as Config
+from gtdbtk.config.common import CONFIG
 from gtdbtk.biolib_lite.taxonomy import Taxonomy
 from gtdbtk.classify import Classify
 from gtdbtk.config.output import *
 from gtdbtk.files.pplacer_classification import PplacerClassifyFileAR53
 
 
 class TestClassify(unittest.TestCase):
@@ -34,15 +34,15 @@
     def setUp(self):
         self.classify = Classify()
         self.out_dir = tempfile.mkdtemp(prefix='gtdbtk_tmp_')
         self.prefix = 'gtdbtk'
         self.pplacer_dir_reference = 'tests/data/pplacer_dir_reference'
         self.aln_dir_ref = 'tests/data/align_dir_reference/align'
         self.user_msa_file = os.path.join(self.aln_dir_ref, 'gtdbtk.ar53.user_msa.fasta')
-        self.taxonomy_file = Config.TAXONOMY_FILE
+        self.taxonomy_file = CONFIG.TAXONOMY_FILE
         self.gtdb_taxonomy = Taxonomy().read(self.taxonomy_file)
 
     def tearDown(self):
         shutil.rmtree(self.out_dir)
 
     def test_standardise_taxonomy(self):
         taxstring = 'p__phylum1;c_class1'
```

### Comparing `gtdbtk-2.2.6/tests/test_cli.py` & `gtdbtk-2.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/tests/test_gtdbtk/test__main__.py` & `gtdbtk-2.3.0/tests/test_gtdbtk/test__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ###############################################################################
 import os
 import random
 import subprocess
 import tempfile
 import unittest
 
-from gtdbtk.config.config import CONCAT_AR53, CONCAT_BAC120, MASK_AR53, MASK_DIR, MASK_BAC120
+from gtdbtk.config.common import CONFIG
 from gtdbtk.files.classify_summary import ClassifySummaryFileAR53
 from gtdbtk.tools import sha256
 
 
 class TestMain(unittest.TestCase):
     """Used to test the CLI. Currently just checks all exit codes."""
 
@@ -172,22 +172,22 @@
                 '--out_dir', self.dir_tmp, '--cpus', self.cpus]
         proc = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE, encoding='utf-8')
         stdout, stderr = proc.communicate()
         self.assertEqual(proc.returncode, 0)
 
     def test_trim_msa(self):
         path_out = os.path.join(self.dir_tmp, 'msa.faa')
-        args = ['python', '-m', 'gtdbtk', 'trim_msa', '--untrimmed_msa', CONCAT_AR53,
+        args = ['python', '-m', 'gtdbtk', 'trim_msa', '--untrimmed_msa', CONFIG.CONCAT_AR53,
                 '--output', path_out, '--reference_mask', 'arc']
         proc = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE, encoding='utf-8')
         stdout, stderr = proc.communicate()
         self.assertEqual(proc.returncode, 0)
 
     def test_trim_msa_reference_mask_arc(self):
-        with open(os.path.join(MASK_DIR, MASK_AR53), 'r') as f:
+        with open(os.path.join(CONFIG.MASK_DIR, CONFIG.MASK_AR53), 'r') as f:
             mask = [x == '1' for x in f.read().strip()]
 
         path_untrimmed_msa = os.path.join(self.dir_tmp, 'untrimmed_msa.fasta')
         path_output = os.path.join(self.dir_tmp, 'trimmed_msa.fasta')
 
         choices = 'ARNDCQEGHILKMFPSTWYV-'
         expected = list()
@@ -213,15 +213,15 @@
                 results[gid] = seq
 
         expected = {'test123': ''.join(expected)}
 
         self.assertDictEqual(results, expected)
 
     def test_trim_msa_reference_mask_bac(self):
-        with open(os.path.join(MASK_DIR, MASK_BAC120), 'r') as f:
+        with open(os.path.join(CONFIG.MASK_DIR, CONFIG.MASK_BAC120), 'r') as f:
             mask = [x == '1' for x in f.read().strip()]
 
         path_untrimmed_msa = os.path.join(self.dir_tmp, 'untrimmed_msa.fasta')
         path_output = os.path.join(self.dir_tmp, 'trimmed_msa.fasta')
 
         choices = 'ARNDCQEGHILKMFPSTWYV-'
         expected = list()
@@ -286,27 +286,27 @@
         path_output = os.path.join(self.dir_tmp, 'msa.faa')
         args = ['python', '-m', 'gtdbtk', 'export_msa', '--domain', 'arc', '--output', path_output]
         p = subprocess.Popen(args)
         p.wait()
         self.assertEqual(p.returncode, 0)
 
         test_hash = sha256(path_output)
-        true_hash = sha256(CONCAT_AR53)
+        true_hash = sha256(CONFIG.CONCAT_AR53)
         self.assertEqual(test_hash, true_hash)
 
     def test_export_msa_bac(self):
         """Test that the MSA can be exported when using the CLI."""
         path_output = os.path.join(self.dir_tmp, 'msa.faa')
         args = ['python', '-m', 'gtdbtk', 'export_msa', '--domain', 'bac', '--output', path_output]
         p = subprocess.Popen(args)
         p.wait()
         self.assertEqual(p.returncode, 0)
 
         test_hash = sha256(path_output)
-        true_hash = sha256(CONCAT_BAC120)
+        true_hash = sha256(CONFIG.CONCAT_BAC120)
         self.assertEqual(test_hash, true_hash)
 
     def test_test(self):
         args = ['python', '-m', 'gtdbtk', 'test', '--out_dir', self.dir_tmp, '--cpus', self.cpus]
         proc = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE, encoding='utf-8')
         stdout, stderr = proc.communicate()
         self.assertEqual(proc.returncode, 0)
```

### Comparing `gtdbtk-2.2.6/tests/test_gtdbtk/test_biolib_lite/test_common.py` & `gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/test_common.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/tests/test_gtdbtk/test_biolib_lite/test_newick.py` & `gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/test_newick.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/tests/test_gtdbtk/test_biolib_lite/test_seq_io.py` & `gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/test_seq_io.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/tests/test_gtdbtk/test_biolib_lite/test_taxonomy.py` & `gtdbtk-2.3.0/tests/test_gtdbtk/test_biolib_lite/test_taxonomy.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/tests/test_gtdbtk/test_external/test_fastani.py` & `gtdbtk-2.3.0/tests/test_gtdbtk/test_external/test_fastani.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 ###############################################################################
 import os
 import shutil
 import tempfile
 import unittest
 import json
 from gtdbtk.external.fastani import FastANI
-import gtdbtk.config.config as Config
+from gtdbtk.config.common import CONFIG
 
 class TestFastANI(unittest.TestCase):
 
     def setUp(self):
         self.dir_tmp = tempfile.mkdtemp(prefix='gtdbtk_tmp_')
         self.cpus = 1
-        self.genome_root = Config.FASTANI_GENOMES
+        self.genome_root = CONFIG.FASTANI_GENOMES
 
     def tearDown(self):
         shutil.rmtree(self.dir_tmp)
 
     def test_run(self):
         """Test that FastANI produces the expected output (version dependent)"""
```

### Comparing `gtdbtk-2.2.6/tests/test_gtdbtk/test_external/test_fasttree.py` & `gtdbtk-2.3.0/tests/test_gtdbtk/test_external/test_fasttree.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 #                                                                             #
 ###############################################################################
 import os
 import shutil
 import tempfile
 import unittest
 
-import gtdbtk.config.config as Config
+from gtdbtk.config.common import CONFIG
 from gtdbtk.external.fasttree import FastTree
 
 
 class TestFastTree(unittest.TestCase):
 
     def setUp(self):
         self.dir_tmp = tempfile.mkdtemp(prefix='gtdbtk_tmp_')
         self.cpus = 1
-        self.genome_root = Config.FASTANI_GENOMES
+        self.genome_root = CONFIG.FASTANI_GENOMES
         self.test_msa = 'tests/data/example.faa'
         self.test_msa_gz = 'tests/data/example.faa.gz'
 
     def tearDown(self):
         shutil.rmtree(self.dir_tmp)
 
     def test_run(self):
```

### Comparing `gtdbtk-2.2.6/tests/test_gtdbtk/test_files/test_marker/test_copy_number.py` & `gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_marker/test_copy_number.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/tests/test_gtdbtk/test_files/test_marker/test_tophit.py` & `gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_marker/test_tophit.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/tests/test_gtdbtk/test_files/test_prodigal/test_tln_table_summary.py` & `gtdbtk-2.3.0/tests/test_gtdbtk/test_files/test_prodigal/test_tln_table_summary.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/tests/test_gtdbtk/test_main.py` & `gtdbtk-2.3.0/tests/test_gtdbtk/test_main.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/tests/test_gtdbtk/test_markers.py` & `gtdbtk-2.3.0/tests/test_gtdbtk/test_markers.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/tests/test_gtdbtk/test_tools.py` & `gtdbtk-2.3.0/tests/test_gtdbtk/test_tools.py`

 * *Files identical despite different names*

### Comparing `gtdbtk-2.2.6/tests/test_gtdbtk/test_trim_msa.py` & `gtdbtk-2.3.0/tests/test_gtdbtk/test_trim_msa.py`

 * *Files identical despite different names*

