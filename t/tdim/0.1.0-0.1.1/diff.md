# Comparing `tmp/tdim-0.1.0-py3-none-any.whl.zip` & `tmp/tdim-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3213 bytes, number of entries: 8
--rw-r--r--  2.0 unx      544 b- defN 23-May-09 20:16 tdim/__init__.py
+Zip file size: 3636 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      544 b- defN 23-May-09 21:24 tdim/__init__.py
 -rw-r--r--  2.0 unx     2641 b- defN 23-May-09 20:52 tdim/__main__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-09 20:31 tdim/py.typed
--rw-r--r--  2.0 unx     1427 b- defN 23-May-09 20:56 tdim-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-09 20:56 tdim-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 23-May-09 20:56 tdim-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-May-09 20:56 tdim-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      589 b- defN 23-May-09 20:56 tdim-0.1.0.dist-info/RECORD
-8 files, 5341 bytes uncompressed, 2187 bytes compressed:  59.1%
+-rw-r--r--  2.0 unx     2389 b- defN 23-May-09 21:25 tdim-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-09 21:25 tdim-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 23-May-09 21:25 tdim-0.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-May-09 21:25 tdim-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      589 b- defN 23-May-09 21:25 tdim-0.1.1.dist-info/RECORD
+8 files, 6303 bytes uncompressed, 2610 bytes compressed:  58.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: tdim/__main__.py
 Comment: 
 
 Filename: tdim/py.typed
 Comment: 
 
-Filename: tdim-0.1.0.dist-info/METADATA
+Filename: tdim-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: tdim-0.1.0.dist-info/WHEEL
+Filename: tdim-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: tdim-0.1.0.dist-info/entry_points.txt
+Filename: tdim-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: tdim-0.1.0.dist-info/top_level.txt
+Filename: tdim-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: tdim-0.1.0.dist-info/RECORD
+Filename: tdim-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdim/__init__.py

```diff
@@ -3,15 +3,15 @@
 ######################################################################
 # Main app information.
 __author__     = "Dave Pearson"
 __copyright__  = "Copyright 2023, Dave Pearson"
 __credits__    = [ "Dave Pearson" ]
 __maintainer__ = "Dave Pearson"
 __email__      = "davep@davep.org"
-__version__    = "0.1.0"
+__version__    = "0.1.1"
 __licence__    = "GPLv3+"
 
 ##############################################################################
 # Export the imports.
 __all__ = []
 
 ### __init__.py ends here
```

## Comparing `tdim-0.1.0.dist-info/RECORD` & `tdim-0.1.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-tdim/__init__.py,sha256=CFLPfwPZ0rPOiAdil29Vv3o8Xy410mFD-s0wkPfhnW4,544
+tdim/__init__.py,sha256=Lrq7Y-EiR18OWyqwLfYbt-X8ArvFTEjog-Jhf8Dt8_c,544
 tdim/__main__.py,sha256=cngvYgrhcDLe0DlxoiBc6NwwJSCnpHtOZ0e3utaAt8s,2641
 tdim/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tdim-0.1.0.dist-info/METADATA,sha256=cvfKsLVZDKSmc829sgFZ2PxfgEjhy_dhBs_hy5daJLg,1427
-tdim-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-tdim-0.1.0.dist-info/entry_points.txt,sha256=t4E26dLCvPVr6Kzju5Ip3Ki1rdihLuxT6fF1q3A8VWc,43
-tdim-0.1.0.dist-info/top_level.txt,sha256=VH0_41WbK5x9uQ6Vk7JC-kr5JS6Cc2jB-P2blMVR9HA,5
-tdim-0.1.0.dist-info/RECORD,,
+tdim-0.1.1.dist-info/METADATA,sha256=uhlWu2zZr8_jLlxJhjBWy1Z0wXkS7USq8xLLHP3li64,2389
+tdim-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+tdim-0.1.1.dist-info/entry_points.txt,sha256=t4E26dLCvPVr6Kzju5Ip3Ki1rdihLuxT6fF1q3A8VWc,43
+tdim-0.1.1.dist-info/top_level.txt,sha256=VH0_41WbK5x9uQ6Vk7JC-kr5JS6Cc2jB-P2blMVR9HA,5
+tdim-0.1.1.dist-info/RECORD,,
```

