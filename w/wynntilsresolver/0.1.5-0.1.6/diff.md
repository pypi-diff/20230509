# Comparing `tmp/wynntilsresolver-0.1.5.tar.gz` & `tmp/wynntilsresolver-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wynntilsresolver-0.1.5.tar", last modified: Sun May  7 21:59:07 2023, max compression
+gzip compressed data, was "wynntilsresolver-0.1.6.tar", last modified: Tue May  9 16:39:27 2023, max compression
```

## Comparing `wynntilsresolver-0.1.5.tar` & `wynntilsresolver-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0      982 2023-05-01 18:24:11.966738 wynntilsresolver-0.1.5/LICENSE
--rwxr-xr-x   0        0        0     1292 2023-05-07 21:59:07.135395 wynntilsresolver-0.1.5/pyproject.toml
--rwxr-xr-x   0        0        0     1595 2023-05-07 21:57:59.122947 wynntilsresolver-0.1.5/readme.md
--rwxr-xr-x   0        0        0      455 2023-05-07 21:42:32.114615 wynntilsresolver-0.1.5/src/wynntilsresolver/__init__.py
--rwxr-xr-x   0        0        0      964 2023-05-07 21:42:27.218536 wynntilsresolver-0.1.5/src/wynntilsresolver/__main__.py
--rwxr-xr-x   0        0        0      459 2023-05-07 21:42:22.729982 wynntilsresolver-0.1.5/src/wynntilsresolver/exceptions.py
--rwxr-xr-x   0        0        0     1374 2023-05-07 21:56:38.495741 wynntilsresolver-0.1.5/src/wynntilsresolver/model.py
--rwxr-xr-x   0        0        0     2439 2023-05-07 21:57:06.674456 wynntilsresolver-0.1.5/src/wynntilsresolver/resolver.py
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 wynntilsresolver-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0      982 2023-05-01 18:24:11.966738 wynntilsresolver-0.1.6/LICENSE
+-rwxr-xr-x   0        0        0     1292 2023-05-09 16:39:27.458678 wynntilsresolver-0.1.6/pyproject.toml
+-rwxr-xr-x   0        0        0     1595 2023-05-07 21:57:59.122947 wynntilsresolver-0.1.6/readme.md
+-rwxr-xr-x   0        0        0      455 2023-05-07 21:42:32.114615 wynntilsresolver-0.1.6/src/wynntilsresolver/__init__.py
+-rwxr-xr-x   0        0        0      964 2023-05-07 21:42:27.218536 wynntilsresolver-0.1.6/src/wynntilsresolver/__main__.py
+-rwxr-xr-x   0        0        0      459 2023-05-07 21:42:22.729982 wynntilsresolver-0.1.6/src/wynntilsresolver/exceptions.py
+-rwxr-xr-x   0        0        0     1462 2023-05-09 16:36:44.896376 wynntilsresolver-0.1.6/src/wynntilsresolver/model.py
+-rwxr-xr-x   0        0        0     2529 2023-05-09 16:38:32.683722 wynntilsresolver-0.1.6/src/wynntilsresolver/resolver.py
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 wynntilsresolver-0.1.6/PKG-INFO
```

### Comparing `wynntilsresolver-0.1.5/LICENSE` & `wynntilsresolver-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-0.1.5/pyproject.toml` & `wynntilsresolver-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "WynntilsResolver"
-version = "0.1.5"
+version = "0.1.6"
 description = "A simple resolver to analyze wynntils' encoded equipment in chat."
 authors = [
     { name = "FYWinds", email = "i@windis.cn" },
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "readme.md"
```

### Comparing `wynntilsresolver-0.1.5/readme.md` & `wynntilsresolver-0.1.6/readme.md`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-0.1.5/src/wynntilsresolver/__main__.py` & `wynntilsresolver-0.1.6/src/wynntilsresolver/__main__.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-0.1.5/src/wynntilsresolver/model.py` & `wynntilsresolver-0.1.6/src/wynntilsresolver/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Author       : FYWinds i@windis.cn
 Date         : 2023-05-01 09:20:21
 LastEditors  : FYWinds i@windis.cn
-LastEditTime : 2023-05-07 17:56:38
+LastEditTime : 2023-05-09 12:36:10
 FilePath     : /src/wynntilsresolver/model.py
 
 Copyright (c) 2023 by FYWinds
 All Rights Reserved.
 Any modifications or distributions of the file
 should mark the original author's name.
 """
@@ -31,20 +31,20 @@
         return self.name
 
 
 @dataclasses.dataclass(frozen=True)
 class Item:
     name: str
     """The name of the item"""
-    ids: List[int]
+    ids: List[int] = dataclasses.field(default_factory=list)
     """The roll values of the item, sorted in wynntils' item identification order
     Can calculate by multiplying the id's base value"""
-    powders: List[Powder]
+    powders: List[Powder] = dataclasses.field(default_factory=list)
     """Powders on the item, without tier"""
-    rerolls: int
+    rerolls: int = 0
     """Rerolls of the item"""
 
 
 class CustomEncoder(json.JSONEncoder):
     def default(self, obj):
         if type(obj) is Powder:
             return str(obj)
```

### Comparing `wynntilsresolver-0.1.5/src/wynntilsresolver/resolver.py` & `wynntilsresolver-0.1.6/src/wynntilsresolver/resolver.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Author       : FYWinds i@windis.cn
 Date         : 2023-05-01 09:08:08
 LastEditors  : FYWinds i@windis.cn
-LastEditTime : 2023-05-07 17:56:51
+LastEditTime : 2023-05-09 12:38:27
 FilePath     : /src/wynntilsresolver/resolver.py
 
 Copyright (c) 2023 by FYWinds
 All Rights Reserved.
 Any modifications or distributions of the file
 should mark the original author's name.
 """
@@ -68,21 +68,25 @@
         for powderNum in powders:
             while powderNum > 0:
                 plist.append(Powder(powderNum % 6 - 1))
                 powderNum = math.floor(powderNum / 6)
         return plist
 
     def _decode_string(self, text: str) -> str:
+        if not text:
+            return ""
         decoded: str = ""
         for i in text:
             value = ord(i) - ord(_OFFSET) + 32
             decoded += chr(value)
         return decoded
 
     def _decode_numbers(self, text: str) -> List[int]:
+        if not text:
+            return []
         decoded: list[int] = []
         for i in text:
             decoded.append(ord(i) - ord(_OFFSET))
         return decoded
 
 
 __all__ = ["Resolver"]
```

### Comparing `wynntilsresolver-0.1.5/PKG-INFO` & `wynntilsresolver-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wynntilsresolver
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple resolver to analyze wynntils' encoded equipment in chat.
 Keywords: wynntils resolver wynncraft
 Author-Email: FYWinds <i@windis.cn>
 License: GLWTPL
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

