# Comparing `tmp/llmpool-0.1.3-py3-none-any.whl.zip` & `tmp/llmpool-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9228 bytes, number of entries: 11
--rw-rw-rw-  2.0 unx      114 b- defN 23-May-08 15:00 llmpool/__init__.py
--rw-rw-rw-  2.0 unx     3897 b- defN 23-May-08 14:27 llmpool/local_model.py
+Zip file size: 9616 bytes, number of entries: 11
+-rw-rw-rw-  2.0 unx      194 b- defN 23-May-09 03:01 llmpool/__init__.py
+-rw-rw-rw-  2.0 unx     3897 b- defN 23-May-09 02:55 llmpool/local_model.py
 -rw-rw-rw-  2.0 unx      591 b- defN 23-May-08 07:36 llmpool/model.py
 -rw-rw-rw-  2.0 unx      919 b- defN 23-May-08 09:30 llmpool/model_pool.py
--rw-rw-rw-  2.0 unx     1868 b- defN 23-May-08 09:20 llmpool/remote_model.py
+-rw-rw-rw-  2.0 unx     1883 b- defN 23-May-09 02:54 llmpool/remote_model.py
 -rw-rw-rw-  2.0 unx     1422 b- defN 23-May-08 14:49 llmpool/utils.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-May-08 15:00 llmpool-0.1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 unx     1632 b- defN 23-May-08 15:00 llmpool-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-May-08 15:00 llmpool-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        8 b- defN 23-May-08 15:00 llmpool-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      842 b- defN 23-May-08 15:00 llmpool-0.1.3.dist-info/RECORD
-11 files, 22742 bytes uncompressed, 7818 bytes compressed:  65.6%
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-May-09 03:01 llmpool-0.1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 unx     2398 b- defN 23-May-09 03:01 llmpool-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-May-09 03:01 llmpool-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        8 b- defN 23-May-09 03:01 llmpool-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      842 b- defN 23-May-09 03:01 llmpool-0.1.4.dist-info/RECORD
+11 files, 23603 bytes uncompressed, 8206 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: llmpool/remote_model.py
 Comment: 
 
 Filename: llmpool/utils.py
 Comment: 
 
-Filename: llmpool-0.1.3.dist-info/LICENSE
+Filename: llmpool-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: llmpool-0.1.3.dist-info/METADATA
+Filename: llmpool-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: llmpool-0.1.3.dist-info/WHEEL
+Filename: llmpool-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: llmpool-0.1.3.dist-info/top_level.txt
+Filename: llmpool-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: llmpool-0.1.3.dist-info/RECORD
+Filename: llmpool-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## llmpool/__init__.py

```diff
@@ -1,4 +1,6 @@
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 from .local_model import LocalLLModel, LocalLoRALLModel
-from .model_pool import LLModelPool
+from .model_pool import LLModelPool
+from .remote_model import TxtGenIfLLModel
+from .utils import instantiate_models
```

## llmpool/remote_model.py

```diff
@@ -48,10 +48,10 @@
             top_k=gen_config.top_k,
             top_p=gen_config.top_p,
             truncate=None,
             typical_p=gen_config.typical_p,
             watermark=False,
         )
 
-        return batch
+        return batch.generated_text
```

## Comparing `llmpool-0.1.3.dist-info/LICENSE` & `llmpool-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `llmpool-0.1.3.dist-info/RECORD` & `llmpool-0.1.4.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-llmpool/__init__.py,sha256=AvF8wVuS5dRIzGoXJIJIkcd2cx1xgwjQ0gYkCKVroFQ,114
+llmpool/__init__.py,sha256=T-RN3R-prUcGOIKajOhZHvlxy4PJ1derAfpjxFoPQco,194
 llmpool/local_model.py,sha256=zzGAdpzAgG5nzox6usdTd0rnB8A2K0YUVBy22zkPGAI,3897
 llmpool/model.py,sha256=l29Usepsgp3z--CB0sJh-8VdGJlmWJIyzqLiZ3ep1Gs,591
 llmpool/model_pool.py,sha256=NazsR-AfxSzxew6DGB5-bePhwgSecuBsv-lB6WmOpt0,919
-llmpool/remote_model.py,sha256=NI2xu2GSUI8u4q35fP_BNUpjnD8eUDiKiPUgFyCjViY,1868
+llmpool/remote_model.py,sha256=6lNzGC8WuCBFGHtQN2_4FVTMD63EoLuHM5lQfYEmQQU,1883
 llmpool/utils.py,sha256=hGdpMy-M3b58779mv-ERzb0h5aBen59lxmcq-18gjMY,1422
-llmpool-0.1.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-llmpool-0.1.3.dist-info/METADATA,sha256=sfLn2iJ_XxndLDF9_p2uIxpW-hl6K2z4_-gXd6KOOvU,1632
-llmpool-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-llmpool-0.1.3.dist-info/top_level.txt,sha256=1kKiMvue6u12IMQD92YMn4xdcQPDejrD0VuDl-pOCjE,8
-llmpool-0.1.3.dist-info/RECORD,,
+llmpool-0.1.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+llmpool-0.1.4.dist-info/METADATA,sha256=-heWP_S4fXV4pqCpQ6wtNqw3SvCJY6XvJvWXDHbNI8Q,2398
+llmpool-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+llmpool-0.1.4.dist-info/top_level.txt,sha256=1kKiMvue6u12IMQD92YMn4xdcQPDejrD0VuDl-pOCjE,8
+llmpool-0.1.4.dist-info/RECORD,,
```

