# Comparing `tmp/ayugespidertools-2.0.3.tar.gz` & `tmp/ayugespidertools-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayugespidertools-2.0.3.tar", max compression
+gzip compressed data, was "ayugespidertools-2.1.0.tar", max compression
```

## Comparing `ayugespidertools-2.0.3.tar` & `ayugespidertools-2.1.0.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-2.0.3/LICENSE
--rw-r--r--   0        0        0    13798 2023-04-27 03:19:49.000000 ayugespidertools-2.0.3/README.md
--rw-r--r--   0        0        0      482 2023-04-26 03:31:14.000000 ayugespidertools-2.0.3/ayugespidertools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-2.0.3/ayugespidertools/commands/__init__.py
--rw-r--r--   0        0        0      158 2023-04-25 08:54:15.594268 ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      536 2023-04-25 08:55:28.881319 ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc
--rw-r--r--   0        0        0      685 2023-04-25 08:54:15.595268 ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc
--rw-r--r--   0        0        0     2860 2023-05-06 06:33:53.042068 ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc
--rw-r--r--   0        0        0     1086 2023-04-25 08:54:15.618268 ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/version.cpython-38.pyc
--rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-2.0.3/ayugespidertools/commands/crawl.py
--rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/commands/genspider.py
--rw-r--r--   0        0        0     4039 2023-05-06 06:32:50.000000 ayugespidertools-2.0.3/ayugespidertools/commands/startproject.py
--rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-2.0.3/ayugespidertools/commands/version.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/common/__init__.py
--rw-r--r--   0        0        0     3704 2023-04-21 05:52:41.000000 ayugespidertools-2.0.3/ayugespidertools/common/encryption.py
--rw-r--r--   0        0        0     6622 2023-04-25 02:55:24.000000 ayugespidertools-2.0.3/ayugespidertools/common/expend.py
--rw-r--r--   0        0        0     6885 2023-05-05 06:09:23.000000 ayugespidertools-2.0.3/ayugespidertools/common/mongodbpipe.py
--rw-r--r--   0        0        0    11765 2023-04-27 08:36:37.000000 ayugespidertools-2.0.3/ayugespidertools/common/multiplexing.py
--rw-r--r--   0        0        0    13474 2023-04-25 02:55:56.000000 ayugespidertools-2.0.3/ayugespidertools/common/mysqlerrhandle.py
--rw-r--r--   0        0        0    32707 2023-04-26 06:59:16.000000 ayugespidertools-2.0.3/ayugespidertools/common/params.py
--rw-r--r--   0        0        0     4264 2023-04-25 02:56:33.000000 ayugespidertools-2.0.3/ayugespidertools/common/spiderdbconf.py
--rw-r--r--   0        0        0     3726 2023-04-12 09:31:20.000000 ayugespidertools-2.0.3/ayugespidertools/common/sqlformat.py
--rw-r--r--   0        0        0     2368 2023-04-27 03:08:07.000000 ayugespidertools-2.0.3/ayugespidertools/common/typevars.py
--rw-r--r--   0        0        0    11325 2023-04-26 08:38:41.000000 ayugespidertools-2.0.3/ayugespidertools/common/utils.py
--rw-r--r--   0        0        0     3693 2023-04-25 02:57:48.000000 ayugespidertools-2.0.3/ayugespidertools/common/yidungap.py
--rw-r--r--   0        0        0      455 2023-04-13 07:37:35.000000 ayugespidertools-2.0.3/ayugespidertools/config.py
--rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-2.0.3/ayugespidertools/formatdata.py
--rw-r--r--   0        0        0     7681 2023-04-25 03:03:41.000000 ayugespidertools-2.0.3/ayugespidertools/imgoperation.py
--rw-r--r--   0        0        0     1934 2023-03-14 06:08:38.000000 ayugespidertools-2.0.3/ayugespidertools/items.py
--rw-r--r--   0        0        0      898 2023-04-24 02:31:51.000000 ayugespidertools-2.0.3/ayugespidertools/middlewares.py
--rw-r--r--   0        0        0     8550 2023-04-12 09:55:11.000000 ayugespidertools-2.0.3/ayugespidertools/mongoclient.py
--rw-r--r--   0        0        0     1140 2023-04-12 09:55:11.000000 ayugespidertools-2.0.3/ayugespidertools/mysqlclient.py
--rw-r--r--   0        0        0     5431 2023-04-25 03:03:58.000000 ayugespidertools-2.0.3/ayugespidertools/oss.py
--rw-r--r--   0        0        0      802 2023-05-04 09:14:56.000000 ayugespidertools-2.0.3/ayugespidertools/pipelines.py
--rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/processmanager.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-2.0.3/ayugespidertools/request.py
--rw-r--r--   0        0        0     2397 2023-04-12 09:55:11.000000 ayugespidertools-2.0.3/ayugespidertools/rpa.py
--rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/runjs.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/__init__.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/http/__init__.py
--rw-r--r--   0        0        0      356 2023-04-26 08:48:02.859698 ayugespidertools-2.0.3/ayugespidertools/scraper/http/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/http/request/__init__.py
--rw-r--r--   0        0        0     1442 2023-04-25 08:54:13.045266 ayugespidertools-2.0.3/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1068 2023-04-27 08:45:17.819120 ayugespidertools-2.0.3/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc
--rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/http/request/form.py
--rw-r--r--   0        0        0     1195 2023-04-24 02:25:23.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/__init__.py
--rw-r--r--   0        0        0      981 2023-04-25 08:58:10.179432 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2248 2023-04-25 08:58:10.180432 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc
--rw-r--r--   0        0        0     1742 2023-04-25 02:58:16.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/headers/ua.py
--rw-r--r--   0        0        0      374 2023-04-24 02:00:59.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/__init__.py
--rw-r--r--   0        0        0      475 2023-04-25 08:58:10.180432 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     7677 2023-04-27 07:35:53.380544 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/__pycache__/aiohttplib.cpython-38.pyc
--rw-r--r--   0        0        0     2200 2023-04-25 08:58:10.182432 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc
--rw-r--r--   0        0        0    10519 2023-04-27 07:35:00.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
--rw-r--r--   0        0        0     4331 2023-04-25 02:58:59.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/requestslib.py
--rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/__init__.py
--rw-r--r--   0        0        0      481 2023-04-25 08:58:10.183432 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3911 2023-04-25 08:58:10.184432 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc
--rw-r--r--   0        0        0     3056 2023-04-26 08:48:05.030700 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc
--rw-r--r--   0        0        0     7795 2023-04-25 08:58:10.186432 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc
--rw-r--r--   0        0        0     4228 2023-04-25 02:59:18.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/dynamic.py
--rw-r--r--   0        0        0     2876 2023-04-26 02:43:33.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/exclusive.py
--rw-r--r--   0        0        0    11201 2023-04-25 02:59:35.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/private.py
--rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/__init__.py
--rw-r--r--   0        0        0      885 2023-04-25 08:58:19.202438 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/download/file.py
--rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/download/image.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/__init__.py
--rw-r--r--   0        0        0      173 2023-04-25 08:58:19.202438 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2624 2023-05-05 08:55:33.703084 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/__pycache__/asynced.cpython-38.pyc
--rw-r--r--   0        0        0     2971 2023-05-05 08:55:33.673084 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc
--rw-r--r--   0        0        0     1820 2023-04-25 08:58:19.205438 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc
--rw-r--r--   0        0        0     2114 2023-05-05 07:48:47.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/asynced.py
--rw-r--r--   0        0        0     2872 2023-05-04 09:09:37.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/fantasy.py
--rw-r--r--   0        0        0     1356 2023-04-25 03:00:42.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/twisted.py
--rw-r--r--   0        0        0    13396 2023-04-25 03:01:05.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__init__.py
--rw-r--r--   0        0        0    11209 2023-04-25 08:58:19.207438 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4019 2023-05-05 08:55:33.680084 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/asynced.cpython-38.pyc
--rw-r--r--   0        0        0      717 2023-04-25 08:58:19.219438 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc
--rw-r--r--   0        0        0     1998 2023-05-04 07:33:52.883359 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc
--rw-r--r--   0        0        0     3619 2023-04-25 08:58:19.223438 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc
--rw-r--r--   0        0        0     4379 2023-05-05 08:25:40.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/asynced.py
--rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/fantasy.py
--rw-r--r--   0        0        0     1754 2023-04-25 03:01:24.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/stats.py
--rw-r--r--   0        0        0     2842 2023-05-04 02:07:52.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/turbo.py
--rw-r--r--   0        0        0     3794 2023-04-25 03:02:20.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/twisted.py
--rw-r--r--   0        0        0     6737 2023-04-25 03:02:38.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/spiders/__init__.py
--rw-r--r--   0        0        0     4569 2023-04-25 08:54:13.141266 ayugespidertools-2.0.3/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      760 2023-04-25 08:54:14.345267 ayugespidertools-2.0.3/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc
--rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/spiders/crawl.py
--rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-2.0.3/ayugespidertools/spiders.py
--rw-r--r--   0        0        0     2065 2023-03-28 09:33:33.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/.gitignore
--rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/README.md
--rw-r--r--   0        0        0      613 2023-04-25 05:46:03.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/VIT/.conf
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/__init__.py
--rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/items.py.tmpl
--rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/run.py.tmpl
--rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/run.sh.tmpl
--rw-r--r--   0        0        0     4093 2023-04-25 04:01:51.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/settings.py.tmpl
--rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/spiders/__init__.py
--rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/requirements.txt
--rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/scrapy.cfg
--rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-2.0.3/ayugespidertools/templates/spiders/async.tmpl
--rw-r--r--   0        0        0     6409 2023-04-25 08:46:25.000000 ayugespidertools-2.0.3/ayugespidertools/templates/spiders/basic.tmpl
--rw-r--r--   0        0        0     1941 2023-04-25 08:47:57.000000 ayugespidertools-2.0.3/ayugespidertools/templates/spiders/crawl.tmpl
--rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-2.0.3/ayugespidertools/templates/spiders/csvfeed.tmpl
--rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-2.0.3/ayugespidertools/templates/spiders/xmlfeed.tmpl
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-2.0.3/ayugespidertools/utils/__init__.py
--rw-r--r--   0        0        0      155 2023-04-25 08:55:31.774321 ayugespidertools-2.0.3/ayugespidertools/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5316 2023-05-06 06:33:52.862068 ayugespidertools-2.0.3/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc
--rw-r--r--   0        0        0     5909 2023-05-06 06:33:34.000000 ayugespidertools-2.0.3/ayugespidertools/utils/cmdline.py
--rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-2.0.3/ayugespidertools/verificationcode.py
--rw-r--r--   0        0        0     3135 2023-05-06 07:47:20.000000 ayugespidertools-2.0.3/pyproject.toml
--rw-r--r--   0        0        0    15541 1970-01-01 00:00:00.000000 ayugespidertools-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-2.1.0/LICENSE
+-rw-r--r--   0        0        0    13798 2023-04-27 03:19:49.000000 ayugespidertools-2.1.0/README.md
+-rw-r--r--   0        0        0      482 2023-04-26 03:31:14.000000 ayugespidertools-2.1.0/ayugespidertools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-2.1.0/ayugespidertools/commands/__init__.py
+-rw-r--r--   0        0        0      158 2023-04-25 08:54:15.594268 ayugespidertools-2.1.0/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      536 2023-04-25 08:55:28.881319 ayugespidertools-2.1.0/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc
+-rw-r--r--   0        0        0      685 2023-04-25 08:54:15.595268 ayugespidertools-2.1.0/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc
+-rw-r--r--   0        0        0     2860 2023-05-06 06:33:53.042068 ayugespidertools-2.1.0/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc
+-rw-r--r--   0        0        0     1086 2023-04-25 08:54:15.618268 ayugespidertools-2.1.0/ayugespidertools/commands/__pycache__/version.cpython-38.pyc
+-rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-2.1.0/ayugespidertools/commands/crawl.py
+-rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/commands/genspider.py
+-rw-r--r--   0        0        0     4039 2023-05-06 06:32:50.000000 ayugespidertools-2.1.0/ayugespidertools/commands/startproject.py
+-rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-2.1.0/ayugespidertools/commands/version.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/common/__init__.py
+-rw-r--r--   0        0        0     3704 2023-04-21 05:52:41.000000 ayugespidertools-2.1.0/ayugespidertools/common/encryption.py
+-rw-r--r--   0        0        0     6622 2023-04-25 02:55:24.000000 ayugespidertools-2.1.0/ayugespidertools/common/expend.py
+-rw-r--r--   0        0        0     6885 2023-05-05 06:09:23.000000 ayugespidertools-2.1.0/ayugespidertools/common/mongodbpipe.py
+-rw-r--r--   0        0        0    11765 2023-04-27 08:36:37.000000 ayugespidertools-2.1.0/ayugespidertools/common/multiplexing.py
+-rw-r--r--   0        0        0    13474 2023-04-25 02:55:56.000000 ayugespidertools-2.1.0/ayugespidertools/common/mysqlerrhandle.py
+-rw-r--r--   0        0        0    32707 2023-04-26 06:59:16.000000 ayugespidertools-2.1.0/ayugespidertools/common/params.py
+-rw-r--r--   0        0        0     4264 2023-04-25 02:56:33.000000 ayugespidertools-2.1.0/ayugespidertools/common/spiderdbconf.py
+-rw-r--r--   0        0        0     3726 2023-04-12 09:31:20.000000 ayugespidertools-2.1.0/ayugespidertools/common/sqlformat.py
+-rw-r--r--   0        0        0     2368 2023-04-27 03:08:07.000000 ayugespidertools-2.1.0/ayugespidertools/common/typevars.py
+-rw-r--r--   0        0        0    11325 2023-04-26 08:38:41.000000 ayugespidertools-2.1.0/ayugespidertools/common/utils.py
+-rw-r--r--   0        0        0     3693 2023-04-25 02:57:48.000000 ayugespidertools-2.1.0/ayugespidertools/common/yidungap.py
+-rw-r--r--   0        0        0      455 2023-04-13 07:37:35.000000 ayugespidertools-2.1.0/ayugespidertools/config.py
+-rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-2.1.0/ayugespidertools/formatdata.py
+-rw-r--r--   0        0        0     7681 2023-04-25 03:03:41.000000 ayugespidertools-2.1.0/ayugespidertools/imgoperation.py
+-rw-r--r--   0        0        0     1934 2023-03-14 06:08:38.000000 ayugespidertools-2.1.0/ayugespidertools/items.py
+-rw-r--r--   0        0        0      898 2023-04-24 02:31:51.000000 ayugespidertools-2.1.0/ayugespidertools/middlewares.py
+-rw-r--r--   0        0        0     8550 2023-04-12 09:55:11.000000 ayugespidertools-2.1.0/ayugespidertools/mongoclient.py
+-rw-r--r--   0        0        0     1140 2023-04-12 09:55:11.000000 ayugespidertools-2.1.0/ayugespidertools/mysqlclient.py
+-rw-r--r--   0        0        0     5431 2023-04-25 03:03:58.000000 ayugespidertools-2.1.0/ayugespidertools/oss.py
+-rw-r--r--   0        0        0      802 2023-05-09 03:25:16.000000 ayugespidertools-2.1.0/ayugespidertools/pipelines.py
+-rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/processmanager.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-2.1.0/ayugespidertools/request.py
+-rw-r--r--   0        0        0     2397 2023-04-12 09:55:11.000000 ayugespidertools-2.1.0/ayugespidertools/rpa.py
+-rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/runjs.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/http/__init__.py
+-rw-r--r--   0        0        0      356 2023-04-26 08:48:02.859698 ayugespidertools-2.1.0/ayugespidertools/scraper/http/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/http/request/__init__.py
+-rw-r--r--   0        0        0     1442 2023-04-25 08:54:13.045266 ayugespidertools-2.1.0/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1068 2023-04-27 08:45:17.819120 ayugespidertools-2.1.0/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc
+-rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/http/request/form.py
+-rw-r--r--   0        0        0     1195 2023-04-24 02:25:23.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/__init__.py
+-rw-r--r--   0        0        0      981 2023-04-25 08:58:10.179432 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2248 2023-04-25 08:58:10.180432 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc
+-rw-r--r--   0        0        0     1742 2023-04-25 02:58:16.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/headers/ua.py
+-rw-r--r--   0        0        0      374 2023-04-24 02:00:59.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/__init__.py
+-rw-r--r--   0        0        0      475 2023-04-25 08:58:10.180432 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7677 2023-04-27 07:35:53.380544 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/__pycache__/aiohttplib.cpython-38.pyc
+-rw-r--r--   0        0        0     2200 2023-04-25 08:58:10.182432 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc
+-rw-r--r--   0        0        0    10519 2023-04-27 07:35:00.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
+-rw-r--r--   0        0        0     4331 2023-04-25 02:58:59.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/requestslib.py
+-rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/__init__.py
+-rw-r--r--   0        0        0      481 2023-04-25 08:58:10.183432 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3911 2023-04-25 08:58:10.184432 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc
+-rw-r--r--   0        0        0     3056 2023-04-26 08:48:05.030700 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc
+-rw-r--r--   0        0        0     7795 2023-04-25 08:58:10.186432 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc
+-rw-r--r--   0        0        0     4228 2023-04-25 02:59:18.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/dynamic.py
+-rw-r--r--   0        0        0     2876 2023-04-26 02:43:33.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/exclusive.py
+-rw-r--r--   0        0        0    11201 2023-04-25 02:59:35.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/private.py
+-rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/__init__.py
+-rw-r--r--   0        0        0      885 2023-04-25 08:58:19.202438 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/download/file.py
+-rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/download/image.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/__init__.py
+-rw-r--r--   0        0        0      173 2023-04-25 08:58:19.202438 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2624 2023-05-05 08:55:33.703084 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/__pycache__/asynced.cpython-38.pyc
+-rw-r--r--   0        0        0     2971 2023-05-05 08:55:33.673084 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc
+-rw-r--r--   0        0        0     1820 2023-04-25 08:58:19.205438 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc
+-rw-r--r--   0        0        0     2114 2023-05-05 07:48:47.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/asynced.py
+-rw-r--r--   0        0        0     2872 2023-05-04 09:09:37.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/fantasy.py
+-rw-r--r--   0        0        0     1356 2023-04-25 03:00:42.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/twisted.py
+-rw-r--r--   0        0        0    13396 2023-04-25 03:01:05.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__init__.py
+-rw-r--r--   0        0        0    11209 2023-04-25 08:58:19.207438 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4205 2023-05-09 01:56:17.338129 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__pycache__/asynced.cpython-38.pyc
+-rw-r--r--   0        0        0      717 2023-04-25 08:58:19.219438 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc
+-rw-r--r--   0        0        0     1998 2023-05-04 07:33:52.883359 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc
+-rw-r--r--   0        0        0     3619 2023-04-25 08:58:19.223438 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc
+-rw-r--r--   0        0        0     4379 2023-05-05 08:25:40.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/asynced.py
+-rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/fantasy.py
+-rw-r--r--   0        0        0     1754 2023-04-25 03:01:24.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/stats.py
+-rw-r--r--   0        0        0     2842 2023-05-04 02:07:52.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/turbo.py
+-rw-r--r--   0        0        0     3794 2023-04-25 03:02:20.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/twisted.py
+-rw-r--r--   0        0        0     6737 2023-04-25 03:02:38.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0     4569 2023-04-25 08:54:13.141266 ayugespidertools-2.1.0/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      760 2023-04-25 08:54:14.345267 ayugespidertools-2.1.0/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc
+-rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-2.1.0/ayugespidertools/scraper/spiders/crawl.py
+-rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-2.1.0/ayugespidertools/spiders.py
+-rw-r--r--   0        0        0     2065 2023-03-28 09:33:33.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/.gitignore
+-rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/README.md
+-rw-r--r--   0        0        0      613 2023-04-25 05:46:03.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/VIT/.conf
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/__init__.py
+-rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/items.py.tmpl
+-rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/run.py.tmpl
+-rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/run.sh.tmpl
+-rw-r--r--   0        0        0     4093 2023-04-25 04:01:51.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/settings.py.tmpl
+-rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/module/spiders/__init__.py
+-rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/requirements.txt
+-rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-2.1.0/ayugespidertools/templates/project/scrapy.cfg
+-rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-2.1.0/ayugespidertools/templates/spiders/async.tmpl
+-rw-r--r--   0        0        0     6409 2023-04-25 08:46:25.000000 ayugespidertools-2.1.0/ayugespidertools/templates/spiders/basic.tmpl
+-rw-r--r--   0        0        0     1941 2023-04-25 08:47:57.000000 ayugespidertools-2.1.0/ayugespidertools/templates/spiders/crawl.tmpl
+-rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-2.1.0/ayugespidertools/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-2.1.0/ayugespidertools/templates/spiders/xmlfeed.tmpl
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-2.1.0/ayugespidertools/utils/__init__.py
+-rw-r--r--   0        0        0      155 2023-04-25 08:55:31.774321 ayugespidertools-2.1.0/ayugespidertools/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5350 2023-05-09 01:56:20.922134 ayugespidertools-2.1.0/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc
+-rw-r--r--   0        0        0     5943 2023-05-09 01:54:08.000000 ayugespidertools-2.1.0/ayugespidertools/utils/cmdline.py
+-rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-2.1.0/ayugespidertools/verificationcode.py
+-rw-r--r--   0        0        0     3135 2023-05-09 01:05:39.000000 ayugespidertools-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    15541 1970-01-01 00:00:00.000000 ayugespidertools-2.1.0/PKG-INFO
```

### Comparing `ayugespidertools-2.0.3/LICENSE` & `ayugespidertools-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/README.md` & `ayugespidertools-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/version.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/commands/__pycache__/version.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/commands/startproject.py` & `ayugespidertools-2.1.0/ayugespidertools/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/commands/version.py` & `ayugespidertools-2.1.0/ayugespidertools/commands/version.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/common/encryption.py` & `ayugespidertools-2.1.0/ayugespidertools/common/encryption.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/common/expend.py` & `ayugespidertools-2.1.0/ayugespidertools/common/expend.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/common/mongodbpipe.py` & `ayugespidertools-2.1.0/ayugespidertools/common/mongodbpipe.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/common/multiplexing.py` & `ayugespidertools-2.1.0/ayugespidertools/common/multiplexing.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/common/mysqlerrhandle.py` & `ayugespidertools-2.1.0/ayugespidertools/common/mysqlerrhandle.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/common/params.py` & `ayugespidertools-2.1.0/ayugespidertools/common/params.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/common/spiderdbconf.py` & `ayugespidertools-2.1.0/ayugespidertools/common/spiderdbconf.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/common/sqlformat.py` & `ayugespidertools-2.1.0/ayugespidertools/common/sqlformat.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/common/typevars.py` & `ayugespidertools-2.1.0/ayugespidertools/common/typevars.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/common/utils.py` & `ayugespidertools-2.1.0/ayugespidertools/common/utils.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/common/yidungap.py` & `ayugespidertools-2.1.0/ayugespidertools/common/yidungap.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/formatdata.py` & `ayugespidertools-2.1.0/ayugespidertools/formatdata.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/imgoperation.py` & `ayugespidertools-2.1.0/ayugespidertools/imgoperation.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/items.py` & `ayugespidertools-2.1.0/ayugespidertools/items.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/middlewares.py` & `ayugespidertools-2.1.0/ayugespidertools/middlewares.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/mongoclient.py` & `ayugespidertools-2.1.0/ayugespidertools/mongoclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/mysqlclient.py` & `ayugespidertools-2.1.0/ayugespidertools/mysqlclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/oss.py` & `ayugespidertools-2.1.0/ayugespidertools/oss.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/pipelines.py` & `ayugespidertools-2.1.0/ayugespidertools/pipelines.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/rpa.py` & `ayugespidertools-2.1.0/ayugespidertools/rpa.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/runjs.py` & `ayugespidertools-2.1.0/ayugespidertools/runjs.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/http/request/__init__.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/http/request/form.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/http/request/form.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/__init__.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/headers/ua.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/headers/ua.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/__pycache__/aiohttplib.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/__pycache__/aiohttplib.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/requestslib.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/netlib/requestslib.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/dynamic.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/dynamic.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/exclusive.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/exclusive.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/private.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/middlewares/proxy/private.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/__init__.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/download/file.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/download/file.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/download/image.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/download/image.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/__pycache__/asynced.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/__pycache__/asynced.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/asynced.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/asynced.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/fantasy.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/fantasy.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/twisted.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mongo/twisted.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__init__.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/asynced.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__pycache__/asynced.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri May  5 08:25:40 2023 UTC, .py size: 4379 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-00000000: 550d 0d0a 0000 0000 84bd 5464 1b11 0000  U.........Td....
+00000000: 550d 0d0a 0000 0000 37c5 5864 5412 0000  U.......7.XdT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6405 6406 6702 5a08 4700 6407 6406  ..d.d.g.Z.G.d.d.
 00000070: 8400 6406 6507 8303 5a09 4700 6408 6405  ..d.e...Z.G.d.d.
-00000080: 8400 6405 6507 8303 5a0a 6401 5300 2909  ..d.e...Z.d.S.).
+00000080: 8400 6405 650a 8303 5a0b 6401 5300 2909  ..d.e...Z.d.S.).
 00000090: e900 0000 004e 2901 da0e 5265 7573 654f  .....N)...ReuseO
 000000a0: 7065 7261 7469 6f6e 2901 da0b 546f 6f6c  peration)...Tool
 000000b0: 7346 6f72 4179 7529 01da 1041 7975 4d79  sForAyu)...AyuMy
 000000c0: 7371 6c50 6970 656c 696e 65da 1241 7379  sqlPipeline..Asy
 000000d0: 6e63 4d79 7371 6c50 6970 656c 696e 65da  ncMysqlPipeline.
 000000e0: 1841 7379 6e63 4e6f 726d 616c 4d79 7371  .AsyncNormalMysq
 000000f0: 6c50 6970 656c 696e 6563 0000 0000 0000  lPipelinec......
@@ -87,30 +87,30 @@
 00000560: 8302 a008 7c03 6403 1900 a101 7d06 7c05  ....|.d.....}.|.
 00000570: 6a09 7d07 7c00 6a0a 7c06 7c07 6404 8d02  j.}.|.j.|.|.d...
 00000580: 7d08 7c04 a00b 7c08 740c 7c07 a00d a100  }.|...|.t.|.....
 00000590: 8301 6405 1400 a102 4900 6400 4800 0100  ..d.....I.d.H...
 000005a0: 7c00 6a02 a00e a100 4900 6400 4800 0100  |.j.....I.d.H...
 000005b0: 5700 3500 5100 4900 6400 4800 5200 5800  W.5.Q.I.d.H.R.X.
 000005c0: 5700 3500 5100 4900 6400 4800 5200 5800  W.5.Q.I.d.H.R.X.
-000005d0: 7c01 5300 a906 4eda 0969 7465 6d5f 6d6f  |.S...N..item_mo
+000005d0: 7c01 5300 2906 4eda 0969 7465 6d5f 6d6f  |.S.).N..item_mo
 000005e0: 6465 da05 4d79 7371 6cda 0574 6162 6c65  de..Mysql..table
-000005f0: 2902 722a 0000 00da 0469 7465 6de9 0200  ).r*.....item...
+000005f0: 2902 7229 0000 00da 0469 7465 6de9 0200  ).r).....item...
 00000600: 0000 290f 7203 0000 00da 1563 6f6e 7665  ..).r......conve
 00000610: 7274 5f69 7465 6d73 5f74 6f5f 6469 6374  rt_items_to_dict
 00000620: 721c 0000 00da 0663 7572 736f 7272 2200  r......cursorr".
 00000630: 0000 da05 7375 7065 7272 0600 0000 da0c  ....superr......
 00000640: 6765 745f 6e65 775f 6974 656d da0e 6765  get_new_item..ge
 00000650: 745f 7461 626c 655f 6e61 6d65 da08 6e65  t_table_name..ne
 00000660: 775f 6974 656d da10 5f67 6574 5f73 716c  w_item.._get_sql
 00000670: 5f62 795f 6974 656d da07 6578 6563 7574  _by_item..execut
 00000680: 65da 0574 7570 6c65 da06 7661 6c75 6573  e..tuple..values
 00000690: da06 636f 6d6d 6974 2909 7212 0000 0072  ..commit).r....r
-000006a0: 2b00 0000 7213 0000 00da 0969 7465 6d5f  +...r......item_
-000006b0: 6469 6374 722e 0000 00da 0a61 6c74 6572  dictr......alter
-000006c0: 5f69 7465 6d72 2a00 0000 7232 0000 00da  _itemr*...r2....
+000006a0: 2a00 0000 7213 0000 00da 0969 7465 6d5f  *...r......item_
+000006b0: 6469 6374 722d 0000 00da 0a61 6c74 6572  dictr-.....alter
+000006c0: 5f69 7465 6d72 2900 0000 7231 0000 00da  _itemr)...r1....
 000006d0: 0373 716c a901 da09 5f5f 636c 6173 735f  .sql....__class_
 000006e0: 5f72 1400 0000 7215 0000 00da 0c70 726f  _r....r......pro
 000006f0: 6365 7373 5f69 7465 6d2a 0000 0073 1e00  cess_item*...s..
 00000700: 0000 0001 0a01 0c01 1401 1001 0a01 02ff  ................
 00000710: 0403 0a01 06ff 0403 0601 0e01 1e01 3001  ..............0.
 00000720: 7a25 4173 796e 634e 6f72 6d61 6c4d 7973  z%AsyncNormalMys
 00000730: 716c 5069 7065 6c69 6e65 2e70 726f 6365  qlPipeline.proce
@@ -122,131 +122,142 @@
 00000790: 7370 6964 6572 3b00 0000 7302 0000 0000  spider;...s.....
 000007a0: 017a 2641 7379 6e63 4e6f 726d 616c 4d79  .z&AsyncNormalMy
 000007b0: 7371 6c50 6970 656c 696e 652e 5f63 6c6f  sqlPipeline._clo
 000007c0: 7365 5f73 7069 6465 7263 0200 0000 0000  se_spiderc......
 000007d0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
 000007e0: 0000 7318 0000 007c 006a 00a0 01a1 0001  ..s....|.j......
 000007f0: 0074 02a0 037c 00a0 04a1 00a1 0153 0072  .t...|.......S.r
-00000800: 3e00 0000 2905 721c 0000 00da 0563 6c6f  >...).r......clo
-00000810: 7365 7202 0000 0072 0f00 0000 7240 0000  ser....r....r@..
+00000800: 3d00 0000 2905 721c 0000 00da 0563 6c6f  =...).r......clo
+00000810: 7365 7202 0000 0072 0f00 0000 723f 0000  ser....r....r?..
 00000820: 0072 1100 0000 7214 0000 0072 1400 0000  .r....r....r....
 00000830: 7215 0000 00da 0c63 6c6f 7365 5f73 7069  r......close_spi
 00000840: 6465 723e 0000 0073 0400 0000 0001 0a01  der>...s........
 00000850: 7a25 4173 796e 634e 6f72 6d61 6c4d 7973  z%AsyncNormalMys
 00000860: 716c 5069 7065 6c69 6e65 2e63 6c6f 7365  qlPipeline.close
-00000870: 5f73 7069 6465 72a9 0ada 085f 5f6e 616d  _spider....__nam
+00000870: 5f73 7069 6465 7229 0ada 085f 5f6e 616d  _spider)...__nam
 00000880: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
 00000890: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
 000008a0: 5f64 6f63 5f5f 7216 0000 0072 1000 0000  _doc__r....r....
-000008b0: 723d 0000 0072 4000 0000 7242 0000 00da  r=...r@...rB....
+000008b0: 723c 0000 0072 3f00 0000 7241 0000 00da  r<...r?...rA....
 000008c0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7214  .__classcell__r.
-000008d0: 0000 0072 1400 0000 723b 0000 0072 1500  ...r....r;...r..
+000008d0: 0000 0072 1400 0000 723a 0000 0072 1500  ...r....r:...r..
 000008e0: 0000 7206 0000 000f 0000 0073 0c00 0000  ..r........s....
 000008f0: 0801 0404 0808 080e 0c11 0803 6300 0000  ............c...
-00000900: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00000910: 0000 0000 0073 4000 0000 6500 5a01 6400  .....s@...e.Z.d.
+00000900: 0000 0000 0000 0000 0000 0000 0002 0000  ................
+00000910: 0040 0000 0073 3800 0000 6500 5a01 6400  .@...s8...e.Z.d.
 00000920: 5a02 6401 5a03 6402 6403 8400 5a04 6404  Z.d.Z.d.d...Z.d.
-00000930: 6405 8400 5a05 8700 6601 6406 6407 8408  d...Z...f.d.d...
-00000940: 5a06 6408 6409 8400 5a07 640a 640b 8400  Z.d.d...Z.d.d...
-00000950: 5a08 8700 0400 5a09 5300 290c 7205 0000  Z.....Z.S.).r...
-00000960: 0075 4e00 0000 0a20 2020 20e9 809a e8bf  .uN....    .....
-00000970: 8720 6169 6f6d 7973 716c 20e5 ae9e e78e  . aiomysql .....
-00000980: b0e5 bc82 e6ad a5e5 8699 e585 a520 4d79  ............. My
-00000990: 7371 6c20 e695 b0e6 8dae e5ba 93e7 9a84  sql ............
-000009a0: e8bf 9ee6 8ea5 e6b1 a0e7 8988 e69c ac0a  ................
-000009b0: 2020 2020 6302 0000 0000 0000 0000 0000      c...........
-000009c0: 0002 0000 0005 0000 0043 0000 0073 4200  .........C...sB.
-000009d0: 0000 7400 7c01 6401 8302 7312 7401 6402  ..t.|.d...s.t.d.
-000009e0: 8301 8201 7c01 6a02 7c00 5f02 7c01 6a03  ....|.j.|._.|.j.
-000009f0: 7c00 5f03 7404 6a05 7c01 6a03 6403 8d01  |._.t.j.|.j.d...
-00000a00: 7c00 5f06 7407 a008 7c00 a009 7c01 a101  |._.t...|...|...
-00000a10: a101 5300 7207 0000 0072 0900 0000 7211  ..S.r....r....r.
-00000a20: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
-00000a30: 0000 7216 0000 0048 0000 0073 0a00 0000  ..r....H...s....
-00000a40: 0001 1202 0801 0801 1001 7a1e 4173 796e  ..........z.Asyn
-00000a50: 634d 7973 716c 5069 7065 6c69 6e65 2e6f  cMysqlPipeline.o
-00000a60: 7065 6e5f 7370 6964 6572 6302 0000 0000  pen_spiderc.....
-00000a70: 0000 0000 0000 0002 0000 000c 0000 00c3  ................
-00000a80: 0000 0073 4400 0000 7400 6a01 7c00 6a02  ...sD...t.j.|.j.
-00000a90: 6a03 7c00 6a02 6a04 7c00 6a02 6a05 7c00  j.|.j.j.|.j.j.|.
-00000aa0: 6a02 6a06 7c00 6a02 6a07 7c00 6a02 6a08  j.j.|.j.j.|.j.j.
-00000ab0: 7400 6a09 6401 6402 6403 6404 8d0a 4900  t.j.d.d.d.d...I.
-00000ac0: 6400 4800 7c00 5f0a 6400 5300 2905 4e54  d.H.|._.d.S.).NT
-00000ad0: e90a 0000 00e9 0100 0000 290a 7218 0000  ..........).r...
-00000ae0: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00000af0: 721c 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
-00000b00: 0a61 7574 6f63 6f6d 6d69 74da 076d 6178  .autocommit..max
-00000b10: 7369 7a65 5a07 6d69 6e73 697a 6529 0b72  sizeZ.minsize).r
-00000b20: 2300 0000 5a0b 6372 6561 7465 5f70 6f6f  #...Z.create_poo
-00000b30: 6c72 0800 0000 7218 0000 0072 1900 0000  lr....r....r....
-00000b40: 721a 0000 0072 1b00 0000 7225 0000 0072  r....r....r%...r
-00000b50: 1d00 0000 7226 0000 00da 0470 6f6f 6c72  ....r&.....poolr
-00000b60: 1100 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
-00000b70: 0000 0072 1000 0000 5000 0000 7318 0000  ...r....P...s...
-00000b80: 0000 0104 0106 0106 0106 0106 0106 0106  ................
-00000b90: 0104 0102 0202 0202 f47a 1f41 7379 6e63  .........z.Async
-00000ba0: 4d79 7371 6c50 6970 656c 696e 652e 5f6f  MysqlPipeline._o
-00000bb0: 7065 6e5f 7370 6964 6572 6303 0000 0000  pen_spiderc.....
-00000bc0: 0000 0000 0000 000a 0000 000b 0000 0083  ................
-00000bd0: 0000 0073 bc00 0000 7400 a001 7c01 a101  ...s....t...|...
-00000be0: 7d03 7c03 6401 1900 6402 6b02 72b8 7c00  }.|.d...d.k.r.|.
-00000bf0: 6a02 a003 a100 3400 4900 6400 4800 9a84  j.....4.I.d.H...
-00000c00: 7d04 7c04 a004 a100 3400 4900 6400 4800  }.|.....4.I.d.H.
-00000c10: 9a62 7d05 7405 7406 7c00 8302 a007 7c03  .b}.t.t.|.....|.
-00000c20: a101 7d06 7405 7406 7c00 8302 a008 7c03  ..}.t.t.|.....|.
-00000c30: 6403 1900 a101 7d07 7c06 6a09 7d08 7c00  d.....}.|.j.}.|.
-00000c40: 6a0a 7c07 7c08 6404 8d02 7d09 740b a00c  j.|.|.d...}.t...
-00000c50: 7c05 a00d 7c09 740e 7c08 a00f a100 8301  |...|.t.|.......
-00000c60: 6405 1400 a102 a101 4900 6400 4800 0100  d.......I.d.H...
-00000c70: 5700 3500 5100 4900 6400 4800 5200 5800  W.5.Q.I.d.H.R.X.
-00000c80: 5700 3500 5100 4900 6400 4800 5200 5800  W.5.Q.I.d.H.R.X.
-00000c90: 7c01 5300 7227 0000 0029 1072 0300 0000  |.S.r'...).r....
-00000ca0: 722d 0000 0072 4d00 0000 da07 6163 7175  r-...rM.....acqu
-00000cb0: 6972 6572 2e00 0000 722f 0000 0072 0500  irer....r/...r..
-00000cc0: 0000 7230 0000 0072 3100 0000 7232 0000  ..r0...r1...r2..
-00000cd0: 0072 3300 0000 721f 0000 00da 0673 6869  .r3...r......shi
-00000ce0: 656c 6472 3400 0000 7235 0000 0072 3600  eldr4...r5...r6.
-00000cf0: 0000 290a 7212 0000 0072 2b00 0000 7213  ..).r....r+...r.
-00000d00: 0000 0072 3800 0000 da04 636f 6e6e 722e  ...r8.....connr.
-00000d10: 0000 0072 3900 0000 722a 0000 0072 3200  ...r9...r*...r2.
-00000d20: 0000 723a 0000 0072 3b00 0000 7214 0000  ..r:...r;...r...
-00000d30: 0072 1500 0000 723d 0000 0060 0000 0073  .r....r=...`...s
-00000d40: 1c00 0000 0001 0a01 0c01 1401 1201 1001  ................
-00000d50: 0a01 06ff 0403 0601 0e01 0401 16ff 2a03  ..............*.
-00000d60: 7a1f 4173 796e 634d 7973 716c 5069 7065  z.AsyncMysqlPipe
-00000d70: 6c69 6e65 2e70 726f 6365 7373 5f69 7465  line.process_ite
-00000d80: 6d63 0100 0000 0000 0000 0000 0000 0100  mc..............
-00000d90: 0000 0200 0000 c300 0000 731e 0000 007c  ..........s....|
-00000da0: 006a 00a0 01a1 0001 007c 006a 00a0 02a1  .j.......|.j....
-00000db0: 0049 0064 0048 0001 0064 0053 0072 3e00  .I.d.H...d.S.r>.
-00000dc0: 0000 2903 724d 0000 0072 4100 0000 da0b  ..).rM...rA.....
-00000dd0: 7761 6974 5f63 6c6f 7365 6472 3f00 0000  wait_closedr?...
-00000de0: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
-00000df0: 4000 0000 7000 0000 7304 0000 0000 010a  @...p...s.......
-00000e00: 017a 2041 7379 6e63 4d79 7371 6c50 6970  .z AsyncMysqlPip
-00000e10: 656c 696e 652e 5f63 6c6f 7365 5f73 7069  eline._close_spi
-00000e20: 6465 7263 0200 0000 0000 0000 0000 0000  derc............
-00000e30: 0200 0000 0400 0000 4300 0000 730e 0000  ........C...s...
-00000e40: 0074 00a0 017c 00a0 02a1 00a1 0153 0072  .t...|.......S.r
-00000e50: 3e00 0000 2903 7202 0000 0072 0f00 0000  >...).r....r....
-00000e60: 7240 0000 0072 1100 0000 7214 0000 0072  r@...r....r....r
-00000e70: 1400 0000 7215 0000 0072 4200 0000 7400  ....r....rB...t.
-00000e80: 0000 7302 0000 0000 017a 1f41 7379 6e63  ..s......z.Async
-00000e90: 4d79 7371 6c50 6970 656c 696e 652e 636c  MysqlPipeline.cl
-00000ea0: 6f73 655f 7370 6964 6572 7243 0000 0072  ose_spiderrC...r
-00000eb0: 1400 0000 7214 0000 0072 3b00 0000 7215  ....r....r;...r.
-00000ec0: 0000 0072 0500 0000 4300 0000 730c 0000  ...r....C...s...
-00000ed0: 0008 0104 0408 0808 100c 1008 0429 0b72  .............).r
-00000ee0: 1f00 0000 7223 0000 00da 2461 7975 6765  ....r#....$ayuge
-00000ef0: 7370 6964 6572 746f 6f6c 732e 636f 6d6d  spidertools.comm
-00000f00: 6f6e 2e6d 756c 7469 706c 6578 696e 6772  on.multiplexingr
-00000f10: 0200 0000 da1d 6179 7567 6573 7069 6465  ......ayugespide
-00000f20: 7274 6f6f 6c73 2e63 6f6d 6d6f 6e2e 7574  rtools.common.ut
-00000f30: 696c 7372 0300 0000 da28 6179 7567 6573  ilsr.....(ayuges
-00000f40: 7069 6465 7274 6f6f 6c73 2e73 6372 6170  pidertools.scrap
-00000f50: 6572 2e70 6970 656c 696e 6573 2e6d 7973  er.pipelines.mys
-00000f60: 716c 7204 0000 00da 075f 5f61 6c6c 5f5f  qlr......__all__
-00000f70: 7206 0000 0072 0500 0000 7214 0000 0072  r....r....r....r
-00000f80: 1400 0000 7214 0000 0072 1500 0000 da08  ....r....r......
-00000f90: 3c6d 6f64 756c 653e 0100 0000 7312 0000  <module>....s...
-00000fa0: 0008 0208 020c 010c 010c 0302 0102 fe04  ................
-00000fb0: 0610 34                                  ..4
+00000930: 6405 8400 5a05 6406 6407 8400 5a06 6408  d...Z.d.d...Z.d.
+00000940: 6409 8400 5a07 640a 640b 8400 5a08 640c  d...Z.d.d...Z.d.
+00000950: 5300 290d 7205 0000 0075 4e00 0000 0a20  S.).r....uN.... 
+00000960: 2020 20e9 809a e8bf 8720 6169 6f6d 7973     ...... aiomys
+00000970: 716c 20e5 ae9e e78e b0e5 bc82 e6ad a5e5  ql .............
+00000980: 8699 e585 a520 4d79 7371 6c20 e695 b0e6  ..... Mysql ....
+00000990: 8dae e5ba 93e7 9a84 e8bf 9ee6 8ea5 e6b1  ................
+000009a0: a0e7 8988 e69c ac0a 2020 2020 6302 0000  ........    c...
+000009b0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+000009c0: 0043 0000 0073 4200 0000 7400 7c01 6401  .C...sB...t.|.d.
+000009d0: 8302 7312 7401 6402 8301 8201 7c01 6a02  ..s.t.d.....|.j.
+000009e0: 7c00 5f02 7c01 6a03 7c00 5f03 7404 6a05  |._.|.j.|._.t.j.
+000009f0: 7c01 6a03 6403 8d01 7c00 5f06 7407 a008  |.j.d...|._.t...
+00000a00: 7c00 a009 7c01 a101 a101 5300 7207 0000  |...|.....S.r...
+00000a10: 0072 0900 0000 7211 0000 0072 1400 0000  .r....r....r....
+00000a20: 7214 0000 0072 1500 0000 7216 0000 0048  r....r....r....H
+00000a30: 0000 0073 0a00 0000 0001 1202 0801 0801  ...s............
+00000a40: 1001 7a1e 4173 796e 634d 7973 716c 5069  ..z.AsyncMysqlPi
+00000a50: 7065 6c69 6e65 2e6f 7065 6e5f 7370 6964  peline.open_spid
+00000a60: 6572 6302 0000 0000 0000 0000 0000 0002  erc.............
+00000a70: 0000 000b 0000 00c3 0000 0073 4200 0000  ...........sB...
+00000a80: 7400 6a01 7c00 6a02 6a03 7c00 6a02 6a04  t.j.|.j.j.|.j.j.
+00000a90: 7c00 6a02 6a05 7c00 6a02 6a06 7c00 6a02  |.j.j.|.j.j.|.j.
+00000aa0: 6a07 7c00 6a02 6a08 7400 6a09 6401 6402  j.|.j.j.t.j.d.d.
+00000ab0: 6403 8d09 4900 6400 4800 7c00 5f0a 6400  d...I.d.H.|._.d.
+00000ac0: 5300 2904 4e54 e914 0000 0029 0972 1800  S.).NT.....).r..
+00000ad0: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00000ae0: 0072 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+00000af0: da0a 6175 746f 636f 6d6d 6974 da07 6d61  ..autocommit..ma
+00000b00: 7873 697a 6529 0b72 2300 0000 5a0b 6372  xsize).r#...Z.cr
+00000b10: 6561 7465 5f70 6f6f 6c72 0800 0000 7218  eate_poolr....r.
+00000b20: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
+00000b30: 0000 7225 0000 0072 1d00 0000 7226 0000  ..r%...r....r&..
+00000b40: 00da 0470 6f6f 6c72 1100 0000 7214 0000  ...poolr....r...
+00000b50: 0072 1400 0000 7215 0000 0072 1000 0000  .r....r....r....
+00000b60: 5000 0000 7316 0000 0000 0104 0106 0106  P...s...........
+00000b70: 0106 0106 0106 0106 0104 0102 0202 f67a  ...............z
+00000b80: 1f41 7379 6e63 4d79 7371 6c50 6970 656c  .AsyncMysqlPipel
+00000b90: 696e 652e 5f6f 7065 6e5f 7370 6964 6572  ine._open_spider
+00000ba0: 6303 0000 0000 0000 0000 0000 0007 0000  c...............
+00000bb0: 000a 0000 00c3 0000 0073 8600 0000 7400  .........s....t.
+00000bc0: a001 7c01 a101 7d03 7c03 6401 1900 6402  ..|...}.|.d...d.
+00000bd0: 6b02 7282 7402 6a03 7c00 6a04 a005 a100  k.r.t.j.|.j.....
+00000be0: 6403 6404 8d02 4900 6400 4800 7d04 7a42  d.d...I.d.H.}.zB
+00000bf0: 7c04 a007 a100 3400 4900 6400 4800 9a22  |.....4.I.d.H.."
+00000c00: 7d05 6405 7d06 7402 a008 7c05 a009 7c06  }.d.}.t...|...|.
+00000c10: 6406 a102 a101 4900 6400 4800 0100 5700  d.....I.d.H...W.
+00000c20: 3500 5100 4900 6400 4800 5200 5800 5700  5.Q.I.d.H.R.X.W.
+00000c30: 3500 7c00 6a04 a006 7c04 a101 0100 5800  5.|.j...|.....X.
+00000c40: 7c01 5300 2907 4e72 2700 0000 7228 0000  |.S.).Nr'...r(..
+00000c50: 0069 f401 0000 2901 da07 7469 6d65 6f75  .i....)...timeou
+00000c60: 747a ae49 4e53 4552 5420 494e 544f 2060  tz.INSERT INTO `
+00000c70: 6465 6d6f 355f 626f 6f6b 5f69 6e66 6f5f  demo5_book_info_
+00000c80: 6c69 7374 6020 2860 626f 6f6b 5f6e 616d  list` (`book_nam
+00000c90: 6560 2c20 6062 6f6f 6b5f 6872 6566 602c  e`, `book_href`,
+00000ca0: 2060 626f 6f6b 5f69 6e74 726f 6029 2076   `book_intro`) v
+00000cb0: 616c 7565 7320 2825 732c 2025 732c 2025  alues (%s, %s, %
+00000cc0: 7329 204f 4e20 4455 504c 4943 4154 4520  s) ON DUPLICATE 
+00000cd0: 4b45 5920 5550 4441 5445 2020 6062 6f6f  KEY UPDATE  `boo
+00000ce0: 6b5f 6e61 6d65 6020 3d20 2573 2c20 6062  k_name` = %s, `b
+00000cf0: 6f6f 6b5f 6872 6566 6020 3d20 2573 2c20  ook_href` = %s, 
+00000d00: 6062 6f6f 6b5f 696e 7472 6f60 203d 2025  `book_intro` = %
+00000d10: 7329 06da 0962 6f6f 6b5f 6e61 6d65 da09  s)...book_name..
+00000d20: 626f 6f6b 5f68 7265 66da 0a62 6f6f 6b5f  book_href..book_
+00000d30: 696e 7472 6f72 4c00 0000 724d 0000 0072  introrL...rM...r
+00000d40: 4e00 0000 290a 7203 0000 0072 2c00 0000  N...).r....r,...
+00000d50: 721f 0000 00da 0877 6169 745f 666f 7272  r......wait_forr
+00000d60: 4a00 0000 da07 6163 7175 6972 65da 0772  J.....acquire..r
+00000d70: 656c 6561 7365 722d 0000 00da 0673 6869  eleaser-.....shi
+00000d80: 656c 6472 3300 0000 2907 7212 0000 0072  eldr3...).r....r
+00000d90: 2a00 0000 7213 0000 0072 3700 0000 da04  *...r....r7.....
+00000da0: 636f 6e6e 722d 0000 0072 3900 0000 7214  connr-...r9...r.
+00000db0: 0000 0072 1400 0000 7215 0000 0072 3c00  ...r....r....r<.
+00000dc0: 0000 6000 0000 731c 0000 0000 010a 010c  ..`...s.........
+00000dd0: 011a 0102 0212 0104 0204 0104 0102 0102  ................
+00000de0: fe02 ff1e 0f0e 027a 1f41 7379 6e63 4d79  .......z.AsyncMy
+00000df0: 7371 6c50 6970 656c 696e 652e 7072 6f63  sqlPipeline.proc
+00000e00: 6573 735f 6974 656d 6301 0000 0000 0000  ess_itemc.......
+00000e10: 0000 0000 0001 0000 0002 0000 00c3 0000  ................
+00000e20: 0073 1e00 0000 7c00 6a00 a001 a100 0100  .s....|.j.......
+00000e30: 7c00 6a00 a002 a100 4900 6400 4800 0100  |.j.....I.d.H...
+00000e40: 6400 5300 723d 0000 0029 0372 4a00 0000  d.S.r=...).rJ...
+00000e50: 7240 0000 00da 0b77 6169 745f 636c 6f73  r@.....wait_clos
+00000e60: 6564 723e 0000 0072 1400 0000 7214 0000  edr>...r....r...
+00000e70: 0072 1500 0000 723f 0000 007c 0000 0073  .r....r?...|...s
+00000e80: 0400 0000 0001 0a01 7a20 4173 796e 634d  ........z AsyncM
+00000e90: 7973 716c 5069 7065 6c69 6e65 2e5f 636c  ysqlPipeline._cl
+00000ea0: 6f73 655f 7370 6964 6572 6302 0000 0000  ose_spiderc.....
+00000eb0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00000ec0: 0000 0073 0e00 0000 7400 a001 7c00 a002  ...s....t...|...
+00000ed0: a100 a101 5300 723d 0000 0029 0372 0200  ....S.r=...).r..
+00000ee0: 0000 720f 0000 0072 3f00 0000 7211 0000  ..r....r?...r...
+00000ef0: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000f00: 7241 0000 0080 0000 0073 0200 0000 0001  rA.......s......
+00000f10: 7a1f 4173 796e 634d 7973 716c 5069 7065  z.AsyncMysqlPipe
+00000f20: 6c69 6e65 2e63 6c6f 7365 5f73 7069 6465  line.close_spide
+00000f30: 724e 2909 7242 0000 0072 4300 0000 7244  rN).rB...rC...rD
+00000f40: 0000 0072 4500 0000 7216 0000 0072 1000  ...rE...r....r..
+00000f50: 0000 723c 0000 0072 3f00 0000 7241 0000  ..r<...r?...rA..
+00000f60: 0072 1400 0000 7214 0000 0072 1400 0000  .r....r....r....
+00000f70: 7215 0000 0072 0500 0000 4300 0000 730c  r....r....C...s.
+00000f80: 0000 0008 0104 0408 0808 1008 1c08 0429  ...............)
+00000f90: 0c72 1f00 0000 7223 0000 00da 2461 7975  .r....r#....$ayu
+00000fa0: 6765 7370 6964 6572 746f 6f6c 732e 636f  gespidertools.co
+00000fb0: 6d6d 6f6e 2e6d 756c 7469 706c 6578 696e  mmon.multiplexin
+00000fc0: 6772 0200 0000 da1d 6179 7567 6573 7069  gr......ayugespi
+00000fd0: 6465 7274 6f6f 6c73 2e63 6f6d 6d6f 6e2e  dertools.common.
+00000fe0: 7574 696c 7372 0300 0000 da28 6179 7567  utilsr.....(ayug
+00000ff0: 6573 7069 6465 7274 6f6f 6c73 2e73 6372  espidertools.scr
+00001000: 6170 6572 2e70 6970 656c 696e 6573 2e6d  aper.pipelines.m
+00001010: 7973 716c 7204 0000 00da 075f 5f61 6c6c  ysqlr......__all
+00001020: 5f5f 7206 0000 00da 066f 626a 6563 7472  __r......objectr
+00001030: 0500 0000 7214 0000 0072 1400 0000 7214  ....r....r....r.
+00001040: 0000 0072 1500 0000 da08 3c6d 6f64 756c  ...r......<modul
+00001050: 653e 0100 0000 7312 0000 0008 0208 020c  e>....s.........
+00001060: 010c 010c 0302 0102 fe04 0610 34         ............4
```

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/asynced.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/asynced.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/stats.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/stats.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/turbo.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/turbo.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/twisted.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/pipelines/mysql/twisted.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/spiders/__init__.py` & `ayugespidertools-2.1.0/ayugespidertools/scraper/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/templates/project/.gitignore` & `ayugespidertools-2.1.0/ayugespidertools/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/templates/project/module/VIT/.conf` & `ayugespidertools-2.1.0/ayugespidertools/templates/project/module/VIT/.conf`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/templates/project/module/items.py.tmpl` & `ayugespidertools-2.1.0/ayugespidertools/templates/project/module/items.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/templates/project/module/middlewares.py.tmpl` & `ayugespidertools-2.1.0/ayugespidertools/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/templates/project/module/settings.py.tmpl` & `ayugespidertools-2.1.0/ayugespidertools/templates/project/module/settings.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/templates/spiders/async.tmpl` & `ayugespidertools-2.1.0/ayugespidertools/templates/spiders/async.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/templates/spiders/basic.tmpl` & `ayugespidertools-2.1.0/ayugespidertools/templates/spiders/basic.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/templates/spiders/crawl.tmpl` & `ayugespidertools-2.1.0/ayugespidertools/templates/spiders/crawl.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/templates/spiders/csvfeed.tmpl` & `ayugespidertools-2.1.0/ayugespidertools/templates/spiders/csvfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/templates/spiders/xmlfeed.tmpl` & `ayugespidertools-2.1.0/ayugespidertools/templates/spiders/xmlfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc` & `ayugespidertools-2.1.0/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat May  6 06:33:34 2023 UTC, .py size: 5909 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,333 +1,335 @@
-00000000: 550d 0d0a 0000 0000 bef4 5564 1517 0000  U.........Ud....
+00000000: 550d 0d0a 0000 0000 c0a7 5964 3717 0000  U.........Yd7...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 2401 0000 6400  .....@...s$...d.
+00000020: 0007 0000 0040 0000 0073 2801 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
-00000060: 6402 6c06 6d07 5a07 6d08 5a08 0100 6400  d.l.m.Z.m.Z...d.
-00000070: 6403 6c09 6d0a 5a0a 0100 6400 6404 6c0b  d.l.m.Z...d.d.l.
-00000080: 6d0c 5a0c 0100 6400 6405 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
-00000090: 0100 6400 6406 6c0f 6d10 5a10 6d11 5a11  ..d.d.l.m.Z.m.Z.
-000000a0: 0100 6400 6407 6c12 6d13 5a13 0100 6400  ..d.d.l.m.Z...d.
-000000b0: 6408 6c14 6d15 5a15 0100 4700 6409 640a  d.l.m.Z...G.d.d.
-000000c0: 8400 640a 6500 6a16 8303 5a17 640b 640c  ..d.e.j...Z.d.d.
-000000d0: 8400 5a18 640d 640e 8400 5a19 6425 6410  ..Z.d.d...Z.d%d.
-000000e0: 6411 8401 5a1a 6412 6413 8400 5a1b 6414  d...Z.d.d...Z.d.
-000000f0: 6415 8400 5a1c 6416 6417 8400 5a1d 6418  d...Z.d.d...Z.d.
-00000100: 6419 8400 5a1e 641a 641b 8400 5a1f 641c  d...Z.d.d...Z.d.
-00000110: 641d 8400 5a20 6426 641e 641f 8401 5a21  d...Z d&d.d...Z!
-00000120: 6420 6421 8400 5a22 6422 6423 8400 5a23  d d!..Z"d"d#..Z#
-00000130: 6524 6424 6b02 9001 7220 7a0a 6521 8300  e$d$k...r z.e!..
-00000140: 0100 5700 3500 6513 8300 0100 5800 6401  ..W.5.e.....X.d.
-00000150: 5300 2927 e900 0000 004e 2902 da0d 5363  S.)'.....N)...Sc
-00000160: 7261 7079 436f 6d6d 616e 64da 1353 6372  rapyCommand..Scr
-00000170: 6170 7948 656c 7046 6f72 6d61 7474 6572  apyHelpFormatter
-00000180: 2901 da0e 4372 6177 6c65 7250 726f 6365  )...CrawlerProce
-00000190: 7373 2901 da0a 5573 6167 6545 7272 6f72  ss)...UsageError
-000001a0: 2901 da0c 7761 6c6b 5f6d 6f64 756c 6573  )...walk_modules
-000001b0: 2902 da14 6765 745f 7072 6f6a 6563 745f  )...get_project_
-000001c0: 7365 7474 696e 6773 da0e 696e 7369 6465  settings..inside
-000001d0: 5f70 726f 6a65 6374 2901 da0f 6761 7262  _project)...garb
-000001e0: 6167 655f 636f 6c6c 6563 7429 01da 0a41  age_collect)...A
-000001f0: 7975 436f 6d6d 616e 6463 0000 0000 0000  yuCommandc......
-00000200: 0000 0000 0000 0000 0000 0300 0000 0000  ................
-00000210: 0000 731c 0000 0065 005a 0164 005a 0287  ..s....e.Z.d.Z..
-00000220: 0066 0164 0164 0284 085a 0387 0004 005a  .f.d.d...Z.....Z
-00000230: 0453 0029 03da 1453 6372 6170 7941 7267  .S.)...ScrapyArg
-00000240: 756d 656e 7450 6172 7365 7263 0200 0000  umentParserc....
-00000250: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000260: 0300 0000 7320 0000 007c 0164 0064 0185  ....s ...|.d.d..
-00000270: 0219 0064 026b 0272 1464 0053 0074 0083  ...d.k.r.d.S.t..
-00000280: 00a0 017c 01a1 0153 0029 034e e902 0000  ...|...S.).N....
-00000290: 007a 022d 3a29 02da 0573 7570 6572 da0f  .z.-:)...super..
-000002a0: 5f70 6172 7365 5f6f 7074 696f 6e61 6c29  _parse_optional)
-000002b0: 02da 0473 656c 66da 0a61 7267 5f73 7472  ...self..arg_str
-000002c0: 696e 67a9 01da 095f 5f63 6c61 7373 5f5f  ing....__class__
-000002d0: a900 fa3f 2f72 6f6f 742f 6d79 7072 6f6a  ...?/root/myproj
-000002e0: 2f41 7975 6765 5370 6964 6572 546f 6f6c  /AyugeSpiderTool
-000002f0: 732f 6179 7567 6573 7069 6465 7274 6f6f  s/ayugespidertoo
-00000300: 6c73 2f75 7469 6c73 2f63 6d64 6c69 6e65  ls/utils/cmdline
-00000310: 2e70 7972 0e00 0000 1300 0000 7306 0000  .pyr........s...
-00000320: 0000 0210 0104 027a 2453 6372 6170 7941  .......z$ScrapyA
-00000330: 7267 756d 656e 7450 6172 7365 722e 5f70  rgumentParser._p
-00000340: 6172 7365 5f6f 7074 696f 6e61 6c29 05da  arse_optional)..
-00000350: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000360: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000370: 655f 5f72 0e00 0000 da0d 5f5f 636c 6173  e__r......__clas
-00000380: 7363 656c 6c5f 5f72 1300 0000 7213 0000  scell__r....r...
-00000390: 0072 1100 0000 7214 0000 0072 0b00 0000  .r....r....r....
-000003a0: 1200 0000 7302 0000 0008 0172 0b00 0000  ....s......r....
-000003b0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-000003c0: 0005 0000 0063 0000 0073 5200 0000 7400  .....c...sR...t.
-000003d0: 7c00 8301 4400 5d44 7d01 7401 7c01 8301  |...D.]D}.t.|...
-000003e0: a002 a100 4400 5d32 7d02 7403 a004 7c02  ....D.]2}.t...|.
-000003f0: a101 7218 7405 7c02 7406 8302 7218 7c02  ..r.t.|.t...r.|.
-00000400: 6a07 7c01 6a08 6b02 7218 7c02 7406 6b02  j.|.j.k.r.|.t.k.
-00000410: 7318 7c02 5600 0100 7118 7108 6400 5300  s.|.V...q.q.d.S.
-00000420: a901 4e29 0972 0600 0000 da04 7661 7273  ..N).r......vars
-00000430: da06 7661 6c75 6573 da07 696e 7370 6563  ..values..inspec
-00000440: 74da 0769 7363 6c61 7373 da0a 6973 7375  t..isclass..issu
-00000450: 6263 6c61 7373 7202 0000 0072 1600 0000  bclassr....r....
-00000460: 7215 0000 0029 03da 0b6d 6f64 756c 655f  r....)...module_
-00000470: 6e61 6d65 da06 6d6f 6475 6c65 da03 6f62  name..module..ob
-00000480: 6a72 1300 0000 7213 0000 0072 1400 0000  jr....r....r....
-00000490: da15 5f69 7465 725f 636f 6d6d 616e 645f  .._iter_command_
-000004a0: 636c 6173 7365 731b 0000 0073 1600 0000  classes....s....
-000004b0: 0003 0c01 1002 08ff 0202 08fe 0203 0afd  ................
-000004c0: 0204 06fc 0206 7222 0000 0063 0200 0000  ......r"...c....
-000004d0: 0000 0000 0000 0000 0500 0000 0400 0000  ................
-000004e0: 4300 0000 733a 0000 0069 007d 0274 007c  C...s:...i.}.t.|
-000004f0: 0083 0144 005d 287d 037c 0173 1a7c 036a  ...D.](}.|.s.|.j
-00000500: 0173 0c7c 036a 02a0 0364 01a1 0164 0219  .s.|.j...d...d..
-00000510: 007d 047c 0383 007c 027c 043c 0071 0c7c  .}.|...|.|.<.q.|
-00000520: 0253 0029 034e da01 2ee9 ffff ffff 2904  .S.).N........).
-00000530: 7222 0000 005a 1072 6571 7569 7265 735f  r"...Z.requires_
-00000540: 7072 6f6a 6563 7472 1600 0000 da05 7370  projectr......sp
-00000550: 6c69 7429 0572 2000 0000 da09 696e 7072  lit).r .....inpr
-00000560: 6f6a 6563 74da 0164 da03 636d 64da 0763  oject..d..cmd..c
-00000570: 6d64 6e61 6d65 7213 0000 0072 1300 0000  mdnamer....r....
-00000580: 7214 0000 00da 195f 6765 745f 636f 6d6d  r......_get_comm
-00000590: 616e 6473 5f66 726f 6d5f 6d6f 6475 6c65  ands_from_module
-000005a0: 2900 0000 730c 0000 0000 0104 010c 010a  )...s...........
-000005b0: 0110 010c 0172 2a00 0000 fa19 6179 7567  .....r*.....ayug
-000005c0: 6573 7069 6465 7274 6f6f 6c73 2e63 6f6d  espidertools.com
-000005d0: 6d61 6e64 7363 0200 0000 0000 0000 0000  mandsc..........
-000005e0: 0000 0500 0000 0400 0000 4300 0000 7348  ..........C...sH
-000005f0: 0000 0069 007d 0274 00a0 017c 01a1 0144  ...i.}.t...|...D
-00000600: 005d 347d 037c 03a0 02a1 007d 0474 03a0  .]4}.|.....}.t..
-00000610: 047c 04a1 0172 327c 0483 007c 027c 036a  .|...r2|...|.|.j
-00000620: 053c 0071 0e74 0664 017c 036a 059b 009d  .<.q.t.d.|.j....
-00000630: 0283 0182 0171 0e7c 0253 0029 024e 7a14  .....q.|.S.).Nz.
-00000640: 496e 7661 6c69 6420 656e 7472 7920 706f  Invalid entry po
-00000650: 696e 7420 2907 da0d 706b 675f 7265 736f  int )...pkg_reso
-00000660: 7572 6365 735a 1169 7465 725f 656e 7472  urcesZ.iter_entr
-00000670: 795f 706f 696e 7473 da04 6c6f 6164 721c  y_points..loadr.
-00000680: 0000 0072 1d00 0000 da04 6e61 6d65 da09  ...r......name..
-00000690: 4578 6365 7074 696f 6e29 0572 2600 0000  Exception).r&...
-000006a0: da05 6772 6f75 70da 0463 6d64 73da 0b65  ..group..cmds..e
-000006b0: 6e74 7279 5f70 6f69 6e74 7221 0000 0072  ntry_pointr!...r
-000006c0: 1300 0000 7213 0000 0072 1400 0000 da1f  ....r....r......
-000006d0: 5f67 6574 5f63 6f6d 6d61 6e64 735f 6672  _get_commands_fr
-000006e0: 6f6d 5f65 6e74 7279 5f70 6f69 6e74 7332  om_entry_points2
-000006f0: 0000 0073 0e00 0000 0001 0401 0e01 0801  ...s............
-00000700: 0a01 0e02 1201 7233 0000 0063 0200 0000  ......r3...c....
-00000710: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-00000720: 4300 0000 7338 0000 0074 0064 017c 0183  C...s8...t.d.|..
-00000730: 027d 027c 02a0 0174 027c 0183 01a1 0101  .}.|...t.|......
-00000740: 007c 0064 0219 007d 037c 0372 347c 02a0  .|.d...}.|.r4|..
-00000750: 0174 007c 037c 0183 02a1 0101 007c 0253  .t.|.|.......|.S
-00000760: 0029 034e 722b 0000 00da 0f43 4f4d 4d41  .).Nr+.....COMMA
-00000770: 4e44 535f 4d4f 4455 4c45 2903 722a 0000  NDS_MODULE).r*..
-00000780: 00da 0675 7064 6174 6572 3300 0000 2904  ...updater3...).
-00000790: da08 7365 7474 696e 6773 7226 0000 0072  ..settingsr&...r
-000007a0: 3100 0000 5a0b 636d 6473 5f6d 6f64 756c  1...Z.cmds_modul
-000007b0: 6572 1300 0000 7213 0000 0072 1400 0000  er....r....r....
-000007c0: da12 5f67 6574 5f63 6f6d 6d61 6e64 735f  .._get_commands_
-000007d0: 6469 6374 3d00 0000 730c 0000 0000 010a  dict=...s.......
-000007e0: 010e 0108 0104 0110 0172 3700 0000 6301  .........r7...c.
-000007f0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00000800: 0000 0043 0000 0073 3a00 0000 6401 7d01  ...C...s:...d.}.
-00000810: 7c00 6402 6400 8502 1900 4400 5d24 7d02  |.d.d.....D.]$}.
-00000820: 7c02 a000 6403 a101 732c 7c00 7c01 3d00  |...d...s,|.|.=.
-00000830: 7c02 0200 0100 5300 7c01 6402 3700 7d01  |.....S.|.d.7.}.
-00000840: 7110 6400 5300 2904 4e72 0100 0000 e901  q.d.S.).Nr......
-00000850: 0000 00fa 012d 2901 da0a 7374 6172 7473  .....-)...starts
-00000860: 7769 7468 2903 da04 6172 6776 da01 69da  with)...argv..i.
-00000870: 0361 7267 7213 0000 0072 1300 0000 7214  .argr....r....r.
-00000880: 0000 00da 115f 706f 705f 636f 6d6d 616e  ....._pop_comman
-00000890: 645f 6e61 6d65 4600 0000 730c 0000 0000  d_nameF...s.....
-000008a0: 0104 0110 010a 0106 0108 0172 3e00 0000  ...........r>...
-000008b0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-000008c0: 0006 0000 0043 0000 0073 4400 0000 7400  .....C...sD...t.
-000008d0: 8300 6a01 6400 6400 6401 8d02 7d02 7c01  ..j.d.d.d...}.|.
-000008e0: 7230 7402 6402 7c02 9b00 6403 7c00 6404  r0t.d.|...d.|.d.
-000008f0: 1900 9b00 6405 9d05 8301 0100 6e10 7402  ....d.......n.t.
-00000900: 6402 7c02 9b00 6406 9d03 8301 0100 6400  d.|...d.......d.
-00000910: 5300 2907 4e29 02da 0461 7267 73da 046f  S.).N)...args..o
-00000920: 7074 737a 1141 7975 6765 5370 6964 6572  ptsz.AyugeSpider
-00000930: 546f 6f6c 7320 7a0c 202d 2070 726f 6a65  Tools z. - proje
-00000940: 6374 3a20 da08 424f 545f 4e41 4d45 da01  ct: ..BOT_NAME..
-00000950: 0a7a 1520 2d20 6e6f 2061 6374 6976 6520  .z. - no active 
-00000960: 7072 6f6a 6563 740a 2903 720a 0000 00da  project.).r.....
-00000970: 0372 756e da05 7072 696e 7429 0372 3600  .run..print).r6.
-00000980: 0000 7226 0000 00da 0776 6572 7369 6f6e  ..r&.....version
-00000990: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-000009a0: 0d5f 7072 696e 745f 6865 6164 6572 4f00  ._print_headerO.
-000009b0: 0000 7308 0000 0000 0110 0104 011c 0272  ..s............r
-000009c0: 4600 0000 6302 0000 0000 0000 0000 0000  F...c...........
-000009d0: 0005 0000 0007 0000 0043 0000 0073 8000  .........C...s..
-000009e0: 0000 7400 7c00 7c01 8302 0100 7401 6401  ..t.|.|.....t.d.
-000009f0: 8301 0100 7401 6402 8301 0100 7401 6403  ....t.d.....t.d.
-00000a00: 8301 0100 7402 7c00 7c01 8302 7d02 7403  ....t.|.|...}.t.
-00000a10: 7c02 a004 a100 8301 4400 5d22 5c02 7d03  |.......D.]"\.}.
-00000a20: 7d04 7401 6404 7c03 6405 9b04 6406 7c04  }.t.d.|.d...d.|.
-00000a30: a005 a100 9b00 9d04 8301 0100 7138 7c01  ............q8|.
-00000a40: 736e 7401 8300 0100 7401 6407 8301 0100  snt.....t.d.....
-00000a50: 7401 8300 0100 7401 6408 8301 0100 6400  t.....t.d.....d.
-00000a60: 5300 2909 4e7a 0655 7361 6765 3a7a 2320  S.).Nz.Usage:z# 
-00000a70: 2061 7975 6765 203c 636f 6d6d 616e 643e   ayuge <command>
-00000a80: 205b 6f70 7469 6f6e 735d 205b 6172 6773   [options] [args
-00000a90: 5d0a 7a13 4176 6169 6c61 626c 6520 636f  ].z.Available co
-00000aa0: 6d6d 616e 6473 3a7a 0220 207a 033c 3133  mmands:z.  z.<13
-00000ab0: fa01 207a 4720 205b 206d 6f72 6520 5d20  .. zG  [ more ] 
-00000ac0: 2020 2020 204d 6f72 6520 636f 6d6d 616e       More comman
-00000ad0: 6473 2061 7661 696c 6162 6c65 2077 6865  ds available whe
-00000ae0: 6e20 7275 6e20 6672 6f6d 2070 726f 6a65  n run from proje
-00000af0: 6374 2064 6972 6563 746f 7279 7a39 5573  ct directoryz9Us
-00000b00: 6520 2261 7975 6765 203c 636f 6d6d 616e  e "ayuge <comman
-00000b10: 643e 202d 6822 2074 6f20 7365 6520 6d6f  d> -h" to see mo
-00000b20: 7265 2069 6e66 6f20 6162 6f75 7420 6120  re info about a 
-00000b30: 636f 6d6d 616e 6429 0672 4600 0000 7244  command).rF...rD
-00000b40: 0000 0072 3700 0000 da06 736f 7274 6564  ...r7.....sorted
-00000b50: da05 6974 656d 735a 0a73 686f 7274 5f64  ..itemsZ.short_d
-00000b60: 6573 6329 0572 3600 0000 7226 0000 0072  esc).r6...r&...r
-00000b70: 3100 0000 7229 0000 005a 0863 6d64 636c  1...r)...Z.cmdcl
-00000b80: 6173 7372 1300 0000 7213 0000 0072 1400  assr....r....r..
-00000b90: 0000 da0f 5f70 7269 6e74 5f63 6f6d 6d61  ...._print_comma
-00000ba0: 6e64 7357 0000 0073 1800 0000 0001 0a01  ndsW...s........
-00000bb0: 0801 0801 0801 0a01 1401 1c01 0401 0601  ................
-00000bc0: 0801 0601 724a 0000 0063 0300 0000 0000  ....rJ...c......
-00000bd0: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-00000be0: 0000 7326 0000 0074 007c 007c 0283 0201  ..s&...t.|.|....
-00000bf0: 0074 0164 017c 019b 0064 029d 0383 0101  .t.d.|...d......
-00000c00: 0074 0164 0383 0101 0064 0053 0029 044e  .t.d.....d.S.).N
-00000c10: 7a11 556e 6b6e 6f77 6e20 636f 6d6d 616e  z.Unknown comman
-00000c20: 643a 2072 4200 0000 7a25 5573 6520 2261  d: rB...z%Use "a
-00000c30: 7975 6765 2220 746f 2073 6565 2061 7661  yuge" to see ava
-00000c40: 696c 6162 6c65 2063 6f6d 6d61 6e64 7329  ilable commands)
-00000c50: 0272 4600 0000 7244 0000 0029 0372 3600  .rF...rD...).r6.
-00000c60: 0000 7229 0000 0072 2600 0000 7213 0000  ..r)...r&...r...
-00000c70: 0072 1300 0000 7214 0000 00da 165f 7072  .r....r......_pr
-00000c80: 696e 745f 756e 6b6e 6f77 6e5f 636f 6d6d  int_unknown_comm
-00000c90: 616e 6466 0000 0073 0600 0000 0001 0a01  andf...s........
-00000ca0: 1001 724b 0000 0063 0200 0000 0000 0000  ..rK...c........
-00000cb0: 0000 0000 0500 0000 0a00 0000 4f00 0000  ............O...
-00000cc0: 7364 0000 007a 0e7c 017c 027c 038e 0101  sd...z.|.|.|....
-00000cd0: 0057 006e 5004 0074 006b 0a72 5e01 007d  .W.nP..t.k.r^..}
-00000ce0: 0401 007a 3274 017c 0483 0172 367c 00a0  ...z2t.|...r6|..
-00000cf0: 0274 017c 0483 01a1 0101 007c 046a 0372  .t.|.......|.j.r
-00000d00: 447c 00a0 03a1 0001 0074 04a0 0564 01a1  D|.......t...d..
-00000d10: 0101 0057 0035 0064 007d 047e 0458 0059  ...W.5.d.}.~.X.Y
-00000d20: 006e 0258 0064 0053 0029 024e 720c 0000  .n.X.d.S.).Nr...
-00000d30: 0029 0672 0500 0000 da03 7374 72da 0565  .).r......str..e
-00000d40: 7272 6f72 da0a 7072 696e 745f 6865 6c70  rror..print_help
-00000d50: da03 7379 73da 0465 7869 7429 05da 0670  ..sys..exit)...p
-00000d60: 6172 7365 72da 0466 756e 63da 0161 da02  arser..func..a..
-00000d70: 6b77 da01 6572 1300 0000 7213 0000 0072  kw..er....r....r
-00000d80: 1400 0000 da0f 5f72 756e 5f70 7269 6e74  ......_run_print
-00000d90: 5f68 656c 706c 0000 0073 1000 0000 0001  _helpl...s......
-00000da0: 0201 0e01 1001 0801 0e01 0601 0801 7256  ..............rV
-00000db0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00000dc0: 0a00 0000 0800 0000 4300 0000 7336 0100  ........C...s6..
-00000dd0: 007c 0064 006b 0872 0e74 006a 017d 007c  .|.d.k.r.t.j.}.|
-00000de0: 0164 006b 0872 4874 0283 007d 017a 0e74  .d.k.rHt...}.z.t
-00000df0: 036a 0464 0119 007d 0257 006e 1404 0074  .j.d...}.W.n...t
-00000e00: 056b 0a72 3e01 0001 0001 0059 006e 0a58  .k.r>......Y.n.X
-00000e10: 007c 027c 0164 013c 0074 0683 007d 0374  .|.|.d.<.t...}.t
-00000e20: 077c 017c 0383 027d 0474 087c 0083 017d  .|.|...}.t.|...}
-00000e30: 057c 0573 7a74 097c 017c 0383 0201 0074  .|.szt.|.|.....t
-00000e40: 00a0 0a64 02a1 0101 006e 1e7c 057c 046b  ...d.....n.|.|.k
-00000e50: 0772 9874 0b7c 017c 057c 0383 0301 0074  .r.t.|.|.|.....t
-00000e60: 00a0 0a64 03a1 0101 007c 047c 0519 007d  ...d.....|.|...}
-00000e70: 0674 0c74 0d64 047c 059b 0064 057c 06a0  .t.t.d.|...d.|..
-00000e80: 0ea1 009b 009d 0464 067c 06a0 0fa1 0064  .......d.|.....d
-00000e90: 078d 047d 077c 016a 107c 066a 1164 0864  ...}.|.j.|.j.d.d
-00000ea0: 098d 0201 007c 017c 065f 127c 06a0 137c  .....|.|._.|...|
-00000eb0: 07a1 0101 007c 076a 147c 0064 0a64 0085  .....|.j.|.d.d..
-00000ec0: 0219 0064 0b8d 015c 027d 087d 0974 157c  ...d...\.}.}.t.|
-00000ed0: 077c 066a 167c 097c 0883 0401 0074 177c  .|.j.|.|.....t.|
-00000ee0: 0183 017c 065f 1874 157c 0774 197c 067c  ...|._.t.|.t.|.|
-00000ef0: 097c 0883 0501 0074 00a0 0a7c 066a 1aa1  .|.....t...|.j..
-00000f00: 0101 0064 0053 0029 0c4e da06 4544 4954  ...d.S.).N..EDIT
-00000f10: 4f52 7201 0000 0072 0c00 0000 7a06 6179  ORr....r....z.ay
-00000f20: 7567 6520 7247 0000 00da 0772 6573 6f6c  uge rG.....resol
-00000f30: 7665 2904 da0f 666f 726d 6174 7465 725f  ve)...formatter_
-00000f40: 636c 6173 73da 0575 7361 6765 da10 636f  class..usage..co
-00000f50: 6e66 6c69 6374 5f68 616e 646c 6572 da0b  nflict_handler..
-00000f60: 6465 7363 7269 7074 696f 6eda 0763 6f6d  description..com
-00000f70: 6d61 6e64 2901 da08 7072 696f 7269 7479  mand)...priority
-00000f80: 7238 0000 0029 0172 3f00 0000 291b 724f  r8...).r?...).rO
-00000f90: 0000 0072 3b00 0000 7207 0000 00da 026f  ...r;...r......o
-00000fa0: 73da 0765 6e76 6972 6f6e da08 4b65 7945  s..environ..KeyE
-00000fb0: 7272 6f72 7208 0000 0072 3700 0000 723e  rrorr....r7...r>
-00000fc0: 0000 0072 4a00 0000 7250 0000 0072 4b00  ...rJ...rP...rK.
-00000fd0: 0000 720b 0000 0072 0300 0000 5a06 7379  ..r....r....Z.sy
-00000fe0: 6e74 6178 5a09 6c6f 6e67 5f64 6573 63da  ntaxZ.long_desc.
-00000ff0: 0773 6574 6469 6374 da10 6465 6661 756c  .setdict..defaul
-00001000: 745f 7365 7474 696e 6773 7236 0000 005a  t_settingsr6...Z
-00001010: 0b61 6464 5f6f 7074 696f 6e73 da10 7061  .add_options..pa
-00001020: 7273 655f 6b6e 6f77 6e5f 6172 6773 7256  rse_known_argsrV
-00001030: 0000 005a 0f70 726f 6365 7373 5f6f 7074  ...Z.process_opt
-00001040: 696f 6e73 7204 0000 005a 0f63 7261 776c  ionsr....Z.crawl
-00001050: 6572 5f70 726f 6365 7373 da0c 5f72 756e  er_process.._run
-00001060: 5f63 6f6d 6d61 6e64 da08 6578 6974 636f  _command..exitco
-00001070: 6465 290a 723b 0000 0072 3600 0000 5a06  de).r;...r6...Z.
-00001080: 6564 6974 6f72 7226 0000 0072 3100 0000  editorr&...r1...
-00001090: 7229 0000 0072 2800 0000 7251 0000 0072  r)...r(...rQ...r
-000010a0: 4000 0000 723f 0000 0072 1300 0000 7213  @...r?...r....r.
-000010b0: 0000 0072 1400 0000 da07 6578 6563 7574  ...r......execut
-000010c0: 6577 0000 0073 4200 0000 0001 0801 0602  ew...sB.........
-000010d0: 0801 0602 0201 0e01 0e01 0602 0802 0601  ................
-000010e0: 0a01 0801 0401 0a01 0c01 0801 0c01 0a02  ................
-000010f0: 0801 0201 0201 1201 0201 06fc 0606 1001  ................
-00001100: 0601 0a01 1801 1002 0a01 1001 7267 0000  ............rg..
-00001110: 0063 0300 0000 0000 0000 0000 0000 0300  .c..............
-00001120: 0000 0400 0000 4300 0000 7324 0000 007c  ......C...s$...|
-00001130: 026a 0072 1474 017c 007c 017c 0283 0301  .j.r.t.|.|.|....
-00001140: 006e 0c7c 00a0 027c 017c 02a1 0201 0064  .n.|...|.|.....d
-00001150: 0053 0072 1900 0000 2903 da07 7072 6f66  .S.r....)...prof
-00001160: 696c 65da 155f 7275 6e5f 636f 6d6d 616e  ile.._run_comman
-00001170: 645f 7072 6f66 696c 6564 7243 0000 0029  d_profiledrC...)
-00001180: 0372 2800 0000 723f 0000 0072 4000 0000  .r(...r?...r@...
-00001190: 7213 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-000011a0: 6500 0000 a100 0000 7306 0000 0000 0106  e.......s.......
-000011b0: 010e 0272 6500 0000 6303 0000 0000 0000  ...re...c.......
-000011c0: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
-000011d0: 0073 5000 0000 7c02 6a00 721c 7401 6a02  .sP...|.j.r.t.j.
-000011e0: a003 6401 7c02 6a00 9b02 6402 9d03 a101  ..d.|.j...d.....
-000011f0: 0100 7404 8300 7d03 7405 a006 a100 7d04  ..t...}.t.....}.
-00001200: 7c04 a007 6403 7408 8300 7c03 a103 0100  |...d.t...|.....
-00001210: 7c02 6a00 724c 7c04 a009 7c02 6a00 a101  |.j.rL|...|.j...
-00001220: 0100 6400 5300 2904 4e7a 2c61 7975 6765  ..d.S.).Nz,ayuge
-00001230: 7370 6964 6572 746f 6f6c 733a 2077 7269  spidertools: wri
-00001240: 7469 6e67 2063 5072 6f66 696c 6520 7374  ting cProfile st
-00001250: 6174 7320 746f 2072 4200 0000 7a13 636d  ats to rB...z.cm
-00001260: 642e 7275 6e28 6172 6773 2c20 6f70 7473  d.run(args, opts
-00001270: 2929 0a72 6800 0000 724f 0000 00da 0673  )).rh...rO.....s
-00001280: 7464 6572 72da 0577 7269 7465 da06 6c6f  tderr..write..lo
-00001290: 6361 6c73 da08 6350 726f 6669 6c65 5a07  cals..cProfileZ.
-000012a0: 5072 6f66 696c 655a 0672 756e 6374 78da  ProfileZ.runctx.
-000012b0: 0767 6c6f 6261 6c73 5a0a 6475 6d70 5f73  .globalsZ.dump_s
-000012c0: 7461 7473 2905 7228 0000 0072 3f00 0000  tats).r(...r?...
-000012d0: 7240 0000 00da 036c 6f63 da01 7072 1300  r@.....loc..pr..
-000012e0: 0000 7213 0000 0072 1400 0000 7269 0000  ..r....r....ri..
-000012f0: 00a8 0000 0073 1200 0000 0001 0601 0601  .....s..........
-00001300: 0cff 0403 0601 0801 1001 0601 7269 0000  ............ri..
-00001310: 00da 085f 5f6d 6169 6e5f 5f29 0172 2b00  ...__main__).r+.
-00001320: 0000 2902 4e4e 2925 da08 6172 6770 6172  ..).NN)%..argpar
-00001330: 7365 726d 0000 0072 1c00 0000 725f 0000  serm...r....r_..
-00001340: 0072 4f00 0000 722c 0000 005a 0f73 6372  .rO...r,...Z.scr
-00001350: 6170 792e 636f 6d6d 616e 6473 7202 0000  apy.commandsr...
-00001360: 0072 0300 0000 5a0e 7363 7261 7079 2e63  .r....Z.scrapy.c
-00001370: 7261 776c 6572 7204 0000 00da 1173 6372  rawlerr......scr
-00001380: 6170 792e 6578 6365 7074 696f 6e73 7205  apy.exceptionsr.
-00001390: 0000 00da 1173 6372 6170 792e 7574 696c  .....scrapy.util
-000013a0: 732e 6d69 7363 7206 0000 005a 1473 6372  s.miscr....Z.scr
-000013b0: 6170 792e 7574 696c 732e 7072 6f6a 6563  apy.utils.projec
-000013c0: 7472 0700 0000 7208 0000 00da 1373 6372  tr....r......scr
-000013d0: 6170 792e 7574 696c 732e 7079 7468 6f6e  apy.utils.python
-000013e0: 7209 0000 005a 2161 7975 6765 7370 6964  r....Z!ayugespid
-000013f0: 6572 746f 6f6c 732e 636f 6d6d 616e 6473  ertools.commands
-00001400: 2e76 6572 7369 6f6e 720a 0000 00da 0e41  .versionr......A
-00001410: 7267 756d 656e 7450 6172 7365 7272 0b00  rgumentParserr..
-00001420: 0000 7222 0000 0072 2a00 0000 7233 0000  ..r"...r*...r3..
-00001430: 0072 3700 0000 723e 0000 0072 4600 0000  .r7...r>...rF...
-00001440: 724a 0000 0072 4b00 0000 7256 0000 0072  rJ...rK...rV...r
-00001450: 6700 0000 7265 0000 0072 6900 0000 7215  g...re...ri...r.
-00001460: 0000 0072 1300 0000 7213 0000 0072 1300  ...r....r....r..
-00001470: 0000 7214 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00001480: 3e01 0000 0073 3a00 0000 0801 0801 0801  >....s:.........
-00001490: 0801 0802 0801 1001 0c01 0c01 0c01 1001  ................
-000014a0: 0c02 0c03 1209 080e 0809 0a0b 0809 0809  ................
-000014b0: 0808 080f 0806 080b 0a2a 0807 080c 0a01  .........*......
-000014c0: 0201 0a05                                ....
+00000060: 6402 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
+00000070: 0100 6400 6403 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
+00000080: 6404 6c0c 6d0d 5a0d 0100 6400 6405 6c0e  d.l.m.Z...d.d.l.
+00000090: 6d0f 5a0f 0100 6400 6406 6c10 6d11 5a11  m.Z...d.d.l.m.Z.
+000000a0: 6d12 5a12 0100 6400 6407 6c13 6d14 5a14  m.Z...d.d.l.m.Z.
+000000b0: 0100 6400 6408 6c15 6d16 5a16 0100 4700  ..d.d.l.m.Z...G.
+000000c0: 6409 640a 8400 640a 6500 6a17 8303 5a18  d.d...d.e.j...Z.
+000000d0: 640b 640c 8400 5a19 640d 640e 8400 5a1a  d.d...Z.d.d...Z.
+000000e0: 6425 6410 6411 8401 5a1b 6412 6413 8400  d%d.d...Z.d.d...
+000000f0: 5a1c 6414 6415 8400 5a1d 6416 6417 8400  Z.d.d...Z.d.d...
+00000100: 5a1e 6418 6419 8400 5a1f 641a 641b 8400  Z.d.d...Z.d.d...
+00000110: 5a20 641c 641d 8400 5a21 6426 641e 641f  Z d.d...Z!d&d.d.
+00000120: 8401 5a22 6420 6421 8400 5a23 6422 6423  ..Z"d d!..Z#d"d#
+00000130: 8400 5a24 6525 6424 6b02 9001 7224 7a0a  ..Z$e%d$k...r$z.
+00000140: 6522 8300 0100 5700 3500 6514 8300 0100  e"....W.5.e.....
+00000150: 5800 6401 5300 2927 e900 0000 004e 2903  X.d.S.)'.....N).
+00000160: da14 4261 7365 5275 6e53 7069 6465 7243  ..BaseRunSpiderC
+00000170: 6f6d 6d61 6e64 da0d 5363 7261 7079 436f  ommand..ScrapyCo
+00000180: 6d6d 616e 64da 1353 6372 6170 7948 656c  mmand..ScrapyHel
+00000190: 7046 6f72 6d61 7474 6572 2901 da0e 4372  pFormatter)...Cr
+000001a0: 6177 6c65 7250 726f 6365 7373 2901 da0a  awlerProcess)...
+000001b0: 5573 6167 6545 7272 6f72 2901 da0c 7761  UsageError)...wa
+000001c0: 6c6b 5f6d 6f64 756c 6573 2902 da14 6765  lk_modules)...ge
+000001d0: 745f 7072 6f6a 6563 745f 7365 7474 696e  t_project_settin
+000001e0: 6773 da0e 696e 7369 6465 5f70 726f 6a65  gs..inside_proje
+000001f0: 6374 2901 da0f 6761 7262 6167 655f 636f  ct)...garbage_co
+00000200: 6c6c 6563 7429 01da 0a41 7975 436f 6d6d  llect)...AyuComm
+00000210: 616e 6463 0000 0000 0000 0000 0000 0000  andc............
+00000220: 0000 0000 0300 0000 0000 0000 731c 0000  ............s...
+00000230: 0065 005a 0164 005a 0287 0066 0164 0164  .e.Z.d.Z...f.d.d
+00000240: 0284 085a 0387 0004 005a 0453 0029 03da  ...Z.....Z.S.)..
+00000250: 1453 6372 6170 7941 7267 756d 656e 7450  .ScrapyArgumentP
+00000260: 6172 7365 7263 0200 0000 0000 0000 0000  arserc..........
+00000270: 0000 0200 0000 0300 0000 0300 0000 7320  ..............s 
+00000280: 0000 007c 0164 0064 0185 0219 0064 026b  ...|.d.d.....d.k
+00000290: 0272 1464 0053 0074 0083 00a0 017c 01a1  .r.d.S.t.....|..
+000002a0: 0153 0029 034e e902 0000 007a 022d 3a29  .S.).N.....z.-:)
+000002b0: 02da 0573 7570 6572 da0f 5f70 6172 7365  ...super.._parse
+000002c0: 5f6f 7074 696f 6e61 6c29 02da 0473 656c  _optional)...sel
+000002d0: 66da 0a61 7267 5f73 7472 696e 67a9 01da  f..arg_string...
+000002e0: 095f 5f63 6c61 7373 5f5f a900 fa3f 2f72  .__class__...?/r
+000002f0: 6f6f 742f 6d79 7072 6f6a 2f41 7975 6765  oot/myproj/Ayuge
+00000300: 5370 6964 6572 546f 6f6c 732f 6179 7567  SpiderTools/ayug
+00000310: 6573 7069 6465 7274 6f6f 6c73 2f75 7469  espidertools/uti
+00000320: 6c73 2f63 6d64 6c69 6e65 2e70 7972 0f00  ls/cmdline.pyr..
+00000330: 0000 1300 0000 7306 0000 0000 0210 0104  ......s.........
+00000340: 027a 2453 6372 6170 7941 7267 756d 656e  .z$ScrapyArgumen
+00000350: 7450 6172 7365 722e 5f70 6172 7365 5f6f  tParser._parse_o
+00000360: 7074 696f 6e61 6c29 05da 085f 5f6e 616d  ptional)...__nam
+00000370: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000380: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0f00  .__qualname__r..
+00000390: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
+000003a0: 5f72 1400 0000 7214 0000 0072 1200 0000  _r....r....r....
+000003b0: 7215 0000 0072 0c00 0000 1200 0000 7302  r....r........s.
+000003c0: 0000 0008 0172 0c00 0000 6301 0000 0000  .....r....c.....
+000003d0: 0000 0000 0000 0003 0000 0005 0000 0063  ...............c
+000003e0: 0000 0073 5600 0000 7400 7c00 8301 4400  ...sV...t.|...D.
+000003f0: 5d48 7d01 7401 7c01 8301 a002 a100 4400  ]H}.t.|.......D.
+00000400: 5d36 7d02 7403 a004 7c02 a101 7218 7405  ]6}.t...|...r.t.
+00000410: 7c02 7406 8302 7218 7c02 6a07 7c01 6a08  |.t...r.|.j.|.j.
+00000420: 6b02 7218 7c02 7406 7409 6602 6b07 7218  k.r.|.t.t.f.k.r.
+00000430: 7c02 5600 0100 7118 7108 6400 5300 a901  |.V...q.q.d.S...
+00000440: 4e29 0a72 0700 0000 da04 7661 7273 da06  N).r......vars..
+00000450: 7661 6c75 6573 da07 696e 7370 6563 74da  values..inspect.
+00000460: 0769 7363 6c61 7373 da0a 6973 7375 6263  .isclass..issubc
+00000470: 6c61 7373 7203 0000 0072 1700 0000 7216  lassr....r....r.
+00000480: 0000 0072 0200 0000 2903 da0b 6d6f 6475  ...r....)...modu
+00000490: 6c65 5f6e 616d 65da 066d 6f64 756c 65da  le_name..module.
+000004a0: 036f 626a 7214 0000 0072 1400 0000 7215  .objr....r....r.
+000004b0: 0000 00da 155f 6974 6572 5f63 6f6d 6d61  ....._iter_comma
+000004c0: 6e64 5f63 6c61 7373 6573 1b00 0000 7316  nd_classes....s.
+000004d0: 0000 0000 030c 0110 0208 ff02 0208 fe02  ................
+000004e0: 030a fd02 040a fc02 0672 2300 0000 6302  .........r#...c.
+000004f0: 0000 0000 0000 0000 0000 0005 0000 0004  ................
+00000500: 0000 0043 0000 0073 3a00 0000 6900 7d02  ...C...s:...i.}.
+00000510: 7400 7c00 8301 4400 5d28 7d03 7c01 731a  t.|...D.](}.|.s.
+00000520: 7c03 6a01 730c 7c03 6a02 a003 6401 a101  |.j.s.|.j...d...
+00000530: 6402 1900 7d04 7c03 8300 7c02 7c04 3c00  d...}.|...|.|.<.
+00000540: 710c 7c02 5300 2903 4eda 012e e9ff ffff  q.|.S.).N.......
+00000550: ff29 0472 2300 0000 5a10 7265 7175 6972  .).r#...Z.requir
+00000560: 6573 5f70 726f 6a65 6374 7217 0000 00da  es_projectr.....
+00000570: 0573 706c 6974 2905 7221 0000 00da 0969  .split).r!.....i
+00000580: 6e70 726f 6a65 6374 da01 64da 0363 6d64  nproject..d..cmd
+00000590: da07 636d 646e 616d 6572 1400 0000 7214  ..cmdnamer....r.
+000005a0: 0000 0072 1500 0000 da19 5f67 6574 5f63  ...r......_get_c
+000005b0: 6f6d 6d61 6e64 735f 6672 6f6d 5f6d 6f64  ommands_from_mod
+000005c0: 756c 6529 0000 0073 0c00 0000 0001 0401  ule)...s........
+000005d0: 0c01 0a01 1001 0c01 722b 0000 00fa 1961  ........r+.....a
+000005e0: 7975 6765 7370 6964 6572 746f 6f6c 732e  yugespidertools.
+000005f0: 636f 6d6d 616e 6473 6302 0000 0000 0000  commandsc.......
+00000600: 0000 0000 0005 0000 0004 0000 0043 0000  .............C..
+00000610: 0073 4800 0000 6900 7d02 7400 a001 7c01  .sH...i.}.t...|.
+00000620: a101 4400 5d34 7d03 7c03 a002 a100 7d04  ..D.]4}.|.....}.
+00000630: 7403 a004 7c04 a101 7232 7c04 8300 7c02  t...|...r2|...|.
+00000640: 7c03 6a05 3c00 710e 7406 6401 7c03 6a05  |.j.<.q.t.d.|.j.
+00000650: 9b00 9d02 8301 8201 710e 7c02 5300 2902  ........q.|.S.).
+00000660: 4e7a 1449 6e76 616c 6964 2065 6e74 7279  Nz.Invalid entry
+00000670: 2070 6f69 6e74 2029 07da 0d70 6b67 5f72   point )...pkg_r
+00000680: 6573 6f75 7263 6573 5a11 6974 6572 5f65  esourcesZ.iter_e
+00000690: 6e74 7279 5f70 6f69 6e74 73da 046c 6f61  ntry_points..loa
+000006a0: 6472 1d00 0000 721e 0000 00da 046e 616d  dr....r......nam
+000006b0: 65da 0945 7863 6570 7469 6f6e 2905 7227  e..Exception).r'
+000006c0: 0000 00da 0567 726f 7570 da04 636d 6473  .....group..cmds
+000006d0: da0b 656e 7472 795f 706f 696e 7472 2200  ..entry_pointr".
+000006e0: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
+000006f0: 00da 1f5f 6765 745f 636f 6d6d 616e 6473  ..._get_commands
+00000700: 5f66 726f 6d5f 656e 7472 795f 706f 696e  _from_entry_poin
+00000710: 7473 3200 0000 730e 0000 0000 0104 010e  ts2...s.........
+00000720: 0108 010a 010e 0212 0172 3400 0000 6302  .........r4...c.
+00000730: 0000 0000 0000 0000 0000 0004 0000 0005  ................
+00000740: 0000 0043 0000 0073 3800 0000 7400 6401  ...C...s8...t.d.
+00000750: 7c01 8302 7d02 7c02 a001 7402 7c01 8301  |...}.|...t.|...
+00000760: a101 0100 7c00 6402 1900 7d03 7c03 7234  ....|.d...}.|.r4
+00000770: 7c02 a001 7400 7c03 7c01 8302 a101 0100  |...t.|.|.......
+00000780: 7c02 5300 2903 4e72 2c00 0000 da0f 434f  |.S.).Nr,.....CO
+00000790: 4d4d 414e 4453 5f4d 4f44 554c 4529 0372  MMANDS_MODULE).r
+000007a0: 2b00 0000 da06 7570 6461 7465 7234 0000  +.....updater4..
+000007b0: 0029 04da 0873 6574 7469 6e67 7372 2700  .)...settingsr'.
+000007c0: 0000 7232 0000 005a 0b63 6d64 735f 6d6f  ..r2...Z.cmds_mo
+000007d0: 6475 6c65 7214 0000 0072 1400 0000 7215  duler....r....r.
+000007e0: 0000 00da 125f 6765 745f 636f 6d6d 616e  ....._get_comman
+000007f0: 6473 5f64 6963 743d 0000 0073 0c00 0000  ds_dict=...s....
+00000800: 0001 0a01 0e01 0801 0401 1001 7238 0000  ............r8..
+00000810: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
+00000820: 0000 0400 0000 4300 0000 733a 0000 0064  ......C...s:...d
+00000830: 017d 017c 0064 0264 0085 0219 0044 005d  .}.|.d.d.....D.]
+00000840: 247d 027c 02a0 0064 03a1 0173 2c7c 007c  $}.|...d...s,|.|
+00000850: 013d 007c 0202 0001 0053 007c 0164 0237  .=.|.....S.|.d.7
+00000860: 007d 0171 1064 0053 0029 044e 7201 0000  .}.q.d.S.).Nr...
+00000870: 00e9 0100 0000 fa01 2d29 01da 0a73 7461  ........-)...sta
+00000880: 7274 7377 6974 6829 03da 0461 7267 76da  rtswith)...argv.
+00000890: 0169 da03 6172 6772 1400 0000 7214 0000  .i..argr....r...
+000008a0: 0072 1500 0000 da11 5f70 6f70 5f63 6f6d  .r......_pop_com
+000008b0: 6d61 6e64 5f6e 616d 6546 0000 0073 0c00  mand_nameF...s..
+000008c0: 0000 0001 0401 1001 0a01 0601 0801 723f  ..............r?
+000008d0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+000008e0: 0300 0000 0600 0000 4300 0000 733e 0000  ........C...s>..
+000008f0: 0074 0083 00a0 01a1 007d 027c 0172 2a74  .t.......}.|.r*t
+00000900: 0264 017c 029b 0064 027c 0064 0319 009b  .d.|...d.|.d....
+00000910: 0064 049d 0583 0101 006e 1074 0264 017c  .d.......n.t.d.|
+00000920: 029b 0064 059d 0383 0101 0064 0053 0029  ...d.......d.S.)
+00000930: 064e 7a11 4179 7567 6553 7069 6465 7254  .Nz.AyugeSpiderT
+00000940: 6f6f 6c73 207a 1320 2d20 6163 7469 7665  ools z. - active
+00000950: 2070 726f 6a65 6374 3a20 da08 424f 545f   project: ..BOT_
+00000960: 4e41 4d45 da01 0a7a 1520 2d20 6e6f 2061  NAME...z. - no a
+00000970: 6374 6976 6520 7072 6f6a 6563 740a 2903  ctive project.).
+00000980: 720b 0000 00da 085f 7665 7273 696f 6eda  r......_version.
+00000990: 0570 7269 6e74 2903 7237 0000 0072 2700  .print).r7...r'.
+000009a0: 0000 da07 7665 7273 696f 6e72 1400 0000  ....versionr....
+000009b0: 7214 0000 0072 1500 0000 da0d 5f70 7269  r....r......_pri
+000009c0: 6e74 5f68 6561 6465 724f 0000 0073 0800  nt_headerO...s..
+000009d0: 0000 0001 0a01 0401 1c02 7245 0000 0063  ..........rE...c
+000009e0: 0200 0000 0000 0000 0000 0000 0500 0000  ................
+000009f0: 0700 0000 4300 0000 7380 0000 0074 007c  ....C...s....t.|
+00000a00: 007c 0183 0201 0074 0164 0183 0101 0074  .|.....t.d.....t
+00000a10: 0164 0283 0101 0074 0164 0383 0101 0074  .d.....t.d.....t
+00000a20: 027c 007c 0183 027d 0274 037c 02a0 04a1  .|.|...}.t.|....
+00000a30: 0083 0144 005d 225c 027d 037d 0474 0164  ...D.]"\.}.}.t.d
+00000a40: 047c 0364 059b 0464 067c 04a0 05a1 009b  .|.d...d.|......
+00000a50: 009d 0483 0101 0071 387c 0173 6e74 0183  .......q8|.snt..
+00000a60: 0001 0074 0164 0783 0101 0074 0183 0001  ...t.d.....t....
+00000a70: 0074 0164 0883 0101 0064 0053 0029 094e  .t.d.....d.S.).N
+00000a80: 7a06 5573 6167 653a 7a23 2020 6179 7567  z.Usage:z#  ayug
+00000a90: 6520 3c63 6f6d 6d61 6e64 3e20 5b6f 7074  e <command> [opt
+00000aa0: 696f 6e73 5d20 5b61 7267 735d 0a7a 1341  ions] [args].z.A
+00000ab0: 7661 696c 6162 6c65 2063 6f6d 6d61 6e64  vailable command
+00000ac0: 733a 7a02 2020 7a03 3c31 33fa 0120 7a47  s:z.  z.<13.. zG
+00000ad0: 2020 5b20 6d6f 7265 205d 2020 2020 2020    [ more ]      
+00000ae0: 4d6f 7265 2063 6f6d 6d61 6e64 7320 6176  More commands av
+00000af0: 6169 6c61 626c 6520 7768 656e 2072 756e  ailable when run
+00000b00: 2066 726f 6d20 7072 6f6a 6563 7420 6469   from project di
+00000b10: 7265 6374 6f72 797a 3955 7365 2022 6179  rectoryz9Use "ay
+00000b20: 7567 6520 3c63 6f6d 6d61 6e64 3e20 2d68  uge <command> -h
+00000b30: 2220 746f 2073 6565 206d 6f72 6520 696e  " to see more in
+00000b40: 666f 2061 626f 7574 2061 2063 6f6d 6d61  fo about a comma
+00000b50: 6e64 2906 7245 0000 0072 4300 0000 7238  nd).rE...rC...r8
+00000b60: 0000 00da 0673 6f72 7465 64da 0569 7465  .....sorted..ite
+00000b70: 6d73 5a0a 7368 6f72 745f 6465 7363 2905  msZ.short_desc).
+00000b80: 7237 0000 0072 2700 0000 7232 0000 0072  r7...r'...r2...r
+00000b90: 2a00 0000 5a08 636d 6463 6c61 7373 7214  *...Z.cmdclassr.
+00000ba0: 0000 0072 1400 0000 7215 0000 00da 0f5f  ...r....r......_
+00000bb0: 7072 696e 745f 636f 6d6d 616e 6473 5700  print_commandsW.
+00000bc0: 0000 7318 0000 0000 010a 0108 0108 0108  ..s.............
+00000bd0: 010a 0114 011c 0104 0106 0108 0106 0172  ...............r
+00000be0: 4900 0000 6303 0000 0000 0000 0000 0000  I...c...........
+00000bf0: 0003 0000 0004 0000 0043 0000 0073 2600  .........C...s&.
+00000c00: 0000 7400 7c00 7c02 8302 0100 7401 6401  ..t.|.|.....t.d.
+00000c10: 7c01 9b00 6402 9d03 8301 0100 7401 6403  |...d.......t.d.
+00000c20: 8301 0100 6400 5300 2904 4e7a 1155 6e6b  ....d.S.).Nz.Unk
+00000c30: 6e6f 776e 2063 6f6d 6d61 6e64 3a20 7241  nown command: rA
+00000c40: 0000 007a 2555 7365 2022 6179 7567 6522  ...z%Use "ayuge"
+00000c50: 2074 6f20 7365 6520 6176 6169 6c61 626c   to see availabl
+00000c60: 6520 636f 6d6d 616e 6473 2902 7245 0000  e commands).rE..
+00000c70: 0072 4300 0000 2903 7237 0000 0072 2a00  .rC...).r7...r*.
+00000c80: 0000 7227 0000 0072 1400 0000 7214 0000  ..r'...r....r...
+00000c90: 0072 1500 0000 da16 5f70 7269 6e74 5f75  .r......_print_u
+00000ca0: 6e6b 6e6f 776e 5f63 6f6d 6d61 6e64 6600  nknown_commandf.
+00000cb0: 0000 7306 0000 0000 010a 0110 0172 4a00  ..s..........rJ.
+00000cc0: 0000 6302 0000 0000 0000 0000 0000 0005  ..c.............
+00000cd0: 0000 000a 0000 004f 0000 0073 6400 0000  .......O...sd...
+00000ce0: 7a0e 7c01 7c02 7c03 8e01 0100 5700 6e50  z.|.|.|.....W.nP
+00000cf0: 0400 7400 6b0a 725e 0100 7d04 0100 7a32  ..t.k.r^..}...z2
+00000d00: 7401 7c04 8301 7236 7c00 a002 7401 7c04  t.|...r6|...t.|.
+00000d10: 8301 a101 0100 7c04 6a03 7244 7c00 a003  ......|.j.rD|...
+00000d20: a100 0100 7404 a005 6401 a101 0100 5700  ....t...d.....W.
+00000d30: 3500 6400 7d04 7e04 5800 5900 6e02 5800  5.d.}.~.X.Y.n.X.
+00000d40: 6400 5300 2902 4e72 0d00 0000 2906 7206  d.S.).Nr....).r.
+00000d50: 0000 00da 0373 7472 da05 6572 726f 72da  .....str..error.
+00000d60: 0a70 7269 6e74 5f68 656c 70da 0373 7973  .print_help..sys
+00000d70: da04 6578 6974 2905 da06 7061 7273 6572  ..exit)...parser
+00000d80: da04 6675 6e63 da01 61da 026b 77da 0165  ..func..a..kw..e
+00000d90: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+00000da0: 0f5f 7275 6e5f 7072 696e 745f 6865 6c70  ._run_print_help
+00000db0: 6c00 0000 7310 0000 0000 0102 010e 0110  l...s...........
+00000dc0: 0108 010e 0106 0108 0172 5500 0000 6302  .........rU...c.
+00000dd0: 0000 0000 0000 0000 0000 000a 0000 0008  ................
+00000de0: 0000 0043 0000 0073 3601 0000 7c00 6400  ...C...s6...|.d.
+00000df0: 6b08 720e 7400 6a01 7d00 7c01 6400 6b08  k.r.t.j.}.|.d.k.
+00000e00: 7248 7402 8300 7d01 7a0e 7403 6a04 6401  rHt...}.z.t.j.d.
+00000e10: 1900 7d02 5700 6e14 0400 7405 6b0a 723e  ..}.W.n...t.k.r>
+00000e20: 0100 0100 0100 5900 6e0a 5800 7c02 7c01  ......Y.n.X.|.|.
+00000e30: 6401 3c00 7406 8300 7d03 7407 7c01 7c03  d.<.t...}.t.|.|.
+00000e40: 8302 7d04 7408 7c00 8301 7d05 7c05 737a  ..}.t.|...}.|.sz
+00000e50: 7409 7c01 7c03 8302 0100 7400 a00a 6402  t.|.|.....t...d.
+00000e60: a101 0100 6e1e 7c05 7c04 6b07 7298 740b  ....n.|.|.k.r.t.
+00000e70: 7c01 7c05 7c03 8303 0100 7400 a00a 6403  |.|.|.....t...d.
+00000e80: a101 0100 7c04 7c05 1900 7d06 740c 740d  ....|.|...}.t.t.
+00000e90: 6404 7c05 9b00 6405 7c06 a00e a100 9b00  d.|...d.|.......
+00000ea0: 9d04 6406 7c06 a00f a100 6407 8d04 7d07  ..d.|.....d...}.
+00000eb0: 7c01 6a10 7c06 6a11 6408 6409 8d02 0100  |.j.|.j.d.d.....
+00000ec0: 7c01 7c06 5f12 7c06 a013 7c07 a101 0100  |.|._.|...|.....
+00000ed0: 7c07 6a14 7c00 640a 6400 8502 1900 640b  |.j.|.d.d.....d.
+00000ee0: 8d01 5c02 7d08 7d09 7415 7c07 7c06 6a16  ..\.}.}.t.|.|.j.
+00000ef0: 7c09 7c08 8304 0100 7417 7c01 8301 7c06  |.|.....t.|...|.
+00000f00: 5f18 7415 7c07 7419 7c06 7c09 7c08 8305  _.t.|.t.|.|.|...
+00000f10: 0100 7400 a00a 7c06 6a1a a101 0100 6400  ..t...|.j.....d.
+00000f20: 5300 290c 4eda 0645 4449 544f 5272 0100  S.).N..EDITORr..
+00000f30: 0000 720d 0000 007a 0661 7975 6765 2072  ..r....z.ayuge r
+00000f40: 4600 0000 da07 7265 736f 6c76 6529 04da  F.....resolve)..
+00000f50: 0f66 6f72 6d61 7474 6572 5f63 6c61 7373  .formatter_class
+00000f60: da05 7573 6167 65da 1063 6f6e 666c 6963  ..usage..conflic
+00000f70: 745f 6861 6e64 6c65 72da 0b64 6573 6372  t_handler..descr
+00000f80: 6970 7469 6f6e da07 636f 6d6d 616e 6429  iption..command)
+00000f90: 01da 0870 7269 6f72 6974 7972 3900 0000  ...priorityr9...
+00000fa0: 2901 da04 6172 6773 291b 724e 0000 0072  )...args).rN...r
+00000fb0: 3c00 0000 7208 0000 00da 026f 73da 0765  <...r......os..e
+00000fc0: 6e76 6972 6f6e da08 4b65 7945 7272 6f72  nviron..KeyError
+00000fd0: 7209 0000 0072 3800 0000 723f 0000 0072  r....r8...r?...r
+00000fe0: 4900 0000 724f 0000 0072 4a00 0000 720c  I...rO...rJ...r.
+00000ff0: 0000 0072 0400 0000 5a06 7379 6e74 6178  ...r....Z.syntax
+00001000: 5a09 6c6f 6e67 5f64 6573 63da 0773 6574  Z.long_desc..set
+00001010: 6469 6374 da10 6465 6661 756c 745f 7365  dict..default_se
+00001020: 7474 696e 6773 7237 0000 005a 0b61 6464  ttingsr7...Z.add
+00001030: 5f6f 7074 696f 6e73 da10 7061 7273 655f  _options..parse_
+00001040: 6b6e 6f77 6e5f 6172 6773 7255 0000 005a  known_argsrU...Z
+00001050: 0f70 726f 6365 7373 5f6f 7074 696f 6e73  .process_options
+00001060: 7205 0000 005a 0f63 7261 776c 6572 5f70  r....Z.crawler_p
+00001070: 726f 6365 7373 da0c 5f72 756e 5f63 6f6d  rocess.._run_com
+00001080: 6d61 6e64 da08 6578 6974 636f 6465 290a  mand..exitcode).
+00001090: 723c 0000 0072 3700 0000 5a06 6564 6974  r<...r7...Z.edit
+000010a0: 6f72 7227 0000 0072 3200 0000 722a 0000  orr'...r2...r*..
+000010b0: 0072 2900 0000 7250 0000 00da 046f 7074  .r)...rP.....opt
+000010c0: 7372 5e00 0000 7214 0000 0072 1400 0000  sr^...r....r....
+000010d0: 7215 0000 00da 0765 7865 6375 7465 7700  r......executew.
+000010e0: 0000 7342 0000 0000 0108 0106 0208 0106  ..sB............
+000010f0: 0202 010e 010e 0106 0208 0206 010a 0108  ................
+00001100: 0104 010a 010c 0108 010c 010a 0208 0102  ................
+00001110: 0102 0112 0102 0106 fc06 0610 0106 010a  ................
+00001120: 0118 0110 020a 0110 0172 6800 0000 6303  .........rh...c.
+00001130: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00001140: 0000 0043 0000 0073 2400 0000 7c02 6a00  ...C...s$...|.j.
+00001150: 7214 7401 7c00 7c01 7c02 8303 0100 6e0c  r.t.|.|.|.....n.
+00001160: 7c00 a002 7c01 7c02 a102 0100 6400 5300  |...|.|.....d.S.
+00001170: 721a 0000 0029 03da 0770 726f 6669 6c65  r....)...profile
+00001180: da15 5f72 756e 5f63 6f6d 6d61 6e64 5f70  .._run_command_p
+00001190: 726f 6669 6c65 64da 0372 756e 2903 7229  rofiled..run).r)
+000011a0: 0000 0072 5e00 0000 7267 0000 0072 1400  ...r^...rg...r..
+000011b0: 0000 7214 0000 0072 1500 0000 7265 0000  ..r....r....re..
+000011c0: 00a1 0000 0073 0600 0000 0001 0601 0e02  .....s..........
+000011d0: 7265 0000 0063 0300 0000 0000 0000 0000  re...c..........
+000011e0: 0000 0500 0000 0500 0000 4300 0000 7350  ..........C...sP
+000011f0: 0000 007c 026a 0072 1c74 016a 02a0 0364  ...|.j.r.t.j...d
+00001200: 017c 026a 009b 0264 029d 03a1 0101 0074  .|.j...d.......t
+00001210: 0483 007d 0374 05a0 06a1 007d 047c 04a0  ...}.t.....}.|..
+00001220: 0764 0374 0883 007c 03a1 0301 007c 026a  .d.t...|.....|.j
+00001230: 0072 4c7c 04a0 097c 026a 00a1 0101 0064  .rL|...|.j.....d
+00001240: 0053 0029 044e 7a2c 6179 7567 6573 7069  .S.).Nz,ayugespi
+00001250: 6465 7274 6f6f 6c73 3a20 7772 6974 696e  dertools: writin
+00001260: 6720 6350 726f 6669 6c65 2073 7461 7473  g cProfile stats
+00001270: 2074 6f20 7241 0000 007a 1363 6d64 2e72   to rA...z.cmd.r
+00001280: 756e 2861 7267 732c 206f 7074 7329 290a  un(args, opts)).
+00001290: 7269 0000 0072 4e00 0000 da06 7374 6465  ri...rN.....stde
+000012a0: 7272 da05 7772 6974 65da 066c 6f63 616c  rr..write..local
+000012b0: 73da 0863 5072 6f66 696c 655a 0750 726f  s..cProfileZ.Pro
+000012c0: 6669 6c65 5a06 7275 6e63 7478 da07 676c  fileZ.runctx..gl
+000012d0: 6f62 616c 735a 0a64 756d 705f 7374 6174  obalsZ.dump_stat
+000012e0: 7329 0572 2900 0000 725e 0000 0072 6700  s).r)...r^...rg.
+000012f0: 0000 da03 6c6f 63da 0170 7214 0000 0072  ....loc..pr....r
+00001300: 1400 0000 7215 0000 0072 6a00 0000 a800  ....r....rj.....
+00001310: 0000 7312 0000 0000 0106 0106 010c ff04  ..s.............
+00001320: 0306 0108 0110 0106 0172 6a00 0000 da08  .........rj.....
+00001330: 5f5f 6d61 696e 5f5f 2901 722c 0000 0029  __main__).r,...)
+00001340: 024e 4e29 26da 0861 7267 7061 7273 6572  .NN)&..argparser
+00001350: 6f00 0000 721d 0000 0072 5f00 0000 724e  o...r....r_...rN
+00001360: 0000 0072 2d00 0000 5a0f 7363 7261 7079  ...r-...Z.scrapy
+00001370: 2e63 6f6d 6d61 6e64 7372 0200 0000 7203  .commandsr....r.
+00001380: 0000 0072 0400 0000 5a0e 7363 7261 7079  ...r....Z.scrapy
+00001390: 2e63 7261 776c 6572 7205 0000 00da 1173  .crawlerr......s
+000013a0: 6372 6170 792e 6578 6365 7074 696f 6e73  crapy.exceptions
+000013b0: 7206 0000 00da 1173 6372 6170 792e 7574  r......scrapy.ut
+000013c0: 696c 732e 6d69 7363 7207 0000 005a 1473  ils.miscr....Z.s
+000013d0: 6372 6170 792e 7574 696c 732e 7072 6f6a  crapy.utils.proj
+000013e0: 6563 7472 0800 0000 7209 0000 00da 1373  ectr....r......s
+000013f0: 6372 6170 792e 7574 696c 732e 7079 7468  crapy.utils.pyth
+00001400: 6f6e 720a 0000 005a 2161 7975 6765 7370  onr....Z!ayugesp
+00001410: 6964 6572 746f 6f6c 732e 636f 6d6d 616e  idertools.comman
+00001420: 6473 2e76 6572 7369 6f6e 720b 0000 00da  ds.versionr.....
+00001430: 0e41 7267 756d 656e 7450 6172 7365 7272  .ArgumentParserr
+00001440: 0c00 0000 7223 0000 0072 2b00 0000 7234  ....r#...r+...r4
+00001450: 0000 0072 3800 0000 723f 0000 0072 4500  ...r8...r?...rE.
+00001460: 0000 7249 0000 0072 4a00 0000 7255 0000  ..rI...rJ...rU..
+00001470: 0072 6800 0000 7265 0000 0072 6a00 0000  .rh...re...rj...
+00001480: 7216 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
+00001490: 1400 0000 7215 0000 00da 083c 6d6f 6475  ....r......<modu
+000014a0: 6c65 3e01 0000 0073 3a00 0000 0801 0801  le>....s:.......
+000014b0: 0801 0801 0802 0801 1401 0c01 0c01 0c01  ................
+000014c0: 1001 0c02 0c03 1209 080e 0809 0a0b 0809  ................
+000014d0: 0809 0808 080f 0806 080b 0a2a 0807 080c  ...........*....
+000014e0: 0a01 0201 0a05                           ......
```

### Comparing `ayugespidertools-2.0.3/ayugespidertools/utils/cmdline.py` & `ayugespidertools-2.1.0/ayugespidertools/utils/cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import cProfile
 import inspect
 import os
 import sys
 
 import pkg_resources
-from scrapy.commands import ScrapyCommand, ScrapyHelpFormatter
+from scrapy.commands import BaseRunSpiderCommand, ScrapyCommand, ScrapyHelpFormatter
 from scrapy.crawler import CrawlerProcess
 from scrapy.exceptions import UsageError
 from scrapy.utils.misc import walk_modules
 from scrapy.utils.project import get_project_settings, inside_project
 from scrapy.utils.python import garbage_collect
 
 from ayugespidertools.commands.version import AyuCommand
@@ -21,23 +21,23 @@
         if arg_string[:2] == "-:":
             return None
 
         return super()._parse_optional(arg_string)
 
 
 def _iter_command_classes(module_name):
-    # TODO: add `name` attribute to commands and and merge this function with
+    # TODO: add `name` attribute to commands and merge this function with
     # scrapy.utils.spider.iter_spider_classes
     for module in walk_modules(module_name):
         for obj in vars(module).values():
             if (
                 inspect.isclass(obj)
                 and issubclass(obj, ScrapyCommand)
                 and obj.__module__ == module.__name__
-                and not obj == ScrapyCommand
+                and obj not in (ScrapyCommand, BaseRunSpiderCommand)
             ):
                 yield obj
 
 
 def _get_commands_from_module(module, inproject):
     d = {}
     for cmd in _iter_command_classes(module):
@@ -73,17 +73,17 @@
         if not arg.startswith("-"):
             del argv[i]
             return arg
         i += 1
 
 
 def _print_header(settings, inproject):
-    version = AyuCommand().run(args=None, opts=None)
+    version = AyuCommand()._version()
     if inproject:
-        print(f"AyugeSpiderTools {version} - project: {settings['BOT_NAME']}\n")
+        print(f"AyugeSpiderTools {version} - active project: {settings['BOT_NAME']}\n")
     else:
         print(f"AyugeSpiderTools {version} - no active project\n")
 
 
 def _print_commands(settings, inproject):
     _print_header(settings, inproject)
     print("Usage:")
```

### Comparing `ayugespidertools-2.0.3/ayugespidertools/verificationcode.py` & `ayugespidertools-2.1.0/ayugespidertools/verificationcode.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.3/pyproject.toml` & `ayugespidertools-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AyugeSpiderTools"
-version = "2.0.3"
+version = "2.1.0"
 description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。"
 authors = ["ayuge <ayugesheng@gmail.com>"]
 maintainers = ["ayuge <ayugesheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ayugespidertools"}]
 repository = "https://github.com/shengchenyang/AyugeSpiderTools"
 documentation = "https://ayugespidertools.readthedocs.io/en/latest/"
@@ -18,15 +18,15 @@
 PyMySQL = "^1.0.2"
 environs = "^9.5.0"
 loguru = "^0.6.0"
 numpy = "1.24.2"
 PyExecJS = "^1.5.1"
 requests = "^2.28.1"
 Pillow = "^9.2.0"
-Scrapy = "2.8.0"
+Scrapy = "2.9.0"
 pandas = "^1.5.0"
 WorkWeixinRobot = "^1.0.1"
 retrying = "^1.3.3"
 SQLAlchemy = "^1.4.41"
 DBUtils = "^3.0.2"
 itemadapter = "^0.7.0"
 aiohttp = "^3.8.3"
```

### Comparing `ayugespidertools-2.0.3/PKG-INFO` & `ayugespidertools-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayugespidertools
-Version: 2.0.3
+Version: 2.1.0
 Summary: scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。
 Home-page: https://www.ayuge.top/mkdocs-material/
 Keywords: crawler,scraping,twisted,aiohttp,asyncio,scrapy,aiomysql,mmh3
 Author: ayuge
 Author-email: ayugesheng@gmail.com
 Maintainer: ayuge
 Maintainer-email: ayugesheng@gmail.com
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: DBUtils (>=3.0.2,<4.0.0)
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
 Requires-Dist: PyExecJS (>=1.5.1,<2.0.0)
 Requires-Dist: PyMySQL (>=1.0.2,<2.0.0)
 Requires-Dist: SQLAlchemy (>=1.4.41,<2.0.0)
-Requires-Dist: Scrapy (==2.8.0)
+Requires-Dist: Scrapy (==2.9.0)
 Requires-Dist: WorkWeixinRobot (>=1.0.1,<2.0.0)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiomysql (>=0.1.1,<0.2.0)
 Requires-Dist: attrs (>=22.2.0,<23.0.0)
 Requires-Dist: environs (>=9.5.0,<10.0.0)
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0)
 Requires-Dist: itemadapter (>=0.7.0,<0.8.0)
```

