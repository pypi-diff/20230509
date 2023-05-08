# Comparing `tmp/Lattice-Graph-Manipulation-0.1.1.tar.gz` & `tmp/Lattice-Graph-Manipulation-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lattice-Graph-Manipulation-0.1.1.tar", last modified: Mon Apr 17 08:27:28 2023, max compression
+gzip compressed data, was "Lattice-Graph-Manipulation-1.0.0.tar", last modified: Mon May  8 22:55:19 2023, max compression
```

## Comparing `Lattice-Graph-Manipulation-0.1.1.tar` & `Lattice-Graph-Manipulation-1.0.0.tar`

### file list

```diff
@@ -1,36 +1,56 @@
--rw-r--r--   0        0        0     1070 2023-02-20 16:18:52.473641 Lattice-Graph-Manipulation-0.1.1/LICENSE
--rw-r--r--   0        0        0     3643 2023-04-16 21:36:33.181824 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/163d539f-a1ca-4026-8f96-8f2f84456739.gv
--rw-r--r--   0        0        0     7806 2023-04-16 21:36:33.208492 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/163d539f-a1ca-4026-8f96-8f2f84456739.gv.pdf
--rw-r--r--   0        0        0      528 2023-04-16 21:39:55.546127 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/6ea664e2-56ad-4b5e-bd5c-c8663a7f834a.gv
--rw-r--r--   0        0        0     6413 2023-04-16 21:39:55.562795 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/6ea664e2-56ad-4b5e-bd5c-c8663a7f834a.gv.pdf
--rw-r--r--   0        0        0     3643 2023-04-16 21:39:26.018518 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/8f764c44-1ca9-4850-89e6-09fcd00c950c.gv
--rw-r--r--   0        0        0     7811 2023-04-16 21:39:26.038519 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/8f764c44-1ca9-4850-89e6-09fcd00c950c.gv.pdf
--rw-r--r--   0        0        0      287 2023-04-16 23:48:35.740878 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/9276b4d9-fa93-4e2b-aea7-7282778d6a73.gv
--rw-r--r--   0        0        0     4730 2023-04-16 23:48:35.764212 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/9276b4d9-fa93-4e2b-aea7-7282778d6a73.gv.pdf
--rw-r--r--   0        0        0      603 2023-04-16 21:35:09.825570 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/Digraph.gv
--rw-r--r--   0        0        0     6440 2023-04-16 21:35:09.848903 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/Digraph.gv.pdf
--rw-r--r--   0        0        0        0 2023-04-16 21:00:24.727352 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/__init__.py
--rw-r--r--   0        0        0      642 2023-04-16 21:36:33.148489 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/a1b83602-e030-4c11-82dc-8edcbb00694f.gv
--rw-r--r--   0        0        0     6435 2023-04-16 21:36:33.175157 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/a1b83602-e030-4c11-82dc-8edcbb00694f.gv.pdf
--rw-r--r--   0        0        0      528 2023-04-16 21:39:46.689183 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/a4bdeb66-f55f-4582-912b-f274819c8137.gv
--rw-r--r--   0        0        0     6403 2023-04-16 21:39:46.709184 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/a4bdeb66-f55f-4582-912b-f274819c8137.gv.pdf
--rw-r--r--   0        0        0      642 2023-04-16 21:39:55.566128 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/c0e68ed3-17db-4d9e-a220-13127da2d063.gv
--rw-r--r--   0        0        0     6439 2023-04-16 21:39:55.586129 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/c0e68ed3-17db-4d9e-a220-13127da2d063.gv.pdf
--rw-r--r--   0        0        0      642 2023-04-16 21:39:25.991851 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/c2cbb9a6-d6bc-4cc9-a222-fdf426574881.gv
--rw-r--r--   0        0        0     6445 2023-04-16 21:39:26.015185 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/c2cbb9a6-d6bc-4cc9-a222-fdf426574881.gv.pdf
--rw-r--r--   0        0        0     3643 2023-04-16 21:39:55.589462 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/e9eaa6c8-c0d8-4f0e-a972-5c6dbcb1b847.gv
--rw-r--r--   0        0        0     7805 2023-04-16 21:39:55.609463 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/e9eaa6c8-c0d8-4f0e-a972-5c6dbcb1b847.gv.pdf
--rw-r--r--   0        0        0     1055 2023-04-16 23:49:48.851041 Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/simple_examples.py
--rw-r--r--   0        0        0        9 2023-02-20 16:18:52.473641 Lattice-Graph-Manipulation-0.1.1/README.md
--rw-r--r--   0        0        0       61 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/__init__.py
--rw-r--r--   0        0        0       99 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/edge/__init__.py
--rw-r--r--   0        0        0      569 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/edge/edge.py
--rw-r--r--   0        0        0      440 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/edge/traversaledge.py
--rw-r--r--   0        0        0      114 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/graph/__init__.py
--rw-r--r--   0        0        0     1615 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/graph/bbtree.py
--rw-r--r--   0        0        0     3883 2023-04-16 21:39:25.921848 Lattice-Graph-Manipulation-0.1.1/lattice/graph/graph.py
--rw-r--r--   0        0        0      872 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/graph/tree.py
--rw-r--r--   0        0        0       43 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/node/__init__.py
--rw-r--r--   0        0        0      875 2023-04-16 21:00:24.730686 Lattice-Graph-Manipulation-0.1.1/lattice/node/node.py
--rw-r--r--   0        0        0      368 2023-04-17 08:27:21.116437 Lattice-Graph-Manipulation-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      196 1970-01-01 00:00:00.000000 Lattice-Graph-Manipulation-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-30 13:12:10.136468 Lattice-Graph-Manipulation-1.0.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/__init__.py
+-rw-r--r--   0        0        0      639 2023-05-07 00:22:21.936580 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/bb_tree.py
+-rw-r--r--   0        0        0     1368 2023-05-05 22:09:45.090958 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv
+-rw-r--r--   0        0        0     5573 2023-05-05 22:09:45.107624 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv.pdf
+-rw-r--r--   0        0        0     4236 2023-05-05 22:01:27.915042 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv
+-rw-r--r--   0        0        0     7654 2023-05-05 22:01:27.935042 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv.pdf
+-rw-r--r--   0        0        0     1368 2023-05-05 21:59:43.450219 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv
+-rw-r--r--   0        0        0     5567 2023-05-05 21:59:43.470219 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv.pdf
+-rw-r--r--   0        0        0     4236 2023-05-05 22:02:54.341480 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv
+-rw-r--r--   0        0        0     7750 2023-05-05 22:02:54.361480 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv.pdf
+-rw-r--r--   0        0        0     4236 2023-05-05 22:04:13.795053 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv
+-rw-r--r--   0        0        0     7593 2023-05-05 22:04:13.815054 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv.pdf
+-rw-r--r--   0        0        0     7905 2023-05-07 00:23:54.513172 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv
+-rw-r--r--   0        0        0     9268 2023-05-07 00:23:54.536505 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv.pdf
+-rw-r--r--   0        0        0     7905 2023-05-07 00:19:22.396730 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv
+-rw-r--r--   0        0        0     9201 2023-05-07 00:19:22.426730 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv.pdf
+-rw-r--r--   0        0        0     4236 2023-05-05 22:02:27.888198 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv
+-rw-r--r--   0        0        0     7617 2023-05-05 22:02:27.911531 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv.pdf
+-rw-r--r--   0        0        0     7905 2023-05-07 00:36:00.902560 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv
+-rw-r--r--   0        0        0     9214 2023-05-07 00:36:00.925894 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv.pdf
+-rw-r--r--   0        0        0     5352 2023-05-05 22:10:28.170815 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv
+-rw-r--r--   0        0        0     7753 2023-05-05 22:10:28.194148 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv.pdf
+-rw-r--r--   0        0        0     7905 2023-05-05 22:10:58.647394 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv
+-rw-r--r--   0        0        0     9267 2023-05-05 22:10:58.670728 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv.pdf
+-rw-r--r--   0        0        0     2304 2023-05-07 00:23:41.253183 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv
+-rw-r--r--   0        0        0     6086 2023-05-07 00:23:41.273183 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv.pdf
+-rw-r--r--   0        0        0      451 2023-05-05 16:12:08.031549 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/b68224e8-ee0f-43bd-ad54-cbb0bc805f8e.gv
+-rw-r--r--   0        0        0     6700 2023-05-05 16:12:08.054882 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/b68224e8-ee0f-43bd-ad54-cbb0bc805f8e.gv.pdf
+-rw-r--r--   0        0        0     7905 2023-05-07 00:34:13.555984 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv
+-rw-r--r--   0        0        0     9276 2023-05-07 00:34:13.579317 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv.pdf
+-rw-r--r--   0        0        0      451 2023-05-07 00:20:50.539988 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/c04b2718-239f-4811-8f73-d78111718784.gv
+-rw-r--r--   0        0        0     6728 2023-05-07 00:20:50.559988 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/c04b2718-239f-4811-8f73-d78111718784.gv.pdf
+-rw-r--r--   0        0        0     2364 2023-05-05 22:01:03.491857 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv
+-rw-r--r--   0        0        0     6142 2023-05-05 22:01:03.511857 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv.pdf
+-rw-r--r--   0        0        0     1368 2023-05-05 21:58:56.455608 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv
+-rw-r--r--   0        0        0     5809 2023-05-05 21:58:56.478942 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv.pdf
+-rw-r--r--   0        0        0      541 2023-05-07 00:36:08.819221 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv
+-rw-r--r--   0        0        0     6146 2023-05-07 00:36:08.852554 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv.pdf
+-rw-r--r--   0        0        0     1045 2023-05-05 22:10:58.580728 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/grid_example.py
+-rw-r--r--   0        0        0      648 2023-05-01 21:34:44.057078 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/simple_examples.py
+-rw-r--r--   0        0        0      413 2023-05-07 00:36:00.802560 Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/simple_graph.py
+-rw-r--r--   0        0        0        9 2023-04-30 13:12:10.136468 Lattice-Graph-Manipulation-1.0.0/README.md
+-rw-r--r--   0        0        0       61 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.0.0/lattice/__init__.py
+-rw-r--r--   0        0        0      148 2023-05-04 09:15:27.080595 Lattice-Graph-Manipulation-1.0.0/lattice/edge/__init__.py
+-rw-r--r--   0        0        0      584 2023-05-01 21:31:00.683002 Lattice-Graph-Manipulation-1.0.0/lattice/edge/edge.py
+-rw-r--r--   0        0        0      440 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.0.0/lattice/edge/traversaledge.py
+-rw-r--r--   0        0        0      358 2023-05-04 09:11:10.130523 Lattice-Graph-Manipulation-1.0.0/lattice/edge/visualedge.py
+-rw-r--r--   0        0        0      114 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.0.0/lattice/graph/__init__.py
+-rw-r--r--   0        0        0     1558 2023-05-01 21:00:58.830421 Lattice-Graph-Manipulation-1.0.0/lattice/graph/bbtree.py
+-rw-r--r--   0        0        0     3979 2023-05-07 00:34:34.319299 Lattice-Graph-Manipulation-1.0.0/lattice/graph/graph.py
+-rw-r--r--   0        0        0      829 2023-05-05 12:55:46.790589 Lattice-Graph-Manipulation-1.0.0/lattice/graph/tree.py
+-rw-r--r--   0        0        0       43 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.0.0/lattice/node/__init__.py
+-rw-r--r--   0        0        0     1151 2023-05-05 21:58:39.058953 Lattice-Graph-Manipulation-1.0.0/lattice/node/node.py
+-rw-r--r--   0        0        0      368 2023-05-08 22:54:49.033681 Lattice-Graph-Manipulation-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      196 1970-01-01 00:00:00.000000 Lattice-Graph-Manipulation-1.0.0/PKG-INFO
```

### Comparing `Lattice-Graph-Manipulation-0.1.1/LICENSE` & `Lattice-Graph-Manipulation-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/163d539f-a1ca-4026-8f96-8f2f84456739.gv.pdf` & `Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 27% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,43 +1,51 @@
 0
 
-4
+1
+
+1
 
-19
+2
+
+2
 
 1
 
 2
 
+2
+
+2
+
 3
 
-6
+3
 
-9
+3
 
-10
+3
 
-8
+3
 
-7
+4
 
-13
+4
 
-20
+4
 
-17
+4
 
-18
+4
 
-15
+3
 
-16
+4
 
-5
+3
 
-14
+4
 
-11
+4
 
-12
+4
```

### Comparing `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/8f764c44-1ca9-4850-89e6-09fcd00c950c.gv.pdf` & `Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 21% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,43 +1,51 @@
 0
 
-6
+1
 
-13
+2
 
-14
+3
 
-11
+4
 
-2
+1
 
 1
 
-5
+2
+
+3
 
 4
 
+2
+
+2
+
+2
+
 3
 
-12
+4
 
-9
+3
 
-10
+3
 
-8
+3
 
-7
+3
 
-20
+4
 
-19
+4
 
-17
+4
 
-18
+4
 
-15
+4
 
-16
+4
```

### Comparing `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/Digraph.gv.pdf` & `Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/b68224e8-ee0f-43bd-ad54-cbb0bc805f8e.gv.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 25% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,9 +1,7 @@
-mynode
-5
-a
-5
-b
-5
-c
+1
+first
+2
+second
+3
```

### Comparing `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/a1b83602-e030-4c11-82dc-8edcbb00694f.gv.pdf` & `Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 22% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,9 +1,27 @@
-mynode
-5
-a
-5
-b
-5
-c
+0
+
+1
+
+1
+
+1
+
+2
+
+2
+
+2
+
+3
+
+3
+
+3
+
+4
+
+4
+
+4
```

### Comparing `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/a4bdeb66-f55f-4582-912b-f274819c8137.gv.pdf` & `Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 23% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,9 +1,19 @@
-mynode
-5
-a
-5
-b
+0
 
-c
+1
+
+3
+
+2
+
+4
+
+1
+
+4
+
+2
+
+3
```

### Comparing `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/c0e68ed3-17db-4d9e-a220-13127da2d063.gv.pdf` & `Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 19% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,9 +1,7 @@
-mynode
-5
-a
-5
-b
-5
-c
+1
+
+2
+second
+3
```

### Comparing `Lattice-Graph-Manipulation-0.1.1/Lattice_Scripts/c2cbb9a6-d6bc-4cc9-a222-fdf426574881.gv.pdf` & `Lattice-Graph-Manipulation-1.0.0/Lattice_Scripts/dot_output/c04b2718-239f-4811-8f73-d78111718784.gv.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 21% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,9 +1,7 @@
-mynode
-5
-a
-5
-b
-5
-c
+1
+first
+2
+second
+3
```

### Comparing `Lattice-Graph-Manipulation-0.1.1/lattice/edge/edge.py` & `Lattice-Graph-Manipulation-1.0.0/lattice/edge/edge.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     """
     Default edge, requires a source and a destination
     We define a cost and a label, attempting to access them will return nothing
     """
     _data: Any
     _label: str
 
-    def __init__(self):
-        self._data = ""
-        self._label = ""
+    def __init__(self, label=''):
+        self._data = None
+        self._label = label
 
     def get_data(self) -> Any:
         """Get the data we have stored in the edge"""
         return self._data
 
     def get_label(self) -> str:
         """Return the label assigned to this edge"""
```

### Comparing `Lattice-Graph-Manipulation-0.1.1/lattice/graph/bbtree.py` & `Lattice-Graph-Manipulation-1.0.0/lattice/graph/bbtree.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 
 class BBTree(Tree):
     """
     Edges are inconsequential
     TODO: Current implementation creates an unbalanced tree, will probably have to look into a more clever solution for this
     """
     _frontier = []  # frontier queue defines which leaves should be added to next
-    _default_display_data = True  # binary tree nodes don't have labels, so we display the values instead
 
     def __init__(self, root_node):
-        root_node = root_node.copy()
+        root_node = root_node.copy(label=root_node.get_label())
         super().__init__(root_node, copy=False)
         self._frontier.append(root_node)
         self._frontier.append(root_node)
 
     def add_nodes(self, *nodes):
         """
         Allows adding multiple nodes at a time
@@ -29,15 +28,15 @@
             self.add_node(given_node)
 
     def add_node(self, node, **kwargs):
         """
         Nodes can only be added to the leaves of the tree
         We define the leaves as the frontier that can be added to
         """
-        new_node = node.copy()
+        new_node = node.copy(label=node.get_label())
         leaf_node = self._frontier.pop(0)
         self._nodes.add(new_node)
 
         # Add the node to the frontier twice as the node can have 2 children
         self._frontier.append(new_node)
         self._frontier.append(new_node)
```

### Comparing `Lattice-Graph-Manipulation-0.1.1/lattice/graph/tree.py` & `Lattice-Graph-Manipulation-1.0.0/lattice/graph/tree.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .graph import Graph, NODE_ID
+from .graph import Graph
 from ..edge.edge import Edge
 
 
 class Tree(Graph):
     """
     A tree is a type of graph that constrains relationship types
     Trees are formally constrained as graphs where all nodes except the root must have one predecessor
@@ -17,12 +17,11 @@
         self._nodes.add(self.root_node)
 
     def add_nodes(self, parent_node, edge: Edge, **kwargs):
         """
         A node must be added by specifying an existing node as a predecessor
         """
         for key, value in kwargs.items():
-            name = NODE_ID + key
             new_node = value.copy(key)
-            setattr(self, name, new_node)
+            setattr(self, key, new_node)
 
             self.add_edge(parent_node, new_node, edge)
```

### Comparing `Lattice-Graph-Manipulation-0.1.1/lattice/node/node.py` & `Lattice-Graph-Manipulation-1.0.0/lattice/node/node.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """
 Basic Node
 """
 from __future__ import annotations
+import uuid
 
 from lattice.edge.edge import Edge
 
 
 class Node:
     _successors: set
     _predecessors: set
     _label: str
+    _fingerprint: uuid.UUID
 
     def __init__(self, pointer, label=None):
         self.pointer = pointer
         self._predecessors = set()
         self._successors = set()
         self._label = label
+        self._fingerprint = uuid.uuid4()
 
     def copy(self, label=None):
         return Node(self.pointer, label)
 
     @property
     def data(self):
         return self.pointer
@@ -28,15 +31,22 @@
     def successors(self):
         return self._successors
 
     @property
     def predecessors(self):
         return self._predecessors
 
-    def add_successor(self, edge: Edge, node: Node):
+    def add_edge(self, edge: Edge, node:Node):
+        self._add_successor(edge, node)
+        node._add_predecessor(edge, self)
+
+    def _add_successor(self, edge: Edge, node: Node):
         self._successors.add((edge, node))
 
-    def add_predecessor(self, edge: Edge, node: Node):
+    def _add_predecessor(self, edge: Edge, node: Node):
         self._predecessors.add((edge, node))
 
     def get_label(self):
         return self._label
+
+    def __repr__(self):
+        return str(self._fingerprint)
```

