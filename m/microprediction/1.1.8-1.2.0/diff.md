# Comparing `tmp/microprediction-1.1.8.tar.gz` & `tmp/microprediction-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microprediction-1.1.8.tar", last modified: Wed Nov  9 16:57:51 2022, max compression
+gzip compressed data, was "microprediction-1.2.0.tar", last modified: Tue May  9 14:01:38 2023, max compression
```

## Comparing `microprediction-1.1.8.tar` & `microprediction-1.2.0.tar`

### file list

```diff
@@ -1,75 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:57:51.947082 microprediction-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    10264 2022-11-09 16:57:51.947082 microprediction-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9734 2022-11-09 16:57:36.000000 microprediction-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:57:51.943082 microprediction-1.1.8/microprediction/
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:57:51.943082 microprediction-1.1.8/microprediction/bespoke/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/bespoke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:57:51.943082 microprediction-1.1.8/microprediction/bespoke/crypto/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/bespoke/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/bespoke/crypto/cryptoconventions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:57:51.943082 microprediction-1.1.8/microprediction/bespoke/golf/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/bespoke/golf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/bespoke/golf/golfconventions.py
--rw-r--r--   0 runner    (1001) docker     (121)      669 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/bespoke/meme_stock.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:57:51.943082 microprediction-1.1.8/microprediction/bespoke/meme_stocks/
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/bespoke/meme_stocks/meme_stock.py
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/conventions.py
--rw-r--r--   0 runner    (1001) docker     (121)    38734 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/crawler.py
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/defaultcrawler.py
--rw-r--r--   0 runner    (1001) docker     (121)     9703 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/fitcrawler.py
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/install.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:57:51.947082 microprediction-1.1.8/microprediction/live/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/live/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3597 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/live/bart_delays.py
--rw-r--r--   0 runner    (1001) docker     (121)     3920 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/live/covid_news.py
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/live/crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     6618 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/live/faang.py
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/live/grains.py
--rw-r--r--   0 runner    (1001) docker     (121)     3650 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/live/iex.py
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/live/iexcredentials.py
--rw-r--r--   0 runner    (1001) docker     (121)     4390 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/live/nyc_bikes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/live/nyc_traffic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2778 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/live/seattle_wind.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/live/water_height.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/live/weightedmid.py
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/live/xrayportfolios.py
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/live/xrayprices.py
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/live/xraytickers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3773 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/looping.py
--rw-r--r--   0 runner    (1001) docker     (121)     3618 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/old_conventions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4236 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/onlinecrawler.py
--rw-r--r--   0 runner    (1001) docker     (121)    16369 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/polling.py
--rw-r--r--   0 runner    (1001) docker     (121)    12815 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     7772 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/reportingcrawler.py
--rw-r--r--   0 runner    (1001) docker     (121)    10153 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/samplers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3987 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/sequentialcrawler.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/set_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/simplecrawler.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/slack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2207 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/statefulcrawler.py
--rw-r--r--   0 runner    (1001) docker     (121)     8860 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/streamskater.py
--rw-r--r--   0 runner    (1001) docker     (121)     1979 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/supporter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:57:51.947082 microprediction-1.1.8/microprediction/univariate/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/univariate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/univariate/arrivals.py
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/univariate/cdfvalues.py
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/univariate/digestdist.py
--rw-r--r--   0 runner    (1001) docker     (121)     3280 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/univariate/distmachine.py
--rw-r--r--   0 runner    (1001) docker     (121)     3889 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/univariate/expnormdist.py
--rw-r--r--   0 runner    (1001) docker     (121)     3517 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/univariate/fitdist.py
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/univariate/normaldist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/univariate/processes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2044 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/univariate/runningmoments.py
--rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/univariate/skewdist.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/whereami.py
--rw-r--r--   0 runner    (1001) docker     (121)    19450 2022-11-09 16:57:36.000000 microprediction-1.1.8/microprediction/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:57:51.943082 microprediction-1.1.8/microprediction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10264 2022-11-09 16:57:51.000000 microprediction-1.1.8/microprediction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2225 2022-11-09 16:57:51.000000 microprediction-1.1.8/microprediction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 16:57:51.000000 microprediction-1.1.8/microprediction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-11-09 16:57:51.000000 microprediction-1.1.8/microprediction.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-11-09 16:57:51.000000 microprediction-1.1.8/microprediction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-09 16:57:51.000000 microprediction-1.1.8/microprediction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-09 16:57:51.947082 microprediction-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-11-09 16:57:36.000000 microprediction-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:38.090517 microprediction-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-09 14:01:38.090517 microprediction-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-05-09 14:01:13.000000 microprediction-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:38.082517 microprediction-1.2.0/microprediction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:38.086517 microprediction-1.2.0/microprediction/bespoke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/bespoke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:38.086517 microprediction-1.2.0/microprediction/bespoke/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/bespoke/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/bespoke/crypto/cryptoconventions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:38.086517 microprediction-1.2.0/microprediction/bespoke/golf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/bespoke/golf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/bespoke/golf/golfconventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/bespoke/meme_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:38.086517 microprediction-1.2.0/microprediction/bespoke/meme_stocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/bespoke/meme_stocks/meme_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38734 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/defaultcrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9808 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/fitcrawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:38.086517 microprediction-1.2.0/microprediction/inclusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/inclusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/inclusion/scipyinclusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/inclusion/timemachinesinclusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/inclusion/tsainclusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/install.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:38.090517 microprediction-1.2.0/microprediction/live/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/bart_delays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/covid_news.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/faang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/grains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/iex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/iexcredentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/nyc_bikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/nyc_traffic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/pga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/rdpstickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/seattle_wind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/tradingday.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/water_height.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/weightedmid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/xrayportfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/xrayprices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/xraytickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/live/xraytickersdiscarded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/looping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/old_conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/onlinecrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/pollingutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18597 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/reportingcrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/sequentialcrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/set_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/simplecrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/statefulcrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/streamskater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/supporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:38.090517 microprediction-1.2.0/microprediction/univariate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/univariate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/univariate/arrivals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/univariate/cdfvalues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/univariate/digestdist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/univariate/distmachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/univariate/expnormdist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/univariate/fitdist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/univariate/normaldist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/univariate/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/univariate/runningmoments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/univariate/skewdist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/whereami.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19625 2023-05-09 14:01:13.000000 microprediction-1.2.0/microprediction/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:38.086517 microprediction-1.2.0/microprediction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-09 14:01:37.000000 microprediction-1.2.0/microprediction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-09 14:01:38.000000 microprediction-1.2.0/microprediction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:01:37.000000 microprediction-1.2.0/microprediction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-09 14:01:37.000000 microprediction-1.2.0/microprediction.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-09 14:01:37.000000 microprediction-1.2.0/microprediction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 14:01:37.000000 microprediction-1.2.0/microprediction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 14:01:38.090517 microprediction-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-09 14:01:13.000000 microprediction-1.2.0/setup.py
```

### Comparing `microprediction-1.1.8/PKG-INFO` & `microprediction-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,37 @@
-Metadata-Version: 2.1
-Name: microprediction
-Version: 1.1.8
-Summary: Client for www.microprediction.org turnkey community prediction
-Home-page: https://github.com/microprediction/microprediction
-Author: microprediction
-Author-email: info@microprediction.org
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
 
-
-# microprediction [docs](https://microprediction.github.io/microprediction/), [client](https://github.com/microprediction/microprediction) and [beer money](https://www.microprediction.org/leaderboard.html) ![deploy](https://github.com/microprediction/microprediction/workflows/deploy/badge.svg) 
+# microprediction [tldr](https://microprediction.github.io/microprediction/tldr), [docs](https://microprediction.github.io/microprediction/), [client](https://github.com/microprediction/microprediction) and [live leaderboards](https://www.microprediction.org/leaderboard.html) ![deploy](https://github.com/microprediction/microprediction/workflows/deploy/badge.svg) 
 Packages and a platform for effecting autonomous prediction using lightweight markets instead of models because:
+ 
+ - Markets are better at prediction than models - just harder to create and wield, until now.
+ - Small "microprediction" ([glossary](https://microprediction.github.io/microprediction/glossary)) markets are surprisingly accurate too, and even [chatGPT can create one](https://medium.com/geekculture/chatgpt-acquires-realtime-operational-intelligence-23675d2e0f3b).
 
- - *Markets are better at prediction than models* ([discuss](https://www.linkedin.com/posts/petercotton_tldr-activity-6983896509490610176-JTJB?utm_source=share&utm_medium=member_desktop)) - just harder to create and wield, until now. 
- - Small "microprediction" markets ([glossary](https://microprediction.github.io/microprediction/glossary)) are surprisingly accurate ([prove me wrong](https://github.com/microprediction/building_an_open_ai_network/discussions/19)).
-
+See [tldr](https://microprediction.github.io/microprediction/tldr) or just [instantly participate](https://microprediction.github.io/microprediction/setup) and you'll grok it, I promise.  
 ### Provocations (more in the [book](https://mitpress.mit.edu/books/microprediction))
 
-- No timeseries model should ever be called SOTA again ([discuss](https://www.linkedin.com/posts/petercotton_timeseries-forecasting-timeseriesanalysis-activity-6987561356862353408-iy2Z?utm_source=share&utm_medium=member_desktop)).  
-- Prediction capability shouldn't be limited by the capabilities of a single mind, algorithm or company ([discuss](https://www.linkedin.com/posts/petercotton_machinelearning-reinforcementlearning-datascience-activity-6992560556863803392-FOM6?utm_source=share&utm_medium=member_desktop)) 
+- A market beat 97% of participants in the M6 contest([post](https://www.linkedin.com/posts/petercotton_the-options-market-beat-94-of-participants-activity-7020917422085795840-Pox0?utm_source=share&utm_medium=member_desktop)) and [announcement](https://www.linkedin.com/posts/spyros-makridakis-b2ba5a52_congratulations-to-the-global-winners-of-activity-7028775981133791232-Mlzs?utm_source=share&utm_medium=member_desktop). 
+- No timeseries model should ever be called SOTA again. [Discuss](https://www.linkedin.com/posts/petercotton_timeseries-forecasting-timeseriesanalysis-activity-6987561356862353408-iy2Z?utm_source=share&utm_medium=member_desktop) and disagree but your argument [probably reduces to a contradiction](https://github.com/microprediction/building_an_open_ai_network/discussions/19).   
+- Modeling [is central planning](https://www.linkedin.com/posts/petercotton_feedback-activity-7029452936686489600-8iuX?utm_source=share&utm_medium=member_desktop), a fatal conceit. Why limit capabilities to a single mind, algorithm or company? 
 - Somebody's algorithm or data will find signal in your model residuals, someday ([instructions](https://microprediction.github.io/microprediction/residuals)).
 - Most of "AI" will be done analogously, eventually, though this will take work. See the [book](https://mitpress.mit.edu/books/microprediction) or [challenge me](https://github.com/microprediction/building_an_open_ai_network/discussions).
 
  
  ![](https://github.com/microprediction/microprediction/blob/master/docs/assets/images/cotton_microprediction_3d_down.png)
 
-## Try it out ([docs](https://microprediction.github.io/microprediction/) and live [help](https://microprediction.github.io/microprediction/meet.html))
+## Try it out ([docs](https://microprediction.github.io/microprediction/), [install](https://github.com/microprediction/microprediction/blob/master/INSTALL.md) and live [help](https://microprediction.github.io/microprediction/meet.html))
 
 If you would like to see how *easy* it is to wield a *new kind of market* to effect turnkey distributional prediction, see the [docs](https://microprediction.github.io/microprediction/) and, therein, observe that you can receive live [help](https://microprediction.github.io/microprediction/meet.html) getting started on Fridays, or in the [slack channel](https://microprediction.github.io/microprediction/slack.html). Key points:
 
- - The microprediction platform makes it [pretty trivial](https://microprediction.github.io/microprediction/publish.html) to initiate your own bespoke market.
+ - No barriers to entry. To predict, just open this [notebook](https://github.com/microprediction/microprediction/blob/master/notebook_examples_submission/enter_microprediction_contest.ipynb) and run it, or cut and paste a [one line bash command](https://microprediction.github.io/microprediction/setup). 
+ - The microprediction platform makes it [pretty trivial](https://microprediction.github.io/microprediction/publish.html) to initiate your own bespoke market too. Just ask Thomas Hjelde Thorensen who recently [posted](https://www.linkedin.com/posts/thomashthoresen_datascience-microprediction-timeseriesforecasting-activity-6999971006274514944-lDID?utm_source=share&utm_medium=member_desktop) about his experience. 
  - [Many algorithms](https://www.microprediction.org/leaderboard.html) already competing to predict [other streams](https://www.microprediction.org/browse_streams.html) can easily predict yours too. 
  - Many more will do so in the future. Anyone can [launch a new algorithm](https://microprediction.github.io/microprediction/predict.html) using anything they like in the Julia, R or Python [ecosystem](https://www.microprediction.com/blog/popular-timeseries-packages) for example (it's a data interface). 
- - If you have a CSV with historical data (one column per variable) you can just send it to me (chat in [slack](https://microprediction.github.io/microprediction/slack.html) say).   
+
+
+Too hard? If you have a CSV with historical data (one column per variable) you can just send it to me (chat in [slack](https://microprediction.github.io/microprediction/slack.html) say). You can also just grab data, see the [reader](https://github.com/microprediction/microprediction/blob/master/microprediction/reader.py).    
 
 # The [TimeMachines](https://github.com/microprediction/timemachines), [Precise](https://github.com/microprediction/precise), and [HumpDay](https://github.com/microprediction/humpday) packages 
 
 I also maintain three benchmarking packages to help me, and maybe you, surf the open-source wave. 
 
 | Topic                  | Package           | Elo ratings | Methods                                                                                                                                                                                  | Data sources | 
 |------------------------|-------------------|-------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------| 
@@ -85,10 +75,9 @@
 
 # About me ([home](https://github.com/microprediction/home))
   - [blog](https://microprediction.medium.com)
   - [slack channel](https://microprediction.github.io/microprediction/slack.html) 
   - [office hours](https://microprediction.github.io/microprediction/meet.html)
   - [papers, articles etc](https://github.com/microprediction/home)
 
-
-
-
+# Acknowledgements
+The live microprediction platform is supported by [Intech Investments](https://www.intechinvestments.com/) and not, as rumoured, the [Center for Artificial Artificial Intelligence](https://microprediction.github.io/microprediction/aai).
```

### Comparing `microprediction-1.1.8/README.md` & `microprediction-1.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,52 @@
+Metadata-Version: 2.1
+Name: microprediction
+Version: 1.2.0
+Summary: Client for www.microprediction.org turnkey community prediction
+Home-page: https://github.com/microprediction/microprediction
+Author: microprediction
+Author-email: info@microprediction.org
+License: MIT
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
 
-# microprediction [docs](https://microprediction.github.io/microprediction/), [client](https://github.com/microprediction/microprediction) and [beer money](https://www.microprediction.org/leaderboard.html) ![deploy](https://github.com/microprediction/microprediction/workflows/deploy/badge.svg) 
-Packages and a platform for effecting autonomous prediction using lightweight markets instead of models because:
 
- - *Markets are better at prediction than models* ([discuss](https://www.linkedin.com/posts/petercotton_tldr-activity-6983896509490610176-JTJB?utm_source=share&utm_medium=member_desktop)) - just harder to create and wield, until now. 
- - Small "microprediction" markets ([glossary](https://microprediction.github.io/microprediction/glossary)) are surprisingly accurate ([prove me wrong](https://github.com/microprediction/building_an_open_ai_network/discussions/19)).
+# microprediction [tldr](https://microprediction.github.io/microprediction/tldr), [docs](https://microprediction.github.io/microprediction/), [client](https://github.com/microprediction/microprediction) and [live leaderboards](https://www.microprediction.org/leaderboard.html) ![deploy](https://github.com/microprediction/microprediction/workflows/deploy/badge.svg) 
+Packages and a platform for effecting autonomous prediction using lightweight markets instead of models because:
+ 
+ - Markets are better at prediction than models - just harder to create and wield, until now.
+ - Small "microprediction" ([glossary](https://microprediction.github.io/microprediction/glossary)) markets are surprisingly accurate too, and even [chatGPT can create one](https://medium.com/geekculture/chatgpt-acquires-realtime-operational-intelligence-23675d2e0f3b).
 
+See [tldr](https://microprediction.github.io/microprediction/tldr) or just [instantly participate](https://microprediction.github.io/microprediction/setup) and you'll grok it, I promise.  
 ### Provocations (more in the [book](https://mitpress.mit.edu/books/microprediction))
 
-- No timeseries model should ever be called SOTA again ([discuss](https://www.linkedin.com/posts/petercotton_timeseries-forecasting-timeseriesanalysis-activity-6987561356862353408-iy2Z?utm_source=share&utm_medium=member_desktop)).  
-- Prediction capability shouldn't be limited by the capabilities of a single mind, algorithm or company ([discuss](https://www.linkedin.com/posts/petercotton_machinelearning-reinforcementlearning-datascience-activity-6992560556863803392-FOM6?utm_source=share&utm_medium=member_desktop)) 
+- A market beat 97% of participants in the M6 contest([post](https://www.linkedin.com/posts/petercotton_the-options-market-beat-94-of-participants-activity-7020917422085795840-Pox0?utm_source=share&utm_medium=member_desktop)) and [announcement](https://www.linkedin.com/posts/spyros-makridakis-b2ba5a52_congratulations-to-the-global-winners-of-activity-7028775981133791232-Mlzs?utm_source=share&utm_medium=member_desktop). 
+- No timeseries model should ever be called SOTA again. [Discuss](https://www.linkedin.com/posts/petercotton_timeseries-forecasting-timeseriesanalysis-activity-6987561356862353408-iy2Z?utm_source=share&utm_medium=member_desktop) and disagree but your argument [probably reduces to a contradiction](https://github.com/microprediction/building_an_open_ai_network/discussions/19).   
+- Modeling [is central planning](https://www.linkedin.com/posts/petercotton_feedback-activity-7029452936686489600-8iuX?utm_source=share&utm_medium=member_desktop), a fatal conceit. Why limit capabilities to a single mind, algorithm or company? 
 - Somebody's algorithm or data will find signal in your model residuals, someday ([instructions](https://microprediction.github.io/microprediction/residuals)).
 - Most of "AI" will be done analogously, eventually, though this will take work. See the [book](https://mitpress.mit.edu/books/microprediction) or [challenge me](https://github.com/microprediction/building_an_open_ai_network/discussions).
 
  
  ![](https://github.com/microprediction/microprediction/blob/master/docs/assets/images/cotton_microprediction_3d_down.png)
 
-## Try it out ([docs](https://microprediction.github.io/microprediction/) and live [help](https://microprediction.github.io/microprediction/meet.html))
+## Try it out ([docs](https://microprediction.github.io/microprediction/), [install](https://github.com/microprediction/microprediction/blob/master/INSTALL.md) and live [help](https://microprediction.github.io/microprediction/meet.html))
 
 If you would like to see how *easy* it is to wield a *new kind of market* to effect turnkey distributional prediction, see the [docs](https://microprediction.github.io/microprediction/) and, therein, observe that you can receive live [help](https://microprediction.github.io/microprediction/meet.html) getting started on Fridays, or in the [slack channel](https://microprediction.github.io/microprediction/slack.html). Key points:
 
- - The microprediction platform makes it [pretty trivial](https://microprediction.github.io/microprediction/publish.html) to initiate your own bespoke market.
+ - No barriers to entry. To predict, just open this [notebook](https://github.com/microprediction/microprediction/blob/master/notebook_examples_submission/enter_microprediction_contest.ipynb) and run it, or cut and paste a [one line bash command](https://microprediction.github.io/microprediction/setup). 
+ - The microprediction platform makes it [pretty trivial](https://microprediction.github.io/microprediction/publish.html) to initiate your own bespoke market too. Just ask Thomas Hjelde Thorensen who recently [posted](https://www.linkedin.com/posts/thomashthoresen_datascience-microprediction-timeseriesforecasting-activity-6999971006274514944-lDID?utm_source=share&utm_medium=member_desktop) about his experience. 
  - [Many algorithms](https://www.microprediction.org/leaderboard.html) already competing to predict [other streams](https://www.microprediction.org/browse_streams.html) can easily predict yours too. 
  - Many more will do so in the future. Anyone can [launch a new algorithm](https://microprediction.github.io/microprediction/predict.html) using anything they like in the Julia, R or Python [ecosystem](https://www.microprediction.com/blog/popular-timeseries-packages) for example (it's a data interface). 
- - If you have a CSV with historical data (one column per variable) you can just send it to me (chat in [slack](https://microprediction.github.io/microprediction/slack.html) say).   
+
+
+Too hard? If you have a CSV with historical data (one column per variable) you can just send it to me (chat in [slack](https://microprediction.github.io/microprediction/slack.html) say). You can also just grab data, see the [reader](https://github.com/microprediction/microprediction/blob/master/microprediction/reader.py).    
 
 # The [TimeMachines](https://github.com/microprediction/timemachines), [Precise](https://github.com/microprediction/precise), and [HumpDay](https://github.com/microprediction/humpday) packages 
 
 I also maintain three benchmarking packages to help me, and maybe you, surf the open-source wave. 
 
 | Topic                  | Package           | Elo ratings | Methods                                                                                                                                                                                  | Data sources | 
 |------------------------|-------------------|-------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------| 
@@ -70,8 +90,11 @@
 
 # About me ([home](https://github.com/microprediction/home))
   - [blog](https://microprediction.medium.com)
   - [slack channel](https://microprediction.github.io/microprediction/slack.html) 
   - [office hours](https://microprediction.github.io/microprediction/meet.html)
   - [papers, articles etc](https://github.com/microprediction/home)
 
+# Acknowledgements
+The live microprediction platform is supported by [Intech Investments](https://www.intechinvestments.com/) and not, as rumoured, the [Center for Artificial Artificial Intelligence](https://microprediction.github.io/microprediction/aai). 
+
```

### Comparing `microprediction-1.1.8/microprediction/__init__.py` & `microprediction-1.2.0/microprediction/__init__.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/bespoke/meme_stock.py` & `microprediction-1.2.0/microprediction/bespoke/meme_stock.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/bespoke/meme_stocks/meme_stock.py` & `microprediction-1.2.0/microprediction/bespoke/meme_stocks/meme_stock.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/conventions.py` & `microprediction-1.2.0/microprediction/conventions.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/crawler.py` & `microprediction-1.2.0/microprediction/crawler.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/fitcrawler.py` & `microprediction-1.2.0/microprediction/fitcrawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,16 @@
             if stored_params is None:
                 try:
                     changed = machine.fit(lagged_values=lagged_values, lagged_times=lagged_times)
                     if changed:
                         print('Found better params for ' + name)
                         pprint(machine.params)
                         print(' ', flush=True)
-                except AttributeError:
+                except (AttributeError, TypeError):
+                    print('There was an error trying to use machine.fit inside fitcrawler')
                     print('Keeping the same params for ' + name)
                     pprint(machine.params)
                     print(' ', flush=True)
 
         return changed
 
     def sample(self, lagged_values, lagged_times=None, name=None, delay=None, **ignored):
```

### Comparing `microprediction-1.1.8/microprediction/live/bart_delays.py` & `microprediction-1.2.0/microprediction/live/bart_delays.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/live/covid_news.py` & `microprediction-1.2.0/microprediction/live/covid_news.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/live/crypto.py` & `microprediction-1.2.0/microprediction/live/crypto.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/live/faang.py` & `microprediction-1.2.0/microprediction/live/faang.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/live/iex.py` & `microprediction-1.2.0/microprediction/live/iex.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,8 +96,9 @@
             print('There are ' + str(len(small)) + ' stocks considered too small ')
 
     return common
 
 
 if __name__=='__main__':
     from microprediction.config_private import IEX_KEY
-    print(iex_latest_prices(tickers=['meta'], api_key=IEX_KEY))
+    tickers = ["aapl","abbv","amzn","bac"]
+    print(iex_common_stock_with_balance_sheet_tickers(tickers=['googl'], api_key=IEX_KEY))
```

### Comparing `microprediction-1.1.8/microprediction/live/nyc_bikes.py` & `microprediction-1.2.0/microprediction/live/nyc_bikes.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/live/nyc_traffic.py` & `microprediction-1.2.0/microprediction/live/nyc_traffic.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/live/seattle_wind.py` & `microprediction-1.2.0/microprediction/live/seattle_wind.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/live/weightedmid.py` & `microprediction-1.2.0/microprediction/live/weightedmid.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/live/xrayprices.py` & `microprediction-1.2.0/microprediction/live/xrayprices.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/looping.py` & `microprediction-1.2.0/microprediction/looping.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/old_conventions.py` & `microprediction-1.2.0/microprediction/old_conventions.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/onlinecrawler.py` & `microprediction-1.2.0/microprediction/onlinecrawler.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/polling.py` & `microprediction-1.2.0/microprediction/polling.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     #  You may wish to override these methods
     # --------------------------------------------
 
     def logger(self, data):
         """ Called after each attempt to poll data and send it """
 
         self.recent.append(data)
-        if len(self.recent) > 100:
-            self.recent = self.recent[-100:]
+        if len(self.recent) > 10:
+            self.recent = self.recent[-10:]
         if self.verbose:
             data_to_print = dict([(k,shorten_lists(v)) for k,v in data.items()])
             pprint(data_to_print)
             print(' ', flush=True)
 
     def downtime(self):
         """ Also called after each attempt to send data """
@@ -88,24 +88,29 @@
     def task(self):
         """ Scheduled task that runs every interval minutes """
         start_time = time.time()
         data = {'start_time': str(datetime.datetime.now())}
         try:
             source_value = self.call_func()
         except Exception as e:
+            data.update({'exception':str(e),'exception_note':'call to call_func failed'})
             source_value = None
+
+        # Send the current value to the sub-routine that must decide whether to return
+        # changes or puke and return None (if the feed is cold, say)
         next_value = self.determine_next_value(source_value)
         data.update({'source_value': source_value,
-                     'next_value': next_value,
+                     'next_values': next_value,
                      'elapsed after polling': time.time() - start_time})
+        if next_value is None:
+            data.update({'explanation':'the feed will not publish as it is COLD'})
         res = self.touch(self.name) if next_value is None else self.set(name=self.name, value=next_value)
         data.update({'value': next_value, "res": res, 'elapsed after sending': time.time() - start_time})
         self.logger(data=data)
         self.downtime()
-        data.update({'elapsed after downtime': time.time() - start_time})
 
     def maybe_bolster_balance_by_mining(self):
         """ Mine just a little to avoid stream dying due to bankruptcy """
         if self.mine:
             balance = self.get_balance()
             if balance < 0:
                 muid_time = time.time()
@@ -128,14 +133,17 @@
         run_start_time = time.time()
         run_end_time = run_start_time + timeout
         while time.time() < run_end_time:
             st = int(round(time.time()))
             self.task()
             et = int(round(time.time()))
             sleep_time = (st - et) % (60 * self.interval)
+            if sleep_time==0:
+                sleep_time = 60 * self.interval
+            print('Sleeping for '+str(sleep_time)+' seconds. ', flush=True)
             time.sleep(sleep_time)
 
 
 class ChangePoll(MicroPoll):
     #    Illustrates predicting the change in a quantity ... when feed is not entirely reliable
     #    If we don't get good data from the feed or it appears to be stale, we don't publish the change
 
@@ -232,15 +240,15 @@
             return self.secondary_func(next_values, *self.secondary_func_args)
         elif isinstance(self.secondary_func_args, dict):
             return self.secondary_func(next_values, **self.secondary_func_args)
         else:
             return self.secondary_func(next_values)
 
     def task(self):
-        """ Scheduled task that runs every minute """
+        """ Scheduled task """
         start_time = time.time()
         data = {'start_time': str(datetime.datetime.now())}
         try:
             source_values = self.call_func()
         except Exception as e:
             source_values = None
         next_values = self.determine_next_values(source_values)
@@ -258,16 +266,17 @@
         if next_values is None:
             res = {'operation': 'touch', 'exec': [self.touch(name=name) for name in self.names]}
         elif self.with_copulas:
             res = self.cset(names=self.names, values=send_values)
         else:
             res = [self.set(name=name, value=value) for name, value in zip(self.names, send_values)]
 
-        data.update({'values': next_values, "res": res, 'elapsed after sending': time.time() - start_time})
-        self.logger(data=data)
+        data.update({'source_values':source_values,'next_values': next_values, "res": res, 'elapsed after sending': time.time() - start_time})
+        if False:
+            self.logger(data=data)
         self.downtime()
         data.update({'elapsed after downtime': time.time() - start_time})
 
 
 def default_change_criterion(old_values, new_values):
     return any([abs(pp - pv) > 1e-6 for pp, pv in zip(old_values, new_values)])
 
@@ -318,33 +327,60 @@
                 self.feed_state = MultiChangePoll.COLD
                 self.alert(message='Something amiss with feed')
                 return None
             else:
                 self.current_values = [float(source_value) for source_value in source_values]
                 value_changes = [float(current_value) - float(prev_value) for current_value, prev_value in
                                  zip(self.current_values, self.prev_values)]
-                material_changes = [abs(vc) > 1e-6 for vc in value_changes]
-                if sum(material_changes)<=self.min_change_count:
+                material_changes = [ int(abs(vc) > 1e-6) for vc in value_changes]
+                n_material_changes = sum(material_changes)
+                if n_material_changes < self.min_change_count:
                     self.feed_state = MultiChangePoll.COLD  # Feed is stale, don't judge
                     self.logger(
-                        {'type': 'feed_status', 'message': "****  Feed unchanged at " + str(datetime.datetime.now())})
+                        {'type': 'feed_status',
+                                 'n_material_changes':n_material_changes,
+                                 'min_change_count':self.min_change_count,
+                                 'Currently retrieved values':self.current_values,
+                                 'Previously retrieved values':self.prev_values,
+                                  'message': "****  Changes not material. Feed status WARM --> COLD at " + str(datetime.datetime.now())})
+                    return None
                 else:
-                    self.prev_values = self.current_values
+                    self.logger(
+                        {'type': 'feed_status',
+                         'n_material_changes': n_material_changes,
+                         'min_change_count': self.min_change_count,
+                         'message': "****  Changes were material. Feed status WARM --> WARM " + str(datetime.datetime.now())})
+                    self.prev_values = [ v for v in self.current_values ]
                     if self.change_func is not None:
                         altered_changes = self.call_change_func(value_changes=value_changes)
                     else:
                         altered_changes = [c for c in value_changes]
                     return altered_changes
 
         elif self.feed_state == MultiChangePoll.COLD:
             # Wait until feed is back up and values start changing
-            self.prev_prev = self.prev_values if self.prev_values else None
-            self.prev_values = source_values
+            self.prev_prev = [ v for v in self.prev_values ] if (self.prev_values is not None) else None
+            self.prev_values = [ v for v in source_values ] if (source_values is not None) else None
             if (self.prev_values is not None) and (self.prev_prev is not None):
                 material_changes = [abs(pp - pv) > 1e-6 for pp, pv in zip(self.prev_prev, self.prev_values)]
-                if sum(material_changes)>=self.min_change_count:
+                n_material_changes = sum(material_changes)
+                if n_material_changes>=self.min_change_count:
                     self.feed_state = MultiChangePoll.WARM
                     self.logger(
-                        {'type': 'feed_status', 'message': '**** Feed resumed at ' + str(datetime.datetime.now())})
+                        {'type': 'feed_status',
+                          'n_material_changes':n_material_changes,
+                          'min_change_count':self.min_change_count,
+                          'message': '**** Feed status COLD --> WARM at ' + str(datetime.datetime.now())})
+            elif self.prev_values is not None:
+                 self.logger(
+                        {'type': 'feed_status',
+                         'reason': 'The previously retrieved value was None, have to wait',
+                         'message': '**** Feed status COLD --> COLD, but values seen ' + str(datetime.datetime.now())})
+            elif self.prev_values is None:
+                  self.logger(
+                        {'type': 'feed_status',
+                         'reason': 'The currently retrieved value was None, have to wait',
+                         'message': '**** Feed status COLD --> COLD at ' + str(datetime.datetime.now()),
+                         'warning': '**** Warning: failed to get current value ' + str(datetime.datetime.now())})
             return None
         else:
             raise Exception('Brain failure')
```

### Comparing `microprediction-1.1.8/microprediction/reportingcrawler.py` & `microprediction-1.2.0/microprediction/reportingcrawler.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/samplers.py` & `microprediction-1.2.0/microprediction/samplers.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/sequentialcrawler.py` & `microprediction-1.2.0/microprediction/sequentialcrawler.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/set_config.py` & `microprediction-1.2.0/microprediction/set_config.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/simplecrawler.py` & `microprediction-1.2.0/microprediction/simplecrawler.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/statefulcrawler.py` & `microprediction-1.2.0/microprediction/statefulcrawler.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/streamskater.py` & `microprediction-1.2.0/microprediction/streamskater.py`

 * *Files 17% similar despite different names*

```diff
@@ -198,7 +198,36 @@
     def include_stream(self, name=None, **ignore):
         return ('~' not in name) and (('faang' in name) or ('gnaaf' in name))
 
     def include_delay(self, delay=None, name=None, **ignore):
         # Example of influencing choice of horizons to predict
         # We skip the shortest horizons
         return delay > self.DELAYS[1]
+
+
+class CompetitionsStreamSkater(StreamSkater):
+
+    # This hits only those streams in competitions
+
+    def __init__(self,**kwargs):
+        super().__init__(**kwargs)
+
+    def include_stream(self, name=None, **ignore):
+        return ('~' not in name) and (('faang' in name) or ('sateb_' in name) or ('gnaaf' in name) or ('c2' in name) or ('c5' in name)  or ('fathom' in name) or ('xray' in name) or ('yarx' in name) or ('electricity' in name))
+
+    def include_delay(self, delay=None, name=None, **ignore):
+        return delay>=self.delays[2]
+
+
+class CompetitiveSkatingFox(SkatingFox):
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+    def include_stream(self, name=None, **ignore):
+        return ('~' not in name) and (
+                    ('faang' in name) or ('sateb_' in name) or ('gnaaf' in name) or ('c2' in name) or (
+                        'c5' in name) or ('fathom' in name) or ('xray' in name) or ('yarx' in name) or (
+                                'electricity' in name))
+
+    def include_delay(self, delay=None, name=None, **ignore):
+        return delay >= self.delays[2]
```

### Comparing `microprediction-1.1.8/microprediction/supporter.py` & `microprediction-1.2.0/microprediction/supporter.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/univariate/arrivals.py` & `microprediction-1.2.0/microprediction/univariate/arrivals.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/univariate/digestdist.py` & `microprediction-1.2.0/microprediction/univariate/digestdist.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/univariate/distmachine.py` & `microprediction-1.2.0/microprediction/univariate/distmachine.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/univariate/expnormdist.py` & `microprediction-1.2.0/microprediction/univariate/expnormdist.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/univariate/fitdist.py` & `microprediction-1.2.0/microprediction/univariate/fitdist.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/univariate/processes.py` & `microprediction-1.2.0/microprediction/univariate/processes.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/univariate/runningmoments.py` & `microprediction-1.2.0/microprediction/univariate/runningmoments.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/univariate/skewdist.py` & `microprediction-1.2.0/microprediction/univariate/skewdist.py`

 * *Files identical despite different names*

### Comparing `microprediction-1.1.8/microprediction/writer.py` & `microprediction-1.2.0/microprediction/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,17 +49,21 @@
             return res.json()
 
     def get_home(self):
         res = requests.put(self.base_url + '/live/' + self.write_key)
         if res.status_code == 200:
             return res.json()
 
-    def set(self, name, value):
+    def set(self, name, value, with_percentiles=False):
         """ Create or update a stream """
-        res = requests.put(self.base_url + '/live/' + name, data={"write_key": self.write_key, "value": value})
+        if with_percentiles:
+            data = {"write_key": self.write_key, "value": value, "with_percentiles":"1"}
+        else:
+            data = {"write_key": self.write_key, "value": value}
+        res = requests.put(self.base_url + '/live/' + name, data)
         if res.status_code == 200:
             return res.json()
         elif res.status_code == 500:
             raise Exception("server error")
         else:
             err = self.get_errors()[:2]
             pprint.pprint(err)
```

### Comparing `microprediction-1.1.8/microprediction.egg-info/PKG-INFO` & `microprediction-1.2.0/microprediction.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 Metadata-Version: 2.1
 Name: microprediction
-Version: 1.1.8
+Version: 1.2.0
 Summary: Client for www.microprediction.org turnkey community prediction
 Home-page: https://github.com/microprediction/microprediction
 Author: microprediction
 Author-email: info@microprediction.org
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
 
-# microprediction [docs](https://microprediction.github.io/microprediction/), [client](https://github.com/microprediction/microprediction) and [beer money](https://www.microprediction.org/leaderboard.html) ![deploy](https://github.com/microprediction/microprediction/workflows/deploy/badge.svg) 
+# microprediction [tldr](https://microprediction.github.io/microprediction/tldr), [docs](https://microprediction.github.io/microprediction/), [client](https://github.com/microprediction/microprediction) and [live leaderboards](https://www.microprediction.org/leaderboard.html) ![deploy](https://github.com/microprediction/microprediction/workflows/deploy/badge.svg) 
 Packages and a platform for effecting autonomous prediction using lightweight markets instead of models because:
+ 
+ - Markets are better at prediction than models - just harder to create and wield, until now.
+ - Small "microprediction" ([glossary](https://microprediction.github.io/microprediction/glossary)) markets are surprisingly accurate too, and even [chatGPT can create one](https://medium.com/geekculture/chatgpt-acquires-realtime-operational-intelligence-23675d2e0f3b).
 
- - *Markets are better at prediction than models* ([discuss](https://www.linkedin.com/posts/petercotton_tldr-activity-6983896509490610176-JTJB?utm_source=share&utm_medium=member_desktop)) - just harder to create and wield, until now. 
- - Small "microprediction" markets ([glossary](https://microprediction.github.io/microprediction/glossary)) are surprisingly accurate ([prove me wrong](https://github.com/microprediction/building_an_open_ai_network/discussions/19)).
-
+See [tldr](https://microprediction.github.io/microprediction/tldr) or just [instantly participate](https://microprediction.github.io/microprediction/setup) and you'll grok it, I promise.  
 ### Provocations (more in the [book](https://mitpress.mit.edu/books/microprediction))
 
-- No timeseries model should ever be called SOTA again ([discuss](https://www.linkedin.com/posts/petercotton_timeseries-forecasting-timeseriesanalysis-activity-6987561356862353408-iy2Z?utm_source=share&utm_medium=member_desktop)).  
-- Prediction capability shouldn't be limited by the capabilities of a single mind, algorithm or company ([discuss](https://www.linkedin.com/posts/petercotton_machinelearning-reinforcementlearning-datascience-activity-6992560556863803392-FOM6?utm_source=share&utm_medium=member_desktop)) 
+- A market beat 97% of participants in the M6 contest([post](https://www.linkedin.com/posts/petercotton_the-options-market-beat-94-of-participants-activity-7020917422085795840-Pox0?utm_source=share&utm_medium=member_desktop)) and [announcement](https://www.linkedin.com/posts/spyros-makridakis-b2ba5a52_congratulations-to-the-global-winners-of-activity-7028775981133791232-Mlzs?utm_source=share&utm_medium=member_desktop). 
+- No timeseries model should ever be called SOTA again. [Discuss](https://www.linkedin.com/posts/petercotton_timeseries-forecasting-timeseriesanalysis-activity-6987561356862353408-iy2Z?utm_source=share&utm_medium=member_desktop) and disagree but your argument [probably reduces to a contradiction](https://github.com/microprediction/building_an_open_ai_network/discussions/19).   
+- Modeling [is central planning](https://www.linkedin.com/posts/petercotton_feedback-activity-7029452936686489600-8iuX?utm_source=share&utm_medium=member_desktop), a fatal conceit. Why limit capabilities to a single mind, algorithm or company? 
 - Somebody's algorithm or data will find signal in your model residuals, someday ([instructions](https://microprediction.github.io/microprediction/residuals)).
 - Most of "AI" will be done analogously, eventually, though this will take work. See the [book](https://mitpress.mit.edu/books/microprediction) or [challenge me](https://github.com/microprediction/building_an_open_ai_network/discussions).
 
  
  ![](https://github.com/microprediction/microprediction/blob/master/docs/assets/images/cotton_microprediction_3d_down.png)
 
-## Try it out ([docs](https://microprediction.github.io/microprediction/) and live [help](https://microprediction.github.io/microprediction/meet.html))
+## Try it out ([docs](https://microprediction.github.io/microprediction/), [install](https://github.com/microprediction/microprediction/blob/master/INSTALL.md) and live [help](https://microprediction.github.io/microprediction/meet.html))
 
 If you would like to see how *easy* it is to wield a *new kind of market* to effect turnkey distributional prediction, see the [docs](https://microprediction.github.io/microprediction/) and, therein, observe that you can receive live [help](https://microprediction.github.io/microprediction/meet.html) getting started on Fridays, or in the [slack channel](https://microprediction.github.io/microprediction/slack.html). Key points:
 
- - The microprediction platform makes it [pretty trivial](https://microprediction.github.io/microprediction/publish.html) to initiate your own bespoke market.
+ - No barriers to entry. To predict, just open this [notebook](https://github.com/microprediction/microprediction/blob/master/notebook_examples_submission/enter_microprediction_contest.ipynb) and run it, or cut and paste a [one line bash command](https://microprediction.github.io/microprediction/setup). 
+ - The microprediction platform makes it [pretty trivial](https://microprediction.github.io/microprediction/publish.html) to initiate your own bespoke market too. Just ask Thomas Hjelde Thorensen who recently [posted](https://www.linkedin.com/posts/thomashthoresen_datascience-microprediction-timeseriesforecasting-activity-6999971006274514944-lDID?utm_source=share&utm_medium=member_desktop) about his experience. 
  - [Many algorithms](https://www.microprediction.org/leaderboard.html) already competing to predict [other streams](https://www.microprediction.org/browse_streams.html) can easily predict yours too. 
  - Many more will do so in the future. Anyone can [launch a new algorithm](https://microprediction.github.io/microprediction/predict.html) using anything they like in the Julia, R or Python [ecosystem](https://www.microprediction.com/blog/popular-timeseries-packages) for example (it's a data interface). 
- - If you have a CSV with historical data (one column per variable) you can just send it to me (chat in [slack](https://microprediction.github.io/microprediction/slack.html) say).   
+
+
+Too hard? If you have a CSV with historical data (one column per variable) you can just send it to me (chat in [slack](https://microprediction.github.io/microprediction/slack.html) say). You can also just grab data, see the [reader](https://github.com/microprediction/microprediction/blob/master/microprediction/reader.py).    
 
 # The [TimeMachines](https://github.com/microprediction/timemachines), [Precise](https://github.com/microprediction/precise), and [HumpDay](https://github.com/microprediction/humpday) packages 
 
 I also maintain three benchmarking packages to help me, and maybe you, surf the open-source wave. 
 
 | Topic                  | Package           | Elo ratings | Methods                                                                                                                                                                                  | Data sources | 
 |------------------------|-------------------|-------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------| 
@@ -85,10 +90,11 @@
 
 # About me ([home](https://github.com/microprediction/home))
   - [blog](https://microprediction.medium.com)
   - [slack channel](https://microprediction.github.io/microprediction/slack.html) 
   - [office hours](https://microprediction.github.io/microprediction/meet.html)
   - [papers, articles etc](https://github.com/microprediction/home)
 
-
+# Acknowledgements
+The live microprediction platform is supported by [Intech Investments](https://www.intechinvestments.com/) and not, as rumoured, the [Center for Artificial Artificial Intelligence](https://microprediction.github.io/microprediction/aai).
```

### Comparing `microprediction-1.1.8/microprediction.egg-info/SOURCES.txt` & `microprediction-1.2.0/microprediction.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 microprediction/defaultcrawler.py
 microprediction/fitcrawler.py
 microprediction/install.py
 microprediction/looping.py
 microprediction/old_conventions.py
 microprediction/onlinecrawler.py
 microprediction/polling.py
+microprediction/pollingutil.py
 microprediction/reader.py
 microprediction/reportingcrawler.py
 microprediction/samplers.py
 microprediction/sequentialcrawler.py
 microprediction/set_config.py
 microprediction/simplecrawler.py
 microprediction/slack.py
@@ -31,30 +32,38 @@
 microprediction/bespoke/__init__.py
 microprediction/bespoke/meme_stock.py
 microprediction/bespoke/crypto/__init__.py
 microprediction/bespoke/crypto/cryptoconventions.py
 microprediction/bespoke/golf/__init__.py
 microprediction/bespoke/golf/golfconventions.py
 microprediction/bespoke/meme_stocks/meme_stock.py
+microprediction/inclusion/__init__.py
+microprediction/inclusion/scipyinclusion.py
+microprediction/inclusion/timemachinesinclusion.py
+microprediction/inclusion/tsainclusion.py
 microprediction/live/__init__.py
 microprediction/live/bart_delays.py
 microprediction/live/covid_news.py
 microprediction/live/crypto.py
 microprediction/live/faang.py
 microprediction/live/grains.py
 microprediction/live/iex.py
 microprediction/live/iexcredentials.py
 microprediction/live/nyc_bikes.py
 microprediction/live/nyc_traffic.py
+microprediction/live/pga.py
+microprediction/live/rdpstickers.py
 microprediction/live/seattle_wind.py
+microprediction/live/tradingday.py
 microprediction/live/water_height.py
 microprediction/live/weightedmid.py
 microprediction/live/xrayportfolios.py
 microprediction/live/xrayprices.py
 microprediction/live/xraytickers.py
+microprediction/live/xraytickersdiscarded.py
 microprediction/univariate/__init__.py
 microprediction/univariate/arrivals.py
 microprediction/univariate/cdfvalues.py
 microprediction/univariate/digestdist.py
 microprediction/univariate/distmachine.py
 microprediction/univariate/expnormdist.py
 microprediction/univariate/fitdist.py
```

### Comparing `microprediction-1.1.8/setup.py` & `microprediction-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="microprediction",
-    version="1.1.8",
+    version="1.2.0",
     description="Client for www.microprediction.org turnkey community prediction",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/microprediction/microprediction",
     author="microprediction",
     author_email="info@microprediction.org",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
-    packages=["microprediction", "microprediction.live", "microprediction.univariate", "microprediction.bespoke",
+    packages=["microprediction", "microprediction.live", "microprediction.inclusion","microprediction.univariate", "microprediction.bespoke",
               "microprediction.bespoke.meme_stocks","microprediction.bespoke.golf","microprediction.bespoke.crypto"],
     test_suite='pytest',
     tests_require=['pytest', 'scipy'],
     include_package_data=True,
-    install_requires=["numpy>=1.20.1", "pandas", "contexttimer", "requests",
+    install_requires=["numpy>=1.23.5", "pandas", "contexttimer", "requests",
                       "getjson>=2.0.0", "microconventions>=1.0.0","pytz>=2021.3",
                       'pycoingecko', 'tdigest','genson','hyperopt',
                       'scikit-learn','statsmodels','copulas'],
     entry_points={
         "console_scripts": [
             "microprediction=microprediction.__main__:main",
         ]
```

