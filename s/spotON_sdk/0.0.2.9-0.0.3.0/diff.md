# Comparing `tmp/spotON_sdk-0.0.2.9.tar.gz` & `tmp/spotON_sdk-0.0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.2.9.tar", last modified: Tue May  9 09:45:34 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.3.0.tar", last modified: Tue May  9 10:07:06 2023, max compression
```

## Comparing `spotON_sdk-0.0.2.9.tar` & `spotON_sdk-0.0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.2.9/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.2.9/LICENSE
--rw-r--r--   0        0        0      317 2023-05-06 23:30:48.724788 spotON_sdk-0.0.2.9/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-09 09:45:20.775132 spotON_sdk-0.0.2.9/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.2.9/spotON_sdk/constants/bidding_zones.py
--rw-r--r--   0        0        0     4566 2023-05-08 14:50:36.071727 spotON_sdk-0.0.2.9/spotON_sdk/constants/countries.py
--rw-r--r--   0        0        0     2065 2023-05-08 20:49:26.007366 spotON_sdk-0.0.2.9/spotON_sdk/constants/markets.py
--rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.2.9/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0     3481 2023-05-09 09:45:16.992573 spotON_sdk-0.0.2.9/spotON_sdk/logic/Entsoe_query.py
--rw-r--r--   0        0        0      993 2023-05-08 23:05:46.585853 spotON_sdk-0.0.2.9/spotON_sdk/logic/dataframe_modifier.py
--rw-r--r--   0        0        0      201 2023-05-08 20:50:42.181852 spotON_sdk-0.0.2.9/tests/test.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.3.0/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.3.0/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-09 09:46:50.739083 spotON_sdk-0.0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-09 10:06:30.699812 spotON_sdk-0.0.3.0/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.3.0/spotON_sdk/constants/bidding_zones.py
+-rw-r--r--   0        0        0     4567 2023-05-09 10:06:06.205353 spotON_sdk-0.0.3.0/spotON_sdk/constants/countries.py
+-rw-r--r--   0        0        0     2065 2023-05-08 20:49:26.007366 spotON_sdk-0.0.3.0/spotON_sdk/constants/markets.py
+-rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.3.0/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0     3480 2023-05-09 10:03:04.606749 spotON_sdk-0.0.3.0/spotON_sdk/logic/Entsoe_query.py
+-rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.3.0/spotON_sdk/logic/dataframe_modifier.py
+-rw-r--r--   0        0        0      201 2023-05-08 20:50:42.181852 spotON_sdk-0.0.3.0/tests/test.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.3.0/PKG-INFO
```

### Comparing `spotON_sdk-0.0.2.9/.gitignore` & `spotON_sdk-0.0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.9/LICENSE` & `spotON_sdk-0.0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.9/spotON_sdk/constants/bidding_zones.py` & `spotON_sdk-0.0.3.0/spotON_sdk/constants/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.9/spotON_sdk/constants/countries.py` & `spotON_sdk-0.0.3.0/spotON_sdk/constants/countries.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     capital: str
     country_code: str
     country_name: str
     UTC_time_difference: int = field(init=False)
     
     def calculate_utc_time_difference(self) -> Optional[pd.Timedelta]:
         try:
-            print ("calculating timezone differecne")
+            #print ("calculating timezone differecne")
             timezone = f"Europe/{self.capital}"
             local_tz = pytz.timezone(timezone)
             utc_dt = pd.Timestamp.utcnow().to_pydatetime()
             local_dt = utc_dt.astimezone(local_tz)
             UTC_time_difference = (local_dt.utcoffset().total_seconds()) // 3600
             delta = pd.Timedelta(hours=UTC_time_difference)
             return delta,UTC_time_difference
```

### Comparing `spotON_sdk-0.0.2.9/spotON_sdk/constants/markets.py` & `spotON_sdk-0.0.3.0/spotON_sdk/constants/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.9/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.3.0/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.2.9/spotON_sdk/logic/Entsoe_query.py` & `spotON_sdk-0.0.3.0/spotON_sdk/logic/Entsoe_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     
     tomorrow_timestamp = tomorrow.strftime("%Y%m%d")
 
     timestamp_start = pd.Timestamp(tomorrow_timestamp,tz=country_code.tz)
 
     timestamp_end = timestamp_start + pd.Timedelta(hours=23)
     if query_Month:
-        timestamp_start = timestamp_start - pd.Timedelta(days=-31)
+        timestamp_start = timestamp_start - pd.Timedelta(days=31)
         timestamp_end = timestamp_start + pd.Timedelta(hours=23,days=31)
 
     CET_Difference = timezone_difference(country_code.tz) 
     timestamp_start = timestamp_start - CET_Difference
 
     start = pd.Timestamp(timestamp_start)
     end = pd.Timestamp(timestamp_end)
```

### Comparing `spotON_sdk-0.0.2.9/spotON_sdk/logic/dataframe_modifier.py` & `spotON_sdk-0.0.3.0/spotON_sdk/logic/dataframe_modifier.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,7 +20,17 @@
     return merged_df
 
 def add_priceRating(df):
     # Assuming your dataframe is called df
     df['rating'] = df['Price'] - df['Price_daily_AVG']
     df['rating_rank'] = df.groupby(df.index.date)['rating'].rank(ascending=True)-1
     return df
+
+def reduce_Filesize(df:pd.DataFrame):
+    df["Price"] = df["Price"].astype('float16')
+    df["Week"] = df["Week"].astype("int8")
+    df["Day"] = df["Day"].astype("int8")
+    df["Hour"] = df["Hour"].astype("int8")
+    df["Price_daily_AVG"] = df["Price_daily_AVG"].astype('float16')
+    df["rating"] = df["rating"].astype('float16')
+    df["rating_rank"] = df["rating_rank"].astype('int8')
+    return df
```

