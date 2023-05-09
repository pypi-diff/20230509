# Comparing `tmp/crosscompute-0.9.4.3.tar.gz` & `tmp/crosscompute-0.9.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosscompute-0.9.4.3.tar", last modified: Sat Apr 29 00:54:00 2023, max compression
+gzip compressed data, was "crosscompute-0.9.4.4.tar", last modified: Tue May  9 13:27:43 2023, max compression
```

## Comparing `crosscompute-0.9.4.3.tar` & `crosscompute-0.9.4.4.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.707458 crosscompute-0.9.4.3/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/LICENSE.md
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4987 2023-04-29 00:54:00.707458 crosscompute-0.9.4.3/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3703 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/README.md
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.695458 crosscompute-0.9.4.3/crosscompute/
--rw-r--r--   0 rhh       (1000) rhh       (1000)       22 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/crosscompute/__init__.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)       38 2022-01-21 18:22:22.000000 crosscompute-0.9.4.3/crosscompute/__main__.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.701458 crosscompute-0.9.4.3/crosscompute/assets/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1292 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/automation.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      910 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/base.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      230 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/button-panel.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      183 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/checkbox-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      579 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/checkbox-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      628 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/checkbox-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      109 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/checkbox-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)    13385 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/configuration.yml
--rw-r--r--   0 rhh       (1000) rhh       (1000)      224 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/default.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)       48 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/embedded.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)    22382 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/favicon.ico
--rw-r--r--   0 rhh       (1000) rhh       (1000)      765 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/file-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      165 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/file-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/file-input.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      631 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/flex.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)      180 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/frame-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/frame-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/image-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/image-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      156 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/json-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-02-28 18:19:08.000000 crosscompute-0.9.4.3/crosscompute/assets/json-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      149 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/link-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/link-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2566 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/crosscompute/assets/live.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      301 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/markdown-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      142 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/markdown-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/pdf-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      137 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/crosscompute/assets/pdf-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)       64 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/pdf.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)       53 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/printed.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)       96 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/radio-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      575 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/radio-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      594 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/radio-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/radio-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      366 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/root.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3271 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/step-body.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      874 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/step.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)       65 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/string-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      432 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/string-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      369 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/string-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      122 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/string-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1095 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/table-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/table-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      159 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/text-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/text-input.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      109 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/assets/text-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/assets/text-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2886 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/constants.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     5072 2023-03-30 19:34:16.000000 crosscompute-0.9.4.3/crosscompute/dependencies.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1055 2022-12-12 19:44:41.000000 crosscompute-0.9.4.3/crosscompute/exceptions.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.702458 crosscompute-0.9.4.3/crosscompute/macros/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-01-21 18:22:22.000000 crosscompute-0.9.4.3/crosscompute/macros/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      717 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/macros/disk.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1530 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/macros/iterable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1088 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/macros/log.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      597 2022-03-14 16:37:10.000000 crosscompute-0.9.4.3/crosscompute/macros/package.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1349 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/macros/security.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.703458 crosscompute-0.9.4.3/crosscompute/routers/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/routers/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     7021 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routers/automation.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1142 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routers/file.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3286 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/crosscompute/routers/root.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1240 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/crosscompute/routers/stream.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      523 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/routers/token.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.705458 crosscompute-0.9.4.3/crosscompute/routines/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-01-21 18:22:22.000000 crosscompute-0.9.4.3/crosscompute/routines/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3195 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routines/asset.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3457 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/routines/authorization.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4877 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routines/automation.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3537 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/routines/batch.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)    41926 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routines/configuration.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     9409 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routines/database.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      914 2022-07-01 15:18:27.000000 crosscompute-0.9.4.3/crosscompute/routines/interface.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1404 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/crosscompute/routines/log.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1523 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/crosscompute/routines/mutation.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     6222 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routines/printer.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     6967 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routines/server.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     7181 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routines/step.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      605 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/crosscompute/routines/uri.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)    30285 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/routines/variable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)    28209 2023-04-29 00:50:49.000000 crosscompute-0.9.4.3/crosscompute/routines/work.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.706458 crosscompute-0.9.4.3/crosscompute/scripts/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-01-21 18:22:22.000000 crosscompute-0.9.4.3/crosscompute/scripts/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3866 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/scripts/configure.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3829 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/crosscompute/scripts/launch.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1123 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/scripts/print.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1721 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/scripts/run.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     4065 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/scripts/serve.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1338 2023-04-27 21:48:39.000000 crosscompute-0.9.4.3/crosscompute/settings.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.696458 crosscompute-0.9.4.3/crosscompute.egg-info/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)     4987 2023-04-29 00:54:00.000000 crosscompute-0.9.4.3/crosscompute.egg-info/PKG-INFO
--rw-rw-r--   0 rhh       (1000) rhh       (1000)     3437 2023-04-29 00:54:00.000000 crosscompute-0.9.4.3/crosscompute.egg-info/SOURCES.txt
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        1 2023-04-29 00:54:00.000000 crosscompute-0.9.4.3/crosscompute.egg-info/dependency_links.txt
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      831 2023-04-29 00:54:00.000000 crosscompute-0.9.4.3/crosscompute.egg-info/entry_points.txt
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      436 2023-04-29 00:54:00.000000 crosscompute-0.9.4.3/crosscompute.egg-info/requires.txt
--rw-rw-r--   0 rhh       (1000) rhh       (1000)       13 2023-04-29 00:54:00.000000 crosscompute-0.9.4.3/crosscompute.egg-info/top_level.txt
--rw-rw-r--   0 rhh       (1000) rhh       (1000)        1 2022-01-21 22:12:56.000000 crosscompute-0.9.4.3/crosscompute.egg-info/zip-safe
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3273 2023-04-29 00:54:00.708458 crosscompute-0.9.4.3/setup.cfg
--rw-rw-r--   0 rhh       (1000) rhh       (1000)       39 2022-01-21 18:22:22.000000 crosscompute-0.9.4.3/setup.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-29 00:54:00.707458 crosscompute-0.9.4.3/tests/
--rw-rw-r--   0 rhh       (1000) rhh       (1000)      168 2022-01-21 18:22:22.000000 crosscompute-0.9.4.3/tests/test_macros_iterable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      428 2023-02-28 18:19:03.000000 crosscompute-0.9.4.3/tests/test_macros_security.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     3759 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/tests/test_routines_configuration.py
--rw-rw-r--   0 rhh       (1000) rhh       (1000)     2285 2022-05-17 17:13:01.000000 crosscompute-0.9.4.3/tests/test_routines_variable.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      656 2023-04-27 21:47:32.000000 crosscompute-0.9.4.3/tests/test_routines_work.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.789167 crosscompute-0.9.4.4/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/LICENSE.md
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4968 2023-05-09 13:27:43.789167 crosscompute-0.9.4.4/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3704 2023-05-04 11:08:59.000000 crosscompute-0.9.4.4/README.md
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.769167 crosscompute-0.9.4.4/crosscompute/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       22 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/__init__.py
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)       38 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/crosscompute/__main__.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.781167 crosscompute-0.9.4.4/crosscompute/assets/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1292 2023-04-26 18:11:29.000000 crosscompute-0.9.4.4/crosscompute/assets/automation.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      910 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/base.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      230 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/button-panel.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      183 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/checkbox-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      579 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/checkbox-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      628 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/checkbox-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      109 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/checkbox-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    13520 2023-05-04 11:08:59.000000 crosscompute-0.9.4.4/crosscompute/assets/configuration.yml
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      224 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/default.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       48 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/embedded.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    22382 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/favicon.ico
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      765 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/file-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      165 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/file-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/file-input.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      737 2023-05-09 05:18:59.000000 crosscompute-0.9.4.4/crosscompute/assets/flex.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      180 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/frame-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/frame-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/image-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/image-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      156 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/json-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-04-25 22:48:18.000000 crosscompute-0.9.4.4/crosscompute/assets/json-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      149 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/link-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/link-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2566 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/live.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      301 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/markdown-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      142 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/markdown-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/pdf-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      137 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/pdf-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       64 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/pdf.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       53 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/printed.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       96 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/radio-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      575 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/radio-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      594 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/radio-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      106 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/radio-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      366 2023-05-04 11:08:59.000000 crosscompute-0.9.4.4/crosscompute/assets/root.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3271 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/step-body.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      874 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/step.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       65 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/string-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      432 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/string-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      369 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/string-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      122 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/string-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1095 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/table-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      139 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/table-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      159 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/text-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      136 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/text-input.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      109 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/assets/text-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/assets/text-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2886 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/constants.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     5072 2023-04-01 20:58:16.000000 crosscompute-0.9.4.4/crosscompute/dependencies.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1055 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/exceptions.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.782167 crosscompute-0.9.4.4/crosscompute/macros/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/crosscompute/macros/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      717 2023-04-05 23:51:33.000000 crosscompute-0.9.4.4/crosscompute/macros/disk.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1530 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/macros/iterable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1088 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/macros/log.py
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)      597 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/crosscompute/macros/package.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1349 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/macros/security.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.783167 crosscompute-0.9.4.4/crosscompute/routers/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/routers/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     7021 2023-04-26 18:11:29.000000 crosscompute-0.9.4.4/crosscompute/routers/automation.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1142 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/routers/file.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3286 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/routers/root.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1240 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/routers/stream.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      523 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/routers/token.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.786167 crosscompute-0.9.4.4/crosscompute/routines/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/crosscompute/routines/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3195 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/routines/asset.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3457 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/routines/authorization.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4806 2023-05-09 05:09:01.000000 crosscompute-0.9.4.4/crosscompute/routines/automation.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3537 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/routines/batch.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    42419 2023-05-09 12:59:04.000000 crosscompute-0.9.4.4/crosscompute/routines/configuration.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     9409 2023-05-04 11:08:59.000000 crosscompute-0.9.4.4/crosscompute/routines/database.py
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)      914 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/crosscompute/routines/interface.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1404 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/crosscompute/routines/log.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1523 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/routines/mutation.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     6222 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/routines/printer.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     6803 2023-05-09 05:01:53.000000 crosscompute-0.9.4.4/crosscompute/routines/server.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     7390 2023-05-09 05:11:33.000000 crosscompute-0.9.4.4/crosscompute/routines/step.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      605 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/routines/uri.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    30285 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/routines/variable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)    28399 2023-05-09 13:25:17.000000 crosscompute-0.9.4.4/crosscompute/routines/work.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.787167 crosscompute-0.9.4.4/crosscompute/scripts/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)        0 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/crosscompute/scripts/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3866 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/scripts/configure.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3829 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/scripts/launch.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1123 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/scripts/print.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1721 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/scripts/run.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4065 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/crosscompute/scripts/serve.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1315 2023-05-09 05:07:31.000000 crosscompute-0.9.4.4/crosscompute/settings.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.770166 crosscompute-0.9.4.4/crosscompute.egg-info/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     4968 2023-05-09 13:27:43.000000 crosscompute-0.9.4.4/crosscompute.egg-info/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3437 2023-05-09 13:27:43.000000 crosscompute-0.9.4.4/crosscompute.egg-info/SOURCES.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-09 13:27:43.000000 crosscompute-0.9.4.4/crosscompute.egg-info/dependency_links.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      831 2023-05-09 13:27:43.000000 crosscompute-0.9.4.4/crosscompute.egg-info/entry_points.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      436 2023-05-09 13:27:43.000000 crosscompute-0.9.4.4/crosscompute.egg-info/requires.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       13 2023-05-09 13:27:43.000000 crosscompute-0.9.4.4/crosscompute.egg-info/top_level.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2022-08-22 13:00:05.000000 crosscompute-0.9.4.4/crosscompute.egg-info/zip-safe
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3253 2023-05-09 13:27:43.790167 crosscompute-0.9.4.4/setup.cfg
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)       39 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/setup.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-09 13:27:43.788167 crosscompute-0.9.4.4/tests/
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)      168 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/tests/test_macros_iterable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      428 2023-02-18 06:45:42.000000 crosscompute-0.9.4.4/tests/test_macros_security.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     3759 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/tests/test_routines_configuration.py
+-rw-rw-r--   0 rhh       (1000) rhh       (1000)     2285 2022-08-15 04:38:47.000000 crosscompute-0.9.4.4/tests/test_routines_variable.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      656 2023-04-25 22:48:21.000000 crosscompute-0.9.4.4/tests/test_routines_work.py
```

### Comparing `crosscompute-0.9.4.3/LICENSE.md` & `crosscompute-0.9.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/PKG-INFO` & `crosscompute-0.9.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: crosscompute
-Version: 0.9.4.3
+Version: 0.9.4.4
 Summary: Automate your Jupyter notebooks and scripts as tools, reports, dashboards.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute/issues
-Project-URL: Documentation, https://github.com/crosscompute/crosscompute-docs
+Project-URL: Documentation, https://docs.crosscompute.com
 Project-URL: Source Code, https://github.com/crosscompute/crosscompute
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -79,14 +79,15 @@
 crosscompute
 
 # Serve automation
 crosscompute automate.yml
 ```
 
 Here are some tutorials and examples:
+
 - [Examples](https://crosscompute.net) [[source](https://github.com/crosscompute/crosscompute-examples)]
 - [Documentation](https://docs.crosscompute.com) [[source](https://github.com/crosscompute/crosscompute-docs)]
 - [Forum](https://forum.crosscompute.com)
 
 ## Development
 
 ```bash
```

### Comparing `crosscompute-0.9.4.3/README.md` & `crosscompute-0.9.4.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 crosscompute
 
 # Serve automation
 crosscompute automate.yml
 ```
 
 Here are some tutorials and examples:
+
 - [Examples](https://crosscompute.net) [[source](https://github.com/crosscompute/crosscompute-examples)]
 - [Documentation](https://docs.crosscompute.com) [[source](https://github.com/crosscompute/crosscompute-docs)]
 - [Forum](https://forum.crosscompute.com)
 
 ## Development
 
 ```bash
```

### Comparing `crosscompute-0.9.4.3/crosscompute/assets/automation.html` & `crosscompute-0.9.4.4/crosscompute/assets/automation.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/assets/base.html` & `crosscompute-0.9.4.4/crosscompute/assets/base.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/assets/checkbox-input.html` & `crosscompute-0.9.4.4/crosscompute/assets/checkbox-input.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/assets/checkbox-output-header.js` & `crosscompute-0.9.4.4/crosscompute/assets/checkbox-output-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/assets/configuration.yml` & `crosscompute-0.9.4.4/crosscompute/assets/configuration.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
-# Reference: https://github.com/crosscompute/crosscompute-examples
-# Gallery: https://crosscompute.net
+# Examples: https://github.com/crosscompute/crosscompute-examples
 # Documentation: https://docs.crosscompute.com
 # Forum: https://forum.crosscompute.com
+# Gallery: https://crosscompute.net
 
 # crosscompute version determines how this file is interpreted (required)
 crosscompute: 0.0.0
 
 # name summarizes what your automation does
 name: Automation X
 
@@ -205,14 +205,20 @@
           color: '#808080'
           padding: 0.1in 0.25in
           skip-first: true
         page-number:
           location: footer
           alignment: right
         name: '{y2 | slug}-{y3}.pdf'
+    - id: report-uri
+      view: link
+      path: report.pdf
+      label: Report URI
+      configuration:
+        path: report-uri.json
 
 # batches are pre-defined runs with specific values set for each input variable
 batches:
 
   # case 0:
   # folder sets values for input variables;
   # folder contains an input subfolder;
```

### Comparing `crosscompute-0.9.4.3/crosscompute/assets/favicon.ico` & `crosscompute-0.9.4.4/crosscompute/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/assets/file-input-header.js` & `crosscompute-0.9.4.4/crosscompute/assets/file-input-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/assets/flex.css` & `crosscompute-0.9.4.4/crosscompute/assets/flex.css`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     font-size: large;
     flex-grow: 1;
   }
   button:hover {
     cursor: pointer;
   }
   ._panel {
-    display: flex;
     flex-direction: row;
     gap: 16px;
   }
   ._continue {
     background: #17A2F5;
     color: white;
     font-weight: bold;
@@ -35,8 +34,18 @@
   ._template > * {
     margin: 0;
   }
   ._view img {
     align-self: start;
     max-width: 100%;
   }
+  @media screen {
+    ._panel {
+      display: flex;
+    }
+  }
+  @media print {
+    ._panel {
+      display: none;
+    }
+  }
 }
```

### Comparing `crosscompute-0.9.4.3/crosscompute/assets/live.html` & `crosscompute-0.9.4.4/crosscompute/assets/live.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/assets/radio-input.html` & `crosscompute-0.9.4.4/crosscompute/assets/radio-input.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/assets/radio-output-header.js` & `crosscompute-0.9.4.4/crosscompute/assets/radio-output-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/assets/step-body.js` & `crosscompute-0.9.4.4/crosscompute/assets/step-body.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/assets/step.html` & `crosscompute-0.9.4.4/crosscompute/assets/step.html`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/assets/table-output-header.js` & `crosscompute-0.9.4.4/crosscompute/assets/table-output-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/constants.py` & `crosscompute-0.9.4.4/crosscompute/constants.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/dependencies.py` & `crosscompute-0.9.4.4/crosscompute/dependencies.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/exceptions.py` & `crosscompute-0.9.4.4/crosscompute/exceptions.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/macros/disk.py` & `crosscompute-0.9.4.4/crosscompute/macros/disk.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/macros/iterable.py` & `crosscompute-0.9.4.4/crosscompute/macros/iterable.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/macros/log.py` & `crosscompute-0.9.4.4/crosscompute/macros/log.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/macros/package.py` & `crosscompute-0.9.4.4/crosscompute/macros/package.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/macros/security.py` & `crosscompute-0.9.4.4/crosscompute/macros/security.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/routers/automation.py` & `crosscompute-0.9.4.4/crosscompute/routers/automation.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/routers/file.py` & `crosscompute-0.9.4.4/crosscompute/routers/file.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/routers/root.py` & `crosscompute-0.9.4.4/crosscompute/routers/root.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/routers/stream.py` & `crosscompute-0.9.4.4/crosscompute/routers/stream.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/routers/token.py` & `crosscompute-0.9.4.4/crosscompute/routers/token.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/routines/asset.py` & `crosscompute-0.9.4.4/crosscompute/routines/asset.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/routines/authorization.py` & `crosscompute-0.9.4.4/crosscompute/routines/authorization.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/routines/automation.py` & `crosscompute-0.9.4.4/crosscompute/routines/automation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # TODO: Return unvalidated configuration when there is an exception
 # TODO: Watch multiple folders if not all under parent folder
-from concurrent.futures import (
-    ThreadPoolExecutor, as_completed)
 from logging import getLogger
 from pathlib import Path
 
 from invisibleroads_macros_web.port import find_open_port
 
 from ..constants import (
     AUTOMATION_PATH,
```

### Comparing `crosscompute-0.9.4.3/crosscompute/routines/batch.py` & `crosscompute-0.9.4.4/crosscompute/routines/batch.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/routines/configuration.py` & `crosscompute-0.9.4.4/crosscompute/routines/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # TODO: Save to ini, toml
 import json
 import shutil
-from collections import Counter
+from collections import Counter, defaultdict
 from configparser import ConfigParser
 from datetime import datetime, timedelta
 from logging import getLogger
 from os import environ
 from os.path import basename, relpath, splitext
 from pathlib import Path
 from string import Template
@@ -494,30 +494,31 @@
     assert_unique_values([
         _.uri for _ in batch_definitions], 'duplicate batch uri {x}')
     return {'batch_definitions': batch_definitions}
 
 
 def validate_environment(configuration):
     d = get_dictionary(configuration, 'environment')
+    package_ids_by_manager_name = get_package_ids_by_manager_name(
+        get_dictionaries(d, 'packages'))
     port_definitions = get_port_definitions(
         d, configuration.get_variable_definitions('log')
         + configuration.get_variable_definitions('debug'))
     environment_variable_ids = get_environment_variable_ids(get_dictionaries(
         d, 'variables'))
     batch_concurrency_name = d.get('batch', 'thread').lower()
     if batch_concurrency_name not in ('process', 'thread', 'single'):
         raise CrossComputeConfigurationError(
             f'"{batch_concurrency_name}" batch concurrency is not supported')
     interval_timedelta, is_interval_strict = get_interval_pack(d.get(
         'interval', '').strip())
     return {
         'engine_name': get_engine_name(d),
         'parent_image_name': d.get('image', 'python').strip(),
-        'package_definitions': [PackageDefinition(_) for _ in get_dictionaries(
-            d, 'packages')],
+        'package_ids_by_manager_name': package_ids_by_manager_name,
         'port_definitions': port_definitions,
         'environment_variable_ids': environment_variable_ids,
         'batch_concurrency_name': batch_concurrency_name,
         'interval_timedelta': interval_timedelta,
         'is_interval_strict': is_interval_strict}
 
 
@@ -938,14 +939,23 @@
             'using engine=unsafe; use engine=podman for untrusted code')
     else:
         raise CrossComputeConfigurationError(
             f'"{engine_name}" engine is not supported')
     return engine_name
 
 
+def get_package_ids_by_manager_name(package_dictionaries):
+    package_ids_by_manager_name = defaultdict(set)
+    package_definitions = [PackageDefinition(_) for _ in package_dictionaries]
+    for package_definition in package_definitions:
+        manager_name = package_definition.manager_name
+        package_ids_by_manager_name[manager_name].add(package_definition.id)
+    return package_ids_by_manager_name
+
+
 def get_port_definitions(environment_dictionary, variable_definitions):
     port_definitions = [PortDefinition(_) for _ in get_dictionaries(
         environment_dictionary, 'ports')]
     for port_definition in port_definitions:
         port_id = port_definition.id
         try:
             variable_definition = find_item(
```

### Comparing `crosscompute-0.9.4.3/crosscompute/routines/database.py` & `crosscompute-0.9.4.4/crosscompute/routines/database.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/routines/interface.py` & `crosscompute-0.9.4.4/crosscompute/routines/interface.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/routines/log.py` & `crosscompute-0.9.4.4/crosscompute/routines/log.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/routines/mutation.py` & `crosscompute-0.9.4.4/crosscompute/routines/mutation.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/routines/printer.py` & `crosscompute-0.9.4.4/crosscompute/routines/printer.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/routines/server.py` & `crosscompute-0.9.4.4/crosscompute/routines/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from fastapi.responses import PlainTextResponse
 from invisibleroads_macros_web.starlette import ExtraResponseHeadersMiddleware
 from starlette.exceptions import HTTPException as StarletteHTTPException
 from watchfiles import watch
 
 from ..constants import (
     Info,
-    BUTTON_TEXT_BY_ID,
     DISK_DEBOUNCE_IN_MILLISECONDS,
     DISK_STEP_IN_MILLISECONDS,
     HOST,
     PORT,
     TEMPLATE_PATH_BY_ID)
 from ..exceptions import (
     CrossComputeError)
@@ -25,15 +24,14 @@
     automation,
     file,
     root,
     stream,
     token)
 from ..settings import (
     StoppableProcess,
-    button_text_by_id,
     site,
     template_environment,
     template_globals,
     template_path_by_id)
 from .database import (
     DiskDatabase,
     PositiveFileFilter)
@@ -159,16 +157,14 @@
             'base_template_path': template_path_by_id['base'],
             'live_template_path': template_path_by_id['live'],
             'google_analytics_id': getenv('GOOGLE_ANALYTICS_ID', ''),
             'server_time': time(),
             'root_uri': self._root_uri,
             'with_restart': self._with_restart})
         template_environment.auto_reload = self._with_restart
-        button_text_by_id.update(BUTTON_TEXT_BY_ID)
-        button_text_by_id.update(configuration.button_text_by_id)
 
 
 def get_app(root_uri, with_prefix):
     prefix = root_uri if with_prefix else ''
     app = FastAPI(root_path='' if with_prefix else root_uri)
     app.add_exception_handler(StarletteHTTPException, handle_http_exception)
     app.include_router(root.router, prefix=prefix)
```

### Comparing `crosscompute-0.9.4.3/crosscompute/routines/step.py` & `crosscompute-0.9.4.4/crosscompute/routines/step.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from html.parser import HTMLParser
 from itertools import count
 from logging import getLogger
 
 from invisibleroads_macros_web.markdown import get_html_from_markdown
 
 from ..constants import (
+    BUTTON_TEXT_BY_ID,
     MUTATION_ROUTE,
     STEP_CODE_BY_NAME,
     STEP_ROUTE,
     VARIABLE_ID_TEMPLATE_PATTERN,
     VARIABLE_ID_WHITELIST_PATTERN)
 from ..macros.iterable import find_item, get_unique_order
-from ..settings import button_text_by_id, template_globals
+from ..settings import template_globals
 from .asset import asset_storage
 from .batch import DiskBatch
 from .variable import Element, VariableView
 
 
 class TemplateFilter(HTMLParser):
 
@@ -74,14 +75,15 @@
     design_name = automation_definition.get_design_name(step_name)
     for_embed = '_embed' in request_params
     for_print = '_print' in request_params
     render_html = partial(
         render_variable_html, variable_definitions=variable_definitions,
         batch=batch, m=m, variable_index=count(),
         root_uri=template_globals['root_uri'], request_params=request_params,
+        button_text_by_id=automation_definition.button_text_by_id,
         step_name=step_name, design_name=design_name, for_print=for_print)
     main_text, template_count = get_main_pack(
         automation_definition, step_name, render_html)
     mutation_reference_uri = get_automation_batch_step_uri(
         automation_definition, batch_definition, step_name)
     return {
         'css_uris': get_unique_order(m['css_uris']),
@@ -93,22 +95,21 @@
         'has_interval': automation_definition.interval_timedelta is not None,
         'is_done': batch.is_done(),
         'mutation_uri': MUTATION_ROUTE.format(uri=mutation_reference_uri)}
 
 
 def render_variable_html(
         match, variable_definitions, batch, m, variable_index, template_index,
-        root_uri, request_params, step_name, design_name, for_print):
+        root_uri, request_params, button_text_by_id, step_name, design_name,
+        for_print):
     matching_inner_text = match.group(1)
     if matching_inner_text == 'ROOT_URI':
         return root_uri
     elif matching_inner_text == 'BUTTON_PANEL':
-        return BUTTON_PANEL_HTML.render({
-            'template_index': template_index,
-            'button_text_by_id': button_text_by_id})
+        return get_button_panel_html(template_index, button_text_by_id)
     terms = matching_inner_text.split('|')
     variable_id = terms[0].strip()
     try:
         variable_definition = find_item(
             variable_definitions, 'id', variable_id)
     except StopIteration:
         L.warning(
@@ -139,24 +140,23 @@
     return '\n'.join(css_texts + get_unique_order(m['css_texts']))
 
 
 def get_main_pack(automation_definition, step_name, render_html):
     a = automation_definition
     template_definitions = a.template_definitions_by_step_name[step_name]
     with_button_panel = step_name == 'input' or len(template_definitions) > 1
+    button_text_by_id = a.button_text_by_id
 
     def format_template(text, i=0, x=''):
         l_ = ' _live' if not i and not x else ''
         x_ = f' data-expression="{x}"' if x else ''
         g = TemplateFilter(render_html, template_index=i).process(text)
         h = get_html_from_markdown(g)
         if with_button_panel and 'class="_continue"' not in h:
-            h += '\n' + BUTTON_PANEL_HTML.render({
-                'template_index': i,
-                'button_text_by_id': button_text_by_id})
+            h += '\n' + get_button_panel_html(i, button_text_by_id)
         return f'<div id="_t{i}" class="_template{l_}"{x_}>\n{h}\n</div>'
 
     if not template_definitions:
         variable_definitions = a.get_variable_definitions(step_name)
         variable_ids = (_.id for _ in variable_definitions)
         text = '\n'.join('{%s}' % _ for _ in variable_ids)
         return format_template(text), 1
@@ -166,14 +166,20 @@
         path = automation_folder / template_definition.path
         with path.open('rt') as f:
             text = f.read().strip()
         parts.append(format_template(text, i, template_definition.expression))
     return '\n'.join(parts), len(template_definitions)
 
 
+def get_button_panel_html(template_index, button_text_by_id):
+    return BUTTON_PANEL_HTML.render({
+        'template_index': template_index,
+        'button_text_by_id': BUTTON_TEXT_BY_ID | button_text_by_id})
+
+
 L = getLogger(__name__)
 
 
 EMBEDDED_CSS = asset_storage.load_raw_text('embedded.css')
 PRINTED_CSS = asset_storage.load_raw_text('printed.css')
 DEFAULT_CSS = asset_storage.load_raw_text('default.css')
 FLEX_CSS = asset_storage.load_raw_text('flex.css')
```

### Comparing `crosscompute-0.9.4.3/crosscompute/routines/uri.py` & `crosscompute-0.9.4.4/crosscompute/routines/uri.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/routines/variable.py` & `crosscompute-0.9.4.4/crosscompute/routines/variable.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/routines/work.py` & `crosscompute-0.9.4.4/crosscompute/routines/work.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # TODO: Consider giving scripts access to CROSSCOMPUTE_ROOT_URI
 import shlex
 import subprocess
-from collections import defaultdict
+from abc import ABC, abstractmethod
 from concurrent.futures import (
     ProcessPoolExecutor, ThreadPoolExecutor, as_completed)
 from contextlib import contextmanager
 from logging import getLogger
 from os import environ, getenv, symlink
 from os.path import relpath
 from random import choice
@@ -48,19 +48,27 @@
     get_variable_data_by_id,
     get_variable_value_by_id,
     process_variable_data,
     save_variable_data,
     update_variable_data)
 
 
-class AbstractEngine():
+class AbstractEngine(ABC):
 
     def __init__(self, with_rebuild=True):
         self.with_rebuild = with_rebuild
 
+    @abstractmethod
+    def prepare(self, automation_definition):
+        pass
+
+    @abstractmethod
+    def run(self, automation_definition, batch_folder, custom_environment):
+        pass
+
     def run_batch(
             self, automation_definition, batch_definition, user_environment):
         reference_time = time()
         batch_folder, batch_environment = prepare_batch(
             automation_definition, batch_definition)
         if not automation_definition.script_definitions:
             return
@@ -87,21 +95,29 @@
         return _process_batch(automation_definition, batch_definition, [
             'output', 'log', 'debug',
         ], {'debug': {
             'source_time': reference_time,
             'execution_time_in_seconds': time() - reference_time,
             'return_code': return_code}})
 
+
+class UnsafeEngine(AbstractEngine):
+
     def prepare(self, automation_definition):
+        # TODO: Consider having a separate venv for each automation
+        d = automation_definition.package_ids_by_manager_name
+        try:
+            for manager_name, package_ids in d.items():
+                subprocess.run([
+                    manager_name, 'install'] + list(package_ids), check=True)
+        except subprocess.CalledProcessError:
+            raise CrossComputeExecutionError()
         for s in automation_definition.script_definitions:
             s.get_command_string()
 
-
-class UnsafeEngine(AbstractEngine):
-
     def run(self, automation_definition, batch_folder, custom_environment):
         step_folder_by_name = _get_step_folder_by_name(
             automation_definition.folder, batch_folder)
         script_definitions = automation_definition.script_definitions
         script_environment = _prepare_script_environment(
             step_folder_by_name, custom_environment, with_path=True)
         debug_folder = step_folder_by_name['debug_folder']
@@ -525,35 +541,32 @@
                 step_folder / 'variables.dictionary', extra_data_by_id)
             variable_data_by_id.update(extra_data_by_id)
     return variable_data_by_id_by_step_name
 
 
 def _prepare_container_file_text(automation_definition):
     path_folders = set()
-    package_ids_by_manager_name = defaultdict(set)
-    for package_definition in automation_definition.package_definitions:
-        manager_name = package_definition.manager_name
-        package_ids_by_manager_name[manager_name].add(package_definition.id)
+    d = automation_definition.package_ids_by_manager_name
     root_package_commands, user_package_commands = [], []
-    if 'apt' in package_ids_by_manager_name:
-        s = ' '.join(sorted(package_ids_by_manager_name['apt']))
+    if 'apt' in d:
+        s = ' '.join(sorted(d['apt']))
         root_package_commands.append(
             f'apt update && apt -y install {s} && apt clean')
-    if 'dnf' in package_ids_by_manager_name:
-        s = ' '.join(sorted(package_ids_by_manager_name['dnf']))
+    if 'dnf' in d:
+        s = ' '.join(sorted(d['dnf']))
         root_package_commands.append(
             f'dnf -y install {s} && dnf clean all')
-    if 'npm' in package_ids_by_manager_name:
-        s = ' '.join(sorted(package_ids_by_manager_name['npm']))
+    if 'npm' in d:
+        s = ' '.join(sorted(d['npm']))
         user_package_commands.append(
             f'npm install {s} --prefix ~/.local -g && '
             f'npm cache clean --force')
         path_folders.add('/home/user/.local/bin')
-    if 'pip' in package_ids_by_manager_name:
-        s = ' '.join(sorted(package_ids_by_manager_name['pip']))
+    if 'pip' in d:
+        s = ' '.join(sorted(d['pip']))
         user_package_commands.append(
             f'pip install {s} --user && '
             f'pip cache purge && rm -rf ~/.cache')
         path_folders.add('/home/user/.local/bin')
     return CONTAINER_FILE_TEXT.render(
         parent_image_name=automation_definition.parent_image_name,
         root_package_commands=root_package_commands,
```

### Comparing `crosscompute-0.9.4.3/crosscompute/scripts/configure.py` & `crosscompute-0.9.4.4/crosscompute/scripts/configure.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/scripts/launch.py` & `crosscompute-0.9.4.4/crosscompute/scripts/launch.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/scripts/print.py` & `crosscompute-0.9.4.4/crosscompute/scripts/print.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/scripts/run.py` & `crosscompute-0.9.4.4/crosscompute/scripts/run.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/scripts/serve.py` & `crosscompute-0.9.4.4/crosscompute/scripts/serve.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute/settings.py` & `crosscompute-0.9.4.4/crosscompute/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,8 +40,7 @@
     'server_time': 0,
     'root_uri': '',
     'with_restart': True}
 TemplateResponse = TemplateResponseFactory(
     template_environment).TemplateResponse
 printer_by_name = {}
 view_by_name = {}
-button_text_by_id = {}
```

### Comparing `crosscompute-0.9.4.3/crosscompute.egg-info/PKG-INFO` & `crosscompute-0.9.4.4/crosscompute.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: crosscompute
-Version: 0.9.4.3
+Version: 0.9.4.4
 Summary: Automate your Jupyter notebooks and scripts as tools, reports, dashboards.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute/issues
-Project-URL: Documentation, https://github.com/crosscompute/crosscompute-docs
+Project-URL: Documentation, https://docs.crosscompute.com
 Project-URL: Source Code, https://github.com/crosscompute/crosscompute
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -79,14 +79,15 @@
 crosscompute
 
 # Serve automation
 crosscompute automate.yml
 ```
 
 Here are some tutorials and examples:
+
 - [Examples](https://crosscompute.net) [[source](https://github.com/crosscompute/crosscompute-examples)]
 - [Documentation](https://docs.crosscompute.com) [[source](https://github.com/crosscompute/crosscompute-docs)]
 - [Forum](https://forum.crosscompute.com)
 
 ## Development
 
 ```bash
```

### Comparing `crosscompute-0.9.4.3/crosscompute.egg-info/SOURCES.txt` & `crosscompute-0.9.4.4/crosscompute.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/crosscompute.egg-info/entry_points.txt` & `crosscompute-0.9.4.4/crosscompute.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/setup.cfg` & `crosscompute-0.9.4.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosscompute
-version = 0.9.4.3
+version = 0.9.4.4
 description = Automate your Jupyter notebooks and scripts as tools, reports, dashboards.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://crosscompute.com
 author = CrossCompute Inc.
 author_email = support@crosscompute.com
 license = MIT
@@ -22,15 +22,15 @@
 	Programming Language :: Python :: 3
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 	Topic :: Internet :: WWW/HTTP :: WSGI
 	Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 	Topic :: Software Development :: Libraries :: Application Frameworks
 project_urls = 
 	Bug Tracker = https://github.com/crosscompute/crosscompute/issues
-	Documentation = https://github.com/crosscompute/crosscompute-docs
+	Documentation = https://docs.crosscompute.com
 	Source Code = https://github.com/crosscompute/crosscompute
 
 [options]
 packages = find:
 python_requires = >=3.10
 install_requires = 
 	fastapi
```

### Comparing `crosscompute-0.9.4.3/tests/test_routines_configuration.py` & `crosscompute-0.9.4.4/tests/test_routines_configuration.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/tests/test_routines_variable.py` & `crosscompute-0.9.4.4/tests/test_routines_variable.py`

 * *Files identical despite different names*

### Comparing `crosscompute-0.9.4.3/tests/test_routines_work.py` & `crosscompute-0.9.4.4/tests/test_routines_work.py`

 * *Files identical despite different names*

