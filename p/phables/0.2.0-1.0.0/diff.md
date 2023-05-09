# Comparing `tmp/phables-0.2.0.tar.gz` & `tmp/phables-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phables-0.2.0.tar", last modified: Wed Feb 22 00:21:03 2023, max compression
+gzip compressed data, was "phables-1.0.0.tar", last modified: Tue May  9 03:51:30 2023, max compression
```

## Comparing `phables-0.2.0.tar` & `phables-1.0.0.tar`

### file list

```diff
@@ -1,67 +1,107 @@
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-22 00:21:03.346918 phables-0.2.0/
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     1079 2023-02-16 03:08:21.000000 phables-0.2.0/LICENSE
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)      125 2023-02-16 03:08:21.000000 phables-0.2.0/MANIFEST.in
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6646 2023-02-22 00:21:03.345955 phables-0.2.0/PKG-INFO
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     6000 2023-02-16 03:08:21.000000 phables-0.2.0/README.md
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-22 00:21:03.317337 phables-0.2.0/phables/
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-16 03:08:21.000000 phables-0.2.0/phables/__init__.py
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     8315 2023-02-16 03:08:21.000000 phables-0.2.0/phables/__main__.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-22 00:21:03.320182 phables-0.2.0/phables/config/
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)      293 2023-02-16 03:08:21.000000 phables-0.2.0/phables/config/config.yaml
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)      533 2023-02-16 03:08:21.000000 phables-0.2.0/phables/config/databases.yaml
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)      242 2023-02-16 03:08:21.000000 phables-0.2.0/phables/phables.CITATION
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     1081 2023-02-16 03:08:21.000000 phables-0.2.0/phables/phables.LICENSE
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)        5 2023-02-16 03:08:21.000000 phables-0.2.0/phables/phables.VERSION
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-22 00:21:03.322846 phables-0.2.0/phables/test_data/
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)    18772 2023-02-16 03:08:21.000000 phables-0.2.0/phables/test_data/assembly_graph.gfa
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)      131 2023-02-16 03:08:21.000000 phables-0.2.0/phables/test_data/edge_coverages.tsv
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)      587 2023-02-16 03:08:21.000000 phables-0.2.0/phables/test_data/edges.fasta.hmmout
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)      122 2023-02-16 03:08:21.000000 phables-0.2.0/phables/test_data/junction_pe_coverage.pickle
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)      272 2023-02-16 03:08:21.000000 phables-0.2.0/phables/test_data/phrogs_annotations.tsv
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     4928 2023-02-16 03:08:21.000000 phables-0.2.0/phables/util.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-22 00:21:03.324564 phables-0.2.0/phables/workflow/
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-22 00:21:03.326605 phables-0.2.0/phables/workflow/envs/
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)       59 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/envs/curl.yaml
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)       94 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/envs/mapping.yaml
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)       71 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/envs/mmseqs.yaml
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)      257 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/envs/phables.yaml
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)       74 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/envs/smg.yaml
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     1763 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/install.smk
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     1696 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/phables.smk
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-22 00:21:03.330276 phables-0.2.0/phables/workflow/rules/
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)      799 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/rules/00_database_preflight.smk
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     2159 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/rules/02_phables_preflight.smk
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     1321 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/rules/02_phables_targets.smk
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)      920 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/rules/03_test_preflight.smk
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)      592 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/rules/03_test_targets.smk
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     1341 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/rules/coverm.smk
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     2109 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/rules/genes.smk
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)      569 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/rules/gfa2fasta.smk
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)      802 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/rules/mapping.smk
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     1172 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/rules/phables.smk
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-22 00:21:03.331249 phables-0.2.0/phables/workflow/scripts/
--rwxrwxr-x   0 vijinimallawaarachchi   (501) staff       (20)     2630 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/scripts/combine_cov.py
--rwxrwxr-x   0 vijinimallawaarachchi   (501) staff       (20)     3358 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/scripts/gfa2fasta.py
--rwxrwxr-x   0 vijinimallawaarachchi   (501) staff       (20)    33055 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/scripts/phables.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-22 00:21:03.334707 phables-0.2.0/phables/workflow/scripts/phables_utils/
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     8077 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/scripts/phables_utils/FD_Inexact.py
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/scripts/phables_utils/__init__.py
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     2586 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/scripts/phables_utils/component_utils.py
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     3413 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/scripts/phables_utils/coverage_utils.py
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     6480 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/scripts/phables_utils/edge_graph_utils.py
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     1760 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/scripts/phables_utils/flow_utils.py
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     2959 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/scripts/phables_utils/gene_utils.py
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     1762 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/scripts/phables_utils/genome_utils.py
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     5343 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/scripts/phables_utils/output_utils.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-22 00:21:03.335214 phables-0.2.0/phables/workflow/scripts/phables_utils/phrogs/
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)  3831481 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/scripts/phables_utils/phrogs/phrog_annot.tsv
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     2557 2023-02-16 03:08:21.000000 phables-0.2.0/phables/workflow/test_phables.smk
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-02-22 00:21:03.319533 phables-0.2.0/phables.egg-info/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6646 2023-02-22 00:21:03.000000 phables-0.2.0/phables.egg-info/PKG-INFO
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1944 2023-02-22 00:21:03.000000 phables-0.2.0/phables.egg-info/SOURCES.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2023-02-22 00:21:03.000000 phables-0.2.0/phables.egg-info/dependency_links.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       50 2023-02-22 00:21:03.000000 phables-0.2.0/phables.egg-info/entry_points.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       43 2023-02-22 00:21:03.000000 phables-0.2.0/phables.egg-info/requires.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        8 2023-02-22 00:21:03.000000 phables-0.2.0/phables.egg-info/top_level.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       38 2023-02-22 00:21:03.347291 phables-0.2.0/setup.cfg
--rw-rw-r--   0 vijinimallawaarachchi   (501) staff       (20)     1422 2023-02-16 03:08:21.000000 phables-0.2.0/setup.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.701600 phables-1.0.0/
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.518041 phables-1.0.0/.github/
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.531479 phables-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      650 2023-01-24 03:27:45.000000 phables-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      126 2023-01-10 00:17:29.000000 phables-1.0.0/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      612 2023-01-24 03:27:45.000000 phables-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.532752 phables-1.0.0/.github/workflows/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2948 2023-01-19 06:09:18.000000 phables-1.0.0/.github/workflows/codeql.yml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1747 2023-01-20 03:32:50.000000 phables-1.0.0/.github/workflows/testing.yml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1914 2023-04-21 05:14:19.000000 phables-1.0.0/.gitignore
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      439 2023-01-10 00:17:29.000000 phables-1.0.0/.readthedocs.yaml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     5265 2023-01-10 00:17:29.000000 phables-1.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     3497 2023-05-09 03:49:37.000000 phables-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1079 2023-02-19 03:25:45.000000 phables-1.0.0/LICENSE
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      125 2023-01-12 05:31:03.000000 phables-1.0.0/MANIFEST.in
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    11079 2023-05-09 03:51:30.701051 phables-1.0.0/PKG-INFO
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10428 2023-05-09 03:49:37.000000 phables-1.0.0/README.md
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.538587 phables-1.0.0/docs/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1020 2023-02-10 09:05:34.000000 phables-1.0.0/docs/assemble.md
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     3026 2023-01-16 00:51:18.000000 phables-1.0.0/docs/comparison.md
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     3788 2023-04-21 05:14:19.000000 phables-1.0.0/docs/faq.md
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     3808 2023-02-02 03:28:12.000000 phables-1.0.0/docs/graph_stats.md
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.579830 phables-1.0.0/docs/images/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)   523874 2023-01-10 00:17:29.000000 phables-1.0.0/docs/images/Phables_workflow.png
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)   133780 2023-01-10 00:17:29.000000 phables-1.0.0/docs/images/components.png
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    58437 2023-01-16 01:26:17.000000 phables-1.0.0/docs/images/histogram_n_nodes.png
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)   344700 2023-02-02 03:25:24.000000 phables-1.0.0/docs/images/pearson_clustermap.png
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)   318753 2023-02-02 03:25:23.000000 phables-1.0.0/docs/images/pearson_heatmap.png
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)   434479 2023-01-10 00:17:29.000000 phables-1.0.0/docs/images/phables_logo.png
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    98145 2023-01-10 00:17:29.000000 phables-1.0.0/docs/images/qual_resolved_genome_unitig_boxen.png
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)   174336 2023-01-10 00:17:29.000000 phables-1.0.0/docs/images/qual_resolved_genome_unitig_violin.png
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1708 2023-04-21 05:14:19.000000 phables-1.0.0/docs/index.md
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     4204 2023-05-09 03:49:37.000000 phables-1.0.0/docs/install.md
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1894 2023-01-10 00:17:29.000000 phables-1.0.0/docs/quality.md
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      301 2023-01-10 00:17:29.000000 phables-1.0.0/docs/requirements.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6246 2023-05-09 03:49:37.000000 phables-1.0.0/docs/usage.md
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      649 2023-04-21 05:16:05.000000 phables-1.0.0/mkdocs.yml
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.588159 phables-1.0.0/phables/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-02-02 03:00:11.000000 phables-1.0.0/phables/.DS_Store
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-01-12 05:31:03.000000 phables-1.0.0/phables/__init__.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     7248 2023-05-09 03:49:37.000000 phables-1.0.0/phables/__main__.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.593493 phables-1.0.0/phables/__pycache__/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      159 2023-02-18 10:21:30.000000 phables-1.0.0/phables/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     5807 2023-02-18 10:21:30.000000 phables-1.0.0/phables/__pycache__/__main__.cpython-310.pyc
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     4923 2023-02-18 10:21:30.000000 phables-1.0.0/phables/__pycache__/util.cpython-310.pyc
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.595610 phables-1.0.0/phables/config/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      438 2023-02-18 10:20:36.000000 phables-1.0.0/phables/config/config.yaml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      533 2023-01-12 05:31:03.000000 phables-1.0.0/phables/config/databases.yaml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      250 2023-05-09 03:49:37.000000 phables-1.0.0/phables/phables.CITATION
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1081 2023-01-12 05:31:03.000000 phables-1.0.0/phables/phables.LICENSE
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        5 2023-05-09 03:49:37.000000 phables-1.0.0/phables/phables.VERSION
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.601223 phables-1.0.0/phables/test_data/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    18772 2023-01-12 06:12:46.000000 phables-1.0.0/phables/test_data/assembly_graph.gfa
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      131 2023-01-12 06:12:46.000000 phables-1.0.0/phables/test_data/edge_coverages.tsv
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      587 2023-01-12 06:12:46.000000 phables-1.0.0/phables/test_data/edges.fasta.hmmout
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      122 2023-01-12 06:12:46.000000 phables-1.0.0/phables/test_data/junction_pe_coverage.pickle
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      272 2023-01-12 06:12:46.000000 phables-1.0.0/phables/test_data/phrogs_annotations.tsv
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     4928 2023-01-13 04:59:11.000000 phables-1.0.0/phables/util.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.603991 phables-1.0.0/phables/workflow/
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.608516 phables-1.0.0/phables/workflow/envs/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       59 2023-02-06 06:39:30.000000 phables-1.0.0/phables/workflow/envs/curl.yaml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       77 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/envs/mapping.yaml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       71 2023-01-12 05:31:03.000000 phables-1.0.0/phables/workflow/envs/mmseqs.yaml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      257 2023-01-12 05:31:03.000000 phables-1.0.0/phables/workflow/envs/phables.yaml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       74 2023-01-12 05:31:03.000000 phables-1.0.0/phables/workflow/envs/smg.yaml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1755 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/install.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1697 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/phables.smk
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.622068 phables-1.0.0/phables/workflow/rules/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      799 2023-02-06 06:39:30.000000 phables-1.0.0/phables/workflow/rules/00_database_preflight.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2161 2023-02-18 10:20:36.000000 phables-1.0.0/phables/workflow/rules/02_phables_preflight.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1189 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/rules/02_phables_targets.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      920 2023-02-16 05:28:06.000000 phables-1.0.0/phables/workflow/rules/03_test_preflight.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      592 2023-01-12 05:31:03.000000 phables-1.0.0/phables/workflow/rules/03_test_targets.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     3343 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/rules/coverage.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2280 2023-04-21 05:14:19.000000 phables-1.0.0/phables/workflow/rules/genes.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      569 2023-02-06 06:39:30.000000 phables-1.0.0/phables/workflow/rules/gfa2fasta.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      898 2023-04-21 05:14:19.000000 phables-1.0.0/phables/workflow/rules/mapping.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1172 2023-02-16 05:28:06.000000 phables-1.0.0/phables/workflow/rules/phables.smk
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.625098 phables-1.0.0/phables/workflow/scripts/
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     2618 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/scripts/combine_cov.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     3358 2023-02-19 03:24:59.000000 phables-1.0.0/phables/workflow/scripts/gfa2fasta.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    34730 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/scripts/phables.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.637049 phables-1.0.0/phables/workflow/scripts/phables_utils/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     8077 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/FD_Inexact.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-01-12 05:31:03.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/__init__.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2591 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/component_utils.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     3413 2023-02-16 05:28:07.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/coverage_utils.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6480 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/edge_graph_utils.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1760 2023-02-16 05:28:07.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/flow_utils.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2930 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/gene_utils.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1828 2023-04-21 05:14:19.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/genome_utils.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     5427 2023-04-21 06:05:21.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/output_utils.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.638106 phables-1.0.0/phables/workflow/scripts/phables_utils/phrogs/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)  3831481 2023-01-12 05:31:03.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/phrogs/phrog_annot.tsv
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2549 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/test_phables.smk
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.591350 phables-1.0.0/phables.egg-info/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    11079 2023-05-09 03:51:30.000000 phables-1.0.0/phables.egg-info/PKG-INFO
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2821 2023-05-09 03:51:30.000000 phables-1.0.0/phables.egg-info/SOURCES.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2023-05-09 03:51:30.000000 phables-1.0.0/phables.egg-info/dependency_links.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       50 2023-05-09 03:51:30.000000 phables-1.0.0/phables.egg-info/entry_points.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       43 2023-05-09 03:51:30.000000 phables-1.0.0/phables.egg-info/requires.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        8 2023-05-09 03:51:30.000000 phables-1.0.0/phables.egg-info/top_level.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)   434479 2023-01-10 00:17:29.000000 phables-1.0.0/phables_logo.png
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       38 2023-05-09 03:51:30.701782 phables-1.0.0/setup.cfg
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1427 2023-05-09 03:49:37.000000 phables-1.0.0/setup.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.697838 phables-1.0.0/tests/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1318 2023-02-19 03:24:59.000000 phables-1.0.0/tests/test_phables.py
```

### Comparing `phables-0.2.0/LICENSE` & `phables-1.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vijini Mallawaarachchi
+Copyright (c) 2023 Vijini Mallawaarachchi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `phables-0.2.0/phables/__main__.py` & `phables-1.0.0/phables/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 @click.group(
     cls=OrderedCommands, context_settings=dict(help_option_names=["-h", "--help"])
 )
 @click.version_option(get_version(), "-v", "--version", is_flag=True)
 def cli():
     """
-    Phables: Phage bubbles resolve bacteriophage genomes in viral metagenomic samples.
+    Phables: from fragmented assemblies to high-quality bacteriophage genomes.
     Please refer the full documentation available on Read the Docs at https://phables.readthedocs.io/
     """
     pass
 
 
 help_msg_extra = """
 \b
@@ -267,52 +267,14 @@
         # Full path to Snakefile
         snakefile_path=snake_base(os.path.join("workflow", "test_phables.smk")),
         merge_config=merge_config,
         **kwargs
     )
 
 
-# # Preprocess command
-# @click.command(
-#     epilog=help_msg_extra,
-#     context_settings=dict(
-#         help_option_names=["-h", "--help"], ignore_unknown_options=True
-#     ),
-# )
-# @click.option(
-#     "--input",
-#     help="Path to assembly graph file in .GFA format",
-#     type=click.Path(exists=True),
-#     required=True,
-# )
-# @click.option(
-#     "--reads", help="Path to directory containing paired-end reads", type=click.Path(exists=True), required=True
-# )
-# @common_options
-# def preprocess(input, reads, output, log, threads, **kwargs):
-#     """Preprocess data"""
-#     # Config to add or update in configfile
-#     merge_config = {
-#         "input": input,
-#         "reads": reads,
-#         "output": output,
-#         "log": log,
-#         "threads": threads
-#     }
-#
-#     # run!
-#     run_snakemake(
-#         # Full path to Snakefile
-#         snakefile_path=snake_base(os.path.join("workflow", "preprocess.smk")),
-#         merge_config=merge_config,
-#         log=log,
-#         **kwargs
-#     )
-
-
 @click.command()
 @common_options
 def config(configfile, **kwargs):
     """Copy the system default config file"""
     copy_config(configfile)
 
 
@@ -320,15 +282,14 @@
 def citation(**kwargs):
     """Print the citation(s) for this tool"""
     print_citation()
 
 
 cli.add_command(run)
 cli.add_command(install)
-# cli.add_command(preprocess)
 cli.add_command(test)
 cli.add_command(config)
 cli.add_command(citation)
 
 
 def main():
     cli()
```

### Comparing `phables-0.2.0/phables/config/databases.yaml` & `phables-1.0.0/phables/config/databases.yaml`

 * *Files identical despite different names*

### Comparing `phables-0.2.0/phables/phables.LICENSE` & `phables-1.0.0/phables/phables.LICENSE`

 * *Files identical despite different names*

### Comparing `phables-0.2.0/phables/test_data/assembly_graph.gfa` & `phables-1.0.0/phables/test_data/assembly_graph.gfa`

 * *Files identical despite different names*

### Comparing `phables-0.2.0/phables/test_data/edges.fasta.hmmout` & `phables-1.0.0/phables/test_data/edges.fasta.hmmout`

 * *Files identical despite different names*

### Comparing `phables-0.2.0/phables/util.py` & `phables-1.0.0/phables/util.py`

 * *Files identical despite different names*

### Comparing `phables-0.2.0/phables/workflow/install.smk` & `phables-1.0.0/phables/workflow/install.smk`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Phables: Phage bubbles resolve bacteriophage genomes in viral metagenomic samples.
+Phables: from fragmented assemblies to high-quality bacteriophage genomes.
 
 2023, Vijini Mallawaarachchi
 
 This is an auxiliary Snakefile to install databases or dependencies.
 """
```

### Comparing `phables-0.2.0/phables/workflow/phables.smk` & `phables-1.0.0/phables/workflow/phables.smk`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Phables: Phage bubbles resolve bacteriophage genomes in viral metagenomic samples.
+Phables: from fragmented assemblies to high-quality bacteriophage genomes.
 
 2023, Vijini Mallawaarachchi
 
 This is the main Snakefile to run phables.
 """
 
 """CONFIGURATION"""
@@ -24,15 +24,15 @@
 target_rules = []
 
 def targetRule(fn):
     assert fn.__name__.startswith("__")
     target_rules.append(fn.__name__[2:])
     return fn
 
-localrules: all, preprocess, phables, print_stages
+localrules: all, preprocess, phables, print_stages, rpkm_coverage
 
 
 """Run stages"""
 @targetRule
 rule all:
     input:
         preprocessTargets,
@@ -63,16 +63,16 @@
 include: os.path.join("rules", "gfa2fasta.smk")
 
 
 # Step 3: Map reads to unitig sequences and get BAM files
 include: os.path.join("rules", "mapping.smk")
 
 
-# Step 4: Run CoverM to get coverage of unitig sequences
-include: os.path.join("rules", "coverm.smk")
+# Step 4: Calculate coverage of unitig sequences
+include: os.path.join("rules", "coverage.smk")
 
 
 # Step 5: Scan unitig sequences for single-copy marker genes and PHROGs
 include: os.path.join("rules", "genes.smk")
 
 
 # Step 6: Run Phables
```

### Comparing `phables-0.2.0/phables/workflow/rules/00_database_preflight.smk` & `phables-1.0.0/phables/workflow/rules/00_database_preflight.smk`

 * *Files identical despite different names*

### Comparing `phables-0.2.0/phables/workflow/rules/02_phables_preflight.smk` & `phables-1.0.0/phables/workflow/rules/02_phables_preflight.smk`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 
 """
 Setting the directory variables
 """
 
-THREADS = config['threads']
+# THREADS = config['threads']
 INPUT = config['input']
 OUTDIR = config['output']
 print(f"Output files will be saved to directory, {OUTDIR}\n")
 
 
 ############################################################################
 # Checking through the reads folder
```

### Comparing `phables-0.2.0/phables/workflow/rules/02_phables_targets.smk` & `phables-1.0.0/phables/workflow/rules/02_phables_targets.smk`

 * *Files 11% similar despite different names*

```diff
@@ -7,28 +7,26 @@
 EDGES_FILE = os.path.join(OUTDIR, "edges.fasta")
 preprocessTargets.append(EDGES_FILE)
 
 BAM_PATH = os.path.join(OUTDIR, 'bam_files/')
 preprocessTargets.append(expand(os.path.join(BAM_PATH, "{sample}.bam"), sample=SAMPLES))
 preprocessTargets.append(expand(os.path.join(BAM_PATH, "{sample}.bam.bai"), sample=SAMPLES))
 
-COVERM_PATH = os.path.join(OUTDIR, 'coverage_rpkm/')
-preprocessTargets.append(expand(os.path.join(COVERM_PATH, "{sample}_rpkm.tsv"), sample=SAMPLES))
+COVERAGE_PATH = os.path.join(OUTDIR, 'coverage_rpkm/')
+preprocessTargets.append(expand(os.path.join(COVERAGE_PATH, "{sample}_rpkm.tsv"), sample=SAMPLES))
 preprocessTargets.append(os.path.join(OUTDIR, "coverage.tsv"))
 preprocessTargets.append(os.path.join(OUTDIR, "edges.fasta.hmmout"))
 
 preprocessTargets.append(os.path.join(OUTDIR, "phrogs_annotations.tsv"))
 
 
 """MISC"""
 COVERAGE_FILE = os.path.join(OUTDIR, 'coverage.tsv')
 PHROG_ANNOT = os.path.join(OUTDIR, 'phrogs_annotations.tsv')
 SMG_FILE = os.path.join(OUTDIR, 'edges.fasta.hmmout')
 GRAPH_FILE = INPUT
 
 
 """PHABLES TARGETS"""
-phablesTargets.append(os.path.join(OUTDIR, "resolved_paths.fasta"))
 phablesTargets.append(os.path.join(OUTDIR, "resolved_genome_info.txt"))
-phablesTargets.append(os.path.join(OUTDIR, "resolved_edges.fasta"))
 phablesTargets.append(os.path.join(OUTDIR, "resolved_component_info.txt"))
 phablesTargets.append(os.path.join(OUTDIR, "component_phrogs.txt"))
```

### Comparing `phables-0.2.0/phables/workflow/rules/03_test_preflight.smk` & `phables-1.0.0/phables/workflow/rules/03_test_preflight.smk`

 * *Files identical despite different names*

### Comparing `phables-0.2.0/phables/workflow/rules/03_test_targets.smk` & `phables-1.0.0/phables/workflow/rules/03_test_targets.smk`

 * *Files identical despite different names*

### Comparing `phables-0.2.0/phables/workflow/rules/gfa2fasta.smk` & `phables-1.0.0/phables/workflow/rules/gfa2fasta.smk`

 * *Files identical despite different names*

### Comparing `phables-0.2.0/phables/workflow/rules/phables.smk` & `phables-1.0.0/phables/workflow/rules/phables.smk`

 * *Files identical despite different names*

### Comparing `phables-0.2.0/phables/workflow/scripts/combine_cov.py` & `phables-1.0.0/phables/workflow/scripts/combine_cov.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/python3
 
-"""combine_cov.py: Combine multiple coverage files of samples from CoverM.
+"""combine_cov.py: Combine multiple coverage files of samples.
 
 """
 
 import glob
 import logging
 import os
 import subprocess
 
 import pandas as pd
 
 __author__ = "Vijini Mallawaarachchi"
-__copyright__ = "Copyright 2022, Phables Project"
+__copyright__ = "Copyright 2023, Phables Project"
 __license__ = "MIT"
 __type__ = "Support Script"
 __maintainer__ = "Vijini Mallawaarachchi"
 __email__ = "viji.mallawaarachchi@gmail.com"
 
 
 def main():
```

### Comparing `phables-0.2.0/phables/workflow/scripts/gfa2fasta.py` & `phables-1.0.0/phables/workflow/scripts/gfa2fasta.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import sys
 
 from Bio import SeqIO
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
 
 __author__ = "Vijini Mallawaarachchi"
-__copyright__ = "Copyright 2022, Phables Project"
+__copyright__ = "Copyright 2023, Phables Project"
 __license__ = "MIT"
 __type__ = "Support Script"
 __maintainer__ = "Vijini Mallawaarachchi"
 __email__ = "viji.mallawaarachchi@gmail.com"
 
 
 def main():
```

### Comparing `phables-0.2.0/phables/workflow/scripts/phables.py` & `phables-1.0.0/phables/workflow/scripts/phables.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,34 +2,37 @@
 
 import logging
 import sys
 import time
 
 import networkx as nx
 from igraph import *
-from phables_utils import (component_utils, edge_graph_utils, flow_utils,
-                           gene_utils)
-from phables_utils.coverage_utils import (get_junction_pe_coverage,
-                                          get_unitig_coverage)
+from phables_utils import component_utils, edge_graph_utils, flow_utils, gene_utils
+from phables_utils.coverage_utils import get_junction_pe_coverage, get_unitig_coverage
 from phables_utils.genome_utils import GenomeComponent, GenomePath
-from phables_utils.output_utils import (write_component_info,
-                                        write_component_phrog_info, write_path,
-                                        write_path_fasta,
-                                        write_res_genome_info, write_unitigs)
+from phables_utils.output_utils import (
+    write_component_info,
+    write_component_phrog_info,
+    write_path,
+    write_path_fasta,
+    write_res_genome_info,
+    write_unitigs,
+)
 from tqdm import tqdm
 
 __author__ = "Vijini Mallawaarachchi"
 __copyright__ = "Copyright 2022, Phables Project"
 __license__ = "MIT"
-__version__ = "0.2.0"
+__version__ = "1.0.0"
 __maintainer__ = "Vijini Mallawaarachchi"
 __email__ = "viji.mallawaarachchi@gmail.com"
 __status__ = "Development"
 
 MAX_VAL = sys.maxsize
+LEN_THRESHOLD = 0.95
 
 # Phables main code
 # ----------------------------------------------------------------------
 
 
 def main():
     # Get arguments
@@ -67,15 +70,15 @@
     else:
         fileHandler = logging.FileHandler(f"{log}")
     fileHandler.setLevel(logging.DEBUG)
     fileHandler.setFormatter(formatter)
     logger.addHandler(fileHandler)
 
     logger.info(
-        "Welcome to Phables: Phage bubbles resolve bacteriophage genomes in viral metagenomic samples."
+        "Welcome to Phables: from fragmented assemblies to high-quality bacteriophage genomes."
     )
 
     logger.info(f"Input arguments: ")
     logger.info(f"Assembly graph file: {graph}")
     logger.info(f"Unitig coverage file: {coverage}")
     logger.info(f"BAM files path: {bampath}")
     logger.info(f"Unitig .hmmout file: {hmmout}")
@@ -162,36 +165,39 @@
     case1_resolved = set()
     case2_found = set()
     case2_resolved = set()
     case3_found = set()
     case3_resolved = set()
 
     phage_like_edges = set()
+    all_phage_like_edges = set()
 
     for my_count in tqdm(pruned_vs, desc="Resolving components"):
         component_time_start = time.time()
 
         my_genomic_paths = []
 
         original_candidate_nodes = pruned_vs[my_count]
 
         candidate_nodes = pruned_vs[my_count]
 
         pruned_graph = assembly_graph.subgraph(candidate_nodes)
 
         has_cycles = False
 
-        # if 5627 not in candidate_nodes:
+        # if 423 not in candidate_nodes:
         #     continue
 
         logger.debug(f"my_count: {my_count}")
 
         logger.debug(f"number of unitigs: {len(candidate_nodes)}")
         logger.debug(f"{candidate_nodes}")
 
+        all_phage_like_edges = all_phage_like_edges.union(set(candidate_nodes))
+
         in_degree = []
         out_degree = []
 
         # Case 2 components
         if len(candidate_nodes) == 2:
             all_self_looped = True
 
@@ -238,27 +244,34 @@
                     elif unitig2_len > unitig1_len and unitig2_len > minlength:
                         unitig_to_consider = unitig2
                         unitig_name = unitig2_name
                         repeat_unitig = unitig1
                         repeat_unitig_name = unitig1_name
 
                     if unitig_to_consider != -1:
+                        logger.debug(
+                            f"Case 2 bubble: {unitig1_name} is {unitig1_len} bp long and {unitig2_name} is {unitig2_len} bp long."
+                        )
                         cycle_number = 1
                         resolved_edges.add(unitig_to_consider)
                         resolved_edges.add(repeat_unitig)
                         path_string = (
                             str(graph_unitigs[repeat_unitig_name])
                             + str(graph_unitigs[unitig_name])
                             + str(
                                 graph_unitigs[repeat_unitig_name].reverse_complement()
                             )
                         )
+                        logger.debug(
+                            f"Terminal repeat detected is {repeat_unitig_name}"
+                        )
 
                         genome_path = GenomePath(
                             f"phage_comp_{my_count}_cycle_{cycle_number}",
+                            "case2",
                             [
                                 f"{repeat_unitig_name}+",
                                 f"{unitig_name}+",
                                 f"{repeat_unitig_name}-",
                             ],
                             [repeat_unitig, unitig_to_consider, repeat_unitig],
                             path_string,
@@ -320,14 +333,15 @@
 
             logger.debug(f"clean_node_count: {clean_node_count}")
 
             for cedge in cycle_edges:
                 G_edge.add_edge(cedge[0], cedge[1], weight=cycle_edges[cedge])
 
             two_comp = sorted(nx.weakly_connected_components(G_edge), key=len)
+            logger.debug(f"No. of weakly connected components: {len(two_comp)}")
 
             if len(two_comp) >= 2:
                 G_edge.remove_nodes_from(list(two_comp[0]))
 
             try:
                 cycles_found = nx.find_cycle(G_edge, orientation="original")
                 if len(cycles_found) > 0:
@@ -367,23 +381,25 @@
                 logger.debug(
                     f"Identified candidate source_sinks from BFS: {source_sink_candidates}"
                 )
 
                 if len(source_sink_candidates) > 0:
                     # Identify the longest source/sink vertex
                     max_length = -1
-                    max_length_vertex = -1
+                    max_length_st_vertex = -1
 
                     for vertex in source_sink_candidates:
                         if len(graph_unitigs[vertex[:-1]]) > max_length:
                             max_length = len(graph_unitigs[vertex[:-1]])
-                            max_length_vertex = vertex
+                            max_length_st_vertex = vertex
 
-                    source_sink = unitig_names_rev[max_length_vertex[:-1]]
-                    logger.debug(f"Identified source_sink from BFS: {source_sink}")
+                    source_sink = unitig_names_rev[max_length_st_vertex[:-1]]
+                    logger.debug(
+                        f"Identified source_sink from BFS: {source_sink}, {max_length_st_vertex}"
+                    )
 
                     candidate_nodes.remove(source_sink)
                     candidate_nodes.insert(0, source_sink)
                     logger.debug(f"Ordered candidate_nodes: {candidate_nodes}")
 
                 else:
                     logger.debug(f"No source/sink node detected")
@@ -399,14 +415,16 @@
                         node_indices_rev[my_counter] = u
                         my_counter += 1
                     if v not in node_indices:
                         node_indices[v] = my_counter
                         node_indices_rev[my_counter] = v
                         my_counter += 1
 
+                    logger.debug(f"Edge: {u}, {v}, {cov['weight']}")
+
                     G.add_edge(node_indices[u], node_indices[v], weight=cov["weight"])
 
                 # Get connections and degree information
                 # ----------------------------------------------------------------------
                 in_degree = []
                 out_degree = []
 
@@ -445,18 +463,24 @@
                 edge_list_indices = {}
 
                 subpaths = {}
                 subpath_count = 0
 
                 visited_edges = []
 
+                logger.debug(f"G_edge.nodes: {list(G_edge.nodes)}")
+                logger.debug(f"G_edge.edges: {G_edge.edges(data=True)}")
+
                 for u, v, cov in G_edge.edges(data=True):
                     u_name = unitig_names_rev[u[:-1]]
                     v_name = unitig_names_rev[v[:-1]]
 
+                    original_edge = (u[:-1], v[:-1])
+                    rev_original_edge = (v[:-1], u[:-1])
+
                     u_index = candidate_nodes.index(u_name)
                     v_index = candidate_nodes.index(v_name)
 
                     edge_list_indices[u_index] = u
                     edge_list_indices[v_index] = v
 
                     juction_cov = junction_pe_coverage[(u[:-1], v[:-1])]
@@ -591,14 +615,15 @@
                                         total_length += len(
                                             str(graph_unitigs[unitig_name])
                                         )
 
                                     # Create GenomePath object with path details
                                     genome_path = GenomePath(
                                         f"phage_comp_{my_count}_cycle_{cycle_number}",
+                                        "case3",
                                         [x for x in path_order],
                                         [unitig_names_rev[x[:-1]] for x in path_order],
                                         path_string,
                                         int(coverage_val),
                                         total_length,
                                         (
                                             path_string.count("G")
@@ -637,14 +662,15 @@
             path_string = str(graph_unitigs[unitig_name])
 
             cycle_number = 1
 
             # Create GenomePath object with path details
             genome_path = GenomePath(
                 f"phage_comp_{my_count}_cycle_{cycle_number}",
+                "case1",
                 [unitig_names[candidate_nodes[0]]],
                 [candidate_nodes[0]],
                 path_string,
                 int(unitig_coverages[unitig_name]),
                 len(graph_unitigs[unitig_name]),
                 (path_string.count("G") + path_string.count("C"))
                 / len(path_string)
@@ -662,14 +688,15 @@
 
         # Order resolved paths in descending order of length
         my_genomic_paths.sort(key=lambda x: (x.length, x.coverage), reverse=True)
 
         final_genomic_paths = []
         comp_resolved_edges = set()
         visited_nodes = set()
+        comp_resolved_paths = set()
 
         frac_unitigs = 1
         n_paths = 0
 
         if len(my_genomic_paths) > 1:
             # Get the degree of the component
             graph_degree = assembly_graph.degree(original_candidate_nodes)
@@ -677,23 +704,34 @@
             path_lengths = []
             path_coverages = []
 
             largest_length = my_genomic_paths[0].length
 
             # Filter genomic paths
             for genomic_path in my_genomic_paths:
-                if genomic_path.length > largest_length * 0.95:
+                passed = False
+
+                if genomic_path.length > largest_length * LEN_THRESHOLD:
+                    passed = True
+
+                path_node_order_string = ",".join(genomic_path.node_order)
+
+                if path_node_order_string in comp_resolved_paths:
+                    passed = False
+
+                if passed:
                     logger.debug(
                         f"{genomic_path.id}\t{genomic_path.length}\t{genomic_path.coverage}"
                     )
                     logger.debug(f"{genomic_path.node_order}")
                     path_lengths.append(genomic_path.length)
                     path_coverages.append(genomic_path.coverage)
                     final_genomic_paths.append(genomic_path)
                     visited_nodes = visited_nodes.union(set(genomic_path.node_order))
+                    comp_resolved_paths.add(path_node_order_string)
                     n_paths += 1
 
                     for path_node in genomic_path.node_id_order:
                         comp_resolved_edges.add(path_node)
 
             frac_unitigs = len(visited_nodes) / len(original_candidate_nodes)
 
@@ -766,40 +804,56 @@
     logger.info(
         f"Total number of components resolved: {len(circular_unitigs)+len(resolved_cyclic)}"
     )
     logger.info(f"Case 1 (resolved/found): {len(case1_resolved)}/{len(case1_found)}")
     logger.info(f"Case 2 (resolved/found): {len(case2_resolved)}/{len(case2_found)}")
     logger.info(f"Case 3 (resolved/found): {len(case3_resolved)}/{len(case3_found)}")
     logger.info(f"Total number of genomes resolved: {len(all_resolved_paths)}")
-    logger.info(f"Resolved genomes can be found in {output}/resolved_paths.fasta")
+
+    if len(all_resolved_paths) == 0:
+        logger.info(f"No genomes were resolved.")
+    else:
+        logger.info(f"Resolved genomes can be found in {output}/resolved_paths.fasta")
 
     # Write edges to file
     # ----------------------------------------------------------------------
 
     write_unitigs(
         phage_like_edges, unitig_names, graph_unitigs, "phage_like_edges", output
     )
+    write_unitigs(
+        all_phage_like_edges,
+        unitig_names,
+        graph_unitigs,
+        "all_phage_like_edges",
+        output,
+    )
     write_unitigs(resolved_edges, unitig_names, graph_unitigs, "resolved_edges", output)
 
     # Record path information
     # ----------------------------------------------------------------------
 
     filename = write_res_genome_info(all_resolved_paths, output)
-    logger.info(f"Resolved genome information can be found in {output}/{filename}")
+    if len(all_resolved_paths) > 0:
+        logger.info(f"Resolved genome information can be found in {output}/{filename}")
 
     # Record component information
     # ----------------------------------------------------------------------
 
     filename = write_component_info(all_components, output)
-    logger.info(f"Resolved component information can be found in {output}/{filename}")
+    if len(all_components) > 0:
+        logger.info(
+            f"Resolved component information can be found in {output}/{filename}"
+        )
 
     filename = write_component_phrog_info(resolved_components, comp_phrogs, output)
-    logger.info(
-        f"PHROGs found in resolved components can be found in {output}/{filename}"
-    )
+    if len(resolved_components) > 0:
+        logger.info(
+            f"PHROGs found in resolved components can be found in {output}/{filename}"
+        )
 
     # Get elapsed time
     # ----------------------------------------------------------------------
 
     # Determine elapsed time
     elapsed_time = time.time() - start_time
```

### Comparing `phables-0.2.0/phables/workflow/scripts/phables_utils/FD_Inexact.py` & `phables-1.0.0/phables/workflow/scripts/phables_utils/FD_Inexact.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 
 import more_itertools
 import networkx as nx
 
 # create logger
-logger = logging.getLogger("phables 0.2.0")
+logger = logging.getLogger("phables 1.0.0")
 
 
 def read_input(graphfile, number_subpath):
     trip_data = open(graphfile, "r").read().split("\n")
     i = 0
     listOfGraphs = {}
     k = 0
```

### Comparing `phables-0.2.0/phables/workflow/scripts/phables_utils/component_utils.py` & `phables-1.0.0/phables/workflow/scripts/phables_utils/component_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,18 @@
     """
 
     pruned_vs = {}
 
     i = 0
 
     comp_phrogs = {}
-    phrogs_found = set()
 
     for component in assembly_graph.components():
+        phrogs_found = set()
+
         head_present = False
         connector_present = False
         tail_present = False
         lysis_present = False
 
         if len(component) > 1:
             for unitig in component:
```

### Comparing `phables-0.2.0/phables/workflow/scripts/phables_utils/coverage_utils.py` & `phables-1.0.0/phables/workflow/scripts/phables_utils/coverage_utils.py`

 * *Files identical despite different names*

### Comparing `phables-0.2.0/phables/workflow/scripts/phables_utils/edge_graph_utils.py` & `phables-1.0.0/phables/workflow/scripts/phables_utils/edge_graph_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections import defaultdict
 
 from Bio import SeqIO
 from Bio.Seq import Seq
 from igraph import *
 
 # Create logger
-logger = logging.getLogger("phables 0.2.0")
+logger = logging.getLogger("phables 1.0.0")
 
 
 class BidirectionalError(Exception):
     """Must set a unique value in a BijectiveMap."""
 
     def __init__(self, value):
         self.value = value
```

### Comparing `phables-0.2.0/phables/workflow/scripts/phables_utils/flow_utils.py` & `phables-1.0.0/phables/workflow/scripts/phables_utils/flow_utils.py`

 * *Files identical despite different names*

### Comparing `phables-0.2.0/phables/workflow/scripts/phables_utils/gene_utils.py` & `phables-1.0.0/phables/workflow/scripts/phables_utils/gene_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     smg_unitigs = set()
 
     unitig_smgs = {}
 
     with open(hmmout, "r") as myfile:
         for line in myfile.readlines():
-            if not line.startswith("#") and line.startswith("edge_"):
+            if not line.startswith("#"):
                 strings = line.strip().split()
 
                 unitig = strings[0]
 
                 # Marker gene name
                 marker_gene = strings[3]
```

### Comparing `phables-0.2.0/phables/workflow/scripts/phables_utils/genome_utils.py` & `phables-1.0.0/phables/workflow/scripts/phables_utils/genome_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Class for genome path
 class GenomePath:
-    def __init__(self, id, node_order, node_id_order, path, coverage, length, gc):
+    def __init__(
+        self, id, bubble_case, node_order, node_id_order, path, coverage, length, gc
+    ):
         self.id = id
+        self.bubble_case = bubble_case
         self.path = path
         self.coverage = coverage
         self.length = length
         self.node_order = node_order
         self.node_id_order = node_id_order
         self.gc = gc
```

### Comparing `phables-0.2.0/phables/workflow/scripts/phables_utils/output_utils.py` & `phables-1.0.0/phables/workflow/scripts/phables_utils/output_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,18 +83,18 @@
 
 def write_res_genome_info(all_resolved_paths, output):
     """
     Write resolved genome information to file
     """
 
     with open(f"{output}/resolved_genome_info.txt", "w") as myfile:
-        myfile.write(f"Path\tCoverage\tLength\tGC content\tNode order\n")
+        myfile.write(f"Path\tCase\tCoverage\tLength\tGC content\tNode order\n")
         for genomic_path in all_resolved_paths:
             myfile.write(
-                f"{genomic_path.id}\t{genomic_path.coverage}\t{genomic_path.length}\t{genomic_path.gc}\t{genomic_path.node_order}\n"
+                f"{genomic_path.id}\t{genomic_path.bubble_case}\t{genomic_path.coverage}\t{genomic_path.length}\t{genomic_path.gc}\t{genomic_path.node_order}\n"
             )
 
     return "resolved_genome_info.txt"
 
 
 def write_path(final_genomic_paths, output):
     """
@@ -137,11 +137,12 @@
 
 def write_component_phrog_info(resolved_components, comp_phrogs, output):
     """
     Write PHROGs found in resolved components
     """
 
     with open(f"{output}/component_phrogs.txt", "w") as myfile:
+        myfile.write(f"Phage component\tPHROG\n")
         for comp in resolved_components:
             myfile.write(f"phage_{comp}\t{comp_phrogs[comp]}\n")
 
     return "component_phrogs.txt"
```

### Comparing `phables-0.2.0/phables/workflow/scripts/phables_utils/phrogs/phrog_annot.tsv` & `phables-1.0.0/phables/workflow/scripts/phables_utils/phrogs/phrog_annot.tsv`

 * *Files identical despite different names*

### Comparing `phables-0.2.0/phables/workflow/test_phables.smk` & `phables-1.0.0/phables/workflow/test_phables.smk`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Phables: Phage bubbles resolve bacteriophage genomes in viral metagenomic samples.
+Phables: from fragmented assemblies to high-quality bacteriophage genomes.
 
 2023, Vijini Mallawaarachchi
 
 This is an auxiliary Snakefile to test phables.
 """
 
 """CONFIGURATION"""
```

### Comparing `phables-0.2.0/phables.egg-info/SOURCES.txt` & `phables-1.0.0/phables.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,55 @@
+.gitignore
+.readthedocs.yaml
+CODE_OF_CONDUCT.md
+CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
+mkdocs.yml
+phables_logo.png
 setup.py
+.github/ISSUE_TEMPLATE/bug_report.md
+.github/ISSUE_TEMPLATE/custom.md
+.github/ISSUE_TEMPLATE/feature_request.md
+.github/workflows/codeql.yml
+.github/workflows/testing.yml
+docs/assemble.md
+docs/comparison.md
+docs/faq.md
+docs/graph_stats.md
+docs/index.md
+docs/install.md
+docs/quality.md
+docs/requirements.txt
+docs/usage.md
+docs/images/Phables_workflow.png
+docs/images/components.png
+docs/images/histogram_n_nodes.png
+docs/images/pearson_clustermap.png
+docs/images/pearson_heatmap.png
+docs/images/phables_logo.png
+docs/images/qual_resolved_genome_unitig_boxen.png
+docs/images/qual_resolved_genome_unitig_violin.png
+phables/.DS_Store
 phables/__init__.py
 phables/__main__.py
 phables/phables.CITATION
 phables/phables.LICENSE
 phables/phables.VERSION
 phables/util.py
 phables.egg-info/PKG-INFO
 phables.egg-info/SOURCES.txt
 phables.egg-info/dependency_links.txt
 phables.egg-info/entry_points.txt
 phables.egg-info/requires.txt
 phables.egg-info/top_level.txt
+phables/__pycache__/__init__.cpython-310.pyc
+phables/__pycache__/__main__.cpython-310.pyc
+phables/__pycache__/util.cpython-310.pyc
 phables/config/config.yaml
 phables/config/databases.yaml
 phables/test_data/assembly_graph.gfa
 phables/test_data/edge_coverages.tsv
 phables/test_data/edges.fasta.hmmout
 phables/test_data/junction_pe_coverage.pickle
 phables/test_data/phrogs_annotations.tsv
@@ -30,15 +62,15 @@
 phables/workflow/envs/phables.yaml
 phables/workflow/envs/smg.yaml
 phables/workflow/rules/00_database_preflight.smk
 phables/workflow/rules/02_phables_preflight.smk
 phables/workflow/rules/02_phables_targets.smk
 phables/workflow/rules/03_test_preflight.smk
 phables/workflow/rules/03_test_targets.smk
-phables/workflow/rules/coverm.smk
+phables/workflow/rules/coverage.smk
 phables/workflow/rules/genes.smk
 phables/workflow/rules/gfa2fasta.smk
 phables/workflow/rules/mapping.smk
 phables/workflow/rules/phables.smk
 phables/workflow/scripts/combine_cov.py
 phables/workflow/scripts/gfa2fasta.py
 phables/workflow/scripts/phables.py
@@ -47,8 +79,9 @@
 phables/workflow/scripts/phables_utils/component_utils.py
 phables/workflow/scripts/phables_utils/coverage_utils.py
 phables/workflow/scripts/phables_utils/edge_graph_utils.py
 phables/workflow/scripts/phables_utils/flow_utils.py
 phables/workflow/scripts/phables_utils/gene_utils.py
 phables/workflow/scripts/phables_utils/genome_utils.py
 phables/workflow/scripts/phables_utils/output_utils.py
-phables/workflow/scripts/phables_utils/phrogs/phrog_annot.tsv
+phables/workflow/scripts/phables_utils/phrogs/phrog_annot.tsv
+tests/test_phables.py
```

### Comparing `phables-0.2.0/setup.py` & `phables-1.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 data_files = [(".", ["LICENSE", "README.md"])]
 
 setup(
     name="phables",
     packages=find_packages(),
     url="https://github.com/Vini2/phables",
     python_requires=">=3.8,<3.11",
-    description="Phables: Phage bubbles resolve bacteriophage genomes in viral metagenomic samples",
+    description="Phables: from fragmented assemblies to high-quality bacteriophage genomes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     version=get_version(),
     author="Vijini Mallawaarachchi",
     author_email="viji.mallawaarachchi@gmail.com",
     data_files=data_files,
     py_modules=["phables"],
@@ -37,15 +37,15 @@
         "snakemake>=7.14.0",
         "pyyaml>=6.0",
         "click>=8.1.3",
     ],
     entry_points={"console_scripts": ["phables=phables.__main__:main"]},
     include_package_data=True,
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Operating System :: OS Independent",
     ],
 )
```

