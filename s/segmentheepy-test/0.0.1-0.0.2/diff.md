# Comparing `tmp/segmentheepy_test-0.0.1-py3-none-any.whl.zip` & `tmp/segmentheepy_test-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10099 bytes, number of entries: 9
--rw-rw-r--  2.0 unx        0 b- defN 23-Jan-31 09:33 segmenthee/__init__.py
--rw-rw-r--  2.0 unx    24732 b- defN 23-Mar-03 11:23 segmenthee/cart_api.py
--rw-rw-r--  2.0 unx      766 b- defN 23-Mar-02 12:58 segmenthee/config.py
--rw-rw-r--  2.0 unx     2023 b- defN 23-Mar-03 10:28 segmenthee/parser_api.py
--rw-rw-r--  2.0 unx     7932 b- defN 23-Mar-03 10:28 segmenthee/shop.py
--rw-rw-r--  2.0 unx      261 b- defN 23-Mar-07 09:53 segmentheepy_test-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-07 09:53 segmentheepy_test-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Mar-07 09:53 segmentheepy_test-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      725 b- defN 23-Mar-07 09:53 segmentheepy_test-0.0.1.dist-info/RECORD
-9 files, 36542 bytes uncompressed, 8845 bytes compressed:  75.8%
+Zip file size: 10118 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-09 16:01 segmenthee/__init__.py
+-rw-rw-r--  2.0 unx    24705 b- defN 23-May-09 16:10 segmenthee/cart_api.py
+-rw-rw-r--  2.0 unx      766 b- defN 23-May-09 16:01 segmenthee/config.py
+-rw-rw-r--  2.0 unx     2023 b- defN 23-May-09 16:01 segmenthee/parser_api.py
+-rw-rw-r--  2.0 unx     7932 b- defN 23-May-09 16:02 segmenthee/shop.py
+-rw-rw-r--  2.0 unx      308 b- defN 23-May-09 18:01 segmentheepy_test-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-09 18:01 segmentheepy_test-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-May-09 18:01 segmentheepy_test-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      725 b- defN 23-May-09 18:01 segmentheepy_test-0.0.2.dist-info/RECORD
+9 files, 36562 bytes uncompressed, 8864 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: segmenthee/parser_api.py
 Comment: 
 
 Filename: segmenthee/shop.py
 Comment: 
 
-Filename: segmentheepy_test-0.0.1.dist-info/METADATA
+Filename: segmentheepy_test-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: segmentheepy_test-0.0.1.dist-info/WHEEL
+Filename: segmentheepy_test-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: segmentheepy_test-0.0.1.dist-info/top_level.txt
+Filename: segmentheepy_test-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: segmentheepy_test-0.0.1.dist-info/RECORD
+Filename: segmentheepy_test-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## segmenthee/cart_api.py

```diff
@@ -40,22 +40,14 @@
     "tabtypetrend": [0.5, 0.025],
     "navigationtrend": [0.5, 0.025],
     "referrertrend": [0.5, 0.025],
     "pagetrend": [0.5, 0.025],
     "sorttrend": [0.5, 0.025]
 }
 
-def UpdateFactors(new_params, verbose=0):
-    global params
-    for key in new_params:
-        if key in params:
-            params[key] = new_params[key]
-    if verbose:
-        print(params)
-
 MAX_CATEGORY = 6
 tabtype_dict = {'New':0, 'Existing':1}
 navigation_dict = {'NAVIGATE':0,'FORWARD':1,'BACK':2,'RELOAD':3}
 origin_dict = {"facebook":0,"google":1,"shop":2}
 sort_dict = {'default':0, 'name':1, 'price':2, 'order':3, 'relevance':4, 'date':5, 'rating':6, 'latest':7, 'discount':8, 'view':9}
 
 
@@ -476,17 +468,22 @@
 # globals
 
 device_dict = {"mobile":0,"tablet":1,"desktop":2}
 os_dict = {"ms":0,"apple":1,"linux":2}
 lang_dict = {"hu":0}
 sessionstatus_dict = {"Browsing":0,"CartModified":1}
 
-def Update(prevstate,bodyevent):
+def Update(prevstate,bodyevent,newparams=None):
+    global params
     if prevstate["sessionstatus"] == "Bot":
         return prevstate
+    if newparams: # not None
+        for key in newparams:
+            if key in params:
+                params[key] = newparams[key]
     return bodyevent.Update(prevstate)
 
 def NewState(origin_string, user_agent_string, lang_string, firstbodyevent):
     
     origin_cls = parser_api.parse_origin(origin_string)
     if origin_cls in origin_dict:
         origin = origin_dict[origin_cls]
```

