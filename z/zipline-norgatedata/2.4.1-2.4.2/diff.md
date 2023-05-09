# Comparing `tmp/zipline_norgatedata-2.4.1-py3-none-any.whl.zip` & `tmp/zipline_norgatedata-2.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 36240 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat     9308 b- defN 23-May-01 01:30 zipline_norgatedata/CHANGES.txt
+Zip file size: 36977 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat     9474 b- defN 23-May-08 07:24 zipline_norgatedata/CHANGES.txt
 -rw-rw-rw-  2.0 fat    16020 b- defN 20-Sep-09 09:35 zipline_norgatedata/LICENSE.txt
 -rw-rw-rw-  2.0 fat       62 b- defN 19-Aug-27 04:23 zipline_norgatedata/__init__.py
 -rw-rw-rw-  2.0 fat    10981 b- defN 23-May-01 11:22 zipline_norgatedata/pipelines.py
--rw-rw-rw-  2.0 fat       23 b- defN 23-May-07 10:02 zipline_norgatedata/version.py
+-rw-rw-rw-  2.0 fat       23 b- defN 23-May-09 12:01 zipline_norgatedata/version.py
 -rw-rw-rw-  2.0 fat    43970 b- defN 23-May-05 08:06 zipline_norgatedata/zipline_norgatedata.py
--rw-rw-rw-  2.0 fat    16020 b- defN 23-May-07 10:03 zipline_norgatedata-2.4.1.dist-info/LICENSE.TXT
--rw-rw-rw-  2.0 fat    25839 b- defN 23-May-07 10:03 zipline_norgatedata-2.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 10:03 zipline_norgatedata-2.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-May-07 10:03 zipline_norgatedata-2.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      990 b- defN 23-May-07 10:03 zipline_norgatedata-2.4.1.dist-info/RECORD
-11 files, 123325 bytes uncompressed, 34542 bytes compressed:  72.0%
+-rw-rw-rw-  2.0 fat    16020 b- defN 23-May-09 12:02 zipline_norgatedata-2.4.2.dist-info/LICENSE.TXT
+-rw-rw-rw-  2.0 fat    28339 b- defN 23-May-09 12:02 zipline_norgatedata-2.4.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-09 12:02 zipline_norgatedata-2.4.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-May-09 12:02 zipline_norgatedata-2.4.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      990 b- defN 23-May-09 12:02 zipline_norgatedata-2.4.2.dist-info/RECORD
+11 files, 125991 bytes uncompressed, 35279 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: zipline_norgatedata/version.py
 Comment: 
 
 Filename: zipline_norgatedata/zipline_norgatedata.py
 Comment: 
 
-Filename: zipline_norgatedata-2.4.1.dist-info/LICENSE.TXT
+Filename: zipline_norgatedata-2.4.2.dist-info/LICENSE.TXT
 Comment: 
 
-Filename: zipline_norgatedata-2.4.1.dist-info/METADATA
+Filename: zipline_norgatedata-2.4.2.dist-info/METADATA
 Comment: 
 
-Filename: zipline_norgatedata-2.4.1.dist-info/WHEEL
+Filename: zipline_norgatedata-2.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: zipline_norgatedata-2.4.1.dist-info/top_level.txt
+Filename: zipline_norgatedata-2.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: zipline_norgatedata-2.4.1.dist-info/RECORD
+Filename: zipline_norgatedata-2.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zipline_norgatedata/CHANGES.txt

```diff
@@ -108,8 +108,12 @@
 v2.2.9 20220715 Documentation change only - force install of iso3166 package to 2.0.2 due to change in name of "Turkey"
 v2.2.10 20220728 Updated iso3166 to be installed via mamba instead of pip
 v2.3.0 20220728 Bump to v2.3.0 due to version checking issue
 v2.3.1 20221027 Added Mac M1/M2 workaround to docs
 v2.3.2 20221114 Notes on Juneteenth holiday patch
 v2.3.3 20230122 Notes on TSXFailures patch
 v2.3.4 20230222 Update documentation to specify sqlalchemy<2
-v2.4.0 20230501 Change to zipline-reloaded and pyfolio-reloaded via conda-forge
+v2.4.0 20230506 Change to zipline-reloaded and pyfolio-reloaded via conda-forge
+v2.4.1 20230507 Minor documentation fixes on installation method
+v2.4.1 20230507 Documentation fixes
+v2.4.2 20230507 Documentation fixes, revised Clenow scripts
+
```

## zipline_norgatedata/version.py

```diff
@@ -1 +1 @@
-__version__ = '2.4.1'
+__version__ = '2.4.2'
```

## Comparing `zipline_norgatedata-2.4.1.dist-info/LICENSE.TXT` & `zipline_norgatedata-2.4.2.dist-info/LICENSE.TXT`

 * *Files identical despite different names*

## Comparing `zipline_norgatedata-2.4.1.dist-info/METADATA` & `zipline_norgatedata-2.4.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline-norgatedata
-Version: 2.4.1
+Version: 2.4.2
 Summary: Zipline extension to provide bundles of data from Norgate Data into the Zipline algorithmic trading library for the Python programming language
 Home-page: https://norgatedata.com
 Author: NorgateData Pty Ltd
 Author-email: support@norgatedata.com
 License: EULA
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Development Status :: 5 - Production/Stable
@@ -81,41 +81,94 @@
 
 ```sh
 pip install zipline-norgatedata --upgrade
 ```
 
 # Exchange Calendar Issues that require patching
 
-Norgate Data has developed the following patches.  Please make sure you implement all of them (most support messages we get are from people that have forgotten to patch all of the files).
+Norgate Data has developed the following patches.  Please make sure you implement the ones applicable to you.
 
-## Patch to add 17 Dec 2008 as holiday for CA Equities
+## Patch to allow backtesting before 20 years ago
 
-On this date, TSX had a major outage and was halted not long after the open, and never reopened.  In general, the financial industry has written off this day as a bust for the purposes of data analysis.
+Unfortunately this is hardcoded into exchange_calendars for some reason.  To extend backtesting beyond more than 20 years from today:
 
+Navigate to the exchange_calendars folder within site packages.  This is typically located at **C:\Users\<your username>\miniconda3\envs\zip310\Lib\site-packages\exchange_calendars**
 
+Edit exchange_calendars.py
+
+Go to line 51 and change:
+```
+GLOBAL_DEFAULT_START = pd.Timestamp.now().floor("D") - pd.DateOffset(years=20)
+```
+to the following (or your desired date)
+```
+GLOBAL_DEFAULT_START = pd.Timestamp('1950-01-03')
+```
+
+## Patch to allow calendars other than US calendars for backtesting
+
+If you see the message "AssertionError: All readers must share target trading_calendar." then you probably need this patch.  Our testing shows that AU and CA stocks users need this.
+
+Navigate to the zipline folder within site packages.  This is typically located at **C:\Users\<your username>\miniconda3\envs\zip310\Lib\site-packages\zipline**
+
+Navigate to the data subfolder and edit the file dipatch_bar_reader.py
+
+Locate the code (around line 50)
+```
+            assert trading_calendar == r.trading_calendar, (
+                "All readers must share target trading_calendar. "
+                "Reader={0} for type={1} uses calendar={2} which does not "
+                "match the desired shared calendar={3} ".format(
+                    r, t, r.trading_calendar, trading_calendar
+                )
+            )
+```
+
+Change it to:
+```
+        assert isinstance(trading_calendar, type(r.trading_calendar)), \
+	        "All readers must share target trading_calendar. " \
+	        "Reader={0} for type={1} uses calendar={2} which does not " \
+	        "match the desired shared calendar={3} ".format(
+	            r, t, r.trading_calendar, trading_calendar)
+```
+
+(For further details, see https://github.com/quantopian/zipline/issues/2684 - this has been an issue for some time and the original solution doesn't address the issue since there are actually two instances of the calendar - one from run_algorithm and one from the register_bundle within extension.py)
+
+
+## Patches for Canadian equities
+
+Of you are a Canadian Stocks user, you probably want to add this as a holiday:
+
+On 17 Dec 2008, TSX had a major outage and was halted not long after the open, and never reopened.  In general, the financial industry has written off this day as a bust for the purposes of data analysis.
+
+The New Years observance shift to Monday only started in 2000.
+
+
+Navigate to the exchange_calendars folder within site packages.  This is typically located at **C:\Users\<your username>\miniconda3\envs\zip310\Lib\site-packages\exchange_calendars**
 Edit exchange_calendar_xtse.py
-Add the following at line 98:
+Add the following at line 95:
 
 ```
 # Significant failures where TSX was, for practical purposes, closed for the entire day
-TSXFailures = [pd.Timestamp("2008-12-17", tz=UTC),]
+TSXFailure20081217 = pd.Timestamp("2008-12-17")
 ```
 
-Edit exchange_calendar_nys.py
+Edit exchange_calendar_xtse.py
 change the following at line 164:
 
 ```
-                September11ClosingsCanada
+        return list(chain(September11ClosingsCanada))
 
 ```
 
 to:
 
 ```
-                September11ClosingsCanada, TSXFailures
+        return list(chain(September11ClosingsCanada),TSXFailure20081217,)
 
 ```
 
 
 
 
 # Backtest Assumptions
@@ -536,26 +589,26 @@
 
 # Testing on Australian ASX data
 
 By default, run_algorithm uses the 'NYSE' trading calendar.  To backtest other markets, you need to specify the calendar.  For the ASX, the calendar name is XASX.    
 
 At the top of your algorithm:
 ```py
-from trading_calendars import get_calendar
+from exchange_calendars import get_calendar
 ```
 
 In the run_algorithm call, add a trading_calendar= line, for example:
 
 ```py
 results = run_algorithm(
     start=start, end=end, 
     initialize=initialize, analyze=analyze, 
     handle_data=handle_data, 
     capital_base=10000, 
-    trading_calendar=get_calendar('XASX'),
+    trading_calendar=get_calendar('XASX',start="1990-01-01"),
     data_frequency = 'daily', 
     bundle='norgatedata-spasx200',
 )
 ```
 
 # Testing on Canadian TSX data
 
@@ -570,29 +623,29 @@
 
 ```py
 results = run_algorithm(
     start=start, end=end, 
     initialize=initialize, analyze=analyze, 
     handle_data=handle_data, 
     capital_base=10000, 
-    trading_calendar=get_calendar('XTSE'),
+    trading_calendar=get_calendar('XTSE',start="1990-01-01"),
     data_frequency = 'daily', 
     bundle='norgatedata-sptsx60',
 )
 ```
 
 Be sure to implement the trading_calendars patch mentioned above too.
 
 # Books/publications that use Zipline, adapted for Norgate Data use
 
 We have adapted the Python code in the following books to use Norgate Data.  
 [Trading Evoled:  Anyone can Build Killer Trading Strategies in Python](https://www.followingthetrend.com/trading-evolved/).  
 
 Source code compatible with Zipline (Reloaded) v2.4 in Jupyter notebook format, can be downloaded here:
-https://norgatedata.com/book-examples/trading-evolved/NorgateDataTradingEvolvedExamples.zipline240.zip
+https://norgatedata.com/book-examples/trading-evolved/NorgateDataTradingEvolvedExamples.zipline240.2.zip
 
 If there are other book/publications that use Zipline and worth adding here, let us know.
 
 # FAQs
 
 ### During a backtest I receive an error ValueError: 'Time Period' is not in list.  How do I fix this?
```

