# Comparing `tmp/hk_libs-1.2.0-py3-none-any.whl.zip` & `tmp/hk_libs-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5584 bytes, number of entries: 7
--rw-r--r--  2.0 unx    11063 b- defN 23-May-06 06:54 hk_libs/HKDict.py
+Zip file size: 5594 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    10882 b- defN 23-May-09 03:38 hk_libs/HKDict.py
 -rw-r--r--  2.0 unx     7020 b- defN 23-May-05 08:18 hk_libs/HKPrint.py
 -rw-r--r--  2.0 unx       88 b- defN 23-May-05 09:42 hk_libs/__init__.py
--rw-r--r--  2.0 unx     2374 b- defN 23-May-06 07:02 hk_libs-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-06 07:02 hk_libs-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-May-06 07:02 hk_libs-1.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      521 b- defN 23-May-06 07:02 hk_libs-1.2.0.dist-info/RECORD
-7 files, 21166 bytes uncompressed, 4666 bytes compressed:  78.0%
+-rw-r--r--  2.0 unx     2374 b- defN 23-May-09 03:40 hk_libs-1.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-09 03:40 hk_libs-1.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-09 03:40 hk_libs-1.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      521 b- defN 23-May-09 03:40 hk_libs-1.2.1.dist-info/RECORD
+7 files, 20985 bytes uncompressed, 4676 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: hk_libs/HKPrint.py
 Comment: 
 
 Filename: hk_libs/__init__.py
 Comment: 
 
-Filename: hk_libs-1.2.0.dist-info/METADATA
+Filename: hk_libs-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: hk_libs-1.2.0.dist-info/WHEEL
+Filename: hk_libs-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: hk_libs-1.2.0.dist-info/top_level.txt
+Filename: hk_libs-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: hk_libs-1.2.0.dist-info/RECORD
+Filename: hk_libs-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hk_libs/HKDict.py

```diff
@@ -122,30 +122,29 @@
         assert type(other) in [HKDict, dict], f"invalid type {type(other)}: only HKDict, dict are available"
         if isinstance(other, dict):
             other = HKDict.from_dict(other)
         return HKDict.from_dict({**self.__dict__, **other.__dict__})
     
     def __iadd__(self, other):
         assert type(other) in [HKDict, dict], f"invalid type {type(other)}: only HKDict, dict are available"
-        if isinstance(other, dict):
-            other = HKDict.from_dict(other)
-        self.__dict__ = {**self.__dict__, **other.__dict__}
+        for key in other:
+            self[key] = other[key]
         return self
     
     def __sub__(self, other):
         assert type(other) in [HKDict, dict], f"invalid type {type(other)}: only HKDict, dict are available"
         if isinstance(other, dict):
             other = HKDict.from_dict(other)
         return HKDict.from_dict({key: value for key, value in self.__dict__.items() if key not in other.__dict__})
     
     def __isub__(self, other):
         assert type(other) in [HKDict, dict], f"invalid type {type(other)}: only HKDict, dict are available"
-        if isinstance(other, dict):
-            other = HKDict.from_dict(other)
-        self.__dict__ = {key: value for key, value in self.__dict__.items() if key not in other.__dict__}
+        for key in other:
+            if key in self:
+                del self[key]
         return self
 
     @staticmethod
     def add(a, b):
         assert type(a) in [HKDict, dict], f"invalid type {type(a)}: only HKDict, dict are available"
         assert type(b) in [HKDict, dict], f"invalid type {type(b)}: only HKDict, dict are available"
         return a + b
```

## Comparing `hk_libs-1.2.0.dist-info/METADATA` & `hk_libs-1.2.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hk-libs
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python library by Heekang Park
 Home-page: https://github.com/HeekangPark/hk_libs
 Author: Heekang Park
 Author-email: park.heekang33@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

