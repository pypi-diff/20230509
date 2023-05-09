# Comparing `tmp/tsx-0.1.3-py3-none-any.whl.zip` & `tmp/tsx-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5810 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       58 b- defN 23-May-02 20:29 tsx/__init__.py
+Zip file size: 5815 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       74 b- defN 23-May-09 12:44 tsx/__init__.py
 -rw-rw-rw-  2.0 fat     8173 b- defN 23-May-07 18:40 tsx/ts.py
--rw-rw-rw-  2.0 fat     1089 b- defN 23-May-07 18:44 tsx-0.1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3756 b- defN 23-May-07 18:44 tsx-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 18:44 tsx-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-May-07 18:44 tsx-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      501 b- defN 23-May-07 18:44 tsx-0.1.3.dist-info/RECORD
-7 files, 13673 bytes uncompressed, 4930 bytes compressed:  63.9%
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-May-09 12:46 tsx-0.1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3756 b- defN 23-May-09 12:46 tsx-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-09 12:46 tsx-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-May-09 12:46 tsx-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      501 b- defN 23-May-09 12:46 tsx-0.1.4.dist-info/RECORD
+7 files, 13689 bytes uncompressed, 4935 bytes compressed:  63.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: tsx/__init__.py
 Comment: 
 
 Filename: tsx/ts.py
 Comment: 
 
-Filename: tsx-0.1.3.dist-info/LICENSE
+Filename: tsx-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: tsx-0.1.3.dist-info/METADATA
+Filename: tsx-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: tsx-0.1.3.dist-info/WHEEL
+Filename: tsx-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: tsx-0.1.3.dist-info/top_level.txt
+Filename: tsx-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: tsx-0.1.3.dist-info/RECORD
+Filename: tsx-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tsx/__init__.py

```diff
@@ -1,3 +1 @@
-from .ts import TS, TSMsec
-
-__all__ = ['TS', 'TSMsec']
+from .ts import TS, TSMsec, FIRST_MONDAY_TS, DAY_SEC, DAY_MSEC, WEEK_SEC
```

## Comparing `tsx-0.1.3.dist-info/LICENSE` & `tsx-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tsx-0.1.3.dist-info/METADATA` & `tsx-0.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsx
-Version: 0.1.3
+Version: 0.1.4
 Summary: TimeStam eXtensions for Python
 Home-page: https://github.com/asuiu/tsx
 Author: Andrei Suiu
 Author-email: andrei.suiu@gmail.com
 License: GPL
 Keywords: timestamp time date datetime ISO 8601
 Classifier: Development Status :: 5 - Production/Stable
```

