# Comparing `tmp/spotON_sdk-0.0.2.6.tar.gz` & `tmp/spotON_sdk-0.0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.2.6.tar", last modified: Mon May  8 23:06:18 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.2.7.tar", last modified: Tue May  9 09:01:17 2023, max compression
```

## Comparing `spotON_sdk-0.0.2.6.tar` & `spotON_sdk-0.0.2.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.2.6/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.2.6/LICENSE
--rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.2.6/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-08 23:05:56.775968 spotON_sdk-0.0.2.6/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.2.6/spotON_sdk/constants/bidding_zones.py
--rw-r--r--   0        0        0     4566 2023-05-08 14:50:36.071727 spotON_sdk-0.0.2.6/spotON_sdk/constants/countries.py
--rw-r--r--   0        0        0     2065 2023-05-08 20:49:26.007366 spotON_sdk-0.0.2.6/spotON_sdk/constants/markets.py
--rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.2.6/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0     3019 2023-05-08 22:52:15.182133 spotON_sdk-0.0.2.6/spotON_sdk/logic/Entsoe_query.py
--rw-r--r--   0        0        0      993 2023-05-08 23:05:46.585853 spotON_sdk-0.0.2.6/spotON_sdk/logic/dataframe_modifier.py
--rw-r--r--   0        0        0      201 2023-05-08 20:50:42.181852 spotON_sdk-0.0.2.6/tests/test.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.2.7/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.2.7/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-09 09:01:08.646406 spotON_sdk-0.0.2.7/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.2.7/spotON_sdk/constants/bidding_zones.py
+-rw-r--r--   0        0        0     4566 2023-05-08 14:50:36.071727 spotON_sdk-0.0.2.7/spotON_sdk/constants/countries.py
+-rw-r--r--   0        0        0     2065 2023-05-08 20:49:26.007366 spotON_sdk-0.0.2.7/spotON_sdk/constants/markets.py
+-rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.2.7/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0     3183 2023-05-09 08:59:26.746251 spotON_sdk-0.0.2.7/spotON_sdk/logic/Entsoe_query.py
+-rw-r--r--   0        0        0      993 2023-05-08 23:05:46.585853 spotON_sdk-0.0.2.7/spotON_sdk/logic/dataframe_modifier.py
+-rw-r--r--   0        0        0      201 2023-05-08 20:50:42.181852 spotON_sdk-0.0.2.7/tests/test.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.2.7/PKG-INFO
```

### Comparing `spotON_sdk-0.0.2.6/.gitignore` & `spotON_sdk-0.0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.6/LICENSE` & `spotON_sdk-0.0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.6/spotON_sdk/constants/bidding_zones.py` & `spotON_sdk-0.0.2.7/spotON_sdk/constants/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.6/spotON_sdk/constants/countries.py` & `spotON_sdk-0.0.2.7/spotON_sdk/constants/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.6/spotON_sdk/constants/markets.py` & `spotON_sdk-0.0.2.7/spotON_sdk/constants/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.6/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.2.7/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.6/spotON_sdk/logic/Entsoe_query.py` & `spotON_sdk-0.0.2.7/spotON_sdk/logic/Entsoe_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,16 +86,21 @@
 
     if today_instead_of_tomorrow:
         tomorrow = today
 
     start,end,CET_Difference = getTimeStamps(country_code,tomorrow,overrideTime)
     
     print (f"{start=}   {end=}  {CET_Difference=}")
+
     series = client.query_day_ahead_prices(country_code,start=start,end=end)
-    return series,CET_Difference
+    print (series)
+    if series:
+        return series,CET_Difference
+    else:
+        raise ValueError(f"No Values to fetch is {start=}   {end=}  {CET_Difference=} \n Is it before 13:30 UTC?")
 
 def create_Dataframe(s:pd.Series,market:Market):
 
     # Convert series to dataframe
     df = s.to_frame()
 
     # Rename the column
```

### Comparing `spotON_sdk-0.0.2.6/spotON_sdk/logic/dataframe_modifier.py` & `spotON_sdk-0.0.2.7/spotON_sdk/logic/dataframe_modifier.py`

 * *Files identical despite different names*

