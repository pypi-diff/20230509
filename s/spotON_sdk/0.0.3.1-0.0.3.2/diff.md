# Comparing `tmp/spotON_sdk-0.0.3.1.tar.gz` & `tmp/spotON_sdk-0.0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.3.1.tar", last modified: Tue May  9 10:38:53 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.3.2.tar", last modified: Tue May  9 14:25:27 2023, max compression
```

## Comparing `spotON_sdk-0.0.3.1.tar` & `spotON_sdk-0.0.3.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.3.1/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.3.1/LICENSE
--rw-r--r--   0        0        0      317 2023-05-09 09:46:50.739083 spotON_sdk-0.0.3.1/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-09 10:38:44.665543 spotON_sdk-0.0.3.1/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.3.1/spotON_sdk/constants/bidding_zones.py
--rw-r--r--   0        0        0     4567 2023-05-09 10:06:06.205353 spotON_sdk-0.0.3.1/spotON_sdk/constants/countries.py
--rw-r--r--   0        0        0     2065 2023-05-08 20:49:26.007366 spotON_sdk-0.0.3.1/spotON_sdk/constants/markets.py
--rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.3.1/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0     3480 2023-05-09 10:03:04.606749 spotON_sdk-0.0.3.1/spotON_sdk/logic/Entsoe_query.py
--rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.3.1/spotON_sdk/logic/dataframe_modifier.py
--rw-r--r--   0        0        0      201 2023-05-08 20:50:42.181852 spotON_sdk-0.0.3.1/tests/test.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.3.2/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.3.2/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-09 09:46:50.739083 spotON_sdk-0.0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-09 14:23:24.407229 spotON_sdk-0.0.3.2/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.3.2/spotON_sdk/constants/bidding_zones.py
+-rw-r--r--   0        0        0     4567 2023-05-09 10:06:06.205353 spotON_sdk-0.0.3.2/spotON_sdk/constants/countries.py
+-rw-r--r--   0        0        0     2068 2023-05-09 14:25:18.706494 spotON_sdk-0.0.3.2/spotON_sdk/constants/markets.py
+-rw-r--r--   0        0        0      712 2023-05-09 14:22:52.716892 spotON_sdk-0.0.3.2/spotON_sdk/logic/BestHour.py
+-rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.3.2/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0     3480 2023-05-09 10:03:04.606749 spotON_sdk-0.0.3.2/spotON_sdk/logic/Entsoe_query.py
+-rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.3.2/spotON_sdk/logic/dataframe_modifier.py
+-rw-r--r--   0        0        0      201 2023-05-08 20:50:42.181852 spotON_sdk-0.0.3.2/tests/test.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.3.2/PKG-INFO
```

### Comparing `spotON_sdk-0.0.3.1/.gitignore` & `spotON_sdk-0.0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.1/LICENSE` & `spotON_sdk-0.0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.1/spotON_sdk/constants/bidding_zones.py` & `spotON_sdk-0.0.3.2/spotON_sdk/constants/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.1/spotON_sdk/constants/countries.py` & `spotON_sdk-0.0.3.2/spotON_sdk/constants/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.1/spotON_sdk/constants/markets.py` & `spotON_sdk-0.0.3.2/spotON_sdk/constants/markets.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,17 +40,17 @@
 
 dataclass
 class Markets():
     austria = Market(Area.AT,Austria)
     germany = Market(Area.DE_LU,Germany)
     luxembourg = Market(Area.DE_LU,Luxembourg)
     sweden1 = Market(Area.SE_1,Sweden)
-    sweden2 = Market(Area.SE_2,Sweden)
-    sweden3 = Market(Area.SE_3,Sweden)
-    sweden4 = Market(Area.SE_4,Sweden)
+    #sweden2 = Market(Area.SE_2,Sweden)
+    #sweden3 = Market(Area.SE_3,Sweden)
+    #sweden4 = Market(Area.SE_4,Sweden)
     markets_List = [value for key, value in vars().items() if isinstance(value, Market)]
 
     @staticmethod
     def get_Market_by_area_code(area_code: str) -> Optional[Market]:
         for country in Markets.markets_List:
             if country.country_code == area_code:
                 return country
```

### Comparing `spotON_sdk-0.0.3.1/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.3.2/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.1/spotON_sdk/logic/Entsoe_query.py` & `spotON_sdk-0.0.3.2/spotON_sdk/logic/Entsoe_query.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.1/spotON_sdk/logic/dataframe_modifier.py` & `spotON_sdk-0.0.3.2/spotON_sdk/logic/dataframe_modifier.py`

 * *Files identical despite different names*

