# Comparing `tmp/Aestate-1.0.9.tar.gz` & `tmp/Aestate-1.0.9a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Aestate-1.0.9.tar", last modified: Tue Apr 25 06:55:03 2023, max compression
+gzip compressed data, was "Aestate-1.0.9a1.tar", last modified: Tue May  9 07:03:59 2023, max compression
```

## Comparing `Aestate-1.0.9.tar` & `Aestate-1.0.9a1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.687219 Aestate-1.0.9/
-drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.641373 Aestate-1.0.9/Aestate.egg-info/
--rw-rw-rw-   0        0        0     9903 2023-04-25 06:55:03.000000 Aestate-1.0.9/Aestate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1408 2023-04-25 06:55:03.000000 Aestate-1.0.9/Aestate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 06:55:03.000000 Aestate-1.0.9/Aestate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-25 06:55:03.000000 Aestate-1.0.9/Aestate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-04-25 06:55:03.000000 Aestate-1.0.9/Aestate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 06:55:03.000000 Aestate-1.0.9/Aestate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11556 2023-03-09 03:30:52.000000 Aestate-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     9903 2023-04-25 06:55:03.687219 Aestate-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     9285 2023-04-25 06:54:22.000000 Aestate-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.643366 Aestate-1.0.9/aestate/
--rw-rw-rw-   0        0        0      396 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.645359 Aestate-1.0.9/aestate/ajson/
--rw-rw-rw-   0        0        0       53 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/ajson/__init__.py
--rw-rw-rw-   0        0        0    11743 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/ajson/ajson.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.649346 Aestate-1.0.9/aestate/base/
--rw-rw-rw-   0        0        0        0 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/base/__init__.py
--rw-rw-rw-   0        0        0      664 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/base/anno.py
--rw-rw-rw-   0        0        0     1504 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/base/manage.py
--rw-rw-rw-   0        0        0     1059 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/base/model.py
--rw-rw-rw-   0        0        0    10358 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/base/proxy.py
--rw-rw-rw-   0        0        0      416 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/conf.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.651339 Aestate-1.0.9/aestate/dbs/
--rw-rw-rw-   0        0        0      156 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/dbs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.652337 Aestate-1.0.9/aestate/dbs/_mssql/
--rw-rw-rw-   0        0        0    13957 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/dbs/_mssql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.654328 Aestate-1.0.9/aestate/dbs/_mysql/
--rw-rw-rw-   0        0        0    17947 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/dbs/_mysql/__init__.py
--rw-rw-rw-   0        0        0     6609 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/dbs/_mysql/tag.py
--rw-rw-rw-   0        0        0      255 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/dbs/base.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.657329 Aestate-1.0.9/aestate/exception/
--rw-rw-rw-   0        0        0     1446 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/exception/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.658315 Aestate-1.0.9/aestate/i18n/
--rw-rw-rw-   0        0        0     3573 2023-04-25 06:54:22.000000 Aestate-1.0.9/aestate/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.663298 Aestate-1.0.9/aestate/util/
--rw-rw-rw-   0        0        0     1298 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/util/CompulsoryRun.py
--rw-rw-rw-   0        0        0    13156 2023-04-25 06:54:22.000000 Aestate-1.0.9/aestate/util/Log.py
--rw-rw-rw-   0        0        0      354 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/util/__init__.py
--rw-rw-rw-   0        0        0     6280 2023-04-25 02:31:39.000000 Aestate-1.0.9/aestate/util/others.py
--rw-rw-rw-   0        0        0      779 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/util/sqlOpera.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.673265 Aestate-1.0.9/aestate/work/
--rw-rw-rw-   0        0        0     2853 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/Adapter.py
--rw-rw-rw-   0        0        0    10336 2023-04-25 06:54:22.000000 Aestate-1.0.9/aestate/work/Annotation.py
--rw-rw-rw-   0        0        0     5402 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/AopContainer.py
--rw-rw-rw-   0        0        0     1977 2023-04-25 06:54:22.000000 Aestate-1.0.9/aestate/work/Cache.py
--rw-rw-rw-   0        0        0     2708 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/Config.py
--rw-rw-rw-   0        0        0     5981 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/Manage.py
--rw-rw-rw-   0        0        0     9658 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/Modes.py
--rw-rw-rw-   0        0        0     4761 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/Serialize.py
--rw-rw-rw-   0        0        0      321 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.674261 Aestate-1.0.9/aestate/work/commands/
--rw-rw-rw-   0        0        0     5549 2023-04-25 06:54:22.000000 Aestate-1.0.9/aestate/work/commands/__init__.py
--rw-rw-rw-   0        0        0    18717 2023-04-25 06:54:22.000000 Aestate-1.0.9/aestate/work/orm.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.677265 Aestate-1.0.9/aestate/work/proxy/
--rw-rw-rw-   0        0        0    10724 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/proxy/SqlOperaProxy.py
--rw-rw-rw-   0        0        0       17 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/proxy/__init__.py
--rw-rw-rw-   0        0        0     5112 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/repository.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.680241 Aestate-1.0.9/aestate/work/sql/
--rw-rw-rw-   0        0        0     6526 2023-04-25 06:54:22.000000 Aestate-1.0.9/aestate/work/sql/ExecuteSql.py
--rw-rw-rw-   0        0        0     5030 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/sql/ProxyOpera.py
--rw-rw-rw-   0        0        0       17 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/sql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.686222 Aestate-1.0.9/aestate/work/xmlhandler/
--rw-rw-rw-   0        0        0     3776 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/xmlhandler/XMLScriptBuilder.py
--rw-rw-rw-   0        0        0       17 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/xmlhandler/__init__.py
--rw-rw-rw-   0        0        0     1796 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/xmlhandler/base.py
--rw-rw-rw-   0        0        0      333 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/xmlhandler/final.py
--rw-rw-rw-   0        0        0    13722 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/xmlhandler/nodes.py
--rw-rw-rw-   0        0        0     2077 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/xmlhandler/utils.py
--rw-rw-rw-   0        0        0      108 2023-03-09 03:30:52.000000 Aestate-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 06:55:03.688215 Aestate-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1618 2023-03-09 03:30:52.000000 Aestate-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:03:59.828801 Aestate-1.0.9a1/
+drwxrwxrwx   0        0        0        0 2023-05-09 07:03:59.787296 Aestate-1.0.9a1/Aestate.egg-info/
+-rw-rw-rw-   0        0        0     9826 2023-05-09 07:03:59.000000 Aestate-1.0.9a1/Aestate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1408 2023-05-09 07:03:59.000000 Aestate-1.0.9a1/Aestate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 07:03:59.000000 Aestate-1.0.9a1/Aestate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-09 07:03:59.000000 Aestate-1.0.9a1/Aestate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-05-09 07:03:59.000000 Aestate-1.0.9a1/Aestate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-09 07:03:59.000000 Aestate-1.0.9a1/Aestate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11556 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/LICENSE
+-rw-rw-rw-   0        0        0     9826 2023-05-09 07:03:59.827792 Aestate-1.0.9a1/PKG-INFO
+-rw-rw-rw-   0        0        0     9206 2023-05-09 06:12:59.000000 Aestate-1.0.9a1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 07:03:59.789297 Aestate-1.0.9a1/aestate/
+-rw-rw-rw-   0        0        0      396 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:03:59.791299 Aestate-1.0.9a1/aestate/ajson/
+-rw-rw-rw-   0        0        0       53 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/ajson/__init__.py
+-rw-rw-rw-   0        0        0    11743 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/ajson/ajson.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:03:59.795299 Aestate-1.0.9a1/aestate/base/
+-rw-rw-rw-   0        0        0        0 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/base/__init__.py
+-rw-rw-rw-   0        0        0      664 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/base/anno.py
+-rw-rw-rw-   0        0        0     1504 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/base/manage.py
+-rw-rw-rw-   0        0        0     1059 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/base/model.py
+-rw-rw-rw-   0        0        0    10358 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/base/proxy.py
+-rw-rw-rw-   0        0        0      416 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:03:59.798299 Aestate-1.0.9a1/aestate/dbs/
+-rw-rw-rw-   0        0        0      156 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/dbs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:03:59.799300 Aestate-1.0.9a1/aestate/dbs/_mssql/
+-rw-rw-rw-   0        0        0    13957 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/dbs/_mssql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:03:59.800308 Aestate-1.0.9a1/aestate/dbs/_mysql/
+-rw-rw-rw-   0        0        0    17947 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/dbs/_mysql/__init__.py
+-rw-rw-rw-   0        0        0     6609 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/dbs/_mysql/tag.py
+-rw-rw-rw-   0        0        0      255 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/dbs/base.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:03:59.801308 Aestate-1.0.9a1/aestate/exception/
+-rw-rw-rw-   0        0        0     1446 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/exception/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:03:59.802299 Aestate-1.0.9a1/aestate/i18n/
+-rw-rw-rw-   0        0        0     3936 2023-05-09 06:12:59.000000 Aestate-1.0.9a1/aestate/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:03:59.806828 Aestate-1.0.9a1/aestate/util/
+-rw-rw-rw-   0        0        0     1298 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/util/CompulsoryRun.py
+-rw-rw-rw-   0        0        0    13156 2023-04-25 06:54:22.000000 Aestate-1.0.9a1/aestate/util/Log.py
+-rw-rw-rw-   0        0        0      354 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/util/__init__.py
+-rw-rw-rw-   0        0        0     6280 2023-04-25 02:31:39.000000 Aestate-1.0.9a1/aestate/util/others.py
+-rw-rw-rw-   0        0        0      779 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/util/sqlOpera.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:03:59.816837 Aestate-1.0.9a1/aestate/work/
+-rw-rw-rw-   0        0        0     2853 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/work/Adapter.py
+-rw-rw-rw-   0        0        0    11003 2023-05-09 06:12:59.000000 Aestate-1.0.9a1/aestate/work/Annotation.py
+-rw-rw-rw-   0        0        0     5402 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/work/AopContainer.py
+-rw-rw-rw-   0        0        0     1977 2023-04-25 06:54:22.000000 Aestate-1.0.9a1/aestate/work/Cache.py
+-rw-rw-rw-   0        0        0     2708 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/work/Config.py
+-rw-rw-rw-   0        0        0     5981 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/work/Manage.py
+-rw-rw-rw-   0        0        0     9658 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/work/Modes.py
+-rw-rw-rw-   0        0        0     4761 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/work/Serialize.py
+-rw-rw-rw-   0        0        0      321 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/work/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:03:59.817828 Aestate-1.0.9a1/aestate/work/commands/
+-rw-rw-rw-   0        0        0     5551 2023-05-09 07:03:50.000000 Aestate-1.0.9a1/aestate/work/commands/__init__.py
+-rw-rw-rw-   0        0        0    18717 2023-04-25 06:54:22.000000 Aestate-1.0.9a1/aestate/work/orm.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:03:59.819056 Aestate-1.0.9a1/aestate/work/proxy/
+-rw-rw-rw-   0        0        0    10724 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/work/proxy/SqlOperaProxy.py
+-rw-rw-rw-   0        0        0       17 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/work/proxy/__init__.py
+-rw-rw-rw-   0        0        0     5112 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/work/repository.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:03:59.821792 Aestate-1.0.9a1/aestate/work/sql/
+-rw-rw-rw-   0        0        0     6526 2023-04-25 06:54:22.000000 Aestate-1.0.9a1/aestate/work/sql/ExecuteSql.py
+-rw-rw-rw-   0        0        0     5030 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/work/sql/ProxyOpera.py
+-rw-rw-rw-   0        0        0       17 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/work/sql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:03:59.826792 Aestate-1.0.9a1/aestate/work/xmlhandler/
+-rw-rw-rw-   0        0        0     3776 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/work/xmlhandler/XMLScriptBuilder.py
+-rw-rw-rw-   0        0        0       17 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/work/xmlhandler/__init__.py
+-rw-rw-rw-   0        0        0     1643 2023-05-09 06:12:59.000000 Aestate-1.0.9a1/aestate/work/xmlhandler/base.py
+-rw-rw-rw-   0        0        0      333 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/aestate/work/xmlhandler/final.py
+-rw-rw-rw-   0        0        0    16376 2023-05-09 06:12:59.000000 Aestate-1.0.9a1/aestate/work/xmlhandler/nodes.py
+-rw-rw-rw-   0        0        0     2043 2023-05-09 06:12:59.000000 Aestate-1.0.9a1/aestate/work/xmlhandler/utils.py
+-rw-rw-rw-   0        0        0      108 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 07:03:59.828801 Aestate-1.0.9a1/setup.cfg
+-rw-rw-rw-   0        0        0     1618 2023-03-09 03:30:52.000000 Aestate-1.0.9a1/setup.py
```

### Comparing `Aestate-1.0.9/Aestate.egg-info/PKG-INFO` & `Aestate-1.0.9a1/Aestate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aestate
-Version: 1.0.9
+Version: 1.0.9a1
 Summary: Aestate framework for Python,You can see:https://gitee.com/aecode/aestate
 Home-page: https://gitee.com/aecode/aestate
 Author: CACode
 Author-email: cacode@163.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://gitee.com/aecode/aestate/issues
 Platform: UNKNOWN
@@ -78,14 +78,15 @@
         <result field="d1_name" properties="name"/>
         <result field="d1_password" properties="password"/>
         <foreign type="example.table.demoModels.Demo" name="demoJoin">
             <result field="d2_id" properties="id"/>
             <result field="d2_name" properties="name"/>
             <result field="d2_password" properties="password"/>
         </foreign>
+        <foreign ref="demoJoin" single="false"/>
     </resultMap>
     <item id="findAllById">
         <select resultType="resultMapLeftJoin">
             SELECT
             <!-- 导入查询的字段 -->
             <!--            <include from="templateField"/>-->
             <include from="tempSymbol"/>
@@ -117,48 +118,44 @@
 
 - 其次就是在兼容性方面，由于这个世界上的数据库种类太多了没办法做到统一， **Aestate**保留了对其他小众数据库的实现接口，尽可能多兼容数据库。
 
 - 数据库表方面，Django是会生成数据django自己系统内部的表，在迁移的时候呢如果做错一步可能对于新手
   来讲后面的修复操作是极其难的，也未必能够在短时间内定位问题并修复。**Aestate**为了解决这个问题，将make
   和手动建表尽可能的兼容，不会生成额外的表和数据，也不会捆绑某个特定系统，将pojo/model复制出来可以直接为下一个项目使用。
 
-- 缓存方面参考了Mybatis的实现方法并略微修改，**Aestate**有两个内存管理模块，用于保证数据的完整性，
+- ~~缓存方面参考了Mybatis的实现方法并略微修改，**Aestate**有两个内存管理模块，用于保证数据的完整性，
   当一些特别大的数据占满缓存时，**Aestate**
   会尽量多的去分配内存保证数据完整性，除外才会去管理内存（不建议操作大于系统内存2/10的数据）。**Aestate**
-  有弹性内存管理方式，会根据系统的执行自动调整缓存大小，尽可能的加快运行速度，减少对数据库的连接次数。
+  有弹性内存管理方式，会根据系统的执行自动调整缓存大小，尽可能的加快运行速度，减少对数据库的连接次数。~~（最新1.0.9已删除缓存策略）
 
 - 自带日志和美化，不需要下载其他插件就可以把日志变色，自动保存日志，这个功能对于爱美的大兄弟简直就 是神仙般的存在（当然也可能只有我喜欢装逼）
 
 
 - 还有很多......
 
 > 寻找志同道合的朋友一起开发**Aestate**  
 > 作者QQ:2075383131(云)  
 > qq群：909044439(Aestate Framework)
 
 # 关于教程和文档地址
 
-因为开发aestate的同学大部分都是来自各地的`穷学生`,我已经没有办法支付的起下一年的服务器费用（508.02元）， 因为这是我`63%`
-的生活费。
-
-以后教程和文档更新依靠CSDN、OSCHINA、知乎、bilibili以及各位捐献云服务器和托管平台等
+文档已经迁移到免费托管平台：http://aestate.angid.eu.org
 
 > csdn: [AECODE](https://blog.csdn.net/qq_43059459)  
 > OSCHINA: [CACode](https://my.oschina.net/u/4841054)  
-> 知乎: [CACode](https://www.zhihu.com/people/ben-ren-pin-kun-seng)  
 > bilibili大学堂: [你在写臭虫?](https://space.bilibili.com/371089110)  
-> 官网域名: [cacode.ren](https://cacode.ren)  
-> 文档官网域名: [doc.cacode.ren](https://doc.cacode.ren)  
+> 官网域名: [cacode.ren](https://cacode.ren)（迁移到腾讯云没备案）  
+> 文档官网域名: [~~doc.cacode.ren~~](https://doc.cacode.ren)&nbsp;[http://aestate.angid.eu.org](http://aestate.angid.eu.org)  
 > Gitee官方: [https://aecode.gitee.io/aestate-doc](https://aecode.gitee.io/aestate-doc)  
 > 项目体系结构: [aecode.gitee.io/aestate](https://aecode.gitee.io/aestate/)
 
 # 先决条件
 
 > Python >=3.6 (其他版本没试过)  
-> 教程文档地址：http://doc.cacode.ren
+> 教程文档地址：~~http://doc.cacode.ren~~&nbsp;http://aestate.angid.eu.org
 
 # 版本说明
 
 基础需要2.7以上的python版本，对于只需要执行sql可以使用2.7以上（不建议）
 
 最优的办法是使用3.6以上，可以使用绝大部分功能
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Aestate Version: 1.0.9 Summary: Aestate framework
+Metadata-Version: 2.1 Name: Aestate Version: 1.0.9a1 Summary: Aestate framework
 for Python,You can see:https://gitee.com/aecode/aestate Home-page: https://
 gitee.com/aecode/aestate Author: CACode Author-email: cacode@163.com License:
 Apache License 2.0 Project-URL: Bug Tracker, https://gitee.com/aecode/aestate/
 issues Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Database Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
@@ -24,37 +24,36 @@
 å¶æ¬¡å°±æ¯å¨å¼å®¹æ§æ¹é¢ï¼ç±äºè¿ä¸ªä¸çä¸çæ°æ®åºç§ç±»å¤ªå¤äºæ²¡åæ³åå°ç»ä¸ï¼
 **Aestate**ä¿çäºå¯¹å¶ä»å°ä¼æ°æ®åºçå®ç°æ¥å£ï¼å°½å¯è½å¤å¼å®¹æ°æ®åºã
 -
 æ°æ®åºè¡¨æ¹é¢ï¼Djangoæ¯ä¼çææ°æ®djangoèªå·±ç³»ç»åé¨çè¡¨ï¼å¨è¿ç§»çæ¶åå¢å¦æåéä¸æ­¥å¯è½å¯¹äºæ°æ
 æ¥è®²åé¢çä¿®å¤æä½æ¯æå¶é¾çï¼ä¹æªå¿è½å¤å¨ç­æ¶é´åå®ä½é®é¢å¹¶ä¿®å¤ã**Aestate**ä¸ºäºè§£å³è¿ä¸ªé®é¢ï¼å°make
 åæå¨å»ºè¡¨å°½å¯è½çå¼å®¹ï¼ä¸ä¼çæé¢å¤çè¡¨åæ°æ®ï¼ä¹ä¸ä¼æç»æä¸ªç¹å®ç³»ç»ï¼å°pojo/
 modelå¤å¶åºæ¥å¯ä»¥ç´æ¥ä¸ºä¸ä¸ä¸ªé¡¹ç®ä½¿ç¨ã -
-ç¼å­æ¹é¢åèäºMybatisçå®ç°æ¹æ³å¹¶ç¥å¾®ä¿®æ¹ï¼**Aestate**æä¸¤ä¸ªåå­ç®¡çæ¨¡åï¼ç¨äºä¿è¯æ°æ®çå®æ´æ§ï¼
+~~ç¼å­æ¹é¢åèäºMybatisçå®ç°æ¹æ³å¹¶ç¥å¾®ä¿®æ¹ï¼**Aestate**æä¸¤ä¸ªåå­ç®¡çæ¨¡åï¼ç¨äºä¿è¯æ°æ®çå®æ´æ§ï¼
 å½ä¸äºç¹å«å¤§çæ°æ®å æ»¡ç¼å­æ¶ï¼**Aestate**
 ä¼å°½éå¤çå»åéåå­ä¿è¯æ°æ®å®æ´æ§ï¼é¤å¤æä¼å»ç®¡çåå­ï¼ä¸å»ºè®®æä½å¤§äºç³»ç»åå­2/
 10çæ°æ®ï¼ã**Aestate**
-æå¼¹æ§åå­ç®¡çæ¹å¼ï¼ä¼æ ¹æ®ç³»ç»çæ§è¡èªå¨è°æ´ç¼å­å¤§å°ï¼å°½å¯è½çå å¿«è¿è¡éåº¦ï¼åå°å¯¹æ°æ®åºçè¿æ¥æ¬¡æ°ã
+æå¼¹æ§åå­ç®¡çæ¹å¼ï¼ä¼æ ¹æ®ç³»ç»çæ§è¡èªå¨è°æ´ç¼å­å¤§å°ï¼å°½å¯è½çå å¿«è¿è¡éåº¦ï¼åå°å¯¹æ°æ®åºçè¿æ¥æ¬¡æ°ã~~ï¼ææ°1.0.9å·²å é¤ç¼å­ç­ç¥ï¼
 -
 èªå¸¦æ¥å¿åç¾åï¼ä¸éè¦ä¸è½½å¶ä»æä»¶å°±å¯ä»¥ææ¥å¿åè²ï¼èªå¨ä¿å­æ¥å¿ï¼è¿ä¸ªåè½å¯¹äºç±ç¾çå¤§åå¼ç®ç´å°±
 æ¯ç¥ä»è¬çå­å¨ï¼å½ç¶ä¹å¯è½åªææåæ¬¢è£é¼ï¼ -
 è¿æå¾å¤...... > å¯»æ¾å¿åéåçæåä¸èµ·å¼å**Aestate** >
 ä½èQQ:2075383131(äº) > qqç¾¤ï¼909044439(Aestate Framework) #
-å³äºæç¨åææ¡£å°å
-å ä¸ºå¼åaestateçåå­¦å¤§é¨åé½æ¯æ¥èªåå°ç`ç©·å­¦ç`,æå·²ç»æ²¡æåæ³æ¯ä»çèµ·ä¸ä¸å¹´çæå¡å¨è´¹ç¨ï¼508.02åï¼ï¼
-å ä¸ºè¿æ¯æ`63%` ççæ´»è´¹ã
-ä»¥åæç¨åææ¡£æ´æ°ä¾é CSDNãOSCHINAãç¥ä¹ãbilibiliä»¥ååä½æç®äºæå¡å¨åæç®¡å¹³å°ç­
-> csdn: [AECODE](https://blog.csdn.net/qq_43059459) > OSCHINA: [CACode](https:/
-/my.oschina.net/u/4841054) > ç¥ä¹: [CACode](https://www.zhihu.com/people/ben-
-ren-pin-kun-seng) > bilibiliå¤§å­¦å : [ä½ å¨åè­è«?](https://
-space.bilibili.com/371089110) > å®ç½åå: [cacode.ren](https://cacode.ren)
-> ææ¡£å®ç½åå: [doc.cacode.ren](https://doc.cacode.ren) > Giteeå®æ¹:
-[https://aecode.gitee.io/aestate-doc](https://aecode.gitee.io/aestate-doc) >
+å³äºæç¨åææ¡£å°å ææ¡£å·²ç»è¿ç§»å°åè´¹æç®¡å¹³å°ï¼http://
+aestate.angid.eu.org > csdn: [AECODE](https://blog.csdn.net/qq_43059459) >
+OSCHINA: [CACode](https://my.oschina.net/u/4841054) > bilibiliå¤§å­¦å :
+[ä½ å¨åè­è«?](https://space.bilibili.com/371089110) > å®ç½åå:
+[cacode.ren](https://cacode.ren)ï¼è¿ç§»å°è¾è®¯äºæ²¡å¤æ¡ï¼ >
+ææ¡£å®ç½åå: [~~doc.cacode.ren~~](https://doc.cacode.ren) [http://
+aestate.angid.eu.org](http://aestate.angid.eu.org) > Giteeå®æ¹: [https://
+aecode.gitee.io/aestate-doc](https://aecode.gitee.io/aestate-doc) >
 é¡¹ç®ä½ç³»ç»æ: [aecode.gitee.io/aestate](https://aecode.gitee.io/aestate/
 ) # åå³æ¡ä»¶ > Python >=3.6 (å¶ä»çæ¬æ²¡è¯è¿) >
-æç¨ææ¡£å°åï¼http://doc.cacode.ren # çæ¬è¯´æ
+æç¨ææ¡£å°åï¼~~http://doc.cacode.ren~~ http://aestate.angid.eu.org #
+çæ¬è¯´æ
 åºç¡éè¦2.7ä»¥ä¸çpythonçæ¬ï¼å¯¹äºåªéè¦æ§è¡sqlå¯ä»¥ä½¿ç¨2.7ä»¥ä¸ï¼ä¸å»ºè®®ï¼
 æä¼çåæ³æ¯ä½¿ç¨3.6ä»¥ä¸ï¼å¯ä»¥ä½¿ç¨ç»å¤§é¨ååè½
 ç±äº1.0.7å¢å å¼æ­¥æ¹æ³ï¼éè¦å¼æ­¥æ§è¡çå°ä¼ä¼´å¯ä»¥ä½¿ç¨python>=3.7.10ä»¥ä¸çæ¬
 # å®è£
 ç®åæºä»£ç ä»å¼æ¾å¨giteeï¼å¤äºç»ç»CACodeä¸ï¼ä»åºå°åä¸ºï¼
 [aestate](https://gitee.com/aecode/aestate)
 ä½¿ç¨pipæanacondaå®è£**Aestate**ï¼ ```shell pip install aestate conda
```

### Comparing `Aestate-1.0.9/Aestate.egg-info/SOURCES.txt` & `Aestate-1.0.9a1/Aestate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/LICENSE` & `Aestate-1.0.9a1/LICENSE`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/PKG-INFO` & `Aestate-1.0.9a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aestate
-Version: 1.0.9
+Version: 1.0.9a1
 Summary: Aestate framework for Python,You can see:https://gitee.com/aecode/aestate
 Home-page: https://gitee.com/aecode/aestate
 Author: CACode
 Author-email: cacode@163.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://gitee.com/aecode/aestate/issues
 Platform: UNKNOWN
@@ -78,14 +78,15 @@
         <result field="d1_name" properties="name"/>
         <result field="d1_password" properties="password"/>
         <foreign type="example.table.demoModels.Demo" name="demoJoin">
             <result field="d2_id" properties="id"/>
             <result field="d2_name" properties="name"/>
             <result field="d2_password" properties="password"/>
         </foreign>
+        <foreign ref="demoJoin" single="false"/>
     </resultMap>
     <item id="findAllById">
         <select resultType="resultMapLeftJoin">
             SELECT
             <!-- 导入查询的字段 -->
             <!--            <include from="templateField"/>-->
             <include from="tempSymbol"/>
@@ -117,48 +118,44 @@
 
 - 其次就是在兼容性方面，由于这个世界上的数据库种类太多了没办法做到统一， **Aestate**保留了对其他小众数据库的实现接口，尽可能多兼容数据库。
 
 - 数据库表方面，Django是会生成数据django自己系统内部的表，在迁移的时候呢如果做错一步可能对于新手
   来讲后面的修复操作是极其难的，也未必能够在短时间内定位问题并修复。**Aestate**为了解决这个问题，将make
   和手动建表尽可能的兼容，不会生成额外的表和数据，也不会捆绑某个特定系统，将pojo/model复制出来可以直接为下一个项目使用。
 
-- 缓存方面参考了Mybatis的实现方法并略微修改，**Aestate**有两个内存管理模块，用于保证数据的完整性，
+- ~~缓存方面参考了Mybatis的实现方法并略微修改，**Aestate**有两个内存管理模块，用于保证数据的完整性，
   当一些特别大的数据占满缓存时，**Aestate**
   会尽量多的去分配内存保证数据完整性，除外才会去管理内存（不建议操作大于系统内存2/10的数据）。**Aestate**
-  有弹性内存管理方式，会根据系统的执行自动调整缓存大小，尽可能的加快运行速度，减少对数据库的连接次数。
+  有弹性内存管理方式，会根据系统的执行自动调整缓存大小，尽可能的加快运行速度，减少对数据库的连接次数。~~（最新1.0.9已删除缓存策略）
 
 - 自带日志和美化，不需要下载其他插件就可以把日志变色，自动保存日志，这个功能对于爱美的大兄弟简直就 是神仙般的存在（当然也可能只有我喜欢装逼）
 
 
 - 还有很多......
 
 > 寻找志同道合的朋友一起开发**Aestate**  
 > 作者QQ:2075383131(云)  
 > qq群：909044439(Aestate Framework)
 
 # 关于教程和文档地址
 
-因为开发aestate的同学大部分都是来自各地的`穷学生`,我已经没有办法支付的起下一年的服务器费用（508.02元）， 因为这是我`63%`
-的生活费。
-
-以后教程和文档更新依靠CSDN、OSCHINA、知乎、bilibili以及各位捐献云服务器和托管平台等
+文档已经迁移到免费托管平台：http://aestate.angid.eu.org
 
 > csdn: [AECODE](https://blog.csdn.net/qq_43059459)  
 > OSCHINA: [CACode](https://my.oschina.net/u/4841054)  
-> 知乎: [CACode](https://www.zhihu.com/people/ben-ren-pin-kun-seng)  
 > bilibili大学堂: [你在写臭虫?](https://space.bilibili.com/371089110)  
-> 官网域名: [cacode.ren](https://cacode.ren)  
-> 文档官网域名: [doc.cacode.ren](https://doc.cacode.ren)  
+> 官网域名: [cacode.ren](https://cacode.ren)（迁移到腾讯云没备案）  
+> 文档官网域名: [~~doc.cacode.ren~~](https://doc.cacode.ren)&nbsp;[http://aestate.angid.eu.org](http://aestate.angid.eu.org)  
 > Gitee官方: [https://aecode.gitee.io/aestate-doc](https://aecode.gitee.io/aestate-doc)  
 > 项目体系结构: [aecode.gitee.io/aestate](https://aecode.gitee.io/aestate/)
 
 # 先决条件
 
 > Python >=3.6 (其他版本没试过)  
-> 教程文档地址：http://doc.cacode.ren
+> 教程文档地址：~~http://doc.cacode.ren~~&nbsp;http://aestate.angid.eu.org
 
 # 版本说明
 
 基础需要2.7以上的python版本，对于只需要执行sql可以使用2.7以上（不建议）
 
 最优的办法是使用3.6以上，可以使用绝大部分功能
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Aestate Version: 1.0.9 Summary: Aestate framework
+Metadata-Version: 2.1 Name: Aestate Version: 1.0.9a1 Summary: Aestate framework
 for Python,You can see:https://gitee.com/aecode/aestate Home-page: https://
 gitee.com/aecode/aestate Author: CACode Author-email: cacode@163.com License:
 Apache License 2.0 Project-URL: Bug Tracker, https://gitee.com/aecode/aestate/
 issues Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Database Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
@@ -24,37 +24,36 @@
 å¶æ¬¡å°±æ¯å¨å¼å®¹æ§æ¹é¢ï¼ç±äºè¿ä¸ªä¸çä¸çæ°æ®åºç§ç±»å¤ªå¤äºæ²¡åæ³åå°ç»ä¸ï¼
 **Aestate**ä¿çäºå¯¹å¶ä»å°ä¼æ°æ®åºçå®ç°æ¥å£ï¼å°½å¯è½å¤å¼å®¹æ°æ®åºã
 -
 æ°æ®åºè¡¨æ¹é¢ï¼Djangoæ¯ä¼çææ°æ®djangoèªå·±ç³»ç»åé¨çè¡¨ï¼å¨è¿ç§»çæ¶åå¢å¦æåéä¸æ­¥å¯è½å¯¹äºæ°æ
 æ¥è®²åé¢çä¿®å¤æä½æ¯æå¶é¾çï¼ä¹æªå¿è½å¤å¨ç­æ¶é´åå®ä½é®é¢å¹¶ä¿®å¤ã**Aestate**ä¸ºäºè§£å³è¿ä¸ªé®é¢ï¼å°make
 åæå¨å»ºè¡¨å°½å¯è½çå¼å®¹ï¼ä¸ä¼çæé¢å¤çè¡¨åæ°æ®ï¼ä¹ä¸ä¼æç»æä¸ªç¹å®ç³»ç»ï¼å°pojo/
 modelå¤å¶åºæ¥å¯ä»¥ç´æ¥ä¸ºä¸ä¸ä¸ªé¡¹ç®ä½¿ç¨ã -
-ç¼å­æ¹é¢åèäºMybatisçå®ç°æ¹æ³å¹¶ç¥å¾®ä¿®æ¹ï¼**Aestate**æä¸¤ä¸ªåå­ç®¡çæ¨¡åï¼ç¨äºä¿è¯æ°æ®çå®æ´æ§ï¼
+~~ç¼å­æ¹é¢åèäºMybatisçå®ç°æ¹æ³å¹¶ç¥å¾®ä¿®æ¹ï¼**Aestate**æä¸¤ä¸ªåå­ç®¡çæ¨¡åï¼ç¨äºä¿è¯æ°æ®çå®æ´æ§ï¼
 å½ä¸äºç¹å«å¤§çæ°æ®å æ»¡ç¼å­æ¶ï¼**Aestate**
 ä¼å°½éå¤çå»åéåå­ä¿è¯æ°æ®å®æ´æ§ï¼é¤å¤æä¼å»ç®¡çåå­ï¼ä¸å»ºè®®æä½å¤§äºç³»ç»åå­2/
 10çæ°æ®ï¼ã**Aestate**
-æå¼¹æ§åå­ç®¡çæ¹å¼ï¼ä¼æ ¹æ®ç³»ç»çæ§è¡èªå¨è°æ´ç¼å­å¤§å°ï¼å°½å¯è½çå å¿«è¿è¡éåº¦ï¼åå°å¯¹æ°æ®åºçè¿æ¥æ¬¡æ°ã
+æå¼¹æ§åå­ç®¡çæ¹å¼ï¼ä¼æ ¹æ®ç³»ç»çæ§è¡èªå¨è°æ´ç¼å­å¤§å°ï¼å°½å¯è½çå å¿«è¿è¡éåº¦ï¼åå°å¯¹æ°æ®åºçè¿æ¥æ¬¡æ°ã~~ï¼ææ°1.0.9å·²å é¤ç¼å­ç­ç¥ï¼
 -
 èªå¸¦æ¥å¿åç¾åï¼ä¸éè¦ä¸è½½å¶ä»æä»¶å°±å¯ä»¥ææ¥å¿åè²ï¼èªå¨ä¿å­æ¥å¿ï¼è¿ä¸ªåè½å¯¹äºç±ç¾çå¤§åå¼ç®ç´å°±
 æ¯ç¥ä»è¬çå­å¨ï¼å½ç¶ä¹å¯è½åªææåæ¬¢è£é¼ï¼ -
 è¿æå¾å¤...... > å¯»æ¾å¿åéåçæåä¸èµ·å¼å**Aestate** >
 ä½èQQ:2075383131(äº) > qqç¾¤ï¼909044439(Aestate Framework) #
-å³äºæç¨åææ¡£å°å
-å ä¸ºå¼åaestateçåå­¦å¤§é¨åé½æ¯æ¥èªåå°ç`ç©·å­¦ç`,æå·²ç»æ²¡æåæ³æ¯ä»çèµ·ä¸ä¸å¹´çæå¡å¨è´¹ç¨ï¼508.02åï¼ï¼
-å ä¸ºè¿æ¯æ`63%` ççæ´»è´¹ã
-ä»¥åæç¨åææ¡£æ´æ°ä¾é CSDNãOSCHINAãç¥ä¹ãbilibiliä»¥ååä½æç®äºæå¡å¨åæç®¡å¹³å°ç­
-> csdn: [AECODE](https://blog.csdn.net/qq_43059459) > OSCHINA: [CACode](https:/
-/my.oschina.net/u/4841054) > ç¥ä¹: [CACode](https://www.zhihu.com/people/ben-
-ren-pin-kun-seng) > bilibiliå¤§å­¦å : [ä½ å¨åè­è«?](https://
-space.bilibili.com/371089110) > å®ç½åå: [cacode.ren](https://cacode.ren)
-> ææ¡£å®ç½åå: [doc.cacode.ren](https://doc.cacode.ren) > Giteeå®æ¹:
-[https://aecode.gitee.io/aestate-doc](https://aecode.gitee.io/aestate-doc) >
+å³äºæç¨åææ¡£å°å ææ¡£å·²ç»è¿ç§»å°åè´¹æç®¡å¹³å°ï¼http://
+aestate.angid.eu.org > csdn: [AECODE](https://blog.csdn.net/qq_43059459) >
+OSCHINA: [CACode](https://my.oschina.net/u/4841054) > bilibiliå¤§å­¦å :
+[ä½ å¨åè­è«?](https://space.bilibili.com/371089110) > å®ç½åå:
+[cacode.ren](https://cacode.ren)ï¼è¿ç§»å°è¾è®¯äºæ²¡å¤æ¡ï¼ >
+ææ¡£å®ç½åå: [~~doc.cacode.ren~~](https://doc.cacode.ren) [http://
+aestate.angid.eu.org](http://aestate.angid.eu.org) > Giteeå®æ¹: [https://
+aecode.gitee.io/aestate-doc](https://aecode.gitee.io/aestate-doc) >
 é¡¹ç®ä½ç³»ç»æ: [aecode.gitee.io/aestate](https://aecode.gitee.io/aestate/
 ) # åå³æ¡ä»¶ > Python >=3.6 (å¶ä»çæ¬æ²¡è¯è¿) >
-æç¨ææ¡£å°åï¼http://doc.cacode.ren # çæ¬è¯´æ
+æç¨ææ¡£å°åï¼~~http://doc.cacode.ren~~ http://aestate.angid.eu.org #
+çæ¬è¯´æ
 åºç¡éè¦2.7ä»¥ä¸çpythonçæ¬ï¼å¯¹äºåªéè¦æ§è¡sqlå¯ä»¥ä½¿ç¨2.7ä»¥ä¸ï¼ä¸å»ºè®®ï¼
 æä¼çåæ³æ¯ä½¿ç¨3.6ä»¥ä¸ï¼å¯ä»¥ä½¿ç¨ç»å¤§é¨ååè½
 ç±äº1.0.7å¢å å¼æ­¥æ¹æ³ï¼éè¦å¼æ­¥æ§è¡çå°ä¼ä¼´å¯ä»¥ä½¿ç¨python>=3.7.10ä»¥ä¸çæ¬
 # å®è£
 ç®åæºä»£ç ä»å¼æ¾å¨giteeï¼å¤äºç»ç»CACodeä¸ï¼ä»åºå°åä¸ºï¼
 [aestate](https://gitee.com/aecode/aestate)
 ä½¿ç¨pipæanacondaå®è£**Aestate**ï¼ ```shell pip install aestate conda
```

### Comparing `Aestate-1.0.9/README.md` & `Aestate-1.0.9a1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         <result field="d1_name" properties="name"/>
         <result field="d1_password" properties="password"/>
         <foreign type="example.table.demoModels.Demo" name="demoJoin">
             <result field="d2_id" properties="id"/>
             <result field="d2_name" properties="name"/>
             <result field="d2_password" properties="password"/>
         </foreign>
+        <foreign ref="demoJoin" single="false"/>
     </resultMap>
     <item id="findAllById">
         <select resultType="resultMapLeftJoin">
             SELECT
             <!-- 导入查询的字段 -->
             <!--            <include from="templateField"/>-->
             <include from="tempSymbol"/>
@@ -99,48 +100,44 @@
 
 - 其次就是在兼容性方面，由于这个世界上的数据库种类太多了没办法做到统一， **Aestate**保留了对其他小众数据库的实现接口，尽可能多兼容数据库。
 
 - 数据库表方面，Django是会生成数据django自己系统内部的表，在迁移的时候呢如果做错一步可能对于新手
   来讲后面的修复操作是极其难的，也未必能够在短时间内定位问题并修复。**Aestate**为了解决这个问题，将make
   和手动建表尽可能的兼容，不会生成额外的表和数据，也不会捆绑某个特定系统，将pojo/model复制出来可以直接为下一个项目使用。
 
-- 缓存方面参考了Mybatis的实现方法并略微修改，**Aestate**有两个内存管理模块，用于保证数据的完整性，
+- ~~缓存方面参考了Mybatis的实现方法并略微修改，**Aestate**有两个内存管理模块，用于保证数据的完整性，
   当一些特别大的数据占满缓存时，**Aestate**
   会尽量多的去分配内存保证数据完整性，除外才会去管理内存（不建议操作大于系统内存2/10的数据）。**Aestate**
-  有弹性内存管理方式，会根据系统的执行自动调整缓存大小，尽可能的加快运行速度，减少对数据库的连接次数。
+  有弹性内存管理方式，会根据系统的执行自动调整缓存大小，尽可能的加快运行速度，减少对数据库的连接次数。~~（最新1.0.9已删除缓存策略）
 
 - 自带日志和美化，不需要下载其他插件就可以把日志变色，自动保存日志，这个功能对于爱美的大兄弟简直就 是神仙般的存在（当然也可能只有我喜欢装逼）
 
 
 - 还有很多......
 
 > 寻找志同道合的朋友一起开发**Aestate**  
 > 作者QQ:2075383131(云)  
 > qq群：909044439(Aestate Framework)
 
 # 关于教程和文档地址
 
-因为开发aestate的同学大部分都是来自各地的`穷学生`,我已经没有办法支付的起下一年的服务器费用（508.02元）， 因为这是我`63%`
-的生活费。
-
-以后教程和文档更新依靠CSDN、OSCHINA、知乎、bilibili以及各位捐献云服务器和托管平台等
+文档已经迁移到免费托管平台：http://aestate.angid.eu.org
 
 > csdn: [AECODE](https://blog.csdn.net/qq_43059459)  
 > OSCHINA: [CACode](https://my.oschina.net/u/4841054)  
-> 知乎: [CACode](https://www.zhihu.com/people/ben-ren-pin-kun-seng)  
 > bilibili大学堂: [你在写臭虫?](https://space.bilibili.com/371089110)  
-> 官网域名: [cacode.ren](https://cacode.ren)  
-> 文档官网域名: [doc.cacode.ren](https://doc.cacode.ren)  
+> 官网域名: [cacode.ren](https://cacode.ren)（迁移到腾讯云没备案）  
+> 文档官网域名: [~~doc.cacode.ren~~](https://doc.cacode.ren)&nbsp;[http://aestate.angid.eu.org](http://aestate.angid.eu.org)  
 > Gitee官方: [https://aecode.gitee.io/aestate-doc](https://aecode.gitee.io/aestate-doc)  
 > 项目体系结构: [aecode.gitee.io/aestate](https://aecode.gitee.io/aestate/)
 
 # 先决条件
 
 > Python >=3.6 (其他版本没试过)  
-> 教程文档地址：http://doc.cacode.ren
+> 教程文档地址：~~http://doc.cacode.ren~~&nbsp;http://aestate.angid.eu.org
 
 # 版本说明
 
 基础需要2.7以上的python版本，对于只需要执行sql可以使用2.7以上（不建议）
 
 最优的办法是使用3.6以上，可以使用绝大部分功能
```

#### html2text {}

```diff
@@ -16,37 +16,36 @@
 å¶æ¬¡å°±æ¯å¨å¼å®¹æ§æ¹é¢ï¼ç±äºè¿ä¸ªä¸çä¸çæ°æ®åºç§ç±»å¤ªå¤äºæ²¡åæ³åå°ç»ä¸ï¼
 **Aestate**ä¿çäºå¯¹å¶ä»å°ä¼æ°æ®åºçå®ç°æ¥å£ï¼å°½å¯è½å¤å¼å®¹æ°æ®åºã
 -
 æ°æ®åºè¡¨æ¹é¢ï¼Djangoæ¯ä¼çææ°æ®djangoèªå·±ç³»ç»åé¨çè¡¨ï¼å¨è¿ç§»çæ¶åå¢å¦æåéä¸æ­¥å¯è½å¯¹äºæ°æ
 æ¥è®²åé¢çä¿®å¤æä½æ¯æå¶é¾çï¼ä¹æªå¿è½å¤å¨ç­æ¶é´åå®ä½é®é¢å¹¶ä¿®å¤ã**Aestate**ä¸ºäºè§£å³è¿ä¸ªé®é¢ï¼å°make
 åæå¨å»ºè¡¨å°½å¯è½çå¼å®¹ï¼ä¸ä¼çæé¢å¤çè¡¨åæ°æ®ï¼ä¹ä¸ä¼æç»æä¸ªç¹å®ç³»ç»ï¼å°pojo/
 modelå¤å¶åºæ¥å¯ä»¥ç´æ¥ä¸ºä¸ä¸ä¸ªé¡¹ç®ä½¿ç¨ã -
-ç¼å­æ¹é¢åèäºMybatisçå®ç°æ¹æ³å¹¶ç¥å¾®ä¿®æ¹ï¼**Aestate**æä¸¤ä¸ªåå­ç®¡çæ¨¡åï¼ç¨äºä¿è¯æ°æ®çå®æ´æ§ï¼
+~~ç¼å­æ¹é¢åèäºMybatisçå®ç°æ¹æ³å¹¶ç¥å¾®ä¿®æ¹ï¼**Aestate**æä¸¤ä¸ªåå­ç®¡çæ¨¡åï¼ç¨äºä¿è¯æ°æ®çå®æ´æ§ï¼
 å½ä¸äºç¹å«å¤§çæ°æ®å æ»¡ç¼å­æ¶ï¼**Aestate**
 ä¼å°½éå¤çå»åéåå­ä¿è¯æ°æ®å®æ´æ§ï¼é¤å¤æä¼å»ç®¡çåå­ï¼ä¸å»ºè®®æä½å¤§äºç³»ç»åå­2/
 10çæ°æ®ï¼ã**Aestate**
-æå¼¹æ§åå­ç®¡çæ¹å¼ï¼ä¼æ ¹æ®ç³»ç»çæ§è¡èªå¨è°æ´ç¼å­å¤§å°ï¼å°½å¯è½çå å¿«è¿è¡éåº¦ï¼åå°å¯¹æ°æ®åºçè¿æ¥æ¬¡æ°ã
+æå¼¹æ§åå­ç®¡çæ¹å¼ï¼ä¼æ ¹æ®ç³»ç»çæ§è¡èªå¨è°æ´ç¼å­å¤§å°ï¼å°½å¯è½çå å¿«è¿è¡éåº¦ï¼åå°å¯¹æ°æ®åºçè¿æ¥æ¬¡æ°ã~~ï¼ææ°1.0.9å·²å é¤ç¼å­ç­ç¥ï¼
 -
 èªå¸¦æ¥å¿åç¾åï¼ä¸éè¦ä¸è½½å¶ä»æä»¶å°±å¯ä»¥ææ¥å¿åè²ï¼èªå¨ä¿å­æ¥å¿ï¼è¿ä¸ªåè½å¯¹äºç±ç¾çå¤§åå¼ç®ç´å°±
 æ¯ç¥ä»è¬çå­å¨ï¼å½ç¶ä¹å¯è½åªææåæ¬¢è£é¼ï¼ -
 è¿æå¾å¤...... > å¯»æ¾å¿åéåçæåä¸èµ·å¼å**Aestate** >
 ä½èQQ:2075383131(äº) > qqç¾¤ï¼909044439(Aestate Framework) #
-å³äºæç¨åææ¡£å°å
-å ä¸ºå¼åaestateçåå­¦å¤§é¨åé½æ¯æ¥èªåå°ç`ç©·å­¦ç`,æå·²ç»æ²¡æåæ³æ¯ä»çèµ·ä¸ä¸å¹´çæå¡å¨è´¹ç¨ï¼508.02åï¼ï¼
-å ä¸ºè¿æ¯æ`63%` ççæ´»è´¹ã
-ä»¥åæç¨åææ¡£æ´æ°ä¾é CSDNãOSCHINAãç¥ä¹ãbilibiliä»¥ååä½æç®äºæå¡å¨åæç®¡å¹³å°ç­
-> csdn: [AECODE](https://blog.csdn.net/qq_43059459) > OSCHINA: [CACode](https:/
-/my.oschina.net/u/4841054) > ç¥ä¹: [CACode](https://www.zhihu.com/people/ben-
-ren-pin-kun-seng) > bilibiliå¤§å­¦å : [ä½ å¨åè­è«?](https://
-space.bilibili.com/371089110) > å®ç½åå: [cacode.ren](https://cacode.ren)
-> ææ¡£å®ç½åå: [doc.cacode.ren](https://doc.cacode.ren) > Giteeå®æ¹:
-[https://aecode.gitee.io/aestate-doc](https://aecode.gitee.io/aestate-doc) >
+å³äºæç¨åææ¡£å°å ææ¡£å·²ç»è¿ç§»å°åè´¹æç®¡å¹³å°ï¼http://
+aestate.angid.eu.org > csdn: [AECODE](https://blog.csdn.net/qq_43059459) >
+OSCHINA: [CACode](https://my.oschina.net/u/4841054) > bilibiliå¤§å­¦å :
+[ä½ å¨åè­è«?](https://space.bilibili.com/371089110) > å®ç½åå:
+[cacode.ren](https://cacode.ren)ï¼è¿ç§»å°è¾è®¯äºæ²¡å¤æ¡ï¼ >
+ææ¡£å®ç½åå: [~~doc.cacode.ren~~](https://doc.cacode.ren) [http://
+aestate.angid.eu.org](http://aestate.angid.eu.org) > Giteeå®æ¹: [https://
+aecode.gitee.io/aestate-doc](https://aecode.gitee.io/aestate-doc) >
 é¡¹ç®ä½ç³»ç»æ: [aecode.gitee.io/aestate](https://aecode.gitee.io/aestate/
 ) # åå³æ¡ä»¶ > Python >=3.6 (å¶ä»çæ¬æ²¡è¯è¿) >
-æç¨ææ¡£å°åï¼http://doc.cacode.ren # çæ¬è¯´æ
+æç¨ææ¡£å°åï¼~~http://doc.cacode.ren~~ http://aestate.angid.eu.org #
+çæ¬è¯´æ
 åºç¡éè¦2.7ä»¥ä¸çpythonçæ¬ï¼å¯¹äºåªéè¦æ§è¡sqlå¯ä»¥ä½¿ç¨2.7ä»¥ä¸ï¼ä¸å»ºè®®ï¼
 æä¼çåæ³æ¯ä½¿ç¨3.6ä»¥ä¸ï¼å¯ä»¥ä½¿ç¨ç»å¤§é¨ååè½
 ç±äº1.0.7å¢å å¼æ­¥æ¹æ³ï¼éè¦å¼æ­¥æ§è¡çå°ä¼ä¼´å¯ä»¥ä½¿ç¨python>=3.7.10ä»¥ä¸çæ¬
 # å®è£
 ç®åæºä»£ç ä»å¼æ¾å¨giteeï¼å¤äºç»ç»CACodeä¸ï¼ä»åºå°åä¸ºï¼
 [aestate](https://gitee.com/aecode/aestate)
 ä½¿ç¨pipæanacondaå®è£**Aestate**ï¼ ```shell pip install aestate conda
```

### Comparing `Aestate-1.0.9/aestate/ajson/ajson.py` & `Aestate-1.0.9a1/aestate/ajson/ajson.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/base/anno.py` & `Aestate-1.0.9a1/aestate/base/anno.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/base/manage.py` & `Aestate-1.0.9a1/aestate/base/manage.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/base/model.py` & `Aestate-1.0.9a1/aestate/base/model.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/base/proxy.py` & `Aestate-1.0.9a1/aestate/base/proxy.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/dbs/_mssql/__init__.py` & `Aestate-1.0.9a1/aestate/dbs/_mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/dbs/_mysql/__init__.py` & `Aestate-1.0.9a1/aestate/dbs/_mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/dbs/_mysql/tag.py` & `Aestate-1.0.9a1/aestate/dbs/_mysql/tag.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/exception/__init__.py` & `Aestate-1.0.9a1/aestate/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/i18n/__init__.py` & `Aestate-1.0.9a1/aestate/i18n/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import threading
 
 from aestate.work.Modes import Singleton
 
 
 class AestateLanguage:
+    """
+    0x804：中文
+    0x409：英文
+    """
     LANG = 0x804
 
 
 class I18n:
     """
     国际化语言,在统一配置下的全局语言解决方案
     """
@@ -54,29 +58,33 @@
             0x804: {
                 '': '未知错误',
                 'if_tag_not_test': 'if 标记中的属性`test` 缺少必需的结构',
                 'xml_syntax_error': 'xml语法错误,不相等的逻辑运算符数量,在:%s',
                 'before_else_not_if': '在 else 标签前面找不到 if 标签',
                 'not_field_name': '被调用的方法中不存在名为 `%s` 的参数',
                 'not_from_node_name': '无法从节点中找到名为 `%s` 的模板',
-                'not_result_map': "找不到 resultMap 模板",
-                "not_type": "无法从节点中找到名为 `type` 的属性",
-                "module_not_found": "模块未找到",
+                'not_result_map': "找不到名为 `%s` 的 resultMap 模板",
+                "result_map_not_type": "无法从节点中找到名为“type”的属性",
+                "module_not_found": "模块 `%s` 未找到",
+                "lack_result_type": "缺少resultType",
+                "not_defined": "找不到定义 `%s`"
             },
             # 英语
             0x409: {
                 '': 'Unknow error',
                 'if_tag_not_test': 'The attribute`test` in the if tag is missing a required structure',
                 'xml_syntax_error': 'Xml syntax error, unequal number of logical operators, from:%s',
                 'before_else_not_if': 'Cannot find the if tag in front of the else tag',
                 'not_field_name': 'The parameter named `%s` does not exist in the called method',
                 'not_from_node_name': 'The template named `%s` could not be found from the node',
-                'not_result_map': "Can't find resultMap template",
-                "not_type": "The attribute named `type` could not be found from the node",
-                "module_not_found": "`%s` Module Not Found",
+                'not_result_map': "ResultMap template named '%s' could not be found",
+                "result_map_not_type": "The attribute named `type` could not be found from the node",
+                "module_not_found": "`%s` Module `%s` Not Found",
+                "lack_result_type": "`%s` Lack result type",
+                "not_defined": "Can't find the defined `%s`"
             },
         })
 
     @staticmethod
     def tt(name):
         return ExceptionI18n().t(name)
```

### Comparing `Aestate-1.0.9/aestate/util/CompulsoryRun.py` & `Aestate-1.0.9a1/aestate/util/CompulsoryRun.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/util/Log.py` & `Aestate-1.0.9a1/aestate/util/Log.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/util/others.py` & `Aestate-1.0.9a1/aestate/util/others.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/util/sqlOpera.py` & `Aestate-1.0.9a1/aestate/util/sqlOpera.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/work/Adapter.py` & `Aestate-1.0.9a1/aestate/work/Adapter.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/work/Annotation.py` & `Aestate-1.0.9a1/aestate/work/Annotation.py`

 * *Files 6% similar despite different names*

```diff
@@ -240,14 +240,16 @@
 
     return set_to_field
 
 
 def Item(_id, d=False):
     """
     将xml的item节点映射到当前方法,对应的id字段为xml节点的id
+    :param _id: 节点id
+    :param d: 查询时返回原始数据
     """
 
     def replaceNextLine(sql):
         sql = str(sql).replace('\n', ' ')
         sql = str(sql).replace('  ', ' ')
         if '  ' in sql:
             return replaceNextLine(sql)
@@ -257,15 +259,21 @@
     def base_func(cls):
         def _wrapper_(*args, **kwargs):
             lines = list(args)
             obj = lines[0]
             xml = obj.xNode
 
             xml_node = None
-            for v in xml.children['item']:
+            # 增删改查的节点加起来得到所有操作节点
+            node_list = xml.children['select'] \
+                        + xml.children['insert'] \
+                        + xml.children['update'] \
+                        + xml.children['delete']
+            # 从所有的可操作节点中寻找id符合的节点
+            for v in node_list:
                 if 'id' in v.attrs.keys() and v.attrs['id'].text == _id:
                     xml_node = v
                     break
             if xml_node is not None:
                 xml_node.params = kwargs
                 result_text_node = xml_node.text(obj)
             else:
@@ -278,23 +286,28 @@
                 ALog.log_error(
                     f"`The node did not return any sentences.file:({obj._xml_file_name})", obj=TagHandlerError,
                     raise_exception=True)
                 return None
             run_sql = replaceNextLine(result_text_node.text)
             sub_sql, params = TextUtil.replace_antlr(run_sql, **kwargs)
             # 返回值ast
-            if 'resultType' in result_text_node.mark.keys():
+            if xml_node.node.tagName.lower() == 'select':
                 result = obj.execute_sql(sql=sub_sql, params=params, mode=EX_MODEL.SELECT, **obj.__dict__)
+                # 将返回的结果解析
                 resultTree = ResultMapNode(obj, result_text_node, result)
                 if d:
                     return result
-                return resultTree.apply()
+                return resultTree.apply(xml.children['resultMap'])
             else:
+                # 是否需要返回最后一行id，默认返回
+                has_last_id = bool(result_text_node.expand_data['last']) \
+                    if 'last' in result_text_node.expand_data.keys() else True
+
                 result = obj.execute_sql(sql=sub_sql, params=params, mode=EX_MODEL.UPDATE,
-                                         **{'last_id': result_text_node.mark['has_last_id'], **obj.__dict__})
+                                         **{'last_id': has_last_id, **obj.__dict__})
                 return result
 
         return _wrapper_
 
     return base_func
```

### Comparing `Aestate-1.0.9/aestate/work/AopContainer.py` & `Aestate-1.0.9a1/aestate/work/AopContainer.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/work/Cache.py` & `Aestate-1.0.9a1/aestate/work/Cache.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/work/Config.py` & `Aestate-1.0.9a1/aestate/work/Config.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/work/Manage.py` & `Aestate-1.0.9a1/aestate/work/Manage.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/work/Modes.py` & `Aestate-1.0.9a1/aestate/work/Modes.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/work/Serialize.py` & `Aestate-1.0.9a1/aestate/work/Serialize.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/work/commands/__init__.py` & `Aestate-1.0.9a1/aestate/work/commands/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- utf-8 -*-
 # encoding:utf-8
 # @Time: 2021/6/27 20:47
 # @Author: CACode
 # 版本有三种状态 正式版从1.0.0往后逐个加 1,对应版本的补丁为'a+补丁次数'
-__version__ = '1.0.9'
+__version__ = '1.0.9a1'
 __description__ = "Aestate framework for Python,You can see:https://gitee.com/aecode/aestate"
 __author__ = "CACode"
 __author_email__ = "cacode@163.com"
 __url__ = "https://gitee.com/aecode/aestate"
 __issues__ = 'https://gitee.com/aecode/aestate/issues'
 __license__ = 'Apache License 2.0'
 __project_name__ = 'Aestate'
```

### Comparing `Aestate-1.0.9/aestate/work/orm.py` & `Aestate-1.0.9a1/aestate/work/orm.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/work/proxy/SqlOperaProxy.py` & `Aestate-1.0.9a1/aestate/work/proxy/SqlOperaProxy.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/work/repository.py` & `Aestate-1.0.9a1/aestate/work/repository.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/work/sql/ExecuteSql.py` & `Aestate-1.0.9a1/aestate/work/sql/ExecuteSql.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/work/sql/ProxyOpera.py` & `Aestate-1.0.9a1/aestate/work/sql/ProxyOpera.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/work/xmlhandler/XMLScriptBuilder.py` & `Aestate-1.0.9a1/aestate/work/xmlhandler/XMLScriptBuilder.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.9/aestate/work/xmlhandler/base.py` & `Aestate-1.0.9a1/aestate/work/xmlhandler/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,29 +26,24 @@
 
 
 class AestateNode(list):
     def __init__(self, root, node):
         list.__init__([])
         self.root = root
         self.node = node
-        # 给定一个标记，让剩下的标签允许存放信息
-        self.mark = {}
+        # 给定一个拓展，让剩下的标签允许存放信息
+        self.expand_data = {k: v.text for k, v in
+                            parse_attributes(node.attributes if hasattr(node, 'attributes') else node.attrs).items()}
 
     def add(self, node, index) -> None:
         self.append(TextNode(self.root, node, index))
 
     @property
     def text(self):
         texts = [i.text for i in self]
-        # for i, v in enumerate(arr):
-        #     if v.node.nodeName in XML_KEY.keys():
-        #         obj = XML_KEY[v.node.nodeName](v)
-        #         texts.append(obj.pure_str(XML_KEY))
-        #     elif v.node.nodeName in XML_TEXT_NODE:
-        #         texts.append(v.node.data)
         return ' '.join(texts)
 
     def __str__(self) -> str:
         return self.text
 
 
 def parse_attributes(attr):
```

### Comparing `Aestate-1.0.9/aestate/work/xmlhandler/nodes.py` & `Aestate-1.0.9a1/aestate/work/xmlhandler/nodes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # -*- utf-8 -*-
 import importlib
 import re
 from abc import ABC
 
 from aestate.exception import NotFindTemplateError, TagAttributeError, TagHandlerError, XmlParseError
 from aestate.i18n import ExceptionI18n
+from aestate.util import others
 from aestate.util.Log import ALog
 from aestate.work.Serialize import QuerySet
+from aestate.work.repository import Repository
 from aestate.work.xmlhandler.XMLScriptBuilder import IfHandler
 from aestate.work.xmlhandler.base import AestateNode
 
 
 class AbstractNode(ABC):
     """抽象节点，所有节点的父类"""
 
@@ -55,30 +57,29 @@
 
     def apply(self, *args, **kwargs):
         # 取得已有的文本
         texts = kwargs['texts']
         axc_node = self.aestate_xml_cls(self.root, self.node, self.params)
         # 返回值类型
         resultType = axc_node.attrs['resultType']
-        texts.mark['resultType'] = resultType.text
         return self.parseNode(texts, self.node)
 
 
 class UpdateNode(AbstractNode):
     class TempTextNode:
         def __init__(self, text):
             self.text = text
 
     def apply(self, *args, **kwargs):
         # 取得已有的文本
         texts = kwargs['texts']
         axc_node = self.aestate_xml_cls(self.root, self.node, self.params)
         # 返回值类型
         has_last_id = axc_node.attrs['last'] if 'last' in axc_node.attrs.keys() else self.TempTextNode('True')
-        texts.mark['has_last_id'] = has_last_id.text == 'True'
+        texts.expand_data['has_last_id'] = has_last_id.text == 'True'
         return self.parseNode(texts, self.node)
 
 
 class IfNode(AbstractNode):
 
     def conditional_test(self, text, syntax_re_text):
         # 移除空集
@@ -104,15 +105,15 @@
 
     def signal_conditional_test(self, text, field):
         """单个判断值对否"""
         rfield = re.findall('#{(.*?)}', field)
         if len(rfield) == 1 and rfield[0] not in self.params.keys():
             # 这里理应等于false,但是由于存在不等号,所以当没有时他应该为!false,也就是true
             return True
-        return not bool(self.params[rfield])
+        return not bool(self.params[rfield[0]])
 
     def apply(self, *args, **kwargs):
         texts = kwargs['texts']
         axc_node = self.aestate_xml_cls(self.root, self.node, self.params)
         if 'test' not in axc_node.attrs.keys():
             ALog.log_error(
                 msg=ExceptionI18n.tt('if_tag_not_test'),
@@ -136,15 +137,15 @@
             # 一种是 字段-符号-值
             syntax_re_text = re.findall('(#\{.*?\})([>=|<=|==|<|>|!=]+)(.*)', text)
             # 一种是 符号-空格(可有可无)-字段
             signal_syntax_re_text = re.findall('!\s*(#\{.*?\})', text)
             if len(syntax_re_text) != 0:
                 success = self.conditional_test(text, syntax_re_text)
             elif len(signal_syntax_re_text) == 1:
-                success = self.signal_conditional_test(text, signal_syntax_re_text[0])
+                success = self.signal_conditional_test(text[0], signal_syntax_re_text[0])
             else:
                 # 缺少必要的test标签语法
                 ALog.log_error(
                     msg=ExceptionI18n.tt('xml_syntax_error') % test_syntax.text,
                     obj=TagAttributeError, LogObject=self.target_obj.log_obj, raise_exception=True)
 
             if len(conditions) > 0:
@@ -169,34 +170,34 @@
             if not if_next:
                 break
         if if_next:
             texts = self.parseNode(texts, node=self.node)
 
         if IfHandler.checking_mark(self.node):
             # 设置为反的
-            texts.mark['if_next'] = not if_next
+            texts.expand_data['if_next'] = not if_next
 
         return texts
 
 
 class ElseNode(AbstractNode):
 
     def apply(self, *args, **kwargs):
         texts = kwargs['texts']
-        if 'if_next' not in texts.mark.keys():
+        if 'if_next' not in texts.expand_data.keys():
             ALog.log_error(
                 msg=ExceptionI18n.tt('before_else_not_if'),
                 obj=TagHandlerError, LogObject=self.target_obj.log_obj, raise_exception=True)
         else:
-            if_next = texts.mark['if_next']
+            if_next = texts.expand_data['if_next']
             if not if_next:
-                texts.mark.pop('if_next')
+                texts.expand_data.pop('if_next')
                 return texts
             else:
-                texts.mark.pop('if_next')
+                texts.expand_data.pop('if_next')
                 return self.parseNode(texts, self.node)
 
 
 class SwitchNode(AbstractNode):
 
     def apply(self, *args, **kwargs):
         texts = kwargs['texts']
@@ -223,60 +224,81 @@
 
 class IncludeNode(AbstractNode):
 
     def apply(self, *args, **kwargs):
         texts = kwargs['texts']
         axc_node = self.aestate_xml_cls(self.root, self.node, self.params)
         from_node_name = axc_node.attrs['from'].text
-        templates = self.target_obj.xNode.children['template']
+        sql_nodes = self.target_obj.xNode.children['sql']
         target_template = None
-        for t in templates:
+        for t in sql_nodes:
             if t.attrs['id'].text == from_node_name:
                 target_template = t
                 break
         if target_template is None:
             ALog.log_error(
                 msg=ExceptionI18n.tt('not_from_node_name') % from_node_name,
                 obj=NotFindTemplateError, LogObject=self.target_obj.log_obj, raise_exception=True)
         texts = self.parseNode(texts, target_template.node)
         return texts
 
 
 class ResultABC(ABC):
     @staticmethod
-    def get_type(structure: dict):
-        t = structure['_type'].split('.')
+    def get_type(type_str: str):
+        t = type_str.split('.')
         cls_name = t[len(t) - 1]
         package_name = '.'.join(t[:len(t) - 1])
-        package = importlib.import_module(package_name)
-        _type = getattr(package, cls_name)
-        return _type
+        try:
+            package = importlib.import_module(package_name)
+            _type = getattr(package, cls_name)
+            return _type
+        except Exception:
+            ALog.log_error(
+                msg=ExceptionI18n.tt('module_not_found') % package_name,
+                obj=NotFindTemplateError, raise_exception=True)
 
     @staticmethod
     def generate(data: list, structure: dict):
         ret = []
         if not isinstance(data, list) and data is not None:
             data = [data]
         if data is not None:
             for _data_item in data:
-                obj = ResultABC.get_type(structure)(abst=True)
+                cls = ResultABC.get_type(structure['_type'])
+                if cls is None:
+                    ALog.log_error(
+                        msg=ExceptionI18n.tt('not_defined') % structure['_type'],
+                        obj=NotFindTemplateError, raise_exception=True)
+                # 判断是否是pojo,不同的类使用不同的方法获取字段
+                is_pojo = others.dp_equals_base(cls, Repository)
+                obj = cls(abst=True) if is_pojo else cls()
+                # obj = cls() if others.dp_equals_base(cls, object) else cls
                 for field, properties in structure.items():
                     if field != '_type' and field != '_single':
                         if isinstance(properties, dict):
-                            obj.add_field(field, ResultABC.generate(_data_item, properties))
+                            if is_pojo:
+                                obj.add_field(field, ResultABC.generate(_data_item, properties))
+                            else:
+                                setattr(obj, field, ResultABC.generate(_data_item, properties))
                             # obj.__append_field__
                             # setattr(obj, field, ResultABC.generate(_data_item, properties))
                         else:
                             # 布尔值替换
-                            obj_fields = obj.getFields()
-                            t = str(type(obj_fields[properties] if properties in obj_fields.keys() else object))
-                            fields_type = re.findall("\'.*\.(.*)\'", t)
-                            if 'boolField' in fields_type:
-                                _data_item[field] = bool(_data_item[field])
-                            obj.add_field(properties, _data_item[field])
+                            if is_pojo:
+                                obj_fields = obj.getFields()
+                                t = str(type(obj_fields[properties] if properties in obj_fields.keys() else object))
+                                fields_type = re.findall("\'.*\.(.*)\'", t)
+                                if 'boolField' in fields_type:
+                                    _data_item[field] = bool(_data_item[field])
+
+                                obj.add_field(properties, _data_item[field])
+                            else:
+                                setattr(obj, properties, _data_item[field])
+
                             # setattr(obj, properties, _data_item[field])
                 if '_single' in structure.keys() and structure['_single'] is True:
                     ret = obj
                 else:
                     ret.append(obj)
         else:
             if '_single' in structure.keys() and structure['_single'] is True:
@@ -292,42 +314,72 @@
 
 class ResultMapNode(object):
     def __init__(self, target_obj, node, data):
         self.target_obj = target_obj
         self.node = node
         self.data = data
 
-    def apply(self):
+    def apply(self, resultMaps):
         resultMapTags = self.target_obj.xNode.children['resultMap']
-        resultNode = None
-        for i in resultMapTags:
-            if i.attrs['id'].text == self.node.mark['resultType']:
-                # 这里不需要break，因为可以重复，取最后一位
-                resultNode = i
-
-        if resultNode is None:
+        if 'resultMap' in self.node.expand_data.keys():
+            resultType = self.node.expand_data['resultMap']
+            resultNode = None
+            for i in resultMapTags:
+                if i.attrs['id'].text == resultType:
+                    # 这里不需要break，因为可以重复，取最后一位
+                    resultNode = i
+            if resultNode is None:
+                ALog.log_error(
+                    msg=ExceptionI18n.tt('not_result_map') % resultType,
+                    obj=NotFindTemplateError, LogObject=self.target_obj.log_obj, raise_exception=True)
+            structure = ForeignNode.apply(resultNode, resultMaps)
+            return ResultABC.generate(self.data, structure)
+        elif 'resultType' in self.node.expand_data.keys():
+            resultType = self.node.expand_data['resultType']
+            # 由于使用resultType没有映射字段，所以使用原有的结构
+            obj = ResultABC.get_type(resultType)
+            # 获取类的字段
+            fields = others.get_static_fields(obj)
+            structure = {
+                '_type': resultType,
+                **{f: f for f in fields}
+            }
+            return ResultABC.generate(self.data, structure)
+        else:
             ALog.log_error(
-                msg=ExceptionI18n.tt('not_result_map'),
+                msg=ExceptionI18n.tt('lack_result_type') % self.node.expand_data['id'],
                 obj=NotFindTemplateError, LogObject=self.target_obj.log_obj, raise_exception=True)
-        structure = ForeignNode.apply(resultNode)
-        return ResultABC.generate(self.data, structure)
 
 
 class ForeignNode:
     @staticmethod
-    def apply(resultNode):
+    def apply(resultNode, resultMaps):
+        """
+        :params resultNode: resultMap节点
+        """
+        # 判断是否有引用ref
+        if 'ref' in resultNode.attrs:
+            result_map_match = None
+            for item in resultMaps:
+                if item.attrs['id'].text == resultNode.attrs['ref'].text:
+                    result_map_match = item
+                    break
+            if result_map_match is None:
+                ALog.log_error(
+                    msg=ExceptionI18n.tt('not_result_map') % resultNode.attrs['ref'].text,
+                    obj=TagAttributeError, raise_exception=True)
+            else:
+                resultNode = result_map_match
+        # 判断结构是否有type返回值类型
         if 'type' not in resultNode.attrs.keys():
             ALog.log_error(
-                msg=ExceptionI18n.tt('not_type'),
+                msg=ExceptionI18n.tt('result_map_not_type'),
                 obj=TagAttributeError, raise_exception=True)
+
         structure = {'_type': resultNode.attrs['type'].text}
         if 'single' in resultNode.attrs.keys():
             structure['_single'] = True if resultNode.attrs['single'].text == 'true' else False
 
         if 'result' in resultNode.children.keys():
             for i in resultNode.children['result']:
-                structure[i.attrs['field'].text] = i.attrs['properties'].text
-
-        if 'foreign' in resultNode.children.keys():
-            for i in resultNode.children['foreign']:
-                structure[i.attrs['name'].text] = ForeignNode.apply(i)
+                structure[i.attrs['column'].text] = i.attrs['properties'].text
         return structure
```

### Comparing `Aestate-1.0.9/aestate/work/xmlhandler/utils.py` & `Aestate-1.0.9a1/aestate/work/xmlhandler/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,16 @@
     def __init__(self, root, node, params: None):
         self.root = root
         self.node = node
         self.params = params if params else {}
         self.children = parse_children(node, node.childNodes if hasattr(node, 'childNodes') else node.children, params)
         self.tags = {}
         self.attrs = parse_attributes(node.attributes if hasattr(node, 'attributes') else node.attrs)
-        self.resultType = None
 
     def text(self, target_obj):
-
         texts = AestateNode(self.root, self.node)
         for root_index, root_value in enumerate(self.node.childNodes):
             t = AestateNode(self.root, root_value)
             if root_value.nodeName in XML_KEY.keys():
                 obj = XML_KEY[root_value.nodeName](target_obj, self.params, AestateXml, self.root, root_value, XML_KEY,
                                                    XML_IGNORE_NODES)
                 texts = obj.apply(texts=texts)
```

### Comparing `Aestate-1.0.9/setup.py` & `Aestate-1.0.9a1/setup.py`

 * *Files identical despite different names*

