# Comparing `tmp/minium-1.4.0.tar.gz` & `tmp/minium-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/minium-1.4.0.tar", last modified: Thu Apr 27 03:03:31 2023, max compression
+gzip compressed data, was "dist/minium-1.4.1.tar", last modified: Tue May  9 06:44:43 2023, max compression
```

## Comparing `minium-1.4.0.tar` & `minium-1.4.1.tar`

### file list

```diff
@@ -1,277 +1,279 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.364473 minium-1.4.0/
--rw-r--r--   0 root         (0) root         (0)      697 2023-04-27 03:03:31.364473 minium-1.4.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.320474 minium-1.4.0/minium/
--rw-r--r--   0 root         (0) root         (0)      948 2023-04-27 02:49:43.000000 minium-1.4.0/minium/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.328473 minium-1.4.0/minium/framework/
--rw-r--r--   0 root         (0) root         (0)       58 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18583 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/assertbase.py
--rw-r--r--   0 root         (0) root         (0)     1587 2022-11-07 03:36:55.000000 minium-1.4.0/minium/framework/casedump.py
--rw-r--r--   0 root         (0) root         (0)     7702 2022-11-07 03:36:55.000000 minium-1.4.0/minium/framework/caseinspect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.328473 minium-1.4.0/minium/framework/dist/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.328473 minium-1.4.0/minium/framework/dist/css/
--rw-r--r--   0 root         (0) root         (0)      437 2022-09-14 13:08:12.000000 minium-1.4.0/minium/framework/dist/css/app.87891bf0.css
--rw-r--r--   0 root         (0) root         (0)   240799 2022-09-14 13:08:12.000000 minium-1.4.0/minium/framework/dist/css/chunk-vendors.52eeca6f.css
--rw-r--r--   0 root         (0) root         (0)     2108 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/dist/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.328473 minium-1.4.0/minium/framework/dist/fonts/
--rw-r--r--   0 root         (0) root         (0)    28200 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/dist/fonts/element-icons.535877f5.woff
--rw-r--r--   0 root         (0) root         (0)    55956 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/dist/fonts/element-icons.732389de.ttf
--rw-r--r--   0 root         (0) root         (0)      847 2022-09-14 13:08:12.000000 minium-1.4.0/minium/framework/dist/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.328473 minium-1.4.0/minium/framework/dist/js/
--rw-r--r--   0 root         (0) root         (0)    17537 2022-09-14 13:08:12.000000 minium-1.4.0/minium/framework/dist/js/app.544bedf4.js
--rw-r--r--   0 root         (0) root         (0)  1346000 2022-09-14 13:08:12.000000 minium-1.4.0/minium/framework/dist/js/chunk-vendors.22ed339a.js
--rw-r--r--   0 root         (0) root         (0)     3463 2023-01-16 03:26:29.000000 minium-1.4.0/minium/framework/errorReport.py
--rw-r--r--   0 root         (0) root         (0)     2402 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.332473 minium-1.4.0/minium/framework/libs/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.332473 minium-1.4.0/minium/framework/libs/tgit/
--rw-r--r--   0 root         (0) root         (0)      152 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/libs/tgit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1007 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/libs/tgit/auth.py
--rw-r--r--   0 root         (0) root         (0)    97301 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/libs/tgit/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.332473 minium-1.4.0/minium/framework/libs/unittest/
--rw-r--r--   0 root         (0) root         (0)      243 2022-12-28 03:15:03.000000 minium-1.4.0/minium/framework/libs/unittest/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11757 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/libs/unittest/case.py
--rw-r--r--   0 root         (0) root         (0)     5656 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/libs/unittest/suite.py
--rw-r--r--   0 root         (0) root         (0)    19830 2022-12-19 02:27:07.000000 minium-1.4.0/minium/framework/loader.py
--rw-r--r--   0 root         (0) root         (0)    10166 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/logcolor.py
--rw-r--r--   0 root         (0) root         (0)     7244 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/miniconfig.py
--rw-r--r--   0 root         (0) root         (0)     3427 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/miniddt.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-02-07 07:19:07.000000 minium-1.4.0/minium/framework/minidoctor.py
--rw-r--r--   0 root         (0) root         (0)     1207 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/minilimit.py
--rw-r--r--   0 root         (0) root         (0)      832 2022-09-14 13:08:12.000000 minium-1.4.0/minium/framework/miniprogram.py
--rw-r--r--   0 root         (0) root         (0)     6669 2022-09-14 13:08:12.000000 minium-1.4.0/minium/framework/miniresult.py
--rw-r--r--   0 root         (0) root         (0)     3216 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/minisuite.py
--rw-r--r--   0 root         (0) root         (0)    29430 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/minitest.py
--rw-r--r--   0 root         (0) root         (0)    17061 2023-04-27 02:49:43.000000 minium-1.4.0/minium/framework/report.py
--rw-r--r--   0 root         (0) root         (0)     3318 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.332473 minium-1.4.0/minium/framework/tools/
--rw-r--r--   0 root         (0) root         (0)       54 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2716 2022-06-30 06:29:28.000000 minium-1.4.0/minium/framework/tools/report_issue.py
--rw-r--r--   0 root         (0) root         (0)     3974 2022-12-19 02:27:07.000000 minium-1.4.0/minium/framework/wording.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.332473 minium-1.4.0/minium/miniprogram/
--rw-r--r--   0 root         (0) root         (0)      688 2023-04-27 02:49:43.000000 minium-1.4.0/minium/miniprogram/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.336473 minium-1.4.0/minium/miniprogram/base_driver/
--rw-r--r--   0 root         (0) root         (0)      191 2022-06-30 06:29:28.000000 minium-1.4.0/minium/miniprogram/base_driver/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47762 2023-04-27 02:49:43.000000 minium-1.4.0/minium/miniprogram/base_driver/app.py
--rw-r--r--   0 root         (0) root         (0)     3909 2023-04-27 02:49:43.000000 minium-1.4.0/minium/miniprogram/base_driver/callback.py
--rw-r--r--   0 root         (0) root         (0)    28828 2023-04-27 02:49:43.000000 minium-1.4.0/minium/miniprogram/base_driver/connection.py
--rw-r--r--   0 root         (0) root         (0)    46414 2023-04-27 02:49:43.000000 minium-1.4.0/minium/miniprogram/base_driver/element.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-04-27 02:49:43.000000 minium-1.4.0/minium/miniprogram/base_driver/minium.py
--rw-r--r--   0 root         (0) root         (0)     4865 2023-04-27 02:49:44.000000 minium-1.4.0/minium/miniprogram/base_driver/minium_log.py
--rw-r--r--   0 root         (0) root         (0)     8485 2023-04-27 02:49:44.000000 minium-1.4.0/minium/miniprogram/base_driver/minium_object.py
--rw-r--r--   0 root         (0) root         (0)    23560 2023-04-27 02:49:44.000000 minium-1.4.0/minium/miniprogram/base_driver/page.py
--rw-r--r--   0 root         (0) root         (0)      771 2022-06-30 06:29:28.000000 minium-1.4.0/minium/miniprogram/base_driver/prefixer.py
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-27 03:03:26.000000 minium-1.4.0/minium/miniprogram/base_driver/version.json
--rw-r--r--   0 root         (0) root         (0)      552 2023-04-27 02:49:44.000000 minium-1.4.0/minium/miniprogram/base_driver/version.py
--rw-r--r--   0 root         (0) root         (0)      263 2022-06-30 06:29:28.000000 minium-1.4.0/minium/miniprogram/base_driver/waiter.py
--rw-r--r--   0 root         (0) root         (0)     6692 2022-06-30 06:29:28.000000 minium-1.4.0/minium/miniprogram/qq_minium.py
--rw-r--r--   0 root         (0) root         (0)    38928 2023-04-27 02:49:44.000000 minium-1.4.0/minium/miniprogram/wx_minium.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.336473 minium-1.4.0/minium/native/
--rw-r--r--   0 root         (0) root         (0)     3218 2022-12-19 02:27:07.000000 minium-1.4.0/minium/native/__init__.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.336473 minium-1.4.0/minium/native/lib/
--rw-r--r--   0 root         (0) root         (0)       58 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.340473 minium-1.4.0/minium/native/lib/android_base/
--rw-r--r--   0 root         (0) root         (0)     1012 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/android_base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.340473 minium-1.4.0/minium/native/lib/at/
--rw-r--r--   0 root         (0) root         (0)     4087 2022-09-14 13:08:12.000000 minium-1.4.0/minium/native/lib/at/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1755 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/apkapi.py
--rw-r--r--   0 root         (0) root         (0)     5609 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/atproxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.344473 minium-1.4.0/minium/native/lib/at/bin/
--rw-r--r--   0 root         (0) root         (0)  3566862 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/bin/AtServer.apk
--rw-r--r--   0 root         (0) root         (0)    95449 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/bin/AtStub.jar
--rw-r--r--   0 root         (0) root         (0)     3222 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/command_line.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.348473 minium-1.4.0/minium/native/lib/at/core/
--rw-r--r--   0 root         (0) root         (0)       37 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      951 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/accesshelper.py
--rw-r--r--   0 root         (0) root         (0)    46986 2022-09-14 13:08:12.000000 minium-1.4.0/minium/native/lib/at/core/adbwrap.py
--rw-r--r--   0 root         (0) root         (0)    10763 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/basedriver.py
--rw-r--r--   0 root         (0) root         (0)    15919 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/case_repair_adapter.py
--rw-r--r--   0 root         (0) root         (0)      624 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/config.py
--rw-r--r--   0 root         (0) root         (0)    31731 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/element.py
--rw-r--r--   0 root         (0) root         (0)      669 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    18740 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/javadriver.py
--rw-r--r--   0 root         (0) root         (0)     3620 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/resguard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.348473 minium-1.4.0/minium/native/lib/at/core/stf/
--rw-r--r--   0 root         (0) root         (0)       56 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/stf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1662 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/stf/mincap.py
--rw-r--r--   0 root         (0) root         (0)     5507 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/stf/minitouch.py
--rw-r--r--   0 root         (0) root         (0)    11600 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/uidevice.py
--rw-r--r--   0 root         (0) root         (0)    17965 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/uixml.py
--rw-r--r--   0 root         (0) root         (0)     2711 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/core/websocketcli.py
--rw-r--r--   0 root         (0) root         (0)     2186 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/eventmonitor.py
--rw-r--r--   0 root         (0) root         (0)     1087 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/hook.py
--rw-r--r--   0 root         (0) root         (0)     8495 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/jlogcat.py
--rw-r--r--   0 root         (0) root         (0)    36015 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/keycode.py
--rw-r--r--   0 root         (0) root         (0)     9492 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/perfcollector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.352473 minium-1.4.0/minium/native/lib/at/tests/
--rw-r--r--   0 root         (0) root         (0)      690 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/AtEvent.py
--rw-r--r--   0 root         (0) root         (0)      326 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/AtSocket.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      480 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/adbtest.py
--rw-r--r--   0 root         (0) root         (0)      490 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/airtesttest.py
--rw-r--r--   0 root         (0) root         (0)    10434 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/atdevicetest.py
--rw-r--r--   0 root         (0) root         (0)      474 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/attestbase.py
--rw-r--r--   0 root         (0) root         (0)     1022 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/drivertest.py
--rw-r--r--   0 root         (0) root         (0)     1768 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/elementtest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.352473 minium-1.4.0/minium/native/lib/at/tests/images/
--rw-r--r--   0 root         (0) root         (0)     7525 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/images/1.jpg
--rw-r--r--   0 root         (0) root         (0)     4388 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/images/2.jpg
--rw-r--r--   0 root         (0) root         (0)    80712 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/images/image.jpg
--rw-r--r--   0 root         (0) root         (0)      493 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/javadrivertest.py
--rw-r--r--   0 root         (0) root         (0)      480 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/minicap_test.py
--rw-r--r--   0 root         (0) root         (0)      375 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/minitest.py
--rw-r--r--   0 root         (0) root         (0)      843 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/minitouch_test.py
--rw-r--r--   0 root         (0) root         (0)      792 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/u2test.py
--rw-r--r--   0 root         (0) root         (0)     1797 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/uixmltest.py
--rw-r--r--   0 root         (0) root         (0)      493 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/vs_test.py
--rw-r--r--   0 root         (0) root         (0)      989 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/tests/webdrivertest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.352473 minium-1.4.0/minium/native/lib/at/utils/
--rw-r--r--   0 root         (0) root         (0)       37 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4896 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/apkinfo.py
--rw-r--r--   0 root         (0) root         (0)   105609 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/axmlparser.py
--rw-r--r--   0 root         (0) root         (0)    27360 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/axmlparser3.py
--rw-r--r--   0 root         (0) root         (0)      526 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/commonhelper.py
--rw-r--r--   0 root         (0) root         (0)     8332 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/decorator.py
--rw-r--r--   0 root         (0) root         (0)      257 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/magic.py
--rw-r--r--   0 root         (0) root         (0)     2457 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/nbsp.py
--rw-r--r--   0 root         (0) root         (0)     1435 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/utils/threadhelper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.352473 minium-1.4.0/minium/native/lib/at/vision/
--rw-r--r--   0 root         (0) root         (0)       56 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/vision/__init__.py
--rw-r--r--   0 root         (0) root         (0)      394 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/vision/template_match.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.356473 minium-1.4.0/minium/native/lib/at/webdriver/
--rw-r--r--   0 root         (0) root         (0)       72 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15310 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/driver.py
--rw-r--r--   0 root         (0) root         (0)      425 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/error.py
--rw-r--r--   0 root         (0) root         (0)     1376 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/jsapi.py
--rw-r--r--   0 root         (0) root         (0)     1519 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/miniapp.py
--rw-r--r--   0 root         (0) root         (0)    18973 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/stub.js
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/tabdescription.py
--rw-r--r--   0 root         (0) root         (0)    13005 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/tabwebsocket.py
--rw-r--r--   0 root         (0) root         (0)     8904 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/webelement.py
--rw-r--r--   0 root         (0) root         (0)     1638 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/webhelper.py
--rw-r--r--   0 root         (0) root         (0)     1399 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/webdriver/wspools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.356473 minium-1.4.0/minium/native/lib/at/wechat/
--rw-r--r--   0 root         (0) root         (0)       79 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/wechat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1421 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/wechat/activtiy.py
--rw-r--r--   0 root         (0) root         (0)      144 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/wechat/appvars.py
--rw-r--r--   0 root         (0) root         (0)       80 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/at/wsimp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.356473 minium-1.4.0/minium/native/lib/case_repair_sdk/
--rw-r--r--   0 root         (0) root         (0)     7663 2022-09-14 13:08:12.000000 minium-1.4.0/minium/native/lib/case_repair_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2816 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/case_repair_sdk/default_trace.py
--rw-r--r--   0 root         (0) root         (0)       22 2022-09-14 13:08:12.000000 minium-1.4.0/minium/native/lib/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.356473 minium-1.4.0/minium/native/lib/wda/
--rw-r--r--   0 root         (0) root         (0)    40664 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/wda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1297 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/wda/screenhelper.py
--rw-r--r--   0 root         (0) root         (0)     1421 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/wda/xcui_element_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.356473 minium-1.4.0/minium/native/lib/wx_wda/
--rw-r--r--   0 root         (0) root         (0)      399 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/wx_wda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13188 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/wx_wda/wdaUI.py
--rw-r--r--   0 root         (0) root         (0)    16169 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/lib/wx_wda/webDriverTool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.356473 minium-1.4.0/minium/native/qq_native/
--rw-r--r--   0 root         (0) root         (0)      118 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/qq_native/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6435 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/qq_native/qandroidnative.py
--rw-r--r--   0 root         (0) root         (0)      804 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/qq_native/qbasenative.py
--rwxr-xr-x   0 root         (0) root         (0)    16882 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/qq_native/qiosnative.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.356473 minium-1.4.0/minium/native/wx_native/
--rw-r--r--   0 root         (0) root         (0)       23 2022-06-30 06:29:28.000000 minium-1.4.0/minium/native/wx_native/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39339 2023-04-27 02:49:44.000000 minium-1.4.0/minium/native/wx_native/androidnative.py
--rw-r--r--   0 root         (0) root         (0)    23791 2023-04-27 02:49:44.000000 minium-1.4.0/minium/native/wx_native/basenative.py
--rw-r--r--   0 root         (0) root         (0)     8053 2023-02-07 11:55:46.000000 minium-1.4.0/minium/native/wx_native/idenative.py
--rw-r--r--   0 root         (0) root         (0)    36096 2023-04-27 02:49:44.000000 minium-1.4.0/minium/native/wx_native/iosnative.py
--rw-r--r--   0 root         (0) root         (0)     3254 2023-04-27 02:49:44.000000 minium-1.4.0/minium/native/wx_native/wording.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.356473 minium-1.4.0/minium/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 06:29:28.000000 minium-1.4.0/minium/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-04-27 02:49:44.000000 minium-1.4.0/minium/utils/emitter.py
--rw-r--r--   0 root         (0) root         (0)      230 2022-10-14 03:16:26.000000 minium-1.4.0/minium/utils/eventloop.py
--rw-r--r--   0 root         (0) root         (0)     3873 2022-09-19 12:42:30.000000 minium-1.4.0/minium/utils/injectjs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.320474 minium-1.4.0/minium/utils/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.360473 minium-1.4.0/minium/utils/js/es5/
--rw-r--r--   0 root         (0) root         (0)      221 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/addCloudCallMockRule.js
--rw-r--r--   0 root         (0) root         (0)      255 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/addNetworkMockRule.js
--rw-r--r--   0 root         (0) root         (0)      277 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/callContextMethod.js
--rw-r--r--   0 root         (0) root         (0)       72 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/checkInject.js
--rw-r--r--   0 root         (0) root         (0)      217 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/cleanCloudCallMockRule.js
--rw-r--r--   0 root         (0) root         (0)      200 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/cleanNetworkMockRule.js
--rw-r--r--   0 root         (0) root         (0)      535 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/createContext.js
--rw-r--r--   0 root         (0) root         (0)      340 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/editEditorText.js
--rw-r--r--   0 root         (0) root         (0)      231 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/evalMockChooseImage.js
--rw-r--r--   0 root         (0) root         (0)      147 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/getAppConfig.js
--rw-r--r--   0 root         (0) root         (0)    38266 2023-04-27 03:03:14.000000 minium-1.4.0/minium/utils/js/es5/helpers.js
--rw-r--r--   0 root         (0) root         (0)      358 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/hookCurrentPageMethod.js
--rw-r--r--   0 root         (0) root         (0)      807 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/hookWxMethod.js
--rw-r--r--   0 root         (0) root         (0)      120 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideHandleAuthModal.js
--rw-r--r--   0 root         (0) root         (0)      207 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideHandleMap.js
--rw-r--r--   0 root         (0) root         (0)      120 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideHandleModal.js
--rw-r--r--   0 root         (0) root         (0)      487 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockAuth.js
--rw-r--r--   0 root         (0) root         (0)      216 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockAuthSetting.js
--rw-r--r--   0 root         (0) root         (0)     1176 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockChooseLocation.js
--rw-r--r--   0 root         (0) root         (0)     1196 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockGetLocation.js
--rw-r--r--   0 root         (0) root         (0)      459 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockGetUserProfile.js
--rw-r--r--   0 root         (0) root         (0)      689 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockGetWeRunData.js
--rw-r--r--   0 root         (0) root         (0)     1480 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockModal.js
--rw-r--r--   0 root         (0) root         (0)      441 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockShowActionSheet.js
--rw-r--r--   0 root         (0) root         (0)      434 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockShowModal.js
--rw-r--r--   0 root         (0) root         (0)      501 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/ideMockSubscribeMessage.js
--rw-r--r--   0 root         (0) root         (0)     5247 2023-04-27 03:03:12.000000 minium-1.4.0/minium/utils/js/es5/mockChooseImage.js
--rw-r--r--   0 root         (0) root         (0)     1583 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/mockCloudCall.js
--rw-r--r--   0 root         (0) root         (0)     2838 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/mockNetwork.js
--rw-r--r--   0 root         (0) root         (0)      726 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/mockRequestStack.js
--rw-r--r--   0 root         (0) root         (0)     1215 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/networkPannel.js
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/releaseHookWxMethod.js
--rw-r--r--   0 root         (0) root         (0)     1171 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/requestStack.js
--rw-r--r--   0 root         (0) root         (0)      285 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/startGetPerformance.js
--rw-r--r--   0 root         (0) root         (0)      198 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/stopGetPerformance.js
--rw-r--r--   0 root         (0) root         (0)     7139 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/testAsync.js
--rw-r--r--   0 root         (0) root         (0)      307 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/uuid.js
--rw-r--r--   0 root         (0) root         (0)      181 2023-04-27 03:03:13.000000 minium-1.4.0/minium/utils/js/es5/waitUtil.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.364473 minium-1.4.0/minium/utils/js/min/
--rw-r--r--   0 root         (0) root         (0)      195 2023-04-27 03:03:26.000000 minium-1.4.0/minium/utils/js/min/addCloudCallMockRule.js
--rw-r--r--   0 root         (0) root         (0)      256 2023-04-27 03:03:23.000000 minium-1.4.0/minium/utils/js/min/addNetworkMockRule.js
--rw-r--r--   0 root         (0) root         (0)      198 2023-04-27 03:03:24.000000 minium-1.4.0/minium/utils/js/min/callContextMethod.js
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-27 03:03:19.000000 minium-1.4.0/minium/utils/js/min/checkInject.js
--rw-r--r--   0 root         (0) root         (0)      191 2023-04-27 03:03:20.000000 minium-1.4.0/minium/utils/js/min/cleanCloudCallMockRule.js
--rw-r--r--   0 root         (0) root         (0)      201 2023-04-27 03:03:19.000000 minium-1.4.0/minium/utils/js/min/cleanNetworkMockRule.js
--rw-r--r--   0 root         (0) root         (0)      412 2023-04-27 03:03:18.000000 minium-1.4.0/minium/utils/js/min/createContext.js
--rw-r--r--   0 root         (0) root         (0)      306 2023-04-27 03:03:21.000000 minium-1.4.0/minium/utils/js/min/editEditorText.js
--rw-r--r--   0 root         (0) root         (0)      183 2023-04-27 03:03:23.000000 minium-1.4.0/minium/utils/js/min/evalMockChooseImage.js
--rw-r--r--   0 root         (0) root         (0)      146 2023-04-27 03:03:21.000000 minium-1.4.0/minium/utils/js/min/getAppConfig.js
--rw-r--r--   0 root         (0) root         (0)    38266 2023-04-27 03:03:25.000000 minium-1.4.0/minium/utils/js/min/helpers.js
--rw-r--r--   0 root         (0) root         (0)      270 2023-04-27 03:03:21.000000 minium-1.4.0/minium/utils/js/min/hookCurrentPageMethod.js
--rw-r--r--   0 root         (0) root         (0)      664 2023-04-27 03:03:23.000000 minium-1.4.0/minium/utils/js/min/hookWxMethod.js
--rw-r--r--   0 root         (0) root         (0)      121 2023-04-27 03:03:17.000000 minium-1.4.0/minium/utils/js/min/ideHandleAuthModal.js
--rw-r--r--   0 root         (0) root         (0)      202 2023-04-27 03:03:16.000000 minium-1.4.0/minium/utils/js/min/ideHandleMap.js
--rw-r--r--   0 root         (0) root         (0)      121 2023-04-27 03:03:24.000000 minium-1.4.0/minium/utils/js/min/ideHandleModal.js
--rw-r--r--   0 root         (0) root         (0)      470 2023-04-27 03:03:15.000000 minium-1.4.0/minium/utils/js/min/ideMockAuth.js
--rw-r--r--   0 root         (0) root         (0)      154 2023-04-27 03:03:18.000000 minium-1.4.0/minium/utils/js/min/ideMockAuthSetting.js
--rw-r--r--   0 root         (0) root         (0)     1118 2023-04-27 03:03:18.000000 minium-1.4.0/minium/utils/js/min/ideMockChooseLocation.js
--rw-r--r--   0 root         (0) root         (0)     1202 2023-04-27 03:03:21.000000 minium-1.4.0/minium/utils/js/min/ideMockGetLocation.js
--rw-r--r--   0 root         (0) root         (0)      428 2023-04-27 03:03:24.000000 minium-1.4.0/minium/utils/js/min/ideMockGetUserProfile.js
--rw-r--r--   0 root         (0) root         (0)      695 2023-04-27 03:03:16.000000 minium-1.4.0/minium/utils/js/min/ideMockGetWeRunData.js
--rw-r--r--   0 root         (0) root         (0)     1413 2023-04-27 03:03:17.000000 minium-1.4.0/minium/utils/js/min/ideMockModal.js
--rw-r--r--   0 root         (0) root         (0)      417 2023-04-27 03:03:19.000000 minium-1.4.0/minium/utils/js/min/ideMockShowActionSheet.js
--rw-r--r--   0 root         (0) root         (0)      417 2023-04-27 03:03:15.000000 minium-1.4.0/minium/utils/js/min/ideMockShowModal.js
--rw-r--r--   0 root         (0) root         (0)      494 2023-04-27 03:03:18.000000 minium-1.4.0/minium/utils/js/min/ideMockSubscribeMessage.js
--rw-r--r--   0 root         (0) root         (0)     4368 2023-04-27 03:03:16.000000 minium-1.4.0/minium/utils/js/min/mockChooseImage.js
--rw-r--r--   0 root         (0) root         (0)     1386 2023-04-27 03:03:22.000000 minium-1.4.0/minium/utils/js/min/mockCloudCall.js
--rw-r--r--   0 root         (0) root         (0)     2327 2023-04-27 03:03:17.000000 minium-1.4.0/minium/utils/js/min/mockNetwork.js
--rw-r--r--   0 root         (0) root         (0)      664 2023-04-27 03:03:23.000000 minium-1.4.0/minium/utils/js/min/mockRequestStack.js
--rw-r--r--   0 root         (0) root         (0)     1192 2023-04-27 03:03:15.000000 minium-1.4.0/minium/utils/js/min/networkPannel.js
--rw-r--r--   0 root         (0) root         (0)      282 2023-04-27 03:03:19.000000 minium-1.4.0/minium/utils/js/min/releaseHookWxMethod.js
--rw-r--r--   0 root         (0) root         (0)     1018 2023-04-27 03:03:20.000000 minium-1.4.0/minium/utils/js/min/requestStack.js
--rw-r--r--   0 root         (0) root         (0)      284 2023-04-27 03:03:22.000000 minium-1.4.0/minium/utils/js/min/startGetPerformance.js
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-27 03:03:20.000000 minium-1.4.0/minium/utils/js/min/stopGetPerformance.js
--rw-r--r--   0 root         (0) root         (0)       94 2023-04-27 03:03:26.000000 minium-1.4.0/minium/utils/js/min/testAsync.js
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-27 03:03:25.000000 minium-1.4.0/minium/utils/js/min/uuid.js
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-27 03:03:22.000000 minium-1.4.0/minium/utils/js/min/waitUtil.js
--rw-r--r--   0 root         (0) root         (0)     1727 2023-04-27 02:49:44.000000 minium-1.4.0/minium/utils/meta.py
--rw-r--r--   0 root         (0) root         (0)      162 2022-06-30 06:29:28.000000 minium-1.4.0/minium/utils/platforms.py
--rw-r--r--   0 root         (0) root         (0)    15200 2023-04-27 02:49:44.000000 minium-1.4.0/minium/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 03:03:31.320474 minium-1.4.0/minium.egg-info/
--rw-r--r--   0 root         (0) root         (0)      697 2023-04-27 03:03:30.000000 minium-1.4.0/minium.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9058 2023-04-27 03:03:30.000000 minium-1.4.0/minium.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 03:03:30.000000 minium-1.4.0/minium.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2023-04-27 03:03:30.000000 minium-1.4.0/minium.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-04-27 03:03:30.000000 minium-1.4.0/minium.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-27 03:03:30.000000 minium-1.4.0/minium.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 03:03:31.364473 minium-1.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2435 2023-04-27 02:49:44.000000 minium-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.526981 minium-1.4.1/
+-rw-r--r--   0 root         (0) root         (0)      697 2023-05-09 06:44:43.526981 minium-1.4.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.482981 minium-1.4.1/minium/
+-rw-r--r--   0 root         (0) root         (0)      948 2023-04-27 02:49:43.000000 minium-1.4.1/minium/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.490981 minium-1.4.1/minium/framework/
+-rw-r--r--   0 root         (0) root         (0)       58 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18583 2023-04-27 02:49:43.000000 minium-1.4.1/minium/framework/assertbase.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2022-11-07 03:36:55.000000 minium-1.4.1/minium/framework/casedump.py
+-rw-r--r--   0 root         (0) root         (0)     7702 2022-11-07 03:36:55.000000 minium-1.4.1/minium/framework/caseinspect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.490981 minium-1.4.1/minium/framework/dist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.490981 minium-1.4.1/minium/framework/dist/css/
+-rw-r--r--   0 root         (0) root         (0)      437 2022-09-14 13:08:12.000000 minium-1.4.1/minium/framework/dist/css/app.87891bf0.css
+-rw-r--r--   0 root         (0) root         (0)   240799 2022-09-14 13:08:12.000000 minium-1.4.1/minium/framework/dist/css/chunk-vendors.52eeca6f.css
+-rw-r--r--   0 root         (0) root         (0)     2108 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/dist/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.490981 minium-1.4.1/minium/framework/dist/fonts/
+-rw-r--r--   0 root         (0) root         (0)    28200 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/dist/fonts/element-icons.535877f5.woff
+-rw-r--r--   0 root         (0) root         (0)    55956 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/dist/fonts/element-icons.732389de.ttf
+-rw-r--r--   0 root         (0) root         (0)      847 2022-09-14 13:08:12.000000 minium-1.4.1/minium/framework/dist/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.490981 minium-1.4.1/minium/framework/dist/js/
+-rw-r--r--   0 root         (0) root         (0)    17537 2022-09-14 13:08:12.000000 minium-1.4.1/minium/framework/dist/js/app.544bedf4.js
+-rw-r--r--   0 root         (0) root         (0)  1346000 2022-09-14 13:08:12.000000 minium-1.4.1/minium/framework/dist/js/chunk-vendors.22ed339a.js
+-rw-r--r--   0 root         (0) root         (0)     3463 2023-01-16 03:26:29.000000 minium-1.4.1/minium/framework/errorReport.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-05-09 06:36:06.000000 minium-1.4.1/minium/framework/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.494981 minium-1.4.1/minium/framework/libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.494981 minium-1.4.1/minium/framework/libs/tgit/
+-rw-r--r--   0 root         (0) root         (0)      152 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/libs/tgit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/libs/tgit/auth.py
+-rw-r--r--   0 root         (0) root         (0)    97301 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/libs/tgit/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.494981 minium-1.4.1/minium/framework/libs/unittest/
+-rw-r--r--   0 root         (0) root         (0)      243 2022-12-28 03:15:03.000000 minium-1.4.1/minium/framework/libs/unittest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11757 2023-04-27 02:49:43.000000 minium-1.4.1/minium/framework/libs/unittest/case.py
+-rw-r--r--   0 root         (0) root         (0)     5656 2023-04-27 02:49:43.000000 minium-1.4.1/minium/framework/libs/unittest/suite.py
+-rw-r--r--   0 root         (0) root         (0)    19830 2022-12-19 02:27:07.000000 minium-1.4.1/minium/framework/loader.py
+-rw-r--r--   0 root         (0) root         (0)    10166 2023-04-27 02:49:43.000000 minium-1.4.1/minium/framework/logcolor.py
+-rw-r--r--   0 root         (0) root         (0)     7244 2023-04-27 02:49:43.000000 minium-1.4.1/minium/framework/miniconfig.py
+-rw-r--r--   0 root         (0) root         (0)     3427 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/miniddt.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-02-07 07:19:07.000000 minium-1.4.1/minium/framework/minidoctor.py
+-rw-r--r--   0 root         (0) root         (0)     1207 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/minilimit.py
+-rw-r--r--   0 root         (0) root         (0)      832 2022-09-14 13:08:12.000000 minium-1.4.1/minium/framework/miniprogram.py
+-rw-r--r--   0 root         (0) root         (0)     6669 2022-09-14 13:08:12.000000 minium-1.4.1/minium/framework/miniresult.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-04-27 02:49:43.000000 minium-1.4.1/minium/framework/minisuite.py
+-rw-r--r--   0 root         (0) root         (0)    29430 2023-04-27 02:49:43.000000 minium-1.4.1/minium/framework/minitest.py
+-rw-r--r--   0 root         (0) root         (0)    17061 2023-04-27 02:49:43.000000 minium-1.4.1/minium/framework/report.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-05-09 06:36:06.000000 minium-1.4.1/minium/framework/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.494981 minium-1.4.1/minium/framework/tools/
+-rw-r--r--   0 root         (0) root         (0)       54 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/tools/report_issue.py
+-rw-r--r--   0 root         (0) root         (0)     3974 2022-12-19 02:27:07.000000 minium-1.4.1/minium/framework/wording.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.494981 minium-1.4.1/minium/miniprogram/
+-rw-r--r--   0 root         (0) root         (0)      688 2023-04-27 02:49:43.000000 minium-1.4.1/minium/miniprogram/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.498981 minium-1.4.1/minium/miniprogram/base_driver/
+-rw-r--r--   0 root         (0) root         (0)      191 2022-06-30 06:29:28.000000 minium-1.4.1/minium/miniprogram/base_driver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47565 2023-05-09 06:36:06.000000 minium-1.4.1/minium/miniprogram/base_driver/app.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2023-04-27 02:49:43.000000 minium-1.4.1/minium/miniprogram/base_driver/callback.py
+-rw-r--r--   0 root         (0) root         (0)    28828 2023-04-27 02:49:43.000000 minium-1.4.1/minium/miniprogram/base_driver/connection.py
+-rw-r--r--   0 root         (0) root         (0)    46414 2023-04-27 02:49:43.000000 minium-1.4.1/minium/miniprogram/base_driver/element.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-04-27 02:49:43.000000 minium-1.4.1/minium/miniprogram/base_driver/minium.py
+-rw-r--r--   0 root         (0) root         (0)     5475 2023-05-09 06:36:06.000000 minium-1.4.1/minium/miniprogram/base_driver/minium_log.py
+-rw-r--r--   0 root         (0) root         (0)     8485 2023-04-27 02:49:44.000000 minium-1.4.1/minium/miniprogram/base_driver/minium_object.py
+-rw-r--r--   0 root         (0) root         (0)    23560 2023-04-27 02:49:44.000000 minium-1.4.1/minium/miniprogram/base_driver/page.py
+-rw-r--r--   0 root         (0) root         (0)      771 2022-06-30 06:29:28.000000 minium-1.4.1/minium/miniprogram/base_driver/prefixer.py
+-rw-r--r--   0 root         (0) root         (0)      132 2023-05-09 06:44:40.000000 minium-1.4.1/minium/miniprogram/base_driver/version.json
+-rw-r--r--   0 root         (0) root         (0)      552 2023-04-27 02:49:44.000000 minium-1.4.1/minium/miniprogram/base_driver/version.py
+-rw-r--r--   0 root         (0) root         (0)      263 2022-06-30 06:29:28.000000 minium-1.4.1/minium/miniprogram/base_driver/waiter.py
+-rw-r--r--   0 root         (0) root         (0)     6692 2022-06-30 06:29:28.000000 minium-1.4.1/minium/miniprogram/qq_minium.py
+-rw-r--r--   0 root         (0) root         (0)    38940 2023-05-09 06:36:06.000000 minium-1.4.1/minium/miniprogram/wx_minium.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.498981 minium-1.4.1/minium/native/
+-rw-r--r--   0 root         (0) root         (0)     3218 2022-12-19 02:27:07.000000 minium-1.4.1/minium/native/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.498981 minium-1.4.1/minium/native/lib/
+-rw-r--r--   0 root         (0) root         (0)       58 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.498981 minium-1.4.1/minium/native/lib/android_base/
+-rw-r--r--   0 root         (0) root         (0)     1012 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/android_base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.502981 minium-1.4.1/minium/native/lib/at/
+-rw-r--r--   0 root         (0) root         (0)     4087 2022-09-14 13:08:12.000000 minium-1.4.1/minium/native/lib/at/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/apkapi.py
+-rw-r--r--   0 root         (0) root         (0)     5609 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/atproxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.506981 minium-1.4.1/minium/native/lib/at/bin/
+-rw-r--r--   0 root         (0) root         (0)  3566862 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/bin/AtServer.apk
+-rw-r--r--   0 root         (0) root         (0)    95449 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/bin/AtStub.jar
+-rw-r--r--   0 root         (0) root         (0)     3222 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/command_line.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.506981 minium-1.4.1/minium/native/lib/at/core/
+-rw-r--r--   0 root         (0) root         (0)       37 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      951 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/accesshelper.py
+-rw-r--r--   0 root         (0) root         (0)    46986 2022-09-14 13:08:12.000000 minium-1.4.1/minium/native/lib/at/core/adbwrap.py
+-rw-r--r--   0 root         (0) root         (0)    10763 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/basedriver.py
+-rw-r--r--   0 root         (0) root         (0)    15919 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/case_repair_adapter.py
+-rw-r--r--   0 root         (0) root         (0)      624 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/config.py
+-rw-r--r--   0 root         (0) root         (0)    31731 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/element.py
+-rw-r--r--   0 root         (0) root         (0)      669 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    18740 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/javadriver.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/resguard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.506981 minium-1.4.1/minium/native/lib/at/core/stf/
+-rw-r--r--   0 root         (0) root         (0)       56 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/stf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/stf/mincap.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/stf/minitouch.py
+-rw-r--r--   0 root         (0) root         (0)    11600 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/uidevice.py
+-rw-r--r--   0 root         (0) root         (0)    17965 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/uixml.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/websocketcli.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/eventmonitor.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/hook.py
+-rw-r--r--   0 root         (0) root         (0)     8495 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/jlogcat.py
+-rw-r--r--   0 root         (0) root         (0)    36015 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/keycode.py
+-rw-r--r--   0 root         (0) root         (0)     9492 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/perfcollector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.506981 minium-1.4.1/minium/native/lib/at/tests/
+-rw-r--r--   0 root         (0) root         (0)      690 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/AtEvent.py
+-rw-r--r--   0 root         (0) root         (0)      326 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/AtSocket.py
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      480 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/adbtest.py
+-rw-r--r--   0 root         (0) root         (0)      490 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/airtesttest.py
+-rw-r--r--   0 root         (0) root         (0)    10434 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/atdevicetest.py
+-rw-r--r--   0 root         (0) root         (0)      474 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/attestbase.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/drivertest.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/elementtest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.510981 minium-1.4.1/minium/native/lib/at/tests/images/
+-rw-r--r--   0 root         (0) root         (0)     7525 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/images/1.jpg
+-rw-r--r--   0 root         (0) root         (0)     4388 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/images/2.jpg
+-rw-r--r--   0 root         (0) root         (0)    80712 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/images/image.jpg
+-rw-r--r--   0 root         (0) root         (0)      493 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/javadrivertest.py
+-rw-r--r--   0 root         (0) root         (0)      480 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/minicap_test.py
+-rw-r--r--   0 root         (0) root         (0)      375 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/minitest.py
+-rw-r--r--   0 root         (0) root         (0)      843 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/minitouch_test.py
+-rw-r--r--   0 root         (0) root         (0)      792 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/u2test.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/uixmltest.py
+-rw-r--r--   0 root         (0) root         (0)      493 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/vs_test.py
+-rw-r--r--   0 root         (0) root         (0)      989 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/webdrivertest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.510981 minium-1.4.1/minium/native/lib/at/utils/
+-rw-r--r--   0 root         (0) root         (0)       37 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4896 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/apkinfo.py
+-rw-r--r--   0 root         (0) root         (0)   105609 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/axmlparser.py
+-rw-r--r--   0 root         (0) root         (0)    27360 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/axmlparser3.py
+-rw-r--r--   0 root         (0) root         (0)      526 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/commonhelper.py
+-rw-r--r--   0 root         (0) root         (0)     8332 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/decorator.py
+-rw-r--r--   0 root         (0) root         (0)      257 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/magic.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/nbsp.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/threadhelper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.510981 minium-1.4.1/minium/native/lib/at/vision/
+-rw-r--r--   0 root         (0) root         (0)       56 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/vision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      394 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/vision/template_match.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.514981 minium-1.4.1/minium/native/lib/at/webdriver/
+-rw-r--r--   0 root         (0) root         (0)       72 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15310 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/driver.py
+-rw-r--r--   0 root         (0) root         (0)      425 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/error.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/jsapi.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/miniapp.py
+-rw-r--r--   0 root         (0) root         (0)    18973 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/stub.js
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/tabdescription.py
+-rw-r--r--   0 root         (0) root         (0)    13005 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/tabwebsocket.py
+-rw-r--r--   0 root         (0) root         (0)     8904 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/webelement.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/webhelper.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/wspools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.514981 minium-1.4.1/minium/native/lib/at/wechat/
+-rw-r--r--   0 root         (0) root         (0)       79 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/wechat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/wechat/activtiy.py
+-rw-r--r--   0 root         (0) root         (0)      144 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/wechat/appvars.py
+-rw-r--r--   0 root         (0) root         (0)       80 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/wsimp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.514981 minium-1.4.1/minium/native/lib/case_repair_sdk/
+-rw-r--r--   0 root         (0) root         (0)     7663 2022-09-14 13:08:12.000000 minium-1.4.1/minium/native/lib/case_repair_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/case_repair_sdk/default_trace.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-09-14 13:08:12.000000 minium-1.4.1/minium/native/lib/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.514981 minium-1.4.1/minium/native/lib/wda/
+-rw-r--r--   0 root         (0) root         (0)    40664 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/wda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/wda/screenhelper.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/wda/xcui_element_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.514981 minium-1.4.1/minium/native/lib/wx_wda/
+-rw-r--r--   0 root         (0) root         (0)      399 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/wx_wda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/wx_wda/wdaUI.py
+-rw-r--r--   0 root         (0) root         (0)    16169 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/wx_wda/webDriverTool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.514981 minium-1.4.1/minium/native/qq_native/
+-rw-r--r--   0 root         (0) root         (0)      118 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/qq_native/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/qq_native/qandroidnative.py
+-rw-r--r--   0 root         (0) root         (0)      804 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/qq_native/qbasenative.py
+-rwxr-xr-x   0 root         (0) root         (0)    16882 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/qq_native/qiosnative.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.514981 minium-1.4.1/minium/native/wx_native/
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/wx_native/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39339 2023-04-27 02:49:44.000000 minium-1.4.1/minium/native/wx_native/androidnative.py
+-rw-r--r--   0 root         (0) root         (0)    23791 2023-04-27 02:49:44.000000 minium-1.4.1/minium/native/wx_native/basenative.py
+-rw-r--r--   0 root         (0) root         (0)     8053 2023-02-07 11:55:46.000000 minium-1.4.1/minium/native/wx_native/idenative.py
+-rw-r--r--   0 root         (0) root         (0)    36096 2023-04-27 02:49:44.000000 minium-1.4.1/minium/native/wx_native/iosnative.py
+-rw-r--r--   0 root         (0) root         (0)     3254 2023-04-27 02:49:44.000000 minium-1.4.1/minium/native/wx_native/wording.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.518981 minium-1.4.1/minium/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 06:29:28.000000 minium-1.4.1/minium/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-04-27 02:49:44.000000 minium-1.4.1/minium/utils/emitter.py
+-rw-r--r--   0 root         (0) root         (0)      230 2022-10-14 03:16:26.000000 minium-1.4.1/minium/utils/eventloop.py
+-rw-r--r--   0 root         (0) root         (0)     3873 2022-09-19 12:42:30.000000 minium-1.4.1/minium/utils/injectjs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.482981 minium-1.4.1/minium/utils/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.522981 minium-1.4.1/minium/utils/js/es5/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/addCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      255 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/addNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      277 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/callContextMethod.js
+-rw-r--r--   0 root         (0) root         (0)       72 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/checkInject.js
+-rw-r--r--   0 root         (0) root         (0)      217 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/cleanCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/cleanNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      535 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/createContext.js
+-rw-r--r--   0 root         (0) root         (0)      340 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/editEditorText.js
+-rw-r--r--   0 root         (0) root         (0)      231 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/evalMockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)      147 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/getAppConfig.js
+-rw-r--r--   0 root         (0) root         (0)      617 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/getUni.js
+-rw-r--r--   0 root         (0) root         (0)    38266 2023-05-09 06:44:27.000000 minium-1.4.1/minium/utils/js/es5/helpers.js
+-rw-r--r--   0 root         (0) root         (0)      358 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/hookCurrentPageMethod.js
+-rw-r--r--   0 root         (0) root         (0)      807 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/hookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)      120 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/ideHandleAuthModal.js
+-rw-r--r--   0 root         (0) root         (0)      207 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/ideHandleMap.js
+-rw-r--r--   0 root         (0) root         (0)      120 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/ideHandleModal.js
+-rw-r--r--   0 root         (0) root         (0)      487 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/ideMockAuth.js
+-rw-r--r--   0 root         (0) root         (0)      216 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/ideMockAuthSetting.js
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/ideMockChooseLocation.js
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/ideMockGetLocation.js
+-rw-r--r--   0 root         (0) root         (0)      459 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/ideMockGetUserProfile.js
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/ideMockGetWeRunData.js
+-rw-r--r--   0 root         (0) root         (0)     1480 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/ideMockModal.js
+-rw-r--r--   0 root         (0) root         (0)      441 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/ideMockShowActionSheet.js
+-rw-r--r--   0 root         (0) root         (0)      434 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/ideMockShowModal.js
+-rw-r--r--   0 root         (0) root         (0)      501 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/ideMockSubscribeMessage.js
+-rw-r--r--   0 root         (0) root         (0)     5247 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/mockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)     1582 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/mockCloudCall.js
+-rw-r--r--   0 root         (0) root         (0)     2837 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/mockNetwork.js
+-rw-r--r--   0 root         (0) root         (0)      726 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/mockRequestStack.js
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/networkPannel.js
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/releaseHookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)     1171 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/requestStack.js
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/startGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/stopGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)     7138 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/testAsync.js
+-rw-r--r--   0 root         (0) root         (0)      307 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/uuid.js
+-rw-r--r--   0 root         (0) root         (0)      181 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/waitUtil.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.526981 minium-1.4.1/minium/utils/js/min/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-09 06:44:39.000000 minium-1.4.1/minium/utils/js/min/addCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      256 2023-05-09 06:44:36.000000 minium-1.4.1/minium/utils/js/min/addNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-09 06:44:37.000000 minium-1.4.1/minium/utils/js/min/callContextMethod.js
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-09 06:44:32.000000 minium-1.4.1/minium/utils/js/min/checkInject.js
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-09 06:44:33.000000 minium-1.4.1/minium/utils/js/min/cleanCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      201 2023-05-09 06:44:32.000000 minium-1.4.1/minium/utils/js/min/cleanNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      412 2023-05-09 06:44:31.000000 minium-1.4.1/minium/utils/js/min/createContext.js
+-rw-r--r--   0 root         (0) root         (0)      306 2023-05-09 06:44:34.000000 minium-1.4.1/minium/utils/js/min/editEditorText.js
+-rw-r--r--   0 root         (0) root         (0)      183 2023-05-09 06:44:36.000000 minium-1.4.1/minium/utils/js/min/evalMockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-09 06:44:34.000000 minium-1.4.1/minium/utils/js/min/getAppConfig.js
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-09 06:44:39.000000 minium-1.4.1/minium/utils/js/min/getUni.js
+-rw-r--r--   0 root         (0) root         (0)    38266 2023-05-09 06:44:38.000000 minium-1.4.1/minium/utils/js/min/helpers.js
+-rw-r--r--   0 root         (0) root         (0)      270 2023-05-09 06:44:34.000000 minium-1.4.1/minium/utils/js/min/hookCurrentPageMethod.js
+-rw-r--r--   0 root         (0) root         (0)      664 2023-05-09 06:44:36.000000 minium-1.4.1/minium/utils/js/min/hookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)      121 2023-05-09 06:44:30.000000 minium-1.4.1/minium/utils/js/min/ideHandleAuthModal.js
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-09 06:44:29.000000 minium-1.4.1/minium/utils/js/min/ideHandleMap.js
+-rw-r--r--   0 root         (0) root         (0)      121 2023-05-09 06:44:37.000000 minium-1.4.1/minium/utils/js/min/ideHandleModal.js
+-rw-r--r--   0 root         (0) root         (0)      470 2023-05-09 06:44:28.000000 minium-1.4.1/minium/utils/js/min/ideMockAuth.js
+-rw-r--r--   0 root         (0) root         (0)      154 2023-05-09 06:44:31.000000 minium-1.4.1/minium/utils/js/min/ideMockAuthSetting.js
+-rw-r--r--   0 root         (0) root         (0)     1118 2023-05-09 06:44:31.000000 minium-1.4.1/minium/utils/js/min/ideMockChooseLocation.js
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-05-09 06:44:34.000000 minium-1.4.1/minium/utils/js/min/ideMockGetLocation.js
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-09 06:44:37.000000 minium-1.4.1/minium/utils/js/min/ideMockGetUserProfile.js
+-rw-r--r--   0 root         (0) root         (0)      695 2023-05-09 06:44:29.000000 minium-1.4.1/minium/utils/js/min/ideMockGetWeRunData.js
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-09 06:44:30.000000 minium-1.4.1/minium/utils/js/min/ideMockModal.js
+-rw-r--r--   0 root         (0) root         (0)      417 2023-05-09 06:44:32.000000 minium-1.4.1/minium/utils/js/min/ideMockShowActionSheet.js
+-rw-r--r--   0 root         (0) root         (0)      417 2023-05-09 06:44:28.000000 minium-1.4.1/minium/utils/js/min/ideMockShowModal.js
+-rw-r--r--   0 root         (0) root         (0)      494 2023-05-09 06:44:31.000000 minium-1.4.1/minium/utils/js/min/ideMockSubscribeMessage.js
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-05-09 06:44:29.000000 minium-1.4.1/minium/utils/js/min/mockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-05-09 06:44:35.000000 minium-1.4.1/minium/utils/js/min/mockCloudCall.js
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-05-09 06:44:30.000000 minium-1.4.1/minium/utils/js/min/mockNetwork.js
+-rw-r--r--   0 root         (0) root         (0)      664 2023-05-09 06:44:36.000000 minium-1.4.1/minium/utils/js/min/mockRequestStack.js
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-05-09 06:44:28.000000 minium-1.4.1/minium/utils/js/min/networkPannel.js
+-rw-r--r--   0 root         (0) root         (0)      282 2023-05-09 06:44:32.000000 minium-1.4.1/minium/utils/js/min/releaseHookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-05-09 06:44:33.000000 minium-1.4.1/minium/utils/js/min/requestStack.js
+-rw-r--r--   0 root         (0) root         (0)      284 2023-05-09 06:44:35.000000 minium-1.4.1/minium/utils/js/min/startGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)      199 2023-05-09 06:44:33.000000 minium-1.4.1/minium/utils/js/min/stopGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)       94 2023-05-09 06:44:39.000000 minium-1.4.1/minium/utils/js/min/testAsync.js
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-09 06:44:38.000000 minium-1.4.1/minium/utils/js/min/uuid.js
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-09 06:44:35.000000 minium-1.4.1/minium/utils/js/min/waitUtil.js
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-04-27 02:49:44.000000 minium-1.4.1/minium/utils/meta.py
+-rw-r--r--   0 root         (0) root         (0)      162 2022-06-30 06:29:28.000000 minium-1.4.1/minium/utils/platforms.py
+-rw-r--r--   0 root         (0) root         (0)    15512 2023-05-09 06:36:06.000000 minium-1.4.1/minium/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.486981 minium-1.4.1/minium.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      697 2023-05-09 06:44:43.000000 minium-1.4.1/minium.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9118 2023-05-09 06:44:43.000000 minium-1.4.1/minium.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 06:44:43.000000 minium-1.4.1/minium.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2023-05-09 06:44:43.000000 minium-1.4.1/minium.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-09 06:44:43.000000 minium-1.4.1/minium.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-09 06:44:43.000000 minium-1.4.1/minium.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 06:44:43.526981 minium-1.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-05-09 06:36:06.000000 minium-1.4.1/setup.py
```

### Comparing `minium-1.4.0/PKG-INFO` & `minium-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minium
-Version: 1.4.0
+Version: 1.4.1
 Summary: Minium is the best MiniProgram auto test framework.
 Home-page: https://minitest.weixin.qq.com/#/
 Author: WeChat-Test
 Author-email: minitest@tencent.com
 License: MIT
 Description: 
         install:
```

### Comparing `minium-1.4.0/minium/__init__.py` & `minium-1.4.1/minium/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/assertbase.py` & `minium-1.4.1/minium/framework/assertbase.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/casedump.py` & `minium-1.4.1/minium/framework/casedump.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/caseinspect.py` & `minium-1.4.1/minium/framework/caseinspect.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/dist/css/chunk-vendors.52eeca6f.css` & `minium-1.4.1/minium/framework/dist/css/chunk-vendors.52eeca6f.css`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/dist/favicon.ico` & `minium-1.4.1/minium/framework/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/dist/fonts/element-icons.535877f5.woff` & `minium-1.4.1/minium/framework/dist/fonts/element-icons.535877f5.woff`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/dist/fonts/element-icons.732389de.ttf` & `minium-1.4.1/minium/framework/dist/fonts/element-icons.732389de.ttf`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/dist/index.html` & `minium-1.4.1/minium/framework/dist/index.html`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/dist/js/app.544bedf4.js` & `minium-1.4.1/minium/framework/dist/js/app.544bedf4.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/dist/js/chunk-vendors.22ed339a.js` & `minium-1.4.1/minium/framework/dist/js/chunk-vendors.22ed339a.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/errorReport.py` & `minium-1.4.1/minium/framework/errorReport.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/exception.py` & `minium-1.4.1/minium/framework/exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,26 +3,19 @@
 """
 Author:         lockerzhang
 Filename:       exception.py
 Create time:    2020/4/22 22:13
 Description:
 
 """
-import minium.miniprogram.base_driver.minium_log as minum_log
-import time
 
 
 class MiniError(Exception):
     def __init__(self, msg):  # real signature unknown
-        ep_data = {}
-        ep_data["TimeStamp"] = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
-        ep_data["Type"] = str(self.__class__.__name__)
-        ep_data["Args"] = msg
-        ep_data["Trace"] = ""
-        minum_log.report_exception(ep_data)
+        self.msg = msg
         Exception.__init__(self, msg)
 
 
 class MiniConnectError(MiniError):
     ...
 
 
@@ -48,14 +41,15 @@
     ...
 
 
 # 调试通道错误
 class MiniDebugConnectionError(MiniConnectError):
     ...
 
+
 # 因断连造成的未收到指令回复
 class MiniTimeoutCauseByConnectionBreakError(
     MiniTimeoutError, MiniConnectionClosedError
 ):
     ...
 
 
@@ -113,9 +107,10 @@
         if len(args) > 0 and isinstance(args[0], ModuleNotFoundError):
             err = args[0]
             super().__init__(err.msg, *args[1:], name=err.name, path=err.path)
             self.with_traceback(err.__traceback__)
         else:
             super().__init__(*args, name=name, path=path)
 
+
 class RemoteDebugConnectionLost(MiniAppError):  # 远程调试服务掉线
     ...
```

### Comparing `minium-1.4.0/minium/framework/libs/tgit/auth.py` & `minium-1.4.1/minium/framework/libs/tgit/auth.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/libs/tgit/client.py` & `minium-1.4.1/minium/framework/libs/tgit/client.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/libs/unittest/case.py` & `minium-1.4.1/minium/framework/libs/unittest/case.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/libs/unittest/suite.py` & `minium-1.4.1/minium/framework/libs/unittest/suite.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/loader.py` & `minium-1.4.1/minium/framework/loader.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/logcolor.py` & `minium-1.4.1/minium/framework/logcolor.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/miniconfig.py` & `minium-1.4.1/minium/framework/miniconfig.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/miniddt.py` & `minium-1.4.1/minium/framework/miniddt.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/minilimit.py` & `minium-1.4.1/minium/framework/minilimit.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/miniprogram.py` & `minium-1.4.1/minium/framework/miniprogram.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/miniresult.py` & `minium-1.4.1/minium/framework/miniresult.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/minisuite.py` & `minium-1.4.1/minium/framework/minisuite.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/minitest.py` & `minium-1.4.1/minium/framework/minitest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/report.py` & `minium-1.4.1/minium/framework/report.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/session.py` & `minium-1.4.1/minium/framework/session.py`

 * *Files 14% similar despite different names*

```diff
@@ -66,24 +66,20 @@
             except Empty:
                 logger.info(f"case queue is empty, test complete, release {self.device_id}")
                 break
             except Exception as e:
                 logger.info("run case error")
                 logger.exception(e)
                 exc_type, exc_value, exc_traceback = sys.exc_info()
-                ep_data = {}
-                ep_data["TimeStamp"] = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
-                ep_data["Type"] = str(exc_type)
-                ep_data["Args"] = str(exc_value)
-                ep_data["Trace"] = repr(traceback.format_tb(exc_traceback))
-                minum_log.report_exception(ep_data)
+                minum_log.report_exception(minum_log.ExceptionData(exc_value))
                 break
 
         try:
-            minitest.full_reset()
+            if not minitest.AssertBase.CONFIG.debug:
+                minitest.full_reset()
         except Exception as e:
             logger.error("reset error")
             logger.exception(e)
 
         # gen report
         if self.generate_report:
             report.imp_main(minitest.AssertBase.CONFIG.outputs)
```

### Comparing `minium-1.4.0/minium/framework/tools/report_issue.py` & `minium-1.4.1/minium/framework/tools/report_issue.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/framework/wording.py` & `minium-1.4.1/minium/framework/wording.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/miniprogram/__init__.py` & `minium-1.4.1/minium/miniprogram/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/miniprogram/base_driver/app.py` & `minium-1.4.1/minium/miniprogram/base_driver/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,31 +15,25 @@
 from .page import Page
 from .minium_object import MiniumObject, RetryableApi
 from ...framework.exception import *
 from ...utils.injectjs import getInjectJsCode, JsMode
 from ...utils.platforms import *
 from ...utils.emitter import ee
 from ...utils.eventloop import event_loop
-from ...utils.utils import get_result, WaitTimeoutError, retry, catch
+from ...utils.utils import get_result, WaitTimeoutError, retry, catch, urlencode
 from .callback import AsyncCallback, Callback
 import os
 import json
 import threading
 import base64
 import io
 import time
 import datetime
 import copy
 
-try:
-    import urllib as urlencoder
-
-    urlencoder.urlencode
-except (ImportError, AttributeError):
-    import urllib3.request as urlencoder
 
 cur_path = os.path.dirname(os.path.realpath(__file__))  # source_path是存放资源文件的路径
 conf_path = os.path.join(os.path.dirname(cur_path), "conf/iOS_conf")
 
 
 class MockNetworkType(Enum):
     ALWAYS = 0
@@ -517,17 +511,17 @@
         :param url:"/page/tabBar/API/index"
         :param params: 页面参数
         :param is_wait_url_change: 是否等待页面变换完成
         :return:Page 对象
         """
         if params:
             url += (
-                ("?" + urlencoder.urlencode(params))
+                ("?" + urlencode(params))
                 if url.find("?") < 0
-                else ("&" + urlencoder.urlencode(params))
+                else ("&" + urlencode(params))
             )
         self.logger.info("NavigateTo: %s" % url)
         page = self._change_route_async("navigateTo", url, is_wait_url_change)
         if page != url.split("?")[0]:
             self.logger.warning("NavigateTo(%s) but(%s)" % (url, page.path))
         return page
 
@@ -539,17 +533,17 @@
         :param url:"/page/tabBar/API/index"
         :param params: 页面参数
         :param is_wait_url_change: 是否等待页面变换完成
         :return:Page 对象
         """
         if params:
             url += (
-                ("?" + urlencoder.urlencode(params))
+                ("?" + urlencode(params))
                 if url.find("?") < 0
-                else ("&" + urlencoder.urlencode(params))
+                else ("&" + urlencode(params))
             )
         self.logger.info("RedirectTo: %s" % url)
         page = self._change_route_async("redirectTo", url, is_wait_url_change)
         if page != url.split("?")[0]:
             self.logger.warning("RedirectTo(%s) but(%s)" % (url, page.path))
         return page
 
@@ -559,17 +553,17 @@
         """
         关闭所有页面, 打开到应用内的某个页面
         :param url: "/page/tabBar/API/index"
         :return:Page 对象
         """
         if params:
             url += (
-                ("?" + urlencoder.urlencode(params))
+                ("?" + urlencode(params))
                 if url.find("?") < 0
-                else ("&" + urlencoder.urlencode(params))
+                else ("&" + urlencode(params))
             )
         self.logger.info("ReLaunch: %s" % url)
         page = self._change_route_async("reLaunch", url, is_wait_url_change)
         if page != url.split("?")[0]:
             self.logger.warning("ReLaunch(%s) but(%s)" % (url, page.path))
         return page
```

### Comparing `minium-1.4.0/minium/miniprogram/base_driver/callback.py` & `minium-1.4.1/minium/miniprogram/base_driver/callback.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/miniprogram/base_driver/connection.py` & `minium-1.4.1/minium/miniprogram/base_driver/connection.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/miniprogram/base_driver/element.py` & `minium-1.4.1/minium/miniprogram/base_driver/element.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/miniprogram/base_driver/minium.py` & `minium-1.4.1/minium/miniprogram/base_driver/minium.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/miniprogram/base_driver/minium_log.py` & `minium-1.4.1/minium/miniprogram/base_driver/minium_log.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,22 +13,59 @@
 import types
 import json
 import requests
 import queue
 import threading
 import logging
 import os
+import time
+import traceback
 from .version import build_version
+from ...framework.exception import MiniError
 
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 # logger = logging.getLogger("DataReport")
 
 REPORT_DOMAIN = "minitest.weixin.qq.com"
 REPORT_PATH = "xbeacon/user_report"
+app_id = None
+version = build_version().get("version")
+revision = build_version().get("revision")
+
+class ReportData(dict):
+    cmd = ""
 
+    def dumps(self):
+        return json.dumps(self)
+
+class ExceptionData(dict):
+    def __init__(self, err: Exception, **kwargs):
+        kwargs["from"] = "minium"
+        self.TimeStamp = getattr(err, "timestamp", None) or time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
+        self.error = err.__class__.__name__
+        self.err_msg = getattr(err, "msg", None) or str(err)
+        self.Uin = 0
+        self.version = version
+        self.revision = revision
+        self.ext = ""
+        self.app_id = app_id
+        self.__dict__.update(kwargs)
+        super().__init__(self.__dict__)
+        self.cmd = "cloud_exception_log"
+
+class ConsumeData(dict):
+    def __init__(self, __map: dict, **kwargs):
+        self.version = version
+        self.revision = revision
+        self.app_id = app_id
+        self.time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+        __map.update(kwargs)
+        self.__dict__.update(__map)
+        super().__init__(self.__dict__)
+        self.cmd = "api_log"
 
 def process_report():
     global existFlag
     while not existFlag:
         lock.acquire()
         lock.wait(10)
         lock.release()
@@ -44,45 +81,45 @@
         fail += 1
         if fail >= 10:
             existFlag = 1
     else:
         fail = 0
 
 
-def report_exception(data: dict):
-    if not app_id:
+def report_exception(data: ExceptionData):
+    if not data.app_id:
         return
-    data["Uin"] = 0
-    data["version"] = ""
-    data["ext"] = ""
-    data["app_id"] = app_id
-    data["AppID"] = app_id
-    return report(data, "exception_log")
+    report_queue.put(data)
+    lock.acquire()
+    lock.notify()
+    lock.release()
 
 
-def report(data: dict, cmd="api_log"):
+def report(data: ReportData):
     """
     report minium_new
     """
     if existFlag:
         return
+    print(f"https://{REPORT_DOMAIN}/{REPORT_PATH}/{data.cmd}")
+    print(data)
     try:
         ret = requests.post(
-            url=f"https://{REPORT_DOMAIN}/{REPORT_PATH}/{cmd}",
-            data=json.dumps(data),
+            url=f"https://{REPORT_DOMAIN}/{REPORT_PATH}/{data.cmd}",
+            data=data.dumps(),
             timeout=10,
         )
         # logger.debug(ret.text)
         report_fail(ret.status_code != 200)
     except Exception as e:
         # logger.debug("data report fail with https")
         try:
             ret = requests.post(
-                url=f"http://{REPORT_DOMAIN}/{REPORT_PATH}/{cmd}",
-                data=json.dumps(data),
+                url=f"http://{REPORT_DOMAIN}/{REPORT_PATH}/{data.cmd}",
+                data=data.dumps(),
                 timeout=10,
             )
             # logger.debug(ret.text)
             report_fail(ret.status_code != 200)
         except Exception as e:
             # logger.error("data report fail with http, give up")
             # logger.exception(e)
@@ -98,72 +135,59 @@
 lock = threading.Condition()
 report_queue = queue.Queue()
 thread = threading.Thread(target=process_report)
 thread.setDaemon(True)
 thread.start()
 
 usage = []
-app_id = None
-version = build_version().get("version")
-revision = build_version().get("revision")
 
+REPORT_THRESHOLD = 10000  # 上报阈值
 
 def minium_log(func):
     """
     函数统计装饰器
     :param func:
     :return:
     """
 
     @wraps(func)
     def wrapper(*args, **kwargs):
-        global usage, app_id, version, revision
+        global usage, app_id
 
         start = datetime.datetime.now()
-        result = func(*args, **kwargs)
+        self = args[0]
+        func_name = f"{self.__class__.__name__}.{func.__name__}"
+        try:
+            result = func(*args, **kwargs)
+        except MiniError as me:
+            report_exception(ExceptionData(me, func=func_name))
+            raise
         end = datetime.datetime.now()
-
-        new_args = [args[0].__dict__] + list(args[1:])
-
-        if (version is None or revision is None) and hasattr(args[0], "version"):
-            version = args[0].version.get("version")
-            revision = args[0].version.get("revision")
-
-        if app_id is None and hasattr(args[0], "app_id"):
-            app_id = args[0].app_id
+        consuming = int((end - start).total_seconds() * 1000)
+        if app_id is None and hasattr(self, "app_id"):
+            app_id = self.app_id
+        if consuming < REPORT_THRESHOLD:
+            return result
+        new_args = list(args[1:])
+        
+        consum_data = ConsumeData({
+            "func": func_name,
+            "args": str(new_args),
+            "kwargs": kwargs,
+            "consuming": consuming
+        })
 
         if app_id is None:
-            usage.append(
-                {
-                    "version": version,
-                    "revision": revision,
-                    "app_id": app_id,
-                    "func": func.__name__,
-                    "args": str(new_args),
-                    "kwargs": kwargs,
-                    "time": datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
-                    "consuming": int((end - start).total_seconds() * 1000),
-                }
-            )
+            usage.append(consum_data)
         else:
-            report_queue.put(
-                {
-                    "version": version,
-                    "revision": revision,
-                    "app_id": app_id,
-                    "func": func.__name__,
-                    "args": str(new_args),
-                    "kwargs": kwargs,
-                    "time": datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
-                    "consuming": int((end - start).total_seconds() * 1000),
-                }
-            )
+            report_queue.put(consum_data)
             for f in usage:
                 f["app_id"] = app_id
                 report_queue.put(f)
+            usage.clear()
             lock.acquire()
             lock.notify()
             lock.release()
         return result
 
     return wrapper
 
@@ -182,8 +206,7 @@
                 and not k.startswith("register")
                 and not k.startswith("notify")
                 and not k.startswith("remove")
             ):
                 attr_dict[k] = minium_log(v)
         return type.__new__(mcs, cls_name, bases, attr_dict)
 
-
```

### Comparing `minium-1.4.0/minium/miniprogram/base_driver/minium_object.py` & `minium-1.4.1/minium/miniprogram/base_driver/minium_object.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/miniprogram/base_driver/page.py` & `minium-1.4.1/minium/miniprogram/base_driver/page.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/miniprogram/base_driver/prefixer.py` & `minium-1.4.1/minium/miniprogram/base_driver/prefixer.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/miniprogram/base_driver/version.py` & `minium-1.4.1/minium/miniprogram/base_driver/version.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/miniprogram/qq_minium.py` & `minium-1.4.1/minium/miniprogram/qq_minium.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/miniprogram/wx_minium.py` & `minium-1.4.1/minium/miniprogram/wx_minium.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 import platform
 import os
 import base64
 import json
 import re
 import threading
+import time
 from websocket import WebSocketConnectionClosedException
 
 from minium.utils.injectjs import getInjectJsCode, setInjectJsMode
 from .base_driver.version import build_version
 from .base_driver.minium import BaseMinium
 from .base_driver.app import App
 from .base_driver.connection import Connection
```

### Comparing `minium-1.4.0/minium/native/__init__.py` & `minium-1.4.1/minium/native/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/android_base/__init__.py` & `minium-1.4.1/minium/native/lib/android_base/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/__init__.py` & `minium-1.4.1/minium/native/lib/at/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/apkapi.py` & `minium-1.4.1/minium/native/lib/at/apkapi.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/atproxy.py` & `minium-1.4.1/minium/native/lib/at/atproxy.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/bin/AtServer.apk` & `minium-1.4.1/minium/native/lib/at/bin/AtServer.apk`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/bin/AtStub.jar` & `minium-1.4.1/minium/native/lib/at/bin/AtStub.jar`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/command_line.py` & `minium-1.4.1/minium/native/lib/at/command_line.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/core/accesshelper.py` & `minium-1.4.1/minium/native/lib/at/core/accesshelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/core/adbwrap.py` & `minium-1.4.1/minium/native/lib/at/core/adbwrap.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/core/basedriver.py` & `minium-1.4.1/minium/native/lib/at/core/basedriver.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/core/case_repair_adapter.py` & `minium-1.4.1/minium/native/lib/at/core/case_repair_adapter.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/core/config.py` & `minium-1.4.1/minium/native/lib/at/core/config.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/core/element.py` & `minium-1.4.1/minium/native/lib/at/core/element.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/core/exceptions.py` & `minium-1.4.1/minium/native/lib/at/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/core/javadriver.py` & `minium-1.4.1/minium/native/lib/at/core/javadriver.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/core/resguard.py` & `minium-1.4.1/minium/native/lib/at/core/resguard.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/core/stf/mincap.py` & `minium-1.4.1/minium/native/lib/at/core/stf/mincap.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/core/stf/minitouch.py` & `minium-1.4.1/minium/native/lib/at/core/stf/minitouch.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/core/uidevice.py` & `minium-1.4.1/minium/native/lib/at/core/uidevice.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/core/uixml.py` & `minium-1.4.1/minium/native/lib/at/core/uixml.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/core/websocketcli.py` & `minium-1.4.1/minium/native/lib/at/core/websocketcli.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/eventmonitor.py` & `minium-1.4.1/minium/native/lib/at/eventmonitor.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/hook.py` & `minium-1.4.1/minium/native/lib/at/hook.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/jlogcat.py` & `minium-1.4.1/minium/native/lib/at/jlogcat.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/keycode.py` & `minium-1.4.1/minium/native/lib/at/keycode.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/perfcollector.py` & `minium-1.4.1/minium/native/lib/at/perfcollector.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/tests/AtEvent.py` & `minium-1.4.1/minium/native/lib/at/tests/AtEvent.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/tests/atdevicetest.py` & `minium-1.4.1/minium/native/lib/at/tests/atdevicetest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/tests/drivertest.py` & `minium-1.4.1/minium/native/lib/at/tests/drivertest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/tests/elementtest.py` & `minium-1.4.1/minium/native/lib/at/tests/elementtest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/tests/images/1.jpg` & `minium-1.4.1/minium/native/lib/at/tests/images/1.jpg`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/tests/images/2.jpg` & `minium-1.4.1/minium/native/lib/at/tests/images/2.jpg`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/tests/images/image.jpg` & `minium-1.4.1/minium/native/lib/at/tests/images/image.jpg`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/tests/minitouch_test.py` & `minium-1.4.1/minium/native/lib/at/tests/minitouch_test.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/tests/u2test.py` & `minium-1.4.1/minium/native/lib/at/tests/u2test.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/tests/uixmltest.py` & `minium-1.4.1/minium/native/lib/at/tests/uixmltest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/tests/webdrivertest.py` & `minium-1.4.1/minium/native/lib/at/tests/webdrivertest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/utils/apkinfo.py` & `minium-1.4.1/minium/native/lib/at/utils/apkinfo.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/utils/axmlparser.py` & `minium-1.4.1/minium/native/lib/at/utils/axmlparser.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/utils/axmlparser3.py` & `minium-1.4.1/minium/native/lib/at/utils/axmlparser3.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/utils/commonhelper.py` & `minium-1.4.1/minium/native/lib/at/utils/commonhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/utils/decorator.py` & `minium-1.4.1/minium/native/lib/at/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/utils/nbsp.py` & `minium-1.4.1/minium/native/lib/at/utils/nbsp.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/utils/threadhelper.py` & `minium-1.4.1/minium/native/lib/at/utils/threadhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/webdriver/driver.py` & `minium-1.4.1/minium/native/lib/at/webdriver/driver.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/webdriver/jsapi.py` & `minium-1.4.1/minium/native/lib/at/webdriver/jsapi.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/webdriver/miniapp.py` & `minium-1.4.1/minium/native/lib/at/webdriver/miniapp.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/webdriver/stub.js` & `minium-1.4.1/minium/native/lib/at/webdriver/stub.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/webdriver/tabdescription.py` & `minium-1.4.1/minium/native/lib/at/webdriver/tabdescription.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/webdriver/tabwebsocket.py` & `minium-1.4.1/minium/native/lib/at/webdriver/tabwebsocket.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/webdriver/webelement.py` & `minium-1.4.1/minium/native/lib/at/webdriver/webelement.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/webdriver/webhelper.py` & `minium-1.4.1/minium/native/lib/at/webdriver/webhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/webdriver/wspools.py` & `minium-1.4.1/minium/native/lib/at/webdriver/wspools.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/at/wechat/activtiy.py` & `minium-1.4.1/minium/native/lib/at/wechat/activtiy.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/case_repair_sdk/__init__.py` & `minium-1.4.1/minium/native/lib/case_repair_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/case_repair_sdk/default_trace.py` & `minium-1.4.1/minium/native/lib/case_repair_sdk/default_trace.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/wda/__init__.py` & `minium-1.4.1/minium/native/lib/wda/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/wda/screenhelper.py` & `minium-1.4.1/minium/native/lib/wda/screenhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/wda/xcui_element_types.py` & `minium-1.4.1/minium/native/lib/wda/xcui_element_types.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/wx_wda/wdaUI.py` & `minium-1.4.1/minium/native/lib/wx_wda/wdaUI.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/lib/wx_wda/webDriverTool.py` & `minium-1.4.1/minium/native/lib/wx_wda/webDriverTool.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/qq_native/qandroidnative.py` & `minium-1.4.1/minium/native/qq_native/qandroidnative.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/qq_native/qbasenative.py` & `minium-1.4.1/minium/native/qq_native/qbasenative.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/qq_native/qiosnative.py` & `minium-1.4.1/minium/native/qq_native/qiosnative.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/wx_native/androidnative.py` & `minium-1.4.1/minium/native/wx_native/androidnative.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/wx_native/basenative.py` & `minium-1.4.1/minium/native/wx_native/basenative.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/wx_native/idenative.py` & `minium-1.4.1/minium/native/wx_native/idenative.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/wx_native/iosnative.py` & `minium-1.4.1/minium/native/wx_native/iosnative.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/native/wx_native/wording.py` & `minium-1.4.1/minium/native/wx_native/wording.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/emitter.py` & `minium-1.4.1/minium/utils/emitter.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/injectjs.py` & `minium-1.4.1/minium/utils/injectjs.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/es5/createContext.js` & `minium-1.4.1/minium/utils/js/es5/createContext.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/es5/helpers.js` & `minium-1.4.1/minium/utils/js/es5/helpers.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/es5/hookWxMethod.js` & `minium-1.4.1/minium/utils/js/es5/hookWxMethod.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/es5/ideMockChooseLocation.js` & `minium-1.4.1/minium/utils/js/es5/ideMockChooseLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/es5/ideMockGetLocation.js` & `minium-1.4.1/minium/utils/js/es5/ideMockGetLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/es5/ideMockGetWeRunData.js` & `minium-1.4.1/minium/utils/js/es5/ideMockGetWeRunData.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/es5/ideMockModal.js` & `minium-1.4.1/minium/utils/js/es5/ideMockModal.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/es5/mockChooseImage.js` & `minium-1.4.1/minium/utils/js/es5/mockChooseImage.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/es5/mockCloudCall.js` & `minium-1.4.1/minium/utils/js/es5/mockCloudCall.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -15,15 +15,15 @@
                                 if (!a(b[e], c[e])) return !1;
                             return !0
                         }
                         for (var f in b)
                             if ("success" != f && "fail" != f && "complete" != f && "_miniMockType" != f) {
                                 if (void 0 === c[f]) return !1;
                                 if (!a(b[f], c[f])) return !1
-                            } return !0;
+                            } return !0
                 }
                 return !1
             },
             b = function(b) {
                 return function(d) {
                     if (!global["__minium_".concat(b, "_mock_rule")]) return c[b].call(this, d);
                     for (var e, f = 0; f < global["__minium_".concat(b, "_mock_rule")].length; f++)
```

### Comparing `minium-1.4.0/minium/utils/js/es5/mockNetwork.js` & `minium-1.4.1/minium/utils/js/es5/mockNetwork.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -15,15 +15,15 @@
                             if (!a(b[e], c[e])) return !1;
                         return !0
                     }
                     for (var f in b)
                         if ("success" != f && "fail" != f && "complete" != f && "_miniMockType" != f) {
                             if (void 0 === c[f]) return !1;
                             if (!a(b[f], c[f])) return !1
-                        } return !0;
+                        } return !0
             }
             return !1
         };
         Object.defineProperty(global, "__minium_%(interface)s_network_mocked", {
             value: !0,
             writable: !1
         }), global["__minium_%(interface)s_network_mock_rule"] || (global["__minium_%(interface)s_network_mock_rule"] = []), global["__minium_%(interface)sTask"] = function() {
```

### Comparing `minium-1.4.0/minium/utils/js/es5/mockRequestStack.js` & `minium-1.4.1/minium/utils/js/es5/mockRequestStack.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/es5/networkPannel.js` & `minium-1.4.1/minium/utils/js/es5/networkPannel.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/es5/requestStack.js` & `minium-1.4.1/minium/utils/js/es5/requestStack.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/es5/testAsync.js` & `minium-1.4.1/minium/utils/js/es5/testAsync.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -319,12 +319,12 @@
             for (; 1;) switch (a.prev = a.next) {
                 case 0:
                     return global.babelHelpers["typeof"](1), a.abrupt("return", new Promise(function(a) {
                         return setTimeout(a, 1e3)
                     }));
                 case 2:
                 case "end":
-                    return a.stop();
+                    return a.stop()
             }
         }, a)
     })), _testAsync.apply(this, arguments)
 }
```

### Comparing `minium-1.4.0/minium/utils/js/min/helpers.js` & `minium-1.4.1/minium/utils/js/min/helpers.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/min/hookWxMethod.js` & `minium-1.4.1/minium/utils/js/min/hookWxMethod.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/min/ideMockChooseLocation.js` & `minium-1.4.1/minium/utils/js/min/ideMockChooseLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/min/ideMockGetLocation.js` & `minium-1.4.1/minium/utils/js/min/ideMockGetLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/min/ideMockGetWeRunData.js` & `minium-1.4.1/minium/utils/js/min/ideMockGetWeRunData.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/min/ideMockModal.js` & `minium-1.4.1/minium/utils/js/min/ideMockModal.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/min/mockChooseImage.js` & `minium-1.4.1/minium/utils/js/min/mockChooseImage.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/min/mockCloudCall.js` & `minium-1.4.1/minium/utils/js/min/mockCloudCall.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/min/mockNetwork.js` & `minium-1.4.1/minium/utils/js/min/mockNetwork.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/min/mockRequestStack.js` & `minium-1.4.1/minium/utils/js/min/mockRequestStack.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/min/networkPannel.js` & `minium-1.4.1/minium/utils/js/min/networkPannel.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/js/min/requestStack.js` & `minium-1.4.1/minium/utils/js/min/requestStack.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/meta.py` & `minium-1.4.1/minium/utils/meta.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.0/minium/utils/utils.py` & `minium-1.4.1/minium/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,25 @@
 import os
 import asyncio
 import functools
 import concurrent.futures
 import json
 import socket
 
+try:
+    import urllib
+    urlencode = urllib.urlencode
+except AttributeError:
+    from urllib.parse import urlencode
+except ImportError:
+    try:
+        from urllib3.request import urlencode
+    except ModuleNotFoundError:  # 2.0.2 后改了
+        raise RuntimeError("maybe you should install urllib3<2.0")
+
 logger = logging.getLogger("minium")
 
 
 def timeout(duration, interval=1):
     """
     重试超时装饰器,在超时之前会每隔{interval}秒重试一次
     注意：被修饰的函数必须要有非空返回,这是重试终止的条件！！！
```

### Comparing `minium-1.4.0/minium.egg-info/PKG-INFO` & `minium-1.4.1/minium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minium
-Version: 1.4.0
+Version: 1.4.1
 Summary: Minium is the best MiniProgram auto test framework.
 Home-page: https://minitest.weixin.qq.com/#/
 Author: WeChat-Test
 Author-email: minitest@tencent.com
 License: MIT
 Description: 
         install:
```

### Comparing `minium-1.4.0/minium.egg-info/SOURCES.txt` & `minium-1.4.1/minium.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,15 @@
 minium/utils/js/es5/checkInject.js
 minium/utils/js/es5/cleanCloudCallMockRule.js
 minium/utils/js/es5/cleanNetworkMockRule.js
 minium/utils/js/es5/createContext.js
 minium/utils/js/es5/editEditorText.js
 minium/utils/js/es5/evalMockChooseImage.js
 minium/utils/js/es5/getAppConfig.js
+minium/utils/js/es5/getUni.js
 minium/utils/js/es5/helpers.js
 minium/utils/js/es5/hookCurrentPageMethod.js
 minium/utils/js/es5/hookWxMethod.js
 minium/utils/js/es5/ideHandleAuthModal.js
 minium/utils/js/es5/ideHandleMap.js
 minium/utils/js/es5/ideHandleModal.js
 minium/utils/js/es5/ideMockAuth.js
@@ -205,14 +206,15 @@
 minium/utils/js/min/checkInject.js
 minium/utils/js/min/cleanCloudCallMockRule.js
 minium/utils/js/min/cleanNetworkMockRule.js
 minium/utils/js/min/createContext.js
 minium/utils/js/min/editEditorText.js
 minium/utils/js/min/evalMockChooseImage.js
 minium/utils/js/min/getAppConfig.js
+minium/utils/js/min/getUni.js
 minium/utils/js/min/helpers.js
 minium/utils/js/min/hookCurrentPageMethod.js
 minium/utils/js/min/hookWxMethod.js
 minium/utils/js/min/ideHandleAuthModal.js
 minium/utils/js/min/ideHandleMap.js
 minium/utils/js/min/ideHandleModal.js
 minium/utils/js/min/ideMockAuth.js
```

### Comparing `minium-1.4.0/setup.py` & `minium-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 import sys
 
-__version__ = "1.4.0"
+__version__ = "1.4.1"
 
 from setuptools import setup, find_packages
 
 # We do not support Python <3.8
 if sys.version_info < (3, 8):
     print(
         "Unfortunately, your python version is not supported!\n"
```

