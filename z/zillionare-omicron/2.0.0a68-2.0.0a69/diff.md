# Comparing `tmp/zillionare_omicron-2.0.0a68.tar.gz` & `tmp/zillionare_omicron-2.0.0a69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillionare_omicron-2.0.0a68.tar", max compression
+gzip compressed data, was "zillionare_omicron-2.0.0a69.tar", max compression
```

## Comparing `zillionare_omicron-2.0.0a68.tar` & `zillionare_omicron-2.0.0a69.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0      112 2023-01-24 12:41:24.903079 zillionare_omicron-2.0.0a68/AUTHORS.md
--rw-r--r--   0        0        0     1663 2023-05-08 08:54:41.853890 zillionare_omicron-2.0.0a68/HISTORY.md
--rw-r--r--   0        0        0     1068 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a68/LICENSE
--rw-r--r--   0        0        0     1331 2023-05-07 03:30:41.208098 zillionare_omicron-2.0.0a68/README.md
--rw-r--r--   0        0        0   503846 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/_static/Omicron_Windows10.docx
--rw-r--r--   0        0        0     5620 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a68/docs/_static/jetbrains-variant-3.svg
--rw-r--r--   0        0        0       84 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/dal/flux.md
--rw-r--r--   0        0        0      110 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/dal/influxclient.md
--rw-r--r--   0        0        0      189 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/dal/serialize.md
--rw-r--r--   0        0        0     5772 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/metrics.md
--rw-r--r--   0        0        0      203 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/omicron.md
--rw-r--r--   0        0        0       73 2023-05-08 07:55:54.700078 zillionare_omicron-2.0.0a68/docs/api/plotting/candlestick.md
--rw-r--r--   0        0        0       69 2023-05-08 07:55:45.740005 zillionare_omicron-2.0.0a68/docs/api/plotting/metrics.md
--rw-r--r--   0        0        0       68 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/security.md
--rw-r--r--   0        0        0       65 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/stock.md
--rw-r--r--   0        0        0       21 2023-05-07 03:32:19.736871 zillionare_omicron-2.0.0a68/docs/api/strategy.md
--rw-r--r--   0        0        0       58 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/talib.md
--rw-r--r--   0        0        0       57 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/api/timeframe.md
--rw-r--r--   0        0        0       66 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a68/docs/api/triggers.md
--rw-r--r--   0        0        0      907 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a68/docs/css/extra.css
--rw-r--r--   0        0        0     1778 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/developer.md
--rw-r--r--   0        0        0       43 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a68/docs/history.md
--rw-r--r--   0        0        0       42 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a68/docs/index.md
--rw-r--r--   0        0        0     1820 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/installation.md
--rw-r--r--   0        0        0     9823 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/docs/usage.md
--rw-r--r--   0        0        0      920 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/omicron/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a68/omicron/config/__init__.py
--rw-r--r--   0        0        0    56389 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/config/calendar.json
--rw-r--r--   0        0        0      441 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/config/defaults.yaml
--rw-r--r--   0        0        0      378 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/config/dev.yaml
--rw-r--r--   0        0        0     1334 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/config/schema.py
--rw-r--r--   0        0        0      816 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a68/omicron/config/sql/v0.6.sql
--rw-r--r--   0        0        0     2785 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/config/sql/v1.0.sql
--rw-r--r--   0        0        0       46 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a68/omicron/core/__init__.py
--rw-r--r--   0        0        0      140 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/core/constants.py
--rw-r--r--   0        0        0     1095 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/core/errors.py
--rw-r--r--   0        0        0       46 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/core/events.py
--rw-r--r--   0        0        0     6517 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/core/triggers.py
--rw-r--r--   0        0        0       71 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/dal/__init__.py
--rw-r--r--   0        0        0     3215 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/dal/cache.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/dal/influx/__init__.py
--rw-r--r--   0        0        0      370 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/dal/influx/errors.py
--rw-r--r--   0        0        0      996 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a68/omicron/dal/influx/escape.py
--rw-r--r--   0        0        0    19097 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a68/omicron/dal/influx/flux.py
--rw-r--r--   0        0        0    16805 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a68/omicron/dal/influx/influxclient.py
--rw-r--r--   0        0        0    27708 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a68/omicron/dal/influx/serialize.py
--rw-r--r--   0        0        0       78 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a68/omicron/extensions/__init__.py
--rw-r--r--   0        0        0      656 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a68/omicron/extensions/decimals.py
--rw-r--r--   0        0        0    15929 2023-05-01 02:32:25.512887 zillionare_omicron-2.0.0a68/omicron/extensions/np.py
--rw-r--r--   0        0        0      492 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a68/omicron/models/__init__.py
--rw-r--r--   0        0        0     7867 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a68/omicron/models/board.py
--rw-r--r--   0        0        0    26127 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/models/security.py
--rw-r--r--   0        0        0    53741 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/models/stock.py
--rw-r--r--   0        0        0    41959 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/models/timeframe.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/notify/__init__.py
--rw-r--r--   0        0        0     5472 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/notify/dingtalk.py
--rw-r--r--   0        0        0     6006 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/notify/mail.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/notify/tts.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/plotting/__init__.py
--rw-r--r--   0        0        0    16523 2023-05-08 08:53:56.981283 zillionare_omicron-2.0.0a68/omicron/plotting/candlestick.py
--rw-r--r--   0        0        0     8474 2023-05-08 08:53:20.740774 zillionare_omicron-2.0.0a68/omicron/plotting/metrics.py
--rw-r--r--   0        0        0        0 2023-05-07 01:07:54.376952 zillionare_omicron-2.0.0a68/omicron/strategy/__init__.py
--rw-r--r--   0        0        0     8909 2023-05-08 08:01:12.268255 zillionare_omicron-2.0.0a68/omicron/strategy/base.py
--rw-r--r--   0        0        0     1099 2023-05-07 02:09:33.855184 zillionare_omicron-2.0.0a68/omicron/strategy/sma.py
--rw-r--r--   0        0        0      114 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a68/omicron/talib/__init__.py
--rw-r--r--   0        0        0     9958 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a68/omicron/talib/core.py
--rw-r--r--   0        0        0    23141 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a68/omicron/talib/morph.py
--rwxr-xr-x   0        0        0     3391 2023-05-08 07:56:23.256312 zillionare_omicron-2.0.0a68/pyproject.toml
--rw-r--r--   0        0        0     5556 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a68/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a68/tests/core/__init__.py
--rw-r--r--   0        0        0      297 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a68/tests/core/test_errors.py
--rw-r--r--   0        0        0     3615 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a68/tests/core/test_triggers.py
--rw-r--r--   0        0        0     1024 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/core/test_types.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/dal/__init__.py
--rw-r--r--   0        0        0      622 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/dal/influx/__init__.py
--rw-r--r--   0        0        0     1177 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/dal/influx/test_escape.py
--rw-r--r--   0        0        0     8531 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/dal/influx/test_flux.py
--rw-r--r--   0        0        0    14284 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/dal/influx/test_influxclient.py
--rw-r--r--   0        0        0    15710 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/dal/influx/test_serialize.py
--rw-r--r--   0        0        0     1253 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.15m.csv
--rw-r--r--   0        0        0      118 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.1M.csv
--rw-r--r--   0        0        0      188 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.1d.csv
--rw-r--r--   0        0        0    22206 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.1m.csv
--rw-r--r--   0        0        0      115 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.1w.csv
--rw-r--r--   0        0        0      654 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.30m.csv
--rw-r--r--   0        0        0     3633 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.5m.csv
--rw-r--r--   0        0        0      352 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.60m.csv
--rw-r--r--   0        0        0  1059606 2023-05-07 02:32:26.029160 zillionare_omicron-2.0.0a68/tests/data/000001.XSHG.1m.csv
--rw-r--r--   0        0        0     8089 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a68/tests/data/000002.XSHE.1d.csv
--rw-r--r--   0        0        0    22419 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/000002.XSHE.1m.csv
--rw-r--r--   0        0        0     7166 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/000002.XSHE.1w.csv
--rw-r--r--   0        0        0     8096 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/000002.XSHE.30m.csv
--rw-r--r--   0        0        0     7585 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/000004.XSHE.1d.csv
--rw-r--r--   0        0        0    20344 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/000004.XSHE.1m.csv
--rw-r--r--   0        0        0     6443 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/000004.XSHE.1w.csv
--rw-r--r--   0        0        0     7688 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/000004.XSHE.30m.csv
--rw-r--r--   0        0        0     4206 2023-05-07 02:31:54.553073 zillionare_omicron-2.0.0a68/tests/data/600000.XSHG.1d.csv
--rw-r--r--   0        0        0     1145 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/README.md
--rw-r--r--   0        0        0     2191 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a68/tests/data/bars_1d.pkl
--rw-r--r--   0        0        0   408697 2023-01-24 12:41:24.943079 zillionare_omicron-2.0.0a68/tests/data/bars_1m.pkl
--rw-r--r--   0        0        0      713 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/data/limits.csv
--rw-r--r--   0        0        0   164066 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/data/stock_bars_flux_query.txt
--rw-r--r--   0        0        0     6315 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/data/test.jpg
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/extensions/__init__.py
--rw-r--r--   0        0        0      594 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/extensions/test_decimals.py
--rw-r--r--   0        0        0     9864 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/extensions/test_np.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/models/__init__.py
--rw-r--r--   0        0        0     6802 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/models/test_board.py
--rw-r--r--   0        0        0    11161 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a68/tests/models/test_security.py
--rw-r--r--   0        0        0    68822 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/models/test_stock.py
--rw-r--r--   0        0        0    36351 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/models/test_timeframe.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/notify/__init__.py
--rw-r--r--   0        0        0      823 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/notify/test_dingtalk.py
--rw-r--r--   0        0        0     2686 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/notify/test_mail.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/performance/influx/__init__.py
--rw-r--r--   0        0        0     3317 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/performance/influx/end2end.py
--rw-r--r--   0        0        0     4197 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/performance/influx/serialize.py
--rw-r--r--   0        0        0      294 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/performance/readme.md
--rw-r--r--   0        0        0      406 2023-01-19 03:32:37.466696 zillionare_omicron-2.0.0a68/tests/pyrightconfig.json
--rw-r--r--   0        0        0        0 2023-05-07 02:10:22.915444 zillionare_omicron-2.0.0a68/tests/strategy/__init__.py
--rw-r--r--   0        0        0     1517 2023-05-07 03:14:15.795948 zillionare_omicron-2.0.0a68/tests/strategy/test_strategy.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/talib/__init__.py
--rw-r--r--   0        0        0     2917 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/talib/test_core.py
--rw-r--r--   0        0        0    37991 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a68/tests/talib/test_morph.py
--rw-r--r--   0        0        0     4334 1970-01-01 00:00:00.000000 zillionare_omicron-2.0.0a68/PKG-INFO
+-rw-r--r--   0        0        0      112 2023-01-24 12:41:24.903079 zillionare_omicron-2.0.0a69/AUTHORS.md
+-rw-r--r--   0        0        0     1726 2023-05-09 07:42:36.089641 zillionare_omicron-2.0.0a69/HISTORY.md
+-rw-r--r--   0        0        0     1068 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a69/LICENSE
+-rw-r--r--   0        0        0     1331 2023-05-07 03:30:41.208098 zillionare_omicron-2.0.0a69/README.md
+-rw-r--r--   0        0        0   503846 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/_static/Omicron_Windows10.docx
+-rw-r--r--   0        0        0     5620 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a69/docs/_static/jetbrains-variant-3.svg
+-rw-r--r--   0        0        0       84 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/dal/flux.md
+-rw-r--r--   0        0        0      110 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/dal/influxclient.md
+-rw-r--r--   0        0        0      189 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/dal/serialize.md
+-rw-r--r--   0        0        0     5772 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/metrics.md
+-rw-r--r--   0        0        0      203 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/omicron.md
+-rw-r--r--   0        0        0       73 2023-05-08 07:55:54.700078 zillionare_omicron-2.0.0a69/docs/api/plotting/candlestick.md
+-rw-r--r--   0        0        0       69 2023-05-08 07:55:45.740005 zillionare_omicron-2.0.0a69/docs/api/plotting/metrics.md
+-rw-r--r--   0        0        0       68 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/security.md
+-rw-r--r--   0        0        0       65 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/stock.md
+-rw-r--r--   0        0        0       21 2023-05-07 03:32:19.736871 zillionare_omicron-2.0.0a69/docs/api/strategy.md
+-rw-r--r--   0        0        0       58 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/talib.md
+-rw-r--r--   0        0        0       57 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/timeframe.md
+-rw-r--r--   0        0        0       66 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a69/docs/api/triggers.md
+-rw-r--r--   0        0        0      907 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a69/docs/css/extra.css
+-rw-r--r--   0        0        0     1778 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/developer.md
+-rw-r--r--   0        0        0       43 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a69/docs/history.md
+-rw-r--r--   0        0        0       42 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a69/docs/index.md
+-rw-r--r--   0        0        0     1820 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/installation.md
+-rw-r--r--   0        0        0     9823 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/usage.md
+-rw-r--r--   0        0        0      920 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/omicron/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/omicron/config/__init__.py
+-rw-r--r--   0        0        0    56389 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/config/calendar.json
+-rw-r--r--   0        0        0      441 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/config/defaults.yaml
+-rw-r--r--   0        0        0      378 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/config/dev.yaml
+-rw-r--r--   0        0        0     1334 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/config/schema.py
+-rw-r--r--   0        0        0      816 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a69/omicron/config/sql/v0.6.sql
+-rw-r--r--   0        0        0     2785 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/config/sql/v1.0.sql
+-rw-r--r--   0        0        0       46 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a69/omicron/core/__init__.py
+-rw-r--r--   0        0        0      140 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/core/constants.py
+-rw-r--r--   0        0        0     1095 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/core/errors.py
+-rw-r--r--   0        0        0       46 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/core/events.py
+-rw-r--r--   0        0        0     6517 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/core/triggers.py
+-rw-r--r--   0        0        0       71 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/dal/__init__.py
+-rw-r--r--   0        0        0     3215 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/dal/cache.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/dal/influx/__init__.py
+-rw-r--r--   0        0        0      370 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/dal/influx/errors.py
+-rw-r--r--   0        0        0      996 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/dal/influx/escape.py
+-rw-r--r--   0        0        0    19097 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a69/omicron/dal/influx/flux.py
+-rw-r--r--   0        0        0    16805 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a69/omicron/dal/influx/influxclient.py
+-rw-r--r--   0        0        0    27708 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a69/omicron/dal/influx/serialize.py
+-rw-r--r--   0        0        0       78 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a69/omicron/extensions/__init__.py
+-rw-r--r--   0        0        0      656 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a69/omicron/extensions/decimals.py
+-rw-r--r--   0        0        0    15929 2023-05-01 02:32:25.512887 zillionare_omicron-2.0.0a69/omicron/extensions/np.py
+-rw-r--r--   0        0        0      492 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a69/omicron/models/__init__.py
+-rw-r--r--   0        0        0     7867 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a69/omicron/models/board.py
+-rw-r--r--   0        0        0    26127 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/models/security.py
+-rw-r--r--   0        0        0    53741 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/models/stock.py
+-rw-r--r--   0        0        0    41959 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/models/timeframe.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/notify/__init__.py
+-rw-r--r--   0        0        0     5472 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/notify/dingtalk.py
+-rw-r--r--   0        0        0     6006 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/notify/mail.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/notify/tts.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/plotting/__init__.py
+-rw-r--r--   0        0        0    16523 2023-05-08 08:53:56.981283 zillionare_omicron-2.0.0a69/omicron/plotting/candlestick.py
+-rw-r--r--   0        0        0     8474 2023-05-08 08:53:20.740774 zillionare_omicron-2.0.0a69/omicron/plotting/metrics.py
+-rw-r--r--   0        0        0        0 2023-05-07 01:07:54.376952 zillionare_omicron-2.0.0a69/omicron/strategy/__init__.py
+-rw-r--r--   0        0        0     9053 2023-05-09 07:41:37.353693 zillionare_omicron-2.0.0a69/omicron/strategy/base.py
+-rw-r--r--   0        0        0     1099 2023-05-07 02:09:33.855184 zillionare_omicron-2.0.0a69/omicron/strategy/sma.py
+-rw-r--r--   0        0        0      114 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/talib/__init__.py
+-rw-r--r--   0        0        0     9958 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a69/omicron/talib/core.py
+-rw-r--r--   0        0        0    23141 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a69/omicron/talib/morph.py
+-rwxr-xr-x   0        0        0     3391 2023-05-09 07:42:01.057668 zillionare_omicron-2.0.0a69/pyproject.toml
+-rw-r--r--   0        0        0     5556 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a69/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a69/tests/core/__init__.py
+-rw-r--r--   0        0        0      297 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a69/tests/core/test_errors.py
+-rw-r--r--   0        0        0     3615 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a69/tests/core/test_triggers.py
+-rw-r--r--   0        0        0     1024 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/core/test_types.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/dal/__init__.py
+-rw-r--r--   0        0        0      622 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/dal/influx/__init__.py
+-rw-r--r--   0        0        0     1177 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/dal/influx/test_escape.py
+-rw-r--r--   0        0        0     8531 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/dal/influx/test_flux.py
+-rw-r--r--   0        0        0    14284 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/dal/influx/test_influxclient.py
+-rw-r--r--   0        0        0    15710 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/dal/influx/test_serialize.py
+-rw-r--r--   0        0        0     1253 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.15m.csv
+-rw-r--r--   0        0        0      118 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.1M.csv
+-rw-r--r--   0        0        0      188 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.1d.csv
+-rw-r--r--   0        0        0    22206 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.1m.csv
+-rw-r--r--   0        0        0      115 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.1w.csv
+-rw-r--r--   0        0        0      654 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.30m.csv
+-rw-r--r--   0        0        0     3633 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.5m.csv
+-rw-r--r--   0        0        0      352 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.60m.csv
+-rw-r--r--   0        0        0  1059606 2023-05-07 02:32:26.029160 zillionare_omicron-2.0.0a69/tests/data/000001.XSHG.1m.csv
+-rw-r--r--   0        0        0     8089 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000002.XSHE.1d.csv
+-rw-r--r--   0        0        0    22419 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/000002.XSHE.1m.csv
+-rw-r--r--   0        0        0     7166 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/000002.XSHE.1w.csv
+-rw-r--r--   0        0        0     8096 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/000002.XSHE.30m.csv
+-rw-r--r--   0        0        0     7585 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/000004.XSHE.1d.csv
+-rw-r--r--   0        0        0    20344 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/000004.XSHE.1m.csv
+-rw-r--r--   0        0        0     6443 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/000004.XSHE.1w.csv
+-rw-r--r--   0        0        0     7688 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/000004.XSHE.30m.csv
+-rw-r--r--   0        0        0     4206 2023-05-07 02:31:54.553073 zillionare_omicron-2.0.0a69/tests/data/600000.XSHG.1d.csv
+-rw-r--r--   0        0        0     1145 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/README.md
+-rw-r--r--   0        0        0     2191 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/bars_1d.pkl
+-rw-r--r--   0        0        0   408697 2023-01-24 12:41:24.943079 zillionare_omicron-2.0.0a69/tests/data/bars_1m.pkl
+-rw-r--r--   0        0        0      713 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/data/limits.csv
+-rw-r--r--   0        0        0   164066 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/data/stock_bars_flux_query.txt
+-rw-r--r--   0        0        0     6315 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/data/test.jpg
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/extensions/__init__.py
+-rw-r--r--   0        0        0      594 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/extensions/test_decimals.py
+-rw-r--r--   0        0        0     9864 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/extensions/test_np.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/models/__init__.py
+-rw-r--r--   0        0        0     6802 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/models/test_board.py
+-rw-r--r--   0        0        0    11161 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/models/test_security.py
+-rw-r--r--   0        0        0    68822 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/models/test_stock.py
+-rw-r--r--   0        0        0    36351 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/models/test_timeframe.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/notify/__init__.py
+-rw-r--r--   0        0        0      823 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/notify/test_dingtalk.py
+-rw-r--r--   0        0        0     2686 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/notify/test_mail.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/performance/influx/__init__.py
+-rw-r--r--   0        0        0     3317 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/performance/influx/end2end.py
+-rw-r--r--   0        0        0     4197 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/performance/influx/serialize.py
+-rw-r--r--   0        0        0      294 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/performance/readme.md
+-rw-r--r--   0        0        0      406 2023-01-19 03:32:37.466696 zillionare_omicron-2.0.0a69/tests/pyrightconfig.json
+-rw-r--r--   0        0        0        0 2023-05-07 02:10:22.915444 zillionare_omicron-2.0.0a69/tests/strategy/__init__.py
+-rw-r--r--   0        0        0     1517 2023-05-07 03:14:15.795948 zillionare_omicron-2.0.0a69/tests/strategy/test_strategy.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/talib/__init__.py
+-rw-r--r--   0        0        0     2917 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/talib/test_core.py
+-rw-r--r--   0        0        0    37991 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/talib/test_morph.py
+-rw-r--r--   0        0        0     4334 1970-01-01 00:00:00.000000 zillionare_omicron-2.0.0a69/PKG-INFO
```

### Comparing `zillionare_omicron-2.0.0a68/HISTORY.md` & `zillionare_omicron-2.0.0a69/HISTORY.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # History
 
+## 2.0.0-alpha.69
+* BaseStrategy增加`available_shares`方法
 ## 2.0.0-alpha.68
 * 增加了MetricsGraph
 * 增加Strategy基类
 * Candlestick增加了布林带指标
 ## 2.0.0-alpha.49 (2022-09-16)
 * 修订了安装文档。
 * 移除了windows下对ta-lib的依赖。请参考[安装指南](docs/installation.md)以获取在windows下安装ta-lib的方法。
```

### Comparing `zillionare_omicron-2.0.0a68/LICENSE` & `zillionare_omicron-2.0.0a69/LICENSE`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/README.md` & `zillionare_omicron-2.0.0a69/README.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/docs/_static/Omicron_Windows10.docx` & `zillionare_omicron-2.0.0a69/docs/_static/Omicron_Windows10.docx`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/docs/_static/jetbrains-variant-3.svg` & `zillionare_omicron-2.0.0a69/docs/_static/jetbrains-variant-3.svg`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/docs/api/metrics.md` & `zillionare_omicron-2.0.0a69/docs/api/metrics.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/docs/css/extra.css` & `zillionare_omicron-2.0.0a69/docs/css/extra.css`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/docs/developer.md` & `zillionare_omicron-2.0.0a69/docs/developer.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/docs/installation.md` & `zillionare_omicron-2.0.0a69/docs/installation.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/docs/usage.md` & `zillionare_omicron-2.0.0a69/docs/usage.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/__init__.py` & `zillionare_omicron-2.0.0a69/omicron/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/config/calendar.json` & `zillionare_omicron-2.0.0a69/omicron/config/calendar.json`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/config/schema.py` & `zillionare_omicron-2.0.0a69/omicron/config/schema.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/config/sql/v0.6.sql` & `zillionare_omicron-2.0.0a69/omicron/config/sql/v0.6.sql`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/config/sql/v1.0.sql` & `zillionare_omicron-2.0.0a69/omicron/config/sql/v1.0.sql`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/core/errors.py` & `zillionare_omicron-2.0.0a69/omicron/core/errors.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/core/triggers.py` & `zillionare_omicron-2.0.0a69/omicron/core/triggers.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/dal/cache.py` & `zillionare_omicron-2.0.0a69/omicron/dal/cache.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/dal/influx/escape.py` & `zillionare_omicron-2.0.0a69/omicron/dal/influx/escape.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/dal/influx/flux.py` & `zillionare_omicron-2.0.0a69/omicron/dal/influx/flux.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/dal/influx/influxclient.py` & `zillionare_omicron-2.0.0a69/omicron/dal/influx/influxclient.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/dal/influx/serialize.py` & `zillionare_omicron-2.0.0a69/omicron/dal/influx/serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/extensions/decimals.py` & `zillionare_omicron-2.0.0a69/omicron/extensions/decimals.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/extensions/np.py` & `zillionare_omicron-2.0.0a69/omicron/extensions/np.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/models/board.py` & `zillionare_omicron-2.0.0a69/omicron/models/board.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/models/security.py` & `zillionare_omicron-2.0.0a69/omicron/models/security.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/models/stock.py` & `zillionare_omicron-2.0.0a69/omicron/models/stock.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/models/timeframe.py` & `zillionare_omicron-2.0.0a69/omicron/models/timeframe.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/notify/dingtalk.py` & `zillionare_omicron-2.0.0a69/omicron/notify/dingtalk.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/notify/mail.py` & `zillionare_omicron-2.0.0a69/omicron/notify/mail.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/plotting/candlestick.py` & `zillionare_omicron-2.0.0a69/omicron/plotting/candlestick.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/plotting/metrics.py` & `zillionare_omicron-2.0.0a69/omicron/plotting/metrics.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/strategy/base.py` & `zillionare_omicron-2.0.0a69/omicron/strategy/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 import jqdatasdk as jq
 import numpy as np
 from coretypes import Frame, FrameType
 from traderclient import TraderClient
 
 from omicron import tf
 from omicron.models.security import Security
-from omicron.models.stock import Stock
 from omicron.plotting.metrics import MetricsGraph
 
 logger = logging.getLogger(__name__)
 
 
 class BaseStrategy:
     def __init__(
@@ -101,42 +100,48 @@
             self._baseline = baseline
         else:
             if account is None or token is None:
                 raise ValueError("account and token must be presented.")
 
             self.broker = TraderClient(url, self.account, self.token, is_backtest=False)
 
-    async def backtest(self, stop_on_error: bool = False, *args, **kwargs):
+    async def backtest(self, stop_on_error: bool = False, **kwargs):
         converter = (
             tf.int2date if self._frame_type in tf.day_level_frames else tf.int2time
         )
         for i, frame in enumerate(
             tf.get_frames(self._bt_start, self._bt_end, self._frame_type)  # type: ignore
         ):
             try:
                 await self.predict(
-                    converter(frame), self._frame_type, i, *args, **kwargs  # type: ignore
+                    converter(frame), self._frame_type, i, **kwargs  # type: ignore
                 )
             except Exception as e:
                 logger.exception(e)
                 if stop_on_error:
                     raise e
 
         self.broker.stop_backtest()
         self.bills = self.broker.bills()
         self.metrics = self.broker.metrics(baseline=self._baseline)
 
     @property
     def cash(self):
+        """返回当前可用现金"""
         return self.broker.available_money
 
     @property
     def positions(self):
+        """返回当前持仓"""
         return self.broker.positions
 
+    def available_shares(self, sec: str):
+        """返回给定股票当前可售股数。"""
+        return self.broker.available_shares(sec)
+
     async def buy(
         self,
         sec: str,
         price: Optional[float] = None,
         vol: Optional[int] = None,
         money: Optional[float] = None,
         order_time: Optional[datetime.datetime] = None,
@@ -203,17 +208,15 @@
         secs = await Security.select(dt).eval()
         in_trading = jq.get_price(
             secs, fields=["paused"], start_date=dt, end_date=dt, skip_paused=True
         )["code"].to_numpy()
 
         return np.intersect1d(buylist, in_trading)
 
-    async def predict(
-        self, frame: Frame, frame_type: FrameType, i: int, *args, **kwargs
-    ):
+    async def predict(self, frame: Frame, frame_type: FrameType, i: int, **kwargs):
         """策略评估函数。在此函数中实现交易信号检测和处理。
 
         Args:
             frame: 当前时间帧
             frame_type: 处理的数据主周期
             i: 当前时间离回测起始的单位数
         """
```

### Comparing `zillionare_omicron-2.0.0a68/omicron/strategy/sma.py` & `zillionare_omicron-2.0.0a69/omicron/strategy/sma.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/talib/core.py` & `zillionare_omicron-2.0.0a69/omicron/talib/core.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/omicron/talib/morph.py` & `zillionare_omicron-2.0.0a69/omicron/talib/morph.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/pyproject.toml` & `zillionare_omicron-2.0.0a69/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.poetry.dev-dependencies]
 [tool.poetry]
 name = "zillionare-omicron"
 packages = [
     {include = "omicron"}
 ]
-version = "2.0.0a68"
+version = "2.0.0a69"
 description = "Core Library for Zillionare"
 authors = ["jieyu <code@jieyu.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://zillionare-omicron.readthedocs.io"
 repository = "https://github.com/zillionare/omicron"
 documentation = "https://zillionare-omicron.readthedocs.io"
```

### Comparing `zillionare_omicron-2.0.0a68/tests/__init__.py` & `zillionare_omicron-2.0.0a69/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/core/test_triggers.py` & `zillionare_omicron-2.0.0a69/tests/core/test_triggers.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/core/test_types.py` & `zillionare_omicron-2.0.0a69/tests/core/test_types.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/dal/influx/__init__.py` & `zillionare_omicron-2.0.0a69/tests/dal/influx/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/dal/influx/test_escape.py` & `zillionare_omicron-2.0.0a69/tests/dal/influx/test_escape.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/dal/influx/test_flux.py` & `zillionare_omicron-2.0.0a69/tests/dal/influx/test_flux.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/dal/influx/test_influxclient.py` & `zillionare_omicron-2.0.0a69/tests/dal/influx/test_influxclient.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/dal/influx/test_serialize.py` & `zillionare_omicron-2.0.0a69/tests/dal/influx/test_serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.15m.csv` & `zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.15m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.1m.csv` & `zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.30m.csv` & `zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/000001.XSHE.5m.csv` & `zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.5m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/000001.XSHG.1m.csv` & `zillionare_omicron-2.0.0a69/tests/data/000001.XSHG.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/000002.XSHE.1d.csv` & `zillionare_omicron-2.0.0a69/tests/data/000002.XSHE.1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/000002.XSHE.1m.csv` & `zillionare_omicron-2.0.0a69/tests/data/000002.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/000002.XSHE.1w.csv` & `zillionare_omicron-2.0.0a69/tests/data/000002.XSHE.1w.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/000002.XSHE.30m.csv` & `zillionare_omicron-2.0.0a69/tests/data/000002.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/000004.XSHE.1d.csv` & `zillionare_omicron-2.0.0a69/tests/data/000004.XSHE.1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/000004.XSHE.1m.csv` & `zillionare_omicron-2.0.0a69/tests/data/000004.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/000004.XSHE.1w.csv` & `zillionare_omicron-2.0.0a69/tests/data/000004.XSHE.1w.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/000004.XSHE.30m.csv` & `zillionare_omicron-2.0.0a69/tests/data/000004.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/600000.XSHG.1d.csv` & `zillionare_omicron-2.0.0a69/tests/data/600000.XSHG.1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/README.md` & `zillionare_omicron-2.0.0a69/tests/data/README.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/bars_1d.pkl` & `zillionare_omicron-2.0.0a69/tests/data/bars_1d.pkl`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/bars_1m.pkl` & `zillionare_omicron-2.0.0a69/tests/data/bars_1m.pkl`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/limits.csv` & `zillionare_omicron-2.0.0a69/tests/data/limits.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/stock_bars_flux_query.txt` & `zillionare_omicron-2.0.0a69/tests/data/stock_bars_flux_query.txt`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/data/test.jpg` & `zillionare_omicron-2.0.0a69/tests/data/test.jpg`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/extensions/test_decimals.py` & `zillionare_omicron-2.0.0a69/tests/extensions/test_decimals.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/extensions/test_np.py` & `zillionare_omicron-2.0.0a69/tests/extensions/test_np.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/models/test_board.py` & `zillionare_omicron-2.0.0a69/tests/models/test_board.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/models/test_security.py` & `zillionare_omicron-2.0.0a69/tests/models/test_security.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/models/test_stock.py` & `zillionare_omicron-2.0.0a69/tests/models/test_stock.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/models/test_timeframe.py` & `zillionare_omicron-2.0.0a69/tests/models/test_timeframe.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/notify/test_dingtalk.py` & `zillionare_omicron-2.0.0a69/tests/notify/test_dingtalk.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/notify/test_mail.py` & `zillionare_omicron-2.0.0a69/tests/notify/test_mail.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/performance/influx/end2end.py` & `zillionare_omicron-2.0.0a69/tests/performance/influx/end2end.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/performance/influx/serialize.py` & `zillionare_omicron-2.0.0a69/tests/performance/influx/serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/strategy/test_strategy.py` & `zillionare_omicron-2.0.0a69/tests/strategy/test_strategy.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/talib/test_core.py` & `zillionare_omicron-2.0.0a69/tests/talib/test_core.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/tests/talib/test_morph.py` & `zillionare_omicron-2.0.0a69/tests/talib/test_morph.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a68/PKG-INFO` & `zillionare_omicron-2.0.0a69/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillionare-omicron
-Version: 2.0.0a68
+Version: 2.0.0a69
 Summary: Core Library for Zillionare
 Home-page: https://zillionare-omicron.readthedocs.io
 License: MIT
 Keywords: AI,quant,trade,stock
 Author: jieyu
 Author-email: code@jieyu.ai
 Requires-Python: >=3.8,<3.9
```

