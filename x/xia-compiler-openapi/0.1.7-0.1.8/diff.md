# Comparing `tmp/xia_compiler_openapi-0.1.7-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_openapi-0.1.8-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 237759 bytes, number of entries: 7
--rw-r--r--  2.0 unx      126 b- defN 23-May-09 08:25 xia_compiler_openapi/__init__.py
--rw-r--r--  2.0 unx   663552 b- defN 23-May-09 08:28 xia_compiler_openapi/compiler.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      150 b- defN 23-May-09 08:28 xia_compiler_openapi-0.1.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      695 b- defN 23-May-09 08:28 xia_compiler_openapi-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-09 08:28 xia_compiler_openapi-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-May-09 08:28 xia_compiler_openapi-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      648 b- defN 23-May-09 08:28 xia_compiler_openapi-0.1.7.dist-info/RECORD
-7 files, 665291 bytes uncompressed, 236589 bytes compressed:  64.4%
+Zip file size: 238353 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      126 b- defN 23-May-09 13:37 xia_compiler_openapi/__init__.py
+-rw-r--r--  2.0 unx   666112 b- defN 23-May-09 13:41 xia_compiler_openapi/compiler.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      150 b- defN 23-May-09 13:41 xia_compiler_openapi-0.1.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      695 b- defN 23-May-09 13:41 xia_compiler_openapi-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-09 13:41 xia_compiler_openapi-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-May-09 13:41 xia_compiler_openapi-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      648 b- defN 23-May-09 13:41 xia_compiler_openapi-0.1.8.dist-info/RECORD
+7 files, 667851 bytes uncompressed, 237183 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_openapi/__init__.py
 Comment: 
 
 Filename: xia_compiler_openapi/compiler.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.7.dist-info/LICENSE.txt
+Filename: xia_compiler_openapi-0.1.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.7.dist-info/METADATA
+Filename: xia_compiler_openapi-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.7.dist-info/WHEEL
+Filename: xia_compiler_openapi-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.7.dist-info/top_level.txt
+Filename: xia_compiler_openapi-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.7.dist-info/RECORD
+Filename: xia_compiler_openapi-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_compiler_openapi/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_compiler_openapi.compiler import XiaCompilerOpenapi
 
 
 __all__ = [
     "XiaCompilerOpenapi",
 ]
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
```

## Comparing `xia_compiler_openapi-0.1.7.dist-info/METADATA` & `xia_compiler_openapi-0.1.8.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-compiler-openapi
-Version: 0.1.7
+Version: 0.1.8
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-compiler-openapi/0.1.7/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-compiler-openapi/0.1.8/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_compiler_openapi-0.1.7.dist-info/RECORD` & `xia_compiler_openapi-0.1.8.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_compiler_openapi/__init__.py,sha256=rAtANIdReHhNF3v-8mZ7XacT2Wc76ZNrT9_XJLBjf3A,126
-xia_compiler_openapi/compiler.cp39-win_amd64.pyd,sha256=W3T1UTjcPzB4XxTdmuqbwDahy2MgPkQBr3B9zsSNJRo,663552
-xia_compiler_openapi-0.1.7.dist-info/LICENSE.txt,sha256=6lRgf9k2ZgrG5cDYuhNoHP6c9esKOIPd28rlbHJdX-g,150
-xia_compiler_openapi-0.1.7.dist-info/METADATA,sha256=Lp23qn7IKuw3xM_wESx8xN6IL6eOYD_osRiGJaCX1yQ,695
-xia_compiler_openapi-0.1.7.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_compiler_openapi-0.1.7.dist-info/top_level.txt,sha256=l-dHwHri9HVBghJIDfyblbK8E8exERfi3dhMi7vW3bE,21
-xia_compiler_openapi-0.1.7.dist-info/RECORD,,
+xia_compiler_openapi/__init__.py,sha256=4c2ceAUCsL35bE-PAhR15ALupdCInWThbRznUMXRnqg,126
+xia_compiler_openapi/compiler.cp39-win_amd64.pyd,sha256=1C9GDNOuTmjWGhOH-DAmFTcLcuZYzVnL0piobd3fBO4,666112
+xia_compiler_openapi-0.1.8.dist-info/LICENSE.txt,sha256=6lRgf9k2ZgrG5cDYuhNoHP6c9esKOIPd28rlbHJdX-g,150
+xia_compiler_openapi-0.1.8.dist-info/METADATA,sha256=I08PyfWD4NE62DgwOKJIMePS49Y1NCzOoHnh78s8mNU,695
+xia_compiler_openapi-0.1.8.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_compiler_openapi-0.1.8.dist-info/top_level.txt,sha256=l-dHwHri9HVBghJIDfyblbK8E8exERfi3dhMi7vW3bE,21
+xia_compiler_openapi-0.1.8.dist-info/RECORD,,
```

