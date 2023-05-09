# Comparing `tmp/neurospeed-2.1.6.tar.gz` & `tmp/neurospeed-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurospeed-2.1.6.tar", last modified: Mon Dec 19 21:08:34 2022, max compression
+gzip compressed data, was "neurospeed-2.1.7.tar", last modified: Tue May  9 15:39:03 2023, max compression
```

## Comparing `neurospeed-2.1.6.tar` & `neurospeed-2.1.7.tar`

### file list

```diff
@@ -1,70 +1,74 @@
-drwxrwxrwx   0        0        0        0 2022-12-19 21:08:34.656893 neurospeed-2.1.6/
--rw-rw-rw-   0        0        0      747 2022-11-15 19:21:32.000000 neurospeed-2.1.6/.gitignore
--rw-rw-rw-   0        0        0     1003 2021-11-12 11:41:41.000000 neurospeed-2.1.6/CHANGES.txt
--rw-rw-rw-   0        0        0     1086 2021-11-02 09:20:12.000000 neurospeed-2.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0     1040 2022-12-19 21:08:34.656893 neurospeed-2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      600 2021-11-03 13:17:48.000000 neurospeed-2.1.6/README.md
--rw-rw-rw-   0        0        0     2214 2021-11-02 09:20:12.000000 neurospeed-2.1.6/README.txt
-drwxrwxrwx   0        0        0        0 2022-12-19 21:08:34.606572 neurospeed-2.1.6/examples/
--rw-rw-rw-   0        0        0    14290 2022-01-11 09:48:01.000000 neurospeed-2.1.6/examples/brainwave_to_midi.py
--rw-rw-rw-   0        0        0    14366 2022-01-19 12:05:37.000000 neurospeed-2.1.6/examples/cognitive_effort_index.py
-drwxrwxrwx   0        0        0        0 2022-12-19 21:08:34.616608 neurospeed-2.1.6/examples/config/
--rw-rw-rw-   0        0        0      241 2021-11-02 09:20:12.000000 neurospeed-2.1.6/examples/config/api_config.json
--rw-rw-rw-   0        0        0      107 2021-11-23 15:38:49.000000 neurospeed-2.1.6/examples/config/customer_config.json
--rw-rw-rw-   0        0        0      145 2022-11-15 19:09:22.000000 neurospeed-2.1.6/examples/config/hia_config1.json
--rw-rw-rw-   0        0        0      145 2022-11-15 19:09:22.000000 neurospeed-2.1.6/examples/config/hia_config2.json
--rw-rw-rw-   0        0        0     7334 2022-11-15 19:09:22.000000 neurospeed-2.1.6/examples/customer_api_flow_example_main.py
--rw-rw-rw-   0        0        0     1771 2022-11-15 19:09:22.000000 neurospeed-2.1.6/examples/downlink_receive_to_HIA_example.py
--rw-rw-rw-   0        0        0     3097 2022-11-15 19:09:22.000000 neurospeed-2.1.6/examples/downlink_send_to_HIA_example.py
--rw-rw-rw-   0        0        0     4863 2022-11-15 19:09:22.000000 neurospeed-2.1.6/examples/export_recorded_user_data_example_main.py
--rw-rw-rw-   0        0        0     7303 2021-11-12 10:23:11.000000 neurospeed-2.1.6/examples/fatigue_notifier_whatsapp_example.py
--rw-rw-rw-   0        0        0     6031 2022-11-16 14:06:37.000000 neurospeed-2.1.6/examples/hia_user_data_sender_example_main.py
--rw-rw-rw-   0        0        0    13540 2022-01-11 14:30:43.000000 neurospeed-2.1.6/examples/plot_engagement_index.py
--rw-rw-rw-   0        0        0    13131 2022-06-23 11:55:31.000000 neurospeed-2.1.6/examples/plot_raw_data_example.py
--rw-rw-rw-   0        0        0     4570 2022-11-15 19:09:22.000000 neurospeed-2.1.6/examples/query_connections_example_main.py
--rw-rw-rw-   0        0        0     8715 2022-11-15 19:09:22.000000 neurospeed-2.1.6/examples/record_raw_data.py
--rw-rw-rw-   0        0        0     3772 2022-11-15 19:09:22.000000 neurospeed-2.1.6/examples/record_user_data_example_main.py
--rw-rw-rw-   0        0        0     2628 2022-11-15 19:09:22.000000 neurospeed-2.1.6/examples/user_api_flow_example_main.py
--rw-rw-rw-   0        0        0      236 2022-11-16 14:06:37.000000 neurospeed-2.1.6/howto.txt
-drwxrwxrwx   0        0        0        0 2022-12-19 21:08:34.616608 neurospeed-2.1.6/images/
--rw-rw-rw-   0        0        0    64772 2021-11-03 13:06:02.000000 neurospeed-2.1.6/images/logo.PNG
-drwxrwxrwx   0        0        0        0 2022-12-19 21:08:34.616608 neurospeed-2.1.6/neurospeed/
--rw-rw-rw-   0        0        0        0 2021-11-02 09:20:12.000000 neurospeed-2.1.6/neurospeed/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-19 21:08:34.626731 neurospeed-2.1.6/neurospeed/api_http_handlers/
--rw-rw-rw-   0        0        0        0 2021-11-02 09:20:12.000000 neurospeed-2.1.6/neurospeed/api_http_handlers/__init__.py
--rw-rw-rw-   0        0        0     3687 2022-11-15 19:11:48.000000 neurospeed-2.1.6/neurospeed/api_http_handlers/exporter_http_handler.py
--rw-rw-rw-   0        0        0     1240 2022-11-15 19:09:22.000000 neurospeed-2.1.6/neurospeed/api_http_handlers/gateway_http_handler.py
--rw-rw-rw-   0        0        0     3802 2022-11-15 19:11:32.000000 neurospeed-2.1.6/neurospeed/api_http_handlers/recorder_http_handler.py
--rw-rw-rw-   0        0        0     2477 2022-11-15 19:09:22.000000 neurospeed-2.1.6/neurospeed/api_http_handlers/ssr_http_handler.py
-drwxrwxrwx   0        0        0        0 2022-12-19 21:08:34.636767 neurospeed-2.1.6/neurospeed/api_socket_handlers/
--rw-rw-rw-   0        0        0        0 2021-11-02 09:20:12.000000 neurospeed-2.1.6/neurospeed/api_socket_handlers/__init__.py
--rw-rw-rw-   0        0        0     4401 2022-11-15 19:09:22.000000 neurospeed-2.1.6/neurospeed/api_socket_handlers/customer_room_handler.py
--rw-rw-rw-   0        0        0     3250 2022-11-15 19:09:22.000000 neurospeed-2.1.6/neurospeed/api_socket_handlers/downlink_room_as_customer_handler.py
--rw-rw-rw-   0        0        0     3935 2022-11-15 19:09:22.000000 neurospeed-2.1.6/neurospeed/api_socket_handlers/downlink_room_as_user_handler.py
--rw-rw-rw-   0        0        0     4550 2022-11-15 19:09:22.000000 neurospeed-2.1.6/neurospeed/api_socket_handlers/user_room_as_customer_handler.py
--rw-rw-rw-   0        0        0     4264 2022-12-19 21:07:42.000000 neurospeed-2.1.6/neurospeed/api_socket_handlers/user_room_as_user_handler.py
-drwxrwxrwx   0        0        0        0 2022-12-19 21:08:34.644834 neurospeed-2.1.6/neurospeed/auth/
--rw-rw-rw-   0        0        0        0 2021-11-02 09:20:12.000000 neurospeed-2.1.6/neurospeed/auth/__init__.py
--rw-rw-rw-   0        0        0     3059 2022-11-15 19:09:22.000000 neurospeed-2.1.6/neurospeed/auth/auth_as_customer_handler.py
--rw-rw-rw-   0        0        0     3324 2022-11-15 19:09:22.000000 neurospeed-2.1.6/neurospeed/auth/auth_as_user_handler.py
-drwxrwxrwx   0        0        0        0 2022-12-19 21:08:34.646852 neurospeed-2.1.6/neurospeed/config/
--rw-rw-rw-   0        0        0      241 2021-11-02 09:20:12.000000 neurospeed-2.1.6/neurospeed/config/api_config.json
--rw-rw-rw-   0        0        0       78 2021-11-02 14:38:19.000000 neurospeed-2.1.6/neurospeed/config/customer_config.json
--rw-rw-rw-   0        0        0      145 2022-11-15 19:09:22.000000 neurospeed-2.1.6/neurospeed/config/hia_config1.json
--rw-rw-rw-   0        0        0      145 2022-11-15 19:09:22.000000 neurospeed-2.1.6/neurospeed/config/hia_config2.json
-drwxrwxrwx   0        0        0        0 2022-12-19 21:08:34.646852 neurospeed-2.1.6/neurospeed/hia_user_data/
--rw-rw-rw-   0        0        0        0 2021-11-02 09:20:12.000000 neurospeed-2.1.6/neurospeed/hia_user_data/__init__.py
--rw-rw-rw-   0        0        0    11991 2022-12-07 10:02:35.000000 neurospeed-2.1.6/neurospeed/hia_user_data/neurobrave_sensor_interface.py
-drwxrwxrwx   0        0        0        0 2022-12-19 21:08:34.656893 neurospeed-2.1.6/neurospeed/utils/
--rw-rw-rw-   0        0        0        0 2021-11-02 09:20:12.000000 neurospeed-2.1.6/neurospeed/utils/__init__.py
--rw-rw-rw-   0        0        0     2239 2022-12-07 10:03:18.000000 neurospeed-2.1.6/neurospeed/utils/api_config_service.py
--rw-rw-rw-   0        0        0      508 2022-11-15 19:09:22.000000 neurospeed-2.1.6/neurospeed/utils/helper_service.py
--rw-rw-rw-   0        0        0     3726 2022-11-15 19:09:22.000000 neurospeed-2.1.6/neurospeed/utils/http_service.py
-drwxrwxrwx   0        0        0        0 2022-12-19 21:08:34.624713 neurospeed-2.1.6/neurospeed.egg-info/
--rw-rw-rw-   0        0        0     1040 2022-12-19 21:08:33.000000 neurospeed-2.1.6/neurospeed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2063 2022-12-19 21:08:34.000000 neurospeed-2.1.6/neurospeed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-19 21:08:33.000000 neurospeed-2.1.6/neurospeed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2022-12-19 21:08:34.000000 neurospeed-2.1.6/neurospeed.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-12-19 21:08:34.000000 neurospeed-2.1.6/neurospeed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-19 21:08:34.656893 neurospeed-2.1.6/setup.cfg
--rw-rw-rw-   0        0        0      821 2022-12-19 21:08:06.000000 neurospeed-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:39:03.015618 neurospeed-2.1.7/
+-rw-rw-rw-   0        0        0      747 2022-11-15 19:21:32.000000 neurospeed-2.1.7/.gitignore
+-rw-rw-rw-   0        0        0     1003 2021-11-12 11:41:41.000000 neurospeed-2.1.7/CHANGES.txt
+-rw-rw-rw-   0        0        0     1086 2021-11-02 09:20:12.000000 neurospeed-2.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     1040 2023-05-09 15:39:03.014621 neurospeed-2.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2021-11-03 13:17:48.000000 neurospeed-2.1.7/README.md
+-rw-rw-rw-   0        0        0     2214 2021-11-02 09:20:12.000000 neurospeed-2.1.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 15:39:02.980151 neurospeed-2.1.7/examples/
+-rw-rw-rw-   0        0        0    14290 2022-01-11 09:48:01.000000 neurospeed-2.1.7/examples/brainwave_to_midi.py
+-rw-rw-rw-   0        0        0    14366 2022-01-19 12:05:37.000000 neurospeed-2.1.7/examples/cognitive_effort_index.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:39:02.982764 neurospeed-2.1.7/examples/config/
+-rw-rw-rw-   0        0        0      306 2023-05-09 15:11:47.000000 neurospeed-2.1.7/examples/config/api_config.json
+-rw-rw-rw-   0        0        0       78 2023-05-09 15:11:29.000000 neurospeed-2.1.7/examples/config/customer_config.json
+-rw-rw-rw-   0        0        0      131 2023-05-09 15:09:10.000000 neurospeed-2.1.7/examples/config/hia_config1.json
+-rw-rw-rw-   0        0        0      131 2023-05-09 15:09:18.000000 neurospeed-2.1.7/examples/config/hia_config2.json
+-rw-rw-rw-   0        0        0     7334 2022-11-15 19:09:22.000000 neurospeed-2.1.7/examples/customer_api_flow_example_main.py
+-rw-rw-rw-   0        0        0     1771 2022-11-15 19:09:22.000000 neurospeed-2.1.7/examples/downlink_receive_to_HIA_example.py
+-rw-rw-rw-   0        0        0     3097 2022-11-15 19:09:22.000000 neurospeed-2.1.7/examples/downlink_send_to_HIA_example.py
+-rw-rw-rw-   0        0        0     4863 2022-11-15 19:09:22.000000 neurospeed-2.1.7/examples/export_recorded_user_data_example_main.py
+-rw-rw-rw-   0        0        0     7303 2021-11-12 10:23:11.000000 neurospeed-2.1.7/examples/fatigue_notifier_whatsapp_example.py
+-rw-rw-rw-   0        0        0    13540 2022-01-11 14:30:43.000000 neurospeed-2.1.7/examples/plot_engagement_index.py
+-rw-rw-rw-   0        0        0    13131 2022-06-23 11:55:31.000000 neurospeed-2.1.7/examples/plot_raw_data_example.py
+-rw-rw-rw-   0        0        0       22 2021-11-11 17:26:19.000000 neurospeed-2.1.7/examples/pywhatkit_dbs.txt
+-rw-rw-rw-   0        0        0     4570 2022-11-15 19:09:22.000000 neurospeed-2.1.7/examples/query_connections_example_main.py
+-rw-rw-rw-   0        0        0     8715 2022-11-15 19:09:22.000000 neurospeed-2.1.7/examples/record_raw_data.py
+-rw-rw-rw-   0        0        0     3772 2022-11-15 19:09:22.000000 neurospeed-2.1.7/examples/record_user_data_example_main.py
+-rw-rw-rw-   0        0        0     4343 2022-12-11 13:20:54.000000 neurospeed-2.1.7/examples/simple_get_data_packet.py
+-rw-rw-rw-   0        0        0     2628 2022-11-15 19:09:22.000000 neurospeed-2.1.7/examples/user_api_flow_example_main.py
+-rw-rw-rw-   0        0        0      236 2022-11-16 14:06:37.000000 neurospeed-2.1.7/howto.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 15:39:02.983765 neurospeed-2.1.7/images/
+-rw-rw-rw-   0        0        0    64772 2021-11-03 13:06:02.000000 neurospeed-2.1.7/images/logo.PNG
+drwxrwxrwx   0        0        0        0 2023-05-09 15:39:02.984812 neurospeed-2.1.7/neurospeed/
+-rw-rw-rw-   0        0        0        0 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:39:02.999838 neurospeed-2.1.7/neurospeed/api_http_handlers/
+-rw-rw-rw-   0        0        0        0 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/api_http_handlers/__init__.py
+-rw-rw-rw-   0        0        0     3687 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/api_http_handlers/exporter_http_handler.py
+-rw-rw-rw-   0        0        0     1240 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/api_http_handlers/gateway_http_handler.py
+-rw-rw-rw-   0        0        0     3802 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/api_http_handlers/recorder_http_handler.py
+-rw-rw-rw-   0        0        0     2477 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/api_http_handlers/ssr_http_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:39:03.003826 neurospeed-2.1.7/neurospeed/api_socket_handlers/
+-rw-rw-rw-   0        0        0        0 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/api_socket_handlers/__init__.py
+-rw-rw-rw-   0        0        0     4401 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/api_socket_handlers/customer_room_handler.py
+-rw-rw-rw-   0        0        0     3250 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/api_socket_handlers/downlink_room_as_customer_handler.py
+-rw-rw-rw-   0        0        0     3935 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/api_socket_handlers/downlink_room_as_user_handler.py
+-rw-rw-rw-   0        0        0     4550 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/api_socket_handlers/user_room_as_customer_handler.py
+-rw-rw-rw-   0        0        0     4264 2022-12-19 18:19:09.000000 neurospeed-2.1.7/neurospeed/api_socket_handlers/user_room_as_user_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:39:03.005873 neurospeed-2.1.7/neurospeed/auth/
+-rw-rw-rw-   0        0        0        0 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/auth/__init__.py
+-rw-rw-rw-   0        0        0     3059 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/auth/auth_as_customer_handler.py
+-rw-rw-rw-   0        0        0     3324 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/auth/auth_as_user_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:39:03.008586 neurospeed-2.1.7/neurospeed/config/
+-rw-rw-rw-   0        0        0      241 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/config/api_config.json
+-rw-rw-rw-   0        0        0       78 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/config/customer_config.json
+-rw-rw-rw-   0        0        0      145 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/config/hia_config1.json
+-rw-rw-rw-   0        0        0      145 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/config/hia_config2.json
+drwxrwxrwx   0        0        0        0 2023-05-09 15:39:03.009585 neurospeed-2.1.7/neurospeed/hia_user_data/
+-rw-rw-rw-   0        0        0        0 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/hia_user_data/__init__.py
+-rw-rw-rw-   0        0        0    12229 2023-03-26 17:29:25.000000 neurospeed-2.1.7/neurospeed/hia_user_data/neurobrave_sensor_interface.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:39:03.011579 neurospeed-2.1.7/neurospeed/macros/
+-rw-rw-rw-   0        0        0        0 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/macros/__init__.py
+-rw-rw-rw-   0        0        0     8242 2023-05-09 14:22:06.000000 neurospeed-2.1.7/neurospeed/macros/macros.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:39:03.013574 neurospeed-2.1.7/neurospeed/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/utils/__init__.py
+-rw-rw-rw-   0        0        0     2239 2022-11-29 12:12:19.000000 neurospeed-2.1.7/neurospeed/utils/api_config_service.py
+-rw-rw-rw-   0        0        0      508 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/utils/helper_service.py
+-rw-rw-rw-   0        0        0     3726 2022-11-22 08:39:34.000000 neurospeed-2.1.7/neurospeed/utils/http_service.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:39:02.995849 neurospeed-2.1.7/neurospeed.egg-info/
+-rw-rw-rw-   0        0        0     1040 2023-05-09 15:39:02.000000 neurospeed-2.1.7/neurospeed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2137 2023-05-09 15:39:02.000000 neurospeed-2.1.7/neurospeed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 15:39:02.000000 neurospeed-2.1.7/neurospeed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-05-09 15:39:02.000000 neurospeed-2.1.7/neurospeed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 15:39:02.000000 neurospeed-2.1.7/neurospeed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 15:39:03.015618 neurospeed-2.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      821 2023-05-09 15:38:07.000000 neurospeed-2.1.7/setup.py
```

### Comparing `neurospeed-2.1.6/.gitignore` & `neurospeed-2.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/CHANGES.txt` & `neurospeed-2.1.7/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/LICENSE.txt` & `neurospeed-2.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/PKG-INFO` & `neurospeed-2.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurospeed
-Version: 2.1.6
+Version: 2.1.7
 Summary: NeuroSpeed Python API
 Home-page: https://bitbucket.org/neurobrave/neurospeed_python_api
 Author: NeuroBrave
 License: LICENSE.txt
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `neurospeed-2.1.6/README.md` & `neurospeed-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/README.txt` & `neurospeed-2.1.7/README.txt`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/examples/brainwave_to_midi.py` & `neurospeed-2.1.7/examples/brainwave_to_midi.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/examples/cognitive_effort_index.py` & `neurospeed-2.1.7/examples/cognitive_effort_index.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/examples/customer_api_flow_example_main.py` & `neurospeed-2.1.7/examples/customer_api_flow_example_main.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/examples/downlink_receive_to_HIA_example.py` & `neurospeed-2.1.7/examples/downlink_receive_to_HIA_example.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/examples/downlink_send_to_HIA_example.py` & `neurospeed-2.1.7/examples/downlink_send_to_HIA_example.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/examples/export_recorded_user_data_example_main.py` & `neurospeed-2.1.7/examples/export_recorded_user_data_example_main.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/examples/fatigue_notifier_whatsapp_example.py` & `neurospeed-2.1.7/examples/fatigue_notifier_whatsapp_example.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/examples/plot_engagement_index.py` & `neurospeed-2.1.7/examples/plot_engagement_index.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/examples/plot_raw_data_example.py` & `neurospeed-2.1.7/examples/plot_raw_data_example.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/examples/query_connections_example_main.py` & `neurospeed-2.1.7/examples/query_connections_example_main.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/examples/record_raw_data.py` & `neurospeed-2.1.7/examples/record_raw_data.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/examples/record_user_data_example_main.py` & `neurospeed-2.1.7/examples/record_user_data_example_main.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/examples/user_api_flow_example_main.py` & `neurospeed-2.1.7/examples/user_api_flow_example_main.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/images/logo.PNG` & `neurospeed-2.1.7/images/logo.PNG`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/neurospeed/api_http_handlers/exporter_http_handler.py` & `neurospeed-2.1.7/neurospeed/api_http_handlers/exporter_http_handler.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/neurospeed/api_http_handlers/gateway_http_handler.py` & `neurospeed-2.1.7/neurospeed/api_http_handlers/gateway_http_handler.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/neurospeed/api_http_handlers/recorder_http_handler.py` & `neurospeed-2.1.7/neurospeed/api_http_handlers/recorder_http_handler.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/neurospeed/api_http_handlers/ssr_http_handler.py` & `neurospeed-2.1.7/neurospeed/api_http_handlers/ssr_http_handler.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/neurospeed/api_socket_handlers/customer_room_handler.py` & `neurospeed-2.1.7/neurospeed/api_socket_handlers/customer_room_handler.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/neurospeed/api_socket_handlers/downlink_room_as_customer_handler.py` & `neurospeed-2.1.7/neurospeed/api_socket_handlers/downlink_room_as_customer_handler.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/neurospeed/api_socket_handlers/downlink_room_as_user_handler.py` & `neurospeed-2.1.7/neurospeed/api_socket_handlers/downlink_room_as_user_handler.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/neurospeed/api_socket_handlers/user_room_as_customer_handler.py` & `neurospeed-2.1.7/neurospeed/api_socket_handlers/user_room_as_customer_handler.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/neurospeed/api_socket_handlers/user_room_as_user_handler.py` & `neurospeed-2.1.7/neurospeed/api_socket_handlers/user_room_as_user_handler.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/neurospeed/auth/auth_as_customer_handler.py` & `neurospeed-2.1.7/neurospeed/auth/auth_as_customer_handler.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/neurospeed/auth/auth_as_user_handler.py` & `neurospeed-2.1.7/neurospeed/auth/auth_as_user_handler.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/neurospeed/hia_user_data/neurobrave_sensor_interface.py` & `neurospeed-2.1.7/neurospeed/hia_user_data/neurobrave_sensor_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,47 +61,52 @@
         
     def send_data(self, data, stream_id):  
         data.append(time.time()) # append timestamp to the end of sample array
  
         # insert data into the stream queue for that stream_id   
         self._streams_dict[stream_id].put(data, timeout = 1)      
 
-    def send_data_direct(self,data_packet,stream_id,timestamp=None, send_without_timestamp = False):
+    def send_data_direct(self,data_packet,stream_id,timestamp=None, send_without_timestamp = False, device_type = None):
         '''
         data packet is type list of multichannel samples, each miltichannel sample is also type list 
         optionally accepts timestamp - must be list with same length as data_packet
         '''
         if self._connection_status:
             data_to_send = []
             # print(data_packet)
             # print(f"received data to transmit type {type(data_packet)}, length {len(data_packet)}")
             if send_without_timestamp:
                 data_to_send = data_packet
             elif timestamp is None:       
-                t = time.time() - 10000000
+                t = time.time()
                 for sample in data_packet:
                     x = sample.copy()
                     x.append(t)
                     data_to_send.append(x)       
             else:
                 for index, sample in enumerate(data_packet):
                     x = sample.copy()
                     x.append(timestamp[index])
                     data_to_send.append(x)
             # print(f"transmitting data type {type(data_to_send)}, length {len(data_to_send)}")
                     
             TX_buffer = {"sample": data_to_send}
-
-            packet_payload = {"stream_id": stream_id, "device_type": self._device_type, "hia_id": self._hia_id, "data": json.dumps(TX_buffer)}                
+            # if device_type is None:
+            #     dev_type = self._device_type
+            # else:
+            #     dev_type= device_type
+            dev_type = self._sensor_info[stream_id]["device_type"]
+            
+            packet_payload = {"stream_id": stream_id, "device_type": dev_type, "hia_id": self._hia_id, "data": json.dumps(TX_buffer)}                
             packet_payload["experiment"] = {
                             "packet_labels": self._current_experiment_labels,
                             "onetime_labels": self._current_experiment_onetime_labels
-                        } 
-            print(len(str(json.dumps(TX_buffer))))
-            
+                            } 
+                
+            #print(len(str(json.dumps(TX_buffer))))
             self._sio.emit(self._packet_endpoint, packet_payload)      
         
         else:
             message = "{} Socket disconnected, stopping user_data upstream for stream_id: {}".format(self._contex, stream_id)
             print(message)
             return
```

### Comparing `neurospeed-2.1.6/neurospeed/utils/api_config_service.py` & `neurospeed-2.1.7/neurospeed/utils/api_config_service.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/neurospeed/utils/http_service.py` & `neurospeed-2.1.7/neurospeed/utils/http_service.py`

 * *Files identical despite different names*

### Comparing `neurospeed-2.1.6/neurospeed.egg-info/PKG-INFO` & `neurospeed-2.1.7/neurospeed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurospeed
-Version: 2.1.6
+Version: 2.1.7
 Summary: NeuroSpeed Python API
 Home-page: https://bitbucket.org/neurobrave/neurospeed_python_api
 Author: NeuroBrave
 License: LICENSE.txt
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `neurospeed-2.1.6/neurospeed.egg-info/SOURCES.txt` & `neurospeed-2.1.7/neurospeed.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 examples/brainwave_to_midi.py
 examples/cognitive_effort_index.py
 examples/customer_api_flow_example_main.py
 examples/downlink_receive_to_HIA_example.py
 examples/downlink_send_to_HIA_example.py
 examples/export_recorded_user_data_example_main.py
 examples/fatigue_notifier_whatsapp_example.py
-examples/hia_user_data_sender_example_main.py
 examples/plot_engagement_index.py
 examples/plot_raw_data_example.py
+examples/pywhatkit_dbs.txt
 examples/query_connections_example_main.py
 examples/record_raw_data.py
 examples/record_user_data_example_main.py
+examples/simple_get_data_packet.py
 examples/user_api_flow_example_main.py
 examples/config/api_config.json
 examples/config/customer_config.json
 examples/config/hia_config1.json
 examples/config/hia_config2.json
 images/logo.PNG
 neurospeed/__init__.py
@@ -46,11 +47,13 @@
 neurospeed/auth/auth_as_user_handler.py
 neurospeed/config/api_config.json
 neurospeed/config/customer_config.json
 neurospeed/config/hia_config1.json
 neurospeed/config/hia_config2.json
 neurospeed/hia_user_data/__init__.py
 neurospeed/hia_user_data/neurobrave_sensor_interface.py
+neurospeed/macros/__init__.py
+neurospeed/macros/macros.py
 neurospeed/utils/__init__.py
 neurospeed/utils/api_config_service.py
 neurospeed/utils/helper_service.py
 neurospeed/utils/http_service.py
```

### Comparing `neurospeed-2.1.6/setup.py` & `neurospeed-2.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
    name='neurospeed',
-   version='2.1.6',
+   version='2.1.7',
    author='NeuroBrave',
    contact_email='oleg@neurobrave.com',
    long_description = long_description,
    long_description_content_type="text/markdown",
    packages=find_packages(),
    scripts=[],
    package_data={'neurospeed': ['config/*']},
```

