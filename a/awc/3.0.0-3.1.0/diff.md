# Comparing `tmp/awc-3.0.0-py2.py3-none-any.whl.zip` & `tmp/awc-3.1.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 23896 bytes, number of entries: 16
--rw-r--r--  2.0 unx     6843 b- defN 23-May-09 15:42 awc/__init__.py
+Zip file size: 23909 bytes, number of entries: 16
+-rw-r--r--  2.0 unx     6843 b- defN 23-May-09 16:10 awc/__init__.py
 -rw-r--r--  2.0 unx      678 b- defN 23-Apr-11 16:56 awc/__main__.py
 -rw-r--r--  2.0 unx     6030 b- defN 23-May-07 23:42 awc/api.py
 -rw-r--r--  2.0 unx      305 b- defN 23-Apr-12 22:27 awc/const.py
 -rw-r--r--  2.0 unx     1479 b- defN 23-Apr-15 21:04 awc/exc.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 12:49 awc/py.typed
--rw-r--r--  2.0 unx     1383 b- defN 23-Apr-13 14:54 awc/util.py
+-rw-r--r--  2.0 unx     1422 b- defN 23-May-09 16:09 awc/util.py
 -rw-r--r--  2.0 unx      614 b- defN 23-Apr-12 22:27 awc/wrn.py
 -rw-r--r--  2.0 unx     4658 b- defN 23-May-09 15:41 awc/sql/__init__.py
 -rw-r--r--  2.0 unx     3459 b- defN 23-May-09 15:41 awc/sql/helpers.py
--rw-------  2.0 unx    35107 b- defN 23-May-09 15:43 awc-3.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3812 b- defN 23-May-09 15:43 awc-3.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-09 15:43 awc-3.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-May-09 15:43 awc-3.0.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 19:04 awc-3.0.0.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1145 b- defN 23-May-09 15:43 awc-3.0.0.dist-info/RECORD
-16 files, 65628 bytes uncompressed, 22060 bytes compressed:  66.4%
+-rw-------  2.0 unx    35107 b- defN 23-May-09 16:11 awc-3.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3812 b- defN 23-May-09 16:11 awc-3.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-09 16:11 awc-3.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-May-09 16:11 awc-3.1.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 19:04 awc-3.1.0.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1145 b- defN 23-May-09 16:11 awc-3.1.0.dist-info/RECORD
+16 files, 65667 bytes uncompressed, 22073 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -24,26 +24,26 @@
 
 Filename: awc/sql/__init__.py
 Comment: 
 
 Filename: awc/sql/helpers.py
 Comment: 
 
-Filename: awc-3.0.0.dist-info/LICENSE
+Filename: awc-3.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: awc-3.0.0.dist-info/METADATA
+Filename: awc-3.1.0.dist-info/METADATA
 Comment: 
 
-Filename: awc-3.0.0.dist-info/WHEEL
+Filename: awc-3.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: awc-3.0.0.dist-info/top_level.txt
+Filename: awc-3.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: awc-3.0.0.dist-info/zip-safe
+Filename: awc-3.1.0.dist-info/zip-safe
 Comment: 
 
-Filename: awc-3.0.0.dist-info/RECORD
+Filename: awc-3.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awc/__init__.py

```diff
@@ -7,15 +7,15 @@
 from functools import wraps
 
 import requests
 from furl import furl  # type: ignore
 
 from . import const, exc, util
 
-__version__: typing.Final[str] = "3.0.0"
+__version__: typing.Final[str] = "3.1.0"
 
 
 class Awc:
     """ari-web comments interface
 
     this is where all API requests begin, you must
     pass an instance of this object to every api wrapper
```

## awc/util.py

```diff
@@ -37,18 +37,20 @@
 
     content: str -- content you want to truncated
     length: int -- to what length should the content be truncated to
     do_warn: bool = True -- do we warn if content is being truncated
 
     return str -- the truncated content"""
 
+    content = content.strip()
+
     if do_warn and len(content) > length:
         warn(ContentTruncatedWarning(content, length))
 
-    return content[:length]
+    return content[:length].strip()
 
 
 def resp_to_bool(resp: str) -> bool:
     """convets a response like 0 and 1 to boolean
 
     resp: str -- the response
```

## Comparing `awc-3.0.0.dist-info/LICENSE` & `awc-3.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awc-3.0.0.dist-info/METADATA` & `awc-3.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awc
-Version: 3.0.0
+Version: 3.1.0
 Summary: wrapper for ari-web comments API
 Home-page: https://ari-web.xyz/gh/awc
 Author: Ari Archer
 Author-email: ari.web.xyz@gmail.com
 License: GPLv3+
 Keywords: http,http-client,comments,api,wrapper,https
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `awc-3.0.0.dist-info/RECORD` & `awc-3.1.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-awc/__init__.py,sha256=PkKqXksEf-5PhxlUnPu-AB6YyuvAci8NZE06_hYJy_k,6843
+awc/__init__.py,sha256=CjXEhXjtr8lIHmY3TSFtlATvbQhSsu5SbvFGbqiLNus,6843
 awc/__main__.py,sha256=d1UfoKcH5bl9qoqWowmcARIitWbbGsasAZfq8RHHsE4,678
 awc/api.py,sha256=f02eIZdXfOZo9f-f7YhN1Rhcz4a55KAzxRfTIxSrzTg,6030
 awc/const.py,sha256=0ctjO9muVRU7kBkqF9LjcgwvP4baLum63UUOxTE1oLw,305
 awc/exc.py,sha256=kGwH4_a8C1EpYx3PvoBXyWiiW451YbHsKi_JGtnsiuk,1479
 awc/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-awc/util.py,sha256=u9-_per8iyglLx9dVfQKJBdSEFZq2-5aymE7XDjoJ0o,1383
+awc/util.py,sha256=VkpiEdESLdZWwAv8OaNkJHVjzP4gmkF8Z4pGplbX0l4,1422
 awc/wrn.py,sha256=K84cpt9OdHQi76vhgMsWFbl8rIN_sH6EkOGptZOUWmQ,614
 awc/sql/__init__.py,sha256=JgJLCahZVJD0Sa9TXjrffMqCyDjxTKEQw5nxwAEOp2s,4658
 awc/sql/helpers.py,sha256=wdaRfqpbuSvtDwMhBl9OFreithQRJQ2NfnKwbdqJGSg,3459
-awc-3.0.0.dist-info/LICENSE,sha256=nqVIZAIjniFxpDnU4HMUA3KRZ8mFA_JpXMNFVQTHlVI,35107
-awc-3.0.0.dist-info/METADATA,sha256=d2mQPHDyg-TpW8a7zHDW9aNxzX58Vt4Z_cJgq1OwoZI,3812
-awc-3.0.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-awc-3.0.0.dist-info/top_level.txt,sha256=Xj3P9OwultDU5KrAvJbWKuD3ki2LWL6tSfbMPu28Hck,4
-awc-3.0.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-awc-3.0.0.dist-info/RECORD,,
+awc-3.1.0.dist-info/LICENSE,sha256=nqVIZAIjniFxpDnU4HMUA3KRZ8mFA_JpXMNFVQTHlVI,35107
+awc-3.1.0.dist-info/METADATA,sha256=FaFOVdRNFy4eTcu3Av0wRoOhl5tNtX6xwQDA9eAbITQ,3812
+awc-3.1.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+awc-3.1.0.dist-info/top_level.txt,sha256=Xj3P9OwultDU5KrAvJbWKuD3ki2LWL6tSfbMPu28Hck,4
+awc-3.1.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+awc-3.1.0.dist-info/RECORD,,
```

