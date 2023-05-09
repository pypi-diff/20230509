# Comparing `tmp/irails-1.2.0.tar.gz` & `tmp/irails-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.2.0.tar", last modified: Sun May  7 08:46:46 2023, max compression
+gzip compressed data, was "irails-1.2.1.tar", last modified: Tue May  9 06:53:18 2023, max compression
```

## Comparing `irails-1.2.0.tar` & `irails-1.2.1.tar`

### file list

```diff
@@ -1,79 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.392803 irails-1.2.0/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7120 2023-05-07 08:46:46.391806 irails-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6339 2023-05-07 08:46:46.000000 irails-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.338033 irails-1.2.0/irails/
--rw-rw-rw-   0        0        0      325 2023-05-07 08:46:02.000000 irails-1.2.0/irails/__init__.py
--rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.2.0/irails/_i18n.py
--rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.2.0/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.2.0/irails/_utils.py
--rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.2.0/irails/auth.py
--rw-rw-rw-   0        0        0    11570 2023-05-07 08:42:59.000000 irails-1.2.0/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.345797 irails-1.2.0/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.346794 irails-1.2.0/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.2.0/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.2.0/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.2.0/irails/cbv.py
--rw-rw-rw-   0        0        0     7252 2023-05-06 13:39:48.000000 irails-1.2.0/irails/config.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.2.0/irails/controller.py
--rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.2.0/irails/controller_utils.py
--rw-rw-rw-   0        0        0    14729 2023-05-07 08:39:08.000000 irails-1.2.0/irails/core.py
--rw-rw-rw-   0        0        0     6338 2023-05-05 11:07:47.000000 irails-1.2.0/irails/database.py
--rw-rw-rw-   0        0        0     8134 2023-05-05 14:29:33.000000 irails-1.2.0/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.2.0/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.2.0/irails/midware_session.py
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.354773 irails-1.2.0/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.2.0/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7813 2023-05-06 13:37:52.000000 irails-1.2.0/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     7603 2023-05-06 13:40:20.000000 irails-1.2.0/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     6836 2023-05-07 08:08:21.000000 irails-1.2.0/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.2.0/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1321 2023-05-04 04:28:43.000000 irails-1.2.0/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.2.0/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.309111 irails-1.2.0/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.363286 irails-1.2.0/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      233 2023-05-05 05:43:26.000000 irails-1.2.0/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.2.0/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.2.0/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.2.0/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.2.0/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.2.0/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.2.0/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.2.0/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.366277 irails-1.2.0/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.2.0/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.368478 irails-1.2.0/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.2.0/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.375848 irails-1.2.0/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.2.0/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.2.0/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.2.0/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.2.0/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.2.0/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0     1103 2023-05-07 08:44:35.000000 irails-1.2.0/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.2.0/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.2.0/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.377844 irails-1.2.0/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.2.0/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.2.0/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.379837 irails-1.2.0/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.313100 irails-1.2.0/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.384824 irails-1.2.0/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.2.0/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.387816 irails-1.2.0/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.2.0/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.2.0/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.2.0/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.315111 irails-1.2.0/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.389811 irails-1.2.0/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.2.0/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.2.0/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-07 08:46:46.343800 irails-1.2.0/irails.egg-info/
--rw-rw-rw-   0        0        0     7120 2023-05-07 08:46:46.000000 irails-1.2.0/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2033 2023-05-07 08:46:46.000000 irails-1.2.0/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 08:46:46.000000 irails-1.2.0/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-07 08:46:46.000000 irails-1.2.0/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      753 2023-05-07 08:46:46.000000 irails-1.2.0/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-07 08:46:46.000000 irails-1.2.0/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 08:46:46.392803 irails-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2955 2023-05-03 14:33:36.000000 irails-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.695625 irails-1.2.1/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7120 2023-05-09 06:53:18.694633 irails-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6339 2023-05-09 06:53:18.000000 irails-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.616999 irails-1.2.1/irails/
+-rw-rw-rw-   0        0        0      325 2023-05-09 06:52:52.000000 irails-1.2.1/irails/__init__.py
+-rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.2.1/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.2.1/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.2.1/irails/_utils.py
+-rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.2.1/irails/auth.py
+-rw-rw-rw-   0        0        0    11570 2023-05-07 08:42:59.000000 irails-1.2.1/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.629977 irails-1.2.1/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.630961 irails-1.2.1/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.2.1/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.2.1/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.2.1/irails/cbv.py
+-rw-rw-rw-   0        0        0     7252 2023-05-09 06:43:06.000000 irails-1.2.1/irails/config.py
+-rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.2.1/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    30828 2023-05-08 14:26:29.000000 irails-1.2.1/irails/core.py
+-rw-rw-rw-   0        0        0     6285 2023-05-08 14:12:16.000000 irails-1.2.1/irails/database.py
+-rw-rw-rw-   0        0        0     8655 2023-05-09 06:39:34.000000 irails-1.2.1/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.2.1/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.2.1/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.2.1/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.639939 irails-1.2.1/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.2.1/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7813 2023-05-06 13:37:52.000000 irails-1.2.1/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.2.1/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     6836 2023-05-07 08:08:21.000000 irails-1.2.1/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.2.1/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1321 2023-05-04 04:28:43.000000 irails-1.2.1/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.2.1/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.585957 irails-1.2.1/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.651906 irails-1.2.1/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      233 2023-05-05 05:43:26.000000 irails-1.2.1/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.2.1/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.2.1/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.2.1/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.2.1/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.2.1/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.2.1/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.2.1/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.655896 irails-1.2.1/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.2.1/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.656892 irails-1.2.1/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.2.1/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.668381 irails-1.2.1/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.2.1/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.2.1/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.2.1/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.2.1/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.2.1/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      835 2023-04-30 12:07:18.000000 irails-1.2.1/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      665 2023-05-09 06:45:32.000000 irails-1.2.1/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.2.1/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.2.1/irails/scripts/tpls/project/configs/upload.yaml
+-rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.2.1/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.670376 irails-1.2.1/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.2.1/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.2.1/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.673367 irails-1.2.1/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.590944 irails-1.2.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.679509 irails-1.2.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.2.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.687370 irails-1.2.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.2.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.2.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.2.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.591943 irails-1.2.1/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.690361 irails-1.2.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.2.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.2.1/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:53:18.626975 irails-1.2.1/irails.egg-info/
+-rw-rw-rw-   0        0        0     7120 2023-05-09 06:53:18.000000 irails-1.2.1/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2135 2023-05-09 06:53:18.000000 irails-1.2.1/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 06:53:18.000000 irails-1.2.1/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-09 06:53:18.000000 irails-1.2.1/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      753 2023-05-09 06:53:18.000000 irails-1.2.1/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-09 06:53:18.000000 irails-1.2.1/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 06:53:18.695625 irails-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2955 2023-05-03 14:33:36.000000 irails-1.2.1/setup.py
```

### Comparing `irails-1.2.0/PKG-INFO` & `irails-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.2.0
+Version: 1.2.1
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.2.0/README.md` & `irails-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/_i18n.py` & `irails-1.2.1/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/_loader.py` & `irails-1.2.1/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/_utils.py` & `irails-1.2.1/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/auth.py` & `irails-1.2.1/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/base_controller.py` & `irails-1.2.1/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.2.1/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.2.1/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/cbv.py` & `irails-1.2.1/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/config.py` & `irails-1.2.1/irails/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,121 +51,109 @@
 def _extract_name(string):
     match = re.search(r'{([^}]*)}', string)
     if match:
         return match.group(1)
     else:
         return None
 
+ 
 class YamlConfig:
-    _raw_config = {}
-    def __init__(self, filename:str="",config:Dict={}):
+    _raw_config: Dict = {}
+    def __init__(self, filename: str = "", config: Dict = {}):
         self.filename = filename
         self.config = config
         self.load()
-    def __getitem__(self,key):
+    def __getitem__(self, key: str):
         return self.get(key)
-    def __setitem__(self,key,value):
-        self.set(key,value)
-    def reload(self):
+    def __setitem__(self, key: str, value):
+       self.set(key, value)
+    def reload(self) -> bool:
         return self.load()
-    def load(self):
+    def load(self) -> bool:
         if os.path.isfile(self.filename):
             with open(self.filename, "r") as f:
                 self.config = yaml.safe_load(f)
                 YamlConfig._raw_config = self.config
-
         elif os.path.isdir(self.filename):
             self.config = self._merge_yaml_files(self.filename)
             YamlConfig._raw_config = self.config
         elif self.config:
             return True
         else:
             if is_cli_mode():
                 pass
             else:
                 raise Exception(f"{self.filename} is not a file or directory")
             return False
         return True
-    def dump(self):
+    def dump(self) -> str:
         return yaml.safe_dump(self.config) if self.config else ""
-    def save(self):
+    def save(self) -> bool:
         if not self.filename:
             return False
         with open(self.filename, "w") as f:
             yaml.safe_dump(self.config, f)
         return True
-    def get(self, key:str, default=None): 
-        
-        
+    def get(self, key: str, default=None):
         value = self.config.get(key, default)
-        if isinstance(value,str) and value.find("{")>-1:
-            while value.find("{")>-1 and value.find("}")>0:
-                name = _extract_name(value)
-                if name:
-                    if name==key:
-                        raise RuntimeError(f"configure file error circular reference `{name}`")
-                    
-                    if name.find(".")>0:
-                        paris = name.split(".")
-                        _root_value = self._raw_config[paris.pop(0)]
-                        _value:Dict = _root_value
-                        while paris:
-                            _k = paris.pop(0) 
-                            _value = _value.get(_k,'')
-                            if not _value:
-                                print(f'Warning config: {name} was empty,it\'s quoted by {key}')
-                            while _value.find("{")>-1 and value.find("}")>0:
-                                _name = _extract_name(_value)
-                                if _name:
-                                    _expr = _root_value.get(_name,"")
-                                    _x = f"{_name}"
-                                    _value = _value.replace('{'+_x+'}',_expr)
-                        return _value
-                        pass
-                    
-                    expr = self.config.get(name,"")
-                x = f"{name}"
-                value = value.replace('{'+x+'}',expr)
-        elif isinstance(value,dict):
-            return YamlConfig(filename="",config=value)
+        if isinstance(value, str):
+            value = self._resolve_value(value, key)
+        elif isinstance(value, dict):
+            value = YamlConfig(filename="", config=value)
         return value
-    
-    def set(self, key, value):
+    def set(self, key: str, value):
         self.config[key] = value
-
-    def delete(self, key):
+    def delete(self, key: str):
         del self.config[key]
-
-    def _merge_dicts(self, dict1, dict2):
+    def _merge_dicts(self, dict1: Dict, dict2: Dict) -> Dict:
         for key in dict2:
             if key in dict1 and isinstance(dict1[key], dict) and isinstance(dict2[key], dict):
                 dict1[key] = self._merge_dicts(dict1[key], dict2[key])
             else:
                 dict1[key] = dict2[key]
         return dict1
-
-    def _merge_yaml_files(self, dir_path):
-        global _log
+    def _merge_yaml_files(self, dir_path: str) -> Dict:
         merged_config = {}
         for file_name in os.listdir(dir_path):
             file_path = os.path.join(dir_path, file_name)
             if os.path.isfile(file_path) and file_name.endswith(".yaml"):
                 file_config = self._load_yaml_file(file_path)
                 if isinstance(file_config, dict):
                     merged_config = self._merge_dicts(merged_config, file_config)
-                # else:
-                #     _log.warn(f"YAML file {file_path} must contain a dictionary")
             elif os.path.isdir(file_path):
                 dir_config = self._merge_yaml_files(file_path)
                 merged_config = self._merge_dicts(merged_config, dir_config)
         return merged_config
-
-    def _load_yaml_file(self, filename):
-        with open(filename, "r") as f:
+    def _load_yaml_file(self, file_path: str) -> Dict:
+        with open(file_path, "r") as f:
             return yaml.safe_load(f)
+    def _resolve_value(self, value: str, key: str) -> str:
+        while "{" in value and "}" in value:
+            name = _extract_name(value)
+            if not name:
+                break
+            if name == key:
+                raise RuntimeError(f"Configure file error: circular reference `{name}`")
+            if "." in name:
+                segment_name, sub_key = name.split(".", 1)
+                if segment_name == "ROOT":
+                    # value = value.replace("{" + name + "}", self.config.get(sub_key, ""))
+                    value = value.replace("{" + name + "}", YamlConfig(config=self._raw_config).get(sub_key, ""))
+                else:
+                    segment_config = self.config.get(segment_name, {})
+                    if isinstance(segment_config, dict):
+                        sub_keys = sub_key.split(".")
+                        sub_value = segment_config
+                        for sub_key in sub_keys:
+                            sub_value = sub_value.get(sub_key, {})
+                        value = value.replace("{" + name + "}", str(sub_value))
+            else:
+                value = value.replace("{" + name + "}", self.config.get(name, ""))
+        return value
+ 
 def __init_log(__logCfg):
     if not __logCfg:
         return None
     from fastapi.logger import logger
     __log_level = __logCfg['level'] or 'DEBUG'
     __log_file = __logCfg['file'] or None 
     __isdebug = config.get("debug") or False
@@ -193,11 +181,19 @@
     
     logger.setLevel(logging._nameToLevel[__log_level]) 
     return logger
     # return logging.getLogger(__logCfg['name'] or 'FastapiMvcFramework')
 
 config = YamlConfig(os.path.join(ROOT_PATH,"configs") )
 
+#test:
+# dbcfg = config.get('database')
+# uri = dbcfg.get("uri")
+# assert uri
+# errors = config.get("errors")
+# p404 = errors.get("error_404_page")
+# assert p404
+
 _log = __init_log(config.get("log"))
 if _log:
     _log.setLevel(logging.DEBUG)
```

### Comparing `irails-1.2.0/irails/controller.py` & `irails-1.2.1/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/controller_utils.py` & `irails-1.2.1/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/database.py` & `irails-1.2.1/irails/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,20 +125,26 @@
         msg = sanitize_path(str(e.args)) 
         command.revision(alembic_cfg, autogenerate=True, message=msg) 
         # upgrade the db
         command.upgrade(alembic_cfg, "head") 
 def get_engine():
     global engine
     return engine
-def init_database( uri:str,debug:bool=False,alembic_ini:str="",cfg=None):
+def init_database( uri:str,debug:bool=False,cfg=None):
     '''
-    params :uri sqlalchemy connection string
+    :uri sqlalchemy connection string
     :params debug mode of debug 
-    :params alembic_ini alembic config file path,when debug=True will auto migrate the changes 
+    :cfg the database configure object
     '''
+    if not cfg:
+        return None
+    if not uri:
+        uri = cfg.get("uri","")
+    if not uri:
+        return None
     global DataMap,mapped_base ,engine
     dbencode = cfg.get('dbencode')
     dbdecode = cfg.get('dbdecode')
     if uri.startswith('sqlite'):
         db_directory = os.path.dirname(uri.split(':///')[1])
         os.makedirs(db_directory, exist_ok=True) 
 
@@ -163,18 +169,14 @@
         # we can then produce a set of mappings from this MetaData.
         mapped_base = automap_base(metadata=DataMap)
         mapped_base.prepare(autoload_with=engine,
             classname_for_table=camelize_classname,
             name_for_collection_relationship=pluralize_collection )
          
         engine.convert_varchar = convert_varchar
-
-        # session = Session(engine)
-        
-        # sysfile = Service.mapped('SysFile')
  
         pass
     #test connect
     try:
         with engine.connect() as conn:
             _log.disabled = False
             _log.debug('database connection successed:' + str(conn))
```

### Comparing `irails-1.2.0/irails/midware.py` & `irails-1.2.1/irails/midware.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,43 +14,58 @@
 
 from starlette.staticfiles import PathLike
 from .config import _log,config
 from .midware_session import (SessionMiddleware,FileStorage,MemoryStorage,RedisStorage,SessionStorage,_SESSION_STORAGES)
 from fastapi.middleware.cors import CORSMiddleware
 from starlette.types import   Scope 
 from .view import _View,env_configs,static_format
-from .config import config
+from .config import config,ROOT_PATH
 
 from fastapi.middleware import Middleware
 from starlette.middleware import Middleware as StarletteMiddleware
 from starlette.types import Receive, Scope, Send
 import jinja2
 import chardet
+
+errors = config.get("errors")
+if errors:
+    error_404 = errors.get('error_404_page')
+    error_500 = errors.get("error_500_page")
+    disabled_path_of_files=[os.path.abspath(error_404),
+                        os.path.abspath(error_500),
+                        ]
+else:
+    disabled_path_of_files=[]
+    
 class MvcStaticFiles(StaticFiles):
     
     def file_response(
         self,
         full_path: PathLike,
         stat_result: os.stat_result,
         scope: Scope,
         status_code: int = 200,
     ) -> Response:
+        
+        if full_path in disabled_path_of_files:
+            return Response(None,404)
         ext = full_path.split(".")[-1] if full_path.find(".")>-1 else ""
         if ext and ext in static_format: 
              
             context = {"request":Request(scope)}
             with open(full_path, 'rb') as f:
                 bstr = f.read()
                 result = chardet.detect(bstr) 
                 content = bstr.decode(result['encoding'])
                  
             tmp = jinja2.Template(source = content,**env_configs)
             txt =  tmp.render(context)
             return Response(txt)
         else:
+            
             return super().file_response(
                 full_path,
                 stat_result,
                 scope,
                 status_code=status_code,
                  
             )
@@ -118,15 +133,17 @@
             else:
                 _session_options["storage"] = _SESSION_STORAGES[_storageType]()
             
         _session_options['secret_key'] = _session_cfg.get("secret_key","") 
     app.add_middleware(SessionMiddleware,**_session_options)
 
     def error_page(code:int,request,e):
-        page = config.get(f"error_{code}_page")
+        page = config.get(f"error_page")
+        if page :
+            page = page.get(f"page_{code}")
         if page and os.path.exists(page):
             viewObj = _View(request=request,response=None,tmpl_path=os.path.abspath(os.path.dirname(page)))
             file = os.path.basename(page)
             content=[]
             if debug:
                 exc_traceback = e.__traceback__ 
                 # show traceback the last files and location
@@ -180,27 +197,27 @@
 
     @app.exception_handler(RequestValidationError)
     async def validation_exception_handler(request, exc):
         _log.error(f"OMG! The client sent invalid data!: {exc}")
         return await request_validation_exception_handler(request, exc)
 
     #denied to access error page for directly
-    @app.route('/public/error_404.html',['GET','POST','HEAD','OPTION','PUT','DELETE'])
-    def _error1(request):
-        raise HTTPException(404,"Not Found.") 
-    @app.route('/public/error_500.html',['GET','POST','HEAD','OPTION','PUT','DELETE'])
-    def _error2(request):
-        raise HTTPException(404,"Not Found.")
+    # @app.route('/public/error_404.html',['GET','POST','HEAD','OPTION','PUT','DELETE'])
+    # def _error1(request):
+    #     raise HTTPException(404,"Not Found.") 
+    # @app.route('/public/error_500.html',['GET','POST','HEAD','OPTION','PUT','DELETE'])
+    # def _error2(request):
+    #     raise HTTPException(404,"Not Found.")
      
-    @app.get("/favicon.ico")
-    def _get_favicon():
-        if os.path.exists("./public/favicon.ico"): 
-            return FileResponse("./public/favicon.ico")
-        else:
-            return Response(content = None,status_code= 404)
+    # @app.get("/favicon.ico")
+    # def _get_favicon():
+    #     if os.path.exists("./public/favicon.ico"): 
+    #         return FileResponse("./public/favicon.ico")
+    #     else:
+    #         return Response(content = None,status_code= 404)
         
     if debug:    
         @app.middleware("http")
         async def preprocess_request(request: Request, call_next): 
             start_time = time.time()  
             response:Response = await call_next(request) 
             process_time = time.time() - start_time
```

### Comparing `irails-1.2.0/irails/midware_casbin.py` & `irails-1.2.1/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/midware_session.py` & `irails-1.2.1/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/scripts/_app.py` & `irails-1.2.1/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/scripts/_controller.py` & `irails-1.2.1/irails/scripts/_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,17 @@
             __init_file = os.path.join(_current_dir,'controllers','__init__.py')
             self.ensure_line(__init_file,f"from . import {controler_path_name}_controller")
             __init_file = os.path.join(_current_dir,'models','__init__.py')
             self.ensure_line(__init_file,f"from . import {controler_path_name}_model")
             __init_file = os.path.join(_current_dir,'services','__init__.py')
             self.ensure_line(__init_file,f"from . import {controler_path_name}_service")
             acts = []
-            for action in self.args.name:
+            actions = self.args.name
+            if len(actions)==0:actions.append('index')
+            for action in actions:
                 acts.append(f"""
     @api.get('/{action}')
     def {action}(self):
         return self.view()                
 """)
                 _view_file = os.path.join(_current_dir,'views',controler_path_name,f"{action}.html")
                 if not os.path.exists(_view_file):
```

### Comparing `irails-1.2.0/irails/scripts/_i18n.py` & `irails-1.2.1/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/scripts/_project.py` & `irails-1.2.1/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/scripts/_run.py` & `irails-1.2.1/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/scripts/main.py` & `irails-1.2.1/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/scripts/tpls/app/home.css.tpl` & `irails-1.2.1/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/scripts/tpls/app/home.tpl` & `irails-1.2.1/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.2.1/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.2.1/irails/scripts/tpls/project/configs/database.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -9,13 +9,13 @@
   # mysql+pymysql://username:password@host:port/database_name 
   # PostgreSQL
   # postgresql+psycopg2://username:password@host:port/database_name 
   # SQLite
   # sqlite:///absolute/path/to/db/file.db 3times of '/'
   # Mssql
   # mssql+pymssql://username:password@hostname:port/database_name 
-  #uri:  #'sqlite:///{dbname}' #empty to disable database connection
+  uri:  sqlite:///{dbname} #empty to disable database connection
   # uri: 'mongodb+srv://dbbruce:smjk123@atlascluster.siz4vrp.mongodb.net/?retryWrites=true&w=majority'
   # uri: 'mssql+pymssql://{dbuser}:{dbpassword}@{dbhost}/{dbname}'
   alembic_ini: 'configs/alembic.ini' #empty or none will disable auto migrate
   dbfirst: false
   maptables: [] #['item','ba_cls_info']
```

### Comparing `irails-1.2.0/irails/scripts/tpls/project/public/error_404.html` & `irails-1.2.1/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/scripts/tpls/project/public/error_500.html` & `irails-1.2.1/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.2.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.2.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.2.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.2.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.2.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails/view.py` & `irails-1.2.1/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/irails.egg-info/PKG-INFO` & `irails-1.2.1/irails.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.2.0
+Version: 1.2.1
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.2.0/irails.egg-info/SOURCES.txt` & `irails-1.2.1/irails.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 irails/_i18n.py
 irails/_loader.py
 irails/_utils.py
 irails/auth.py
 irails/base_controller.py
 irails/cbv.py
 irails/config.py
-irails/controller.py
 irails/controller_utils.py
 irails/core.py
 irails/database.py
 irails/midware.py
 irails/midware_casbin.py
 irails/midware_session.py
+irails/mvc_router.py
 irails/view.py
 irails.egg-info/PKG-INFO
 irails.egg-info/SOURCES.txt
 irails.egg-info/dependency_links.txt
 irails.egg-info/entry_points.txt
 irails.egg-info/requires.txt
 irails.egg-info/top_level.txt
@@ -41,20 +41,22 @@
 irails/scripts/tpls/app/service.tpl
 irails/scripts/tpls/app/test.tpl
 irails/scripts/tpls/app/view.tpl
 irails/scripts/tpls/project/.gitignore
 irails/scripts/tpls/project/main.py
 irails/scripts/tpls/project/apps/__init__.py
 irails/scripts/tpls/project/configs/alembic.ini
+irails/scripts/tpls/project/configs/authencation.yaml
 irails/scripts/tpls/project/configs/cache.yaml
 irails/scripts/tpls/project/configs/casbin-adapter.csv
 irails/scripts/tpls/project/configs/casbin-model.conf
 irails/scripts/tpls/project/configs/database.yaml
 irails/scripts/tpls/project/configs/general.yaml
 irails/scripts/tpls/project/configs/session.yaml
+irails/scripts/tpls/project/configs/upload.yaml
 irails/scripts/tpls/project/public/error_404.html
 irails/scripts/tpls/project/public/error_500.html
 irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
 irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
 irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
 irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
 irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
```

### Comparing `irails-1.2.0/irails.egg-info/requires.txt` & `irails-1.2.1/irails.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irails-1.2.0/setup.py` & `irails-1.2.1/setup.py`

 * *Files identical despite different names*

