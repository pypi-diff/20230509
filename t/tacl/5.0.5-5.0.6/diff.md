# Comparing `tmp/tacl-5.0.5.tar.gz` & `tmp/tacl-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tacl-5.0.5.tar", last modified: Sat Sep 24 07:42:09 2022, max compression
+gzip compressed data, was "tacl-5.0.6.tar", last modified: Tue May  9 21:30:59 2023, max compression
```

## Comparing `tacl-5.0.5.tar` & `tacl-5.0.6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2022-09-24 07:42:09.584192 tacl-5.0.5/
--rw-r--r--   0 jamie     (1000) jamie     (1000)    12447 2022-09-24 02:16:09.000000 tacl-5.0.5/CHANGES
--rw-r--r--   0 jamie     (1000) jamie     (1000)    32472 2021-07-14 09:03:57.000000 tacl-5.0.5/LICENCE
--rw-r--r--   0 jamie     (1000) jamie     (1000)       51 2021-07-14 09:04:58.000000 tacl-5.0.5/MANIFEST.in
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1843 2022-09-24 07:42:09.584192 tacl-5.0.5/PKG-INFO
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1267 2021-07-14 09:01:38.000000 tacl-5.0.5/README.rst
--rw-r--r--   0 jamie     (1000) jamie     (1000)       95 2022-09-17 00:34:49.000000 tacl-5.0.5/pyproject.toml
--rw-r--r--   0 jamie     (1000) jamie     (1000)      911 2022-09-24 07:42:09.584192 tacl-5.0.5/setup.cfg
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2022-09-24 07:42:09.580192 tacl-5.0.5/tacl/
--rw-r--r--   0 jamie     (1000) jamie     (1000)      705 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    32400 2022-09-23 22:30:27.000000 tacl-5.0.5/tacl/__main__.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2022-09-24 07:42:09.580192 tacl-5.0.5/tacl/assets/
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2022-09-24 07:42:09.580192 tacl-5.0.5/tacl/assets/results_highlight/
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1229 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/assets/results_highlight/heatmap.js
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2022-09-24 07:42:09.584192 tacl-5.0.5/tacl/assets/templates/
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1801 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/assets/templates/lifetime.html
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1186 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/assets/templates/ngram_highlight.html
--rw-r--r--   0 jamie     (1000) jamie     (1000)      954 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/assets/templates/results_highlight.html
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1103 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/assets/templates/sequence.html
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2022-09-24 07:42:09.584192 tacl-5.0.5/tacl/assets/xslt/
--rw-r--r--   0 jamie     (1000) jamie     (1000)      807 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/assets/xslt/CBETA_T0062_rest.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)      891 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/assets/xslt/CBETA_T0220_reparent_divs.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1284 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/assets/xslt/CBETA_T0418_fix_verse.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2115 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/assets/xslt/CBETA_extract_commentary.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1165 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/assets/xslt/CBETA_extract_div.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1801 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/assets/xslt/CBETA_extract_verse.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)      748 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/assets/xslt/CBETA_remove_divs.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)     4563 2022-07-25 04:12:22.000000 tacl-5.0.5/tacl/assets/xslt/prepare_tei_cbeta_github.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2710 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/assets/xslt/strip_tei.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)     4330 2021-10-08 21:27:56.000000 tacl-5.0.5/tacl/catalogue.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2022-09-24 07:42:09.584192 tacl-5.0.5/tacl/cli/
--rw-r--r--   0 jamie     (1000) jamie     (1000)        0 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/cli/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3449 2021-09-27 01:52:24.000000 tacl-5.0.5/tacl/cli/formatters.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3808 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/cli/utils.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1579 2021-07-14 09:03:55.000000 tacl-5.0.5/tacl/colour.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    40010 2022-09-23 22:28:20.000000 tacl-5.0.5/tacl/constants.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     4253 2022-09-23 04:53:43.000000 tacl-5.0.5/tacl/corpus.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    36087 2022-09-19 01:51:28.000000 tacl-5.0.5/tacl/data_store.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1044 2021-07-14 09:03:55.000000 tacl-5.0.5/tacl/decorators.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      610 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/exceptions.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     7990 2021-07-14 09:03:55.000000 tacl-5.0.5/tacl/highlighter.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    19580 2021-07-14 09:03:57.000000 tacl-5.0.5/tacl/jitc.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     6635 2021-07-14 09:03:55.000000 tacl-5.0.5/tacl/lifetime_report.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    10364 2022-09-23 03:38:57.000000 tacl-5.0.5/tacl/normaliser.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3064 2022-05-05 07:43:28.000000 tacl-5.0.5/tacl/report.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    44873 2022-09-20 05:59:36.000000 tacl-5.0.5/tacl/results.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    13355 2021-09-27 01:52:15.000000 tacl-5.0.5/tacl/sequence.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     5494 2021-09-12 03:15:37.000000 tacl-5.0.5/tacl/splitter.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     5400 2021-07-14 09:03:56.000000 tacl-5.0.5/tacl/statistics_report.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3711 2021-07-14 09:03:55.000000 tacl-5.0.5/tacl/stripper.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    29157 2022-08-03 23:23:09.000000 tacl-5.0.5/tacl/tei_corpus.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     6013 2022-09-20 05:54:17.000000 tacl-5.0.5/tacl/text.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1140 2021-07-14 09:03:55.000000 tacl-5.0.5/tacl/tokenizer.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1248 2021-07-14 09:03:55.000000 tacl-5.0.5/tacl/work_joiner.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2022-09-24 07:42:09.580192 tacl-5.0.5/tacl.egg-info/
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1843 2022-09-24 07:42:09.000000 tacl-5.0.5/tacl.egg-info/PKG-INFO
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1277 2022-09-24 07:42:09.000000 tacl-5.0.5/tacl.egg-info/SOURCES.txt
--rw-r--r--   0 jamie     (1000) jamie     (1000)        1 2022-09-24 07:42:09.000000 tacl-5.0.5/tacl.egg-info/dependency_links.txt
--rw-r--r--   0 jamie     (1000) jamie     (1000)       44 2022-09-24 07:42:09.000000 tacl-5.0.5/tacl.egg-info/entry_points.txt
--rw-r--r--   0 jamie     (1000) jamie     (1000)       45 2022-09-24 07:42:09.000000 tacl-5.0.5/tacl.egg-info/requires.txt
--rw-r--r--   0 jamie     (1000) jamie     (1000)        5 2022-09-24 07:42:09.000000 tacl-5.0.5/tacl.egg-info/top_level.txt
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-05-09 21:30:59.338202 tacl-5.0.6/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    12631 2023-05-09 20:58:08.000000 tacl-5.0.6/CHANGES
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    32472 2021-07-14 09:03:57.000000 tacl-5.0.6/LICENCE
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      162 2022-12-26 23:02:02.000000 tacl-5.0.6/MANIFEST.in
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    39343 2023-05-09 21:30:59.338202 tacl-5.0.6/PKG-INFO
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1267 2021-07-14 09:01:38.000000 tacl-5.0.6/README.rst
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      879 2023-05-09 21:22:44.000000 tacl-5.0.6/pyproject.toml
+-rw-r--r--   0 jamie     (1000) jamie     (1000)       38 2023-05-09 21:30:59.338202 tacl-5.0.6/setup.cfg
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-05-09 21:30:59.334202 tacl-5.0.6/tacl/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      705 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    32400 2022-09-23 22:30:27.000000 tacl-5.0.6/tacl/__main__.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-05-09 21:30:59.334202 tacl-5.0.6/tacl/assets/
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-05-09 21:30:59.338202 tacl-5.0.6/tacl/assets/results_highlight/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1229 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/results_highlight/heatmap.js
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-05-09 21:30:59.338202 tacl-5.0.6/tacl/assets/templates/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1801 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/templates/lifetime.html
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1186 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/templates/ngram_highlight.html
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      954 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/templates/results_highlight.html
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1103 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/templates/sequence.html
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-05-09 21:30:59.338202 tacl-5.0.6/tacl/assets/xslt/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      807 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/xslt/CBETA_T0062_rest.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      891 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/xslt/CBETA_T0220_reparent_divs.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1284 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/xslt/CBETA_T0418_fix_verse.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2115 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/xslt/CBETA_extract_commentary.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1800 2023-04-07 08:50:00.000000 tacl-5.0.6/tacl/assets/xslt/CBETA_extract_div.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1801 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/xslt/CBETA_extract_verse.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      748 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/xslt/CBETA_remove_divs.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     4838 2023-03-05 23:53:29.000000 tacl-5.0.6/tacl/assets/xslt/prepare_tei_cbeta_github.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3381 2023-03-05 08:38:21.000000 tacl-5.0.6/tacl/assets/xslt/strip_tei.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     4330 2021-10-08 21:27:56.000000 tacl-5.0.6/tacl/catalogue.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-05-09 21:30:59.338202 tacl-5.0.6/tacl/cli/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)        0 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/cli/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3449 2021-09-27 01:52:24.000000 tacl-5.0.6/tacl/cli/formatters.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3808 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/cli/utils.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1579 2021-07-14 09:03:55.000000 tacl-5.0.6/tacl/colour.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    40247 2022-10-01 23:28:52.000000 tacl-5.0.6/tacl/constants.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     4253 2022-09-23 04:53:43.000000 tacl-5.0.6/tacl/corpus.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    36087 2022-09-19 01:51:28.000000 tacl-5.0.6/tacl/data_store.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1044 2021-07-14 09:03:55.000000 tacl-5.0.6/tacl/decorators.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      610 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/exceptions.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     7990 2023-01-30 22:09:57.000000 tacl-5.0.6/tacl/highlighter.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    19580 2021-07-14 09:03:57.000000 tacl-5.0.6/tacl/jitc.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     6635 2021-07-14 09:03:55.000000 tacl-5.0.6/tacl/lifetime_report.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    10364 2022-09-23 03:38:57.000000 tacl-5.0.6/tacl/normaliser.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3064 2022-05-05 07:43:28.000000 tacl-5.0.6/tacl/report.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    45042 2022-10-16 22:23:08.000000 tacl-5.0.6/tacl/results.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    13355 2021-09-27 01:52:15.000000 tacl-5.0.6/tacl/sequence.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     5494 2021-09-12 03:15:37.000000 tacl-5.0.6/tacl/splitter.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     5400 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/statistics_report.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3873 2023-04-07 09:23:18.000000 tacl-5.0.6/tacl/stripper.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    32720 2023-04-10 20:22:44.000000 tacl-5.0.6/tacl/tei_corpus.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     6013 2022-09-20 05:54:17.000000 tacl-5.0.6/tacl/text.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1140 2021-07-14 09:03:55.000000 tacl-5.0.6/tacl/tokenizer.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1248 2021-07-14 09:03:55.000000 tacl-5.0.6/tacl/work_joiner.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-05-09 21:30:59.334202 tacl-5.0.6/tacl.egg-info/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    39343 2023-05-09 21:30:59.000000 tacl-5.0.6/tacl.egg-info/PKG-INFO
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1267 2023-05-09 21:30:59.000000 tacl-5.0.6/tacl.egg-info/SOURCES.txt
+-rw-r--r--   0 jamie     (1000) jamie     (1000)        1 2023-05-09 21:30:59.000000 tacl-5.0.6/tacl.egg-info/dependency_links.txt
+-rw-r--r--   0 jamie     (1000) jamie     (1000)       44 2023-05-09 21:30:59.000000 tacl-5.0.6/tacl.egg-info/entry_points.txt
+-rw-r--r--   0 jamie     (1000) jamie     (1000)       44 2023-05-09 21:30:59.000000 tacl-5.0.6/tacl.egg-info/requires.txt
+-rw-r--r--   0 jamie     (1000) jamie     (1000)        5 2023-05-09 21:30:59.000000 tacl-5.0.6/tacl.egg-info/top_level.txt
```

### Comparing `tacl-5.0.5/CHANGES` & `tacl-5.0.6/CHANGES`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+5.0.6  2023-05-10  Jamie Norrish  <jamie@artefact.org.nz>
+
+  * Reworked build configuration.
+
+  * Updated corpus preparation for Taisho, both markup handling and
+    further splits.
+
+
 5.0.5  2022-09-24  Jamie Norrish  <jamie@artefact.org.nz>
 
   * Improved performance of denormalisation sufficiently to be useful
     in real cases.
 
 
 5.0.4  2022-08-06  Jamie Norrish  <jamie@artefact.org.nz>
```

### Comparing `tacl-5.0.5/LICENCE` & `tacl-5.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/PKG-INFO` & `tacl-5.0.6/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: tacl
-Version: 5.0.5
-Summary: Text analyser for corpus linguistics
-Home-page: https://github.com/ajenhl/tacl
-Author: Jamie Norrish
-Author-email: jamie@artefact.org.nz
-License: GPLv3+
-Project-URL: Documentation, http://tacl.readthedocs.io/en/latest/
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Text Processing :: Linguistic
-License-File: LICENCE
-
 TACL
 ====
 
 tacl is a tool for performing basic text analysis on the texts
 available from the `Chinese Buddhist Electronic Text Association`_
 (CBETA). It is largely generic, however, and can operate with minor
 modifications on other corpora.
```

### Comparing `tacl-5.0.5/tacl/__init__.py` & `tacl-5.0.6/tacl/__init__.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/__main__.py` & `tacl-5.0.6/tacl/__main__.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/assets/results_highlight/heatmap.js` & `tacl-5.0.6/tacl/assets/results_highlight/heatmap.js`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/assets/templates/lifetime.html` & `tacl-5.0.6/tacl/assets/templates/lifetime.html`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/assets/templates/ngram_highlight.html` & `tacl-5.0.6/tacl/assets/templates/ngram_highlight.html`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/assets/templates/results_highlight.html` & `tacl-5.0.6/tacl/assets/templates/results_highlight.html`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/assets/templates/sequence.html` & `tacl-5.0.6/tacl/assets/templates/sequence.html`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/assets/xslt/CBETA_T0062_rest.xsl` & `tacl-5.0.6/tacl/assets/xslt/CBETA_T0062_rest.xsl`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/assets/xslt/CBETA_T0220_reparent_divs.xsl` & `tacl-5.0.6/tacl/assets/xslt/CBETA_T0220_reparent_divs.xsl`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/assets/xslt/CBETA_T0418_fix_verse.xsl` & `tacl-5.0.6/tacl/assets/xslt/CBETA_T0418_fix_verse.xsl`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/assets/xslt/CBETA_extract_commentary.xsl` & `tacl-5.0.6/tacl/assets/xslt/CBETA_extract_commentary.xsl`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/assets/xslt/CBETA_extract_div.xsl` & `tacl-5.0.6/tacl/assets/xslt/CBETA_extract_div.xsl`

 * *Files 22% similar despite different names*

#### Comparing `tacl-5.0.5/tacl/assets/xslt/CBETA_extract_div.xsl` & `tacl-5.0.6/tacl/assets/xslt/CBETA_extract_div.xsl`

```diff
@@ -3,23 +3,39 @@
   <xsl:output encoding="UTF-8" method="xml"/>
   <xsl:param name="position"/>
   <xsl:param name="div_type"/>
   <xsl:param name="treatment"/>
   <xsl:template match="tei:body">
     <xsl:copy>
       <xsl:apply-templates select="@*"/>
-      <xsl:variable name="div" select=".//cb:div[@type=$div_type][count(ancestor::cb:div[@type=$div_type] | preceding::cb:div[@type=$div_type])=$position]"/>
-      <xsl:copy-of select="$div"/>
-      <xsl:if test="$treatment = 'merge_to_preceding'">
-        <xsl:variable name="next-div" select="$div/following::cb:div[@type=$div_type][1]"/>
-        <xsl:if test="not(normalize-space($next-div/cb:mulu/text()))">
-          <xsl:copy-of select="$next-div"/>
-        </xsl:if>
-      </xsl:if>
+      <xsl:choose>
+        <xsl:when test="$div_type">
+          <xsl:variable name="div" select=".//cb:div[@type=$div_type][count(ancestor::cb:div[@type=$div_type] | preceding::cb:div[@type=$div_type])=$position]"/>
+          <xsl:call-template name="handle_div">
+            <xsl:with-param name="div" select="$div"/>
+          </xsl:call-template>
+        </xsl:when>
+        <xsl:otherwise>
+          <xsl:variable name="div" select=".//cb:div[not(@type)][count(ancestor::cb:div[not(@type)] | preceding::cb:div[not(@type)])=$position]"/>
+          <xsl:call-template name="handle_div">
+            <xsl:with-param name="div" select="$div"/>
+          </xsl:call-template>
+        </xsl:otherwise>
+      </xsl:choose>
     </xsl:copy>
   </xsl:template>
   <xsl:template match="@*|node()">
     <xsl:copy>
       <xsl:apply-templates select="@*|node()"/>
     </xsl:copy>
   </xsl:template>
+  <xsl:template name="handle_div">
+    <xsl:param name="div"/>
+    <xsl:copy-of select="$div"/>
+    <xsl:if test="$treatment = 'merge_to_preceding'">
+      <xsl:variable name="next-div" select="$div/following::cb:div[@type=$div_type][1]"/>
+      <xsl:if test="not(normalize-space($next-div/cb:mulu/text()))">
+        <xsl:copy-of select="$next-div"/>
+      </xsl:if>
+    </xsl:if>
+  </xsl:template>
 </xsl:stylesheet>
```

### Comparing `tacl-5.0.5/tacl/assets/xslt/CBETA_extract_verse.xsl` & `tacl-5.0.6/tacl/assets/xslt/CBETA_extract_verse.xsl`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/assets/xslt/CBETA_remove_divs.xsl` & `tacl-5.0.6/tacl/assets/xslt/CBETA_remove_divs.xsl`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/assets/xslt/prepare_tei_cbeta_github.xsl` & `tacl-5.0.6/tacl/assets/xslt/prepare_tei_cbeta_github.xsl`

 * *Files 10% similar despite different names*

#### Comparing `tacl-5.0.5/tacl/assets/xslt/prepare_tei_cbeta_github.xsl` & `tacl-5.0.6/tacl/assets/xslt/prepare_tei_cbeta_github.xsl`

```diff
@@ -3,15 +3,15 @@
   <!-- In order to handle app crit entries that are demarcated by
        tei:anchor elements, every tei element and piece of text is
        checked for being within a pair of anchors. If it is not, then
        it is processed as normal by templates in the mode "copy". -->
   <xsl:output encoding="UTF-8" method="xml"/>
   <xsl:strip-space elements="*"/>
   <xsl:key name="anchored" match="tei:note[@target]" use="substring-after(@target, '#')"/>
-  <xsl:key name="anchored_start" match="*[@from]" use="substring-after(@from, '#')"/>
+  <xsl:key name="anchored_start" match="cb:div[@type='apparatus']//*[@from]" use="substring-after(@from, '#')"/>
   <xsl:template match="tei:anchor" mode="copy">
     <xsl:apply-templates select="key('anchored', @xml:id)"/>
     <xsl:apply-templates select="key('anchored_start', @xml:id)"/>
   </xsl:template>
   <!-- Keep tei:app/@from in order to be able to text-specific
        manipulations (eg, for T0418). -->
   <xsl:template match="tei:app/@to"/>
@@ -42,15 +42,14 @@
         <xsl:value-of select="tei:charProp[tei:localName='rjchar']/tei:value"/>
       </xsl:when>
       <xsl:otherwise>
         <xsl:text>GAIJI WITHOUT REPRESENTATION</xsl:text>
       </xsl:otherwise>
     </xsl:choose>
   </xsl:template>
-  <xsl:template match="tei:listWit" mode="copy"/>
   <xsl:template match="tei:note/@target"/>
   <xsl:template match="tei:*/@wit">
     <xsl:attribute name="wit">
       <xsl:for-each select="id(translate(., '#', ''))">
         <xsl:value-of select="."/>
       </xsl:for-each>
     </xsl:attribute>
@@ -63,14 +62,22 @@
         <xsl:text>|</xsl:text>
         <xsl:value-of select="tei:name"/>
         <xsl:text>}</xsl:text>
       </xsl:for-each>
     </xsl:attribute>
   </xsl:template>
   <xsl:template match="tei:editionStmt/tei:respStmt" mode="copy"/>
+  <xsl:template match="tei:witness" mode="copy">
+    <xsl:copy>
+      <!-- We do not want the xml:id attribute, since this witness
+           list will be superceded by the witness list for the
+           teiCorpus. -->
+      <xsl:apply-templates select="node()"/>
+    </xsl:copy>
+  </xsl:template>
   <xsl:template match="cb:tt/@from"/>
   <xsl:template match="cb:tt/@to"/>
   <!-- Handling moving the apparatus criticus etc into the body. -->
   <xsl:template match="tei:*|text()" priority="10">
     <xsl:variable name="beginning" select="substring-after(preceding-sibling::tei:anchor[starts-with(@xml:id, 'beg')][1]/@xml:id, 'beg')"/>
     <xsl:variable name="ending" select="substring-after(following-sibling::tei:anchor[starts-with(@xml:id, 'end')][1]/@xml:id, 'end')"/>
     <xsl:if test="not($beginning and $beginning = $ending)">
```

### Comparing `tacl-5.0.5/tacl/assets/xslt/strip_tei.xsl` & `tacl-5.0.6/tacl/assets/xslt/strip_tei.xsl`

 * *Files 23% similar despite different names*

#### Comparing `tacl-5.0.5/tacl/assets/xslt/strip_tei.xsl` & `tacl-5.0.6/tacl/assets/xslt/strip_tei.xsl`

```diff
@@ -30,14 +30,17 @@
     <xsl:text/>
     <xsl:apply-templates select="node()"/>
   </xsl:template>
   <xsl:template match="tei:lb[not(local-name(following-sibling::node()[1])='lb')]">
     <xsl:call-template name="add_blank_line"/>
   </xsl:template>
   <xsl:template match="tei:lem">
+    <!-- Although sometimes witnesses are defined on the tei:lem,
+         sometimes they are not, and all that matters is that the
+         current witness is not associated with a tei:rdg. -->
     <xsl:if test="not(../tei:rdg[contains(concat(' ', @wit, ' '), $witness_ref)])">
       <xsl:apply-templates/>
     </xsl:if>
   </xsl:template>
   <xsl:template match="cb:mulu"/>
   <xsl:template match="tei:note"/>
   <xsl:template match="tei:note[@place = 'inline']">
@@ -45,17 +48,34 @@
   </xsl:template>
   <xsl:template match="tei:rdg">
     <xsl:variable name="wit" select="concat(' ', @wit, ' ')"/>
     <xsl:if test="contains($wit, $witness_ref)">
       <xsl:apply-templates/>
     </xsl:if>
   </xsl:template>
+  <xsl:template match="cb:sg">
+    <xsl:text>(</xsl:text>
+    <xsl:apply-templates/>
+    <xsl:text>)</xsl:text>
+  </xsl:template>
+  <xsl:template match="cb:t">
+    <xsl:choose>
+      <xsl:when test="@xml:lang = 'zh-Hant'">
+        <xsl:apply-templates/>
+      </xsl:when>
+      <xsl:when test="not(preceding-sibling::cb:t) and not(../cb:t[@xml:lang='zh-Hant'])">
+        <xsl:apply-templates/>
+      </xsl:when>
+      <xsl:when test="cb:yin">
+        <xsl:apply-templates/>
+      </xsl:when>
+    </xsl:choose>
+  </xsl:template>
   <xsl:template match="tei:teiHeader"/>
   <xsl:template match="tei:body//tei:title"/>
   <xsl:template match="text()">
     <xsl:value-of select="normalize-space()"/>
   </xsl:template>
-  <xsl:template match="cb:t[not(@xml:lang='zh')]"/>
   <xsl:template name="add_blank_line">
     <xsl:text/>
   </xsl:template>
 </xsl:stylesheet>
```

### Comparing `tacl-5.0.5/tacl/catalogue.py` & `tacl-5.0.6/tacl/catalogue.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/cli/formatters.py` & `tacl-5.0.6/tacl/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/cli/utils.py` & `tacl-5.0.6/tacl/cli/utils.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/colour.py` & `tacl-5.0.6/tacl/colour.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/constants.py` & `tacl-5.0.6/tacl/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,16 +417,16 @@
 RESULTS_COLLAPSE_WITNESSES_HELP = '''\
     Collapse result rows for multiple witnesses having the same count
     for an n-gram. Instead of the "{}" column, all of the witnesses
     (per work) with the same n-gram count are listed, comma separated,
     in the "{}" column.'''.format(SIGLUM_FIELDNAME, SIGLA_FIELDNAME)
 RESULTS_DENORMALISE_CORPUS_HELP = '''\
     Path to directory containing the original (unnormalised)
-    corpus. This option must be given along with --denormalise-mapping
-    in order for denormalisation to be performed.'''
+    corpus. This option must be given along with --denormalise in
+    order for denormalisation to be performed.'''
 RESULTS_DENORMALISE_MAPPING_HELP = '''\
     Denormalise result n-grams using mapping at the supplied path. The
     unnormalised corpus must also be specified in the
     --denormalise-corpus option.'''
 RESULTS_DESCRIPTION = '''\
     Modify a query results file by adding, removing or otherwise
     manipulating result rows. Outputs the new set of results.'''
@@ -460,14 +460,19 @@
     with an extra column, "{}", giving the normalised form each was
     derived from. Since denormalised intersect results may no longer
     conform to normal intersect rules (that each n-gram occurs at
     least once within each label), running some further operations
     (such as extend) is likely to cause unwanted removal of
     results.
 
+    --denormalise should always be performed (if at all) before
+    --reduce. The counts of the denormalised n-grams will be the full
+    count of all instances in a witness, even if a --reduce on the
+    normalised results had reduced counts.
+
     It is important to be careful with the use of --reduce. Coupled
     with filters such as --max-size, --min-count, etc, many results
     may be discarded without trace (since the reduce occurs
     first). Note too that performing "reduce" on a set of results more
     than once will make the results inaccurate!
 
     --min-count and --max-count set the range within which the total
```

### Comparing `tacl-5.0.5/tacl/corpus.py` & `tacl-5.0.6/tacl/corpus.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/data_store.py` & `tacl-5.0.6/tacl/data_store.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/decorators.py` & `tacl-5.0.6/tacl/decorators.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/exceptions.py` & `tacl-5.0.6/tacl/exceptions.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/highlighter.py` & `tacl-5.0.6/tacl/highlighter.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/jitc.py` & `tacl-5.0.6/tacl/jitc.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/lifetime_report.py` & `tacl-5.0.6/tacl/lifetime_report.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/normaliser.py` & `tacl-5.0.6/tacl/normaliser.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/report.py` & `tacl-5.0.6/tacl/report.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/results.py` & `tacl-5.0.6/tacl/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         if self._matches.empty:
             self._matches[constants.LABEL_COUNT_FIELDNAME] = 0
         else:
             self._matches.loc[:, constants.LABEL_COUNT_FIELDNAME] = 0
             self._matches = self._matches.groupby(
                 [constants.LABEL_FIELDNAME, constants.NGRAM_FIELDNAME],
-                sort=False).apply(add_label_count)
+                group_keys=False, sort=False).apply(add_label_count)
         self._logger.info('Finished adding label count')
 
     @requires_columns([constants.NGRAM_FIELDNAME, constants.WORK_FIELDNAME,
                        constants.COUNT_FIELDNAME, constants.LABEL_FIELDNAME])
     def add_label_work_count(self):
         """Adds to each result row a count of the number of works within the
         label contain that n-gram.
@@ -116,15 +116,15 @@
 
         if self._matches.empty:
             self._matches[constants.LABEL_WORK_COUNT_FIELDNAME] = 0
         else:
             self._matches.loc[:, constants.LABEL_WORK_COUNT_FIELDNAME] = 0
             self._matches = self._matches.groupby(
                 [constants.LABEL_FIELDNAME, constants.NGRAM_FIELDNAME],
-                sort=False).apply(add_label_text_count)
+                group_keys=False, sort=False).apply(add_label_text_count)
         self._logger.info('Finished adding label work count')
 
     def _annotate_bifurcated_extend_data(self, row, smaller, larger, tokenize,
                                          join):
         """Returns `row` annotated with whether it should be deleted or not.
 
         An n-gram is marked for deletion if:
@@ -252,30 +252,29 @@
         self._matches.loc[:, constants.SIGLA_FIELDNAME] = \
             self._matches[constants.SIGLUM_FIELDNAME]
         # This code makes the not unwarranted assumption that the same
         # n-gram means the same size and that the same work means the
         # same label.
         grouped = self._matches.groupby(
             [constants.WORK_FIELDNAME, constants.NGRAM_FIELDNAME,
-             constants.COUNT_FIELDNAME], sort=False)
+             constants.COUNT_FIELDNAME], group_keys=False, sort=False)
 
         def merge_sigla(df):
             # Take the first result row; only the siglum should differ
             # between them, and there may only be one row.
             merged = df[0:1]
             sigla = list(df[constants.SIGLA_FIELDNAME])
             sigla.sort()
             merged[constants.SIGLUM_FIELDNAME] = ', '.join(sigla)
             return merged
 
         self._matches = grouped.apply(merge_sigla)
         del self._matches[constants.SIGLA_FIELDNAME]
         self._matches.rename(columns={constants.SIGLUM_FIELDNAME:
-                                      constants.SIGLA_FIELDNAME},
-                             inplace=True)
+                                      constants.SIGLA_FIELDNAME}, inplace=True)
 
     def csv(self, fh):
         """Writes the results data to `fh` in CSV format and returns `fh`.
 
         :param fh: file to write data to
         :type fh: file object
         :rtype: file object
@@ -366,15 +365,16 @@
                         ngram, []).append(denormalised_ngram)
                     ngram_archive.setdefault(ngram, {}).setdefault(
                         size, []).append(denormalised_ngram)
             rows = create_denormalised_results(witness, work, siglum, label,
                                                ngram_data)
             return pd.DataFrame(rows, columns=fieldnames)
 
-        matches = self._matches.groupby(group_cols, sort=False).apply(
+        matches = self._matches.groupby(group_cols, group_keys=False,
+                                        sort=False).apply(
             denormalise_witness_ngrams)
         self._matches = matches
 
     @requires_columns([constants.NGRAM_FIELDNAME])
     def excise(self, ngram):
         """Removes all rows whose n-gram contains `ngram`.
 
@@ -613,16 +613,16 @@
                 constants.COUNT_FIELDNAME].sum()
             return match
 
         group_cols = [constants.WORK_FIELDNAME, constants.SIGLUM_FIELDNAME]
         # Remove zero-count results.
         self._matches = self._matches[
             self._matches[constants.COUNT_FIELDNAME] != 0]
-        self._matches = self._matches.groupby(group_cols, sort=False).apply(
-            witness_summary)
+        self._matches = self._matches.groupby(group_cols, group_keys=False,
+                                              sort=False).apply(witness_summary)
         del self._matches[constants.NGRAM_FIELDNAME]
         del self._matches[constants.SIZE_FIELDNAME]
         del self._matches[constants.COUNT_FIELDNAME]
 
     @staticmethod
     def _is_intersect_results(results):
         """Returns True if all of the n-grams in `results` exist in all of
@@ -727,15 +727,16 @@
         # won't have been added. Therefore just return immediately.
         if self._matches.empty:
             return
         matches = self._matches
         if label is not None:
             matches = matches[matches[constants.LABEL_FIELDNAME] == label]
         matches = matches.groupby(
-            constants.NGRAM_FIELDNAME, sort=False).apply(calculate_total)
+            constants.NGRAM_FIELDNAME, group_keys=False, sort=False).apply(
+                calculate_total)
         ngrams = None
         if minimum:
             ngrams = matches[matches['total_count'] >= minimum][
                 constants.NGRAM_FIELDNAME].unique()
         if maximum:
             max_ngrams = matches[matches['total_count'] <= maximum][
                 constants.NGRAM_FIELDNAME].unique()
```

### Comparing `tacl-5.0.5/tacl/sequence.py` & `tacl-5.0.6/tacl/sequence.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/splitter.py` & `tacl-5.0.6/tacl/splitter.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/statistics_report.py` & `tacl-5.0.6/tacl/statistics_report.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/stripper.py` & `tacl-5.0.6/tacl/stripper.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,18 +46,21 @@
                               witness_element.get(constants.XML + 'id')))
         if not witnesses:
             witnesses = [(constants.BASE_WITNESS, constants.BASE_WITNESS_ID)]
         return witnesses
 
     def _output_file(self, work, witnesses):
         work_dir = os.path.join(self._output_dir, work)
+        if not witnesses:
+            self._logger.warning('No text to output for {}'.format(work))
+            return
         try:
             os.makedirs(work_dir)
         except OSError as err:
-            logging.error('Could not create output directory: {}'.format(
+            self._logger.error('Could not create output directory: {}'.format(
                 err))
             raise
         for witness in witnesses.keys():
             witness_file_path = os.path.join(
                 work_dir, '{}.txt'.format(witness))
             with open(witness_file_path, 'wb') as output_file:
                 output_file.write(witnesses[witness].encode('utf-8'))
@@ -82,15 +85,16 @@
         work = os.path.splitext(os.path.basename(filename))[0]
         stripped_file_path = os.path.join(self._output_dir, work)
         self._logger.info('Stripping file {} into {}'.format(
             file_path, stripped_file_path))
         try:
             tei_doc = etree.parse(file_path)
         except etree.XMLSyntaxError:
-            logging.warning('XML file "{}" is invalid'.format(filename))
+            self._logger.warning('XML file "{}" is invalid'.format(filename))
             return
         witnesses = {}
         for witness, witness_id in self.get_witnesses(tei_doc):
             witness_param = "'{}'".format(witness_id)
             text = str(self.transform(tei_doc, witness_id=witness_param))
-            witnesses[witness] = text
+            if text.strip():
+                witnesses[witness] = text
         return work, witnesses
```

### Comparing `tacl-5.0.5/tacl/tei_corpus.py` & `tacl-5.0.6/tacl/tei_corpus.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,29 +124,31 @@
         :type source_tree: `etree._ElementTree`
         :rtype: `tuple` of `list`s
 
         """
         witnesses = set()
         bearers = source_tree.xpath('//tei:app/tei:*[@wit]',
                                     namespaces=constants.NAMESPACES)
-        for bearer in bearers:
-            for witness in witnesses_splitter.split(bearer.get('wit')):
-                if witness:
-                    witnesses.add(witness)
+        for witness in source_tree.xpath("//tei:witness",
+                                         namespaces=constants.NAMESPACES):
+            witnesses.add(witness.text[1:-1])
         return sorted(witnesses), bearers
 
     def _handle_resps(self, root):
         raise NotImplementedError
 
     def _handle_witnesses(self, root):
         """Returns `root` with a witness list added to the TEI header and @wit
         values changed to references."""
         witnesses, bearers = self.get_witnesses(root)
         if not witnesses:
             return root
+        for wit_list in root.xpath("//tei:listWit",
+                                   namespaces=constants.NAMESPACES):
+            wit_list.getparent().remove(wit_list)
         source_desc = root.xpath(
             '/tei:teiCorpus/tei:teiHeader/tei:fileDesc/tei:sourceDesc',
             namespaces=constants.NAMESPACES)[0]
         wit_list = etree.SubElement(source_desc, TEI + 'listWit')
         for index, siglum in enumerate(witnesses):
             wit = etree.SubElement(wit_list, TEI + 'witness')
             xml_id = 'wit{}'.format(index + 1)
@@ -208,19 +210,18 @@
                 'tei:author', namespaces=constants.NAMESPACES)[0].text
         except IndexError:
             pass
         return root
 
     def _postprocess(self, work, tree):
         """Post-process the XML document `tree`."""
+        self._output_tree('{}.xml'.format(work), tree)
         pp_func = '_postprocess_{}'.format(work)
         if hasattr(self, pp_func):
             getattr(self, pp_func)(work, tree)
-        else:
-            self._output_tree('{}.xml'.format(work), tree)
 
     def tidy(self):
         if not os.path.exists(self._output_dir):
             try:
                 os.makedirs(self._output_dir)
             except OSError as err:
                 self._logger.error(
@@ -385,16 +386,19 @@
         """Post-process the XML document `root`."""
         div_types = [('xu', 'xu'), ('w', 'endmatter')]
         tree = self._extract_divs(work, tree, div_types)
         super()._postprocess(work, tree)
 
     def _postprocess_div_mulu(self, work, tree, div_type,
                               treatment=LEAVE_UNNAMED_DIVS, exclude=None):
-        divs = tree.xpath('//cb:div[@type="{}"]'.format(div_type),
-                          namespaces=constants.NAMESPACES)
+        if not div_type:
+            xpath = '//cb:div[not(@type)]'
+        else:
+            xpath = '//cb:div[@type="{}"]'.format(div_type)
+        divs = tree.xpath(xpath, namespaces=constants.NAMESPACES)
         seen_filenames = {}
         for position, div in enumerate(divs):
             div_tree = self._transform_div(tree, position=str(position),
                                            div_type='"{}"'.format(div_type),
                                            treatment='"{}"'.format(treatment))
             div_tree = self._remove_subdivs(div_tree, exclude)
             try:
@@ -459,16 +463,23 @@
             seen_filenames = self._output_tree(div_filename, div_tree,
                                                seen_filenames)
         jing_divs = tree.xpath('//cb:div[@type="jing"]',
                                namespaces=constants.NAMESPACES)
         for position, div in enumerate(jing_divs):
             div_tree = self._transform_div(tree, position=str(position),
                                            div_type='"jing"')
-            pin_mulu = self._get_mulu(div, '../cb:mulu[1]/text()')
-            jing_mulu = self._get_mulu(div, 'cb:mulu[1]/text()')
+            try:
+                pin_mulu = self._get_mulu(
+                    div, 'ancestor::cb:div[@type="pin"][1]/cb:mulu[1]/text()')
+            except IndexError:
+                pin_mulu = 'unnamed'
+            try:
+                jing_mulu = self._get_mulu(div, 'cb:mulu[1]/text()')
+            except IndexError:
+                jing_mulu = 'unnumbered'
             div_filename = '{}-{}-{}.xml'.format(work, pin_mulu, jing_mulu)
             self._output_tree(div_filename, div_tree)
 
     def _postprocess_T0150A(self, work, tree):
         """Post-process the XML document T0150A.xml.
 
         Divide into multiple files, one for each cb:div[@type='jing'],
@@ -476,16 +487,15 @@
 
         """
         self._postprocess_div_mulu(work, tree, 'jing')
 
     def _postprocess_T0152(self, work, tree):
         """Post-process the XML document T0152.xml.
 
-        Extract the first (should be only) cb:div[@type='other'] into
-        its own file.
+        Extract the first cb:div[@type='other'] into its own file.
 
         Divide into multiple files, one for each cb:div[@type='jing'],
         named according to the cb:mulu content for that div.
 
         """
         div_tree = self._transform_div(tree, position='0', div_type='"other"')
         div_tree = self._remove_subdivs(div_tree, ['jing'])
@@ -528,35 +538,114 @@
         verse_tree = extract_verse(tree)
         verse_filename = '{}-verses.xml'.format(work)
         self._output_tree(verse_filename, verse_tree)
         prose_tree = extract_verse(tree, inverse='1')
         prose_filename = '{}-ex-verses.xml'.format(work)
         self._output_tree(prose_filename, prose_tree)
 
+    def _postprocess_T0201(self, work, tree):
+        """Post-process the XML document T0201.xml.
+
+        Divide into multiple files, one for each cb:div[@type='other'].
+
+        """
+        self._postprocess_div_mulu(work, tree, 'other')
+
+    def _postprocess_T0202(self, work, tree):
+        """Post-process the XML document T0202.xml.
+
+        Divide into multiple files, one for each cb:div[@type='pin'].
+
+        """
+        self._postprocess_div_mulu(work, tree, 'pin')
+
+    def _postprocess_T0203(self, work, tree):
+        """Post-process the XML document T0203.xml.
+
+        Divide into multiple files, one for each cb:div[@type='other'].
+
+        """
+        self._postprocess_div_mulu(work, tree, 'other')
+
+    def _postprocess_T0204(self, work, tree):
+        """Post-process the XML document T0204.xml.
+
+        Divide into multiple files, one for each cb:div[@type='other'].
+
+        """
+        self._postprocess_div_mulu(work, tree, 'other')
+
+    def _postprocess_T0205(self, work, tree):
+        """Post-process the XML document T0205.xml.
+
+        Divide into multiple files, one for each cb:div[@type='other'].
+
+        """
+        self._postprocess_div_mulu(work, tree, 'other')
+
+    def _postprocess_T0206(self, work, tree):
+        """Post-process the XML document T0206.xml.
+
+        Divide into multiple files, one for each cb:div[@type='other'].
+
+        """
+        self._postprocess_div_mulu(work, tree, 'other')
+
+    def _postprocess_T0207(self, work, tree):
+        """Post-process the XML document T0207.xml.
+
+        Divide into multiple files, one for each cb:div[@type='other']
+        and cb:div with no @type.
+
+        """
+        self._postprocess_div_mulu(work, tree, 'other')
+        self._postprocess_div_mulu(work, tree, '')
+
+    def _postprocess_T0208(self, work, tree):
+        """Post-process the XML document T0208.xml.
+
+        Divide into multiple files, one for each cb:div[@type='other']
+        and cb:div with no @type.
+
+        """
+        self._postprocess_div_mulu(work, tree, 'other')
+        self._postprocess_div_mulu(work, tree, '')
+
+    def _postprocess_T0209(self, work, tree):
+        """Post-process the XML document T0209.xml.
+
+        Divide into multiple files, one for each cb:div[@type='other'].
+
+        """
+        self._postprocess_div_mulu(work, tree, 'other')
+
     def _postprocess_T0220(self, work, tree):
         """Post-process the XML document T0220.xml.
 
         Divide into multiple files, one for each cb:div[@type='hui'],
         named according to its position. This is complicated by the
         fact that one of the parts (T0220b) is meant to be entirely
         within the single hui of T0220a but does not have any
         containing div.
 
+        Also divide into one file for each cb:div[@type='dharani'].
+
         """
         xslt_filename = resource_filename(
             __name__, 'assets/xslt/CBETA_T0220_reparent_divs.xsl')
         move_non_hui_divs = etree.XSLT(etree.parse(xslt_filename))
         tree = move_non_hui_divs(tree)
         divs = tree.xpath('//cb:div[@type="hui"]',
                           namespaces=constants.NAMESPACES)
         for position, div in enumerate(divs):
             div_tree = self._transform_div(tree, position=str(position),
                                            div_type='"hui"')
             div_filename = '{}-{}.xml'.format(work, position + 1)
             self._output_tree(div_filename, div_tree)
+        self._postprocess_div_mulu(work, tree, 'dharani')
 
     def _postprocess_T0225(self, work, tree):
         """Post-process the XML document T0225.xml.
 
         Divide into two files, one containing all of the
         tei:note[@place='inline'] material, and one the rest.
 
@@ -658,23 +747,23 @@
     def _postprocess_T1361(self, work, tree):
         """Post-process the XML document T1361.xml.
 
         Divide into two files: the cb:div[@type='jing'] and the
         cb:div[@type='廣釋'].
 
         """
-        div_tree = self._transform_div(tree, position='0', div_type='jing')
+        div_tree = self._transform_div(tree, position='0', div_type='"jing"')
         div_filename = '{}-root.xml'.format(work)
         self._output_tree(div_filename, div_tree)
-        div_tree = self._transform_div(tree, position='0', div_type='廣釋')
+        div_tree = self._transform_div(tree, position='0', div_type='"廣釋"')
         div_filename = '{}-廣釋.xml'.format(work)
         self._output_tree(div_filename, div_tree)
 
     def _postprocess_T1646(self, work, tree):
-        """Post-process the XML document T0664.xml.
+        """Post-process the XML document T0646.xml.
 
         Divide into multiple files, one for each cb:div[@type='pin'],
         named according to the cb:mulu content for that div.
 
         """
         self._postprocess_div_mulu(work, tree, 'pin')
 
@@ -703,8 +792,19 @@
             file_path, output_file))
         try:
             tei_doc = etree.parse(file_path)
         except etree.XMLSyntaxError as err:
             self._logger.error('XML file "{}" is invalid: {}'.format(
                 file_path, err))
             raise
+        # Remove spanning anchors that point to something other than
+        # an item in the apparatus criticus.
+        xpath = '//tei:anchor[starts-with(@xml:id, "beg") or ' \
+            'starts-with(@xml:id, "end")]'
+        for anchor in tei_doc.xpath(xpath, namespaces=constants.NAMESPACES):
+            ref = "#{}".format(anchor.get(constants.XML + 'id'))
+            xpath = '/tei:TEI/tei:text/tei:back/cb:div[@type="apparatus"]//' \
+                'tei:app[@from = $ref or @to = $ref]'
+            if not tei_doc.xpath(xpath, namespaces=constants.NAMESPACES,
+                                 ref=ref):
+                anchor.attrib.clear()
         return self.transform(tei_doc).getroot()
```

### Comparing `tacl-5.0.5/tacl/text.py` & `tacl-5.0.6/tacl/text.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/tokenizer.py` & `tacl-5.0.6/tacl/tokenizer.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl/work_joiner.py` & `tacl-5.0.6/tacl/work_joiner.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.5/tacl.egg-info/SOURCES.txt` & `tacl-5.0.6/tacl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 CHANGES
 LICENCE
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 tacl/__init__.py
 tacl/__main__.py
 tacl/catalogue.py
 tacl/colour.py
 tacl/constants.py
 tacl/corpus.py
 tacl/data_store.py
```

