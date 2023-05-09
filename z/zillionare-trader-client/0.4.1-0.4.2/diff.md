# Comparing `tmp/zillionare_trader_client-0.4.1.tar.gz` & `tmp/zillionare_trader_client-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillionare_trader_client-0.4.1.tar", max compression
+gzip compressed data, was "zillionare_trader_client-0.4.2.tar", max compression
```

## Comparing `zillionare_trader_client-0.4.1.tar` & `zillionare_trader_client-0.4.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1068 2023-04-04 02:55:06.813294 zillionare_trader_client-0.4.1/LICENSE
--rw-r--r--   0        0        0     1752 2023-04-04 02:55:06.813294 zillionare_trader_client-0.4.1/README.md
--rw-r--r--   0        0        0     2513 2023-05-06 07:21:53.012380 zillionare_trader_client-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6831 2023-05-05 12:28:42.792689 zillionare_trader_client-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0     2191 2023-04-04 02:55:06.817294 zillionare_trader_client-0.4.1/tests/data/bars_1d.pkl
--rw-r--r--   0        0        0   408697 2023-04-04 02:55:06.825294 zillionare_trader_client-0.4.1/tests/data/bars_1m.pkl
--rw-r--r--   0        0        0    56389 2023-05-05 09:15:16.952210 zillionare_trader_client-0.4.1/tests/data/calendar.json
--rw-r--r--   0        0        0      881 2023-05-05 09:05:10.906134 zillionare_trader_client-0.4.1/tests/data/defaults.yaml
--rw-r--r--   0        0        0      931 2023-04-04 02:55:06.825294 zillionare_trader_client-0.4.1/tests/data/hljh_1d.csv
--rw-r--r--   0        0        0   214231 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/data/hljh_1m.csv
--rw-r--r--   0        0        0      303 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/data/hljh_limits.csv
--rw-r--r--   0        0        0      902 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/data/limits.csv
--rw-r--r--   0        0        0     1078 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/data/limits.pkl
--rw-r--r--   0        0        0      438 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/data/readme.md
--rw-r--r--   0        0        0      896 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/data/tyst_1d.csv
--rw-r--r--   0        0        0   207056 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/data/tyst_1m.csv
--rw-r--r--   0        0        0      315 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/data/tyst_limits.csv
--rw-r--r--   0        0        0     1339 2023-05-05 09:31:56.254023 zillionare_trader_client-0.4.1/tests/helper.py
--rw-r--r--   0        0        0     4117 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/performance.py
--rw-r--r--   0        0        0    10301 2023-05-05 10:59:19.119637 zillionare_trader_client-0.4.1/tests/test_traderclient.py
--rw-r--r--   0        0        0     1620 2023-05-05 12:07:44.696724 zillionare_trader_client-0.4.1/tests/test_transport.py
--rw-r--r--   0        0        0      183 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.1/traderclient/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.1/traderclient/cli.py
--rw-r--r--   0        0        0    29101 2023-05-06 06:53:48.601741 zillionare_trader_client-0.4.1/traderclient/client.py
--rw-r--r--   0        0        0      487 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.1/traderclient/datatypes.py
--rw-r--r--   0        0        0     6983 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.1/traderclient/demo.py
--rw-r--r--   0        0        0      350 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.1/traderclient/errors.py
--rw-r--r--   0        0        0     3750 2023-05-06 06:54:02.837816 zillionare_trader_client-0.4.1/traderclient/transport.py
--rw-r--r--   0        0        0     1572 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.1/traderclient/utils.py
--rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 zillionare_trader_client-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-04 02:55:06.813294 zillionare_trader_client-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1752 2023-04-04 02:55:06.813294 zillionare_trader_client-0.4.2/README.md
+-rw-r--r--   0        0        0     2513 2023-05-09 11:52:53.635475 zillionare_trader_client-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     6831 2023-05-05 12:28:42.792689 zillionare_trader_client-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     2191 2023-04-04 02:55:06.817294 zillionare_trader_client-0.4.2/tests/data/bars_1d.pkl
+-rw-r--r--   0        0        0   408697 2023-04-04 02:55:06.825294 zillionare_trader_client-0.4.2/tests/data/bars_1m.pkl
+-rw-r--r--   0        0        0    56389 2023-05-05 09:15:16.952210 zillionare_trader_client-0.4.2/tests/data/calendar.json
+-rw-r--r--   0        0        0      881 2023-05-05 09:05:10.906134 zillionare_trader_client-0.4.2/tests/data/defaults.yaml
+-rw-r--r--   0        0        0      931 2023-04-04 02:55:06.825294 zillionare_trader_client-0.4.2/tests/data/hljh_1d.csv
+-rw-r--r--   0        0        0   214231 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/data/hljh_1m.csv
+-rw-r--r--   0        0        0      303 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/data/hljh_limits.csv
+-rw-r--r--   0        0        0      902 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/data/limits.csv
+-rw-r--r--   0        0        0     1078 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/data/limits.pkl
+-rw-r--r--   0        0        0      438 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/data/readme.md
+-rw-r--r--   0        0        0      896 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/data/tyst_1d.csv
+-rw-r--r--   0        0        0   207056 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/data/tyst_1m.csv
+-rw-r--r--   0        0        0      315 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/data/tyst_limits.csv
+-rw-r--r--   0        0        0     1339 2023-05-05 09:31:56.254023 zillionare_trader_client-0.4.2/tests/helper.py
+-rw-r--r--   0        0        0     4117 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.2/tests/performance.py
+-rw-r--r--   0        0        0    10473 2023-05-09 11:06:48.224979 zillionare_trader_client-0.4.2/tests/test_traderclient.py
+-rw-r--r--   0        0        0     1620 2023-05-05 12:07:44.696724 zillionare_trader_client-0.4.2/tests/test_transport.py
+-rw-r--r--   0        0        0      183 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.2/traderclient/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.2/traderclient/cli.py
+-rw-r--r--   0        0        0    28929 2023-05-09 11:52:11.899518 zillionare_trader_client-0.4.2/traderclient/client.py
+-rw-r--r--   0        0        0      487 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.2/traderclient/datatypes.py
+-rw-r--r--   0        0        0     6983 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.2/traderclient/demo.py
+-rw-r--r--   0        0        0      350 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.2/traderclient/errors.py
+-rw-r--r--   0        0        0     3750 2023-05-06 06:54:02.837816 zillionare_trader_client-0.4.2/traderclient/transport.py
+-rw-r--r--   0        0        0     1572 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.2/traderclient/utils.py
+-rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 zillionare_trader_client-0.4.2/PKG-INFO
```

### Comparing `zillionare_trader_client-0.4.1/LICENSE` & `zillionare_trader_client-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/README.md` & `zillionare_trader_client-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/pyproject.toml` & `zillionare_trader_client-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "zillionare-trader-client"
-version = "0.4.1"
+version = "0.4.2"
 homepage = "https://github.com/zillionare/trader-client"
 description = "Zillionare Trader Client"
 authors = ["Aaron Yang <code@jieyu.ai>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `zillionare_trader_client-0.4.1/tests/__init__.py` & `zillionare_trader_client-0.4.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/tests/data/bars_1d.pkl` & `zillionare_trader_client-0.4.2/tests/data/bars_1d.pkl`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/tests/data/bars_1m.pkl` & `zillionare_trader_client-0.4.2/tests/data/bars_1m.pkl`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/tests/data/calendar.json` & `zillionare_trader_client-0.4.2/tests/data/calendar.json`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/tests/data/defaults.yaml` & `zillionare_trader_client-0.4.2/tests/data/defaults.yaml`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/tests/data/hljh_1d.csv` & `zillionare_trader_client-0.4.2/tests/data/hljh_1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/tests/data/hljh_1m.csv` & `zillionare_trader_client-0.4.2/tests/data/hljh_1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/tests/data/limits.csv` & `zillionare_trader_client-0.4.2/tests/data/limits.csv`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/tests/data/limits.pkl` & `zillionare_trader_client-0.4.2/tests/data/limits.pkl`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/tests/data/tyst_1d.csv` & `zillionare_trader_client-0.4.2/tests/data/tyst_1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/tests/data/tyst_1m.csv` & `zillionare_trader_client-0.4.2/tests/data/tyst_1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/tests/helper.py` & `zillionare_trader_client-0.4.2/tests/helper.py`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/tests/performance.py` & `zillionare_trader_client-0.4.2/tests/performance.py`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/tests/test_traderclient.py` & `zillionare_trader_client-0.4.2/tests/test_traderclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,38 +108,41 @@
         self.assertAlmostEqual(balance["available"], 995289.528, 2)
         self.assertAlmostEqual(balance["market_value"], 4750, 2)
         self.assertAlmostEqual(balance["assets"], 1000039.528, 2)
         self.assertAlmostEqual(balance["pnl"], 39.5289, 2)
         self.assertAlmostEqual(balance["ppnl"], 39.5289 / 1_000_000, 2)
 
     def test_positions(self):
-        # this also test available_shares
-        positions = self.client.positions
+        # this will test available_shares too
+        positions = self.client.get_positions()
         self.assertEqual(0, positions.size)
 
         self.client.buy(
             "002537.XSHE", 10, 500, order_time=datetime.datetime(2022, 3, 1, 10, 4)
         )
 
-        positions = self.client.positions
+        positions = self.client.get_positions()
         self.assertListEqual(positions["security"].tolist(), ["002537.XSHE"])
         self.assertListEqual(positions["shares"].tolist(), [500])
         self.assertListEqual(positions["sellable"].tolist(), [0])
         np.testing.assert_array_almost_equal(positions["price"], [9.42], decimal=2)
 
         positions = self.client.get_positions(datetime.date(2022, 3, 7))
         self.assertListEqual(positions["security"].tolist(), ["002537.XSHE"])
         self.assertListEqual(positions["shares"].tolist(), [500])
         self.assertListEqual(positions["sellable"].tolist(), [500])
         np.testing.assert_array_almost_equal(positions["price"], [9.42], decimal=2)
 
-        # last_tradeday is still 2022, 3, 1, so the available_shares is 0
-        r = self.client.available_shares("002537.XSHE")
+        # last_trade day is still 2022, 3, 1, so the available_shares is 0
+        r = self.client.available_shares("002537.XSHE", datetime.date(2022, 3, 1))
         self.assertEqual(r, 0)
 
+        r = self.client.available_shares("002537.XSHE", datetime.date(2022, 3, 7))
+        self.assertEqual(r, 500.0)
+
     def test_market_buy(self):
         r = self.client.market_buy(
             "002537.XSHE", 500, order_time=datetime.datetime(2022, 3, 1, 10, 4)
         )
 
         self.assertEqual(r["security"], "002537.XSHE")
         self.assertAlmostEqual(r["price"], 9.420000076293945, 2)
@@ -261,15 +264,15 @@
         self.assertEqual(r["filled"], 500)
         self.assertEqual(r["time"], date)
 
         # first call, info should be invoked
         self.assertAlmostEqual(self.client.available_money, 995289.53, 2)
         self.assertTrue(self.client._is_dirty == False)
 
-        shares = self.client.available_shares("002537.XSHE")
+        shares = self.client.available_shares("002537.XSHE", dt=date)
         self.assertEqual(shares, 0)
         with mock.patch("traderclient.client.TraderClient.info") as mocked:
             # 第二次调用，不从远端取
             self.client.available_money
             mocked.assert_not_called()
 
         # no price provided, market buy
```

### Comparing `zillionare_trader_client-0.4.1/tests/test_transport.py` & `zillionare_trader_client-0.4.2/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/traderclient/client.py` & `zillionare_trader_client-0.4.2/traderclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,26 +175,14 @@
         if self._is_backtest:
             return self._principal
 
         url = self._cmd_url("info")
         r = get(url, headers=self.headers)
         return r.get("principal")
 
-    @property
-    def positions(self):
-        """当前账户最新持仓"""
-        if self._is_dirty or self._positions is None:
-            url = self._cmd_url("positions")
-
-            r = get(url, headers=self.headers)
-
-            self._positions = r
-
-        return self._positions
-
     def get_positions(self, dt: Optional[datetime.date] = None) -> np.ndarray:
         """取该子账户当前持仓信息
 
         Warning:
             在回测模式下，持仓信息不包含alias字段
 
         Args:
@@ -204,31 +192,31 @@
         """
         url = self._cmd_url("positions")
 
         r = get(url, params={"date": dt}, headers=self.headers)
 
         return r
 
-    def available_shares(self, security: str) -> int:
-        """返回某支股票当前可用数量
-
-        在回测模式下，使用持仓表最后一日的记录进行过滤。
+    def available_shares(
+        self, security: str, dt: Optional[datetime.date] = None
+    ) -> float:
+        """返回某支股票在`dt`日的可售数量
 
         Args:
             security: 股票代码
+            dt: 持仓查询日期。在实盘下可为None，表明取最新持仓。
 
         Returns:
-            int: 指定股票今日可卖数量，无可卖即为0
+            float: 指定股票在`dt`日可卖数量，无可卖即为0
         """
-        if self._is_dirty or self._positions is None:
-            url = self._cmd_url("positions")
+        if self._is_backtest and dt is None:
+            raise ValueError("`dt` is required under backtest!")
 
-            r = get(url, headers=self.headers)
-
-            self._positions = r
+        if self._is_dirty or self._positions is None:
+            self._positions = self.get_positions(dt)
             # 此时持仓虽然同步了，但其它数据，比如cash并未同步，所以不能更改_is_dirty状态
 
         found = self._positions[self._positions["security"] == security]
         if found.size == 1:
             return found["sellable"][0].item()
         elif found.size == 0:
             return 0
@@ -285,15 +273,15 @@
         timeout: float = 0.5,
         order_time: Optional[datetime.datetime] = None,
         **kwargs,
     ) -> Dict:
         """按金额买入股票。
 
         Returns:
-            参考[buy][traderclient.client.buy]
+            参考[buy][traderclient.client.TraderClient.buy]
         """
         order_time = order_time or datetime.datetime.now()
 
         if price is None:
             price = await self._get_market_buy_price(security, order_time)
             volume = int(money / price / 100) * 100
 
@@ -627,15 +615,15 @@
             time_out (int, optional): 缺省超时为0.5秒
             order_time: 下单时间。在回测模式下使用。
 
         Returns:
             Union[List, Dict]: 股票卖出委托单的详细信息，于sell指令相同
         """
         if percent <= 0 or percent > 1:
-            raise ValueError(f"percent should between [0, 1]")
+            raise ValueError("percent should between [0, 1]")
         if len(security) < 6:
             raise ValueError(f"wrong security format {security}")
 
         url = self._cmd_url("sell_percent")
         parameters = {
             "security": security,
             "price": price,
@@ -667,15 +655,15 @@
             percent (float): 调用者给出的百分比，(0, 1]
             time_out (int, optional): 缺省超时为0.5秒
 
         Returns:
             List: 所有卖出股票的委托单信息，于sell指令相同
         """
         if percent <= 0 or percent > 1:
-            raise ValueError(f"percent should between [0, 1]")
+            raise ValueError("percent should between [0, 1]")
 
         url = self._cmd_url("sell_all")
         parameters = {"percent": percent, "timeout": timeout}
 
         self._is_dirty = True
         return post_json(url, params=parameters, headers=self.headers)
```

### Comparing `zillionare_trader_client-0.4.1/traderclient/demo.py` & `zillionare_trader_client-0.4.2/traderclient/demo.py`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/traderclient/transport.py` & `zillionare_trader_client-0.4.2/traderclient/transport.py`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/traderclient/utils.py` & `zillionare_trader_client-0.4.2/traderclient/utils.py`

 * *Files identical despite different names*

### Comparing `zillionare_trader_client-0.4.1/PKG-INFO` & `zillionare_trader_client-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillionare-trader-client
-Version: 0.4.1
+Version: 0.4.2
 Summary: Zillionare Trader Client
 Home-page: https://github.com/zillionare/trader-client
 License: MIT
 Author: Aaron Yang
 Author-email: code@jieyu.ai
 Requires-Python: >=3.8,<3.9
 Classifier: Development Status :: 2 - Pre-Alpha
```

