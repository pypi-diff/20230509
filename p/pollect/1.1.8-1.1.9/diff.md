# Comparing `tmp/pollect-1.1.8.tar.gz` & `tmp/pollect-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pollect-1.1.8.tar", last modified: Fri Aug  5 13:02:30 2022, max compression
+gzip compressed data, was "pollect-1.1.9.tar", last modified: Sun Aug 21 10:04:29 2022, max compression
```

## Comparing `pollect-1.1.8.tar` & `pollect-1.1.9.tar`

### file list

```diff
@@ -1,107 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.528955 pollect-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-08-05 13:02:21.000000 pollect-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13606 2022-08-05 13:02:30.524955 pollect-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13080 2022-08-05 13:02:21.000000 pollect-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.520955 pollect-1.1.8/pollect/
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/Pollect.py
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.520955 pollect-1.1.8/pollect/core/
--rw-r--r--   0 runner    (1001) docker     (121)     6185 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/core/Core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/core/ExecutionScheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)     4301 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/core/Factories.py
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/core/Helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/core/Log.py
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/core/OSEnv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/core/ValueCache.py
--rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/core/ValueSet.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.520955 pollect-1.1.8/pollect/core/config/
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/core/config/ConfigContainer.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/core/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.520955 pollect-1.1.8/pollect/core/events/
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/core/events/Event.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/core/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.520955 pollect-1.1.8/pollect/libs/
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/Units.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.520955 pollect-1.1.8/pollect/libs/google/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/google/AppConfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/google/FileProvider.py
--rw-r--r--   0 runner    (1001) docker     (121)     4590 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/google/GcsBackend.py
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/google/Helper.py
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/google/MetricsData.py
--rw-r--r--   0 runner    (1001) docker     (121)     2830 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/google/StatsParser.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.520955 pollect-1.1.8/pollect/libs/google/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/google/metrics/AppVersionMetrics.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/google/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.520955 pollect-1.1.8/pollect/libs/google/parser/
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/google/parser/AppVersionParser.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/google/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.520955 pollect-1.1.8/pollect/libs/modbus/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/modbus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.524955 pollect-1.1.8/pollect/libs/sma/
--rw-r--r--   0 runner    (1001) docker     (121)     8119 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/sma/SmaEnergyMeter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/sma/SmaModbus.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/sma/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.524955 pollect-1.1.8/pollect/libs/viessmann/
--rw-r--r--   0 runner    (1001) docker     (121)    12443 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/viessmann/ViessmannApi.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/libs/viessmann/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.524955 pollect-1.1.8/pollect/sources/
--rw-r--r--   0 runner    (1001) docker     (121)     3703 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/AppStoreConnectSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     3627 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/BindSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/DiskUsageSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/FritzSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/GdcSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1999 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/HomematicIpSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/HttpSource.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/IOSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/InterfaceSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     2407 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/MMISource.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/MemoryUsageSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/OpenhabSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     2955 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/PlexSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/ProcessSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/SensorsSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/SmaEnergyMeterSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1599 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/SmaPvModbusSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/SmartCtlSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     8237 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/SnmpGetSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     3191 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/Source.py
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/TcpTimeSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     4196 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/TpLinkEapSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     7263 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/ViessmannSource.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.524955 pollect-1.1.8/pollect/sources/helper/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/helper/ProbeValue.py
--rw-r--r--   0 runner    (1001) docker     (121)     2997 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/helper/PsutilStats.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/sources/helper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.524955 pollect-1.1.8/pollect/writers/
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/writers/PrometheusSslWriter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/writers/PrometheusWriter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2052 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/writers/Writer.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:21.000000 pollect-1.1.8/pollect/writers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.520955 pollect-1.1.8/pollect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13606 2022-08-05 13:02:30.000000 pollect-1.1.8/pollect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2598 2022-08-05 13:02:30.000000 pollect-1.1.8/pollect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-05 13:02:30.000000 pollect-1.1.8/pollect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-08-05 13:02:30.000000 pollect-1.1.8/pollect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-05 13:02:30.000000 pollect-1.1.8/pollect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-05 13:02:30.000000 pollect-1.1.8/pollect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-05 13:02:30.528955 pollect-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-08-05 13:02:21.000000 pollect-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.524955 pollect-1.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:21.000000 pollect-1.1.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.524955 pollect-1.1.8/tests/libs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:21.000000 pollect-1.1.8/tests/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:30.524955 pollect-1.1.8/tests/libs/sma/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 13:02:21.000000 pollect-1.1.8/tests/libs/sma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-08-05 13:02:21.000000 pollect-1.1.8/tests/libs/sma/test_SmaEnergyMeter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-08-05 13:02:21.000000 pollect-1.1.8/tests/test_ConfigContainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4109 2022-08-05 13:02:21.000000 pollect-1.1.8/tests/test_Core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-08-05 13:02:21.000000 pollect-1.1.8/tests/test_Event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-08-05 13:02:21.000000 pollect-1.1.8/tests/test_Http.py
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-08-05 13:02:21.000000 pollect-1.1.8/tests/test_ProcessSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-08-05 13:02:21.000000 pollect-1.1.8/tests/test_SensorsSource.py
--rw-r--r--   0 runner    (1001) docker     (121)     4869 2022-08-05 13:02:21.000000 pollect-1.1.8/tests/test_SmartCtl.py
--rw-r--r--   0 runner    (1001) docker     (121)     7459 2022-08-05 13:02:21.000000 pollect-1.1.8/tests/test_SnmpGetSource.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.659635 pollect-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-08-21 10:04:22.000000 pollect-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    14505 2022-08-21 10:04:29.659635 pollect-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14025 2022-08-21 10:04:22.000000 pollect-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.651634 pollect-1.1.9/pollect/
+-rw-r--r--   0 runner    (1001) docker     (121)     1998 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/Pollect.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.651634 pollect-1.1.9/pollect/core/
+-rw-r--r--   0 runner    (1001) docker     (121)     6531 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/core/Core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/core/ExecutionScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4301 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/core/Factories.py
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/core/Helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/core/Log.py
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/core/OSEnv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/core/ValueCache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/core/ValueSet.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.651634 pollect-1.1.9/pollect/core/config/
+-rw-r--r--   0 runner    (1001) docker     (121)     2163 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/core/config/ConfigContainer.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/core/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.651634 pollect-1.1.9/pollect/core/events/
+-rw-r--r--   0 runner    (1001) docker     (121)      530 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/core/events/Event.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/core/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.651634 pollect-1.1.9/pollect/libs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/Units.py
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.651634 pollect-1.1.9/pollect/libs/google/
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/google/AppConfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/google/FileProvider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4590 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/google/GcsBackend.py
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/google/Helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/google/MetricsData.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2830 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/google/StatsParser.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.651634 pollect-1.1.9/pollect/libs/google/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/google/metrics/AppVersionMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/google/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.651634 pollect-1.1.9/pollect/libs/google/parser/
+-rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/google/parser/AppVersionParser.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/google/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.651634 pollect-1.1.9/pollect/libs/modbus/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/modbus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.651634 pollect-1.1.9/pollect/libs/sma/
+-rw-r--r--   0 runner    (1001) docker     (121)     8119 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/sma/SmaEnergyMeter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/sma/SmaModbus.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/sma/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.655634 pollect-1.1.9/pollect/libs/viessmann/
+-rw-r--r--   0 runner    (1001) docker     (121)    12443 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/viessmann/ViessmannApi.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/libs/viessmann/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.655634 pollect-1.1.9/pollect/sources/
+-rw-r--r--   0 runner    (1001) docker     (121)     3703 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/AppStoreConnectSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3627 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/BindSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/DiskUsageSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/FritzSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/GdcSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1999 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/HomematicIpSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4313 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/HttpIngressSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/HttpSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/IOSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/InterfaceSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2407 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/MMISource.py
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/MemoryUsageSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/OpenhabSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2955 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/PlexSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/ProcessSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/SensorsSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/SmaEnergyMeterSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1609 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/SmaPvModbusSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/SmartCtlSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8237 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/SnmpGetSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3276 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/Source.py
+-rw-r--r--   0 runner    (1001) docker     (121)      938 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/TcpTimeSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4196 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/TpLinkEapSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7263 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/ViessmannSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.655634 pollect-1.1.9/pollect/sources/helper/
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/helper/ProbeValue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2997 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/helper/PsutilStats.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/sources/helper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.655634 pollect-1.1.9/pollect/writers/
+-rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/writers/PrometheusSslWriter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3640 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/writers/PrometheusWriter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/writers/Writer.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/pollect/writers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.651634 pollect-1.1.9/pollect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    14505 2022-08-21 10:04:29.000000 pollect-1.1.9/pollect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2722 2022-08-21 10:04:29.000000 pollect-1.1.9/pollect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-21 10:04:29.000000 pollect-1.1.9/pollect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-21 10:04:29.000000 pollect-1.1.9/pollect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-21 10:04:29.000000 pollect-1.1.9/pollect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-21 10:04:29.000000 pollect-1.1.9/pollect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-21 10:04:29.659635 pollect-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-08-21 10:04:22.000000 pollect-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.655634 pollect-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.655634 pollect-1.1.9/tests/libs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/tests/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.659635 pollect-1.1.9/tests/libs/sma/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/tests/libs/sma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-08-21 10:04:22.000000 pollect-1.1.9/tests/libs/sma/test_SmaEnergyMeter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-08-21 10:04:22.000000 pollect-1.1.9/tests/test_ConfigContainer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5215 2022-08-21 10:04:22.000000 pollect-1.1.9/tests/test_Core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-08-21 10:04:22.000000 pollect-1.1.9/tests/test_Event.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-08-21 10:04:22.000000 pollect-1.1.9/tests/test_Http.py
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-08-21 10:04:22.000000 pollect-1.1.9/tests/test_ProcessSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-08-21 10:04:22.000000 pollect-1.1.9/tests/test_SensorsSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4869 2022-08-21 10:04:22.000000 pollect-1.1.9/tests/test_SmartCtl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8416 2022-08-21 10:04:22.000000 pollect-1.1.9/tests/test_SnmpGetSource.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:29.659635 pollect-1.1.9/tests/writers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-21 10:04:22.000000 pollect-1.1.9/tests/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1796 2022-08-21 10:04:22.000000 pollect-1.1.9/tests/writers/test_PrometheusWriter.py
```

### Comparing `pollect-1.1.8/LICENSE` & `pollect-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/PKG-INFO` & `pollect-1.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: pollect
-Version: 1.1.8
-Summary: Metrics collection daemon (similar to collectd)
+Version: 1.1.9
+Summary: Metrics collection daemon and exporter
 Home-page: https://github.com/davidgiga1993/pollect
 Author: davidgiga1993
 Author-email: david@dev-core.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pollect - python data collection daemon
 
 pollect is a daemon for collecting system and application metrics in periodical intervals.
-(similar to collectd). It's designed to require very little dependencies to run.
+(similar to collectd). It's designed to require very little dependencies and to be easily customizable.
 
 # Architecture
 
 ```
  ------------                           ----------
  | executor |  -- result of sources --> | writer |
  ------------                           ----------
@@ -75,15 +73,15 @@
     sources:
       - type: LoadAvg
   - collection: slowerMetrics
     tickTime: 120
     sources:
       - type: Http # See Http below for more details
         url: https://google.com
-        labels:
+        labels: # Additional labels/tags for the metrics
           # It is also possible to access env variables anywhere
           # in the config
           system: prod
           home: ${HOME}
 ```
 
 A more advanced configuration sample can be found in the `pollect.[json|yml]` file.
@@ -351,14 +349,48 @@
   "keyFile": "my_api_key.p8",
   "issuerId": "asdasd-123123asd-asd12312-asd",
   "vendorNumber": "882223",
   "dbDir": "db"
 }
 ```
 
+## Http Ingress source `HttpIngress`
+Requires the `gevent` package
+This source starts a simple http webserver and where you can post metrics to.
+It's intended if you want to push metrics to pollect, instead of using the default pull probes.
+
+```yml
+- type: HttpIngress
+  name: Ingress
+  port: 9005 # Listener port
+  metrics: # You can define multiple metrics
+    sample_metric: # Name of the metric
+      type: counter # Optional, gauge by default, counter will cause the value to increment by X every time
+      labels: # Labels for this metric
+        - host
+```
+
+You can update the metrics using a simple http json post:
+```bash
+curl -X POST http://pollect:9005 \
+-H 'Content-Type: application/json' \
+--data-binary @- << EOF
+{
+    "metrics": {
+      "sample_metric": {
+        "value": 124
+        "labels": {
+          "host": "my-hostname"
+        }
+      }
+    }
+}
+EOF
+```
+
 # Writers
 
 A writer represents the destination where the collected data is written to.
 
 ## Dry run `DryRun`
 
 Prints the collected data to the stdout
@@ -433,9 +465,7 @@
 {
 "type": "extensions.MultiRandom"
 }
 ]
 ```
 
 A similar principle is used for the writers. Take a look at the `sources`and `writers` folders for more examples.
-
-
```

### Comparing `pollect-1.1.8/README.md` & `pollect-1.1.9/pollect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,26 @@
+Metadata-Version: 2.1
+Name: pollect
+Version: 1.1.9
+Summary: Metrics collection daemon and exporter
+Home-page: https://github.com/davidgiga1993/pollect
+Author: davidgiga1993
+Author-email: david@dev-core.org
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pollect - python data collection daemon
 
 pollect is a daemon for collecting system and application metrics in periodical intervals.
-(similar to collectd). It's designed to require very little dependencies to run.
+(similar to collectd). It's designed to require very little dependencies and to be easily customizable.
 
 # Architecture
 
 ```
  ------------                           ----------
  | executor |  -- result of sources --> | writer |
  ------------                           ----------
@@ -58,15 +73,15 @@
     sources:
       - type: LoadAvg
   - collection: slowerMetrics
     tickTime: 120
     sources:
       - type: Http # See Http below for more details
         url: https://google.com
-        labels:
+        labels: # Additional labels/tags for the metrics
           # It is also possible to access env variables anywhere
           # in the config
           system: prod
           home: ${HOME}
 ```
 
 A more advanced configuration sample can be found in the `pollect.[json|yml]` file.
@@ -334,14 +349,48 @@
   "keyFile": "my_api_key.p8",
   "issuerId": "asdasd-123123asd-asd12312-asd",
   "vendorNumber": "882223",
   "dbDir": "db"
 }
 ```
 
+## Http Ingress source `HttpIngress`
+Requires the `gevent` package
+This source starts a simple http webserver and where you can post metrics to.
+It's intended if you want to push metrics to pollect, instead of using the default pull probes.
+
+```yml
+- type: HttpIngress
+  name: Ingress
+  port: 9005 # Listener port
+  metrics: # You can define multiple metrics
+    sample_metric: # Name of the metric
+      type: counter # Optional, gauge by default, counter will cause the value to increment by X every time
+      labels: # Labels for this metric
+        - host
+```
+
+You can update the metrics using a simple http json post:
+```bash
+curl -X POST http://pollect:9005 \
+-H 'Content-Type: application/json' \
+--data-binary @- << EOF
+{
+    "metrics": {
+      "sample_metric": {
+        "value": 124
+        "labels": {
+          "host": "my-hostname"
+        }
+      }
+    }
+}
+EOF
+```
+
 # Writers
 
 A writer represents the destination where the collected data is written to.
 
 ## Dry run `DryRun`
 
 Prints the collected data to the stdout
```

### Comparing `pollect-1.1.8/pollect/Pollect.py` & `pollect-1.1.9/pollect/Pollect.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,22 +23,29 @@
         return load_config(config + '.yml')
     except FileNotFoundError:
         return load_config(config + '.json')
 
 
 def main():
     parser = argparse.ArgumentParser()
+    parser.add_argument('--version', dest='version', action='store_true',
+                        help='Prints the current version')
     parser.add_argument('-d', '--debug', dest='debug', action='store_true')
     parser.add_argument('-c', '--config', dest='config', default='config',
                         help='Configuration file which should be read. If no file extension is given '
                              'both (yml and json) will be checked.')
     parser.add_argument('-r', '--dry-run', dest='dry_run', action='store_true',
-                        help='Prints the probed data to the stdout instead of sending it to the writer')
+                        help='Prints the probed data to stdout instead of sending it to the writer')
     args = parser.parse_args()
 
+    if args.version:
+        from pollect import __version__
+        print(f'Pollect {__version__}')
+        return
+
     if args.debug:
         Log.set_debug()
 
     scheduler = None
 
     def signal_handler(signal, frame):
         nonlocal scheduler
```

### Comparing `pollect-1.1.8/pollect/core/Core.py` & `pollect-1.1.9/pollect/core/Core.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             executor.initialize_objects(source_factory)
             executors.append(executor)
         return executors
 
 
 class Executor(Log):
     """
-    Executes probes
+    Executes a collection of probes.
     """
 
     config: Dict[str, any]
     writer: Writer
     tick_time: int = 0
     collection_name: str
     global_config: Configuration
@@ -120,29 +120,39 @@
     def execute(self):
         """
         Probes all data sources and writes the data using the current writer
         """
         partial_write = self.writer.supports_partial_write()
         futures = []
 
-        # Probe the actual data
         for source in self._sources:
             assert isinstance(source, Source)
             future = self.thread_pool.submit(self._probe_and_write if partial_write else self._probe, source)
             futures.append(future)
 
         if partial_write:
+            # Data has already been written to the exporter
             return
 
         # Wait and merge the results
         data = []
         for future in futures:
             # noinspection PyTypeChecker
             self._merge(future.result(), data)
-        self._write(data)
+        self._write(data, self)
+
+    def _probe_and_write(self, source: Source):
+        """
+        Probes a single source and writes the data to the writer
+        :param source: Source
+        """
+        value_sets = self._probe(source)
+        data = []
+        self._merge(value_sets, data)
+        self._write(data, source)
 
     def _probe(self, source: Source) -> Optional[List[ValueSet]]:
         """
         Probes a single source
         :param source: Source
         :return: The probe result data
         """
@@ -156,24 +166,14 @@
             return value_sets
         except Exception as e:
             # Catch all errors that could occur and ignore them
             traceback.print_exc()
             self.log.error(f'Error while probing using source {source}: {e}')
         return None
 
-    def _probe_and_write(self, source: Source):
-        """
-        Probes a single source and writes the data to the writer
-        :param source: Source
-        """
-        value_sets = self._probe(source)
-        data = []
-        self._merge(value_sets, data)
-        self._write(data)
-
     def _merge(self, value_sets: List[ValueSet], results: List[ValueSet]):
         """
         Merges the given value sets
         :param value_sets: Value sets which should be merged
         :param results: Result list
         """
         now = int(time.time())
@@ -181,17 +181,23 @@
             value_set.time = now
             if len(value_set.name) > 0:
                 value_set.name = self.collection_name + '.' + value_set.name
             else:
                 value_set.name = self.collection_name
             results.append(value_set)
 
-    def _write(self, value_sets: List[ValueSet]):
+    def _write(self, value_sets: List[ValueSet], source_ref: object):
+        """
+        Writes the given value sets using the current exporter
+        :param value_sets: Value sets
+        :param source_ref: Reference object which collected the data.
+        This is used to detect if a metric has been removed
+        """
         if len(value_sets) == 0:
             return
 
         # Write the data
         self.log.info('Writing data...')
         try:
-            self.writer.write(value_sets)
+            self.writer.write(value_sets, source_ref)
         except Exception as e:
             self.log.error(f'Could not write data: {e}')
```

### Comparing `pollect-1.1.8/pollect/core/ExecutionScheduler.py` & `pollect-1.1.9/pollect/core/ExecutionScheduler.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/core/Factories.py` & `pollect-1.1.9/pollect/core/Factories.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/core/Helper.py` & `pollect-1.1.9/pollect/core/Helper.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/core/Log.py` & `pollect-1.1.9/pollect/core/Log.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/core/ValueCache.py` & `pollect-1.1.9/pollect/core/ValueCache.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/core/ValueSet.py` & `pollect-1.1.9/pollect/core/ValueSet.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/core/config/ConfigContainer.py` & `pollect-1.1.9/pollect/core/config/ConfigContainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     def keys(self):
         return self._data.keys()
 
     def values(self):
         for value in self._data.values():
             yield self._resolve(value)
 
+    def items(self):
+        return self._data.items()
+
     def get(self, key: str, default: any = None, required: bool = False,
             ignore_missing_env: Optional[str] = None) -> Optional[any]:
         if key not in self._data:
             if required:
                 raise KeyError(f'{key} not found')
             return default
```

### Comparing `pollect-1.1.8/pollect/core/events/Event.py` & `pollect-1.1.9/pollect/core/events/Event.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/libs/Units.py` & `pollect-1.1.9/pollect/libs/Units.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/libs/google/FileProvider.py` & `pollect-1.1.9/pollect/libs/google/FileProvider.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/libs/google/GcsBackend.py` & `pollect-1.1.9/pollect/libs/google/GcsBackend.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/libs/google/Helper.py` & `pollect-1.1.9/pollect/libs/google/Helper.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/libs/google/StatsParser.py` & `pollect-1.1.9/pollect/libs/google/StatsParser.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/libs/google/parser/AppVersionParser.py` & `pollect-1.1.9/pollect/libs/google/parser/AppVersionParser.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/libs/sma/SmaEnergyMeter.py` & `pollect-1.1.9/pollect/libs/sma/SmaEnergyMeter.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/libs/sma/SmaModbus.py` & `pollect-1.1.9/pollect/libs/sma/SmaModbus.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,27 +59,33 @@
 
 
 class SmaModbus(Log):
     """
     Communicates via modbus to SMA PV invertes
     """
     _unit_id: int = -1
+    _is_connected: bool = False
 
     def __init__(self, host: str, port: int = 502):
         super().__init__()
         self._client = ModbusTcpClient(host, port)
 
+    def is_connected(self) -> bool:
+        return self._is_connected
+
     def connect(self):
         self._client.connect()
         # Ask for unit ID
         reply = self._client.read_holding_registers(42109, 4, unit=1)
         self._unit_id = reply.registers[3]
+        self._is_connected = True
 
     def close(self):
         self._client.close()
+        self._is_connected = False
 
     def read(self, reg: Register) -> ValueWithUnit:
         value = u32(self._client.read_holding_registers(reg.id, 2, unit=self._unit_id))
         if value == 0xffffffff or value == 0x80000000:
             # Use 0 as a more sane "not available" value
             value = 0
         return ValueWithUnit(value, reg.unit)
```

### Comparing `pollect-1.1.8/pollect/libs/viessmann/ViessmannApi.py` & `pollect-1.1.9/pollect/libs/viessmann/ViessmannApi.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/AppStoreConnectSource.py` & `pollect-1.1.9/pollect/sources/AppStoreConnectSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/BindSource.py` & `pollect-1.1.9/pollect/sources/BindSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/DiskUsageSource.py` & `pollect-1.1.9/pollect/sources/DiskUsageSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/FritzSource.py` & `pollect-1.1.9/pollect/sources/FritzSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/GdcSource.py` & `pollect-1.1.9/pollect/sources/GdcSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/HomematicIpSource.py` & `pollect-1.1.9/pollect/sources/HomematicIpSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/HttpSource.py` & `pollect-1.1.9/pollect/sources/HttpSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/IOSource.py` & `pollect-1.1.9/pollect/sources/IOSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/InterfaceSource.py` & `pollect-1.1.9/pollect/sources/InterfaceSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/MMISource.py` & `pollect-1.1.9/pollect/sources/MMISource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/MemoryUsageSource.py` & `pollect-1.1.9/pollect/sources/MemoryUsageSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/OpenhabSource.py` & `pollect-1.1.9/pollect/sources/OpenhabSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/PlexSource.py` & `pollect-1.1.9/pollect/sources/PlexSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/ProcessSource.py` & `pollect-1.1.9/pollect/sources/ProcessSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/SensorsSource.py` & `pollect-1.1.9/pollect/sources/SensorsSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/SmaEnergyMeterSource.py` & `pollect-1.1.9/pollect/sources/SmaEnergyMeterSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/SmaPvModbusSource.py` & `pollect-1.1.9/pollect/sources/SmaPvModbusSource.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,21 +10,20 @@
     Source for SMA PV inverters (via modbus TCP)
     """
 
     def __init__(self, config):
         super().__init__(config)
         self._sma = SmaModbus(config['host'], config.get('port', 502))
 
-    def setup(self, global_conf):
-        self._sma.connect()
-
     def shutdown(self):
         self._sma.close()
 
     def _probe(self) -> Optional[ValueSet] or List[ValueSet]:
+        if not self._sma.is_connected():
+            self._sma.connect()
         base_set = ValueSet()
         base_set.add(Value(self._sma.read(SmaRegisters.REG_TEMP).get_as_base_unit(), name='temp'))
         base_set.add(Value(self._sma.read(SmaRegisters.REG_FREQUENCY).get_as_base_unit(), name='frequency'))
         base_set.add(Value(self._sma.read(SmaRegisters.REG_POWER_EFFECTIVE_SUM).get_as_base_unit(), name='power'))
         base_set.add(Value(self._sma.read(SmaRegisters.REG_DC_INPUT_VOLTAGE).get_as_base_unit(), name='dc_voltage'))
         base_set.add(Value(self._sma.read(SmaRegisters.REG_DC_INPUT_CURRENT).get_as_base_unit(), name='dc_current'))
```

### Comparing `pollect-1.1.8/pollect/sources/SmartCtlSource.py` & `pollect-1.1.9/pollect/sources/SmartCtlSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/SnmpGetSource.py` & `pollect-1.1.9/pollect/sources/SnmpGetSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/Source.py` & `pollect-1.1.9/pollect/sources/Source.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 from pollect.core.ValueSet import ValueSet, Value
 
 if typing.TYPE_CHECKING:
     from pollect.core.Core import Configuration
 
 
 class Source(Log):
+    """
+    A single metrics source. May return multiple metrics and labels
+    """
+
     type: str = None
     """
     Type string of this source
     """
 
     name: Optional[str] = None
     """
```

### Comparing `pollect-1.1.8/pollect/sources/TcpTimeSource.py` & `pollect-1.1.9/pollect/sources/TcpTimeSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/TpLinkEapSource.py` & `pollect-1.1.9/pollect/sources/TpLinkEapSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/ViessmannSource.py` & `pollect-1.1.9/pollect/sources/ViessmannSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/sources/helper/PsutilStats.py` & `pollect-1.1.9/pollect/sources/helper/PsutilStats.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/pollect/writers/PrometheusSslWriter.py` & `pollect-1.1.9/pollect/writers/PrometheusSslWriter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import threading
 from urllib.parse import parse_qs
 
 from gevent import pywsgi
 from prometheus_client import exposition
 from prometheus_client import registry
 
 from pollect.writers.PrometheusWriter import PrometheusWriter
@@ -34,14 +35,19 @@
             headers = [('Content-Type', content_type)]
 
             start_response('200 OK', headers)
             return [output]
 
         logger = logging.getLogger('prom')
         logger.setLevel(logging.ERROR)
-        self._server = pywsgi.WSGIServer(('0.0.0.0', self._port), serve, keyfile=self._key, certfile=self._cert,
-                                         log=logger)
-        self._server.start()
+
+        def start():
+            self._server = pywsgi.WSGIServer(('127.0.0.1', self._port), serve,
+                                             keyfile=self._key, certfile=self._cert,
+                                             log=logger)
+            self._server.start()
+
+        launcher = threading.Thread(target=start)
+        launcher.start()
 
     def stop(self):
         self._server.stop()
-
```

### Comparing `pollect-1.1.8/pollect.egg-info/PKG-INFO` & `pollect-1.1.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,11 @@
-Metadata-Version: 2.1
-Name: pollect
-Version: 1.1.8
-Summary: Metrics collection daemon (similar to collectd)
-Home-page: https://github.com/davidgiga1993/pollect
-Author: davidgiga1993
-Author-email: david@dev-core.org
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pollect - python data collection daemon
 
 pollect is a daemon for collecting system and application metrics in periodical intervals.
-(similar to collectd). It's designed to require very little dependencies to run.
+(similar to collectd). It's designed to require very little dependencies and to be easily customizable.
 
 # Architecture
 
 ```
  ------------                           ----------
  | executor |  -- result of sources --> | writer |
  ------------                           ----------
@@ -75,15 +58,15 @@
     sources:
       - type: LoadAvg
   - collection: slowerMetrics
     tickTime: 120
     sources:
       - type: Http # See Http below for more details
         url: https://google.com
-        labels:
+        labels: # Additional labels/tags for the metrics
           # It is also possible to access env variables anywhere
           # in the config
           system: prod
           home: ${HOME}
 ```
 
 A more advanced configuration sample can be found in the `pollect.[json|yml]` file.
@@ -351,14 +334,48 @@
   "keyFile": "my_api_key.p8",
   "issuerId": "asdasd-123123asd-asd12312-asd",
   "vendorNumber": "882223",
   "dbDir": "db"
 }
 ```
 
+## Http Ingress source `HttpIngress`
+Requires the `gevent` package
+This source starts a simple http webserver and where you can post metrics to.
+It's intended if you want to push metrics to pollect, instead of using the default pull probes.
+
+```yml
+- type: HttpIngress
+  name: Ingress
+  port: 9005 # Listener port
+  metrics: # You can define multiple metrics
+    sample_metric: # Name of the metric
+      type: counter # Optional, gauge by default, counter will cause the value to increment by X every time
+      labels: # Labels for this metric
+        - host
+```
+
+You can update the metrics using a simple http json post:
+```bash
+curl -X POST http://pollect:9005 \
+-H 'Content-Type: application/json' \
+--data-binary @- << EOF
+{
+    "metrics": {
+      "sample_metric": {
+        "value": 124
+        "labels": {
+          "host": "my-hostname"
+        }
+      }
+    }
+}
+EOF
+```
+
 # Writers
 
 A writer represents the destination where the collected data is written to.
 
 ## Dry run `DryRun`
 
 Prints the collected data to the stdout
@@ -433,9 +450,7 @@
 {
 "type": "extensions.MultiRandom"
 }
 ]
 ```
 
 A similar principle is used for the writers. Take a look at the `sources`and `writers` folders for more examples.
-
-
```

### Comparing `pollect-1.1.8/pollect.egg-info/SOURCES.txt` & `pollect-1.1.9/pollect.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 pollect/core/ValueSet.py
 pollect/core/__init__.py
 pollect/core/config/ConfigContainer.py
 pollect/core/config/__init__.py
 pollect/core/events/Event.py
 pollect/core/events/__init__.py
 pollect/libs/Units.py
+pollect/libs/Utils.py
 pollect/libs/__init__.py
 pollect/libs/google/AppConfig.py
 pollect/libs/google/FileProvider.py
 pollect/libs/google/GcsBackend.py
 pollect/libs/google/Helper.py
 pollect/libs/google/MetricsData.py
 pollect/libs/google/StatsParser.py
@@ -43,14 +44,15 @@
 pollect/libs/viessmann/__init__.py
 pollect/sources/AppStoreConnectSource.py
 pollect/sources/BindSource.py
 pollect/sources/DiskUsageSource.py
 pollect/sources/FritzSource.py
 pollect/sources/GdcSource.py
 pollect/sources/HomematicIpSource.py
+pollect/sources/HttpIngressSource.py
 pollect/sources/HttpSource.py
 pollect/sources/IOSource.py
 pollect/sources/InterfaceSource.py
 pollect/sources/MMISource.py
 pollect/sources/MemoryUsageSource.py
 pollect/sources/OpenhabSource.py
 pollect/sources/PlexSource.py
@@ -79,8 +81,10 @@
 tests/test_Http.py
 tests/test_ProcessSource.py
 tests/test_SensorsSource.py
 tests/test_SmartCtl.py
 tests/test_SnmpGetSource.py
 tests/libs/__init__.py
 tests/libs/sma/__init__.py
-tests/libs/sma/test_SmaEnergyMeter.py
+tests/libs/sma/test_SmaEnergyMeter.py
+tests/writers/__init__.py
+tests/writers/test_PrometheusWriter.py
```

### Comparing `pollect-1.1.8/tests/libs/sma/test_SmaEnergyMeter.py` & `pollect-1.1.9/tests/libs/sma/test_SmaEnergyMeter.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/tests/test_ConfigContainer.py` & `pollect-1.1.9/tests/test_ConfigContainer.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/tests/test_Core.py` & `pollect-1.1.9/tests/test_Core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from time import sleep
 from unittest import TestCase
 
+import requests
 import schedule
 
 from pollect.core.Core import Configuration
 from pollect.core.ExecutionScheduler import ExecutionScheduler
 from pollect.core.Factories import SourceFactory, WriterFactory
 from pollect.writers.Writer import InMemoryWriter, ParallelInMemoryWriter
 
@@ -70,15 +71,15 @@
             "executors": [
                 {
                     "collection": "pollect",
                     "sources": [
                         {
                             "type": "Http",
                             "name": "dev_core",
-                            "url": "https://google.com",
+                            "url": ["https://google.com"],
                             "timeout": 1
                         },
                     ]
                 }
             ]
         }
         config = Configuration(raw_config)
@@ -88,14 +89,48 @@
         sleep(1)
         schedule.run_pending()
 
         self.assertIsInstance(config.writer, InMemoryWriter)
         data = config.writer.data
         self.assertGreater(len(data), 0)
 
+    def test_exec_partial_prometheus(self):
+        raw_config = {
+            "tickTime": 1,
+            "threads": 2,
+            "writer": {
+                "type": "Prometheus",
+                "port": 9123,
+            },
+            "executors": [
+                {
+                    "collection": "pollect",
+                    "sources": [
+                        {
+                            "type": "Http",
+                            "name": "dev_core",
+                            "url": ["https://google.com", "https://github.com"],
+                            "timeout": 1
+                        },
+                    ]
+                }
+            ]
+        }
+        config = Configuration(raw_config)
+        executors = config.create_executors()
+        scheduler = ExecutionScheduler(config, executors)
+        scheduler.create()
+        sleep(1)
+        schedule.run_pending()
+        sleep(4)
+        reply = requests.get('http://localhost:9123')
+        scheduler.stop()
+        self.assertIn('github', reply.text)
+        self.assertIn('google', reply.text)
+
     def test_exec_parallel(self):
         raw_config = {
             "tickTime": 30,
             "threads": 2,
             "writer": {
                 "type": "ParallelInMemory"
             },
```

### Comparing `pollect-1.1.8/tests/test_Event.py` & `pollect-1.1.9/tests/test_Event.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/tests/test_Http.py` & `pollect-1.1.9/tests/test_Http.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/tests/test_SensorsSource.py` & `pollect-1.1.9/tests/test_SensorsSource.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/tests/test_SmartCtl.py` & `pollect-1.1.9/tests/test_SmartCtl.py`

 * *Files identical despite different names*

### Comparing `pollect-1.1.8/tests/test_SnmpGetSource.py` & `pollect-1.1.9/tests/test_SnmpGetSource.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,15 @@
         self.assertEqual(11, data.values[2].value)
 
     @patch('pollect.sources.SnmpGetSource.subprocess.check_output')
     def test_range_with_labels(self, mock_check_output):
         std_out = '''iso.3.6.1.2.1.16.1.1.1.3.1 = Counter32: 123
 iso.3.6.1.2.1.16.1.1.1.3.2 = Counter32: 10
 iso.3.6.1.2.1.16.1.1.1.3.3 = Counter32: 11
+iso.3.6.1.2.1.50.1.1.1.3.1 = Counter32: 11
 
 iso.3.6.1.2.1.31.1.1.1.18.1 = STRING: "test name1"
 iso.3.6.1.2.1.31.1.1.1.18.2 = STRING: "test name2"
 iso.3.6.1.2.1.31.1.1.1.18.3 = STRING: "test name3"
 '''
         mock_check_output.return_value = std_out.encode('utf-8')
 
@@ -118,19 +119,33 @@
                 },
                 'range': {
                     'from': 1,
                     'to': 3,
                     'label': 'randomParam',
                 },
                 'name': 'Test'
+            },
+                {
+                'oid': 'iso.3.6.1.2.1.50.1.1.1.3.${randomParam}',
+                'oidLabels': {
+                    # Use the same labels as for the metric above
+                    'portName': 'iso.3.6.1.2.1.31.1.1.1.18.${randomParam}'
+                },
+                'range': {
+                    'from': 1,
+                    'to': 3,
+                    'label': 'randomParam',
+                },
+                'name': 'Test'
             }],
             'type': '-'
         })
         source = SnmpGetSource(config)
-        data = source.probe()[0]
+        result = source.probe()
+        data = result[0]
         self.assertEqual(3, len(data.values))
         self.assertEqual('Test', data.values[0].name)
         self.assertEqual('Test', data.values[1].name)
         self.assertEqual('Test', data.values[2].name)
         self.assertEqual('randomParam', data.labels[0])
         self.assertEqual('portName', data.labels[1])
         self.assertEqual('1', data.values[0].label_values[0])
@@ -139,14 +154,23 @@
         self.assertEqual('test name1', data.values[0].label_values[1])
         self.assertEqual('test name2', data.values[1].label_values[1])
         self.assertEqual('test name3', data.values[2].label_values[1])
         self.assertEqual(123, data.values[0].value)
         self.assertEqual(10, data.values[1].value)
         self.assertEqual(11, data.values[2].value)
 
+        data = result[1]
+        self.assertEqual(1, len(data.values))
+        self.assertEqual('Test', data.values[0].name)
+        self.assertEqual('randomParam', data.labels[0])
+        self.assertEqual('portName', data.labels[1])
+        self.assertEqual('1', data.values[0].label_values[0])
+        self.assertEqual('test name1', data.values[0].label_values[1])
+        self.assertEqual(11, data.values[0].value)
+
     @patch('pollect.sources.SnmpGetSource.subprocess.check_output')
     def test_rate(self, mock_check_output):
         std_out = 'iso.3.6.1.2.1.16.1.1.1.3.48 = Counter32: 0'
         mock_check_output.return_value = std_out.encode('utf-8')
 
         source = SnmpGetSource({
             'host': '10.1.1.1',
```

