# Comparing `tmp/jquants_api_client-1.1.2.tar.gz` & `tmp/jquants_api_client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jquants_api_client-1.1.2.tar", max compression
+gzip compressed data, was "jquants_api_client-1.2.0.tar", max compression
```

## Comparing `jquants_api_client-1.1.2.tar` & `jquants_api_client-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-04-27 04:50:47.685389 jquants_api_client-1.1.2/LICENSE
--rw-r--r--   0        0        0     5631 2023-04-27 04:50:47.685389 jquants_api_client-1.1.2/README.md
--rw-r--r--   0        0        0       66 2023-04-27 04:50:47.685389 jquants_api_client-1.1.2/jquantsapi/__init__.py
--rw-r--r--   0        0        0    54334 2023-04-27 04:50:47.685389 jquants_api_client-1.1.2/jquantsapi/client.py
--rw-r--r--   0        0        0    15206 2023-04-27 04:50:47.685389 jquants_api_client-1.1.2/jquantsapi/constants.py
--rw-r--r--   0        0        0      517 2023-04-27 04:50:47.685389 jquants_api_client-1.1.2/jquantsapi/enums.py
--rw-r--r--   0        0        0     1676 2023-04-27 04:51:00.489623 jquants_api_client-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     7141 1970-01-01 00:00:00.000000 jquants_api_client-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 05:10:43.054810 jquants_api_client-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5631 2023-05-09 05:10:43.054810 jquants_api_client-1.2.0/README.md
+-rw-r--r--   0        0        0       66 2023-05-09 05:10:43.054810 jquants_api_client-1.2.0/jquantsapi/__init__.py
+-rw-r--r--   0        0        0    56245 2023-05-09 05:10:43.054810 jquants_api_client-1.2.0/jquantsapi/client.py
+-rw-r--r--   0        0        0    15273 2023-05-09 05:10:43.058810 jquants_api_client-1.2.0/jquantsapi/constants.py
+-rw-r--r--   0        0        0      517 2023-05-09 05:10:43.058810 jquants_api_client-1.2.0/jquantsapi/enums.py
+-rw-r--r--   0        0        0     1676 2023-05-09 05:11:01.715065 jquants_api_client-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7141 1970-01-01 00:00:00.000000 jquants_api_client-1.2.0/PKG-INFO
```

### Comparing `jquants_api_client-1.1.2/LICENSE` & `jquants_api_client-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.1.2/README.md` & `jquants_api_client-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.1.2/jquantsapi/client.py` & `jquants_api_client-1.2.0/jquantsapi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1558,7 +1558,68 @@
                 )
                 for s in dates
             ]
             for future in as_completed(futures):
                 df = future.result()
                 buff.append(df)
         return pd.concat(buff).sort_values(["Code", "Date"])
+
+    # /trading_calendar
+    def _get_markets_trading_calendar_raw(
+        self,
+        holiday_division: str = "",
+        from_yyyymmdd: str = "",
+        to_yyyymmdd: str = "",
+    ) -> str:
+        """
+        get trading calendar raw API returns
+
+        Args:
+            holiday_division: 休日区分
+            from_yyyymmdd: 取得開始日
+            to_yyyymmdd: 取得終了日
+
+        Returns:
+            str: trading calendar
+        """
+        url = f"{self.JQUANTS_API_BASE}/markets/trading_calendar"
+        params = {}
+        if holiday_division != "":
+            params["holidaydivision"] = holiday_division
+        if from_yyyymmdd != "":
+            params["from"] = from_yyyymmdd
+        if to_yyyymmdd != "":
+            params["to"] = to_yyyymmdd
+        ret = self._get(url, params)
+        ret.encoding = self.RAW_ENCODING
+        return ret.text
+
+    def get_markets_trading_calendar(
+        self,
+        holiday_division: str = "",
+        from_yyyymmdd: str = "",
+        to_yyyymmdd: str = "",
+    ) -> pd.DataFrame:
+        """
+        取引カレンダーを取得
+
+        Args:
+            holiday_division: 休日区分
+            from_yyyymmdd: 取得開始日
+            to_yyyymmdd: 取得終了日
+
+        Returns:
+            pd.DataFrame: 取り引きカレンダー (Date列でソートされています)
+        """
+        j = self._get_markets_trading_calendar_raw(
+            holiday_division=holiday_division,
+            from_yyyymmdd=from_yyyymmdd,
+            to_yyyymmdd=to_yyyymmdd,
+        )
+        d = json.loads(j)
+        df = pd.DataFrame.from_dict(d["trading_calendar"])
+        cols = constants.MARKETS_TRADING_CALENDAR
+        if len(df) == 0:
+            return pd.DataFrame([], columns=cols)
+        df["Date"] = pd.to_datetime(df["Date"], format="%Y-%m-%d")
+        df.sort_values(["Date"], inplace=True)
+        return df[cols]
```

### Comparing `jquants_api_client-1.1.2/jquantsapi/constants.py` & `jquants_api_client-1.2.0/jquantsapi/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,7 +463,12 @@
     "MorningOpen",
     "MorningHigh",
     "MorningLow",
     "MorningClose",
     "MorningVolume",
     "MorningTurnoverValue",
 ]
+
+MARKETS_TRADING_CALENDAR = [
+    "Date",
+    "HolidayDivision",
+]
```

### Comparing `jquants_api_client-1.1.2/jquantsapi/enums.py` & `jquants_api_client-1.2.0/jquantsapi/enums.py`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.1.2/pyproject.toml` & `jquants_api_client-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jquants-api-client"
-version = "1.1.2" # use poetry-dynamic-versioning
+version = "1.2.0" # use poetry-dynamic-versioning
 authors = [
     "J-Quants Project Contributors <j-quants@jpx.co.jp>",
 ]
 description = "J-Quants API Client Library"
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
```

### Comparing `jquants_api_client-1.1.2/PKG-INFO` & `jquants_api_client-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jquants-api-client
-Version: 1.1.2
+Version: 1.2.0
 Summary: J-Quants API Client Library
 Home-page: https://github.com/J-Quants/jquants-api-client-python
 License: Apache-2.0
 Keywords: jquants,api,client,J-Quants
 Author: J-Quants Project Contributors
 Author-email: j-quants@jpx.co.jp
 Requires-Python: >=3.7.1,<4.0.0
```

