# Comparing `tmp/spotON_sdk-0.0.2.4.tar.gz` & `tmp/spotON_sdk-0.0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.2.4.tar", last modified: Mon May  8 22:36:43 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.2.5.tar", last modified: Mon May  8 22:52:56 2023, max compression
```

## Comparing `spotON_sdk-0.0.2.4.tar` & `spotON_sdk-0.0.2.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.2.4/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.2.4/LICENSE
--rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.2.4/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-08 22:36:29.578546 spotON_sdk-0.0.2.4/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.2.4/spotON_sdk/constants/bidding_zones.py
--rw-r--r--   0        0        0     4566 2023-05-08 14:50:36.071727 spotON_sdk-0.0.2.4/spotON_sdk/constants/countries.py
--rw-r--r--   0        0        0     2065 2023-05-08 20:49:26.007366 spotON_sdk-0.0.2.4/spotON_sdk/constants/markets.py
--rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.2.4/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0     2947 2023-05-08 22:35:11.772939 spotON_sdk-0.0.2.4/spotON_sdk/logic/Entsoe_query.py
--rw-r--r--   0        0        0      201 2023-05-08 20:50:42.181852 spotON_sdk-0.0.2.4/tests/test.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.2.5/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.2.5/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-08 22:52:49.115995 spotON_sdk-0.0.2.5/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.2.5/spotON_sdk/constants/bidding_zones.py
+-rw-r--r--   0        0        0     4566 2023-05-08 14:50:36.071727 spotON_sdk-0.0.2.5/spotON_sdk/constants/countries.py
+-rw-r--r--   0        0        0     2065 2023-05-08 20:49:26.007366 spotON_sdk-0.0.2.5/spotON_sdk/constants/markets.py
+-rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.2.5/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0     3019 2023-05-08 22:52:15.182133 spotON_sdk-0.0.2.5/spotON_sdk/logic/Entsoe_query.py
+-rw-r--r--   0        0        0      201 2023-05-08 20:50:42.181852 spotON_sdk-0.0.2.5/tests/test.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.2.5/PKG-INFO
```

### Comparing `spotON_sdk-0.0.2.4/.gitignore` & `spotON_sdk-0.0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.4/LICENSE` & `spotON_sdk-0.0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.4/spotON_sdk/constants/bidding_zones.py` & `spotON_sdk-0.0.2.5/spotON_sdk/constants/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.4/spotON_sdk/constants/countries.py` & `spotON_sdk-0.0.2.5/spotON_sdk/constants/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.4/spotON_sdk/constants/markets.py` & `spotON_sdk-0.0.2.5/spotON_sdk/constants/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.4/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.2.5/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.4/spotON_sdk/logic/Entsoe_query.py` & `spotON_sdk-0.0.2.5/spotON_sdk/logic/Entsoe_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,19 +75,21 @@
     df.columns = ['value']
 
     # Set the index to be a DatetimeIndex
     df.index = pd.DatetimeIndex(df.index,tz=country_code.tz)
     df.index = df.index 
 
     return df
-def query_Data(country_code,client,overrideTime :str|None = None):
+
+def query_Data(country_code,client,overrideTime :str|None = None,today_instead_of_tomorrow= False):
     today = get_Time_in(country_code.tz)
     tomorrow = today + pd.Timedelta(days=1)
-    tomorrow = today
 
+    if today_instead_of_tomorrow:
+        tomorrow = today
 
     start,end,CET_Difference = getTimeStamps(country_code,tomorrow,overrideTime)
     
     print (f"{start=}   {end=}  {CET_Difference=}")
     series = client.query_day_ahead_prices(country_code,start=start,end=end)
     return series,CET_Difference
```

