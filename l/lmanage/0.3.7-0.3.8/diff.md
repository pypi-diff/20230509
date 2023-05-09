# Comparing `tmp/lmanage-0.3.7.tar.gz` & `tmp/lmanage-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmanage-0.3.7.tar", max compression
+gzip compressed data, was "lmanage-0.3.8.tar", max compression
```

## Comparing `lmanage-0.3.7.tar` & `lmanage-0.3.8.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0    11358 2021-07-16 17:02:14.912118 lmanage-0.3.7/LICENSE
--rw-r--r--   0        0        0     2695 2023-04-27 21:32:50.653908 lmanage-0.3.7/README.md
--rw-r--r--   0        0        0      926 2022-12-15 21:59:31.502790 lmanage-0.3.7/lmanage/.vimspector.json
--rw-r--r--   0        0        0      598 2023-03-23 16:57:22.191458 lmanage-0.3.7/lmanage/__init__.py
--rw-r--r--   0        0        0      598 2023-03-23 16:57:22.195458 lmanage-0.3.7/lmanage/capturator/__init__.py
--rw-r--r--   0        0        0     2063 2023-03-23 16:57:22.195458 lmanage-0.3.7/lmanage/capturator/commands.py
--rw-r--r--   0        0        0        0 2023-04-19 21:34:25.230519 lmanage-0.3.7/lmanage/capturator/content_capturation/__init__.py
--rw-r--r--   0        0        0     1855 2023-05-08 17:34:54.913053 lmanage-0.3.7/lmanage/capturator/content_capturation/board_capture.py
--rw-r--r--   0        0        0     2618 2023-05-04 22:07:41.433704 lmanage-0.3.7/lmanage/capturator/content_capturation/dashboard_capture.py
--rw-r--r--   0        0        0     3227 2023-04-26 23:19:51.736692 lmanage-0.3.7/lmanage/capturator/content_capturation/look_capture.py
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.7/lmanage/capturator/folder_capturation/__init__.py
--rw-r--r--   0        0        0     1136 2023-04-19 21:34:25.230519 lmanage-0.3.7/lmanage/capturator/folder_capturation/create_folder_yaml_structure.py
--rw-r--r--   0        0        0     8063 2023-04-26 23:19:51.736692 lmanage-0.3.7/lmanage/capturator/folder_capturation/folder_config.py
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.7/lmanage/capturator/user_attribute_capturation/__init__.py
--rw-r--r--   0        0        0     2341 2023-04-26 23:19:51.736692 lmanage-0.3.7/lmanage/capturator/user_attribute_capturation/capture_ua_permissions.py
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.7/lmanage/capturator/user_group_capturation/__init__.py
--rw-r--r--   0        0        0     3565 2023-04-26 23:16:43.844504 lmanage-0.3.7/lmanage/capturator/user_group_capturation/group_config.py
--rw-r--r--   0        0        0     2923 2023-04-26 23:16:43.844504 lmanage-0.3.7/lmanage/capturator/user_group_capturation/role_config.py
--rw-r--r--   0        0        0     3765 2023-03-23 16:57:22.195458 lmanage-0.3.7/lmanage/capturator/user_group_capturation/user_permission.py
--rw-r--r--   0        0        0     5141 2023-05-05 22:42:39.755506 lmanage-0.3.7/lmanage/capture_instance_permission_structure.py
--rw-r--r--   0        0        0      928 2023-04-26 23:16:43.844504 lmanage-0.3.7/lmanage/cli.py
--rw-r--r--   0        0        0      353 2022-06-24 18:34:27.402555 lmanage-0.3.7/lmanage/configurator/.vimspector.json
--rw-r--r--   0        0        0      598 2023-03-23 16:57:22.191458 lmanage-0.3.7/lmanage/configurator/__init__.py
--rw-r--r--   0        0        0     2026 2023-03-23 16:57:22.191458 lmanage-0.3.7/lmanage/configurator/commands.py
--rw-r--r--   0        0        0        0 2023-04-19 21:34:25.230519 lmanage-0.3.7/lmanage/configurator/content_configuration/__init__.py
--rw-r--r--   0        0        0     2716 2023-05-08 17:42:53.204117 lmanage-0.3.7/lmanage/configurator/content_configuration/create_boards.py
--rw-r--r--   0        0        0     2679 2023-05-08 18:13:26.279080 lmanage-0.3.7/lmanage/configurator/content_configuration/create_content_prep.py
--rw-r--r--   0        0        0     1343 2023-05-09 17:23:59.031587 lmanage-0.3.7/lmanage/configurator/content_configuration/create_dashboards.py
--rw-r--r--   0        0        0     4072 2023-04-26 23:19:51.736692 lmanage-0.3.7/lmanage/configurator/content_configuration/create_looks.py
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.191458 lmanage-0.3.7/lmanage/configurator/folder_configuration/__init__.py
--rw-r--r--   0        0        0    13653 2023-04-26 23:16:43.844504 lmanage-0.3.7/lmanage/configurator/folder_configuration/create_folder_permissions.py
--rw-r--r--   0        0        0     5786 2023-04-19 21:34:25.230519 lmanage-0.3.7/lmanage/configurator/folder_configuration/create_folders.py
--rw-r--r--   0        0        0     1615 2023-04-19 21:34:25.234519 lmanage-0.3.7/lmanage/configurator/folder_configuration/folder_config.py
--rw-r--r--   0        0        0     5706 2023-02-07 21:50:06.720732 lmanage-0.3.7/lmanage/configurator/instance_configuration_settings/fullinstance.yaml
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.191458 lmanage-0.3.7/lmanage/configurator/user_attribute_configuration/__init__.py
--rw-r--r--   0        0        0     4102 2023-05-09 17:06:42.831339 lmanage-0.3.7/lmanage/configurator/user_attribute_configuration/create_ua_permissions.py
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.7/lmanage/configurator/user_group_configuration/__init__.py
--rw-r--r--   0        0        0     4420 2023-04-26 23:16:43.844504 lmanage-0.3.7/lmanage/configurator/user_group_configuration/group_config.py
--rw-r--r--   0        0        0     5978 2023-04-26 23:16:43.848504 lmanage-0.3.7/lmanage/configurator/user_group_configuration/role_config.py
--rw-r--r--   0        0        0     4727 2023-04-26 23:16:43.848504 lmanage-0.3.7/lmanage/configurator/user_group_configuration/user_permission.py
--rwxr-xr-x   0        0        0      702 2022-12-15 21:59:31.634799 lmanage-0.3.7/lmanage/find_replace.sh
--rw-r--r--   0        0        0      446 2022-06-24 18:34:27.574567 lmanage-0.3.7/lmanage/mapview/.vimspector.json
--rw-r--r--   0        0        0      575 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/__init__.py
--rw-r--r--   0        0        0     3645 2023-03-23 16:57:22.191458 lmanage-0.3.7/lmanage/mapview/compare_content_to_lookml.py
--rw-r--r--   0        0        0     1873 2022-06-24 18:34:27.602569 lmanage-0.3.7/lmanage/mapview/hugo.csv
--rw-r--r--   0        0        0     2092 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/instancedata.py
--rw-r--r--   0        0        0    14973 2023-04-26 23:16:43.868505 lmanage-0.3.7/lmanage/mapview/legacy_get_content_with_views.py
--rw-r--r--   0        0        0     1633 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/main.py
--rw-r--r--   0        0        0     2773 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/mapexplores.py
--rw-r--r--   0        0        0     1503 2023-03-23 16:57:22.191458 lmanage-0.3.7/lmanage/mapview/mapview_execute.py
--rw-r--r--   0        0        0     2182 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/matched_field_analysis.py
--rw-r--r--   0        0        0     7197 2022-06-24 18:34:27.694576 lmanage-0.3.7/lmanage/mapview/pandas_multiple.xlsx
--rw-r--r--   0        0        0     2881 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/parse_sql_tables.py
--rw-r--r--   0        0        0      324 2022-06-24 18:34:27.714578 lmanage-0.3.7/lmanage/mapview/utils/.vimspector.json
--rw-r--r--   0        0        0      575 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/utils/__init__.py
--rw-r--r--   0        0        0     1234 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/utils/create_df.py
--rw-r--r--   0        0        0     3046 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/utils/parse_lookml.py
--rw-r--r--   0        0        0     5008 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/utils/parsing_sql.py
--rw-r--r--   0        0        0     6749 2023-05-09 17:19:57.683778 lmanage-0.3.7/lmanage/provision_instance_permission_structure.py
--rw-r--r--   0        0        0      575 2023-03-23 16:57:22.191458 lmanage-0.3.7/lmanage/utils/__init__.py
--rw-r--r--   0        0        0     1183 2023-05-03 23:35:07.193770 lmanage-0.3.7/lmanage/utils/errorhandling.py
--rw-r--r--   0        0        0     3108 2023-05-08 17:34:24.651084 lmanage-0.3.7/lmanage/utils/looker_object_constructors.py
--rw-r--r--   0        0        0     2247 2023-05-06 00:24:47.778206 lmanage-0.3.7/lmanage/utils/parse_yaml.py
--rw-r--r--   0        0        0     1029 2023-05-09 17:26:59.015362 lmanage-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     3995 1970-01-01 00:00:00.000000 lmanage-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    11358 2021-07-16 17:02:14.912118 lmanage-0.3.8/LICENSE
+-rw-r--r--   0        0        0     2695 2023-04-27 21:32:50.653908 lmanage-0.3.8/README.md
+-rw-r--r--   0        0        0      926 2022-12-15 21:59:31.502790 lmanage-0.3.8/lmanage/.vimspector.json
+-rw-r--r--   0        0        0      598 2023-03-23 16:57:22.191458 lmanage-0.3.8/lmanage/__init__.py
+-rw-r--r--   0        0        0      598 2023-03-23 16:57:22.195458 lmanage-0.3.8/lmanage/capturator/__init__.py
+-rw-r--r--   0        0        0     2063 2023-03-23 16:57:22.195458 lmanage-0.3.8/lmanage/capturator/commands.py
+-rw-r--r--   0        0        0        0 2023-04-19 21:34:25.230519 lmanage-0.3.8/lmanage/capturator/content_capturation/__init__.py
+-rw-r--r--   0        0        0     1855 2023-05-08 17:34:54.913053 lmanage-0.3.8/lmanage/capturator/content_capturation/board_capture.py
+-rw-r--r--   0        0        0     2618 2023-05-04 22:07:41.433704 lmanage-0.3.8/lmanage/capturator/content_capturation/dashboard_capture.py
+-rw-r--r--   0        0        0     3227 2023-04-26 23:19:51.736692 lmanage-0.3.8/lmanage/capturator/content_capturation/look_capture.py
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.8/lmanage/capturator/folder_capturation/__init__.py
+-rw-r--r--   0        0        0     1136 2023-04-19 21:34:25.230519 lmanage-0.3.8/lmanage/capturator/folder_capturation/create_folder_yaml_structure.py
+-rw-r--r--   0        0        0     8063 2023-04-26 23:19:51.736692 lmanage-0.3.8/lmanage/capturator/folder_capturation/folder_config.py
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.8/lmanage/capturator/user_attribute_capturation/__init__.py
+-rw-r--r--   0        0        0     2341 2023-04-26 23:19:51.736692 lmanage-0.3.8/lmanage/capturator/user_attribute_capturation/capture_ua_permissions.py
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.8/lmanage/capturator/user_group_capturation/__init__.py
+-rw-r--r--   0        0        0     3565 2023-04-26 23:16:43.844504 lmanage-0.3.8/lmanage/capturator/user_group_capturation/group_config.py
+-rw-r--r--   0        0        0     2923 2023-04-26 23:16:43.844504 lmanage-0.3.8/lmanage/capturator/user_group_capturation/role_config.py
+-rw-r--r--   0        0        0     3765 2023-03-23 16:57:22.195458 lmanage-0.3.8/lmanage/capturator/user_group_capturation/user_permission.py
+-rw-r--r--   0        0        0     5149 2023-05-09 17:31:20.432450 lmanage-0.3.8/lmanage/capture_instance_permission_structure.py
+-rw-r--r--   0        0        0      928 2023-04-26 23:16:43.844504 lmanage-0.3.8/lmanage/cli.py
+-rw-r--r--   0        0        0      353 2022-06-24 18:34:27.402555 lmanage-0.3.8/lmanage/configurator/.vimspector.json
+-rw-r--r--   0        0        0      598 2023-03-23 16:57:22.191458 lmanage-0.3.8/lmanage/configurator/__init__.py
+-rw-r--r--   0        0        0     2026 2023-03-23 16:57:22.191458 lmanage-0.3.8/lmanage/configurator/commands.py
+-rw-r--r--   0        0        0        0 2023-04-19 21:34:25.230519 lmanage-0.3.8/lmanage/configurator/content_configuration/__init__.py
+-rw-r--r--   0        0        0     2716 2023-05-08 17:42:53.204117 lmanage-0.3.8/lmanage/configurator/content_configuration/create_boards.py
+-rw-r--r--   0        0        0     2679 2023-05-08 18:13:26.279080 lmanage-0.3.8/lmanage/configurator/content_configuration/create_content_prep.py
+-rw-r--r--   0        0        0     1343 2023-05-09 17:23:59.031587 lmanage-0.3.8/lmanage/configurator/content_configuration/create_dashboards.py
+-rw-r--r--   0        0        0     4072 2023-04-26 23:19:51.736692 lmanage-0.3.8/lmanage/configurator/content_configuration/create_looks.py
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.191458 lmanage-0.3.8/lmanage/configurator/folder_configuration/__init__.py
+-rw-r--r--   0        0        0    13653 2023-04-26 23:16:43.844504 lmanage-0.3.8/lmanage/configurator/folder_configuration/create_folder_permissions.py
+-rw-r--r--   0        0        0     5786 2023-04-19 21:34:25.230519 lmanage-0.3.8/lmanage/configurator/folder_configuration/create_folders.py
+-rw-r--r--   0        0        0     1615 2023-04-19 21:34:25.234519 lmanage-0.3.8/lmanage/configurator/folder_configuration/folder_config.py
+-rw-r--r--   0        0        0     5706 2023-02-07 21:50:06.720732 lmanage-0.3.8/lmanage/configurator/instance_configuration_settings/fullinstance.yaml
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.191458 lmanage-0.3.8/lmanage/configurator/user_attribute_configuration/__init__.py
+-rw-r--r--   0        0        0     4102 2023-05-09 17:06:42.831339 lmanage-0.3.8/lmanage/configurator/user_attribute_configuration/create_ua_permissions.py
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.8/lmanage/configurator/user_group_configuration/__init__.py
+-rw-r--r--   0        0        0     4420 2023-04-26 23:16:43.844504 lmanage-0.3.8/lmanage/configurator/user_group_configuration/group_config.py
+-rw-r--r--   0        0        0     5978 2023-04-26 23:16:43.848504 lmanage-0.3.8/lmanage/configurator/user_group_configuration/role_config.py
+-rw-r--r--   0        0        0     4727 2023-04-26 23:16:43.848504 lmanage-0.3.8/lmanage/configurator/user_group_configuration/user_permission.py
+-rwxr-xr-x   0        0        0      702 2022-12-15 21:59:31.634799 lmanage-0.3.8/lmanage/find_replace.sh
+-rw-r--r--   0        0        0      446 2022-06-24 18:34:27.574567 lmanage-0.3.8/lmanage/mapview/.vimspector.json
+-rw-r--r--   0        0        0      575 2023-03-23 16:57:22.187458 lmanage-0.3.8/lmanage/mapview/__init__.py
+-rw-r--r--   0        0        0     3645 2023-03-23 16:57:22.191458 lmanage-0.3.8/lmanage/mapview/compare_content_to_lookml.py
+-rw-r--r--   0        0        0     1873 2022-06-24 18:34:27.602569 lmanage-0.3.8/lmanage/mapview/hugo.csv
+-rw-r--r--   0        0        0     2092 2023-03-23 16:57:22.187458 lmanage-0.3.8/lmanage/mapview/instancedata.py
+-rw-r--r--   0        0        0    14973 2023-04-26 23:16:43.868505 lmanage-0.3.8/lmanage/mapview/legacy_get_content_with_views.py
+-rw-r--r--   0        0        0     1633 2023-03-23 16:57:22.187458 lmanage-0.3.8/lmanage/mapview/main.py
+-rw-r--r--   0        0        0     2773 2023-03-23 16:57:22.187458 lmanage-0.3.8/lmanage/mapview/mapexplores.py
+-rw-r--r--   0        0        0     1503 2023-03-23 16:57:22.191458 lmanage-0.3.8/lmanage/mapview/mapview_execute.py
+-rw-r--r--   0        0        0     2182 2023-03-23 16:57:22.187458 lmanage-0.3.8/lmanage/mapview/matched_field_analysis.py
+-rw-r--r--   0        0        0     7197 2022-06-24 18:34:27.694576 lmanage-0.3.8/lmanage/mapview/pandas_multiple.xlsx
+-rw-r--r--   0        0        0     2881 2023-03-23 16:57:22.187458 lmanage-0.3.8/lmanage/mapview/parse_sql_tables.py
+-rw-r--r--   0        0        0      324 2022-06-24 18:34:27.714578 lmanage-0.3.8/lmanage/mapview/utils/.vimspector.json
+-rw-r--r--   0        0        0      575 2023-03-23 16:57:22.187458 lmanage-0.3.8/lmanage/mapview/utils/__init__.py
+-rw-r--r--   0        0        0     1234 2023-03-23 16:57:22.187458 lmanage-0.3.8/lmanage/mapview/utils/create_df.py
+-rw-r--r--   0        0        0     3046 2023-03-23 16:57:22.187458 lmanage-0.3.8/lmanage/mapview/utils/parse_lookml.py
+-rw-r--r--   0        0        0     5008 2023-03-23 16:57:22.187458 lmanage-0.3.8/lmanage/mapview/utils/parsing_sql.py
+-rw-r--r--   0        0        0     6749 2023-05-09 17:19:57.683778 lmanage-0.3.8/lmanage/provision_instance_permission_structure.py
+-rw-r--r--   0        0        0      575 2023-03-23 16:57:22.191458 lmanage-0.3.8/lmanage/utils/__init__.py
+-rw-r--r--   0        0        0     1183 2023-05-03 23:35:07.193770 lmanage-0.3.8/lmanage/utils/errorhandling.py
+-rw-r--r--   0        0        0     3108 2023-05-08 17:34:24.651084 lmanage-0.3.8/lmanage/utils/looker_object_constructors.py
+-rw-r--r--   0        0        0     2247 2023-05-06 00:24:47.778206 lmanage-0.3.8/lmanage/utils/parse_yaml.py
+-rw-r--r--   0        0        0     1029 2023-05-09 17:32:33.849247 lmanage-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     3995 1970-01-01 00:00:00.000000 lmanage-0.3.8/PKG-INFO
```

### Comparing `lmanage-0.3.7/LICENSE` & `lmanage-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/README.md` & `lmanage-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/.vimspector.json` & `lmanage-0.3.8/lmanage/.vimspector.json`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/__init__.py` & `lmanage-0.3.8/lmanage/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/capturator/__init__.py` & `lmanage-0.3.8/lmanage/capturator/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/capturator/commands.py` & `lmanage-0.3.8/lmanage/capturator/commands.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/capturator/content_capturation/board_capture.py` & `lmanage-0.3.8/lmanage/capturator/content_capturation/board_capture.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/capturator/content_capturation/dashboard_capture.py` & `lmanage-0.3.8/lmanage/capturator/content_capturation/dashboard_capture.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/capturator/content_capturation/look_capture.py` & `lmanage-0.3.8/lmanage/capturator/content_capturation/look_capture.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/capturator/folder_capturation/create_folder_yaml_structure.py` & `lmanage-0.3.8/lmanage/capturator/folder_capturation/create_folder_yaml_structure.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/capturator/folder_capturation/folder_config.py` & `lmanage-0.3.8/lmanage/capturator/folder_capturation/folder_config.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/capturator/user_attribute_capturation/capture_ua_permissions.py` & `lmanage-0.3.8/lmanage/capturator/user_attribute_capturation/capture_ua_permissions.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/capturator/user_group_capturation/group_config.py` & `lmanage-0.3.8/lmanage/capturator/user_group_capturation/group_config.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/capturator/user_group_capturation/role_config.py` & `lmanage-0.3.8/lmanage/capturator/user_group_capturation/role_config.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/capturator/user_group_capturation/user_permission.py` & `lmanage-0.3.8/lmanage/capturator/user_group_capturation/user_permission.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/capture_instance_permission_structure.py` & `lmanage-0.3.8/lmanage/capture_instance_permission_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,18 +82,18 @@
         file.write('\n\n# USER_ATTRIBUTES\n')
         yaml.dump(looker_ua, file)
 
 ###############################################################
 # Capture Users Content #######################################
 ###############################################################
     # Capture Content Boards
-    boards = bc.CaptureBoards(sdk=sdk).execute()
-    with open(f'{yaml_path}_content.yaml', 'w+') as file:
-        file.write('\n\n# BoardData\n')
-        yaml.dump(boards, file)
+    # boards = bc.CaptureBoards(sdk=sdk).execute()
+    # with open(f'{yaml_path}_content.yaml', 'w+') as file:
+    #     file.write('\n\n# BoardData\n')
+    #     yaml.dump(boards, file)
 
     # Capture Look Content
     looks = lc.CaptureLookObject(
         sdk=sdk, folder_root=folder_root_dict).execute()
     with open(f'{yaml_path}_content.yaml', 'a') as file:
         file.write('\n\n# LookData\n')
         yaml.dump(looks, file)
```

### Comparing `lmanage-0.3.7/lmanage/cli.py` & `lmanage-0.3.8/lmanage/cli.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/configurator/__init__.py` & `lmanage-0.3.8/lmanage/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/configurator/commands.py` & `lmanage-0.3.8/lmanage/configurator/commands.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/configurator/content_configuration/create_boards.py` & `lmanage-0.3.8/lmanage/configurator/content_configuration/create_boards.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/configurator/content_configuration/create_content_prep.py` & `lmanage-0.3.8/lmanage/configurator/content_configuration/create_content_prep.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/configurator/content_configuration/create_dashboards.py` & `lmanage-0.3.8/lmanage/configurator/content_configuration/create_dashboards.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/configurator/content_configuration/create_looks.py` & `lmanage-0.3.8/lmanage/configurator/content_configuration/create_looks.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/configurator/folder_configuration/create_folder_permissions.py` & `lmanage-0.3.8/lmanage/configurator/folder_configuration/create_folder_permissions.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/configurator/folder_configuration/create_folders.py` & `lmanage-0.3.8/lmanage/configurator/folder_configuration/create_folders.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/configurator/folder_configuration/folder_config.py` & `lmanage-0.3.8/lmanage/configurator/folder_configuration/folder_config.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/configurator/instance_configuration_settings/fullinstance.yaml` & `lmanage-0.3.8/lmanage/configurator/instance_configuration_settings/fullinstance.yaml`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/configurator/user_attribute_configuration/create_ua_permissions.py` & `lmanage-0.3.8/lmanage/configurator/user_attribute_configuration/create_ua_permissions.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/configurator/user_group_configuration/group_config.py` & `lmanage-0.3.8/lmanage/configurator/user_group_configuration/group_config.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/configurator/user_group_configuration/role_config.py` & `lmanage-0.3.8/lmanage/configurator/user_group_configuration/role_config.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/configurator/user_group_configuration/user_permission.py` & `lmanage-0.3.8/lmanage/configurator/user_group_configuration/user_permission.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/find_replace.sh` & `lmanage-0.3.8/lmanage/find_replace.sh`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/mapview/__init__.py` & `lmanage-0.3.8/lmanage/mapview/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/mapview/compare_content_to_lookml.py` & `lmanage-0.3.8/lmanage/mapview/compare_content_to_lookml.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/mapview/hugo.csv` & `lmanage-0.3.8/lmanage/mapview/hugo.csv`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/mapview/instancedata.py` & `lmanage-0.3.8/lmanage/mapview/instancedata.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/mapview/legacy_get_content_with_views.py` & `lmanage-0.3.8/lmanage/mapview/legacy_get_content_with_views.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/mapview/main.py` & `lmanage-0.3.8/lmanage/mapview/main.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/mapview/mapexplores.py` & `lmanage-0.3.8/lmanage/mapview/mapexplores.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/mapview/mapview_execute.py` & `lmanage-0.3.8/lmanage/mapview/mapview_execute.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/mapview/matched_field_analysis.py` & `lmanage-0.3.8/lmanage/mapview/matched_field_analysis.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/mapview/pandas_multiple.xlsx` & `lmanage-0.3.8/lmanage/mapview/pandas_multiple.xlsx`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/mapview/parse_sql_tables.py` & `lmanage-0.3.8/lmanage/mapview/parse_sql_tables.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/mapview/utils/__init__.py` & `lmanage-0.3.8/lmanage/mapview/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/mapview/utils/create_df.py` & `lmanage-0.3.8/lmanage/mapview/utils/create_df.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/mapview/utils/parse_lookml.py` & `lmanage-0.3.8/lmanage/mapview/utils/parse_lookml.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/mapview/utils/parsing_sql.py` & `lmanage-0.3.8/lmanage/mapview/utils/parsing_sql.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/provision_instance_permission_structure.py` & `lmanage-0.3.8/lmanage/provision_instance_permission_structure.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/utils/__init__.py` & `lmanage-0.3.8/lmanage/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/utils/errorhandling.py` & `lmanage-0.3.8/lmanage/utils/errorhandling.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/utils/looker_object_constructors.py` & `lmanage-0.3.8/lmanage/utils/looker_object_constructors.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/lmanage/utils/parse_yaml.py` & `lmanage-0.3.8/lmanage/utils/parse_yaml.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.7/pyproject.toml` & `lmanage-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lmanage"
-version = "0.3.07"
+version = "0.3.08"
 description = "LManage is a collection of useful tools for Looker admins to help curate and cleanup content and it's associated source LookML."
 keywords = ["keyword", "another_keyword"]
 authors = ["hselbie <hselbie@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/looker-open-source/lmanage"
 repository = "https://github.com/looker-open-source/lmanage"
```

### Comparing `lmanage-0.3.7/PKG-INFO` & `lmanage-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmanage
-Version: 0.3.7
+Version: 0.3.8
 Summary: LManage is a collection of useful tools for Looker admins to help curate and cleanup content and it's associated source LookML.
 Home-page: https://github.com/looker-open-source/lmanage
 Keywords: keyword,another_keyword
 Author: hselbie
 Author-email: hselbie@gmail.com
 Requires-Python: >=3.8,<3.9
 Classifier: Programming Language :: Python :: 3
```

