# Comparing `tmp/lmanage-0.3.6.tar.gz` & `tmp/lmanage-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmanage-0.3.6.tar", max compression
+gzip compressed data, was "lmanage-0.3.7.tar", max compression
```

## Comparing `lmanage-0.3.6.tar` & `lmanage-0.3.7.tar`

### file list

```diff
@@ -1,63 +1,65 @@
--rw-r--r--   0        0        0    11358 2021-07-16 17:02:14.912118 lmanage-0.3.6/LICENSE
--rw-r--r--   0        0        0     2695 2023-04-27 21:32:50.653908 lmanage-0.3.6/README.md
--rw-r--r--   0        0        0      926 2022-12-15 21:59:31.502790 lmanage-0.3.6/lmanage/.vimspector.json
--rw-r--r--   0        0        0      598 2023-03-23 16:57:22.191458 lmanage-0.3.6/lmanage/__init__.py
--rw-r--r--   0        0        0      598 2023-03-23 16:57:22.195458 lmanage-0.3.6/lmanage/capturator/__init__.py
--rw-r--r--   0        0        0     2063 2023-03-23 16:57:22.195458 lmanage-0.3.6/lmanage/capturator/commands.py
--rw-r--r--   0        0        0        0 2023-04-19 21:34:25.230519 lmanage-0.3.6/lmanage/capturator/content_capturation/__init__.py
--rw-r--r--   0        0        0     2406 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/capturator/content_capturation/dashboard_capture.py
--rw-r--r--   0        0        0     3227 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/capturator/content_capturation/look_capture.py
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.6/lmanage/capturator/folder_capturation/__init__.py
--rw-r--r--   0        0        0     1136 2023-04-19 21:34:25.230519 lmanage-0.3.6/lmanage/capturator/folder_capturation/create_folder_yaml_structure.py
--rw-r--r--   0        0        0     8063 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/capturator/folder_capturation/folder_config.py
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.6/lmanage/capturator/user_attribute_capturation/__init__.py
--rw-r--r--   0        0        0     2341 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/capturator/user_attribute_capturation/capture_ua_permissions.py
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.6/lmanage/capturator/user_group_capturation/__init__.py
--rw-r--r--   0        0        0     3565 2023-04-26 23:16:43.844504 lmanage-0.3.6/lmanage/capturator/user_group_capturation/group_config.py
--rw-r--r--   0        0        0     2923 2023-04-26 23:16:43.844504 lmanage-0.3.6/lmanage/capturator/user_group_capturation/role_config.py
--rw-r--r--   0        0        0     3765 2023-03-23 16:57:22.195458 lmanage-0.3.6/lmanage/capturator/user_group_capturation/user_permission.py
--rw-r--r--   0        0        0     4715 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/capture_instance_permission_structure.py
--rw-r--r--   0        0        0      928 2023-04-26 23:16:43.844504 lmanage-0.3.6/lmanage/cli.py
--rw-r--r--   0        0        0      353 2022-06-24 18:34:27.402555 lmanage-0.3.6/lmanage/configurator/.vimspector.json
--rw-r--r--   0        0        0      598 2023-03-23 16:57:22.191458 lmanage-0.3.6/lmanage/configurator/__init__.py
--rw-r--r--   0        0        0     2026 2023-03-23 16:57:22.191458 lmanage-0.3.6/lmanage/configurator/commands.py
--rw-r--r--   0        0        0        0 2023-04-19 21:34:25.230519 lmanage-0.3.6/lmanage/configurator/content_configuration/__init__.py
--rw-r--r--   0        0        0     2167 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/configurator/content_configuration/create_content_prep.py
--rw-r--r--   0        0        0     1045 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/configurator/content_configuration/create_dashboards.py
--rw-r--r--   0        0        0     4072 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/configurator/content_configuration/create_looks.py
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.191458 lmanage-0.3.6/lmanage/configurator/folder_configuration/__init__.py
--rw-r--r--   0        0        0    13653 2023-04-26 23:16:43.844504 lmanage-0.3.6/lmanage/configurator/folder_configuration/create_folder_permissions.py
--rw-r--r--   0        0        0     5786 2023-04-19 21:34:25.230519 lmanage-0.3.6/lmanage/configurator/folder_configuration/create_folders.py
--rw-r--r--   0        0        0     1615 2023-04-19 21:34:25.234519 lmanage-0.3.6/lmanage/configurator/folder_configuration/folder_config.py
--rw-r--r--   0        0        0     5706 2023-02-07 21:50:06.720732 lmanage-0.3.6/lmanage/configurator/instance_configuration_settings/fullinstance.yaml
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.191458 lmanage-0.3.6/lmanage/configurator/user_attribute_configuration/__init__.py
--rw-r--r--   0        0        0     4072 2023-04-19 21:34:25.234519 lmanage-0.3.6/lmanage/configurator/user_attribute_configuration/create_ua_permissions.py
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.6/lmanage/configurator/user_group_configuration/__init__.py
--rw-r--r--   0        0        0     4420 2023-04-26 23:16:43.844504 lmanage-0.3.6/lmanage/configurator/user_group_configuration/group_config.py
--rw-r--r--   0        0        0     5978 2023-04-26 23:16:43.848504 lmanage-0.3.6/lmanage/configurator/user_group_configuration/role_config.py
--rw-r--r--   0        0        0     4727 2023-04-26 23:16:43.848504 lmanage-0.3.6/lmanage/configurator/user_group_configuration/user_permission.py
--rwxr-xr-x   0        0        0      702 2022-12-15 21:59:31.634799 lmanage-0.3.6/lmanage/find_replace.sh
--rw-r--r--   0        0        0      446 2022-06-24 18:34:27.574567 lmanage-0.3.6/lmanage/mapview/.vimspector.json
--rw-r--r--   0        0        0      575 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/__init__.py
--rw-r--r--   0        0        0     3645 2023-03-23 16:57:22.191458 lmanage-0.3.6/lmanage/mapview/compare_content_to_lookml.py
--rw-r--r--   0        0        0     1873 2022-06-24 18:34:27.602569 lmanage-0.3.6/lmanage/mapview/hugo.csv
--rw-r--r--   0        0        0     2092 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/instancedata.py
--rw-r--r--   0        0        0    14973 2023-04-26 23:16:43.868505 lmanage-0.3.6/lmanage/mapview/legacy_get_content_with_views.py
--rw-r--r--   0        0        0     1633 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/main.py
--rw-r--r--   0        0        0     2773 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/mapexplores.py
--rw-r--r--   0        0        0     1503 2023-03-23 16:57:22.191458 lmanage-0.3.6/lmanage/mapview/mapview_execute.py
--rw-r--r--   0        0        0     2182 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/matched_field_analysis.py
--rw-r--r--   0        0        0     7197 2022-06-24 18:34:27.694576 lmanage-0.3.6/lmanage/mapview/pandas_multiple.xlsx
--rw-r--r--   0        0        0     2881 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/parse_sql_tables.py
--rw-r--r--   0        0        0      324 2022-06-24 18:34:27.714578 lmanage-0.3.6/lmanage/mapview/utils/.vimspector.json
--rw-r--r--   0        0        0      575 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/utils/__init__.py
--rw-r--r--   0        0        0     1234 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/utils/create_df.py
--rw-r--r--   0        0        0     3046 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/utils/parse_lookml.py
--rw-r--r--   0        0        0     5008 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/utils/parsing_sql.py
--rw-r--r--   0        0        0     6375 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/provision_instance_permission_structure.py
--rw-r--r--   0        0        0      575 2023-03-23 16:57:22.191458 lmanage-0.3.6/lmanage/utils/__init__.py
--rw-r--r--   0        0        0     1662 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/utils/errorhandling.py
--rw-r--r--   0        0        0     2643 2023-04-19 21:34:25.234519 lmanage-0.3.6/lmanage/utils/looker_object_constructors.py
--rw-r--r--   0        0        0     2027 2023-04-19 21:34:25.234519 lmanage-0.3.6/lmanage/utils/parse_yaml.py
--rw-r--r--   0        0        0     1029 2023-04-26 23:19:51.748692 lmanage-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     3995 1970-01-01 00:00:00.000000 lmanage-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11358 2021-07-16 17:02:14.912118 lmanage-0.3.7/LICENSE
+-rw-r--r--   0        0        0     2695 2023-04-27 21:32:50.653908 lmanage-0.3.7/README.md
+-rw-r--r--   0        0        0      926 2022-12-15 21:59:31.502790 lmanage-0.3.7/lmanage/.vimspector.json
+-rw-r--r--   0        0        0      598 2023-03-23 16:57:22.191458 lmanage-0.3.7/lmanage/__init__.py
+-rw-r--r--   0        0        0      598 2023-03-23 16:57:22.195458 lmanage-0.3.7/lmanage/capturator/__init__.py
+-rw-r--r--   0        0        0     2063 2023-03-23 16:57:22.195458 lmanage-0.3.7/lmanage/capturator/commands.py
+-rw-r--r--   0        0        0        0 2023-04-19 21:34:25.230519 lmanage-0.3.7/lmanage/capturator/content_capturation/__init__.py
+-rw-r--r--   0        0        0     1855 2023-05-08 17:34:54.913053 lmanage-0.3.7/lmanage/capturator/content_capturation/board_capture.py
+-rw-r--r--   0        0        0     2618 2023-05-04 22:07:41.433704 lmanage-0.3.7/lmanage/capturator/content_capturation/dashboard_capture.py
+-rw-r--r--   0        0        0     3227 2023-04-26 23:19:51.736692 lmanage-0.3.7/lmanage/capturator/content_capturation/look_capture.py
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.7/lmanage/capturator/folder_capturation/__init__.py
+-rw-r--r--   0        0        0     1136 2023-04-19 21:34:25.230519 lmanage-0.3.7/lmanage/capturator/folder_capturation/create_folder_yaml_structure.py
+-rw-r--r--   0        0        0     8063 2023-04-26 23:19:51.736692 lmanage-0.3.7/lmanage/capturator/folder_capturation/folder_config.py
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.7/lmanage/capturator/user_attribute_capturation/__init__.py
+-rw-r--r--   0        0        0     2341 2023-04-26 23:19:51.736692 lmanage-0.3.7/lmanage/capturator/user_attribute_capturation/capture_ua_permissions.py
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.7/lmanage/capturator/user_group_capturation/__init__.py
+-rw-r--r--   0        0        0     3565 2023-04-26 23:16:43.844504 lmanage-0.3.7/lmanage/capturator/user_group_capturation/group_config.py
+-rw-r--r--   0        0        0     2923 2023-04-26 23:16:43.844504 lmanage-0.3.7/lmanage/capturator/user_group_capturation/role_config.py
+-rw-r--r--   0        0        0     3765 2023-03-23 16:57:22.195458 lmanage-0.3.7/lmanage/capturator/user_group_capturation/user_permission.py
+-rw-r--r--   0        0        0     5141 2023-05-05 22:42:39.755506 lmanage-0.3.7/lmanage/capture_instance_permission_structure.py
+-rw-r--r--   0        0        0      928 2023-04-26 23:16:43.844504 lmanage-0.3.7/lmanage/cli.py
+-rw-r--r--   0        0        0      353 2022-06-24 18:34:27.402555 lmanage-0.3.7/lmanage/configurator/.vimspector.json
+-rw-r--r--   0        0        0      598 2023-03-23 16:57:22.191458 lmanage-0.3.7/lmanage/configurator/__init__.py
+-rw-r--r--   0        0        0     2026 2023-03-23 16:57:22.191458 lmanage-0.3.7/lmanage/configurator/commands.py
+-rw-r--r--   0        0        0        0 2023-04-19 21:34:25.230519 lmanage-0.3.7/lmanage/configurator/content_configuration/__init__.py
+-rw-r--r--   0        0        0     2716 2023-05-08 17:42:53.204117 lmanage-0.3.7/lmanage/configurator/content_configuration/create_boards.py
+-rw-r--r--   0        0        0     2679 2023-05-08 18:13:26.279080 lmanage-0.3.7/lmanage/configurator/content_configuration/create_content_prep.py
+-rw-r--r--   0        0        0     1343 2023-05-09 17:23:59.031587 lmanage-0.3.7/lmanage/configurator/content_configuration/create_dashboards.py
+-rw-r--r--   0        0        0     4072 2023-04-26 23:19:51.736692 lmanage-0.3.7/lmanage/configurator/content_configuration/create_looks.py
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.191458 lmanage-0.3.7/lmanage/configurator/folder_configuration/__init__.py
+-rw-r--r--   0        0        0    13653 2023-04-26 23:16:43.844504 lmanage-0.3.7/lmanage/configurator/folder_configuration/create_folder_permissions.py
+-rw-r--r--   0        0        0     5786 2023-04-19 21:34:25.230519 lmanage-0.3.7/lmanage/configurator/folder_configuration/create_folders.py
+-rw-r--r--   0        0        0     1615 2023-04-19 21:34:25.234519 lmanage-0.3.7/lmanage/configurator/folder_configuration/folder_config.py
+-rw-r--r--   0        0        0     5706 2023-02-07 21:50:06.720732 lmanage-0.3.7/lmanage/configurator/instance_configuration_settings/fullinstance.yaml
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.191458 lmanage-0.3.7/lmanage/configurator/user_attribute_configuration/__init__.py
+-rw-r--r--   0        0        0     4102 2023-05-09 17:06:42.831339 lmanage-0.3.7/lmanage/configurator/user_attribute_configuration/create_ua_permissions.py
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.7/lmanage/configurator/user_group_configuration/__init__.py
+-rw-r--r--   0        0        0     4420 2023-04-26 23:16:43.844504 lmanage-0.3.7/lmanage/configurator/user_group_configuration/group_config.py
+-rw-r--r--   0        0        0     5978 2023-04-26 23:16:43.848504 lmanage-0.3.7/lmanage/configurator/user_group_configuration/role_config.py
+-rw-r--r--   0        0        0     4727 2023-04-26 23:16:43.848504 lmanage-0.3.7/lmanage/configurator/user_group_configuration/user_permission.py
+-rwxr-xr-x   0        0        0      702 2022-12-15 21:59:31.634799 lmanage-0.3.7/lmanage/find_replace.sh
+-rw-r--r--   0        0        0      446 2022-06-24 18:34:27.574567 lmanage-0.3.7/lmanage/mapview/.vimspector.json
+-rw-r--r--   0        0        0      575 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/__init__.py
+-rw-r--r--   0        0        0     3645 2023-03-23 16:57:22.191458 lmanage-0.3.7/lmanage/mapview/compare_content_to_lookml.py
+-rw-r--r--   0        0        0     1873 2022-06-24 18:34:27.602569 lmanage-0.3.7/lmanage/mapview/hugo.csv
+-rw-r--r--   0        0        0     2092 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/instancedata.py
+-rw-r--r--   0        0        0    14973 2023-04-26 23:16:43.868505 lmanage-0.3.7/lmanage/mapview/legacy_get_content_with_views.py
+-rw-r--r--   0        0        0     1633 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/main.py
+-rw-r--r--   0        0        0     2773 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/mapexplores.py
+-rw-r--r--   0        0        0     1503 2023-03-23 16:57:22.191458 lmanage-0.3.7/lmanage/mapview/mapview_execute.py
+-rw-r--r--   0        0        0     2182 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/matched_field_analysis.py
+-rw-r--r--   0        0        0     7197 2022-06-24 18:34:27.694576 lmanage-0.3.7/lmanage/mapview/pandas_multiple.xlsx
+-rw-r--r--   0        0        0     2881 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/parse_sql_tables.py
+-rw-r--r--   0        0        0      324 2022-06-24 18:34:27.714578 lmanage-0.3.7/lmanage/mapview/utils/.vimspector.json
+-rw-r--r--   0        0        0      575 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/utils/__init__.py
+-rw-r--r--   0        0        0     1234 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/utils/create_df.py
+-rw-r--r--   0        0        0     3046 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/utils/parse_lookml.py
+-rw-r--r--   0        0        0     5008 2023-03-23 16:57:22.187458 lmanage-0.3.7/lmanage/mapview/utils/parsing_sql.py
+-rw-r--r--   0        0        0     6749 2023-05-09 17:19:57.683778 lmanage-0.3.7/lmanage/provision_instance_permission_structure.py
+-rw-r--r--   0        0        0      575 2023-03-23 16:57:22.191458 lmanage-0.3.7/lmanage/utils/__init__.py
+-rw-r--r--   0        0        0     1183 2023-05-03 23:35:07.193770 lmanage-0.3.7/lmanage/utils/errorhandling.py
+-rw-r--r--   0        0        0     3108 2023-05-08 17:34:24.651084 lmanage-0.3.7/lmanage/utils/looker_object_constructors.py
+-rw-r--r--   0        0        0     2247 2023-05-06 00:24:47.778206 lmanage-0.3.7/lmanage/utils/parse_yaml.py
+-rw-r--r--   0        0        0     1029 2023-05-09 17:26:59.015362 lmanage-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     3995 1970-01-01 00:00:00.000000 lmanage-0.3.7/PKG-INFO
```

### Comparing `lmanage-0.3.6/LICENSE` & `lmanage-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/README.md` & `lmanage-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/.vimspector.json` & `lmanage-0.3.7/lmanage/.vimspector.json`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/__init__.py` & `lmanage-0.3.7/lmanage/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/capturator/__init__.py` & `lmanage-0.3.7/lmanage/capturator/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/capturator/commands.py` & `lmanage-0.3.7/lmanage/capturator/commands.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/capturator/content_capturation/dashboard_capture.py` & `lmanage-0.3.7/lmanage/capturator/content_capturation/dashboard_capture.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,23 +15,25 @@
         self.folder_root = folder_root
 
     def get_all_dashboards(self) -> dict:
         system_folders = ['Users','Embed Users','Embed Groups', 'LookML Dashboards']
         scrub_dashboards = {}
         with yaspin().white.bold.shark.on_blue as sp:
             sp.text="getting all system dashboard metadata (can take a while)"
-            all_dashboards = self.sdk.all_dashboards(fields="id,folder")
+            all_dashboards = self.sdk.all_dashboards(fields="id,folder, slug")
         
         for dash in all_dashboards:
             if dash.folder.id == 'lookml':
                 continue
             else:
                 folder_root = self.folder_root.get(dash.folder.id, [{'name':'Users'}])[0]['name']
                 if dash.folder.id in list(self.folder_root.keys()) and folder_root not in system_folders:
-                    scrub_dashboards[dash.id] = dash.folder.id 
+                    scrub_dashboards[dash.id] = {}
+                    scrub_dashboards[dash.id]['folder_id'] = dash.folder.id
+                    scrub_dashboards[dash.id]['slug'] = dash.slug 
         return scrub_dashboards
 
     def get_dashboard_lookml(self, all_dashboards: dict) -> list:
         #logging.info("Beginning Dashboard Capture:")
         response = []
   
         for dash_id in tqdm(all_dashboards, desc = "Dashboard Capture", unit=" dashboards", colour="#2c8558"):
@@ -47,15 +49,16 @@
                         lookml = self.sdk.dashboard_lookml(dashboard_id=dash_id)
                     except:
                         return_sleep_message(call_number=trys, quiet=True)
                 
                 captured_dashboard = DashboardObject(
                     legacy_folder_id=all_dashboards.get(dash_id),
                     lookml=lookml.lookml,
-                    dashboard_id=dash_id)
+                    dashboard_id=dash_id,
+                    dashboard_slug=all_dashboards.get(dash_id).get('slug'))
                 response.append(captured_dashboard)
         return response
 
     def execute(self):
         all_dashboards = self.get_all_dashboards()
         captured_dash = self.get_dashboard_lookml(all_dashboards)
         return captured_dash
```

### Comparing `lmanage-0.3.6/lmanage/capturator/content_capturation/look_capture.py` & `lmanage-0.3.7/lmanage/capturator/content_capturation/look_capture.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/capturator/folder_capturation/create_folder_yaml_structure.py` & `lmanage-0.3.7/lmanage/capturator/folder_capturation/create_folder_yaml_structure.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/capturator/folder_capturation/folder_config.py` & `lmanage-0.3.7/lmanage/capturator/folder_capturation/folder_config.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/capturator/user_attribute_capturation/capture_ua_permissions.py` & `lmanage-0.3.7/lmanage/capturator/user_attribute_capturation/capture_ua_permissions.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/capturator/user_group_capturation/group_config.py` & `lmanage-0.3.7/lmanage/capturator/user_group_capturation/group_config.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/capturator/user_group_capturation/role_config.py` & `lmanage-0.3.7/lmanage/capturator/user_group_capturation/role_config.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/capturator/user_group_capturation/user_permission.py` & `lmanage-0.3.7/lmanage/capturator/user_group_capturation/user_permission.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/capture_instance_permission_structure.py` & `lmanage-0.3.7/lmanage/capture_instance_permission_structure.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import logging
 import coloredlogs
 import looker_sdk
 import ruamel.yaml
-import json
 from lmanage.capturator.user_group_capturation import role_config as rc
 from lmanage.capturator.user_attribute_capturation import capture_ua_permissions as cup
-from lmanage.capturator.folder_capturation import folder_config as fc
-from lmanage.capturator.folder_capturation import create_folder_yaml_structure as cfp
-from lmanage.capturator.content_capturation import dashboard_capture as dc
-from lmanage.capturator.content_capturation import look_capture as lc
-from lmanage.utils import looker_object_constructors as loc
+from lmanage.capturator.folder_capturation import folder_config as fc, create_folder_yaml_structure as cfp
+from lmanage.capturator.content_capturation import dashboard_capture as dc, look_capture as lc, board_capture as bc
+from lmanage.utils import looker_object_constructors as loc, errorhandling as eh
 
 logger = logging.getLogger(__name__)
 coloredlogs.install(level='INFO')
 logging.getLogger("looker_sdk").setLevel(logging.WARNING)
 
 
 def main(**kwargs):
@@ -24,23 +21,29 @@
 
     logger.info('creating yaml configuration file')
 
     if ini_file:
         sdk = looker_sdk.init40(config_file=ini_file)
     else:
         sdk = looker_sdk.init40()
+    if eh.user_authentication_test(sdk=sdk):
+        logger.info('User is successfully authenticated to the API')
+    else:
+        raise Exception(
+            "User is not successfully authenticated please verify credentials")
 
     yaml = ruamel.yaml.YAML()
     yaml.register_class(loc.LookerFolder)
     yaml.register_class(loc.LookerModelSet)
     yaml.register_class(loc.LookerPermissionSet)
     yaml.register_class(loc.LookerRoles)
     yaml.register_class(loc.LookerUserAttribute)
     yaml.register_class(loc.LookObject)
     yaml.register_class(loc.DashboardObject)
+    yaml.register_class(loc.BoardObject)
 
 ###############################################################
 # Capture Folder Config #######################################
 ###############################################################
     folder_returns = fc.CaptureFolderConfig(sdk=sdk).execute()
     folder_structure_list = folder_returns[1]
 
@@ -78,28 +81,35 @@
     with open(f'{yaml_path}.yaml', 'a') as file:
         file.write('\n\n# USER_ATTRIBUTES\n')
         yaml.dump(looker_ua, file)
 
 ###############################################################
 # Capture Users Content #######################################
 ###############################################################
-    # Capture Look Content
-    looks = lc.CaptureLookObject(sdk=sdk, folder_root=folder_root_dict).execute()
+    # Capture Content Boards
+    boards = bc.CaptureBoards(sdk=sdk).execute()
     with open(f'{yaml_path}_content.yaml', 'w+') as file:
+        file.write('\n\n# BoardData\n')
+        yaml.dump(boards, file)
+
+    # Capture Look Content
+    looks = lc.CaptureLookObject(
+        sdk=sdk, folder_root=folder_root_dict).execute()
+    with open(f'{yaml_path}_content.yaml', 'a') as file:
         file.write('\n\n# LookData\n')
         yaml.dump(looks, file)
 
     # Capture Dashboard Content
-    dash_content = dc.CaptureDashboards(sdk=sdk, folder_root=folder_root_dict).execute()
+    dash_content = dc.CaptureDashboards(
+        sdk=sdk, folder_root=folder_root_dict).execute()
     with open(f'{yaml_path}_content.yaml', 'a') as file:
         fd_yml_txt = '\n\n# Dashboard Content\n'
         file.write(fd_yml_txt)
         yaml.dump(dash_content, file)
 
-
     # FIND UNIQUE USER ATTRIBUTES AND ATTRIBUTE TO TEAM
     logger.info('\n\n\n Lmanage has finished capturing your Looker instance!\n')
     logger.info('\n\nplease find captured settings metadata at: \n%s.yaml \n\ncaptured content metadata at:\n%s_content.yaml', yaml_path, yaml_path)
 
 
 if __name__ == "__main__":
     instance = 'dev'
```

### Comparing `lmanage-0.3.6/lmanage/cli.py` & `lmanage-0.3.7/lmanage/cli.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/configurator/__init__.py` & `lmanage-0.3.7/lmanage/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/configurator/commands.py` & `lmanage-0.3.7/lmanage/configurator/commands.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/configurator/content_configuration/create_content_prep.py` & `lmanage-0.3.7/lmanage/configurator/content_configuration/create_content_prep.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,24 @@
     def empty_looker_look_trash(self) -> None:
         trash_look = self.sdk.search_looks(deleted=True)
         trash_look_id_list = [look.id for look in trash_look]
         for look_id in tqdm(trash_look_id_list, 'Emptying Look Trash', unit='Look', colour="#2c8558"):
             self.sdk.delete_look(look_id=look_id)
             logger.debug(
                 f'cleaning the trash dashboard {look_id} from instance')
+                
+                
+    def delete_boards(self, all_board: list) -> None:
+        delete_board_list = [board.id for board in all_board]
+        for board_id in tqdm(delete_board_list, 'Scrubbing Instance Boards', unit='boards', colour="#2c8558"):
+            self.sdk.delete_board(board_id=board_id)
+            logger.debug(
+                f'cleaning the trash board {board_id} from instance')
+
+
 
     def delete_instance_dash(self, dashboards: list) -> None:
         delete_id_list = [dash.id for dash in dashboards]
         for dash_id in tqdm(delete_id_list, 'Scrubbing Instance Dashboards', unit='dashboards', colour="#2c8558"):
             self.sdk.delete_dashboard(dashboard_id=dash_id)
             logger.debug(
                 f'cleaning the trash dashboard {dash_id} from instance')
@@ -37,11 +47,13 @@
             self.sdk.delete_look(look_id=look_id)
             logger.debug(
                 f'cleaning the trash dashboard {look_id} from instance')
 
     def execute(self):
         all_dash_list = self.sdk.all_dashboards()
         all_look_list = self.sdk.all_looks()
+        all_board_list = self.sdk.all_boards()
         self.delete_instance_dash(dashboards=all_dash_list)
         self.delete_instance_look(looks=all_look_list   )
+        self.delete_boards(all_board=all_board_list)
         self.empty_looker_dashboard_trash()
         self.empty_looker_look_trash()
```

### Comparing `lmanage-0.3.6/lmanage/configurator/content_configuration/create_dashboards.py` & `lmanage-0.3.7/lmanage/configurator/content_configuration/create_dashboards.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,20 +10,28 @@
     def __init__(self, sdk, folder_mapping, content_metadata) -> None:
         self.sdk = sdk
         self.folder_mapping = folder_mapping
         self.content_metadata = content_metadata
 
     
     def upload_dashboards(self) -> None:
+        resp = []
         for dash in tqdm(self.content_metadata, desc = "Dashboard Upload", unit="dashboards", colour="#2c8558"):
-            t = dash.get('legacy_folder_id')
+            print(type(dash))
+            t = dash.get('legacy_folder_id').get('folder_id')
             new_folder_id = self.folder_mapping.get(t)
             new_folder_id = new_folder_id if new_folder_id != 'Shared' else 1 
             body = models.WriteDashboardLookml(
                 folder_id=new_folder_id, 
                 lookml=dash['lookml']
             )
             # lookml = self.amend_lookml_str(dash['lookml'])
-            self.sdk.import_dashboard_from_lookml(body=body)
+            temp = {}
+            new_dash = self.sdk.import_dashboard_from_lookml(body=body)
+            temp[dash['dashboard_id']] = new_dash.dashboard_id if new_dash.dashboard_id else dash['dashboard_slug']
+            resp.append(temp)
+        return resp
+
 
     def execute(self):
-        self.upload_dashboards()
+        mapping = self.upload_dashboards()
+        return mapping
```

### Comparing `lmanage-0.3.6/lmanage/configurator/content_configuration/create_looks.py` & `lmanage-0.3.7/lmanage/configurator/content_configuration/create_looks.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/configurator/folder_configuration/create_folder_permissions.py` & `lmanage-0.3.7/lmanage/configurator/folder_configuration/create_folder_permissions.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/configurator/folder_configuration/create_folders.py` & `lmanage-0.3.7/lmanage/configurator/folder_configuration/create_folders.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/configurator/folder_configuration/folder_config.py` & `lmanage-0.3.7/lmanage/configurator/folder_configuration/folder_config.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/configurator/instance_configuration_settings/fullinstance.yaml` & `lmanage-0.3.7/lmanage/configurator/instance_configuration_settings/fullinstance.yaml`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/configurator/user_attribute_configuration/create_ua_permissions.py` & `lmanage-0.3.7/lmanage/configurator/user_attribute_configuration/create_ua_permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     def sync_user_attributes(self):
         instance_ua = self.existing_user_attributes()
         config_ua = [ua.get('name') for ua in self.user_attribute_metadata]
         sys_default_ua = [
             'email',
             'first_name',
             'id',
+            'google_user_id',
             'landing_page',
             'last_name',
             'number_format',
             'locale',
             'name'
         ]
```

### Comparing `lmanage-0.3.6/lmanage/configurator/user_group_configuration/group_config.py` & `lmanage-0.3.7/lmanage/configurator/user_group_configuration/group_config.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/configurator/user_group_configuration/role_config.py` & `lmanage-0.3.7/lmanage/configurator/user_group_configuration/role_config.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/configurator/user_group_configuration/user_permission.py` & `lmanage-0.3.7/lmanage/configurator/user_group_configuration/user_permission.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/find_replace.sh` & `lmanage-0.3.7/lmanage/find_replace.sh`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/mapview/__init__.py` & `lmanage-0.3.7/lmanage/mapview/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/mapview/compare_content_to_lookml.py` & `lmanage-0.3.7/lmanage/mapview/compare_content_to_lookml.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/mapview/hugo.csv` & `lmanage-0.3.7/lmanage/mapview/hugo.csv`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/mapview/instancedata.py` & `lmanage-0.3.7/lmanage/mapview/instancedata.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/mapview/legacy_get_content_with_views.py` & `lmanage-0.3.7/lmanage/mapview/legacy_get_content_with_views.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/mapview/main.py` & `lmanage-0.3.7/lmanage/mapview/main.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/mapview/mapexplores.py` & `lmanage-0.3.7/lmanage/mapview/mapexplores.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/mapview/mapview_execute.py` & `lmanage-0.3.7/lmanage/mapview/mapview_execute.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/mapview/matched_field_analysis.py` & `lmanage-0.3.7/lmanage/mapview/matched_field_analysis.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/mapview/pandas_multiple.xlsx` & `lmanage-0.3.7/lmanage/mapview/pandas_multiple.xlsx`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/mapview/parse_sql_tables.py` & `lmanage-0.3.7/lmanage/mapview/parse_sql_tables.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/mapview/utils/__init__.py` & `lmanage-0.3.7/lmanage/mapview/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/mapview/utils/create_df.py` & `lmanage-0.3.7/lmanage/mapview/utils/create_df.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/mapview/utils/parse_lookml.py` & `lmanage-0.3.7/lmanage/mapview/utils/parse_lookml.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/mapview/utils/parsing_sql.py` & `lmanage-0.3.7/lmanage/mapview/utils/parsing_sql.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/provision_instance_permission_structure.py` & `lmanage-0.3.7/lmanage/provision_instance_permission_structure.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 import logging
 import coloredlogs
 import looker_sdk
 from lmanage.configurator.user_attribute_configuration import create_ua_permissions as cuap
-from lmanage.configurator.folder_configuration import folder_config as fc
-from lmanage.configurator.folder_configuration import create_folder_permissions as cfp
-from lmanage.configurator.folder_configuration import create_folders as cf
-from lmanage.configurator.user_group_configuration import role_config as rc
-from lmanage.configurator.user_group_configuration import group_config as gc
-from lmanage.configurator.user_group_configuration import user_permission as up
-from lmanage.configurator.content_configuration import create_looks as cl
-from lmanage.configurator.content_configuration import create_dashboards as cd
-from lmanage.configurator.content_configuration import create_content_prep as ccp
-from lmanage.utils import parse_yaml as py
+from lmanage.configurator.folder_configuration import folder_config as fc, create_folder_permissions as cfp, create_folders as cf
+from lmanage.configurator.user_group_configuration import role_config as rc, group_config as gc, user_permission as up
+from lmanage.configurator.content_configuration import create_looks as cl, create_dashboards as cd, create_content_prep as ccp, create_boards as cb
+from lmanage.utils import parse_yaml as py, errorhandling as eh
 
 
 logger = logging.getLogger(__name__)
 coloredlogs.install(level='INFO')
 logging.getLogger("looker_sdk").setLevel(logging.WARNING)
 
 
@@ -30,14 +24,19 @@
     settings_yaml = py.Yaml(yaml_path=f'{yaml_split[0]}.yaml')
     content_yaml = py.Yaml(yaml_path=f'{yaml_split[0]}_content.yaml')
 
     if ini_file:
         sdk = looker_sdk.init40(config_file=ini_file)
     else:
         sdk = looker_sdk.init40()
+    
+    if eh.user_authentication_test(sdk=sdk):
+        logger.info('User is successfully authenticated to the API')
+    else:
+        raise Exception("User is not successfully authenticated please verify credentials")
 
     folder_metadata = settings_yaml.get_folder_metadata()
     if not folder_metadata:
         logger.warn(
             f'no folder_metadata specified please check your yaml file at {yaml_split[0]}.yaml')
     permission_set_metadata = settings_yaml.get_permission_metadata()
     if not permission_set_metadata:
@@ -62,14 +61,19 @@
             f'no look_metadata specified please check your yaml file at {yaml_split[0]}_content.yaml')
 
     dash_metadata = content_yaml.get_dash_metadata()
     if not dash_metadata:
         logger.warn(
             f'no dash_metadata specified please check your yaml file at {yaml_split[0]}_content.yaml')
 
+    board_metadata = content_yaml.get_board_metadata()
+    if not board_metadata:
+        logger.warn(
+            f'no board_metadata specified please check your yaml file at {yaml_split[0]}_content.yaml')
+
 
 ################################################################
 # Role Config ################################################
 ################################################################
     # Create Permission and Model Sets
     rc.CreateRoleBase(permissions=permission_set_metadata,
                       model_sets=model_set_metadata, sdk=sdk).execute()
@@ -119,20 +123,24 @@
 ###############################################################
     # EMPTY TRASH CAN OF ALL DELETED CONTENT
     ccp.CleanInstanceContent(sdk=sdk).execute()
     
     # FIND LOOKS AND REMAKE THEM
     look_creator = cl.CreateInstanceLooks(
         folder_mapping=folder_mapping_obj, sdk=sdk, content_metadata=look_metadata)
-    look_creator.execute()
+    look_mapping_dict = look_creator.execute()
 
     # Find DASHBOARDS AND REMAKE THEM
     dash_creator = cd.Create_Dashboards(
         sdk=sdk, folder_mapping=folder_mapping_obj, content_metadata=dash_metadata)
-    dash_creator.execute()
+    content_mapping_dict = dash_creator.execute()
+
+    # REMAKE BOARDS
+    # board_creator = cb.Create_Boards(sdk=sdk,board_metadata=board_metadata, dashboard_mapping=dash_creator, look_mapping=look_creator)
+    # board_creator.execute()
 
     logger.info('lmanage has finished configuring your Looker instance!')
 
 
 if __name__ == "__main__":
     YP = ('/usr/local/google/home/hugoselbie/code_sample/py/'
           'lmanage/tests/example_yamls/dev_output.yaml')
```

### Comparing `lmanage-0.3.6/lmanage/utils/__init__.py` & `lmanage-0.3.7/lmanage/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.6/lmanage/utils/errorhandling.py` & `lmanage-0.3.7/lmanage/utils/errorhandling.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ast
 import logging
 import coloredlogs
+from looker_sdk import error
 from time import sleep
 import random
 
 logger = logging.getLogger(__name__)
 coloredlogs.install(level='DEBUG')
 
 
@@ -19,39 +20,21 @@
     if len(input.errors) == 0:
         err_response = input.message
     else:
         err_response = input.errors[0].message
 
     return err_response
 
-def backoff_jitter(func):
-    """
-    This decorator adds jitter to a loop.
-    Args:
-      delay: The delay in seconds.
-    Returns:
-      A decorator that adds jitter to a loop.
-    """
-    def wrapper(*args, **kwargs):
-        result = func(*args, **kwargs)
-        jitter_delay = random.uniform(0.3,1.3)
-        sleep(jitter_delay)
-        print(f' {jitter_delay}')
-        return result
-    return wrapper
-
-    # def (func):
-    #     def wrapper(*args, **kwargs):
-    #         for _ in range(int(delay)):
-    #             func(*args, **kwargs)
-    #             sleep(random.uniform(0, delay))
-    #     return wrapper
-    # return decorator
-
-
+def user_authentication_test(sdk) -> bool:
+    try:
+        sdk.me()
+        return True
+    except error.SDKError():
+        return False
+    
 def return_sleep_message(call_number=0, quiet=False):
     call_number = call_number+1
     sleep_number = 2 ** call_number
     sleep(sleep_number)
     if not quiet:
         logger.warn(f'Looker is overwhelmed sleeping for {sleep_number} secs')
```

### Comparing `lmanage-0.3.6/lmanage/utils/looker_object_constructors.py` & `lmanage-0.3.7/lmanage/utils/looker_object_constructors.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,11 +78,22 @@
         self.look_id = look_id
         self.title = title
         self.query_obj = query_obj
         self.description = description
 
 
 class DashboardObject():
-    def __init__(self, legacy_folder_id, lookml, dashboard_id) -> None:
+    def __init__(self, legacy_folder_id, lookml, dashboard_id, dashboard_slug) -> None:
         self.legacy_folder_id = legacy_folder_id
         self.lookml = lookml
-        self.dashboard_id = dashboard_id
+        self.dashboard_id = dashboard_id
+        self.dashboard_slug = dashboard_slug
+
+
+class BoardObject():
+    def __init__(self, content_metadata_id, section_order, title, primary_homepage, board_sections, description) -> None:
+        self.content_metadata_id = content_metadata_id
+        self.section_order = section_order
+        self.title = title
+        self.primary_homepage = primary_homepage
+        self.board_sections = board_sections
+        self.description = description
```

### Comparing `lmanage-0.3.6/lmanage/utils/parse_yaml.py` & `lmanage-0.3.7/lmanage/utils/parse_yaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,7 +59,14 @@
     
     def get_dash_metadata(self):
         response = []
         for objects in self.parsed_yaml:
             if 'lookml' in list(objects.keys()):
                 response.append(objects)
         return response
+
+    def get_board_metadata(self):
+        response = []
+        for objects in self.parsed_yaml:
+            if 'board_sections' in list(objects.keys()):
+                response.append(objects)
+        return response
```

### Comparing `lmanage-0.3.6/pyproject.toml` & `lmanage-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lmanage"
-version = "0.3.06"
+version = "0.3.07"
 description = "LManage is a collection of useful tools for Looker admins to help curate and cleanup content and it's associated source LookML."
 keywords = ["keyword", "another_keyword"]
 authors = ["hselbie <hselbie@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/looker-open-source/lmanage"
 repository = "https://github.com/looker-open-source/lmanage"
```

### Comparing `lmanage-0.3.6/PKG-INFO` & `lmanage-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmanage
-Version: 0.3.6
+Version: 0.3.7
 Summary: LManage is a collection of useful tools for Looker admins to help curate and cleanup content and it's associated source LookML.
 Home-page: https://github.com/looker-open-source/lmanage
 Keywords: keyword,another_keyword
 Author: hselbie
 Author-email: hselbie@gmail.com
 Requires-Python: >=3.8,<3.9
 Classifier: Programming Language :: Python :: 3
```

