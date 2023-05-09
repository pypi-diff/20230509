# Comparing `tmp/pear_ebi-0.1.61.tar.gz` & `tmp/pear_ebi-0.1.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pear_ebi-0.1.61.tar", last modified: Tue Apr 25 16:25:10 2023, max compression
+gzip compressed data, was "pear_ebi-0.1.62.tar", last modified: Tue May  9 17:10:21 2023, max compression
```

## Comparing `pear_ebi-0.1.61.tar` & `pear_ebi-0.1.62.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-25 16:25:10.240580 pear_ebi-0.1.61/
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1120 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/LICENSE.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)       93 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/MANIFEST.in
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5309 2023-04-25 16:25:10.250580 pear_ebi-0.1.61/PKG-INFO
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5052 2023-03-22 14:38:42.000000 pear_ebi-0.1.61/README.md
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-25 16:25:10.010572 pear_ebi-0.1.61/pear_ebi/
--rw-r--r--   0 andrear   (1000) andrear   (1000)      349 2023-04-25 16:24:59.000000 pear_ebi-0.1.61/pear_ebi/__init__.py
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)    18447 2023-04-05 18:11:56.000000 pear_ebi-0.1.61/pear_ebi/__main__.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-25 16:25:10.010572 pear_ebi-0.1.61/pear_ebi/calculate_distances/
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-25 16:25:10.230579 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/
--rw-r--r--   0 andrear   (1000) andrear   (1000)       36 2023-02-14 10:37:26.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/AUTHORS
--rw-r--r--   0 andrear   (1000) andrear   (1000)    18337 2023-02-20 10:02:47.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/COPYING
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:26.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/ChangeLog
--rw-r--r--   0 andrear   (1000) andrear   (1000)     9732 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/INSTALL
--rw-r--r--   0 andrear   (1000) andrear   (1000)    20283 2023-02-20 10:02:47.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/Makefile
--rw-r--r--   0 andrear   (1000) andrear   (1000)      490 2023-02-14 10:37:26.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/Makefile.am
--rw-r--r--   0 andrear   (1000) andrear   (1000)    20957 2023-02-20 10:02:47.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/Makefile.in
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:26.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/NEWS
--rw-r--r--   0 andrear   (1000) andrear   (1000)      157 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/README
--rw-r--r--   0 andrear   (1000) andrear   (1000)    50999 2023-02-14 10:37:26.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/Random.cpp
--rw-r--r--   0 andrear   (1000) andrear   (1000)  3230664 2023-02-14 10:37:26.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/Random.o
--rw-r--r--   0 andrear   (1000) andrear   (1000)    33526 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/aclocal.m4
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2366 2023-02-14 10:37:26.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/config.h
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2148 2023-02-14 10:37:26.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/config.h.in
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2271 2023-02-14 10:37:26.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/config.hh
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2073 2023-02-14 10:37:26.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/config.hh.in
--rw-r--r--   0 andrear   (1000) andrear   (1000)    16107 2023-02-20 10:02:47.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/config.log
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)    31318 2023-02-20 16:30:29.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/config.status
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)   188210 2023-02-20 16:30:29.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/configure
--rw-r--r--   0 andrear   (1000) andrear   (1000)      485 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/configure.ac
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)   186547 2023-02-20 16:30:29.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/configure.lineno
--rw-r--r--   0 andrear   (1000) andrear   (1000)    16466 2023-02-14 10:37:26.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/depcomp
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2243 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hash.cc
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1915 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hash.hh
--rw-r--r--   0 andrear   (1000) andrear   (1000)   595768 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hash.o
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2968 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hashfunc.cc
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2166 2023-02-20 10:02:48.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hashfunc.hh
--rw-r--r--   0 andrear   (1000) andrear   (1000)   331744 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hashfunc.o
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)  4547960 2023-02-20 16:30:29.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hashrf
--rw-r--r--   0 andrear   (1000) andrear   (1000)    28716 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hashrf.cc
--rw-r--r--   0 andrear   (1000) andrear   (1000)  6651416 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hashrf.o
--rw-r--r--   0 andrear   (1000) andrear   (1000)     9556 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/install-sh
--rw-r--r--   0 andrear   (1000) andrear   (1000)      795 2023-02-20 10:02:47.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/label-map.cc
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1026 2023-02-20 10:02:47.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/label-map.hh
--rw-r--r--   0 andrear   (1000) andrear   (1000)   540936 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/label-map.o
--rw-r--r--   0 andrear   (1000) andrear   (1000)    11374 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/missing
--rw-r--r--   0 andrear   (1000) andrear   (1000)    12315 2023-02-20 10:02:47.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/newick.c
--rw-r--r--   0 andrear   (1000) andrear   (1000)      723 2023-02-20 10:02:47.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/newick.h
--rw-r--r--   0 andrear   (1000) andrear   (1000)    38568 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/newick.o
--rw-r--r--   0 andrear   (1000) andrear   (1000)       24 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/stamp-h1
--rw-r--r--   0 andrear   (1000) andrear   (1000)      660 2023-02-22 10:35:23.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/RF_pypy.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/__init__.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     4810 2023-04-03 16:09:45.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/hashrf.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)    24634 2023-04-03 16:09:45.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/maple_RF.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-25 16:25:10.240580 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/._CMakeFiles
--rw-r--r--   0 andrear   (1000) andrear   (1000)      269 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/._CMakeLists.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/._COPYING
--rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/._COPYING.LESSER
--rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/._CPackConfig.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/._CPackSourceConfig.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/._CTestTestfile.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/._Makefile
--rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/._README
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/._bin
--rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/._cmake_install.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/._icon.ico
--rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/._icon.jpg
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/._tqDist
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/._trees
--rw-r--r--   0 andrear   (1000) andrear   (1000)    15581 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/CMakeCache.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2436 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/CMakeLists.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)    35820 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/COPYING
--rw-r--r--   0 andrear   (1000) andrear   (1000)     7815 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/COPYING.LESSER
--rw-r--r--   0 andrear   (1000) andrear   (1000)     4094 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/CPackConfig.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)     4880 2023-02-14 10:37:27.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/CPackSourceConfig.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)      275 2023-02-20 10:02:48.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/CTestTestfile.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)    12995 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/Makefile
--rw-r--r--   0 andrear   (1000) andrear   (1000)     3071 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/README
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1828 2023-02-14 10:37:28.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/cmake_install.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)    32038 2023-02-14 10:37:28.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/icon.ico
--rw-r--r--   0 andrear   (1000) andrear   (1000)     7953 2023-02-14 10:37:28.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/icon.jpg
--rw-r--r--   0 andrear   (1000) andrear   (1000)      205 2023-02-20 10:02:50.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/install_manifest.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5429 2023-04-03 16:09:45.000000 pear_ebi-0.1.61/pear_ebi/calculate_distances/tqdist.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-25 16:25:10.240580 pear_ebi-0.1.61/pear_ebi/embeddings/
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1790 2023-04-05 18:11:55.000000 pear_ebi-0.1.61/pear_ebi/embeddings/Isomap_e.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1838 2023-04-05 18:11:55.000000 pear_ebi-0.1.61/pear_ebi/embeddings/LLE_e.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1936 2023-04-05 18:11:55.000000 pear_ebi-0.1.61/pear_ebi/embeddings/PCA_e.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.61/pear_ebi/embeddings/__init__.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1473 2023-03-22 16:31:08.000000 pear_ebi-0.1.61/pear_ebi/embeddings/emb_quality.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-25 16:25:10.240580 pear_ebi-0.1.61/pear_ebi/embeddings/graph/
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.61/pear_ebi/embeddings/graph/__init__.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)    39664 2023-04-25 16:24:55.000000 pear_ebi-0.1.61/pear_ebi/embeddings/graph/graph.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2208 2023-04-05 18:11:55.000000 pear_ebi-0.1.61/pear_ebi/embeddings/tSNE_e.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-25 16:25:10.240580 pear_ebi-0.1.61/pear_ebi/interactive_mode/
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.61/pear_ebi/interactive_mode/__init__.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5859 2023-02-22 10:35:24.000000 pear_ebi-0.1.61/pear_ebi/interactive_mode/interactive.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-25 16:25:10.240580 pear_ebi-0.1.61/pear_ebi/subsample/
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.61/pear_ebi/subsample/__init__.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     3855 2023-02-20 16:46:41.000000 pear_ebi-0.1.61/pear_ebi/subsample/subsample.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5050 2023-02-20 16:46:42.000000 pear_ebi-0.1.61/pear_ebi/subsample/subsample_multiprocess.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     3681 2023-04-19 10:09:29.000000 pear_ebi-0.1.61/pear_ebi/tree_emb_parser.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)    33266 2023-04-20 15:17:02.000000 pear_ebi-0.1.61/pear_ebi/tree_set.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-25 16:25:10.010572 pear_ebi-0.1.61/pear_ebi.egg-info/
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5309 2023-04-25 16:25:09.000000 pear_ebi-0.1.61/pear_ebi.egg-info/PKG-INFO
--rw-r--r--   0 andrear   (1000) andrear   (1000)     4297 2023-04-25 16:25:09.000000 pear_ebi-0.1.61/pear_ebi.egg-info/SOURCES.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)        1 2023-04-25 16:25:09.000000 pear_ebi-0.1.61/pear_ebi.egg-info/dependency_links.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)       52 2023-04-25 16:25:09.000000 pear_ebi-0.1.61/pear_ebi.egg-info/entry_points.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-20 16:30:29.000000 pear_ebi-0.1.61/pear_ebi.egg-info/not-zip-safe
--rw-r--r--   0 andrear   (1000) andrear   (1000)       94 2023-04-25 16:25:09.000000 pear_ebi-0.1.61/pear_ebi.egg-info/requires.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)        9 2023-04-25 16:25:09.000000 pear_ebi-0.1.61/pear_ebi.egg-info/top_level.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)      228 2023-02-20 16:30:29.000000 pear_ebi-0.1.61/pyproject.toml
--rw-r--r--   0 andrear   (1000) andrear   (1000)      107 2023-04-25 16:25:10.250580 pear_ebi-0.1.61/setup.cfg
--rw-r--r--   0 andrear   (1000) andrear   (1000)      946 2023-04-25 16:25:02.000000 pear_ebi-0.1.61/setup.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-25 16:25:10.240580 pear_ebi-0.1.61/test/
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1191 2023-04-03 16:09:45.000000 pear_ebi-0.1.61/test/test.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-05-09 17:10:21.776494 pear_ebi-0.1.62/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1120 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/LICENSE.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)       93 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/MANIFEST.in
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5801 2023-05-09 17:10:21.776494 pear_ebi-0.1.62/PKG-INFO
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5353 2023-05-09 17:08:05.000000 pear_ebi-0.1.62/README.md
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-05-09 17:10:21.736493 pear_ebi-0.1.62/pear_ebi/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      349 2023-05-09 17:03:46.000000 pear_ebi-0.1.62/pear_ebi/__init__.py
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)    18447 2023-04-05 18:11:56.000000 pear_ebi-0.1.62/pear_ebi/__main__.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-05-09 17:10:21.746493 pear_ebi-0.1.62/pear_ebi/calculate_distances/
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-05-09 17:10:21.776494 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)       36 2023-02-14 10:37:26.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/AUTHORS
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    18337 2023-02-20 10:02:47.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/COPYING
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:26.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/ChangeLog
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     9732 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/INSTALL
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    20283 2023-02-20 10:02:47.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/Makefile
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      490 2023-02-14 10:37:26.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/Makefile.am
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    20957 2023-02-20 10:02:47.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/Makefile.in
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:26.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/NEWS
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      157 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/README
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    50999 2023-02-14 10:37:26.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/Random.cpp
+-rw-r--r--   0 andrear   (1000) andrear   (1000)  3230664 2023-02-14 10:37:26.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/Random.o
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    33526 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/aclocal.m4
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2366 2023-02-14 10:37:26.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/config.h
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2148 2023-02-14 10:37:26.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/config.h.in
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2271 2023-02-14 10:37:26.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/config.hh
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2073 2023-02-14 10:37:26.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/config.hh.in
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    16107 2023-02-20 10:02:47.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/config.log
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)    31318 2023-02-20 16:30:29.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/config.status
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)   188210 2023-02-20 16:30:29.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/configure
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      485 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/configure.ac
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)   186547 2023-02-20 16:30:29.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/configure.lineno
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    16466 2023-02-14 10:37:26.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/depcomp
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2243 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hash.cc
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1915 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hash.hh
+-rw-r--r--   0 andrear   (1000) andrear   (1000)   595768 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hash.o
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2968 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hashfunc.cc
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2166 2023-02-20 10:02:48.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hashfunc.hh
+-rw-r--r--   0 andrear   (1000) andrear   (1000)   331744 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hashfunc.o
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)  4547960 2023-02-20 16:30:29.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hashrf
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    28716 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hashrf.cc
+-rw-r--r--   0 andrear   (1000) andrear   (1000)  6651416 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hashrf.o
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     9556 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/install-sh
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      795 2023-02-20 10:02:47.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/label-map.cc
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1026 2023-02-20 10:02:47.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/label-map.hh
+-rw-r--r--   0 andrear   (1000) andrear   (1000)   540936 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/label-map.o
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    11374 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/missing
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    12315 2023-02-20 10:02:47.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/newick.c
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      723 2023-02-20 10:02:47.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/newick.h
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    38568 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/newick.o
+-rw-r--r--   0 andrear   (1000) andrear   (1000)       24 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/stamp-h1
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      660 2023-02-22 10:35:23.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/RF_pypy.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/__init__.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     4810 2023-04-03 16:09:45.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/hashrf.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    24634 2023-04-03 16:09:45.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/maple_RF.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-05-09 17:10:21.776494 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/._CMakeFiles
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      269 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/._CMakeLists.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/._COPYING
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/._COPYING.LESSER
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/._CPackConfig.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/._CPackSourceConfig.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/._CTestTestfile.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/._Makefile
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/._README
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/._bin
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/._cmake_install.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/._icon.ico
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/._icon.jpg
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/._tqDist
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/._trees
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    15581 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/CMakeCache.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2436 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/CMakeLists.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    35820 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/COPYING
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     7815 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/COPYING.LESSER
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     4094 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/CPackConfig.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     4880 2023-02-14 10:37:27.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/CPackSourceConfig.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      275 2023-02-20 10:02:48.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/CTestTestfile.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    12995 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/Makefile
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     3071 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/README
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1828 2023-02-14 10:37:28.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/cmake_install.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    32038 2023-02-14 10:37:28.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/icon.ico
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     7953 2023-02-14 10:37:28.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/icon.jpg
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      205 2023-02-20 10:02:50.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/install_manifest.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5429 2023-04-03 16:09:45.000000 pear_ebi-0.1.62/pear_ebi/calculate_distances/tqdist.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-05-09 17:10:21.776494 pear_ebi-0.1.62/pear_ebi/embeddings/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1790 2023-04-05 18:11:55.000000 pear_ebi-0.1.62/pear_ebi/embeddings/Isomap_e.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1838 2023-04-05 18:11:55.000000 pear_ebi-0.1.62/pear_ebi/embeddings/LLE_e.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1936 2023-04-05 18:11:55.000000 pear_ebi-0.1.62/pear_ebi/embeddings/PCA_e.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.62/pear_ebi/embeddings/__init__.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1473 2023-03-22 16:31:08.000000 pear_ebi-0.1.62/pear_ebi/embeddings/emb_quality.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-05-09 17:10:21.776494 pear_ebi-0.1.62/pear_ebi/embeddings/graph/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.62/pear_ebi/embeddings/graph/__init__.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    39664 2023-05-09 14:17:50.000000 pear_ebi-0.1.62/pear_ebi/embeddings/graph/graph.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2208 2023-04-05 18:11:55.000000 pear_ebi-0.1.62/pear_ebi/embeddings/tSNE_e.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-05-09 17:10:21.776494 pear_ebi-0.1.62/pear_ebi/interactive_mode/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.62/pear_ebi/interactive_mode/__init__.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5859 2023-02-22 10:35:24.000000 pear_ebi-0.1.62/pear_ebi/interactive_mode/interactive.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-05-09 17:10:21.776494 pear_ebi-0.1.62/pear_ebi/subsample/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.62/pear_ebi/subsample/__init__.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     3855 2023-02-20 16:46:41.000000 pear_ebi-0.1.62/pear_ebi/subsample/subsample.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5050 2023-02-20 16:46:42.000000 pear_ebi-0.1.62/pear_ebi/subsample/subsample_multiprocess.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     3681 2023-04-19 10:09:29.000000 pear_ebi-0.1.62/pear_ebi/tree_emb_parser.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    33264 2023-05-09 14:17:50.000000 pear_ebi-0.1.62/pear_ebi/tree_set.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-05-09 17:10:21.746493 pear_ebi-0.1.62/pear_ebi.egg-info/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5801 2023-05-09 17:10:21.000000 pear_ebi-0.1.62/pear_ebi.egg-info/PKG-INFO
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     4297 2023-05-09 17:10:21.000000 pear_ebi-0.1.62/pear_ebi.egg-info/SOURCES.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        1 2023-05-09 17:10:21.000000 pear_ebi-0.1.62/pear_ebi.egg-info/dependency_links.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)       52 2023-05-09 17:10:21.000000 pear_ebi-0.1.62/pear_ebi.egg-info/entry_points.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-20 16:30:29.000000 pear_ebi-0.1.62/pear_ebi.egg-info/not-zip-safe
+-rw-r--r--   0 andrear   (1000) andrear   (1000)       94 2023-05-09 17:10:21.000000 pear_ebi-0.1.62/pear_ebi.egg-info/requires.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        9 2023-05-09 17:10:21.000000 pear_ebi-0.1.62/pear_ebi.egg-info/top_level.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      228 2023-02-20 16:30:29.000000 pear_ebi-0.1.62/pyproject.toml
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      107 2023-05-09 17:10:21.786494 pear_ebi-0.1.62/setup.cfg
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1382 2023-05-09 17:10:01.000000 pear_ebi-0.1.62/setup.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-05-09 17:10:21.776494 pear_ebi-0.1.62/test/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1191 2023-04-03 16:09:45.000000 pear_ebi-0.1.62/test/test.py
```

### Comparing `pear_ebi-0.1.61/LICENSE.txt` & `pear_ebi-0.1.62/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/PKG-INFO` & `pear_ebi-0.1.62/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,84 +1,76 @@
-Metadata-Version: 2.1
-Name: pear_ebi
-Version: 0.1.61
-Summary: Embeds phylogenetic tree distances and produce representations
-Home-page: https://github.com/AndreaRubbi/TreeEmbedding
-Author: Andrea Rubbi
-Author-email: andrea.rubbi.98@gmail.com
-License: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-
- <h1> <font color='green'>P</font>hylogeny <font color='green'>E</font>mbedding  & <br>  <font color='green'>A</font>pproximate <font color='green'>R</font>epresentation </h1>
- <img src="logos/LOGO_PEAR.png" width="100" height="100" style='position:absolute; left:400px; top:-15px' >
-
-## Goldman Group - European Bioinformatics Institute <img src="logos/goldman_logo.png" width="30" height="30">
-
-PEAR can:
-1. Compute the distance matrix given a set of phylogenetic trees;
-2. Embed and represent the distance matrix in 2D or 3D.
-
-See also the <a href="https://andrearubbi.github.io/Pear-EBI/index.html"> autogenerated documentation </a> and <a href="https://pypi.org/project/pear-ebi/"> PyPI </a>.
-
-PEAR usage
-==========
-Pear is both a python software and library. It can be installed with `python -m pip install pear_ebi` or downloaded from <a href="https://github.com/AndreaRubbi/Pear-EBI">Github</a>. Pear is currently compatible with Linux and Mac OSs.
-
-PEAR as a python library
-------------------------
-Once installed, Pear can be used to upload newick trees in python and represent them in embedded spaces. We recommend to use it on either jupyter notebook or lab, as these tools allow for more interaction with the graphs. On these platforms, the user is allowed to interact with widgets that allows to modify several parameteres of the plots. For specific uses and applications, see the <a href='https://github.com/AndreaRubbi/Pear-EBI/tree/pear_ebi/examples_tree_sets'>examples</a>.
-
-PEAR as a program
------------------
-Run `pear_ebi --help` to see the complete list of arguments and flags.
-### Simple usage
-
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf`
-
-this script calculates the unweighted <a href='https://doi.org/10.1016/0025-5564(81)90043-2'>Robison Foulds</a> distances between the trees in the file "beast_run1.trees", which contains 1001 phylogenetic trees.
-
-the flag *-m* indicates the method used to compute the dissimilarity between phylogeneic trees. In this case, [HasRF](https://code.google.com/archive/p/hashrf/) has been used.
-
-To embed these distances in a lower-dimensional space, we can use PCoA (MDS) or tSNE:
-
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf -pca 2`
-
-we therefore embedded the distance matrix in 2 dimensions. Using the flag *-quality* one can assess the correlation between the distances in the N-dimensional space and in the embedding; while *-report* computes more insightful metrics such as the trustworthiness and continuity of the embedding.
-
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf -pca 2 -plot --show`
-
-The flags *-plot* and *--show* indicate that PEAR has to plot the embeddings and show them, respectively. *-plot* doesn't require any indication on the number of dimensions as it plots the embeddings in 2 dimensions if the distances are embedded in 2 dimensions, while it plots on 2 and 3 dimensions in any other case.
-
-One can specify any number of files containing trees. Moreover, it is possible to specify a directory using *-dir*, and possibly a pattern using *-pattern*, in order to select multiple files.
-
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -subset 100` shows the 3D and 2D embedding of a subset of 100 trees from the original collection.
-
-#### Tree Set
-
-It's possible to compute the distance matrix and re-use it in future runs of PEAR by specifying the distance matrix file with the flag *-d*. Additionally, it's possible to define the name of the output file (*-o*).
-
-If any additional metadata is available, this may be specified by indicating a *.csv* file containing a dataframe of compatible shape.
-
-### Config file
-A standard config toml file can be used for specific emebddings of multiple sets of trees. Instances of toml files are reported in the <a href='https://github.com/AndreaRubbi/Pear-EBI/tree/pear_ebi/examples_tree_sets'>examples</a> folder.
-
-Using the config file allows one to use all the features of PEAR, including additional embedding methods and plot designs. The config file can also be used to specify lists of indexes of interesting trees in the sets, in order to highlight them in the final plots.
-
-### Interactive mode
-`pear_ebi --i` :
-this script launches the program in the interactive mode. Once the program starts, it is going to guide you through its usage thanks to an intuitive interface.
-
-
-### Additional Dependencies
-In order to get the complete report on the quality of embeddings, it may be necessary to run the following command to install additional dependencies:
-
-`sudo apt-get install '^libxcb.*-dev' libx11-xcb-dev libglu1-mesa-dev libxrender-dev libxi-dev libxkbcommon-dev libxkbcommon-x11-dev`
-
-It may be necessary to also install `libgcc` and remove old versions of `libstdc++` from the interpreter libraries.
-________________________
-
-## Licensing
-
-This project is released under the terms of the MIT Open Source License. View
-*LICENSE.txt* for more information.
+
+ <h1> <font color='green'>P</font>hylogeny <font color='green'>E</font>mbedding  & <br>  <font color='green'>A</font>pproximate <font color='green'>R</font>epresentation </h1>
+ <img src="https://github.com/AndreaRubbi/Pear-EBI/raw/pear_ebi/logos/LOGO_PEAR.png" width="100" height="100" style='position:absolute; left:400px; top:-15px' >
+
+ <img src="https://img.shields.io/github/license/AndreaRubbi/Pear-EBI?color=red&label=License&style=plastic"> <img src="https://img.shields.io/pypi/v/pear_ebi?color=purple&label=version&style=plastic"> <img src="https://img.shields.io/pypi/implementation/pear_ebi?style=plastic"> <img src="https://img.shields.io/pypi/pyversions/pear_ebi?color=green&style=plastic">
+
+
+
+## Goldman Group - European Bioinformatics Institute <img src="https://github.com/AndreaRubbi/Pear-EBI/raw/pear_ebi/logos/goldman_logo.png" width="30" height="30">
+
+PEAR can:
+1. Compute the distance matrix given a set of phylogenetic trees;
+2. Embed and represent the distance matrix in 2D or 3D.
+
+See also the <a href="https://andrearubbi.github.io/Pear-EBI/index.html"> autogenerated documentation </a> and <a href="https://pypi.org/project/pear-ebi/"> PyPI </a>.
+
+PEAR usage
+==========
+Pear is both a python software and library. It can be installed with `python -m pip install pear_ebi` or downloaded from <a href="https://github.com/AndreaRubbi/Pear-EBI">Github</a>. Pear is currently compatible with Linux and Mac OSs.
+
+PEAR as a python library
+------------------------
+Once installed, Pear can be used to upload newick trees in python and represent them in embedded spaces. We recommend to use it on either jupyter notebook or lab, as these tools allow for more interaction with the graphs. On these platforms, the user is allowed to interact with widgets that allows to modify several parameteres of the plots. For specific uses and applications, see the <a href='https://github.com/AndreaRubbi/Pear-EBI/tree/pear_ebi/examples_tree_sets'>examples</a>.
+
+PEAR as a program
+-----------------
+Run `pear_ebi --help` to see the complete list of arguments and flags.
+### Simple usage
+
+`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf_RF`
+
+this script calculates the unweighted <a href='https://doi.org/10.1016/0025-5564(81)90043-2'>Robison Foulds</a> distances between the trees in the file "beast_run1.trees", which contains 1001 phylogenetic trees.
+
+the flag *-m* indicates the method used to compute the dissimilarity between phylogeneic trees. In this case, [HasRF](https://code.google.com/archive/p/hashrf/) has been used.
+
+To embed these distances in a lower-dimensional space, we can use PCoA (MDS) or tSNE:
+
+`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf_RF -pca 2`
+
+we therefore embedded the distance matrix in 2 dimensions. Using the flag *-quality* one can assess the correlation between the distances in the N-dimensional space and in the embedding.
+
+`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf_RF -pca 2 -plot`
+
+The flag *-plot* indicates that PEAR has to plot the embeddings and show them, respectively. If an embedding method is specified the plots are produced anyway. Plotting doesn't require any indication on the number of dimensions as the embeddings are represented in 2 dimensions if the distances are embedded in 2 dimensions, while it plots on 2 and 3 dimensions in any other case.
+
+One can specify any number of files containing trees. Moreover, it is possible to specify a single directory using *-dir*, and possibly a pattern using *-pattern*, in order to select multiple files.
+
+#### Tree Set
+
+It's possible to compute the distance matrix and re-use it in subsequent runs of PEAR by specifying the distance matrix file with the flag *-d*. Additionally, it's possible to define the name of the output file (*-o*).
+
+If any additional metadata is available, this may be specified by indicating a *.csv* file containing a dataframe of compatible shape.
+
+### Config file
+A standard config toml file can be used for specific emebddings of multiple sets of trees. Instances of toml files are reported in the <a href='https://github.com/AndreaRubbi/Pear-EBI/tree/pear_ebi/examples_tree_sets'>examples</a> folder.
+
+Using the config file allows one to use all the features of PEAR, including additional embedding methods and plot designs. The config file can also be used to specify lists of indexes of interesting trees in the sets, in order to highlight them in the final plots.
+
+### Interactive mode
+`pear_ebi --i` :
+this script launches the program in the interactive mode. Once the program starts, it is going to guide you through its usage thanks to an intuitive interface.
+
+
+ <!--- ### Additional Dependencies
+ In order to get the complete report on the quality of embeddings, it may be necessary to
+ run the following command to install additional dependencies:
+
+ `sudo apt-get install '^libxcb.*-dev' libx11-xcb-dev libglu1-mesa-dev libxrender-dev libxi-dev libxkbcommon-dev libxkbcommon-x11-dev`
+
+ It may be necessary to also install `libgcc` and remove old versions of `libstdc++` from the interpreter libraries. --->
+________________________
+
+## Licensing
+
+This project is released under the terms of the MIT Open Source License. View
+*LICENSE.txt* for more information.
```

#### html2text {}

```diff
@@ -1,63 +1,56 @@
-Metadata-Version: 2.1 Name: pear_ebi Version: 0.1.61 Summary: Embeds
-phylogenetic tree distances and produce representations Home-page: https://
-github.com/AndreaRubbi/TreeEmbedding Author: Andrea Rubbi Author-email:
-andrea.rubbi.98@gmail.com License: MIT License Description-Content-Type: text/
-markdown License-File: LICENSE.txt
 ****** Phylogeny Embedding &
 Approximate Representation ******
-[logos/LOGO_PEAR.png] ## Goldman Group - European Bioinformatics Institute
-[logos/goldman_logo.png] PEAR can: 1. Compute the distance matrix given a set
-of phylogenetic trees; 2. Embed and represent the distance matrix in 2D or 3D.
-See also the autogenerated_documentation and PyPI. PEAR usage ========== Pear
-is both a python software and library. It can be installed with `python -m pip
+[https://github.com/AndreaRubbi/Pear-EBI/raw/pear_ebi/logos/LOGO_PEAR.png]
+[https://img.shields.io/github/license/AndreaRubbi/Pear-
+EBI?color=red&label=License&style=plastic] [https://img.shields.io/pypi/v/
+pear_ebi?color=purple&label=version&style=plastic] [https://img.shields.io/
+pypi/implementation/pear_ebi?style=plastic] [https://img.shields.io/pypi/
+pyversions/pear_ebi?color=green&style=plastic] ## Goldman Group - European
+Bioinformatics Institute [https://github.com/AndreaRubbi/Pear-EBI/raw/pear_ebi/
+logos/goldman_logo.png] PEAR can: 1. Compute the distance matrix given a set of
+phylogenetic trees; 2. Embed and represent the distance matrix in 2D or 3D. See
+also the autogenerated_documentation and PyPI. PEAR usage ========== Pear is
+both a python software and library. It can be installed with `python -m pip
 install pear_ebi` or downloaded from Github. Pear is currently compatible with
 Linux and Mac OSs. PEAR as a python library ------------------------ Once
 installed, Pear can be used to upload newick trees in python and represent them
 in embedded spaces. We recommend to use it on either jupyter notebook or lab,
 as these tools allow for more interaction with the graphs. On these platforms,
 the user is allowed to interact with widgets that allows to modify several
 parameteres of the plots. For specific uses and applications, see the examples.
 PEAR as a program ----------------- Run `pear_ebi --help` to see the complete
 list of arguments and flags. ### Simple usage `pear_ebi examples_trees_sets/
-beast_trees/beast_run1.trees -m hashrf` this script calculates the unweighted
-Robison_Foulds distances between the trees in the file "beast_run1.trees",
-which contains 1001 phylogenetic trees. the flag *-m* indicates the method used
-to compute the dissimilarity between phylogeneic trees. In this case, [HasRF]
-(https://code.google.com/archive/p/hashrf/) has been used. To embed these
-distances in a lower-dimensional space, we can use PCoA (MDS) or tSNE:
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf -pca 2` we
-therefore embedded the distance matrix in 2 dimensions. Using the flag *-
-quality* one can assess the correlation between the distances in the N-
-dimensional space and in the embedding; while *-report* computes more
-insightful metrics such as the trustworthiness and continuity of the embedding.
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf -pca 2 -
-plot --show` The flags *-plot* and *--show* indicate that PEAR has to plot the
-embeddings and show them, respectively. *-plot* doesn't require any indication
-on the number of dimensions as it plots the embeddings in 2 dimensions if the
-distances are embedded in 2 dimensions, while it plots on 2 and 3 dimensions in
-any other case. One can specify any number of files containing trees. Moreover,
-it is possible to specify a directory using *-dir*, and possibly a pattern
-using *-pattern*, in order to select multiple files. `pear_ebi
-examples_trees_sets/beast_trees/beast_run1.trees -subset 100` shows the 3D and
-2D embedding of a subset of 100 trees from the original collection. #### Tree
-Set It's possible to compute the distance matrix and re-use it in future runs
-of PEAR by specifying the distance matrix file with the flag *-d*.
-Additionally, it's possible to define the name of the output file (*-o*). If
-any additional metadata is available, this may be specified by indicating a
-*.csv* file containing a dataframe of compatible shape. ### Config file A
-standard config toml file can be used for specific emebddings of multiple sets
-of trees. Instances of toml files are reported in the examples folder. Using
-the config file allows one to use all the features of PEAR, including
-additional embedding methods and plot designs. The config file can also be used
-to specify lists of indexes of interesting trees in the sets, in order to
-highlight them in the final plots. ### Interactive mode `pear_ebi --i` : this
-script launches the program in the interactive mode. Once the program starts,
-it is going to guide you through its usage thanks to an intuitive interface.
-### Additional Dependencies In order to get the complete report on the quality
-of embeddings, it may be necessary to run the following command to install
-additional dependencies: `sudo apt-get install '^libxcb.*-dev' libx11-xcb-dev
-libglu1-mesa-dev libxrender-dev libxi-dev libxkbcommon-dev libxkbcommon-x11-
-dev` It may be necessary to also install `libgcc` and remove old versions of
-`libstdc++` from the interpreter libraries. ________________________ ##
-Licensing This project is released under the terms of the MIT Open Source
-License. View *LICENSE.txt* for more information.
+beast_trees/beast_run1.trees -m hashrf_RF` this script calculates the
+unweighted Robison_Foulds distances between the trees in the file
+"beast_run1.trees", which contains 1001 phylogenetic trees. the flag *-m*
+indicates the method used to compute the dissimilarity between phylogeneic
+trees. In this case, [HasRF](https://code.google.com/archive/p/hashrf/) has
+been used. To embed these distances in a lower-dimensional space, we can use
+PCoA (MDS) or tSNE: `pear_ebi examples_trees_sets/beast_trees/beast_run1.trees
+-m hashrf_RF -pca 2` we therefore embedded the distance matrix in 2 dimensions.
+Using the flag *-quality* one can assess the correlation between the distances
+in the N-dimensional space and in the embedding. `pear_ebi examples_trees_sets/
+beast_trees/beast_run1.trees -m hashrf_RF -pca 2 -plot` The flag *-plot*
+indicates that PEAR has to plot the embeddings and show them, respectively. If
+an embedding method is specified the plots are produced anyway. Plotting
+doesn't require any indication on the number of dimensions as the embeddings
+are represented in 2 dimensions if the distances are embedded in 2 dimensions,
+while it plots on 2 and 3 dimensions in any other case. One can specify any
+number of files containing trees. Moreover, it is possible to specify a single
+directory using *-dir*, and possibly a pattern using *-pattern*, in order to
+select multiple files. #### Tree Set It's possible to compute the distance
+matrix and re-use it in subsequent runs of PEAR by specifying the distance
+matrix file with the flag *-d*. Additionally, it's possible to define the name
+of the output file (*-o*). If any additional metadata is available, this may be
+specified by indicating a *.csv* file containing a dataframe of compatible
+shape. ### Config file A standard config toml file can be used for specific
+emebddings of multiple sets of trees. Instances of toml files are reported in
+the examples folder. Using the config file allows one to use all the features
+of PEAR, including additional embedding methods and plot designs. The config
+file can also be used to specify lists of indexes of interesting trees in the
+sets, in order to highlight them in the final plots. ### Interactive mode
+`pear_ebi --i` : this script launches the program in the interactive mode. Once
+the program starts, it is going to guide you through its usage thanks to an
+intuitive interface.  ________________________ ## Licensing This project is
+released under the terms of the MIT Open Source License. View *LICENSE.txt* for
+more information.
```

### Comparing `pear_ebi-0.1.61/README.md` & `pear_ebi-0.1.62/pear_ebi.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,91 @@
-
- <h1> <font color='green'>P</font>hylogeny <font color='green'>E</font>mbedding  & <br>  <font color='green'>A</font>pproximate <font color='green'>R</font>epresentation </h1>
- <img src="logos/LOGO_PEAR.png" width="100" height="100" style='position:absolute; left:400px; top:-15px' >
-
-## Goldman Group - European Bioinformatics Institute <img src="logos/goldman_logo.png" width="30" height="30">
-
-PEAR can:
-1. Compute the distance matrix given a set of phylogenetic trees;
-2. Embed and represent the distance matrix in 2D or 3D.
-
-See also the <a href="https://andrearubbi.github.io/Pear-EBI/index.html"> autogenerated documentation </a> and <a href="https://pypi.org/project/pear-ebi/"> PyPI </a>.
-
-PEAR usage
-==========
-Pear is both a python software and library. It can be installed with `python -m pip install pear_ebi` or downloaded from <a href="https://github.com/AndreaRubbi/Pear-EBI">Github</a>. Pear is currently compatible with Linux and Mac OSs.
-
-PEAR as a python library
-------------------------
-Once installed, Pear can be used to upload newick trees in python and represent them in embedded spaces. We recommend to use it on either jupyter notebook or lab, as these tools allow for more interaction with the graphs. On these platforms, the user is allowed to interact with widgets that allows to modify several parameteres of the plots. For specific uses and applications, see the <a href='https://github.com/AndreaRubbi/Pear-EBI/tree/pear_ebi/examples_tree_sets'>examples</a>.
-
-PEAR as a program
------------------
-Run `pear_ebi --help` to see the complete list of arguments and flags.
-### Simple usage
-
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf`
-
-this script calculates the unweighted <a href='https://doi.org/10.1016/0025-5564(81)90043-2'>Robison Foulds</a> distances between the trees in the file "beast_run1.trees", which contains 1001 phylogenetic trees.
-
-the flag *-m* indicates the method used to compute the dissimilarity between phylogeneic trees. In this case, [HasRF](https://code.google.com/archive/p/hashrf/) has been used.
-
-To embed these distances in a lower-dimensional space, we can use PCoA (MDS) or tSNE:
-
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf -pca 2`
-
-we therefore embedded the distance matrix in 2 dimensions. Using the flag *-quality* one can assess the correlation between the distances in the N-dimensional space and in the embedding; while *-report* computes more insightful metrics such as the trustworthiness and continuity of the embedding.
-
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf -pca 2 -plot --show`
-
-The flags *-plot* and *--show* indicate that PEAR has to plot the embeddings and show them, respectively. *-plot* doesn't require any indication on the number of dimensions as it plots the embeddings in 2 dimensions if the distances are embedded in 2 dimensions, while it plots on 2 and 3 dimensions in any other case.
-
-One can specify any number of files containing trees. Moreover, it is possible to specify a directory using *-dir*, and possibly a pattern using *-pattern*, in order to select multiple files.
-
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -subset 100` shows the 3D and 2D embedding of a subset of 100 trees from the original collection.
-
-#### Tree Set
-
-It's possible to compute the distance matrix and re-use it in future runs of PEAR by specifying the distance matrix file with the flag *-d*. Additionally, it's possible to define the name of the output file (*-o*).
-
-If any additional metadata is available, this may be specified by indicating a *.csv* file containing a dataframe of compatible shape.
-
-### Config file
-A standard config toml file can be used for specific emebddings of multiple sets of trees. Instances of toml files are reported in the <a href='https://github.com/AndreaRubbi/Pear-EBI/tree/pear_ebi/examples_tree_sets'>examples</a> folder.
-
-Using the config file allows one to use all the features of PEAR, including additional embedding methods and plot designs. The config file can also be used to specify lists of indexes of interesting trees in the sets, in order to highlight them in the final plots.
-
-### Interactive mode
-`pear_ebi --i` :
-this script launches the program in the interactive mode. Once the program starts, it is going to guide you through its usage thanks to an intuitive interface.
-
-
-### Additional Dependencies
-In order to get the complete report on the quality of embeddings, it may be necessary to run the following command to install additional dependencies:
-
-`sudo apt-get install '^libxcb.*-dev' libx11-xcb-dev libglu1-mesa-dev libxrender-dev libxi-dev libxkbcommon-dev libxkbcommon-x11-dev`
-
-It may be necessary to also install `libgcc` and remove old versions of `libstdc++` from the interpreter libraries.
-________________________
-
-## Licensing
-
-This project is released under the terms of the MIT Open Source License. View
-*LICENSE.txt* for more information.
+Metadata-Version: 2.1
+Name: pear-ebi
+Version: 0.1.62
+Summary: Embeds phylogenetic tree distances and produce representations
+Home-page: https://github.com/AndreaRubbi/TreeEmbedding
+Author: Andrea Rubbi
+Author-email: andrea.rubbi.98@gmail.com
+License: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+ <h1> <font color='green'>P</font>hylogeny <font color='green'>E</font>mbedding  & <br>  <font color='green'>A</font>pproximate <font color='green'>R</font>epresentation </h1>
+ <img src="https://github.com/AndreaRubbi/Pear-EBI/raw/pear_ebi/logos/LOGO_PEAR.png" width="100" height="100" style='position:absolute; left:400px; top:-15px' >
+
+ <img src="https://img.shields.io/github/license/AndreaRubbi/Pear-EBI?color=red&label=License&style=plastic"> <img src="https://img.shields.io/pypi/v/pear_ebi?color=purple&label=version&style=plastic"> <img src="https://img.shields.io/pypi/implementation/pear_ebi?style=plastic"> <img src="https://img.shields.io/pypi/pyversions/pear_ebi?color=green&style=plastic">
+
+
+
+## Goldman Group - European Bioinformatics Institute <img src="https://github.com/AndreaRubbi/Pear-EBI/raw/pear_ebi/logos/goldman_logo.png" width="30" height="30">
+
+PEAR can:
+1. Compute the distance matrix given a set of phylogenetic trees;
+2. Embed and represent the distance matrix in 2D or 3D.
+
+See also the <a href="https://andrearubbi.github.io/Pear-EBI/index.html"> autogenerated documentation </a> and <a href="https://pypi.org/project/pear-ebi/"> PyPI </a>.
+
+PEAR usage
+==========
+Pear is both a python software and library. It can be installed with `python -m pip install pear_ebi` or downloaded from <a href="https://github.com/AndreaRubbi/Pear-EBI">Github</a>. Pear is currently compatible with Linux and Mac OSs.
+
+PEAR as a python library
+------------------------
+Once installed, Pear can be used to upload newick trees in python and represent them in embedded spaces. We recommend to use it on either jupyter notebook or lab, as these tools allow for more interaction with the graphs. On these platforms, the user is allowed to interact with widgets that allows to modify several parameteres of the plots. For specific uses and applications, see the <a href='https://github.com/AndreaRubbi/Pear-EBI/tree/pear_ebi/examples_tree_sets'>examples</a>.
+
+PEAR as a program
+-----------------
+Run `pear_ebi --help` to see the complete list of arguments and flags.
+### Simple usage
+
+`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf_RF`
+
+this script calculates the unweighted <a href='https://doi.org/10.1016/0025-5564(81)90043-2'>Robison Foulds</a> distances between the trees in the file "beast_run1.trees", which contains 1001 phylogenetic trees.
+
+the flag *-m* indicates the method used to compute the dissimilarity between phylogeneic trees. In this case, [HasRF](https://code.google.com/archive/p/hashrf/) has been used.
+
+To embed these distances in a lower-dimensional space, we can use PCoA (MDS) or tSNE:
+
+`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf_RF -pca 2`
+
+we therefore embedded the distance matrix in 2 dimensions. Using the flag *-quality* one can assess the correlation between the distances in the N-dimensional space and in the embedding.
+
+`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf_RF -pca 2 -plot`
+
+The flag *-plot* indicates that PEAR has to plot the embeddings and show them, respectively. If an embedding method is specified the plots are produced anyway. Plotting doesn't require any indication on the number of dimensions as the embeddings are represented in 2 dimensions if the distances are embedded in 2 dimensions, while it plots on 2 and 3 dimensions in any other case.
+
+One can specify any number of files containing trees. Moreover, it is possible to specify a single directory using *-dir*, and possibly a pattern using *-pattern*, in order to select multiple files.
+
+#### Tree Set
+
+It's possible to compute the distance matrix and re-use it in subsequent runs of PEAR by specifying the distance matrix file with the flag *-d*. Additionally, it's possible to define the name of the output file (*-o*).
+
+If any additional metadata is available, this may be specified by indicating a *.csv* file containing a dataframe of compatible shape.
+
+### Config file
+A standard config toml file can be used for specific emebddings of multiple sets of trees. Instances of toml files are reported in the <a href='https://github.com/AndreaRubbi/Pear-EBI/tree/pear_ebi/examples_tree_sets'>examples</a> folder.
+
+Using the config file allows one to use all the features of PEAR, including additional embedding methods and plot designs. The config file can also be used to specify lists of indexes of interesting trees in the sets, in order to highlight them in the final plots.
+
+### Interactive mode
+`pear_ebi --i` :
+this script launches the program in the interactive mode. Once the program starts, it is going to guide you through its usage thanks to an intuitive interface.
+
+
+ <!--- ### Additional Dependencies
+ In order to get the complete report on the quality of embeddings, it may be necessary to
+ run the following command to install additional dependencies:
+
+ `sudo apt-get install '^libxcb.*-dev' libx11-xcb-dev libglu1-mesa-dev libxrender-dev libxi-dev libxkbcommon-dev libxkbcommon-x11-dev`
+
+ It may be necessary to also install `libgcc` and remove old versions of `libstdc++` from the interpreter libraries. --->
+________________________
+
+## Licensing
+
+This project is released under the terms of the MIT Open Source License. View
+*LICENSE.txt* for more information.
```

#### html2text {}

```diff
@@ -1,58 +1,63 @@
+Metadata-Version: 2.1 Name: pear-ebi Version: 0.1.62 Summary: Embeds
+phylogenetic tree distances and produce representations Home-page: https://
+github.com/AndreaRubbi/TreeEmbedding Author: Andrea Rubbi Author-email:
+andrea.rubbi.98@gmail.com License: MIT License Classifier: Development Status
+:: 3 - Alpha Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Description-Content-Type: text/markdown License-File: LICENSE.txt
 ****** Phylogeny Embedding &
 Approximate Representation ******
-[logos/LOGO_PEAR.png] ## Goldman Group - European Bioinformatics Institute
-[logos/goldman_logo.png] PEAR can: 1. Compute the distance matrix given a set
-of phylogenetic trees; 2. Embed and represent the distance matrix in 2D or 3D.
-See also the autogenerated_documentation and PyPI. PEAR usage ========== Pear
-is both a python software and library. It can be installed with `python -m pip
+[https://github.com/AndreaRubbi/Pear-EBI/raw/pear_ebi/logos/LOGO_PEAR.png]
+[https://img.shields.io/github/license/AndreaRubbi/Pear-
+EBI?color=red&label=License&style=plastic] [https://img.shields.io/pypi/v/
+pear_ebi?color=purple&label=version&style=plastic] [https://img.shields.io/
+pypi/implementation/pear_ebi?style=plastic] [https://img.shields.io/pypi/
+pyversions/pear_ebi?color=green&style=plastic] ## Goldman Group - European
+Bioinformatics Institute [https://github.com/AndreaRubbi/Pear-EBI/raw/pear_ebi/
+logos/goldman_logo.png] PEAR can: 1. Compute the distance matrix given a set of
+phylogenetic trees; 2. Embed and represent the distance matrix in 2D or 3D. See
+also the autogenerated_documentation and PyPI. PEAR usage ========== Pear is
+both a python software and library. It can be installed with `python -m pip
 install pear_ebi` or downloaded from Github. Pear is currently compatible with
 Linux and Mac OSs. PEAR as a python library ------------------------ Once
 installed, Pear can be used to upload newick trees in python and represent them
 in embedded spaces. We recommend to use it on either jupyter notebook or lab,
 as these tools allow for more interaction with the graphs. On these platforms,
 the user is allowed to interact with widgets that allows to modify several
 parameteres of the plots. For specific uses and applications, see the examples.
 PEAR as a program ----------------- Run `pear_ebi --help` to see the complete
 list of arguments and flags. ### Simple usage `pear_ebi examples_trees_sets/
-beast_trees/beast_run1.trees -m hashrf` this script calculates the unweighted
-Robison_Foulds distances between the trees in the file "beast_run1.trees",
-which contains 1001 phylogenetic trees. the flag *-m* indicates the method used
-to compute the dissimilarity between phylogeneic trees. In this case, [HasRF]
-(https://code.google.com/archive/p/hashrf/) has been used. To embed these
-distances in a lower-dimensional space, we can use PCoA (MDS) or tSNE:
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf -pca 2` we
-therefore embedded the distance matrix in 2 dimensions. Using the flag *-
-quality* one can assess the correlation between the distances in the N-
-dimensional space and in the embedding; while *-report* computes more
-insightful metrics such as the trustworthiness and continuity of the embedding.
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf -pca 2 -
-plot --show` The flags *-plot* and *--show* indicate that PEAR has to plot the
-embeddings and show them, respectively. *-plot* doesn't require any indication
-on the number of dimensions as it plots the embeddings in 2 dimensions if the
-distances are embedded in 2 dimensions, while it plots on 2 and 3 dimensions in
-any other case. One can specify any number of files containing trees. Moreover,
-it is possible to specify a directory using *-dir*, and possibly a pattern
-using *-pattern*, in order to select multiple files. `pear_ebi
-examples_trees_sets/beast_trees/beast_run1.trees -subset 100` shows the 3D and
-2D embedding of a subset of 100 trees from the original collection. #### Tree
-Set It's possible to compute the distance matrix and re-use it in future runs
-of PEAR by specifying the distance matrix file with the flag *-d*.
-Additionally, it's possible to define the name of the output file (*-o*). If
-any additional metadata is available, this may be specified by indicating a
-*.csv* file containing a dataframe of compatible shape. ### Config file A
-standard config toml file can be used for specific emebddings of multiple sets
-of trees. Instances of toml files are reported in the examples folder. Using
-the config file allows one to use all the features of PEAR, including
-additional embedding methods and plot designs. The config file can also be used
-to specify lists of indexes of interesting trees in the sets, in order to
-highlight them in the final plots. ### Interactive mode `pear_ebi --i` : this
-script launches the program in the interactive mode. Once the program starts,
-it is going to guide you through its usage thanks to an intuitive interface.
-### Additional Dependencies In order to get the complete report on the quality
-of embeddings, it may be necessary to run the following command to install
-additional dependencies: `sudo apt-get install '^libxcb.*-dev' libx11-xcb-dev
-libglu1-mesa-dev libxrender-dev libxi-dev libxkbcommon-dev libxkbcommon-x11-
-dev` It may be necessary to also install `libgcc` and remove old versions of
-`libstdc++` from the interpreter libraries. ________________________ ##
-Licensing This project is released under the terms of the MIT Open Source
-License. View *LICENSE.txt* for more information.
+beast_trees/beast_run1.trees -m hashrf_RF` this script calculates the
+unweighted Robison_Foulds distances between the trees in the file
+"beast_run1.trees", which contains 1001 phylogenetic trees. the flag *-m*
+indicates the method used to compute the dissimilarity between phylogeneic
+trees. In this case, [HasRF](https://code.google.com/archive/p/hashrf/) has
+been used. To embed these distances in a lower-dimensional space, we can use
+PCoA (MDS) or tSNE: `pear_ebi examples_trees_sets/beast_trees/beast_run1.trees
+-m hashrf_RF -pca 2` we therefore embedded the distance matrix in 2 dimensions.
+Using the flag *-quality* one can assess the correlation between the distances
+in the N-dimensional space and in the embedding. `pear_ebi examples_trees_sets/
+beast_trees/beast_run1.trees -m hashrf_RF -pca 2 -plot` The flag *-plot*
+indicates that PEAR has to plot the embeddings and show them, respectively. If
+an embedding method is specified the plots are produced anyway. Plotting
+doesn't require any indication on the number of dimensions as the embeddings
+are represented in 2 dimensions if the distances are embedded in 2 dimensions,
+while it plots on 2 and 3 dimensions in any other case. One can specify any
+number of files containing trees. Moreover, it is possible to specify a single
+directory using *-dir*, and possibly a pattern using *-pattern*, in order to
+select multiple files. #### Tree Set It's possible to compute the distance
+matrix and re-use it in subsequent runs of PEAR by specifying the distance
+matrix file with the flag *-d*. Additionally, it's possible to define the name
+of the output file (*-o*). If any additional metadata is available, this may be
+specified by indicating a *.csv* file containing a dataframe of compatible
+shape. ### Config file A standard config toml file can be used for specific
+emebddings of multiple sets of trees. Instances of toml files are reported in
+the examples folder. Using the config file allows one to use all the features
+of PEAR, including additional embedding methods and plot designs. The config
+file can also be used to specify lists of indexes of interesting trees in the
+sets, in order to highlight them in the final plots. ### Interactive mode
+`pear_ebi --i` : this script launches the program in the interactive mode. Once
+the program starts, it is going to guide you through its usage thanks to an
+intuitive interface.  ________________________ ## Licensing This project is
+released under the terms of the MIT Open Source License. View *LICENSE.txt* for
+more information.
```

### Comparing `pear_ebi-0.1.61/pear_ebi/__main__.py` & `pear_ebi-0.1.62/pear_ebi/__main__.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/COPYING` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/COPYING`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/INSTALL` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/INSTALL`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/Makefile` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/Makefile`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/Makefile.in` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/Makefile.in`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/Random.cpp` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/Random.cpp`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/Random.o` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/Random.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/aclocal.m4` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/aclocal.m4`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/config.h` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/config.h`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/config.h.in` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/config.h.in`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/config.hh` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/config.hh`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/config.hh.in` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/config.hh.in`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/config.log` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/config.log`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/config.status` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/config.status`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/configure` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/configure`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/configure.lineno` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/configure.lineno`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/depcomp` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/depcomp`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hash.cc` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hash.cc`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hash.hh` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hash.hh`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hash.o` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hash.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hashfunc.cc` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hashfunc.cc`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hashfunc.hh` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hashfunc.hh`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hashfunc.o` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hashfunc.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hashrf` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hashrf`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hashrf.cc` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hashrf.cc`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/hashrf.o` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/hashrf.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/install-sh` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/install-sh`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/label-map.cc` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/label-map.cc`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/label-map.hh` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/label-map.hh`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/label-map.o` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/label-map.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/missing` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/missing`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/newick.c` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/newick.c`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/newick.h` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/newick.h`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/HashRF/newick.o` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/HashRF/newick.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/RF_pypy.py` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/RF_pypy.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/hashrf.py` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/hashrf.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/maple_RF.py` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/maple_RF.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/CMakeCache.txt` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/CMakeCache.txt`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/CMakeLists.txt` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/COPYING` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/COPYING`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/COPYING.LESSER` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/CPackConfig.cmake` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/CPackConfig.cmake`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/CPackSourceConfig.cmake` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/CPackSourceConfig.cmake`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/Makefile` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/Makefile`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/README` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/README`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/cmake_install.cmake` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/icon.ico` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/icon.ico`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/tqDist/icon.jpg` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/tqDist/icon.jpg`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/calculate_distances/tqdist.py` & `pear_ebi-0.1.62/pear_ebi/calculate_distances/tqdist.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/embeddings/Isomap_e.py` & `pear_ebi-0.1.62/pear_ebi/embeddings/Isomap_e.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/embeddings/LLE_e.py` & `pear_ebi-0.1.62/pear_ebi/embeddings/LLE_e.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/embeddings/PCA_e.py` & `pear_ebi-0.1.62/pear_ebi/embeddings/PCA_e.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/embeddings/emb_quality.py` & `pear_ebi-0.1.62/pear_ebi/embeddings/emb_quality.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/embeddings/graph/graph.py` & `pear_ebi-0.1.62/pear_ebi/embeddings/graph/graph.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/embeddings/tSNE_e.py` & `pear_ebi-0.1.62/pear_ebi/embeddings/tSNE_e.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/interactive_mode/interactive.py` & `pear_ebi-0.1.62/pear_ebi/interactive_mode/interactive.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/subsample/subsample.py` & `pear_ebi-0.1.62/pear_ebi/subsample/subsample.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/subsample/subsample_multiprocess.py` & `pear_ebi-0.1.62/pear_ebi/subsample/subsample_multiprocess.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/tree_emb_parser.py` & `pear_ebi-0.1.62/pear_ebi/tree_emb_parser.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/pear_ebi/tree_set.py` & `pear_ebi-0.1.62/pear_ebi/tree_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 import time
 import uuid
 import warnings
 
 import numpy as np
 import pandas as pd
 from rich import print
-
 # ? rich is a very nice library that allows to
 # ? easily format the output of console
 # ? https://github.com/Textualize/rich
 from rich.console import Console
 
 # getting the name of the directory
 current = os.path.dirname(os.path.realpath(__file__))
```

### Comparing `pear_ebi-0.1.61/pear_ebi.egg-info/PKG-INFO` & `pear_ebi-0.1.62/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
-Name: pear-ebi
-Version: 0.1.61
+Name: pear_ebi
+Version: 0.1.62
 Summary: Embeds phylogenetic tree distances and produce representations
 Home-page: https://github.com/AndreaRubbi/TreeEmbedding
 Author: Andrea Rubbi
 Author-email: andrea.rubbi.98@gmail.com
 License: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
  <h1> <font color='green'>P</font>hylogeny <font color='green'>E</font>mbedding  & <br>  <font color='green'>A</font>pproximate <font color='green'>R</font>epresentation </h1>
- <img src="logos/LOGO_PEAR.png" width="100" height="100" style='position:absolute; left:400px; top:-15px' >
+ <img src="https://github.com/AndreaRubbi/Pear-EBI/raw/pear_ebi/logos/LOGO_PEAR.png" width="100" height="100" style='position:absolute; left:400px; top:-15px' >
 
-## Goldman Group - European Bioinformatics Institute <img src="logos/goldman_logo.png" width="30" height="30">
+ <img src="https://img.shields.io/github/license/AndreaRubbi/Pear-EBI?color=red&label=License&style=plastic"> <img src="https://img.shields.io/pypi/v/pear_ebi?color=purple&label=version&style=plastic"> <img src="https://img.shields.io/pypi/implementation/pear_ebi?style=plastic"> <img src="https://img.shields.io/pypi/pyversions/pear_ebi?color=green&style=plastic">
+
+
+
+## Goldman Group - European Bioinformatics Institute <img src="https://github.com/AndreaRubbi/Pear-EBI/raw/pear_ebi/logos/goldman_logo.png" width="30" height="30">
 
 PEAR can:
 1. Compute the distance matrix given a set of phylogenetic trees;
 2. Embed and represent the distance matrix in 2D or 3D.
 
 See also the <a href="https://andrearubbi.github.io/Pear-EBI/index.html"> autogenerated documentation </a> and <a href="https://pypi.org/project/pear-ebi/"> PyPI </a>.
 
@@ -30,55 +38,54 @@
 Once installed, Pear can be used to upload newick trees in python and represent them in embedded spaces. We recommend to use it on either jupyter notebook or lab, as these tools allow for more interaction with the graphs. On these platforms, the user is allowed to interact with widgets that allows to modify several parameteres of the plots. For specific uses and applications, see the <a href='https://github.com/AndreaRubbi/Pear-EBI/tree/pear_ebi/examples_tree_sets'>examples</a>.
 
 PEAR as a program
 -----------------
 Run `pear_ebi --help` to see the complete list of arguments and flags.
 ### Simple usage
 
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf`
+`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf_RF`
 
 this script calculates the unweighted <a href='https://doi.org/10.1016/0025-5564(81)90043-2'>Robison Foulds</a> distances between the trees in the file "beast_run1.trees", which contains 1001 phylogenetic trees.
 
 the flag *-m* indicates the method used to compute the dissimilarity between phylogeneic trees. In this case, [HasRF](https://code.google.com/archive/p/hashrf/) has been used.
 
 To embed these distances in a lower-dimensional space, we can use PCoA (MDS) or tSNE:
 
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf -pca 2`
-
-we therefore embedded the distance matrix in 2 dimensions. Using the flag *-quality* one can assess the correlation between the distances in the N-dimensional space and in the embedding; while *-report* computes more insightful metrics such as the trustworthiness and continuity of the embedding.
+`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf_RF -pca 2`
 
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf -pca 2 -plot --show`
+we therefore embedded the distance matrix in 2 dimensions. Using the flag *-quality* one can assess the correlation between the distances in the N-dimensional space and in the embedding.
 
-The flags *-plot* and *--show* indicate that PEAR has to plot the embeddings and show them, respectively. *-plot* doesn't require any indication on the number of dimensions as it plots the embeddings in 2 dimensions if the distances are embedded in 2 dimensions, while it plots on 2 and 3 dimensions in any other case.
+`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf_RF -pca 2 -plot`
 
-One can specify any number of files containing trees. Moreover, it is possible to specify a directory using *-dir*, and possibly a pattern using *-pattern*, in order to select multiple files.
+The flag *-plot* indicates that PEAR has to plot the embeddings and show them, respectively. If an embedding method is specified the plots are produced anyway. Plotting doesn't require any indication on the number of dimensions as the embeddings are represented in 2 dimensions if the distances are embedded in 2 dimensions, while it plots on 2 and 3 dimensions in any other case.
 
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -subset 100` shows the 3D and 2D embedding of a subset of 100 trees from the original collection.
+One can specify any number of files containing trees. Moreover, it is possible to specify a single directory using *-dir*, and possibly a pattern using *-pattern*, in order to select multiple files.
 
 #### Tree Set
 
-It's possible to compute the distance matrix and re-use it in future runs of PEAR by specifying the distance matrix file with the flag *-d*. Additionally, it's possible to define the name of the output file (*-o*).
+It's possible to compute the distance matrix and re-use it in subsequent runs of PEAR by specifying the distance matrix file with the flag *-d*. Additionally, it's possible to define the name of the output file (*-o*).
 
 If any additional metadata is available, this may be specified by indicating a *.csv* file containing a dataframe of compatible shape.
 
 ### Config file
 A standard config toml file can be used for specific emebddings of multiple sets of trees. Instances of toml files are reported in the <a href='https://github.com/AndreaRubbi/Pear-EBI/tree/pear_ebi/examples_tree_sets'>examples</a> folder.
 
 Using the config file allows one to use all the features of PEAR, including additional embedding methods and plot designs. The config file can also be used to specify lists of indexes of interesting trees in the sets, in order to highlight them in the final plots.
 
 ### Interactive mode
 `pear_ebi --i` :
 this script launches the program in the interactive mode. Once the program starts, it is going to guide you through its usage thanks to an intuitive interface.
 
 
-### Additional Dependencies
-In order to get the complete report on the quality of embeddings, it may be necessary to run the following command to install additional dependencies:
+ <!--- ### Additional Dependencies
+ In order to get the complete report on the quality of embeddings, it may be necessary to
+ run the following command to install additional dependencies:
 
-`sudo apt-get install '^libxcb.*-dev' libx11-xcb-dev libglu1-mesa-dev libxrender-dev libxi-dev libxkbcommon-dev libxkbcommon-x11-dev`
+ `sudo apt-get install '^libxcb.*-dev' libx11-xcb-dev libglu1-mesa-dev libxrender-dev libxi-dev libxkbcommon-dev libxkbcommon-x11-dev`
 
-It may be necessary to also install `libgcc` and remove old versions of `libstdc++` from the interpreter libraries.
+ It may be necessary to also install `libgcc` and remove old versions of `libstdc++` from the interpreter libraries. --->
 ________________________
 
 ## Licensing
 
 This project is released under the terms of the MIT Open Source License. View
 *LICENSE.txt* for more information.
```

#### html2text {}

```diff
@@ -1,63 +1,63 @@
-Metadata-Version: 2.1 Name: pear-ebi Version: 0.1.61 Summary: Embeds
+Metadata-Version: 2.1 Name: pear_ebi Version: 0.1.62 Summary: Embeds
 phylogenetic tree distances and produce representations Home-page: https://
 github.com/AndreaRubbi/TreeEmbedding Author: Andrea Rubbi Author-email:
-andrea.rubbi.98@gmail.com License: MIT License Description-Content-Type: text/
-markdown License-File: LICENSE.txt
+andrea.rubbi.98@gmail.com License: MIT License Classifier: Development Status
+:: 3 - Alpha Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Description-Content-Type: text/markdown License-File: LICENSE.txt
 ****** Phylogeny Embedding &
 Approximate Representation ******
-[logos/LOGO_PEAR.png] ## Goldman Group - European Bioinformatics Institute
-[logos/goldman_logo.png] PEAR can: 1. Compute the distance matrix given a set
-of phylogenetic trees; 2. Embed and represent the distance matrix in 2D or 3D.
-See also the autogenerated_documentation and PyPI. PEAR usage ========== Pear
-is both a python software and library. It can be installed with `python -m pip
+[https://github.com/AndreaRubbi/Pear-EBI/raw/pear_ebi/logos/LOGO_PEAR.png]
+[https://img.shields.io/github/license/AndreaRubbi/Pear-
+EBI?color=red&label=License&style=plastic] [https://img.shields.io/pypi/v/
+pear_ebi?color=purple&label=version&style=plastic] [https://img.shields.io/
+pypi/implementation/pear_ebi?style=plastic] [https://img.shields.io/pypi/
+pyversions/pear_ebi?color=green&style=plastic] ## Goldman Group - European
+Bioinformatics Institute [https://github.com/AndreaRubbi/Pear-EBI/raw/pear_ebi/
+logos/goldman_logo.png] PEAR can: 1. Compute the distance matrix given a set of
+phylogenetic trees; 2. Embed and represent the distance matrix in 2D or 3D. See
+also the autogenerated_documentation and PyPI. PEAR usage ========== Pear is
+both a python software and library. It can be installed with `python -m pip
 install pear_ebi` or downloaded from Github. Pear is currently compatible with
 Linux and Mac OSs. PEAR as a python library ------------------------ Once
 installed, Pear can be used to upload newick trees in python and represent them
 in embedded spaces. We recommend to use it on either jupyter notebook or lab,
 as these tools allow for more interaction with the graphs. On these platforms,
 the user is allowed to interact with widgets that allows to modify several
 parameteres of the plots. For specific uses and applications, see the examples.
 PEAR as a program ----------------- Run `pear_ebi --help` to see the complete
 list of arguments and flags. ### Simple usage `pear_ebi examples_trees_sets/
-beast_trees/beast_run1.trees -m hashrf` this script calculates the unweighted
-Robison_Foulds distances between the trees in the file "beast_run1.trees",
-which contains 1001 phylogenetic trees. the flag *-m* indicates the method used
-to compute the dissimilarity between phylogeneic trees. In this case, [HasRF]
-(https://code.google.com/archive/p/hashrf/) has been used. To embed these
-distances in a lower-dimensional space, we can use PCoA (MDS) or tSNE:
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf -pca 2` we
-therefore embedded the distance matrix in 2 dimensions. Using the flag *-
-quality* one can assess the correlation between the distances in the N-
-dimensional space and in the embedding; while *-report* computes more
-insightful metrics such as the trustworthiness and continuity of the embedding.
-`pear_ebi examples_trees_sets/beast_trees/beast_run1.trees -m hashrf -pca 2 -
-plot --show` The flags *-plot* and *--show* indicate that PEAR has to plot the
-embeddings and show them, respectively. *-plot* doesn't require any indication
-on the number of dimensions as it plots the embeddings in 2 dimensions if the
-distances are embedded in 2 dimensions, while it plots on 2 and 3 dimensions in
-any other case. One can specify any number of files containing trees. Moreover,
-it is possible to specify a directory using *-dir*, and possibly a pattern
-using *-pattern*, in order to select multiple files. `pear_ebi
-examples_trees_sets/beast_trees/beast_run1.trees -subset 100` shows the 3D and
-2D embedding of a subset of 100 trees from the original collection. #### Tree
-Set It's possible to compute the distance matrix and re-use it in future runs
-of PEAR by specifying the distance matrix file with the flag *-d*.
-Additionally, it's possible to define the name of the output file (*-o*). If
-any additional metadata is available, this may be specified by indicating a
-*.csv* file containing a dataframe of compatible shape. ### Config file A
-standard config toml file can be used for specific emebddings of multiple sets
-of trees. Instances of toml files are reported in the examples folder. Using
-the config file allows one to use all the features of PEAR, including
-additional embedding methods and plot designs. The config file can also be used
-to specify lists of indexes of interesting trees in the sets, in order to
-highlight them in the final plots. ### Interactive mode `pear_ebi --i` : this
-script launches the program in the interactive mode. Once the program starts,
-it is going to guide you through its usage thanks to an intuitive interface.
-### Additional Dependencies In order to get the complete report on the quality
-of embeddings, it may be necessary to run the following command to install
-additional dependencies: `sudo apt-get install '^libxcb.*-dev' libx11-xcb-dev
-libglu1-mesa-dev libxrender-dev libxi-dev libxkbcommon-dev libxkbcommon-x11-
-dev` It may be necessary to also install `libgcc` and remove old versions of
-`libstdc++` from the interpreter libraries. ________________________ ##
-Licensing This project is released under the terms of the MIT Open Source
-License. View *LICENSE.txt* for more information.
+beast_trees/beast_run1.trees -m hashrf_RF` this script calculates the
+unweighted Robison_Foulds distances between the trees in the file
+"beast_run1.trees", which contains 1001 phylogenetic trees. the flag *-m*
+indicates the method used to compute the dissimilarity between phylogeneic
+trees. In this case, [HasRF](https://code.google.com/archive/p/hashrf/) has
+been used. To embed these distances in a lower-dimensional space, we can use
+PCoA (MDS) or tSNE: `pear_ebi examples_trees_sets/beast_trees/beast_run1.trees
+-m hashrf_RF -pca 2` we therefore embedded the distance matrix in 2 dimensions.
+Using the flag *-quality* one can assess the correlation between the distances
+in the N-dimensional space and in the embedding. `pear_ebi examples_trees_sets/
+beast_trees/beast_run1.trees -m hashrf_RF -pca 2 -plot` The flag *-plot*
+indicates that PEAR has to plot the embeddings and show them, respectively. If
+an embedding method is specified the plots are produced anyway. Plotting
+doesn't require any indication on the number of dimensions as the embeddings
+are represented in 2 dimensions if the distances are embedded in 2 dimensions,
+while it plots on 2 and 3 dimensions in any other case. One can specify any
+number of files containing trees. Moreover, it is possible to specify a single
+directory using *-dir*, and possibly a pattern using *-pattern*, in order to
+select multiple files. #### Tree Set It's possible to compute the distance
+matrix and re-use it in subsequent runs of PEAR by specifying the distance
+matrix file with the flag *-d*. Additionally, it's possible to define the name
+of the output file (*-o*). If any additional metadata is available, this may be
+specified by indicating a *.csv* file containing a dataframe of compatible
+shape. ### Config file A standard config toml file can be used for specific
+emebddings of multiple sets of trees. Instances of toml files are reported in
+the examples folder. Using the config file allows one to use all the features
+of PEAR, including additional embedding methods and plot designs. The config
+file can also be used to specify lists of indexes of interesting trees in the
+sets, in order to highlight them in the final plots. ### Interactive mode
+`pear_ebi --i` : this script launches the program in the interactive mode. Once
+the program starts, it is going to guide you through its usage thanks to an
+intuitive interface.  ________________________ ## Licensing This project is
+released under the terms of the MIT Open Source License. View *LICENSE.txt* for
+more information.
```

### Comparing `pear_ebi-0.1.61/pear_ebi.egg-info/SOURCES.txt` & `pear_ebi-0.1.62/pear_ebi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.61/test/test.py` & `pear_ebi-0.1.62/test/test.py`

 * *Files identical despite different names*

