# Comparing `tmp/spotON_sdk-0.0.2.8.tar.gz` & `tmp/spotON_sdk-0.0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.2.8.tar", last modified: Tue May  9 09:08:42 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.2.9.tar", last modified: Tue May  9 09:45:34 2023, max compression
```

## Comparing `spotON_sdk-0.0.2.8.tar` & `spotON_sdk-0.0.2.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.2.8/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.2.8/LICENSE
--rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.2.8/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-09 09:08:37.105836 spotON_sdk-0.0.2.8/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.2.8/spotON_sdk/constants/bidding_zones.py
--rw-r--r--   0        0        0     4566 2023-05-08 14:50:36.071727 spotON_sdk-0.0.2.8/spotON_sdk/constants/countries.py
--rw-r--r--   0        0        0     2065 2023-05-08 20:49:26.007366 spotON_sdk-0.0.2.8/spotON_sdk/constants/markets.py
--rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.2.8/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0     3276 2023-05-09 09:08:28.638506 spotON_sdk-0.0.2.8/spotON_sdk/logic/Entsoe_query.py
--rw-r--r--   0        0        0      993 2023-05-08 23:05:46.585853 spotON_sdk-0.0.2.8/spotON_sdk/logic/dataframe_modifier.py
--rw-r--r--   0        0        0      201 2023-05-08 20:50:42.181852 spotON_sdk-0.0.2.8/tests/test.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.2.9/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.2.9/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-09 09:45:20.775132 spotON_sdk-0.0.2.9/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.2.9/spotON_sdk/constants/bidding_zones.py
+-rw-r--r--   0        0        0     4566 2023-05-08 14:50:36.071727 spotON_sdk-0.0.2.9/spotON_sdk/constants/countries.py
+-rw-r--r--   0        0        0     2065 2023-05-08 20:49:26.007366 spotON_sdk-0.0.2.9/spotON_sdk/constants/markets.py
+-rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.2.9/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0     3481 2023-05-09 09:45:16.992573 spotON_sdk-0.0.2.9/spotON_sdk/logic/Entsoe_query.py
+-rw-r--r--   0        0        0      993 2023-05-08 23:05:46.585853 spotON_sdk-0.0.2.9/spotON_sdk/logic/dataframe_modifier.py
+-rw-r--r--   0        0        0      201 2023-05-08 20:50:42.181852 spotON_sdk-0.0.2.9/tests/test.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.2.9/PKG-INFO
```

### Comparing `spotON_sdk-0.0.2.8/.gitignore` & `spotON_sdk-0.0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.8/LICENSE` & `spotON_sdk-0.0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.8/spotON_sdk/constants/bidding_zones.py` & `spotON_sdk-0.0.2.9/spotON_sdk/constants/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.8/spotON_sdk/constants/countries.py` & `spotON_sdk-0.0.2.9/spotON_sdk/constants/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.8/spotON_sdk/constants/markets.py` & `spotON_sdk-0.0.2.9/spotON_sdk/constants/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.8/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.2.9/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.8/spotON_sdk/logic/Entsoe_query.py` & `spotON_sdk-0.0.2.9/spotON_sdk/logic/Entsoe_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,21 +32,24 @@
     tz1_offset = timezone1.utcoffset(date)
     tz2_offset = timezone2.utcoffset(date)
 
     timedelta = tz2_offset - tz1_offset
     return pd.Timedelta(timedelta)
 
 
-def getTimeStamps(country_code,tomorrow,overrideTime):
+def getTimeStamps(country_code,tomorrow,overrideTime,query_Month):
     
     tomorrow_timestamp = tomorrow.strftime("%Y%m%d")
 
     timestamp_start = pd.Timestamp(tomorrow_timestamp,tz=country_code.tz)
 
     timestamp_end = timestamp_start + pd.Timedelta(hours=23)
+    if query_Month:
+        timestamp_start = timestamp_start - pd.Timedelta(days=-31)
+        timestamp_end = timestamp_start + pd.Timedelta(hours=23,days=31)
 
     CET_Difference = timezone_difference(country_code.tz) 
     timestamp_start = timestamp_start - CET_Difference
 
     start = pd.Timestamp(timestamp_start)
     end = pd.Timestamp(timestamp_end)
 
@@ -76,22 +79,23 @@
 
     # Set the index to be a DatetimeIndex
     df.index = pd.DatetimeIndex(df.index,tz=country_code.tz)
     df.index = df.index 
 
     return df
 
-def query_Data(country_code,client,overrideTime :str|None = None,today_instead_of_tomorrow= False):
+def query_Data(country_code,client,overrideTime :str|None = None,today_instead_of_tomorrow= False,query_Month = False):
     today = get_Time_in(country_code.tz)
     tomorrow = today + pd.Timedelta(days=1)
 
     if today_instead_of_tomorrow:
         tomorrow = today
 
-    start,end,CET_Difference = getTimeStamps(country_code,tomorrow,overrideTime)
+
+    start,end,CET_Difference = getTimeStamps(country_code,tomorrow,overrideTime,query_Month)
     
     print (f"{start=}   {end=}  {CET_Difference=}")
     try:
         series = client.query_day_ahead_prices(country_code,start=start,end=end)
         return series,CET_Difference
     except NoMatchingDataError as e:
         print(f"No Values to fetch is {start=}   {end=}  {CET_Difference=} \n Is it before 13:30 UTC?","NoMatchingDataError occurred:", str(e))
```

### Comparing `spotON_sdk-0.0.2.8/spotON_sdk/logic/dataframe_modifier.py` & `spotON_sdk-0.0.2.9/spotON_sdk/logic/dataframe_modifier.py`

 * *Files identical despite different names*

