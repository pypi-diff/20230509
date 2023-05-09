# Comparing `tmp/OBITools3-3.0.1b8.tar.gz` & `tmp/OBITools3-3.0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OBITools3-3.0.1b8.tar", last modified: Mon May 10 04:23:22 2021, max compression
+gzip compressed data, was "dist/OBITools3-3.0.1b9.tar", last modified: Wed Jun  2 03:59:20 2021, max compression
```

## Comparing `OBITools3-3.0.1b8.tar` & `OBITools3-3.0.1b9.tar`

### file list

```diff
@@ -1,308 +1,308 @@
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.731318 OBITools3-3.0.1b8/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      336 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/MANIFEST.in
--rw-r--r--   0 mercierc (520622000) domain users (520600513)     7509 2021-05-10 04:23:22.731318 OBITools3-3.0.1b8/PKG-INFO
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6445 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/README.md
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.291388 OBITools3-3.0.1b8/python/
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.303386 OBITools3-3.0.1b8/python/OBITools3.egg-info/
--rw-r--r--   0 mercierc (520622000) domain users (520600513)     7509 2021-05-10 04:23:22.000000 OBITools3-3.0.1b8/python/OBITools3.egg-info/PKG-INFO
--rw-r--r--   0 mercierc (520622000) domain users (520600513)     8784 2021-05-10 04:23:22.000000 OBITools3-3.0.1b8/python/OBITools3.egg-info/SOURCES.txt
--rw-r--r--   0 mercierc (520622000) domain users (520600513)        1 2021-05-10 04:23:22.000000 OBITools3-3.0.1b8/python/OBITools3.egg-info/dependency_links.txt
--rw-r--r--   0 mercierc (520622000) domain users (520600513)       10 2021-05-10 04:23:22.000000 OBITools3-3.0.1b8/python/OBITools3.egg-info/top_level.txt
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.307385 OBITools3-3.0.1b8/python/obitools3/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/__init__.py
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.323383 OBITools3-3.0.1b8/python/obitools3/apps/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/apps/__init__.py
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       82 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/apps/arguments.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1748 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/apps/arguments.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       68 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/apps/command.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1010 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/apps/command.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      313 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/apps/config.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3127 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/apps/config.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       56 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/apps/logging.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1097 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/apps/logging.pyx
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.323383 OBITools3-3.0.1b8/python/obitools3/apps/optiongroups/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    11995 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/apps/optiongroups/__init__.py
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1371 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/apps/progress.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4983 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/apps/progress.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      158 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/apps/temp.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2340 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/apps/temp.pyx
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.391372 OBITools3-3.0.1b8/python/obitools3/commands/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/__init__.py
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     9700 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/addtaxids.pyx
--rw-r--r--   0 mercierc (520622000) domain users (520600513)      712 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/align.pxd
--rw-r--r--   0 mercierc (520622000) domain users (520600513)    12645 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/align.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       85 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/alignpairedend.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     9324 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/alignpairedend.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    15453 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/annotate.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4544 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/build_ref_db.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6323 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/cat.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6014 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/clean.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      776 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/clean_dms.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1819 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/count.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     9866 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/ecopcr.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6726 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/ecotag.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2942 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/export.pyx
--rw-r--r--   0 mercierc (520622000) domain users (520600513)    16565 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/grep.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4213 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/head.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1819 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/history.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    18363 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/import.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1141 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/less.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1095 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/ls.pyx
--rw-r--r--   0 mercierc (520622000) domain users (520600513)    28351 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/ngsfilter.pyx
--rw-r--r--   0 mercierc (520622000) domain users (520600513)      977 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/rm.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5862 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/sort.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     9038 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/stats.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4463 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/tail.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    20584 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/test.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      493 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/uniq.pxd
--rw-r--r--   0 mercierc (520622000) domain users (520600513)    25321 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/commands/uniq.pyx
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.407369 OBITools3-3.0.1b8/python/obitools3/dms/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       43 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/__init__.py
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.427366 OBITools3-3.0.1b8/python/obitools3/dms/capi/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/capi/__init__.py
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1440 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/capi/apat.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      388 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/capi/build_reference_db.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1615 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/capi/kmer_similarity.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      493 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/capi/obiclean.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1584 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/capi/obidms.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2661 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/capi/obidmscolumn.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      952 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/capi/obiecopcr.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      530 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/capi/obiecotag.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      250 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/capi/obierrno.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1989 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/capi/obilcsalign.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2844 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/capi/obitaxonomy.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1308 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/capi/obitypes.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      240 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/capi/obiutils.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    19912 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/capi/obiview.pxd
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.439364 OBITools3-3.0.1b8/python/obitools3/dms/column/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       47 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/__init__.py
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1593 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/column.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    25380 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/column.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      602 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/column_idx.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4821 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/column_idx.pyx
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.467360 OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       86 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/__init__.py
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1209 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/bool.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     7859 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/bool.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      672 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/char.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     8128 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/char.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      675 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/float.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     7957 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/float.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      669 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/int.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     7849 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/int.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      942 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/qual.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    11771 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/qual.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      697 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/seq.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     8896 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/seq.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      697 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/str.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     8955 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/str.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      279 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/dms.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    10855 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/dms.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1208 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/obiseq.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    15643 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/obiseq.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      495 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/object.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2762 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/object.pyx
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.475359 OBITools3-3.0.1b8/python/obitools3/dms/taxo/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      126 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/taxo/__init__.py
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1064 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/taxo/taxo.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    14382 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/taxo/taxo.pyx
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.479358 OBITools3-3.0.1b8/python/obitools3/dms/view/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      176 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/view/__init__.py
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.487357 OBITools3-3.0.1b8/python/obitools3/dms/view/typed_view/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       77 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/view/typed_view/__init__.py
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       96 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/view/typed_view/view_NUC_SEQS.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2600 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/view/typed_view/view_NUC_SEQS.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1876 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/view/view.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    36210 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/dms/view/view.pyx
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.499355 OBITools3-3.0.1b8/python/obitools3/files/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/files/__init__.py
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       96 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/files/linebuffer.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      488 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/files/linebuffer.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      388 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/files/uncompress.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3695 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/files/uncompress.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      115 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/files/universalopener.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      380 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/files/universalopener.pyx
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.511353 OBITools3-3.0.1b8/python/obitools3/format/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/format/__init__.py
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      246 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/format/fasta.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      780 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/format/fasta.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      246 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/format/fastq.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      888 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/format/fastq.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      161 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/format/header.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2808 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/format/header.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      156 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/format/tab.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2341 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/format/tab.pyx
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.547347 OBITools3-3.0.1b8/python/obitools3/libalign/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4988 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/__init__.py
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      232 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/_assemble.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5734 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/_assemble.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2117 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/_dynamic.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     9675 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/_dynamic.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      177 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/_freeendgap.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5467 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/_freeendgap.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      153 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/_freeendgapfm.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      368 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/_freeendgapfm.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      248 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/_nws.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5403 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/_nws.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3801 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/_qsassemble.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3973 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/_qsrassemble.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      247 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/_rassemble.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5422 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/_rassemble.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     8771 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/_solexapairend.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      941 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/apat_pattern.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5813 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/apat_pattern.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1093 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/shifted_ali.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5522 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/shifted_ali.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1369 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/libalign/solexapairend.py
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.579342 OBITools3-3.0.1b8/python/obitools3/parsers/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/__init__.py
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      183 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/embl.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5802 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/embl.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       30 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/embl_genbank_features.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4120 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/embl_genbank_features.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      183 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/fasta.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4437 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/fasta.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      184 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/fastq.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4726 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/fastq.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      183 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/genbank.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6035 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/genbank.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       84 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/header.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      919 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/header.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      150 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/ngsfilter.pxd
--rw-r--r--   0 mercierc (520622000) domain users (520600513)     2538 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/ngsfilter.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      150 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/tab.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2831 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/tab.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      186 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/universal.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5600 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/parsers/universal.pyx
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.583341 OBITools3-3.0.1b8/python/obitools3/uri/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        4 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/uri/__init__.py
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      336 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/uri/decode.pxd
--rw-r--r--   0 mercierc (520622000) domain users (520600513)    21387 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/uri/decode.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      831 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/utils.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    11421 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/utils.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       78 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/version.py
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.595339 OBITools3-3.0.1b8/python/obitools3/writers/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/writers/__init__.py
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      189 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/writers/fasta.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      924 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/writers/fasta.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      186 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/writers/fastq.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      986 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/writers/fastq.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      184 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/writers/tab.pxd
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1050 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/python/obitools3/writers/tab.pyx
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      107 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/requirements.txt
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.595339 OBITools3-3.0.1b8/scripts/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1860 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/scripts/obi
--rw-r--r--   0 mercierc (520622000) domain users (520600513)       38 2021-05-10 04:23:22.731318 OBITools3-3.0.1b8/setup.cfg
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5491 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/setup.py
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.703322 OBITools3-3.0.1b8/src/
--rw-r--r--   0 mercierc (520622000) domain users (520600513)     1804 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/CMakeLists.txt
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    14989 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/_sse.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2124 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/array_indexer.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1728 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/array_indexer.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5916 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/bloom.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6084 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/bloom.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    31089 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/build_reference_db.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2390 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/build_reference_db.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1573 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/char_str_indexer.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2226 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/char_str_indexer.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    10648 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/crc64.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      280 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/crc64.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2583 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/dna_seq_indexer.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2185 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/dna_seq_indexer.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     8083 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/encode.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6428 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/encode.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3933 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/hashtable.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2974 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/hashtable.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    18073 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/kmer_similarity.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5985 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/kmer_similarity.h
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.711321 OBITools3-3.0.1b8/src/libecoPCR/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      704 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/ecoError.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1579 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/ecoMalloc.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2672 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/ecoPCR.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4945 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/ecoapat.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2847 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/ecodna.c
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.719319 OBITools3-3.0.1b8/src/libecoPCR/libapat/
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.723319 OBITools3-3.0.1b8/src/libecoPCR/libapat/CODES/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      808 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/libapat/CODES/dft_code.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3595 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/libapat/CODES/dna_code.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2454 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/libapat/CODES/prot_code.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2142 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/libapat/Gmach.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2864 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/libapat/Gtypes.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     7506 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/libapat/apat.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     8994 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/libapat/apat_parse.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    10574 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/libapat/apat_search.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    10808 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/libapat/libstki.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4244 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/libapat/libstki.h
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.723319 OBITools3-3.0.1b8/src/libecoPCR/libthermo/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    21993 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/libthermo/nnparams.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1672 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libecoPCR/libthermo/nnparams.h
-drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-05-10 04:23:22.731318 OBITools3-3.0.1b8/src/libjson/
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    73193 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libjson/cJSON.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    14566 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libjson/cJSON.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     7876 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libjson/json_utils.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2231 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/libjson/json_utils.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2974 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/linked_list.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3287 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/linked_list.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1351 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/murmurhash2.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      214 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/murmurhash2.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    20680 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obi_clean.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3458 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obi_clean.h
--rw-r--r--   0 mercierc (520622000) domain users (520600513)    40257 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obi_ecopcr.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5866 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obi_ecopcr.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    24853 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obi_ecotag.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3135 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obi_ecotag.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    37348 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obi_lcs.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     8552 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obi_lcs.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    67056 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obiavl.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    18321 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obiavl.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2377 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obiblob.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3081 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obiblob.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1770 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obiblob_indexer.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5564 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obiblob_indexer.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      871 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidebug.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    49586 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidms.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    18958 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidms.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)   106642 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidms_taxonomy.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    16339 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidms_taxonomy.h
--rw-r--r--   0 mercierc (520622000) domain users (520600513)    81581 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    23527 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2105 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_array.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2223 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_array.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1554 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_blob.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2173 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_blob.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2058 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_bool.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3676 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_bool.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2058 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_char.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3676 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_char.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2075 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_float.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3696 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_float.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2031 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_idx.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5031 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_idx.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2039 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_int.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3656 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_int.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5665 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_qual.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     9645 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_qual.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2806 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_seq.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3958 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_seq.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2825 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_str.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3958 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumn_str.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5435 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumndir.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5768 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obidmscolumndir.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      395 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obierrno.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6601 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obierrno.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      638 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obilittlebigman.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1951 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obilittlebigman.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      783 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obisig.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      722 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obisig.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2217 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obitypes.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4924 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obitypes.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)   124725 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obiview.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)   109464 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/obiview.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    34278 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/sse_banded_LCS_alignment.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6454 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/sse_banded_LCS_alignment.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1542 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/uint8_indexer.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2470 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/uint8_indexer.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     9657 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/upperband.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      963 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/upperband.h
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    14965 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/utils.c
--rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6593 2021-05-10 04:17:25.000000 OBITools3-3.0.1b8/src/utils.h
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.516281 OBITools3-3.0.1b9/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      336 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/MANIFEST.in
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)     7509 2021-06-02 03:59:20.512282 OBITools3-3.0.1b9/PKG-INFO
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6445 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/README.md
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.172331 OBITools3-3.0.1b9/python/
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.184330 OBITools3-3.0.1b9/python/OBITools3.egg-info/
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)     7509 2021-06-02 03:59:20.000000 OBITools3-3.0.1b9/python/OBITools3.egg-info/PKG-INFO
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)     8784 2021-06-02 03:59:20.000000 OBITools3-3.0.1b9/python/OBITools3.egg-info/SOURCES.txt
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)        1 2021-06-02 03:59:20.000000 OBITools3-3.0.1b9/python/OBITools3.egg-info/dependency_links.txt
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)       10 2021-06-02 03:59:20.000000 OBITools3-3.0.1b9/python/OBITools3.egg-info/top_level.txt
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.188329 OBITools3-3.0.1b9/python/obitools3/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/__init__.py
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.200327 OBITools3-3.0.1b9/python/obitools3/apps/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/apps/__init__.py
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       82 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/apps/arguments.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1748 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/apps/arguments.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       68 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/apps/command.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1010 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/apps/command.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      313 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/apps/config.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3127 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/apps/config.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       56 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/apps/logging.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1097 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/apps/logging.pyx
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.204327 OBITools3-3.0.1b9/python/obitools3/apps/optiongroups/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    12453 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/apps/optiongroups/__init__.py
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1371 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/apps/progress.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4983 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/apps/progress.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      158 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/apps/temp.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2340 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/apps/temp.pyx
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.256319 OBITools3-3.0.1b9/python/obitools3/commands/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/__init__.py
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     9742 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/addtaxids.pyx
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)      712 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/align.pxd
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)    12645 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/align.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       85 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/alignpairedend.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     9324 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/alignpairedend.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    15453 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/annotate.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4500 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/build_ref_db.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6323 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/cat.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6024 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/clean.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      776 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/clean_dms.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2149 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/count.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     9866 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/ecopcr.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6726 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/ecotag.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2942 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/export.pyx
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)    16944 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/grep.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4213 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/head.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1819 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/history.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    20954 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/import.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1141 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/less.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1095 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/ls.pyx
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)    28351 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/ngsfilter.pyx
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)      977 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/rm.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5862 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/sort.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     9224 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/stats.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4463 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/tail.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    20584 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/test.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      493 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/uniq.pxd
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)    25321 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/commands/uniq.pyx
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.268317 OBITools3-3.0.1b9/python/obitools3/dms/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       43 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/__init__.py
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.284315 OBITools3-3.0.1b9/python/obitools3/dms/capi/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/capi/__init__.py
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1440 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/capi/apat.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      388 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/capi/build_reference_db.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1615 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/capi/kmer_similarity.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      493 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/capi/obiclean.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1584 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/capi/obidms.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2661 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/capi/obidmscolumn.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      952 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/capi/obiecopcr.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      530 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/capi/obiecotag.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      250 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/capi/obierrno.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1989 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/capi/obilcsalign.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2844 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/capi/obitaxonomy.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1308 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/capi/obitypes.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      240 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/capi/obiutils.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    19912 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/capi/obiview.pxd
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.292314 OBITools3-3.0.1b9/python/obitools3/dms/column/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       47 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/__init__.py
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1593 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/column.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    25380 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/column.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      602 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/column_idx.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4821 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/column_idx.pyx
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.316311 OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       86 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/__init__.py
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1209 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/bool.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     7859 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/bool.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      672 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/char.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     8128 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/char.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      675 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/float.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     7957 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/float.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      669 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/int.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     7849 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/int.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      942 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/qual.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    11771 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/qual.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      697 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/seq.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     8896 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/seq.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      697 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/str.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     8955 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/str.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      279 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/dms.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    10855 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/dms.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1208 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/obiseq.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    15643 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/obiseq.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      495 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/object.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2762 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/object.pyx
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.320310 OBITools3-3.0.1b9/python/obitools3/dms/taxo/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      126 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/taxo/__init__.py
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1064 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/taxo/taxo.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    14382 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/taxo/taxo.pyx
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.324309 OBITools3-3.0.1b9/python/obitools3/dms/view/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      176 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/view/__init__.py
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.332308 OBITools3-3.0.1b9/python/obitools3/dms/view/typed_view/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       77 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/view/typed_view/__init__.py
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       96 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/view/typed_view/view_NUC_SEQS.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2600 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/view/typed_view/view_NUC_SEQS.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1876 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/view/view.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    36272 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/dms/view/view.pyx
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.340307 OBITools3-3.0.1b9/python/obitools3/files/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/files/__init__.py
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       96 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/files/linebuffer.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      488 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/files/linebuffer.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      388 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/files/uncompress.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3695 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/files/uncompress.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      115 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/files/universalopener.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      380 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/files/universalopener.pyx
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.348306 OBITools3-3.0.1b9/python/obitools3/format/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/format/__init__.py
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      246 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/format/fasta.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      780 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/format/fasta.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      246 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/format/fastq.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      888 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/format/fastq.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      161 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/format/header.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2808 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/format/header.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      156 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/format/tab.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2341 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/format/tab.pyx
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.380301 OBITools3-3.0.1b9/python/obitools3/libalign/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4988 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/__init__.py
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      232 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/_assemble.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5734 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/_assemble.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2117 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/_dynamic.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     9675 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/_dynamic.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      177 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/_freeendgap.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5467 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/_freeendgap.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      153 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/_freeendgapfm.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      368 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/_freeendgapfm.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      248 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/_nws.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5403 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/_nws.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3801 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/_qsassemble.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3973 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/_qsrassemble.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      247 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/_rassemble.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5422 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/_rassemble.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     8771 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/_solexapairend.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      941 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/apat_pattern.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5813 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/apat_pattern.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1093 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/shifted_ali.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5522 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/shifted_ali.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1369 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/libalign/solexapairend.py
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.404298 OBITools3-3.0.1b9/python/obitools3/parsers/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/__init__.py
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      183 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/embl.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5802 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/embl.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       30 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/embl_genbank_features.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4120 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/embl_genbank_features.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      183 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/fasta.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4437 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/fasta.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      184 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/fastq.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4726 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/fastq.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      183 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/genbank.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6035 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/genbank.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       84 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/header.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      919 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/header.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      150 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/ngsfilter.pxd
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)     2538 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/ngsfilter.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      150 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/tab.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2831 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/tab.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      186 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/universal.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5600 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/parsers/universal.pyx
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.408297 OBITools3-3.0.1b9/python/obitools3/uri/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        4 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/uri/__init__.py
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      336 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/uri/decode.pxd
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)    21450 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/uri/decode.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      839 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/utils.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    11891 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/utils.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)       78 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/version.py
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.416296 OBITools3-3.0.1b9/python/obitools3/writers/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/writers/__init__.py
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      189 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/writers/fasta.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      924 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/writers/fasta.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      186 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/writers/fastq.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      986 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/writers/fastq.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      184 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/writers/tab.pxd
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1050 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/python/obitools3/writers/tab.pyx
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      107 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/requirements.txt
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.416296 OBITools3-3.0.1b9/scripts/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1860 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/scripts/obi
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)       38 2021-06-02 03:59:20.516281 OBITools3-3.0.1b9/setup.cfg
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5491 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/setup.py
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.492285 OBITools3-3.0.1b9/src/
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)     1804 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/CMakeLists.txt
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    14989 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/_sse.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2124 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/array_indexer.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1728 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/array_indexer.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5916 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/bloom.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6084 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/bloom.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    31173 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/build_reference_db.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2390 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/build_reference_db.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1573 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/char_str_indexer.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2226 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/char_str_indexer.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    10648 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/crc64.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      280 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/crc64.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2583 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/dna_seq_indexer.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2185 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/dna_seq_indexer.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     8083 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/encode.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6428 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/encode.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3933 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/hashtable.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2974 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/hashtable.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    18073 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/kmer_similarity.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5985 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/kmer_similarity.h
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.496284 OBITools3-3.0.1b9/src/libecoPCR/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      704 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/ecoError.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1579 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/ecoMalloc.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2672 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/ecoPCR.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4945 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/ecoapat.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2847 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/ecodna.c
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.504283 OBITools3-3.0.1b9/src/libecoPCR/libapat/
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.508282 OBITools3-3.0.1b9/src/libecoPCR/libapat/CODES/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      808 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/libapat/CODES/dft_code.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3595 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/libapat/CODES/dna_code.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2454 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/libapat/CODES/prot_code.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2142 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/libapat/Gmach.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2864 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/libapat/Gtypes.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     7506 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/libapat/apat.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     8994 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/libapat/apat_parse.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    10574 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/libapat/apat_search.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    10808 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/libapat/libstki.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4244 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/libapat/libstki.h
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.508282 OBITools3-3.0.1b9/src/libecoPCR/libthermo/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    21993 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/libthermo/nnparams.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1672 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libecoPCR/libthermo/nnparams.h
+drwxr-xr-x   0 mercierc (520622000) domain users (520600513)        0 2021-06-02 03:59:20.512282 OBITools3-3.0.1b9/src/libjson/
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    73193 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libjson/cJSON.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    14566 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libjson/cJSON.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     7876 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libjson/json_utils.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2231 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/libjson/json_utils.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2974 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/linked_list.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3287 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/linked_list.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1351 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/murmurhash2.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      214 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/murmurhash2.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    20680 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obi_clean.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3458 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obi_clean.h
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)    40257 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obi_ecopcr.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5866 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obi_ecopcr.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    24853 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obi_ecotag.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3135 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obi_ecotag.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    37348 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obi_lcs.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     8552 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obi_lcs.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    67056 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obiavl.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    18321 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obiavl.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2377 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obiblob.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3081 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obiblob.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1770 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obiblob_indexer.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5564 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obiblob_indexer.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      871 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidebug.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    49586 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidms.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    18958 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidms.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)   106642 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidms_taxonomy.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    16339 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidms_taxonomy.h
+-rw-r--r--   0 mercierc (520622000) domain users (520600513)    81581 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    23532 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2105 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_array.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2223 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_array.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1554 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_blob.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2173 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_blob.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2058 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_bool.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3676 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_bool.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2058 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_char.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3676 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_char.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2075 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_float.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3696 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_float.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2031 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_idx.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5031 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_idx.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2039 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_int.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3656 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_int.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5665 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_qual.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     9645 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_qual.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2806 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_seq.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3958 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_seq.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2825 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_str.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     3958 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumn_str.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5435 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumndir.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     5768 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obidmscolumndir.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      395 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obierrno.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6601 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obierrno.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      638 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obilittlebigman.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1951 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obilittlebigman.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      783 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obisig.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      722 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obisig.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2217 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obitypes.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     4924 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obitypes.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)   124725 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obiview.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)   109464 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/obiview.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    34278 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/sse_banded_LCS_alignment.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6454 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/sse_banded_LCS_alignment.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     1542 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/uint8_indexer.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     2470 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/uint8_indexer.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     9657 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/upperband.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)      963 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/upperband.h
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)    14965 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/utils.c
+-rwxr-xr-x   0 mercierc (520622000) domain users (520600513)     6593 2021-06-02 03:44:31.000000 OBITools3-3.0.1b9/src/utils.h
```

### Comparing `OBITools3-3.0.1b8/PKG-INFO` & `OBITools3-3.0.1b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OBITools3
-Version: 3.0.1b8
+Version: 3.0.1b9
 Summary: A package for the management of analyses and data in DNA metabarcoding.
 Home-page: https://metabarcoding.org/obitools3
 Author: Celine Mercier
 Author-email: celine.mercier@metabarcoding.org
 License: CeCILL-V2
 Description: The `OBITools3`: A package for the management of analyses and data in DNA metabarcoding   
         ---------------------------------------------
```

### Comparing `OBITools3-3.0.1b8/README.md` & `OBITools3-3.0.1b9/README.md`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/OBITools3.egg-info/PKG-INFO` & `OBITools3-3.0.1b9/python/OBITools3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OBITools3
-Version: 3.0.1b8
+Version: 3.0.1b9
 Summary: A package for the management of analyses and data in DNA metabarcoding.
 Home-page: https://metabarcoding.org/obitools3
 Author: Celine Mercier
 Author-email: celine.mercier@metabarcoding.org
 License: CeCILL-V2
 Description: The `OBITools3`: A package for the management of analyses and data in DNA metabarcoding   
         ---------------------------------------------
```

### Comparing `OBITools3-3.0.1b8/python/OBITools3.egg-info/SOURCES.txt` & `OBITools3-3.0.1b9/python/OBITools3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/apps/arguments.pyx` & `OBITools3-3.0.1b9/python/obitools3/apps/arguments.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/apps/command.pyx` & `OBITools3-3.0.1b9/python/obitools3/apps/command.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/apps/config.pyx` & `OBITools3-3.0.1b9/python/obitools3/apps/config.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/apps/logging.pyx` & `OBITools3-3.0.1b9/python/obitools3/apps/logging.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/apps/optiongroups/__init__.py` & `OBITools3-3.0.1b9/python/obitools3/apps/optiongroups/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,21 @@
                      const=b'fastq',
                      help="Input file is in fastq format")
 
     group.add_argument('--silva-input',
                      action="store_const", dest="obi:inputformat",
                      default=None,
                      const=b'silva',
-                     help="Input file is in SILVA fasta format")
+                     help="Input file is in SILVA fasta format. If NCBI taxonomy provided with --taxonomy, taxid and scientific name will be added for each sequence.")
+
+    group.add_argument('--rdp-input',
+                     action="store_const", dest="obi:inputformat",
+                     default=None,
+                     const=b'rdp',
+                     help="Input file is in RDP training set fasta format. If NCBI taxonomy provided with --taxonomy, taxid and scientific name will be added for each sequence.")
 
     group.add_argument('--embl-input',
                      action="store_const", dest="obi:inputformat",
                      default=None,
                      const=b'embl',
                      help="Input file is in embl nucleic format")
```

### Comparing `OBITools3-3.0.1b8/python/obitools3/apps/progress.pxd` & `OBITools3-3.0.1b9/python/obitools3/apps/progress.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/apps/progress.pyx` & `OBITools3-3.0.1b9/python/obitools3/apps/progress.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/apps/temp.pyx` & `OBITools3-3.0.1b9/python/obitools3/apps/temp.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/addtaxids.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/addtaxids.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -41,23 +41,23 @@
 
     group.add_argument('-t', '--taxid-tag', 
                        action="store", 
                        dest="addtaxids:taxid_tag",
                        metavar="<TAXID_TAG>",
                        default=b"TAXID",
                        help="Name of the tag to store the found taxid "
-                            "(default: 'TAXID'.")
+                            "(default: 'TAXID').")
 
     group.add_argument('-n', '--taxon-name-tag', 
                        action="store", 
                        dest="addtaxids:taxon_name_tag",
                        metavar="<SCIENTIFIC_NAME_TAG>",
                        default=b"SCIENTIFIC_NAME",
                        help="Name of the tag giving the scientific name of the taxon "
-                            "(default: 'SCIENTIFIC_NAME'.")
+                            "(default: 'SCIENTIFIC_NAME').")
 
     group.add_argument('-g', '--try-genus-match',
                      action="store_true", dest="addtaxids:try_genus_match",
                      default=False,
                      help="Try matching the first word of <SCIENTIFIC_NAME_TAG> when can't find corresponding taxid for a taxon. "
                           "If there is a match it is added in the 'parent_taxid' tag. (Can be used by 'obi taxonomy' to add the taxon under that taxid).")
 
@@ -170,14 +170,15 @@
                 pb(i)
             taxon_name = taxon_name_column[i]
             taxon = taxo.get_taxon_by_name(taxon_name, res_anc)
             if taxon is not None:
                 taxid_column[i] = taxon.taxid
                 found_count+=1
             elif try_genus: # try finding genus or other parent taxon from the first word
+                #print(i, o_view[i].id)
                 taxon_name_sp = taxon_name.split(b" ")
                 taxon = taxo.get_taxon_by_name(taxon_name_sp[0], res_anc)
                 if taxon is not None:
                     parent_taxid_column[i] = taxon.taxid
                     parent_found_count+=1
                     if logfile:
                         print("Found parent taxon for", tostr(taxon_name), file=logfile)
```

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/align.pxd` & `OBITools3-3.0.1b9/python/obitools3/commands/align.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/align.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/align.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         raise Exception("Could not read input")
     i_dms = input[0]
     i_dms_name = input[0].name
     i_uri = input[1]
     i_view_name = i_uri.split(b"/")[0]
     i_column_name = b""
     i_element_name = b""
-    if len(i_uri.split(b"/")) == 2:
+    if len(i_uri.split(b"/")) >= 2:
         i_column_name = i_uri.split(b"/")[1]
     if len(i_uri.split(b"/")) == 3:
         i_element_name = i_uri.split(b"/")[2]
     if len(i_uri.split(b"/")) > 3:
         raise Exception("Input URI contains too many elements:", config['obi']['inputURI'])
 
     # Open the second input if there is one
@@ -177,15 +177,15 @@
                            dms_only=True)
         if input_2 is None:
             raise Exception("Could not read second input")
         i_dms_2 = input_2[0]
         i_dms_name_2 = i_dms_2.name
         i_uri_2 = input_2[1]
         original_i_view_name_2 = i_uri_2.split(b"/")[0]
-        if len(i_uri_2.split(b"/")) == 2:
+        if len(i_uri_2.split(b"/")) >= 2:
             i_column_name_2 = i_uri_2.split(b"/")[1]
         if len(i_uri_2.split(b"/")) == 3:
             i_element_name_2 = i_uri_2.split(b"/")[2]
         if len(i_uri_2.split(b"/")) > 3:
             raise Exception("Input URI contains too many elements:", config['align']['inputuri2'])
 
         # If the 2 input DMS are not the same, temporarily import 2nd input view in first input DMS
```

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/alignpairedend.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/alignpairedend.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/annotate.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/annotate.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/build_ref_db.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/build_ref_db.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,17 @@
     addNoProgressBarOption(parser)
  
     group = parser.add_argument_group('obi build_ref_db specific options')
 
     group.add_argument('--threshold','-t',
                       action="store", dest="build_ref_db:threshold",
                       metavar='<THRESHOLD>',
-                      default=0.0,
+                      default=0.99,
                       type=float,
-                      help="Score threshold as a normalized identity, e.g. 0.95 for an identity of 95%%. Default: 0.00"
-                           " (no threshold).")
+                      help="Score threshold as a normalized identity, e.g. 0.95 for an identity of 95%%. Default: 0.99.")
 
 
 def run(config):
         
     DMS.obi_atexit()
     
     logger("info", "obi build_ref_db")
```

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/cat.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/cat.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 Column.new_column(o_view, NUC_SEQUENCE_COLUMN, OBI_SEQ)
             Column.new_column(o_view, QUALITY_COLUMN, OBI_QUAL, associated_column_name=NUC_SEQUENCE_COLUMN, associated_column_version=o_view[NUC_SEQUENCE_COLUMN].version)    
         if not remove_rev_qual:
             Column.new_column(o_view, REVERSE_SEQUENCE_COLUMN, OBI_SEQ)
             Column.new_column(o_view, REVERSE_QUALITY_COLUMN, OBI_QUAL, associated_column_name=REVERSE_SEQUENCE_COLUMN, associated_column_version=o_view[REVERSE_SEQUENCE_COLUMN].version)
         
     # Initialize multiple elements columns
-    if type(output_0)==BufferedWriter: 
+    if type(output_0)!=BufferedWriter: 
         dict_cols = {}
         for v_uri in config["cat"]["views_to_cat"]:
             v = open_uri(v_uri)[1]
             for coln in v.keys():
                 col = v[coln]
                 if v[coln].nb_elements_per_line > 1:
                     if coln not in dict_cols:
```

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/clean.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/clean.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -50,19 +50,19 @@
  
     group.add_argument('--heads-only', '-H',
                        action="store_true", 
                        dest="clean:heads-only",
                        default=False,
                        help="Only sequences labeled as heads are kept in the output. Default: False")
 
-    group.add_argument('--cluster-tags', '-C',
-                       action="store_true", 
-                       dest="clean:cluster-tags",
-                       default=False,
-                       help="Adds tags for each sequence giving its cluster's head and weight for each sample.")
+#    group.add_argument('--cluster-tags', '-C',
+#                       action="store_true", 
+#                       dest="clean:cluster-tags",
+#                       default=False,
+#                       help="Adds tags for each sequence giving its cluster's head and weight for each sample.")
 
     group.add_argument('--thread-count','-p',   # TODO should probably be in a specific option group
                        action="store", dest="clean:thread-count",
                        metavar='<THREAD COUNT>',
                        default=-1,
                        type=int,
                        help="Number of threads to use for the computation. Default: the maximum available.")
@@ -138,8 +138,9 @@
     # If the input and the output DMS are different or if stdout output, delete the temporary imported view used to create the final view
     if i_dms != o_dms or type(output_0)==BufferedWriter:
         View.delete_view(i_dms, o_view_name)
         o_dms.close(force=True)
     
     i_dms.close(force=True)
 
-    logger("info", "Done.")
+    logger("info", "Done.")
+
```

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/clean_dms.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/clean_dms.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/ecopcr.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/ecopcr.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/ecotag.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/ecotag.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/export.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/export.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/grep.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/grep.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -254,14 +254,21 @@
 
         return good
     
     return filter
 
 
 def Taxonomy_filter_generator(taxo, options):
+    
+    if (("required_ranks" in options and options["required_ranks"]) or \
+       ("required_taxids" in options and options["required_taxids"]) or \
+       ("ignored_taxids" in options and options["ignored_taxids"])) and \
+       (taxo is None):
+        raise RollbackException("obi grep error: can't use taxonomy options without providing a taxonomy. Rollbacking view")
+    
     if taxo is not None:
         def tax_filter(seq):
             good = True
             if b'TAXID' in seq and seq[b'TAXID'] is not None:   # TODO use macro
                 taxid = seq[b'TAXID']
                 if "required_ranks" in options and options["required_ranks"]:
                     taxon_at_rank = reduce(lambda x,y: x and y,
```

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/head.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/head.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/history.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/history.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/import.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/import.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -30,30 +30,34 @@
                                         SCIENTIFIC_NAME_COLUMN
                                         
 from obitools3.dms.capi.obidms cimport obi_import_view
 
 from obitools3.dms.capi.obitypes cimport obitype_t, \
                                          OBI_VOID, \
                                          OBI_QUAL, \
-                                         OBI_STR
+                                         OBI_STR, \
+                                         OBI_INT
 
 from obitools3.dms.capi.obierrno cimport obi_errno
 
 from obitools3.apps.optiongroups import addImportInputOption, \
                                         addTabularInputOption, \
                                         addTaxdumpInputOption, \
-                                        addMinimalOutputOption
+                                        addMinimalOutputOption, \
+                                        addNoProgressBarOption, \
+                                        addTaxonomyOption
 
 from obitools3.uri.decode import open_uri
 
 from obitools3.apps.config import logger
 
 from cpython.exc cimport PyErr_CheckSignals
 
 from io import BufferedWriter
+import ast
 
 
 __title__="Import sequences from different formats into a DMS"
  
  
 default_config = {   'destview'     : None,
                      'skip'         : 0,
@@ -65,15 +69,17 @@
                  }
 
 def addOptions(parser):
     
     addImportInputOption(parser)
     addTabularInputOption(parser)
     addTaxdumpInputOption(parser)
+    addTaxonomyOption(parser)
     addMinimalOutputOption(parser)
+    addNoProgressBarOption(parser)
 
     group = parser.add_argument_group('obi import specific options')
 
     group.add_argument('--preread',
                      action="store_true", dest="import:preread",
                      default=False,
                      help="Do a first readthrough of the dataset if it contains huge dictionaries (more than 100 keys) for "
@@ -81,26 +87,31 @@
 
     group.add_argument('--space-priority',
                      action="store_true", dest="import:space_priority",
                      default=False,
                      help="If importing a view into another DMS, do it by importing each line, saving disk space if the original view "
                           "has a line selection associated.")
 
+#    group.add_argument('--only-id',
+#                     action="store", dest="import:onlyid",
+#                     help="only id")
+
 def run(config):
     
     cdef   tuple       input
     cdef   tuple       output 
     cdef   int         i
     cdef   type        value_type
     cdef   obitype_t   value_obitype
     cdef   obitype_t   old_type
     cdef   obitype_t   new_type
     cdef   bint        get_quality
     cdef   bint        NUC_SEQS_view
     cdef   bint        silva
+    cdef   bint        rdp
     cdef   int         nb_elts
     cdef   object      d
     cdef   View        view
     cdef   object      entries
     cdef   object      entry
     cdef   Column      id_col
     cdef   Column      def_col
@@ -176,50 +187,68 @@
         taxo.write(taxo_name)
         taxo.close()
         o_dms.record_command_line(" ".join(sys.argv[1:]))
         o_dms.close(force=True)
         logger("info", "Done.")
         return
 
+    # Open taxonomy if there is one
+    if 'taxoURI' in config['obi'] and config['obi']['taxoURI'] is not None:
+        taxo_uri = open_uri(config['obi']['taxoURI'])
+        if taxo_uri is None or taxo_uri[2] == bytes:
+            raise Exception("Couldn't open taxonomy")
+        taxo = taxo_uri[1]
+
+    else :
+        taxo = None
+
     # If importing a view between two DMS and not wanting to save space if line selection in original view, use C API
     if isinstance(input[1], View) and not config['import']['space_priority']:
         if obi_import_view(input[0].name_with_full_path, o_dms.name_with_full_path, input[1].name, tobytes((config['obi']['outputURI'].split('/'))[-1])) < 0 :
             input[0].close(force=True)
             output[0].close(force=True)
             raise Exception("Error importing a view in a DMS")
         o_dms.record_command_line(" ".join(sys.argv[1:]))
         input[0].close(force=True)
         output[0].close(force=True)
         logger("info", "Done.")
         return
 
-    if entry_count >= 0:
+    # Reinitialize the progress bar
+    if entry_count >= 0 and config['obi']['noprogressbar'] == False:
         pb = ProgressBar(entry_count, config)
+    else:
+        pb = None
         
     NUC_SEQS_view = False
     if isinstance(output[1], View) :
         view = output[1]
         if output[2] == View_NUC_SEQS :
             NUC_SEQS_view = True
     else: 
         raise NotImplementedError()
-        
+
     # Save basic columns in variables for optimization
     if NUC_SEQS_view :
         id_col = view[ID_COLUMN]
         def_col = view[DEFINITION_COLUMN]
         seq_col = view[NUC_SEQUENCE_COLUMN]
 
-    # Prepare taxon scientific name if SILVA file
-    if 'inputformat' in config['obi'] and config['obi']['inputformat'] == b"silva":
+    # Prepare taxon scientific name and taxid refs if RDP or SILVA file
+    silva = False
+    rdp = False
+    if 'inputformat' in config['obi'] and (config['obi']['inputformat'] == b"silva" or config['obi']['inputformat'] == b"rdp"):
+        #if taxo is None:
+        #    raise Exception("A taxonomy (as built by 'obi import --taxdump') must be provided for SILVA and RDP files")
         silva = True
-        sci_name_col = Column.new_column(view, SCIENTIFIC_NAME_COLUMN, OBI_STR)
-    else:
-        silva = False
-    
+        rdp = True
+        if taxo is not None:
+            sci_name_col = Column.new_column(view, SCIENTIFIC_NAME_COLUMN, OBI_STR)
+            taxid_col = Column.new_column(view, TAXID_COLUMN, OBI_INT)
+
     dcols = {}
 
     # First read through the entries to prepare columns with dictionaries as they are very time-expensive to rewrite
     if config['import']['preread']:
         logger("info", "First readthrough...")
         entries = input[1]
         i = 0
@@ -261,24 +290,34 @@
                               dict_column=True), \
                           dict_dict[tag][1])
     
         
         # Reinitialize the input
         if isinstance(input[0], CompressedFile):
             input_is_file = True
-        if entry_count >= 0:
+        
+        # Reinitialize the progress bar
+        if entry_count >= 0 and config['obi']['noprogressbar'] == False:
             pb = ProgressBar(entry_count, config)
+        else:
+            pb = None
+
         try:
             input[0].close()
         except AttributeError:
             pass
         input = open_uri(config['obi']['inputURI'], force_file=input_is_file)
         if input is None:
             raise Exception("Could not open input URI")
     
+#    if 'onlyid' in config['import']:
+#        onlyid = tobytes(config['import']['onlyid'])
+#    else:
+#        onlyid = None
+    
     entries = input[1]
     i = 0
     for entry in entries :
         
         PyErr_CheckSignals()
 
         if entry is None:  # error or exception handled at lower level, not raised because Python generators can't resume after any exception is raised
@@ -288,14 +327,17 @@
                 raise RollbackException("obi import error, rollbacking view", view)
         
         if pb is not None:
             pb(i)
         elif not i%50000:
             logger("info", "Imported %d entries", i)
         
+#        if onlyid is not None and entry.id != onlyid:
+#            continue
+        
         try:
              
             if NUC_SEQS_view: 
                 id_col[i] = entry.id           
                 def_col[i] = entry.definition
                 seq_col[i] = entry.seq
                 # Check if there is a sequencing quality associated by checking the first entry    # TODO haven't found a more robust solution yet
@@ -303,51 +345,70 @@
                     get_quality = QUALITY_COLUMN in entry
                     if get_quality:
                         Column.new_column(view, QUALITY_COLUMN, OBI_QUAL)
                         qual_col = view[QUALITY_COLUMN]
                 if get_quality:
                     qual_col[i] = entry.quality
                     
-                # Parse taxon scientific name if SILVA file
-                if silva:
-                    sci_name = entry.definition.split(b";")[-1]
-                    sci_name_col[i] = sci_name
-             
+                # Parse taxon scientific name if RDP file
+                if (rdp or silva) and taxo is not None:
+                    sci_names = entry.definition.split(b";")
+                    for sci_name in reversed(sci_names):
+                        if sci_name.split()[0] != b'unidentified' and sci_name.split()[0] != b'uncultured' and sci_name.split()[0] != b'metagenome' :
+                            taxon = taxo.get_taxon_by_name(sci_name)
+                            if taxon is not None:
+                                sci_name_col[i] = taxon.name
+                                taxid_col[i] = taxon.taxid
+                                #print(taxid_col[i], sci_name_col[i])
+                                break
+
             for tag in entry :
                 
                 if tag != ID_COLUMN and tag != DEFINITION_COLUMN and tag != NUC_SEQUENCE_COLUMN and tag != QUALITY_COLUMN :  # TODO dirty 
                                     
                     value = entry[tag]
                     if tag == b"taxid":
                         tag = TAXID_COLUMN
                     if tag == b"count":
                         tag = COUNT_COLUMN
                     if tag[:7] == b"merged_":
                         tag = MERGED_PREFIX+tag[7:]
-                        
+
+                    if type(value) == bytes and value[:1]==b"[" :
+                        try:
+                            if type(eval(value)) == list:
+                                value = eval(value)
+                                #print(value)
+                        except:
+                            pass
+                    
                     if tag not in dcols :
-                         
+                                                
                         value_type = type(value)
                         nb_elts = 1
                         value_obitype = OBI_VOID
                         dict_col = False
-                         
-                        if value_type == dict or value_type == list :
+                        
+                        if value_type == dict :
                             nb_elts = len(value)
                             elt_names = list(value)
-                            if value_type == dict :
-                                dict_col = True
+                            dict_col = True
                         else :
                             nb_elts = 1
                             elt_names = None
-                         
+                        
+                        if value_type == list :
+                            tuples = True
+                        else:
+                            tuples = False
+                        
                         value_obitype = get_obitype(value)
-                         
+                                                
                         if value_obitype != OBI_VOID :
-                            dcols[tag] = (Column.new_column(view, tag, value_obitype, nb_elements_per_line=nb_elts, elements_names=elt_names, dict_column=dict_col), value_obitype)
+                            dcols[tag] = (Column.new_column(view, tag, value_obitype, nb_elements_per_line=nb_elts, elements_names=elt_names, dict_column=dict_col, tuples=tuples), value_obitype)
                                                      
                             # Fill value
                             dcols[tag][0][i] = value
                          
                         # TODO else log error?
      
                     else :
@@ -415,19 +476,20 @@
                                 for t in dcols :
                                     dcols[t] = (view[t], dcols[t][1])
                                  
                                 # Fill value
                                 dcols[tag][0][i] = value
         
         except Exception as e:
-            print("\nCould not import sequence:", entry, "(error raised:", e, ")")
+            print("\nCould not import sequence:", repr(entry), "(error raised:", e, ")")
             if 'skiperror' in config['obi'] and not config['obi']['skiperror']:
                 raise e
             else:
                 pass
+                i-=1  # overwrite problematic entry
         
         i+=1
  
     if pb is not None:
         pb(i, force=True)
         print("", file=sys.stderr)
     logger("info", "Imported %d entries", len(view))
```

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/less.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/less.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/ls.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/ls.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/ngsfilter.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/ngsfilter.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/rm.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/rm.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/sort.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/sort.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/stats.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/stats.pyx`

 * *Files 9% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         taxo_uri = open_uri(config['obi']['taxoURI'])
         if taxo_uri is None or taxo_uri[2] == bytes:
             raise Exception("Couldn't open taxonomy")
         taxo = taxo_uri[1]
     else :
         taxo = None
 
-    statistics = set(config['stats']['minimum']) | set(config['stats']['maximum']) | set(config['stats']['mean'])
+    statistics = set(config['stats']['minimum']) | set(config['stats']['maximum']) | set(config['stats']['mean']) | set(config['stats']['var']) | set(config['stats']['sd'])
     total = 0
     catcount={}
     totcount={}
     values={}
     lcat=0
     
     # Initialize the progress bar
@@ -191,15 +191,15 @@
         category=tuple(category)
         catcount[category]=catcount.get(category,0)+1
         try: 
             totcount[category]=totcount.get(category,0)+line[COUNT_COLUMN]
         except KeyError:
             totcount[category]=totcount.get(category,0)+1
         for var in statistics:
-            if var in line:
+            if var in line and line[var] is not None:
                 v = line[var]
                 if var not in values:
                     values[var]={}
                 if category not in values[var]:
                     values[var][category]=[]
                 values[var][category].append(v)    
 
@@ -234,22 +234,42 @@
         varvar= "%s"
         
     if config['stats']['sd']:
         sdvar= "sd_%%-%ds" % max(len(x) for x in config['stats']['sd'])
     else:
         sdvar= "%s"
         
-    hcat = "\t".join([pcat % x for x in config['stats']['categories']]) + \
-           "\t".join([minvar % x for x in config['stats']['minimum']])  + \
-           "\t".join([maxvar % x for x in config['stats']['maximum']])  + \
-           "\t".join([meanvar % x for x in config['stats']['mean']])  + \
-           "\t".join([varvar % x for x in config['stats']['var']])  + \
-           "\t".join([sdvar % x for x in config['stats']['sd']]) + \
-           "count\t" + \
-           "total" 
+    hcat = ""
+    
+    for x in config['stats']['categories']:
+        hcat += pcat % x
+        hcat += "\t"
+    
+    for x in config['stats']['minimum']:
+        hcat += minvar % x
+        hcat += "\t"
+
+    for x in config['stats']['maximum']:
+        hcat += maxvar % x
+        hcat += "\t"
+
+    for x in config['stats']['mean']:
+        hcat += meanvar % x
+        hcat += "\t"
+    
+    for x in config['stats']['var']:
+        hcat += varvar % x
+        hcat += "\t"
+
+    for x in config['stats']['sd']:
+        hcat += sdvar % x
+        hcat += "\t"
+
+    hcat += "count\ttotal" 
+    
     print(hcat)
     sorted_stats = sorted(catcount.items(), key = lambda kv:(totcount[kv[0]]), reverse=True)
     for i in range(len(sorted_stats)):
         c = sorted_stats[i][0]
         for v in c:
             if type(v) == bytes:
                 print(pcat % tostr(v)+"\t", end="")
```

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/tail.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/tail.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/test.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/test.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/commands/uniq.pyx` & `OBITools3-3.0.1b9/python/obitools3/commands/uniq.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/capi/apat.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/capi/apat.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/capi/kmer_similarity.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/capi/kmer_similarity.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/capi/obidms.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/capi/obidms.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/capi/obidmscolumn.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/capi/obidmscolumn.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/capi/obiecopcr.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/capi/obiecopcr.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/capi/obiecotag.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/capi/obiecotag.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/capi/obilcsalign.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/capi/obilcsalign.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/capi/obitaxonomy.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/capi/obitaxonomy.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/capi/obitypes.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/capi/obitypes.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/capi/obiview.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/capi/obiview.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/column.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/column/column.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/column.pyx` & `OBITools3-3.0.1b9/python/obitools3/dms/column/column.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/column_idx.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/column/column_idx.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/column_idx.pyx` & `OBITools3-3.0.1b9/python/obitools3/dms/column/column_idx.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/bool.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/bool.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/bool.pyx` & `OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/bool.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/char.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/char.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/char.pyx` & `OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/char.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/float.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/float.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/float.pyx` & `OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/float.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/int.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/int.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/int.pyx` & `OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/int.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/qual.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/qual.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/qual.pyx` & `OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/qual.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/seq.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/seq.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/seq.pyx` & `OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/seq.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/str.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/str.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/column/typed_column/str.pyx` & `OBITools3-3.0.1b9/python/obitools3/dms/column/typed_column/str.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/dms.pyx` & `OBITools3-3.0.1b9/python/obitools3/dms/dms.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/obiseq.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/obiseq.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/obiseq.pyx` & `OBITools3-3.0.1b9/python/obitools3/dms/obiseq.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/object.pyx` & `OBITools3-3.0.1b9/python/obitools3/dms/object.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/taxo/taxo.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/taxo/taxo.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/taxo/taxo.pyx` & `OBITools3-3.0.1b9/python/obitools3/dms/taxo/taxo.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/view/typed_view/view_NUC_SEQS.pyx` & `OBITools3-3.0.1b9/python/obitools3/dms/view/typed_view/view_NUC_SEQS.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/view/view.pxd` & `OBITools3-3.0.1b9/python/obitools3/dms/view/view.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/dms/view/view.pyx` & `OBITools3-3.0.1b9/python/obitools3/dms/view/view.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     # TODO try cdef again
     def get_view_class(bytes view_type):
         global __VIEW_CLASS__
         return __VIEW_CLASS__.get(view_type, View) 
  
  
     @staticmethod
-    def import_view(object dms_1, object dms_2, object view_name_1, object view_name_2):
+    def import_view(object dms_1, object dms_2, object view_name_1, object view_name_2): # TODO argument to import line by line to avoid huge AVL copy
         if obi_import_view(tobytes(dms_1), tobytes(dms_2), tobytes(view_name_1), tobytes(view_name_2)) < 0 :
             raise Exception("Error importing a view")
 
 
     @staticmethod
     def delete_view(DMS dms, object view_name):
         if (obi_delete_view(dms.pointer(), tobytes(view_name)) < 0):
```

### Comparing `OBITools3-3.0.1b8/python/obitools3/files/uncompress.pyx` & `OBITools3-3.0.1b9/python/obitools3/files/uncompress.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/format/fasta.pyx` & `OBITools3-3.0.1b9/python/obitools3/format/fasta.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/format/fastq.pyx` & `OBITools3-3.0.1b9/python/obitools3/format/fastq.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/format/header.pyx` & `OBITools3-3.0.1b9/python/obitools3/format/header.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/format/tab.pyx` & `OBITools3-3.0.1b9/python/obitools3/format/tab.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/libalign/__init__.py` & `OBITools3-3.0.1b9/python/obitools3/libalign/__init__.py`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/libalign/_assemble.pyx` & `OBITools3-3.0.1b9/python/obitools3/libalign/_assemble.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/libalign/_dynamic.pxd` & `OBITools3-3.0.1b9/python/obitools3/libalign/_dynamic.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/libalign/_dynamic.pyx` & `OBITools3-3.0.1b9/python/obitools3/libalign/_dynamic.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/libalign/_freeendgap.pyx` & `OBITools3-3.0.1b9/python/obitools3/libalign/_freeendgap.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/libalign/_nws.pyx` & `OBITools3-3.0.1b9/python/obitools3/libalign/_nws.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/libalign/_qsassemble.pyx` & `OBITools3-3.0.1b9/python/obitools3/libalign/_qsassemble.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/libalign/_qsrassemble.pyx` & `OBITools3-3.0.1b9/python/obitools3/libalign/_qsrassemble.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/libalign/_rassemble.pyx` & `OBITools3-3.0.1b9/python/obitools3/libalign/_rassemble.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/libalign/_solexapairend.pyx` & `OBITools3-3.0.1b9/python/obitools3/libalign/_solexapairend.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/libalign/apat_pattern.pxd` & `OBITools3-3.0.1b9/python/obitools3/libalign/apat_pattern.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/libalign/apat_pattern.pyx` & `OBITools3-3.0.1b9/python/obitools3/libalign/apat_pattern.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/libalign/shifted_ali.pxd` & `OBITools3-3.0.1b9/python/obitools3/libalign/shifted_ali.pxd`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/libalign/shifted_ali.pyx` & `OBITools3-3.0.1b9/python/obitools3/libalign/shifted_ali.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/libalign/solexapairend.py` & `OBITools3-3.0.1b9/python/obitools3/libalign/solexapairend.py`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/parsers/embl.pyx` & `OBITools3-3.0.1b9/python/obitools3/parsers/embl.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/parsers/embl_genbank_features.pyx` & `OBITools3-3.0.1b9/python/obitools3/parsers/embl_genbank_features.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/parsers/fasta.pyx` & `OBITools3-3.0.1b9/python/obitools3/parsers/fasta.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/parsers/fastq.pyx` & `OBITools3-3.0.1b9/python/obitools3/parsers/fastq.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/parsers/genbank.pyx` & `OBITools3-3.0.1b9/python/obitools3/parsers/genbank.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/parsers/header.pyx` & `OBITools3-3.0.1b9/python/obitools3/parsers/header.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/parsers/ngsfilter.pyx` & `OBITools3-3.0.1b9/python/obitools3/parsers/ngsfilter.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/parsers/tab.pyx` & `OBITools3-3.0.1b9/python/obitools3/parsers/tab.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/parsers/universal.pyx` & `OBITools3-3.0.1b9/python/obitools3/parsers/universal.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/uri/decode.pyx` & `OBITools3-3.0.1b9/python/obitools3/uri/decode.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     urib = urib.replace(b".obiview", b"")
     urib = urib.replace(b".obicol", b"")
     urib = urib.replace(b"/VIEWS", b"")
     urib = urib.replace(b"TAXONOMY", b"taxonomy")
     
     config = getConfiguration()
     urip = urlparse(urib)
-            
+        
     if 'obi' not in config:
         config['obi']={}
     
     if not force_file and "defaultdms" in config["obi"]:
         default_dms=config["obi"]["defaultdms"]
     else:
         default_dms=None
@@ -205,29 +205,30 @@
         create=(not input) and (not config["obi"]["nocreatedms"])
     except KeyError:
         create=not input
     
     scheme = urip.scheme
     
     error = None
-    
-    if urib != b"-" and \
+        
+    if b'/taxonomy/' in urib or \
+        (urib != b"-" and \
         (scheme==b"dms" or \
          (scheme==b"" and \
           (((not input) and "outputformat" not in config["obi"]) or \
-          (input and "inputformat" not in config["obi"])))):   # TODO maybe not best way
-        
+          (input and "inputformat" not in config["obi"]))))):   # TODO maybe not best way
+                
         if default_dms is not None and b"/" not in urip.path:   # assuming view to open in default DMS (TODO discuss)
             dms=(default_dms, urip.path)
         else:
             dms = open_dms(urip.path, create)
         
         if dms is None and default_dms is not None:
             dms=(default_dms, urip.path)
-
+                
         if dms is not None:
             if dms_only:
                 return (dms[0],
                         dms[1],
                         type(dms[1]),
                         urlunparse(urip),
                         len(dms[0]))
@@ -244,15 +245,15 @@
                                         path=urip.path,
                                         params=urip.params, 
                                         query=urip.query, 
                                         fragment=urip.fragment)
                 
                 if default_dms is None:
                     config["obi"]["defaultdms"]=resource[0]
-                                
+                
                 return (resource[0],
                         resource[1],
                         type(resource[1]),
                         urlunparse(urip),
                         len(resource[1]))
             except Exception as e:
                 global obi_errno
@@ -460,15 +461,15 @@
                 commentchar=tobytes(config["obi"]["commentchar"])
             except KeyError:
                 commentchar=b'#'
 
         if format is not None:
             if seqtype==b"nuc":
                 objclass = Nuc_Seq    # Nuc_Seq_Stored? TODO
-                if format==b"fasta" or format==b"silva":
+                if format==b"fasta" or format==b"silva" or format==b"rdp":
                     if input:
                         iseq = fastaNucIterator(file, 
                                                 skip=skip, 
                                                 only=only,
                                                 nastring=nastring)
                     else:
                         iseq = FastaNucWriter(FastaFormat(printNAKeys=printna, NAString=nastring),
```

### Comparing `OBITools3-3.0.1b8/python/obitools3/utils.pxd` & `OBITools3-3.0.1b9/python/obitools3/utils.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 cdef object bytes2str_object(object value)
 cdef object str2bytes_object(object value)
 
 cdef object clean_empty_values_from_object(object value, exclude=*)
 
 cdef obitype_t get_obitype_single_value(object value)
 cdef obitype_t update_obitype(obitype_t obitype, object new_value)
-cdef obitype_t get_obitype_iterable_value(object value)
+cdef obitype_t get_obitype_iterable_value(object value, type t)
 cdef obitype_t get_obitype(object value)
 
 cdef object __etag__(bytes x, bytes nastring=*)
```

### Comparing `OBITools3-3.0.1b8/python/obitools3/utils.pyx` & `OBITools3-3.0.1b9/python/obitools3/utils.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -256,46 +256,59 @@
 
 cdef obitype_t update_obitype(obitype_t obitype, object new_value) :
     
     cdef type new_type
     
     new_type = type(new_value)
     
-    if obitype == OBI_INT :
-        if new_type == float or new_value > OBI_INT_MAX :
-            return OBI_FLOAT
+    #if new_type == NoneType:  # doesn't work because Cython sucks
+    if new_value == None or new_type==list or new_type==dict or new_type==tuple:
+        return obitype
+    
     # TODO BOOL vers INT/FLOAT
-    elif new_type == str or new_type == bytes :
+    if new_type == str or new_type == bytes :
         if obitype == OBI_SEQ and is_a_DNA_seq(tobytes(new_value)) :
             pass
         else :
             return OBI_STR
-    
+    elif obitype == OBI_INT :
+        if new_type == float or new_value > OBI_INT_MAX :
+            return OBI_FLOAT
+        
     return obitype
 
 
-cdef obitype_t get_obitype_iterable_value(object value) :
+cdef obitype_t get_obitype_iterable_value(object value, type t) :
     
     cdef obitype_t value_obitype
     
     value_obitype = OBI_VOID
     
-    for k in value :
-        if value_obitype == OBI_VOID :
-            value_obitype = get_obitype_single_value(value[k])
-        else :
-            value_obitype = update_obitype(value_obitype, value[k])
+    if t == dict:
+        for k in value :
+            if value_obitype == OBI_VOID :
+                value_obitype = get_obitype_single_value(value[k])
+            else :
+                value_obitype = update_obitype(value_obitype, value[k])
+    
+    elif t == list or t == tuple:
+        for v in value :
+            if value_obitype == OBI_VOID :
+                value_obitype = get_obitype_single_value(v)
+            else :
+                value_obitype = update_obitype(value_obitype, v)
     
     return value_obitype
 
 
 cdef obitype_t get_obitype(object value) :
     
-    if type(value) == dict or type(value) == list or type(value) == tuple :
-        return get_obitype_iterable_value(value)
+    t = type(value)
+    if t == dict or t == list or t == tuple :
+        return get_obitype_iterable_value(value, t)
     
     else :
         return get_obitype_single_value(value)
 
 
 __re_int__      = re.compile(b"^[+-]?[0-9]+$")
 __re_float__    = re.compile(b"^[+-]?[0-9]+(\.[0-9]*)?([eE][+-]?[0-9]+)?$")
```

### Comparing `OBITools3-3.0.1b8/python/obitools3/writers/fasta.pyx` & `OBITools3-3.0.1b9/python/obitools3/writers/fasta.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/writers/fastq.pyx` & `OBITools3-3.0.1b9/python/obitools3/writers/fastq.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/python/obitools3/writers/tab.pyx` & `OBITools3-3.0.1b9/python/obitools3/writers/tab.pyx`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/scripts/obi` & `OBITools3-3.0.1b9/scripts/obi`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/setup.py` & `OBITools3-3.0.1b9/setup.py`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/CMakeLists.txt` & `OBITools3-3.0.1b9/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/_sse.h` & `OBITools3-3.0.1b9/src/_sse.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/array_indexer.c` & `OBITools3-3.0.1b9/src/array_indexer.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/array_indexer.h` & `OBITools3-3.0.1b9/src/array_indexer.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/bloom.c` & `OBITools3-3.0.1b9/src/bloom.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/bloom.h` & `OBITools3-3.0.1b9/src/bloom.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/build_reference_db.c` & `OBITools3-3.0.1b9/src/build_reference_db.c`

 * *Files 1% similar despite different names*

```diff
@@ -859,15 +859,16 @@
 				return -1;
 			}
 		}
 	}
 	fprintf(stderr,"\rDone : 100 %%           \n");
 
 	// Add information about the threshold used to build the DB
-	snprintf(threshold_str, 5, "%f", threshold);
+#define snprintf_nowarn(...) (snprintf(__VA_ARGS__) < 0 ? abort() : (void)0)
+	snprintf_nowarn(threshold_str, 5, "%f", threshold);
 
 	new_comments = obi_add_comment((o_view->infos)->comments, DB_THRESHOLD_KEY_IN_COMMENTS, threshold_str);
 	if (new_comments == NULL)
 	{
 		obidebug(1, "\nError adding a comment (db threshold) to a view, key: %s, value: %s", DB_THRESHOLD_KEY_IN_COMMENTS, threshold_str);
 		return -1;
 	}
```

### Comparing `OBITools3-3.0.1b8/src/build_reference_db.h` & `OBITools3-3.0.1b9/src/build_reference_db.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/char_str_indexer.c` & `OBITools3-3.0.1b9/src/char_str_indexer.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/char_str_indexer.h` & `OBITools3-3.0.1b9/src/char_str_indexer.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/crc64.c` & `OBITools3-3.0.1b9/src/crc64.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/dna_seq_indexer.c` & `OBITools3-3.0.1b9/src/dna_seq_indexer.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/dna_seq_indexer.h` & `OBITools3-3.0.1b9/src/dna_seq_indexer.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/encode.c` & `OBITools3-3.0.1b9/src/encode.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/encode.h` & `OBITools3-3.0.1b9/src/encode.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/hashtable.c` & `OBITools3-3.0.1b9/src/hashtable.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/hashtable.h` & `OBITools3-3.0.1b9/src/hashtable.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/kmer_similarity.c` & `OBITools3-3.0.1b9/src/kmer_similarity.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/kmer_similarity.h` & `OBITools3-3.0.1b9/src/kmer_similarity.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/ecoError.c` & `OBITools3-3.0.1b9/src/libecoPCR/ecoError.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/ecoMalloc.c` & `OBITools3-3.0.1b9/src/libecoPCR/ecoMalloc.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/ecoPCR.h` & `OBITools3-3.0.1b9/src/libecoPCR/ecoPCR.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/ecoapat.c` & `OBITools3-3.0.1b9/src/libecoPCR/ecoapat.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/ecodna.c` & `OBITools3-3.0.1b9/src/libecoPCR/ecodna.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/libapat/CODES/dft_code.h` & `OBITools3-3.0.1b9/src/libecoPCR/libapat/CODES/dft_code.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/libapat/CODES/dna_code.h` & `OBITools3-3.0.1b9/src/libecoPCR/libapat/CODES/dna_code.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/libapat/CODES/prot_code.h` & `OBITools3-3.0.1b9/src/libecoPCR/libapat/CODES/prot_code.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/libapat/Gmach.h` & `OBITools3-3.0.1b9/src/libecoPCR/libapat/Gmach.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/libapat/Gtypes.h` & `OBITools3-3.0.1b9/src/libecoPCR/libapat/Gtypes.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/libapat/apat.h` & `OBITools3-3.0.1b9/src/libecoPCR/libapat/apat.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/libapat/apat_parse.c` & `OBITools3-3.0.1b9/src/libecoPCR/libapat/apat_parse.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/libapat/apat_search.c` & `OBITools3-3.0.1b9/src/libecoPCR/libapat/apat_search.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/libapat/libstki.c` & `OBITools3-3.0.1b9/src/libecoPCR/libapat/libstki.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/libapat/libstki.h` & `OBITools3-3.0.1b9/src/libecoPCR/libapat/libstki.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/libthermo/nnparams.c` & `OBITools3-3.0.1b9/src/libecoPCR/libthermo/nnparams.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libecoPCR/libthermo/nnparams.h` & `OBITools3-3.0.1b9/src/libecoPCR/libthermo/nnparams.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libjson/cJSON.c` & `OBITools3-3.0.1b9/src/libjson/cJSON.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libjson/cJSON.h` & `OBITools3-3.0.1b9/src/libjson/cJSON.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libjson/json_utils.c` & `OBITools3-3.0.1b9/src/libjson/json_utils.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/libjson/json_utils.h` & `OBITools3-3.0.1b9/src/libjson/json_utils.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/linked_list.c` & `OBITools3-3.0.1b9/src/linked_list.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/linked_list.h` & `OBITools3-3.0.1b9/src/linked_list.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/murmurhash2.c` & `OBITools3-3.0.1b9/src/murmurhash2.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obi_clean.c` & `OBITools3-3.0.1b9/src/obi_clean.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obi_clean.h` & `OBITools3-3.0.1b9/src/obi_clean.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obi_ecopcr.c` & `OBITools3-3.0.1b9/src/obi_ecopcr.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obi_ecopcr.h` & `OBITools3-3.0.1b9/src/obi_ecopcr.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obi_ecotag.c` & `OBITools3-3.0.1b9/src/obi_ecotag.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obi_ecotag.h` & `OBITools3-3.0.1b9/src/obi_ecotag.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obi_lcs.c` & `OBITools3-3.0.1b9/src/obi_lcs.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obi_lcs.h` & `OBITools3-3.0.1b9/src/obi_lcs.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obiavl.c` & `OBITools3-3.0.1b9/src/obiavl.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obiavl.h` & `OBITools3-3.0.1b9/src/obiavl.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obiblob.c` & `OBITools3-3.0.1b9/src/obiblob.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obiblob.h` & `OBITools3-3.0.1b9/src/obiblob.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obiblob_indexer.c` & `OBITools3-3.0.1b9/src/obiblob_indexer.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obiblob_indexer.h` & `OBITools3-3.0.1b9/src/obiblob_indexer.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidebug.h` & `OBITools3-3.0.1b9/src/obidebug.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidms.c` & `OBITools3-3.0.1b9/src/obidms.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidms.h` & `OBITools3-3.0.1b9/src/obidms.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidms_taxonomy.c` & `OBITools3-3.0.1b9/src/obidms_taxonomy.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidms_taxonomy.h` & `OBITools3-3.0.1b9/src/obidms_taxonomy.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn.c` & `OBITools3-3.0.1b9/src/obidmscolumn.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn.h` & `OBITools3-3.0.1b9/src/obidmscolumn.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 #define ELEMENTS_NAMES_MAX (1000000)     	  	/**< The maximum length of the list of elements names.	// TODO Discuss
                                 	       	   	 */
 #define NB_ELTS_MAX_IF_DEFAULT_NAME (1000000) 	/**< The maximum number of elements per line if the default element names
 										   	   	 *   are used ("0\01\02\0...\0n"), considering ELEMENTS_NAMES_MAX.  // TODO not up to date
 										   	   	 */
 #define COLUMN_GROWTH_FACTOR (2)	 	  		/**< The growth factor when a column is enlarged.
                                 	   	   	   	 */
-#define MAXIMUM_LINE_COUNT (1000000000)   		/**< The maximum line count for the data of a column (1E9). //TODO
+#define MAXIMUM_LINE_COUNT (1000000000000)      /**< The maximum line count for the data of a column (1E12). //TODO
                                 	       	   	 */
 #define COMMENTS_MAX_LENGTH (4096)        		/**< The maximum length for comments.
  	 	 	 	 	 	 	 	 	       	   	 */
 #define FORMATTED_ELT_NAMES_SEPARATOR '\0'		/**< The separator between elements names once formatted to be stored in columns.
  	 	 	 	 	 	 	 	 	       	   	 */
 #define NOT_FORMATTED_ELT_NAMES_SEPARATOR ';'   /**< The separator between elements names before being formatted to be stored in columns (e.g. as sent by the upper layer).
  	 	 	 	 	 	 	 	 	 	 	 	 */
```

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_array.c` & `OBITools3-3.0.1b9/src/obidmscolumn_array.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_array.h` & `OBITools3-3.0.1b9/src/obidmscolumn_array.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_blob.c` & `OBITools3-3.0.1b9/src/obidmscolumn_blob.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_blob.h` & `OBITools3-3.0.1b9/src/obidmscolumn_blob.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_bool.c` & `OBITools3-3.0.1b9/src/obidmscolumn_bool.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_bool.h` & `OBITools3-3.0.1b9/src/obidmscolumn_bool.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_char.c` & `OBITools3-3.0.1b9/src/obidmscolumn_char.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_char.h` & `OBITools3-3.0.1b9/src/obidmscolumn_char.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_float.c` & `OBITools3-3.0.1b9/src/obidmscolumn_float.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_float.h` & `OBITools3-3.0.1b9/src/obidmscolumn_float.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_idx.c` & `OBITools3-3.0.1b9/src/obidmscolumn_idx.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_idx.h` & `OBITools3-3.0.1b9/src/obidmscolumn_idx.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_int.c` & `OBITools3-3.0.1b9/src/obidmscolumn_int.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_int.h` & `OBITools3-3.0.1b9/src/obidmscolumn_int.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_qual.c` & `OBITools3-3.0.1b9/src/obidmscolumn_qual.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_qual.h` & `OBITools3-3.0.1b9/src/obidmscolumn_qual.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_seq.c` & `OBITools3-3.0.1b9/src/obidmscolumn_seq.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_seq.h` & `OBITools3-3.0.1b9/src/obidmscolumn_seq.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_str.c` & `OBITools3-3.0.1b9/src/obidmscolumn_str.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumn_str.h` & `OBITools3-3.0.1b9/src/obidmscolumn_str.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumndir.c` & `OBITools3-3.0.1b9/src/obidmscolumndir.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obidmscolumndir.h` & `OBITools3-3.0.1b9/src/obidmscolumndir.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obierrno.h` & `OBITools3-3.0.1b9/src/obierrno.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obilittlebigman.c` & `OBITools3-3.0.1b9/src/obilittlebigman.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obilittlebigman.h` & `OBITools3-3.0.1b9/src/obilittlebigman.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obisig.c` & `OBITools3-3.0.1b9/src/obisig.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obisig.h` & `OBITools3-3.0.1b9/src/obisig.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obitypes.c` & `OBITools3-3.0.1b9/src/obitypes.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obitypes.h` & `OBITools3-3.0.1b9/src/obitypes.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obiview.c` & `OBITools3-3.0.1b9/src/obiview.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/obiview.h` & `OBITools3-3.0.1b9/src/obiview.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/sse_banded_LCS_alignment.c` & `OBITools3-3.0.1b9/src/sse_banded_LCS_alignment.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/sse_banded_LCS_alignment.h` & `OBITools3-3.0.1b9/src/sse_banded_LCS_alignment.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/uint8_indexer.c` & `OBITools3-3.0.1b9/src/uint8_indexer.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/uint8_indexer.h` & `OBITools3-3.0.1b9/src/uint8_indexer.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/upperband.c` & `OBITools3-3.0.1b9/src/upperband.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/upperband.h` & `OBITools3-3.0.1b9/src/upperband.h`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/utils.c` & `OBITools3-3.0.1b9/src/utils.c`

 * *Files identical despite different names*

### Comparing `OBITools3-3.0.1b8/src/utils.h` & `OBITools3-3.0.1b9/src/utils.h`

 * *Files identical despite different names*

