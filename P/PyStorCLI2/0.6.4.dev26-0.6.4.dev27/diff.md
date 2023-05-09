# Comparing `tmp/PyStorCLI2-0.6.4.dev26.tar.gz` & `tmp/PyStorCLI2-0.6.4.dev27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyStorCLI2-0.6.4.dev26.tar", last modified: Mon May  8 10:48:37 2023, max compression
+gzip compressed data, was "PyStorCLI2-0.6.4.dev27.tar", last modified: Mon May  8 13:48:14 2023, max compression
```

## Comparing `PyStorCLI2-0.6.4.dev26.tar` & `PyStorCLI2-0.6.4.dev27.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.349512 PyStorCLI2-0.6.4.dev26/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.325511 PyStorCLI2-0.6.4.dev26/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.329511 PyStorCLI2-0.6.4.dev26/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.329511 PyStorCLI2-0.6.4.dev26/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-08 10:48:37.349512 PyStorCLI2-0.6.4.dev26/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.333511 PyStorCLI2-0.6.4.dev26/PyStorCLI2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-08 10:48:37.000000 PyStorCLI2-0.6.4.dev26/PyStorCLI2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-08 10:48:37.000000 PyStorCLI2-0.6.4.dev26/PyStorCLI2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 10:48:37.000000 PyStorCLI2-0.6.4.dev26/PyStorCLI2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-08 10:48:37.000000 PyStorCLI2-0.6.4.dev26/PyStorCLI2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-08 10:48:37.000000 PyStorCLI2-0.6.4.dev26/PyStorCLI2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 10:48:37.000000 PyStorCLI2-0.6.4.dev26/PyStorCLI2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.333511 PyStorCLI2-0.6.4.dev26/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-08 10:48:07.000000 PyStorCLI2-0.6.4.dev26/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)   930903 2023-05-08 10:48:07.000000 PyStorCLI2-0.6.4.dev26/docs/pystorcli2.html
--rw-r--r--   0 runner    (1001) docker     (123)   387607 2023-05-08 10:48:08.000000 PyStorCLI2-0.6.4.dev26/docs/search.js
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.333511 PyStorCLI2-0.6.4.dev26/pystorcli/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.333511 PyStorCLI2-0.6.4.dev26/pystorcli/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5262 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/bin/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/cachevault.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/cmdRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.337512 PyStorCLI2-0.6.4.dev26/pystorcli/controller/
--rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/controller/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.337512 PyStorCLI2-0.6.4.dev26/pystorcli/drive/
--rw-r--r--   0 runner    (1001) docker     (123)    18731 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/drive/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/drive/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.337512 PyStorCLI2-0.6.4.dev26/pystorcli/enclosure/
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/enclosure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16215 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/storcli.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-08 10:48:37.000000 PyStorCLI2-0.6.4.dev26/pystorcli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.337512 PyStorCLI2-0.6.4.dev26/pystorcli/virtualdrive/
--rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/virtualdrive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/virtualdrive/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/virtualdrive/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli/virtualdrive/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.337512 PyStorCLI2-0.6.4.dev26/pystorcli2/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.337512 PyStorCLI2-0.6.4.dev26/pystorcli2/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5262 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/bin/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/cachevault.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/cmdRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.337512 PyStorCLI2-0.6.4.dev26/pystorcli2/controller/
--rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/controller/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.341512 PyStorCLI2-0.6.4.dev26/pystorcli2/drive/
--rw-r--r--   0 runner    (1001) docker     (123)    18731 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/drive/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/drive/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.341512 PyStorCLI2-0.6.4.dev26/pystorcli2/enclosure/
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/enclosure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16215 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/storcli.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-08 10:48:37.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.341512 PyStorCLI2-0.6.4.dev26/pystorcli2/virtualdrive/
--rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/virtualdrive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/virtualdrive/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/virtualdrive/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli2/virtualdrive/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.341512 PyStorCLI2-0.6.4.dev26/pystorcli_mirror/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/pystorcli_mirror/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 10:48:37.349512 PyStorCLI2-0.6.4.dev26/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.341512 PyStorCLI2-0.6.4.dev26/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/baseTest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.329511 PyStorCLI2-0.6.4.dev26/tests/datatest/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.329511 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.341512 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test00/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.345512 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test01/
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test01/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test01/__c1_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test01/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test01/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.345512 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test02/
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test02/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test02/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test02/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.345512 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test03/
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test03/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test03/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test03/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.345512 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.345512 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid0_00/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid0_00/__c0_add_vd_r0_name=create_vd_raid0_drives=35_12-13_strip=512_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid0_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid0_00/__c0_v1_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid0_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid0_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.345512 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid1_00/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid1_00/__c0_add_vd_r1_name=create_vd_raid1_drives=35_12-13_strip=512_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid1_00/__c0_add_vd_r1_name=create_vd_raid1_drives=35_12-13_strip=512_PDperArray=2_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid1_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid1_00/__c0_v1_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid1_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid1_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.345512 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/delete_vd_00/
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/delete_vd_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/delete_vd_00/__c0_v1_del_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/delete_vd_00/__c0_v1_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/delete_vd_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/delete_vd_00/device.json
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.349512 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/set_state_offline_00/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_set_offline_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/set_state_offline_00/__c0_e35_sall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/set_state_offline_00/__c0_e35_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/set_state_offline_00/__c0_eall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/set_state_offline_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/set_state_offline_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/set_state_offline_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.349512 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_events_00/
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_events_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_events_00/__c0_show_events_file=_root_raid_events.log_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_events_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_events_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.349512 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_foreign_config_00/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_foreign_config_00/__c0__fall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_foreign_config_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_foreign_config_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_foreign_config_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.349512 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_foreign_config_01/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_foreign_config_01/__c0__fall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_foreign_config_01/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_foreign_config_01/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_foreign_config_01/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.349512 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/spindown_disk_00/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_spindown_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/spindown_disk_00/__c0_e35_sall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/spindown_disk_00/__c0_e35_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/spindown_disk_00/__c0_eall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/spindown_disk_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/spindown_disk_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/spindown_disk_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.329511 PyStorCLI2-0.6.4.dev26/tests/datatest/storcliSet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:48:37.349512 PyStorCLI2-0.6.4.dev26/tests/datatest/storcliSet/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/datatest/storcliSet/dummy/device.json
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/storclifile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-08 10:47:50.000000 PyStorCLI2-0.6.4.dev26/tests/test_storcli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.406348 PyStorCLI2-0.6.4.dev27/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.386348 PyStorCLI2-0.6.4.dev27/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.390348 PyStorCLI2-0.6.4.dev27/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.390348 PyStorCLI2-0.6.4.dev27/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-08 13:48:14.402348 PyStorCLI2-0.6.4.dev27/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.390348 PyStorCLI2-0.6.4.dev27/PyStorCLI2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-08 13:48:14.000000 PyStorCLI2-0.6.4.dev27/PyStorCLI2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-08 13:48:14.000000 PyStorCLI2-0.6.4.dev27/PyStorCLI2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:48:14.000000 PyStorCLI2-0.6.4.dev27/PyStorCLI2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-08 13:48:14.000000 PyStorCLI2-0.6.4.dev27/PyStorCLI2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-08 13:48:14.000000 PyStorCLI2-0.6.4.dev27/PyStorCLI2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:48:14.000000 PyStorCLI2-0.6.4.dev27/PyStorCLI2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.390348 PyStorCLI2-0.6.4.dev27/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-08 13:47:49.000000 PyStorCLI2-0.6.4.dev27/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)   930903 2023-05-08 13:47:49.000000 PyStorCLI2-0.6.4.dev27/docs/pystorcli2.html
+-rw-r--r--   0 runner    (1001) docker     (123)   387607 2023-05-08 13:47:49.000000 PyStorCLI2-0.6.4.dev27/docs/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.394348 PyStorCLI2-0.6.4.dev27/pystorcli/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.394348 PyStorCLI2-0.6.4.dev27/pystorcli/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5262 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/bin/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/cachevault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/cmdRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.394348 PyStorCLI2-0.6.4.dev27/pystorcli/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/controller/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.394348 PyStorCLI2-0.6.4.dev27/pystorcli/drive/
+-rw-r--r--   0 runner    (1001) docker     (123)    18731 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/drive/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/drive/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.394348 PyStorCLI2-0.6.4.dev27/pystorcli/enclosure/
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/enclosure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16215 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/storcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-08 13:48:14.000000 PyStorCLI2-0.6.4.dev27/pystorcli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.394348 PyStorCLI2-0.6.4.dev27/pystorcli/virtualdrive/
+-rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/virtualdrive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/virtualdrive/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/virtualdrive/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli/virtualdrive/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.394348 PyStorCLI2-0.6.4.dev27/pystorcli2/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.394348 PyStorCLI2-0.6.4.dev27/pystorcli2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5262 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/bin/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/cachevault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/cmdRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.394348 PyStorCLI2-0.6.4.dev27/pystorcli2/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/controller/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.394348 PyStorCLI2-0.6.4.dev27/pystorcli2/drive/
+-rw-r--r--   0 runner    (1001) docker     (123)    18731 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/drive/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/drive/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.394348 PyStorCLI2-0.6.4.dev27/pystorcli2/enclosure/
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/enclosure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16215 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/storcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-08 13:48:14.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.398348 PyStorCLI2-0.6.4.dev27/pystorcli2/virtualdrive/
+-rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/virtualdrive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/virtualdrive/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/virtualdrive/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli2/virtualdrive/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.398348 PyStorCLI2-0.6.4.dev27/pystorcli_mirror/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/pystorcli_mirror/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:48:14.406348 PyStorCLI2-0.6.4.dev27/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.398348 PyStorCLI2-0.6.4.dev27/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/baseTest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.386348 PyStorCLI2-0.6.4.dev27/tests/datatest/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.386348 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.398348 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test00/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.398348 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test01/
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test01/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test01/__c1_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test01/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test01/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.398348 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test02/
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test02/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test02/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test02/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.398348 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test03/
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test03/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test03/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test03/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.398348 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.398348 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid0_00/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid0_00/__c0_add_vd_r0_name=create_vd_raid0_drives=35_12-13_strip=512_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid0_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid0_00/__c0_v1_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid0_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid0_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.398348 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid1_00/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid1_00/__c0_add_vd_r1_name=create_vd_raid1_drives=35_12-13_strip=512_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid1_00/__c0_add_vd_r1_name=create_vd_raid1_drives=35_12-13_strip=512_PDperArray=2_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid1_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid1_00/__c0_v1_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid1_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid1_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.402348 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/delete_vd_00/
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/delete_vd_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/delete_vd_00/__c0_v1_del_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/delete_vd_00/__c0_v1_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/delete_vd_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/delete_vd_00/device.json
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.402348 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/set_state_offline_00/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_set_offline_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/set_state_offline_00/__c0_e35_sall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/set_state_offline_00/__c0_e35_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/set_state_offline_00/__c0_eall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/set_state_offline_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/set_state_offline_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/set_state_offline_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.402348 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_events_00/
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_events_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_events_00/__c0_show_events_file=_root_raid_events.log_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_events_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_events_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.402348 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_foreign_config_00/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_foreign_config_00/__c0__fall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_foreign_config_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_foreign_config_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_foreign_config_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.402348 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_foreign_config_01/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_foreign_config_01/__c0__fall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_foreign_config_01/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_foreign_config_01/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_foreign_config_01/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.402348 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/spindown_disk_00/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_spindown_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/spindown_disk_00/__c0_e35_sall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/spindown_disk_00/__c0_e35_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/spindown_disk_00/__c0_eall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/spindown_disk_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/spindown_disk_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/spindown_disk_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.386348 PyStorCLI2-0.6.4.dev27/tests/datatest/storcliSet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:48:14.402348 PyStorCLI2-0.6.4.dev27/tests/datatest/storcliSet/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/datatest/storcliSet/dummy/device.json
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/storclifile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-08 13:47:32.000000 PyStorCLI2-0.6.4.dev27/tests/test_storcli.py
```

### Comparing `PyStorCLI2-0.6.4.dev26/.github/workflows/check.yml` & `PyStorCLI2-0.6.4.dev27/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/.github/workflows/publish-to-pypi.yml` & `PyStorCLI2-0.6.4.dev27/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/CHANGELOG.md` & `PyStorCLI2-0.6.4.dev27/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Version 0.6.4
 =============
 
 - **New features**:
   -----------------
-- [**Controller**]        Added methods to control the foreign configuration. (PR [#11](https://github.com/Naudit/pystorcli2/pull/11))
-- [**Controller**]        Now some storcli calls can return an error and get handled without raising exceptions. (Issue [#13](https://github.com/Naudit/pystorcli2/issues/13))
-- [**Drive**]             Added some aliases to `drive.state` & `drive.set_state` method. (Issue [#12](https://github.com/Naudit/pystorcli2/issues/12))
-- Added enum-class StorcliError. This Enum stores any posible (documented) error reported by storcli. We can expect & catch some of them if we want to
+  - [**Controller**]        Added methods to control the foreign configuration. (PR [#11](https://github.com/Naudit/pystorcli2/pull/11))
+  - [**Controller**]        Now some storcli calls can return an error and get handled without raising exceptions. (Issue [#13](https://github.com/Naudit/pystorcli2/issues/13))
+  - [**Drive**]             Added some aliases to `drive.state` & `drive.set_state` method. (Issue [#12](https://github.com/Naudit/pystorcli2/issues/12))
+  - Added enum-class StorcliError. This Enum stores any posible (documented) error reported by storcli. We can expect & catch some of them if we want to
 
 - **Changes**:
   ----------
   - [**Storcli**]         Migrated from subprocess.run -> subprocess.popen. Requested by @ulmitov in Issue [#13](https://github.com/Naudit/pystorcli2/issues/13)
 
 Thanks to @ulmitov & @dgilbert101 for the contributions to this release
```

### Comparing `PyStorCLI2-0.6.4.dev26/LICENSE` & `PyStorCLI2-0.6.4.dev27/LICENSE`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/PKG-INFO` & `PyStorCLI2-0.6.4.dev27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStorCLI2
-Version: 0.6.4.dev26
+Version: 0.6.4.dev27
 Summary: StorCLI module wrapper 2
 Author-email: Rafael Leira <rafael.leira@naudit.es>, Martin Dojcak <martin.dojcak@lablabs.io>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Naudit/pystorcli2
 Keywords: storcli,wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `PyStorCLI2-0.6.4.dev26/PyStorCLI2.egg-info/PKG-INFO` & `PyStorCLI2-0.6.4.dev27/PyStorCLI2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStorCLI2
-Version: 0.6.4.dev26
+Version: 0.6.4.dev27
 Summary: StorCLI module wrapper 2
 Author-email: Rafael Leira <rafael.leira@naudit.es>, Martin Dojcak <martin.dojcak@lablabs.io>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Naudit/pystorcli2
 Keywords: storcli,wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `PyStorCLI2-0.6.4.dev26/PyStorCLI2.egg-info/SOURCES.txt` & `PyStorCLI2-0.6.4.dev27/PyStorCLI2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/README.md` & `PyStorCLI2-0.6.4.dev27/README.md`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/docs/pystorcli2.html` & `PyStorCLI2-0.6.4.dev27/docs/pystorcli2.html`

 * *Files 0% similar despite different names*

```diff
@@ -616,15 +616,15 @@
 </span></pre></div>
 
 
             </section>
                 <section id="__version__">
                     <div class="attr variable">
             <span class="name">__version__</span>        =
-<span class="default_value">&#39;0.6.4.dev26&#39;</span>
+<span class="default_value">&#39;0.6.4.dev27&#39;</span>
 
         
     </div>
     <a class="headerlink" href="#__version__"></a>
```

#### html2text {}

```diff
@@ -197,15 +197,15 @@
 14from .drive import DriveState, Drive, Drives
 15from .virtualdrive import VirtualDrive, VirtualDrives
 16
 17__all__ = ['__version__', 'StorCLI', 'Controller', 'Controllers',
 18           'Enclosure', 'Enclosures', 'DriveState', 'Drive', 'Drives',
 'VirtualDrive', 'VirtualDrives']
 
-__version__ = '0.6.4.dev26'
+__version__ = '0.6.4.dev27'
    ⁰
 class StorCLI: View Source
 _29class StorCLI(object):
 _30    """StorCLI command line wrapper
 _31
 _32    Instance of this class is storcli command line wrapper
 _33
```

### Comparing `PyStorCLI2-0.6.4.dev26/docs/search.js` & `PyStorCLI2-0.6.4.dev27/docs/search.js`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pyproject.toml` & `PyStorCLI2-0.6.4.dev27/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/__init__.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/bin/metrics.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/bin/metrics.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/cachevault.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/cachevault.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/cmdRunner.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/cmdRunner.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/common.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/common.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/controller/__init__.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/controller/metrics.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/controller/metrics.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/drive/__init__.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/drive/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/drive/metrics.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/drive/metrics.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/drive/state.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/drive/state.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/enclosure/__init__.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/enclosure/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/errors.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/errors.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/exc.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/exc.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/storcli.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/storcli.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/virtualdrive/__init__.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/virtualdrive/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/virtualdrive/access.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/virtualdrive/access.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/virtualdrive/metrics.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/virtualdrive/metrics.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli/virtualdrive/state.py` & `PyStorCLI2-0.6.4.dev27/pystorcli/virtualdrive/state.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/__init__.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/bin/metrics.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/bin/metrics.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/cachevault.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/cachevault.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/cmdRunner.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/cmdRunner.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/common.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/common.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/controller/__init__.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/controller/metrics.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/controller/metrics.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/drive/__init__.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/drive/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/drive/metrics.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/drive/metrics.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/drive/state.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/drive/state.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/enclosure/__init__.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/enclosure/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/errors.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/errors.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/exc.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/exc.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/storcli.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/storcli.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/virtualdrive/__init__.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/virtualdrive/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/virtualdrive/access.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/virtualdrive/access.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/virtualdrive/metrics.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/virtualdrive/metrics.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli2/virtualdrive/state.py` & `PyStorCLI2-0.6.4.dev27/pystorcli2/virtualdrive/state.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/pystorcli_mirror/__init__.py` & `PyStorCLI2-0.6.4.dev27/pystorcli_mirror/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/baseTest.py` & `PyStorCLI2-0.6.4.dev27/tests/baseTest.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test01/__c0_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test01/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test01/__c1_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test01/__c1_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test01/_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test01/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test02/__c0_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test02/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test02/_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test02/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test03/__c0_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test03/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/controllerSet/test03/_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/controllerSet/test03/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid0_00/__c0_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid0_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid0_00/__c0_v1_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid0_00/__c0_v1_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid0_00/_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid0_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid1_00/__c0_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid1_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid1_00/__c0_v1_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid1_00/__c0_v1_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/create_vd_raid1_00/_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/create_vd_raid1_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/delete_vd_00/__c0_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/delete_vd_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/delete_vd_00/__c0_v1_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/delete_vd_00/__c0_v1_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/delete_vd_00/_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/delete_vd_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/set_state_offline_00/__c0_e35_sall_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/set_state_offline_00/__c0_e35_sall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/set_state_offline_00/__c0_e35_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/set_state_offline_00/__c0_e35_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/set_state_offline_00/__c0_eall_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/set_state_offline_00/__c0_eall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/set_state_offline_00/__c0_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/set_state_offline_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/set_state_offline_00/_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/set_state_offline_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_events_00/__c0_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_events_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_events_00/_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_events_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_foreign_config_00/__c0__fall_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_foreign_config_00/__c0__fall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_foreign_config_00/__c0_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_foreign_config_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_foreign_config_00/_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_foreign_config_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_foreign_config_01/__c0_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_foreign_config_01/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/show_foreign_config_01/_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/show_foreign_config_01/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/spindown_disk_00/__c0_e35_sall_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/spindown_disk_00/__c0_e35_sall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/spindown_disk_00/__c0_e35_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/spindown_disk_00/__c0_e35_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/spindown_disk_00/__c0_eall_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/spindown_disk_00/__c0_eall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/spindown_disk_00/__c0_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/spindown_disk_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/datatest/namedSet/spindown_disk_00/_show_J.json` & `PyStorCLI2-0.6.4.dev27/tests/datatest/namedSet/spindown_disk_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/exceptions.py` & `PyStorCLI2-0.6.4.dev27/tests/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/storclifile.py` & `PyStorCLI2-0.6.4.dev27/tests/storclifile.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/test_common.py` & `PyStorCLI2-0.6.4.dev27/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/test_controllers.py` & `PyStorCLI2-0.6.4.dev27/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/test_operations.py` & `PyStorCLI2-0.6.4.dev27/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.4.dev26/tests/test_storcli.py` & `PyStorCLI2-0.6.4.dev27/tests/test_storcli.py`

 * *Files identical despite different names*

