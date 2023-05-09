# Comparing `tmp/irails-1.2.1.tar.gz` & `tmp/irails-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.2.1.tar", last modified: Tue May  9 06:53:18 2023, max compression
+gzip compressed data, was "irails-1.2.2.tar", last modified: Tue May  9 15:26:05 2023, max compression
```

## Comparing `irails-1.2.1.tar` & `irails-1.2.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.695625 irails-1.2.1/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7120 2023-05-09 06:53:18.694633 irails-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     6339 2023-05-09 06:53:18.000000 irails-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.616999 irails-1.2.1/irails/
--rw-rw-rw-   0        0        0      325 2023-05-09 06:52:52.000000 irails-1.2.1/irails/__init__.py
--rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.2.1/irails/_i18n.py
--rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.2.1/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.2.1/irails/_utils.py
--rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.2.1/irails/auth.py
--rw-rw-rw-   0        0        0    11570 2023-05-07 08:42:59.000000 irails-1.2.1/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.629977 irails-1.2.1/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.630961 irails-1.2.1/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.2.1/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.2.1/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.2.1/irails/cbv.py
--rw-rw-rw-   0        0        0     7252 2023-05-09 06:43:06.000000 irails-1.2.1/irails/config.py
--rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.2.1/irails/controller_utils.py
--rw-rw-rw-   0        0        0    30828 2023-05-08 14:26:29.000000 irails-1.2.1/irails/core.py
--rw-rw-rw-   0        0        0     6285 2023-05-08 14:12:16.000000 irails-1.2.1/irails/database.py
--rw-rw-rw-   0        0        0     8655 2023-05-09 06:39:34.000000 irails-1.2.1/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.2.1/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.2.1/irails/midware_session.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.2.1/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.639939 irails-1.2.1/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.2.1/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7813 2023-05-06 13:37:52.000000 irails-1.2.1/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.2.1/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     6836 2023-05-07 08:08:21.000000 irails-1.2.1/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.2.1/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1321 2023-05-04 04:28:43.000000 irails-1.2.1/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.2.1/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.585957 irails-1.2.1/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.651906 irails-1.2.1/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      233 2023-05-05 05:43:26.000000 irails-1.2.1/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.2.1/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.2.1/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.2.1/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.2.1/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.2.1/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.2.1/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.2.1/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.655896 irails-1.2.1/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.2.1/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.656892 irails-1.2.1/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.2.1/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.668381 irails-1.2.1/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.2.1/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.2.1/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.2.1/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.2.1/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.2.1/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      835 2023-04-30 12:07:18.000000 irails-1.2.1/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      665 2023-05-09 06:45:32.000000 irails-1.2.1/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.2.1/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.2.1/irails/scripts/tpls/project/configs/upload.yaml
--rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.2.1/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.670376 irails-1.2.1/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.2.1/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.2.1/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.673367 irails-1.2.1/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.590944 irails-1.2.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.679509 irails-1.2.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.2.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.687370 irails-1.2.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.2.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.2.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.2.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.591943 irails-1.2.1/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.690361 irails-1.2.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.2.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.2.1/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.626975 irails-1.2.1/irails.egg-info/
--rw-rw-rw-   0        0        0     7120 2023-05-09 06:53:18.000000 irails-1.2.1/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2135 2023-05-09 06:53:18.000000 irails-1.2.1/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 06:53:18.000000 irails-1.2.1/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-09 06:53:18.000000 irails-1.2.1/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      753 2023-05-09 06:53:18.000000 irails-1.2.1/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-09 06:53:18.000000 irails-1.2.1/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 06:53:18.695625 irails-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2955 2023-05-03 14:33:36.000000 irails-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.319811 irails-1.2.2/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5079 2023-05-09 15:26:05.318814 irails-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4296 2023-05-09 11:36:53.000000 irails-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.261651 irails-1.2.2/irails/
+-rw-rw-rw-   0        0        0      334 2023-05-09 15:25:50.000000 irails-1.2.2/irails/__init__.py
+-rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.2.2/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.2.2/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.2.2/irails/_utils.py
+-rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.2.2/irails/auth.py
+-rw-rw-rw-   0        0        0    11570 2023-05-07 08:42:59.000000 irails-1.2.2/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.271694 irails-1.2.2/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.272692 irails-1.2.2/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.2.2/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.2.2/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.2.2/irails/cbv.py
+-rw-rw-rw-   0        0        0     7252 2023-05-09 06:43:06.000000 irails-1.2.2/irails/config.py
+-rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.2.2/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    30828 2023-05-08 14:26:29.000000 irails-1.2.2/irails/core.py
+-rw-rw-rw-   0        0        0     6285 2023-05-08 14:12:16.000000 irails-1.2.2/irails/database.py
+-rw-rw-rw-   0        0        0     8655 2023-05-09 06:39:34.000000 irails-1.2.2/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.2.2/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.2.2/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.2.2/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.279923 irails-1.2.2/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.2.2/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7803 2023-05-09 15:18:47.000000 irails-1.2.2/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.2.2/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     6836 2023-05-07 08:08:21.000000 irails-1.2.2/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.2.2/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1321 2023-05-04 04:28:43.000000 irails-1.2.2/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.2.2/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.233710 irails-1.2.2/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.288894 irails-1.2.2/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.2.2/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.2.2/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.2.2/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.2.2/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.2.2/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.2.2/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.2.2/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.2.2/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.290888 irails-1.2.2/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.2.2/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.291885 irails-1.2.2/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.2.2/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.302856 irails-1.2.2/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.2.2/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.2.2/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.2.2/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.2.2/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.2.2/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      835 2023-04-30 12:07:18.000000 irails-1.2.2/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      665 2023-05-09 06:45:32.000000 irails-1.2.2/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.2.2/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.2.2/irails/scripts/tpls/project/configs/upload.yaml
+-rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.2.2/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.304851 irails-1.2.2/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.2.2/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.2.2/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.307843 irails-1.2.2/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.237700 irails-1.2.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.310836 irails-1.2.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.2.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.314825 irails-1.2.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.2.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.2.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.2.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.238698 irails-1.2.2/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.316819 irails-1.2.2/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.2.2/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.2.2/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.269615 irails-1.2.2/irails.egg-info/
+-rw-rw-rw-   0        0        0     5079 2023-05-09 15:26:05.000000 irails-1.2.2/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2135 2023-05-09 15:26:05.000000 irails-1.2.2/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 15:26:05.000000 irails-1.2.2/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-09 15:26:05.000000 irails-1.2.2/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      766 2023-05-09 15:26:05.000000 irails-1.2.2/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-09 15:26:05.000000 irails-1.2.2/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 15:26:05.319811 irails-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.2.2/setup.py
```

### Comparing `irails-1.2.1/irails/_i18n.py` & `irails-1.2.2/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/_loader.py` & `irails-1.2.2/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/_utils.py` & `irails-1.2.2/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/auth.py` & `irails-1.2.2/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/base_controller.py` & `irails-1.2.2/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.2.2/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.2.2/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/cbv.py` & `irails-1.2.2/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/config.py` & `irails-1.2.2/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/controller_utils.py` & `irails-1.2.2/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/core.py` & `irails-1.2.2/irails/core.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/database.py` & `irails-1.2.2/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/midware.py` & `irails-1.2.2/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/midware_casbin.py` & `irails-1.2.2/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/midware_session.py` & `irails-1.2.2/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/mvc_router.py` & `irails-1.2.2/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/_app.py` & `irails-1.2.2/irails/scripts/_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,16 +102,16 @@
         dest_file = os.path.normpath(dest_file)
         if os.path.exists(dest_file):
             print(f'{dest_file} is exists,skip...')
             return True
         with open(dest_file,'w') as f:
             f.write("""
 # -*- coding: utf-8 -*- 
-from irails import api_router,api,Request,Response,BaseController,application
-@api_router(auth='none')
+from irails import route,api,Request,Response,BaseController,application
+@route(auth='none')
 class HomeController(BaseController): 
     @api.get("/")
     def home(self): 
         '''
         :title Home
         '''
         routers_map = application.routers_map
```

### Comparing `irails-1.2.1/irails/scripts/_controller.py` & `irails-1.2.2/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/_i18n.py` & `irails-1.2.2/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/_project.py` & `irails-1.2.2/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/_run.py` & `irails-1.2.2/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/main.py` & `irails-1.2.2/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/tpls/app/home.css.tpl` & `irails-1.2.2/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/tpls/app/home.tpl` & `irails-1.2.2/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.2.2/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.2.2/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.2.2/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/tpls/project/public/error_404.html` & `irails-1.2.2/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/tpls/project/public/error_500.html` & `irails-1.2.2/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.2.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.2.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.2.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.2.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.2.2/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails/view.py` & `irails-1.2.2/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails.egg-info/SOURCES.txt` & `irails-1.2.2/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.2.1/irails.egg-info/requires.txt` & `irails-1.2.2/irails.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,7 +39,9 @@
 ujson==5.5.0
 urllib3==1.26.15
 uvicorn==0.21.1
 watchfiles==0.19.0
 websockets==11.0.2
 yarg==0.1.9
 chardet==5.1.0
+polib
+mkdocs
```

### Comparing `irails-1.2.1/setup.py` & `irails-1.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,25 +24,17 @@
     code_lines = content.split('\n')   
     code_block = spec + '\n' + '\n'.join(code_lines) + '\n```\n'
     lines = lines[:start] + [code_block] + lines[end+1:]
 
     with open('readme.md', 'w') as file:
         file.writelines(lines)
 
-update_readme('apps/app/controllers/test_controller.py','```python')
-update_readme('apps/app/views/test/home.html','```html')
-# import subprocess
-# result = subprocess.run(['cmd','/c','tree','./app'], capture_output=True)
-# gbk_to_utf8 = result.stdout.decode("gbk").encode("utf-8")
-# gbk_to_utf8=gbk_to_utf8.replace(b'\r',b'\n')
-# if gbk_to_utf8: 
-#     gbk_to_utf8 = gbk_to_utf8.decode("utf-8")
-#     gbk_to_utf8 = gbk_to_utf8.split("\n")[3:]
-#     gbk_to_utf8 = '\n'.join(gbk_to_utf8)
-# update_readme('','```dir',gbk_to_utf8)
+# update_readme('apps/app/controllers/test_controller.py','```python')
+# update_readme('apps/app/views/test/home.html','```html')
+ 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open('requirements.txt', encoding="utf-8-sig") as f:
     requirements = f.readlines()
```

