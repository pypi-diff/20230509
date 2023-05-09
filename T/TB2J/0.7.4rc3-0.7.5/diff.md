# Comparing `tmp/TB2J-0.7.4rc3.tar.gz` & `tmp/TB2J-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TB2J-0.7.4rc3.tar", last modified: Thu Jun 30 13:33:31 2022, max compression
+gzip compressed data, was "TB2J-0.7.5.tar", last modified: Tue May  9 15:34:38 2023, max compression
```

## Comparing `TB2J-0.7.4rc3.tar` & `TB2J-0.7.5.tar`

### file list

```diff
@@ -1,76 +1,74 @@
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-30 13:33:31.601678 TB2J-0.7.4rc3/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1327 2020-07-08 14:12:19.000000 TB2J-0.7.4rc3/LICENSE
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1257 2022-06-30 13:33:31.597678 TB2J-0.7.4rc3/PKG-INFO
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1914 2022-06-29 07:51:51.000000 TB2J-0.7.4rc3/README.md
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-30 13:33:31.589678 TB2J-0.7.4rc3/TB2J/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     7082 2022-06-28 09:12:36.000000 TB2J-0.7.4rc3/TB2J/Jdownfolder.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1771 2022-06-28 09:12:36.000000 TB2J-0.7.4rc3/TB2J/Jtensor.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     3994 2022-04-19 18:50:05.000000 TB2J-0.7.4rc3/TB2J/Oiju.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     7423 2022-04-19 18:59:46.000000 TB2J-0.7.4rc3/TB2J/Oiju_epc.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       26 2022-06-29 10:23:38.000000 TB2J-0.7.4rc3/TB2J/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2884 2022-02-27 23:27:25.000000 TB2J-0.7.4rc3/TB2J/citation.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2489 2022-01-16 11:30:39.000000 TB2J-0.7.4rc3/TB2J/contour.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2952 2022-06-30 13:32:49.000000 TB2J-0.7.4rc3/TB2J/cut_cell.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     3518 2022-04-19 18:50:05.000000 TB2J-0.7.4rc3/TB2J/epc.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    28490 2022-06-30 11:14:23.000000 TB2J-0.7.4rc3/TB2J/exchange.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    11699 2022-06-30 11:12:22.000000 TB2J-0.7.4rc3/TB2J/exchangeCL2.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     8372 2022-04-30 07:59:33.000000 TB2J-0.7.4rc3/TB2J/exchange_pert.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     9017 2022-04-19 18:50:05.000000 TB2J-0.7.4rc3/TB2J/exchange_qspace.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-30 13:33:31.593678 TB2J-0.7.4rc3/TB2J/external/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      137 2022-04-30 08:05:35.000000 TB2J-0.7.4rc3/TB2J/external/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     5943 2022-04-30 07:58:12.000000 TB2J-0.7.4rc3/TB2J/external/p_tqdm.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     6630 2022-04-19 18:50:05.000000 TB2J-0.7.4rc3/TB2J/gpaw_wrapper.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    12273 2022-02-27 23:27:25.000000 TB2J-0.7.4rc3/TB2J/green.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1571 2022-02-27 23:27:25.000000 TB2J-0.7.4rc3/TB2J/greentest.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-30 13:33:31.593678 TB2J-0.7.4rc3/TB2J/io_exchange/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       32 2020-07-08 14:12:19.000000 TB2J-0.7.4rc3/TB2J/io_exchange/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    16889 2022-06-29 19:25:14.000000 TB2J-0.7.4rc3/TB2J/io_exchange/io_exchange.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     6720 2022-04-19 18:45:40.000000 TB2J-0.7.4rc3/TB2J/io_exchange/io_multibinit.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     4024 2022-04-19 18:44:14.000000 TB2J-0.7.4rc3/TB2J/io_exchange/io_tomsasd.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    10198 2022-04-19 18:43:25.000000 TB2J-0.7.4rc3/TB2J/io_exchange/io_txt.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     3190 2022-04-19 18:40:58.000000 TB2J-0.7.4rc3/TB2J/io_exchange/io_uppasd.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     5563 2022-06-28 09:12:36.000000 TB2J-0.7.4rc3/TB2J/io_exchange/io_vampire.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     6921 2022-04-19 18:50:05.000000 TB2J-0.7.4rc3/TB2J/io_merge.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      533 2022-03-01 14:26:44.000000 TB2J-0.7.4rc3/TB2J/kpoints.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    18281 2021-11-24 10:31:21.000000 TB2J-0.7.4rc3/TB2J/manager.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    17881 2022-04-19 19:02:24.000000 TB2J-0.7.4rc3/TB2J/myTB.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     4722 2021-10-04 10:59:57.000000 TB2J-0.7.4rc3/TB2J/orbmap.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     4092 2022-02-27 23:27:25.000000 TB2J-0.7.4rc3/TB2J/pauli.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1223 2022-04-19 18:50:05.000000 TB2J-0.7.4rc3/TB2J/pert.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1435 2022-04-19 18:50:05.000000 TB2J-0.7.4rc3/TB2J/plot.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     1126 2021-05-27 13:46:56.000000 TB2J-0.7.4rc3/TB2J/rotate_atoms.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    10355 2022-04-19 18:50:05.000000 TB2J-0.7.4rc3/TB2J/sisl_wrapper.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-30 13:33:31.597678 TB2J-0.7.4rc3/TB2J/spinham/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)        0 2020-07-08 14:12:19.000000 TB2J-0.7.4rc3/TB2J/spinham/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2234 2021-09-17 19:59:43.000000 TB2J-0.7.4rc3/TB2J/spinham/base_parser.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      741 2020-07-08 14:12:19.000000 TB2J-0.7.4rc3/TB2J/spinham/constants.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    13322 2022-04-19 18:57:57.000000 TB2J-0.7.4rc3/TB2J/spinham/hamiltonian.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     9870 2021-11-24 10:31:21.000000 TB2J-0.7.4rc3/TB2J/spinham/hamiltonian_terms.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     7011 2022-04-19 19:03:09.000000 TB2J-0.7.4rc3/TB2J/spinham/plot.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2176 2021-10-04 10:59:57.000000 TB2J-0.7.4rc3/TB2J/spinham/qsolver.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2238 2021-02-01 11:14:39.000000 TB2J-0.7.4rc3/TB2J/spinham/spin_api.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    10923 2022-04-19 19:03:17.000000 TB2J-0.7.4rc3/TB2J/spinham/spin_xml.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    12149 2021-03-23 09:04:55.000000 TB2J-0.7.4rc3/TB2J/spinham/supercell.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    19588 2022-06-29 10:42:47.000000 TB2J-0.7.4rc3/TB2J/supercell.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     3896 2022-04-19 19:03:29.000000 TB2J-0.7.4rc3/TB2J/utest.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     9358 2022-04-19 18:53:16.000000 TB2J-0.7.4rc3/TB2J/utils.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      276 2022-04-13 09:35:56.000000 TB2J-0.7.4rc3/TB2J/versioninfo.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-30 13:33:31.597678 TB2J-0.7.4rc3/TB2J/wannier/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       70 2021-10-04 10:59:57.000000 TB2J-0.7.4rc3/TB2J/wannier/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     3664 2022-02-27 23:27:25.000000 TB2J-0.7.4rc3/TB2J/wannier/w90_parser.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-30 13:33:31.593678 TB2J-0.7.4rc3/TB2J.egg-info/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1257 2022-06-30 13:33:31.000000 TB2J-0.7.4rc3/TB2J.egg-info/PKG-INFO
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1402 2022-06-30 13:33:31.000000 TB2J-0.7.4rc3/TB2J.egg-info/SOURCES.txt
--rw-rw-r--   0 hexu      (1000) hexu      (1000)        1 2022-06-30 13:33:31.000000 TB2J-0.7.4rc3/TB2J.egg-info/dependency_links.txt
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       68 2022-06-30 13:33:31.000000 TB2J-0.7.4rc3/TB2J.egg-info/requires.txt
--rw-rw-r--   0 hexu      (1000) hexu      (1000)        5 2022-06-30 13:33:31.000000 TB2J-0.7.4rc3/TB2J.egg-info/top_level.txt
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-30 13:33:31.597678 TB2J-0.7.4rc3/scripts/
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     1663 2021-03-27 13:32:37.000000 TB2J-0.7.4rc3/scripts/TB2J_downfold.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     1185 2022-06-29 10:14:59.000000 TB2J-0.7.4rc3/scripts/TB2J_eigen.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     3379 2022-03-01 14:30:46.000000 TB2J-0.7.4rc3/scripts/TB2J_magnon.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     1277 2021-02-01 11:14:39.000000 TB2J-0.7.4rc3/scripts/TB2J_merge.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)      715 2021-11-24 10:31:21.000000 TB2J-0.7.4rc3/scripts/TB2J_rotate.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     5083 2022-02-27 23:27:25.000000 TB2J-0.7.4rc3/scripts/siesta2J.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     7092 2021-11-24 10:31:21.000000 TB2J-0.7.4rc3/scripts/wann2J.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       38 2022-06-30 13:33:31.601678 TB2J-0.7.4rc3/setup.cfg
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1789 2022-06-30 13:33:28.000000 TB2J-0.7.4rc3/setup.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-09 15:34:38.145051 TB2J-0.7.5/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1327 2023-05-09 15:15:14.000000 TB2J-0.7.5/LICENSE
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2023-05-09 15:34:38.145051 TB2J-0.7.5/PKG-INFO
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1902 2023-05-09 15:15:38.000000 TB2J-0.7.5/README.md
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-09 15:34:38.145051 TB2J-0.7.5/TB2J/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     7121 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/Jdownfolder.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1771 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/Jtensor.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3994 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/Oiju.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     7423 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/Oiju_epc.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)       22 2023-05-09 15:34:33.000000 TB2J-0.7.5/TB2J/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2884 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/citation.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2489 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/contour.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3518 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/epc.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    29412 2023-05-09 15:33:43.000000 TB2J-0.7.5/TB2J/exchange.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    11701 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/exchangeCL2.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     8372 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/exchange_pert.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9017 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/exchange_qspace.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-09 15:34:38.145051 TB2J-0.7.5/TB2J/external/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      137 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/external/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     5943 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/external/p_tqdm.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6630 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/gpaw_wrapper.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    12286 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/green.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1571 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/greentest.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-09 15:34:38.145051 TB2J-0.7.5/TB2J/io_exchange/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       32 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/io_exchange/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    16870 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/io_exchange/io_exchange.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6720 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/io_exchange/io_multibinit.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4024 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/io_exchange/io_tomsasd.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    10198 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/io_exchange/io_txt.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3190 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/io_exchange/io_uppasd.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     5639 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/io_exchange/io_vampire.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6921 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/io_merge.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      533 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/kpoints.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    18356 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/manager.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    17974 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/myTB.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4756 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/orbmap.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4092 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/pauli.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1223 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/pert.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1435 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/plot.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1126 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/rotate_atoms.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    11639 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/sisl_wrapper.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-09 15:34:38.145051 TB2J-0.7.5/TB2J/spinham/
+-rw-rw-r--   0 hexu      (1032) phythema   (500)        0 2020-07-08 14:12:19.000000 TB2J-0.7.5/TB2J/spinham/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2234 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/spinham/base_parser.py
+-rw-rw-r--   0 hexu      (1032) phythema   (500)      741 2020-07-08 14:12:19.000000 TB2J-0.7.5/TB2J/spinham/constants.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    13323 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/spinham/hamiltonian.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9870 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/spinham/hamiltonian_terms.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     7011 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/spinham/plot.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2215 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/spinham/qsolver.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2238 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/spinham/spin_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    10923 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/spinham/spin_xml.py
+-rw-rw-r--   0 hexu      (1032) phythema   (500)    12149 2021-03-23 09:04:55.000000 TB2J-0.7.5/TB2J/spinham/supercell.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3896 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/utest.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9358 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/utils.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      276 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/versioninfo.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-09 15:34:38.145051 TB2J-0.7.5/TB2J/wannier/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       70 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/wannier/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4092 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/wannier/w90_parser.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-09 15:34:38.145051 TB2J-0.7.5/TB2J.egg-info/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2023-05-09 15:34:38.000000 TB2J-0.7.5/TB2J.egg-info/PKG-INFO
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1367 2023-05-09 15:34:38.000000 TB2J-0.7.5/TB2J.egg-info/SOURCES.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)        1 2023-05-09 15:34:38.000000 TB2J-0.7.5/TB2J.egg-info/dependency_links.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)       68 2023-05-09 15:34:38.000000 TB2J-0.7.5/TB2J.egg-info/requires.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)        5 2023-05-09 15:34:38.000000 TB2J-0.7.5/TB2J.egg-info/top_level.txt
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-09 15:34:38.145051 TB2J-0.7.5/scripts/
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     2160 2023-05-09 15:15:38.000000 TB2J-0.7.5/scripts/TB2J_downfold.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1186 2023-05-09 15:15:38.000000 TB2J-0.7.5/scripts/TB2J_eigen.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     3379 2023-05-09 15:15:14.000000 TB2J-0.7.5/scripts/TB2J_magnon.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1475 2023-05-09 15:15:38.000000 TB2J-0.7.5/scripts/TB2J_merge.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)      715 2023-05-09 15:15:14.000000 TB2J-0.7.5/scripts/TB2J_rotate.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     5083 2023-05-09 15:15:14.000000 TB2J-0.7.5/scripts/siesta2J.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     7092 2023-05-09 15:15:14.000000 TB2J-0.7.5/scripts/wann2J.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)       38 2023-05-09 15:34:38.145051 TB2J-0.7.5/setup.cfg
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1785 2023-05-09 15:34:15.000000 TB2J-0.7.5/setup.py
```

### Comparing `TB2J-0.7.4rc3/LICENSE` & `TB2J-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/PKG-INFO` & `TB2J-0.7.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TB2J
-Version: 0.7.4rc3
+Version: 0.7.5
 Summary: TB2J: First principle to Heisenberg exchange J using tight-binding Green function method
 Home-page: UNKNOWN
 Author: Xu He
 Author-email: mailhexu@gmail.com
 License: BSD-2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `TB2J-0.7.4rc3/README.md` & `TB2J-0.7.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,20 +18,20 @@
  - Minimal user input, which allows for a black-box like experience and automatic workflows.
  - Versatile API on both the input (DFT Hamiltonian) and the output (Heisenberg model) sides.
 
 For more information, see the documentation on
  <https://tb2j.readthedocs.io/en/latest/>
 
 ## Dependencies
-* python (tested for version 3.7 to 3.10)
+* python (tested for ver 3.6)
 * numpy 
 * scipy
 * ASE (atomic simulation environment) 
 * matplotlib  (optional) if you want to plot magnon band structure directly. 
 * sisl (optional) for Siesta interface
 
 ## Installation
 pip install TB2J
 
 ## Message:
-- We welcome contributions. If you would like to add the interface to other codes, or extend the capability of TB2J, please contact us! <mailheux_AT_gmail_DOT_com>
+- We welcome contributions. If you would like to add the interface to other codes, or extend the capability of TB2J, please contact us! <mailhexu_AT_gmail_DOT_com>
```

### Comparing `TB2J-0.7.4rc3/TB2J/Jdownfolder.py` & `TB2J-0.7.5/TB2J/Jdownfolder.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,28 +16,29 @@
     for i in range(n):
         indn[i::n] += i
     return indn
 
 
 class JDownfolder():
 
-    def __init__(self, JR, Rlist, iM, iL, qmesh, is_collinear=True):
+    def __init__(self, JR, Rlist, iM, iL, qmesh, iso_only=False):
         self.JR = JR
         self.Rlist = Rlist
         self.nR = len(Rlist)
         self.nM = len(iM)
         self.nL = len(iL)
         self.nsite = self.nM + self.nL
         self.iM = iM
         self.iL = iL
         self.qmesh = qmesh
         self.qpts = monkhorst_pack(qmesh)
         self.nqpt = len(self.qpts)
         self.nMn = self.nM*3
         self.nLn = self.nL*3
+        self.iso_only=iso_only
 
     def get_Jq(self, q):
         Jq = np.zeros(self.JR[0].shape, dtype=complex)
         for iR, R in enumerate(self.Rlist):
             phase = np.exp(2.0j * np.pi * np.dot(q, R))
             Jq += self.JR[iR] * phase
         return Jq
@@ -65,18 +66,18 @@
         JML = J[np.ix_(self.iMn, self.iLn)]
         Jn = JMM - JML @ np.linalg.inv(JLL) @ JLM
         return Jn
 
 
 class JDownfolder_pickle():
 
-    def __init__(self, inpath, metals, ligands, outpath, qmesh=[7, 7, 7]):
+    def __init__(self, inpath, metals, ligands, outpath, qmesh=[7, 7, 7], iso_only=False):
         self.exc = SpinIO.load_pickle(path=inpath, fname="TB2J.pickle")
 
-        self.is_colinear = self.exc.dmi_ddict is None
+        self.iso_only = (self.exc.dmi_ddict is None) or iso_only
 
         self.metals = metals
         self.ligands = ligands
         self.outpath = outpath
 
         # read atomic structure
         self.atoms = self.exc.atoms
@@ -103,21 +104,21 @@
         self.nM = len(self.iM)
         self.nL = len(self.iL)
         self.nsite = self.nM + self.nL
 
     def _downfold(self):
         JR2 = self.exc.get_full_Jtensor_for_Rlist(asr=True)
         d = JDownfolder(JR2, self.exc.Rlist, iM=self.iM,
-                        iL=self.iL, qmesh=self.qmesh, is_collinear=self.is_colinear)
+                        iL=self.iL, qmesh=self.qmesh, iso_only=self.iso_only)
         Jd = d.get_JR()
 
         self._prepare_distance()
         self._prepare_index_spin()
         self.Jdict = {}
-        if self.is_colinear:
+        if self.iso_only:
             self.DMIdict = None
             self.Janidict = None
         else:
             self.DMIdict = {}
             self.Janidict = {}
 
         for iR, R in enumerate(d.Rlist):
@@ -126,23 +127,23 @@
                     if ispin >= 0 and jspin >= 0:
                         if not (tuple(R) == (0, 0, 0) and ispin == jspin):
                             # self interaction.
                             J33 = Jd[iR, ispin * 3:ispin * 3 + 3,
                                      jspin * 3:jspin * 3 + 3]
                             J, DMI, Jani = decompose_J_tensor(J33)
                             self.Jdict[(tuple(R), ispin, jspin)] = J
-                            if not self.is_colinear:
+                            if not self.iso_only:
                                 self.DMIdict[(tuple(R), ispin, jspin)] = DMI
                                 self.Janidict[(tuple(R), ispin, jspin)] = Jani
 
         io = SpinIO(atoms=self.atoms,
                     spinat=self.exc.spinat,
                     charges=self.exc.charges,
                     index_spin=self.index_spin,
-                    colinear=self.is_colinear,
+                    colinear=self.iso_only,
                     distance_dict=self.distance_dict,
                     exchange_Jdict=self.Jdict,
                     dmi_ddict=self.DMIdict,
                     Jani_dict=self.Janidict,
                     )
 
         io.write_all(self.outpath)
```

### Comparing `TB2J-0.7.4rc3/TB2J/Jtensor.py` & `TB2J-0.7.5/TB2J/Jtensor.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/Oiju.py` & `TB2J-0.7.5/TB2J/Oiju.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/Oiju_epc.py` & `TB2J-0.7.5/TB2J/Oiju_epc.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/citation.py` & `TB2J-0.7.5/TB2J/citation.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/contour.py` & `TB2J-0.7.5/TB2J/contour.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/epc.py` & `TB2J-0.7.5/TB2J/epc.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/exchange.py` & `TB2J-0.7.5/TB2J/exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             efermi,
             basis=None,
             magnetic_elements=[],
             include_orbs={},
             kmesh=[4, 4, 4],
             emin=-15,  # integration lower bound, relative to fermi energy
             # integration upper bound. Should be 0 (fermi energy). But DFT codes define Fermi energy in various ways.
-            emax=0.05,
+        emax=0.05,
             nz=100,
             # the delta in the (i delta) in green's function to prevent divergence
             height=0.5,
             nz1=150,  # grid from emin to emin+(i delta)
             nz2=300,  # grid from emin +(i delta) to emax+(i delta)
             nz3=150,  # grid from emax + (i delta) to emax
             exclude_orbs=[],  #
@@ -195,15 +195,25 @@
 
         # sanity check to see if some magnetic atom has no orbital.
         for iatom in self.ind_mag_atoms:
             if iatom not in self.orb_dict:
                 raise ValueError(
                     f"""Cannot find any orbital for atom {iatom}, which is supposed to be magnetic. Please check the Wannier functions."""
                 )
-
+        if not self._is_collinear:
+            for iatom, orb in self.orb_dict.items():
+                nsorb = len(self.orb_dict[iatom])
+                if and (nsorb % 2 != 0):
+                    raise ValueError(
+                        f"""The number of spin-orbitals for atom {iatom} is not even,
+{nsorb} spin-orbitals are found near this atom.
+which means the spin up/down does not have same number of orbitals. 
+This is often because the Wannier functions are wrongly defined,
+or badly localized. Please check the Wannier centers in the Wannier90 output file. 
+""")
         self._spin_dict = {}
         self._atom_dict = {}
         for ispin, iatom in enumerate(self.ind_mag_atoms):
             self._spin_dict[iatom] = ispin
             self._atom_dict[ispin] = iatom
 
         self._prepare_orb_mmat()
@@ -225,19 +235,23 @@
                     mmat, reduced_orbs = map_orbs_matrix(
                         orbs,
                         spinor=not (self._is_collinear),
                         include_only=None)
 
                 self.mmats[iatom] = mmat
                 self.orbital_names[iatom] = reduced_orbs
-                self.norb_reduced[iatom] = len(reduced_orbs) // 2
+                # Note that for siesta, spin up and spin down has same orb name.
+                # Therefor there is no nedd to /2
+                self.norb_reduced[iatom] = len(reduced_orbs)
         else:
             self.orbital_names = self.labels
             for iatom, orbs in self.labels.items():
-                self.norb_reduced[iatom] = len(orbs) // 2
+                # Note that for siesta, spin up and spin down has same orb name.
+                # thus //2
+                self.norb_reduced[iatom] = len(orbs)//2
 
     def ispin(self, iatom):
         return self._spin_dict[iatom]
 
     def iatom(self, ispin):
         return self._atom_dict[ispin]
 
@@ -648,25 +662,32 @@
         return AijR, AijR_orb, self.get_rho_e(rhoR)
 
     def save_AijR(self, AijRs, fname):
         result = dict(path=self.contour.path, AijRs=AijRs)
         with open(fname, 'wb') as myfile:
             pickle.dump(result, myfile)
 
+    def validate(self):
+        """
+        Do some sanity check before proceding.
+        """
+
     def calculate_all(self):
         """
         The top level.
         """
         print("Green's function Calculation started.")
 
         rhoRs = []
         AijRs = {}
 
         AijRs_orb = {}
 
+        self.validate()
+
         npole = len(self.contour.path)
         if self.np > 1:
             #executor = ProcessPool(nodes=self.np)
             #results = executor.map(self.get_AijR_rhoR, self.contour.path)
             results = p_map(self.get_AijR_rhoR,
                             self.contour.path,
                             num_cpus=self.np)
```

### Comparing `TB2J-0.7.4rc3/TB2J/exchangeCL2.py` & `TB2J-0.7.5/TB2J/exchangeCL2.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,21 +27,21 @@
         """
         self.tbmodel_up, self.tbmodel_dn = tbmodels
         self.backend_name = self.tbmodel_up.name
         self.Gup = TBGreen(self.tbmodel_up,
                            self.kmesh,
                            self.efermi,
                            use_cache=self._use_cache,
-                           #cache_path='TB2J_results/cache/spinup',
+                           # cache_path='TB2J_results/cache/spinup',
                            nproc=self.np)
         self.Gdn = TBGreen(self.tbmodel_dn,
                            self.kmesh,
                            self.efermi,
                            use_cache=self._use_cache,
-                           #cache_path='TB2J_results/cache/spindn',
+                           # cache_path='TB2J_results/cache/spindn',
                            nproc=self.np)
         self.norb = self.Gup.norb
         self.nbasis = self.Gup.nbasis + self.Gdn.nbasis
         self.rho_up_list = []
         self.rho_dn_list = []
         self.rho_up = np.zeros((self.norb, self.norb), dtype=float)
         self.rho_dn = np.zeros((self.norb, self.norb), dtype=float)
```

### Comparing `TB2J-0.7.4rc3/TB2J/exchange_pert.py` & `TB2J-0.7.5/TB2J/exchange_pert.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/exchange_qspace.py` & `TB2J-0.7.5/TB2J/exchange_qspace.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/external/p_tqdm.py` & `TB2J-0.7.5/TB2J/external/p_tqdm.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/gpaw_wrapper.py` & `TB2J-0.7.5/TB2J/gpaw_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/green.py` & `TB2J-0.7.5/TB2J/green.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,16 @@
             f"Writting wavefunctions and Hamiltonian in cache {self.cache_path}"
         )
 
     def clean_cache(self):
         if (self.cache_path is not None) and os.path.exists(self.cache_path):
             rmtree(self.cache_path)
 
-    def _prepare_eigen(self):
+
+    def _prepare_eigen(self, solve=True):
         """
         calculate eigen values and vectors for all kpts and save.
         Note that the convention 2 is used here, where the 
         phase factor is e^(ik.R), not e^(ik.(R+rj-ri))
         """
         nkpts = len(self.kpts)
         self.evals = np.zeros((nkpts, self.nbasis), dtype=float)
```

### Comparing `TB2J-0.7.4rc3/TB2J/greentest.py` & `TB2J-0.7.5/TB2J/greentest.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/io_exchange/io_exchange.py` & `TB2J-0.7.5/TB2J/io_exchange/io_exchange.py`

 * *Files 5% similar despite different names*

```diff
@@ -174,20 +174,14 @@
 """
         if description is not None:
             self.description += description
 
         self.orbital_names = orbital_names
         self.TB2J_version = __version__
 
-    def get_ispin(self, iatom):
-        return self.index_spin[iatom]
-
-    def get_iatom(self, ispin):
-        return self.ind_atoms[ispin]
-
     def _build_Rlist(self):
         Rset = set()
         ispin_set = set()
         for R, i, j in self.exchange_Jdict:
             Rset.add(R)
             ispin_set.add(i)
             ispin_set.add(j)
@@ -213,30 +207,33 @@
     def get_Jani(self, i, j, R):
         key = (tuple(R), i, j,)
         if self.Jani_dict is not None and key in self.Jani_dict:
             return self.Jani_dict[(tuple(R), i, j)]
         else:
             return None
 
-    def get_J_tensor(self, i, j, R):
-        Jtensor = combine_J_tensor(Jiso=self.get_J(i, j, R),
+    def get_J_tensor(self, i, j, R, iso_only=False):
+        if iso_only:
+            Jtensor= np.eye(3)*self.get_J(i, j, R)
+        else:
+            Jtensor = combine_J_tensor(Jiso=self.get_J(i, j, R),
                                    D=self.get_DMI(i, j, R),
                                    Jani=self.get_Jani(i, j, R))
         return(Jtensor)
 
     def get_full_Jtensor_for_one_R(self, R):
         n3 = self.nspin * 3
         Jmat = np.zeros((n3, n3), dtype=float)
         for i in range(self.nspin):
             for j in range(self.nspin):
                 Jmat[i * 3:i * 3 + 3,
                      j * 3:j * 3 + 3] = self.get_J_tensor(i, j, R)
         return Jmat
 
-    def get_full_Jtensor_for_Rlist(self, asr=False):
+    def get_full_Jtensor_for_Rlist(self, asr=False, iso_only=False):
         n3 = self.nspin * 3
         nR = len(self.Rlist)
         Jmat = np.zeros((nR, n3, n3), dtype=float)
         for iR, R in enumerate(self.Rlist):
             Jmat[iR] = self.get_full_Jtensor_for_one_R(R)
         if asr:
             iR0 = np.argmin(np.linalg.norm(self.Rlist, axis=1))
```

### Comparing `TB2J-0.7.4rc3/TB2J/io_exchange/io_multibinit.py` & `TB2J-0.7.5/TB2J/io_exchange/io_multibinit.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/io_exchange/io_tomsasd.py` & `TB2J-0.7.5/TB2J/io_exchange/io_tomsasd.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/io_exchange/io_txt.py` & `TB2J-0.7.5/TB2J/io_exchange/io_txt.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/io_exchange/io_uppasd.py` & `TB2J-0.7.5/TB2J/io_exchange/io_uppasd.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/io_exchange/io_vampire.py` & `TB2J-0.7.5/TB2J/io_exchange/io_vampire.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,20 +9,22 @@
     write_vampire_unitcell_file(cls, os.path.join(path, 'vampire.UCF'))
     write_vampire_mat_file(cls, os.path.join(path, 'vampire.mat'))
     write_vampire_inp_file(cls, os.path.join(path, 'input'))
 
 
 def write_vampire_unitcell_file(cls, fname):
     with open(fname, 'w') as myfile:
+        
+        cell = cls.atoms.get_cell().array
+        lattice_parameters = np.linalg.norm(cell, axis=-1)
         myfile.write("# Unit cell size (Angstrom):\n")
-        myfile.write("1 1 1\n")
+        np.savetxt(myfile, [lattice_parameters], fmt='%f')
         myfile.write("# Unit cell lattice vectors:\n")
-        for l in cls.atoms.get_cell():
-            myfile.write(" ".join([str(x) for x in l]))
-            myfile.write("\n")
+        np.savetxt(myfile, cell / lattice_parameters, fmt='%f')
+
         myfile.write("# Atoms\n")
         nspins = sum([1 if i > -1 else 0 for i in cls.index_spin])
         myfile.write("%s %s\n" % (nspins, nspins))
         natom = len(cls.atoms)
         for i in range(natom):
             text = ""
             id_spin = cls.index_spin[i]
```

### Comparing `TB2J-0.7.4rc3/TB2J/io_merge.py` & `TB2J-0.7.5/TB2J/io_merge.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/kpoints.py` & `TB2J-0.7.5/TB2J/kpoints.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/manager.py` & `TB2J-0.7.5/TB2J/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,19 +261,20 @@
 
     from packaging import version
     if version.parse(sisl.__version__) <= version.parse("0.10.0"):
         raise ImportError(
             f"sisl version is {sisl.__version__}, but should be larger than 0.10.0."
         )
     fdf = sisl.get_sile(fdf_fname)
+    geom = fdf.read_geometry()
     H = fdf.read_hamiltonian()
     if H.spin.is_colinear:
         print("Reading Siesta hamiltonian: colinear spin.")
-        tbmodel_up = SislWrapper(H, spin=0)
-        tbmodel_dn = SislWrapper(H, spin=1)
+        tbmodel_up = SislWrapper(H, spin=0, geom=geom)
+        tbmodel_dn = SislWrapper(H, spin=1, geom=geom)
         basis = dict(zip(tbmodel_up.orbs, list(range(tbmodel_up.norb))))
         print("Starting to calculate exchange.")
         description = f""" Input from collinear Siesta data.
  working directory: {os.getcwd()}
  fdf_fname: {fdf_fname}.
 \n"""
         exchange = ExchangeCL2(
@@ -298,15 +299,15 @@
         print(
             f"All calculation finsihed. The results are in {output_path} directory."
         )
 
     elif H.spin.is_colinear and False:
         print(
             "Reading Siesta hamiltonian: colinear spin. Treat as non-colinear. For testing only.")
-        tbmodel = SislWrapper(H, spin='merge')
+        tbmodel = SislWrapper(H, spin='merge', geom=geom)
         basis = dict(zip(tbmodel.orbs, list(range(tbmodel.nbasis))))
         print("Starting to calculate exchange.")
         description = f""" Input from collinear Siesta data.
  working directory: {os.getcwd()}
  fdf_fname: {fdf_fname}.
 \n"""
         exchange = ExchangeNCL(tbmodels=tbmodel,
@@ -331,15 +332,15 @@
         print(
             f"All calculation finsihed. The results are in {output_path} directory."
         )
 
     elif H.spin.is_spinorbit or H.spin.is_noncolinear:
 
         print("Reading Siesta hamiltonian: non-colinear spin.")
-        tbmodel = SislWrapper(H, spin=None)
+        tbmodel = SislWrapper(H, spin=None, geom=geom)
         basis = dict(zip(tbmodel.orbs, list(range(tbmodel.nbasis))))
         print("Starting to calculate exchange.")
         description = f""" Input from non-collinear Siesta data.
  working directory: {os.getcwd()}
  fdf_fname: {fdf_fname}.
 Warning: The DMI component parallel to the spin orientation, the Jani which has the component of that orientation should be disregarded
  e.g. if the spins are along z, the xz, yz, zz, zx, zy components and the z component of DMI.
```

### Comparing `TB2J-0.7.4rc3/TB2J/myTB.py` & `TB2J-0.7.5/TB2J/myTB.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             self._matrix = csr_matrix
         self.atoms = None
         self.R2kfactor = 2.0j * np.pi
         self.k2Rfactor = -2.0j * np.pi
         self.is_siesta = False
         self.is_orthogonal = True
 
-        self._name='Wannier'
+        self._name = 'Wannier'
 
     def set_atoms(self, atoms):
         self.atoms = atoms
 
     @property
     def nspin(self):
         return self._nspin
@@ -168,53 +168,53 @@
         """
         The hopping parameters, not including any onsite energy.
         """
         data = copy.deepcopy(self.data)
         np.fill_diagonal(data[(0, 0, 0)], 0.0)
         return data
 
-
     @staticmethod
     def read_from_wannier_dir(path,
                               prefix,
                               atoms=None,
                               nls=True,
                               groupby=None):
         """
         read tight binding model from a wannier function directory. 
         :param path: path
         :param prefix: prefix to the wannier files, often wannier90, or wannier90_up, or wannier90_dn for vasp.
         """
-        #tbmodel = Model.from_wannier_folder(
+        # tbmodel = Model.from_wannier_folder(
         #    folder=path, prefix=prefix)
         #m = MyTB.from_tbmodel(tbmodel)
 
         nbasis, data = parse_ham(fname=os.path.join(path, prefix + '_hr.dat'))
         xcart, _, _ = parse_xyz(fname=os.path.join(path, prefix +
                                                    '_centres.xyz'))
+        if atoms is None:
+            atoms = parse_atoms(os.path.join(path, prefix+'.win'))
         cell = atoms.get_cell()
         xred = cell.scaled_positions(xcart)
         if groupby == 'spin':
             norb = nbasis // 2
             xtmp = copy.deepcopy(xred)
             xred[::2] = xtmp[:norb]
             xred[1::2] = xtmp[norb:]
             for key, val in data.items():
                 dtmp = copy.deepcopy(val)
-                data[key][::2, ::2]   = dtmp[:norb, :norb]
-                data[key][::2, 1::2]  = dtmp[:norb, norb:]
-                data[key][1::2, ::2]  = dtmp[norb:, :norb]
+                data[key][::2, ::2] = dtmp[:norb, :norb]
+                data[key][::2, 1::2] = dtmp[:norb, norb:]
+                data[key][1::2, ::2] = dtmp[norb:, :norb]
                 data[key][1::2, 1::2] = dtmp[norb:, norb:]
         ind, positions = auto_assign_basis_name(xred, atoms)
         m = MyTB(nbasis=nbasis, data=data, positions=xred)
         nm = m.shift_position(positions)
         nm.set_atoms(atoms)
         return nm
 
-
     @staticmethod
     def load_banddownfolder(path,
                             prefix,
                             atoms=None,
                             nls=True,
                             groupby='spin'):
         from banddownfolder.scdm.lwf import LWF
@@ -222,15 +222,15 @@
         nbasis = lwf.nwann
         nspin = 1
         positions = lwf.wann_centers
         ndim = lwf.ndim
         H_mnR = defaultdict(lambda: np.zeros((nbasis, nbasis), dtype=complex))
 
         for iR, R in enumerate(lwf.Rlist):
-            R=tuple(R)
+            R = tuple(R)
             val = lwf.HwannR[iR]
             if np.linalg.norm(R) < 0.001:
                 H_mnR[R] = val/2.0
                 #H_mnR[R] -= np.diag(np.diag(val) / 2.0)
             else:
                 H_mnR[R] = val/2.0
         m = MyTB(nbasis,
@@ -286,15 +286,15 @@
         """
         nk = len(kpts)
         hams = np.zeros((nk, self.nbasis, self.nbasis), dtype=complex)
         evals = np.zeros((nk, self.nbasis), dtype=float)
         evecs = np.zeros((nk, self.nbasis, self.nbasis), dtype=complex)
         for ik, k in enumerate(kpts):
             hams[ik], S, evals[ik], evecs[ik] = self.HSE_k(tuple(k),
-                                                         convention=convention)
+                                                           convention=convention)
         return hams, None, evals, evecs
 
     def prepare_phase_rjri(self):
         """
         The matrix P: P(i, j) = r(j)-r(i)
         """
         self.rjminusri = self.xred[None, :, :] - self.xred[:, None, :]
@@ -442,15 +442,14 @@
         if self.atoms is not None:
             atom_numbers[:] = np.array(self.atoms.get_atomic_numbers())
             atom_xred[:] = np.array(
                 self.atoms.get_scaled_positions(wrap=False))
             atom_cell[:] = np.array(self.atoms.get_cell())
         root.close()
 
-
     @staticmethod
     def load_MyTB(fname):
         """
         Load from a netcdf file.
         :param fname: netcdf filename.
         :Returns: tight binding model.
         """
```

### Comparing `TB2J-0.7.4rc3/TB2J/orbmap.py` & `TB2J-0.7.5/TB2J/orbmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,13 +49,15 @@
 
 
 def test():
     odict = {0: ['3sZ1', '3sZ1', '4sZ1', '4sZ1', '4sZ2', '4sZ2', '3pyZ1', '3pyZ1', '3pzZ1', '3pzZ1', '3pxZ1', '3pxZ1', '3dxyZ1', '3dxyZ1', '3dyzZ1', '3dyzZ1', '3dz2Z1', '3dz2Z1', '3dxzZ1', '3dxzZ1', '3dx2-y2Z1', '3dx2-y2Z1', '3dxyZ2', '3dxyZ2', '3dyzZ2', '3dyzZ2', '3dz2Z2', '3dz2Z2', '3dxzZ2', '3dxzZ2', '3dx2-y2Z2', '3dx2-y2Z2', '4pyZ1P', '4pyZ1P', '4pzZ1P', '4pzZ1P', '4pxZ1P', '4pxZ1P'], 1: ['3sZ1', '3sZ1', '4sZ1', '4sZ1', '4sZ2', '4sZ2', '3pyZ1', '3pyZ1', '3pzZ1', '3pzZ1', '3pxZ1', '3pxZ1', '3dxyZ1', '3dxyZ1', '3dyzZ1', '3dyzZ1', '3dz2Z1', '3dz2Z1', '3dxzZ1', '3dxzZ1', '3dx2-y2Z1', '3dx2-y2Z1', '3dxyZ2', '3dxyZ2', '3dyzZ2', '3dyzZ2', '3dz2Z2', '3dz2Z2', '3dxzZ2', '3dxzZ2', '3dx2-y2Z2', '3dx2-y2Z2', '4pyZ1P', '4pyZ1P', '4pzZ1P', '4pzZ1P', '4pxZ1P', '4pxZ1P'], 2: ['5sZ1', '5sZ1', '5sZ2', '5sZ2', '5pyZ1', '5pyZ1', '5pzZ1', '5pzZ1', '5pxZ1', '5pxZ1', '5pyZ2', '5pyZ2', '5pzZ2', '5pzZ2', '5pxZ2', '5pxZ2', '5dxyZ1P', '5dxyZ1P', '5dyzZ1P', '5dyzZ1P', '5dz2Z1P', '5dz2Z1P', '5dxzZ1P', '5dxzZ1P', '5dx2-y2Z1P', '5dx2-y2Z1P'], 3: ['5sZ1', '5sZ1', '5sZ2', '5sZ2', '5pyZ1', '5pyZ1', '5pzZ1', '5pzZ1', '5pxZ1', '5pxZ1', '5pyZ2', '5pyZ2', '5pzZ2', '5pzZ2', '5pxZ2',
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             '5pxZ2', '5dxyZ1P', '5dxyZ1P', '5dyzZ1P', '5dyzZ1P', '5dz2Z1P', '5dz2Z1P', '5dxzZ1P', '5dxzZ1P', '5dx2-y2Z1P', '5dx2-y2Z1P'], 4: ['5sZ1', '5sZ1', '5sZ2', '5sZ2', '5pyZ1', '5pyZ1', '5pzZ1', '5pzZ1', '5pxZ1', '5pxZ1', '5pyZ2', '5pyZ2', '5pzZ2', '5pzZ2', '5pxZ2', '5pxZ2', '5dxyZ1P', '5dxyZ1P', '5dyzZ1P', '5dyzZ1P', '5dz2Z1P', '5dz2Z1P', '5dxzZ1P', '5dxzZ1P', '5dx2-y2Z1P', '5dx2-y2Z1P'], 5: ['5sZ1', '5sZ1', '5sZ2', '5sZ2', '5pyZ1', '5pyZ1', '5pzZ1', '5pzZ1', '5pxZ1', '5pxZ1', '5pyZ2', '5pyZ2', '5pzZ2', '5pzZ2', '5pxZ2', '5pxZ2', '5dxyZ1P', '5dxyZ1P', '5dyzZ1P', '5dyzZ1P', '5dz2Z1P', '5dz2Z1P', '5dxzZ1P', '5dxzZ1P', '5dx2-y2Z1P', '5dx2-y2Z1P'], 6: ['5sZ1', '5sZ1', '5sZ2', '5sZ2', '5pyZ1', '5pyZ1', '5pzZ1', '5pzZ1', '5pxZ1', '5pxZ1', '5pyZ2', '5pyZ2', '5pzZ2', '5pzZ2', '5pxZ2', '5pxZ2', '5dxyZ1P', '5dxyZ1P', '5dyzZ1P', '5dyzZ1P', '5dz2Z1P', '5dz2Z1P', '5dxzZ1P', '5dxzZ1P', '5dx2-y2Z1P', '5dx2-y2Z1P'], 7: ['5sZ1', '5sZ1', '5sZ2', '5sZ2', '5pyZ1', '5pyZ1', '5pzZ1', '5pzZ1', '5pxZ1', '5pxZ1', '5pyZ2', '5pyZ2', '5pzZ2', '5pzZ2', '5pxZ2', '5pxZ2', '5dxyZ1P', '5dxyZ1P', '5dyzZ1P', '5dyzZ1P', '5dz2Z1P', '5dz2Z1P', '5dxzZ1P', '5dxzZ1P', '5dx2-y2Z1P', '5dx2-y2Z1P']}
 
     olist = odict[0]
-    map_orbs_matrix(olist, spinor=True)
-    map_orbs_matrix(olist, spinor=True, include_only=['3d'])
+    r1=map_orbs_matrix(olist, spinor=True)
+    print(r1)
+    r2=map_orbs_matrix(olist, spinor=True, include_only=['3d'])
+    print(r2)
 
 
 if __name__=="__main__":
     test()
```

### Comparing `TB2J-0.7.4rc3/TB2J/pauli.py` & `TB2J-0.7.5/TB2J/pauli.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/pert.py` & `TB2J-0.7.5/TB2J/pert.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/plot.py` & `TB2J-0.7.5/TB2J/plot.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/rotate_atoms.py` & `TB2J-0.7.5/TB2J/rotate_atoms.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/sisl_wrapper.py` & `TB2J-0.7.5/TB2J/sisl_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,31 +4,34 @@
 from TB2J.utils import symbol_number
 from collections import defaultdict
 from scipy.linalg import eigh
 from TB2J.myTB import AbstractTB
 
 
 class SislWrapper(AbstractTB):
-    def __init__(self, sisl_hamiltonian, spin=None):
+    def __init__(self, sisl_hamiltonian, geom=None, spin=None):
         self.is_siesta = False
         self.is_orthogonal = False
         self.ham = sisl_hamiltonian
         # k2Rfactor : H(k) = \int_R H(R) * e^(k2Rfactor * k.R)
         self.R2kfactor = 2.0j * np.pi  #
         if spin == 'up':
             spin = 0
         elif spin == 'down':
             spin = 1
-        if spin not in [None, 0, 1, 'merge']:
+        if spin not in [None, 0, 1, 'merge', "fakemerge"]:
             raise ValueError("spin should be None/0/1, but is %s" % spin)
         self.spin = spin
         self.orbs = []
         self.orb_dict = defaultdict(lambda: [])
-        g = self.ham._geometry
-        _atoms = self.ham._geometry._atoms
+        if geom is None:
+            g = self.ham._geometry
+        else:
+            g=geom
+        _atoms = geom._atoms
         atomic_numbers = []
         self.positions = g.xyz
         self.cell = np.array(g.sc.cell)
         for ia, a in enumerate(_atoms):
             atomic_numbers.append(a.Z)
         self.atoms = Atoms(numbers=atomic_numbers,
                            cell=self.cell,
@@ -41,15 +44,16 @@
                     orb_names = [f"{symnum}|{x.name()}|up" for x in a.orbital]
                 except:
                     orb_names = [f"{symnum}|{x.name()}|up" for x in a.orbitals]
                 self.orbs += orb_names
                 self.orb_dict[ia] += orb_names
             self.norb = len(self.orbs)
             self.nbasis = self.norb
-        elif self.ham.spin.is_spinorbit or self.ham.spin.is_noncolinear or self.spin == 'merge':
+        elif (self.ham.spin.is_spinorbit or self.ham.spin.is_noncolinear 
+                or self.spin == 'merge' or self.spin == "fakemerge"):
             for ia, a in enumerate(_atoms):
                 symnum = sdict[ia]
                 orb_names = []
                 for x in a.orbitals: 
                     for spin in {'up', 'down'}:
                         orb_names.append(f"{symnum}|{x.name()}|{spin}")
                 self.orbs += orb_names
@@ -90,14 +94,27 @@
             evals = np.zeros(self.nbasis, dtype=float)
             evecs = np.zeros((self.nbasis, self.nbasis), dtype=complex)
             evals[::2] = evals0
             evals[1::2] = evals1
             evecs[::2, ::2] = evecs0
             evecs[1::2, 1::2] = evecs1
 
+        elif self.spin == "fakemerge":
+            evals0, evecs0 = self.ham.eigh(k=k,
+                                           eigvals_only=False,
+                                           gauge=gauge)
+            evals1, evecs1 = self.ham.eigh(k=k,
+                                           eigvals_only=False,
+                                           gauge=gauge)
+            evals = np.zeros(self.nbasis, dtype=float)
+            evecs = np.zeros((self.nbasis, self.nbasis), dtype=complex)
+            evals[::2] = evals0
+            evals[1::2] = evals1
+            evecs[::2, ::2] = evecs0
+            evecs[1::2, 1::2] = evecs1
         return evals, evecs
 
     def Hk(self, k, convention=2):
         if convention == 1:
             gauge = 'r'
         elif convention == 2:
             gauge = 'R'
@@ -111,14 +128,22 @@
                                                     spin=0,
                                                     gauge=gauge,
                                                     format='dense')
             H[1::2, 1::2] = self.ham.Hk(k,
                                                     spin=1,
                                                     gauge=gauge,
                                                     format='dense')
+        elif self.spin == "fakemerge":
+            H = np.zeros((self.nbasis, self.nbasis), dtype='complex')
+            H[::2, ::2] = self.ham.Hk(k,
+                                                    gauge=gauge,
+                                                    format='dense')
+            H[1::2, 1::2] = self.ham.Hk(k,
+                                                    gauge=gauge,
+                                                    format='dense')
         return H
 
     def eigen(self, k, convention=2):
         return self.solve(k)
 
     def gen_ham(self, k, convention=2):
         return self.Hk(k, convention=convention)
@@ -129,15 +154,15 @@
         elif convention == 2:
             pass
         S0 = self.ham.Sk(k, gauge='R', format='dense')
         if self.spin is None:
             S = S0
         elif self.spin in [0, 1]:
             S = S0
-        elif self.spin == 'merge':
+        elif self.spin == 'merge' or self.spin == "fakemerge":
             S = np.zeros((self.nbasis, self.nbasis), dtype='complex')
             S[::2, ::2] = S0
             S[1::2, 1::2] = S0
         return S
 
     def solve_all(self, kpts, orth=False):
         evals = []
@@ -156,15 +181,16 @@
         return np.array(evals, dtype=float), np.array(evecs,
                                                       dtype=complex,
                                                       order='C')
 
     def HSE_k(self, k,convention=2):
         Hk = self.Hk(k, convention=convention)
         Sk = self.Sk(k, convention=convention)
-        evalue, evec = self.solve(k, convention=convention)
+        evalue, evec = eigh(Hk, Sk)
+        #evalue, evec = self.solve(k, convention=convention)
         return Hk, Sk, evalue, evec
 
 
     def HS_and_eigen(self, kpts, convention=2):
         nkpts = len(kpts)
         evals = np.zeros((nkpts, self.nbasis), dtype=float)
         self.nkpts=nkpts
```

### Comparing `TB2J-0.7.4rc3/TB2J/spinham/base_parser.py` & `TB2J-0.7.5/TB2J/spinham/base_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/spinham/constants.py` & `TB2J-0.7.5/TB2J/spinham/constants.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/spinham/hamiltonian.py` & `TB2J-0.7.5/TB2J/spinham/hamiltonian.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         return self.pos
 
     def _map_to_magnetic_only(self):
         """
         select the sites with spin and re-index.
         """
         ms = np.linalg.norm(self._spin, axis=1)
-        self.magsites = np.where(ms > 0.00001 * mu_B)[0]
+        self.magsites = np.where(ms > -0.00001 * mu_B)[0]
         self.ms = ms[self.magsites]
         S = self._spin[self.magsites]
         self.nspin = len(S)
         # self.S = np.array(
         #    [S[i] / self.ms[i] for i in range(self.nspin)],
         #    dtype='float64')
         self.s = S / self.ms[:, None]
```

### Comparing `TB2J-0.7.4rc3/TB2J/spinham/hamiltonian_terms.py` & `TB2J-0.7.5/TB2J/spinham/hamiltonian_terms.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/spinham/plot.py` & `TB2J-0.7.5/TB2J/spinham/plot.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/spinham/qsolver.py` & `TB2J-0.7.5/TB2J/spinham/qsolver.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 #!/usr/bin/env python
 import math
 import numpy as np
 import scipy.linalg as linalg
 
+
 class QSolver(object):
     def __init__(self, hamiltonian):
         self.ham = hamiltonian
         self.nspin = self.ham.nspin
         M = linalg.norm(self.ham.spinat, axis=1)
-        self.M_mat=np.kron(np.sqrt(np.einsum('i,j->ij', M, M)), np.ones((3,3)))
-        self.Eref=None
+        self.M_mat = np.kron(
+            np.sqrt(np.einsum('i,j->ij', M, M)), np.ones((3, 3)))
+        self.Eref = None
 
     def get_Eref(self):
         mat = np.zeros((3 * self.nspin, 3 * self.nspin), dtype=complex)
         for key, val in self.ham.get_total_hessian_ijR().items():
             i, j, R = key
             mat[i * 3:i * 3 + 3, j * 3:j * 3 + 3] -= val
-        mat=mat*4.0/self.M_mat
-        SZ=np.zeros(self.nspin*3,dtype=float)
-        SZ[2::3]=1.0
-        SZ/=np.linalg.norm(SZ)
-        self.Eref=np.dot(SZ, np.dot(mat, SZ)).real
+        mat = mat*4.0/self.M_mat
+        SZ = np.zeros(self.nspin*3, dtype=float)
+        SZ[2::3] = 1.0
+        SZ /= np.linalg.norm(SZ)
+        self.Eref = np.dot(SZ, np.dot(mat, SZ)).real
         return self.Eref
 
     def solve_k(self, kpt, eigen_vectors=True, Jq=False):
         if self.Eref is None and not Jq:
             self.get_Eref()
         mat = np.zeros((3 * self.nspin, 3 * self.nspin), dtype=complex)
         for key, val in self.ham.get_total_hessian_ijR().items():
             i, j, R = key
             mat[i * 3:i * 3 + 3, j * 3:j * 3 + 3] -= val * np.exp(
-               2.0j * math.pi * np.dot(kpt, R))
+                2.0j * math.pi * np.dot(kpt, R))
         if not Jq:
-            mat=mat*4.0/self.M_mat
+            mat = mat*4.0/self.M_mat
         if eigen_vectors:
             evals, evecs = linalg.eigh(mat)
-            evals=np.real(evals)
+            evals = np.real(evals)
             if not Jq:
-                evals-=self.Eref
+                evals -= self.Eref
             return evals, evecs
         else:
             evals = np.linalg.eigvalsh(mat)
             if not Jq:
-                evals-=self.Eref
+                evals -= self.Eref
             return evals
 
     def solve_all(self, kpts, eigen_vectors=True, Jq=False):
         eval_list = []
         evec_list = []
         if eigen_vectors:
             for kpt in kpts:
```

### Comparing `TB2J-0.7.4rc3/TB2J/spinham/spin_api.py` & `TB2J-0.7.5/TB2J/spinham/spin_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/spinham/spin_xml.py` & `TB2J-0.7.5/TB2J/spinham/spin_xml.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/spinham/supercell.py` & `TB2J-0.7.5/TB2J/spinham/supercell.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/utest.py` & `TB2J-0.7.5/TB2J/utest.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/utils.py` & `TB2J-0.7.5/TB2J/utils.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/TB2J/wannier/w90_parser.py` & `TB2J-0.7.5/TB2J/wannier/w90_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 from ase.atoms import Atoms
 from ase.units import Angstrom, Bohr
 
 unit_dict = {'ANG': Angstrom, 'BOHR': Bohr}
 
 
 def parse_xyz(fname):
+    """
+    wannier90 xyz file parser.
+    
+    :param fname: relative or absolute path to the xyz file.  str.
+    """
     atoms = read(fname)
     symbols = atoms.get_chemical_symbols()
     pos = atoms.get_positions()
     wann_pos = []
     atoms_pos = []
     atoms_symbols = []
     for s, x in zip(symbols, pos):
@@ -23,15 +28,17 @@
             atoms_symbols.append(s)
             atoms_pos.append(x)
     return np.array(wann_pos), atoms_symbols, np.array(atoms_pos)
 
 
 def parse_ham(fname='wannier90_hr.dat', cutoff=None):
     """
-    wannier90 hr file phaser.
+    wannier90 hr file parser.
+    
+    :param fname: relative or absolute path to the hamiltonian file.  str.
 
     :param cutoff: the energy cutoff.  None | number | list (of Emin, Emax).
     """
     with open(fname, 'r') as myfile:
         lines = myfile.readlines()
     n_wann = int(lines[1].strip())
     n_R = int(lines[2].strip())
@@ -58,14 +65,19 @@
                 H_mnR[R][m, n] = val / 2.0
         else:
             H_mnR[R][m, n] = val / 2.0
     return n_wann, H_mnR
 
 
 def parse_cell(fname, unit=Angstrom):
+    """
+    wannier90 hr cell parser.
+    
+    :param fname: relative or absolute path to the file.  str.
+    """
 
     uc_regex = re.compile(
         r'BEGIN\s+UNIT_CELL_CART\s+'
         r'(?P<units>BOHR|ANG)?'
         r'(?P<cell>.+)'
         r'END\s+UNIT_CELL_CART\s+', re.VERBOSE | re.IGNORECASE | re.DOTALL)
     with open(fname) as myfile:
@@ -81,14 +93,19 @@
     else:
         factor = Angstrom
     cell = cell * factor / unit
     return cell
 
 
 def parse_atoms(fname):
+    """
+    wannier90 hr atoms parser.
+    
+    :param fname: relative or absolute path to the file.  str.
+    """
     cell = parse_cell(fname)
     atoms_regex = re.compile(
         r'BEGIN\s+ATOMS_(?P<suffix>(FRAC)|(CART))\s+'
         r'(?P<units>BOHR|ANG)?'
         r'(?P<atoms>.+)'
         r'END\s+ATOMS_(?P=suffix)\s+', re.VERBOSE | re.IGNORECASE | re.DOTALL)
```

### Comparing `TB2J-0.7.4rc3/TB2J.egg-info/PKG-INFO` & `TB2J-0.7.5/TB2J.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TB2J
-Version: 0.7.4rc3
+Version: 0.7.5
 Summary: TB2J: First principle to Heisenberg exchange J using tight-binding Green function method
 Home-page: UNKNOWN
 Author: Xu He
 Author-email: mailhexu@gmail.com
 License: BSD-2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `TB2J-0.7.4rc3/TB2J.egg-info/SOURCES.txt` & `TB2J-0.7.5/TB2J.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 TB2J/Jdownfolder.py
 TB2J/Jtensor.py
 TB2J/Oiju.py
 TB2J/Oiju_epc.py
 TB2J/__init__.py
 TB2J/citation.py
 TB2J/contour.py
-TB2J/cut_cell.py
 TB2J/epc.py
 TB2J/exchange.py
 TB2J/exchangeCL2.py
 TB2J/exchange_pert.py
 TB2J/exchange_qspace.py
 TB2J/gpaw_wrapper.py
 TB2J/green.py
@@ -23,15 +22,14 @@
 TB2J/myTB.py
 TB2J/orbmap.py
 TB2J/pauli.py
 TB2J/pert.py
 TB2J/plot.py
 TB2J/rotate_atoms.py
 TB2J/sisl_wrapper.py
-TB2J/supercell.py
 TB2J/utest.py
 TB2J/utils.py
 TB2J/versioninfo.py
 TB2J.egg-info/PKG-INFO
 TB2J.egg-info/SOURCES.txt
 TB2J.egg-info/dependency_links.txt
 TB2J.egg-info/requires.txt
```

### Comparing `TB2J-0.7.4rc3/scripts/TB2J_downfold.py` & `TB2J-0.7.5/scripts/TB2J_downfold.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,22 +34,37 @@
     parser.add_argument("--ligands",
                         "-l",
                         type=str,
                         help='List of ligand elements',
                         nargs='+',
                         default=[])
 
+    parser.add_argument('--qmesh',
+                        help='kmesh in the format of kx ky kz',
+                        type=int,
+                        nargs='*',
+                        default=[5, 5, 5])
+
+    parser.add_argument(
+        '--iso_only',
+        help="whether to downfold only the isotropic part. The other parts will be neglected.",
+        action='store_true',
+        default=False)
+
     args = parser.parse_args()
 
     if len(args.metals) == []:
         print("List of magnetic cation elements cannot be empty")
 
     if len(args.ligands) == []:
         print("List of ligand elements cannot be empty")
 
+
     JDownfolder_pickle(inpath=args.inpath,
                        metals=args.metals,
                        ligands=args.ligands,
-                       outpath=args.outpath)
+                       outpath=args.outpath,
+                       qmesh=args.qmesh,
+                       iso_only=args.iso_only)
 
 
 main()
```

### Comparing `TB2J-0.7.4rc3/scripts/TB2J_eigen.py` & `TB2J-0.7.5/scripts/TB2J_eigen.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         help='qmesh in the format of kx ky kz. Monkhorst pack or Gamma-centered.',
         type=int,
         nargs='*',
         default=[8, 8, 8])
 
     parser.add_argument(
         '--gamma',
-        help="whether shift the qpoint grid to  Gamma-centered. Default: True",
+        help="whether shift the qpoint grid to  Gamma-centered. Default: False",
         action='store_true',
         default=True)
 
     parser.add_argument(
         "--output_fname",
         type=str,
         help='The file name of the output. Default: eigenJq.txt',
```

### Comparing `TB2J-0.7.4rc3/scripts/TB2J_magnon.py` & `TB2J-0.7.5/scripts/TB2J_magnon.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/scripts/TB2J_merge.py` & `TB2J-0.7.5/scripts/TB2J_merge.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,12 +20,18 @@
     parser.add_argument(
         '--type',
         '-T',
         type=str,
         help=
         'The type of calculations, either structure of spin, meaning that the three calculations are done by rotating the structure/spin. '
     )
+    parser.add_argument(
+        "--output_path",
+        help="The path of the output directory, default is TB2J_results",
+        type=str,
+        default="TB2J_results")
+
     args = parser.parse_args()
-    merge(*(args.directories), args.type.strip().lower())
+    merge(*(args.directories), args.type.strip().lower(), path=args.output_path)
 
 
 main()
```

### Comparing `TB2J-0.7.4rc3/scripts/TB2J_rotate.py` & `TB2J-0.7.5/scripts/TB2J_rotate.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/scripts/siesta2J.py` & `TB2J-0.7.5/scripts/siesta2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/scripts/wann2J.py` & `TB2J-0.7.5/scripts/wann2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc3/setup.py` & `TB2J-0.7.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
-__version__ = "0.7.4.rc3"
+__version__ = "0.7.5"
 
 long_description = """TB2J is a Python package aimed to compute automatically the magnetic interactions (superexchange  and Dzyaloshinskii-Moriya) between atoms of magnetic crystals from DFT Hamiltonian based on Wannier functions or Linear combination of atomic orbitals. It uses the Green's function method and take the local rigid spin rotation as a perturbation. The package can take the output from Wannier90, which is interfaced with many density functional theory codes or from codes based on localised orbitals. A minimal user input is needed, which allows for an easily integration into a high-throughput workflows. """
 
 setup(
     name='TB2J',
     version=__version__,
     description='TB2J: First principle to Heisenberg exchange J using tight-binding Green function method',
```

