# Comparing `tmp/DXR-1.8.6.tar.gz` & `tmp/DXR-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DXR-1.8.6.tar", last modified: Tue May  9 02:03:11 2023, max compression
+gzip compressed data, was "DXR-1.8.7.tar", last modified: Tue May  9 05:18:40 2023, max compression
```

## Comparing `DXR-1.8.6.tar` & `DXR-1.8.7.tar`

### file list

```diff
@@ -1,81 +1,84 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 02:03:11.981649 DXR-1.8.6/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 02:03:11.882645 DXR-1.8.6/DXR.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-05-09 02:03:11.000000 DXR-1.8.6/DXR.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1443 2023-05-09 02:03:11.000000 DXR-1.8.6/DXR.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-09 02:03:11.000000 DXR-1.8.6/DXR.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       40 2023-05-09 02:03:11.000000 DXR-1.8.6/DXR.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-05-09 02:03:11.000000 DXR-1.8.6/DXR.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      122 2023-05-09 02:03:11.000000 DXR-1.8.6/DXR.egg-info/top_level.txt
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 02:03:11.884482 DXR-1.8.6/Dxr_Chat/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7881 2023-05-08 11:48:13.000000 DXR-1.8.6/Dxr_Chat/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.8.6/Dxr_Chat/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.8.6/Dxr_Chat/utils.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 02:03:11.888854 DXR-1.8.6/Dxr_bytes/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.8.6/Dxr_bytes/Dxr_bytes.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_bytes/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 02:03:11.892390 DXR-1.8.6/Dxr_file/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.8.6/Dxr_file/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.8.6/Dxr_file/dxr_file.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2859 2023-05-09 02:03:01.000000 DXR-1.8.6/Dxr_file/dxr_request.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2427 2023-04-28 02:39:04.000000 DXR-1.8.6/Dxr_file/dxr_request_ros.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3427 2023-04-24 05:40:55.000000 DXR-1.8.6/Dxr_file/dxr_requests.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.8.6/Dxr_file/dxr_ssh.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 02:03:11.920412 DXR-1.8.6/Dxr_grpc/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.8.6/Dxr_grpc/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.8.6/Dxr_grpc/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.8.6/Dxr_grpc/audios_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.8.6/Dxr_grpc/audios_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.8.6/Dxr_grpc/dxr_grpc_audio_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.8.6/Dxr_grpc/dxr_grpc_audio_server.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.8.6/Dxr_grpc/dxr_grpc_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.8.6/Dxr_grpc/dxr_grpc_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 02:03:11.926245 DXR-1.8.6/Dxr_isapi/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.8.6/Dxr_isapi/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    29134 2023-05-08 05:52:49.000000 DXR-1.8.6/Dxr_isapi/api.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.8.6/Dxr_isapi/constants.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.8.6/Dxr_isapi/error.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.8.6/Dxr_isapi/ir_client.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 02:03:11.929891 DXR-1.8.6/Dxr_log/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_log/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_log/log.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 02:03:11.935618 DXR-1.8.6/Dxr_mqtt/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_mqtt/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_mqtt/dxr_log.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    14253 2023-04-14 07:14:34.000000 DXR-1.8.6/Dxr_mqtt/dxr_mqtt.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_mqtt/dxr_mqtt_2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.8.6/Dxr_mqtt/msg.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 02:03:11.938737 DXR-1.8.6/Dxr_serial/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.8.6/Dxr_serial/Dxr_serial.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_serial/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 02:03:11.947132 DXR-1.8.6/Dxr_utils/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_utils/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_utils/dxr_ftp.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_utils/dxr_utils.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_utils/gvalues.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 02:03:11.967271 DXR-1.8.6/Dxr_video/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_video/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_video/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_video/HCNetSDK.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_video/PlayCtrl.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_video/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_video/global_values.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_video/test_main.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_video/video.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_video/video_hk.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_video/video_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 02:03:11.969796 DXR-1.8.6/Dxr_voice/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.8.6/Dxr_voice/dxr_tts.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.8.6/Dxr_voice/dxr_whisper.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 02:03:11.971219 DXR-1.8.6/Dxr_yaml/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.8.6/Dxr_yaml/Dxr_yaml.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.8.6/Dxr_yaml/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-05-09 02:03:11.981228 DXR-1.8.6/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.8.6/README.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 02:03:11.980285 DXR-1.8.6/dxr_cli/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7902 2023-05-08 16:46:33.000000 DXR-1.8.6/dxr_cli/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-24 09:19:18.000000 DXR-1.8.6/dxr_cli/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7478 2023-05-08 23:55:40.000000 DXR-1.8.6/dxr_cli/cli.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8176 2023-05-08 23:51:46.000000 DXR-1.8.6/dxr_cli/code_execution.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-04 13:36:41.000000 DXR-1.8.6/dxr_cli/utils.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-09 02:03:11.981833 DXR-1.8.6/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      675 2023-05-09 02:03:08.000000 DXR-1.8.6/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 05:18:40.336014 DXR-1.8.7/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 05:18:40.210655 DXR-1.8.7/DXR.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-05-09 05:18:40.000000 DXR-1.8.7/DXR.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1491 2023-05-09 05:18:40.000000 DXR-1.8.7/DXR.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-09 05:18:40.000000 DXR-1.8.7/DXR.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       40 2023-05-09 05:18:40.000000 DXR-1.8.7/DXR.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-05-09 05:18:40.000000 DXR-1.8.7/DXR.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      132 2023-05-09 05:18:40.000000 DXR-1.8.7/DXR.egg-info/top_level.txt
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 05:18:40.213115 DXR-1.8.7/Dxr_Chat/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7881 2023-05-08 11:48:13.000000 DXR-1.8.7/Dxr_Chat/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.8.7/Dxr_Chat/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.8.7/Dxr_Chat/utils.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 05:18:40.217167 DXR-1.8.7/Dxr_bytes/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.8.7/Dxr_bytes/Dxr_bytes.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_bytes/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 05:18:40.225029 DXR-1.8.7/Dxr_file/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.8.7/Dxr_file/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.8.7/Dxr_file/dxr_file.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2859 2023-05-09 02:03:01.000000 DXR-1.8.7/Dxr_file/dxr_request.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2427 2023-04-28 02:39:04.000000 DXR-1.8.7/Dxr_file/dxr_request_ros.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3427 2023-04-24 05:40:55.000000 DXR-1.8.7/Dxr_file/dxr_requests.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.8.7/Dxr_file/dxr_ssh.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 05:18:40.235263 DXR-1.8.7/Dxr_grpc/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.8.7/Dxr_grpc/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.8.7/Dxr_grpc/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.8.7/Dxr_grpc/audios_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.8.7/Dxr_grpc/audios_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.8.7/Dxr_grpc/dxr_grpc_audio_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.8.7/Dxr_grpc/dxr_grpc_audio_server.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.8.7/Dxr_grpc/dxr_grpc_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.8.7/Dxr_grpc/dxr_grpc_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 05:18:40.243057 DXR-1.8.7/Dxr_isapi/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.8.7/Dxr_isapi/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    29134 2023-05-08 05:52:49.000000 DXR-1.8.7/Dxr_isapi/api.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.8.7/Dxr_isapi/constants.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.8.7/Dxr_isapi/error.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.8.7/Dxr_isapi/ir_client.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 05:18:40.245461 DXR-1.8.7/Dxr_log/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_log/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_log/log.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 05:18:40.251163 DXR-1.8.7/Dxr_mqtt/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_mqtt/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_mqtt/dxr_log.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    14253 2023-04-14 07:14:34.000000 DXR-1.8.7/Dxr_mqtt/dxr_mqtt.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_mqtt/dxr_mqtt_2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.8.7/Dxr_mqtt/msg.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 05:18:40.254948 DXR-1.8.7/Dxr_redis/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:36:17.000000 DXR-1.8.7/Dxr_redis/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4615 2023-05-09 04:48:00.000000 DXR-1.8.7/Dxr_redis/redis_client.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 05:18:40.263680 DXR-1.8.7/Dxr_serial/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.8.7/Dxr_serial/Dxr_serial.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_serial/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 05:18:40.278945 DXR-1.8.7/Dxr_utils/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_utils/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_utils/dxr_ftp.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_utils/dxr_utils.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_utils/gvalues.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 05:18:40.305827 DXR-1.8.7/Dxr_video/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_video/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_video/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_video/HCNetSDK.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_video/PlayCtrl.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_video/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_video/global_values.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_video/test_main.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_video/video.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_video/video_hk.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_video/video_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 05:18:40.308806 DXR-1.8.7/Dxr_voice/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.8.7/Dxr_voice/dxr_tts.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.8.7/Dxr_voice/dxr_whisper.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 05:18:40.311787 DXR-1.8.7/Dxr_yaml/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.8.7/Dxr_yaml/Dxr_yaml.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.8.7/Dxr_yaml/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-05-09 05:18:40.326758 DXR-1.8.7/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.8.7/README.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-09 05:18:40.324279 DXR-1.8.7/dxr_cli/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7902 2023-05-08 16:46:33.000000 DXR-1.8.7/dxr_cli/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-24 09:19:18.000000 DXR-1.8.7/dxr_cli/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    10106 2023-05-09 05:17:00.000000 DXR-1.8.7/dxr_cli/cli.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8176 2023-05-08 23:51:46.000000 DXR-1.8.7/dxr_cli/code_execution.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-04 13:36:41.000000 DXR-1.8.7/dxr_cli/utils.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-09 05:18:40.336265 DXR-1.8.7/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      688 2023-05-09 05:18:35.000000 DXR-1.8.7/setup.py
```

### Comparing `DXR-1.8.6/DXR.egg-info/SOURCES.txt` & `DXR-1.8.7/DXR.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 Dxr_log/__init__.py
 Dxr_log/log.py
 Dxr_mqtt/__init__.py
 Dxr_mqtt/dxr_log.py
 Dxr_mqtt/dxr_mqtt.py
 Dxr_mqtt/dxr_mqtt_2.py
 Dxr_mqtt/msg.py
+Dxr_redis/__init__.py
+Dxr_redis/redis_client.py
 Dxr_serial/Dxr_serial.py
 Dxr_serial/__init__.py
 Dxr_utils/__init__.py
 Dxr_utils/dxr_ftp.py
 Dxr_utils/dxr_utils.py
 Dxr_utils/gvalues.py
 Dxr_video/Datas_pb2.py
```

### Comparing `DXR-1.8.6/Dxr_Chat/ChatGPT.py` & `DXR-1.8.7/Dxr_Chat/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_Chat/utils.py` & `DXR-1.8.7/Dxr_Chat/utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_bytes/Dxr_bytes.py` & `DXR-1.8.7/Dxr_bytes/Dxr_bytes.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_file/dxr_file.py` & `DXR-1.8.7/Dxr_file/dxr_file.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_file/dxr_request.py` & `DXR-1.8.7/Dxr_file/dxr_request.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_file/dxr_request_ros.py` & `DXR-1.8.7/Dxr_file/dxr_request_ros.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_file/dxr_requests.py` & `DXR-1.8.7/Dxr_file/dxr_requests.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_file/dxr_ssh.py` & `DXR-1.8.7/Dxr_file/dxr_ssh.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_grpc/Datas_pb2.py` & `DXR-1.8.7/Dxr_grpc/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_grpc/Datas_pb2_grpc.py` & `DXR-1.8.7/Dxr_grpc/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_grpc/audios_pb2.py` & `DXR-1.8.7/Dxr_grpc/audios_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_grpc/audios_pb2_grpc.py` & `DXR-1.8.7/Dxr_grpc/audios_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_grpc/dxr_grpc_audio_client.py` & `DXR-1.8.7/Dxr_grpc/dxr_grpc_audio_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_grpc/dxr_grpc_audio_server.py` & `DXR-1.8.7/Dxr_grpc/dxr_grpc_audio_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_grpc/dxr_grpc_client.py` & `DXR-1.8.7/Dxr_grpc/dxr_grpc_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_grpc/dxr_grpc_server.py` & `DXR-1.8.7/Dxr_grpc/dxr_grpc_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_isapi/api.py` & `DXR-1.8.7/Dxr_isapi/api.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_isapi/error.py` & `DXR-1.8.7/Dxr_isapi/error.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_isapi/ir_client.py` & `DXR-1.8.7/Dxr_isapi/ir_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_log/log.py` & `DXR-1.8.7/Dxr_log/log.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_mqtt/dxr_mqtt.py` & `DXR-1.8.7/Dxr_mqtt/dxr_mqtt.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_mqtt/dxr_mqtt_2.py` & `DXR-1.8.7/Dxr_mqtt/dxr_mqtt_2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_mqtt/msg.py` & `DXR-1.8.7/Dxr_mqtt/msg.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_serial/Dxr_serial.py` & `DXR-1.8.7/Dxr_serial/Dxr_serial.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_utils/dxr_ftp.py` & `DXR-1.8.7/Dxr_utils/dxr_ftp.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_utils/dxr_utils.py` & `DXR-1.8.7/Dxr_utils/dxr_utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_video/Datas_pb2.py` & `DXR-1.8.7/Dxr_video/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_video/Datas_pb2_grpc.py` & `DXR-1.8.7/Dxr_video/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_video/HCNetSDK.py` & `DXR-1.8.7/Dxr_video/HCNetSDK.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_video/PlayCtrl.py` & `DXR-1.8.7/Dxr_video/PlayCtrl.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_video/test_main.py` & `DXR-1.8.7/Dxr_video/test_main.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_video/video.py` & `DXR-1.8.7/Dxr_video/video.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_video/video_hk.py` & `DXR-1.8.7/Dxr_video/video_hk.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_video/video_server.py` & `DXR-1.8.7/Dxr_video/video_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_voice/dxr_tts.py` & `DXR-1.8.7/Dxr_voice/dxr_tts.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/Dxr_yaml/Dxr_yaml.py` & `DXR-1.8.7/Dxr_yaml/Dxr_yaml.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/README.md` & `DXR-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/dxr_cli/ChatGPT.py` & `DXR-1.8.7/dxr_cli/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/dxr_cli/cli.py` & `DXR-1.8.7/dxr_cli/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import subprocess
 import click
 
 import requests
 from .ChatGPT import Chatbot
 import os
 import sys
 from rich.live import Live
@@ -68,15 +69,15 @@
             return None, step - 1
         elif key == '\x1b[C':
             return scripts[script_index], step + 1
             
 
 @dxr.command()
 def bash():
-    """Bash scripts"""
+    """执行云端上的脚本"""
     import os
     # scripts = get_bash_scripts()
     # script = choose_script(scripts)
     # sub_scripts = get_bash_script_dir(script)
     # sub_script = choose_script(sub_scripts)
     # bash_script = get_bash_script(script, sub_script)
     # print("=" * 80)
@@ -136,15 +137,15 @@
                 live.update(md, refresh=True)
                 
 
 @click.command()
 @click.option("--model", default="gpt-3.5-turbo", help="Specify which GPT model to use")
 @click.option("--maxtoken", default=4096, help="Maximum number of tokens in a single prompt")
 def git(model, maxtoken):
-    """Git scripts"""
+    """问问关于git的问题"""
     print("这是一个git命令行助手,你可以通过这个助手来学习git命令")
     # use openai to generate git scripts
     base_url, api_key = get_api_key()
     bot = Chatbot(api_key=api_key, base_url=base_url, system_prompt="""
     你是一个很好的git命令行助手，你可以帮助我更好的使用git, 
     根据我的问题,你可以给我提供一些git命令
     """, engine=model, max_tokens=maxtoken)
@@ -208,14 +209,79 @@
     md = Markdown("")
     with Live(md, auto_refresh=True) as live:
         tmp = ""
         for r in res:
             tmp += r
             md = Markdown(tmp)
             live.update(md, refresh=True)
+            
+            
+            
+@click.command()
+@click.argument('args', nargs=-1)
+@click.option("--model", default="gpt-3.5-turbo", help="Specify which GPT model to use")
+@click.option("--maxtoken", default=4096, help="Maximum number of tokens in a single prompt")
+@click.option("--lines", default=100, help="Number of lines before and after the error to capture as context")
+def run(args, model, maxtoken, lines):
+    """
+    接收不固定参数的命令，并执行它们。如果发生错误，将捕获并显示错误输出及其上下文。
+    """
+    try:
+        language = get_language(args)
+        # 将参数元组转换为列表，并将其传递给subprocess.run函数
+        result = subprocess.run(
+            list(args), stderr=subprocess.PIPE, stdout=subprocess.PIPE, text=True, check=True
+        )
+    except subprocess.CalledProcessError as e:
+        # 找出可能涉及的文件
+        source_files = [arg for arg in args if os.path.isfile(arg)]
+        file_contents = []
+
+        for file in source_files:
+            # 检查文件字数是否超过2000
+            num_chars = os.stat(file).st_size
+            if num_chars <= 2000:
+                with open(file, 'r', encoding='utf-8') as f:
+                    content = f.read()
+            else:
+                # 取前后各100行的代码
+                with open(file, 'r', encoding='utf-8') as f:
+                    head_lines = [next(f) for _ in range(lines)]
+                with open(file, 'r', encoding='utf-8') as f:
+                    tail_lines = f.readlines()[-lines:]
+
+                content = "".join(head_lines) + "\n...\n" + "".join(tail_lines)
+
+            file_contents.append(content)
+
+        # 获取错误输出
+        error_output = e.stderr
+        
+        # 打印错误输出
+        click.echo(error_output)
+
+        # 将文件内容与错误输出合并
+        total_input = f"Error Output:\n{error_output}\n\n"
+        for i, content in enumerate(file_contents):
+            total_input += f"File Content ({source_files[i]}):\n{content}\n\n"
+
+        # 使用GPT模型处理整个输入
+        with LoadingMessage():
+            response = chatgpt_explanation(language, total_input, model, maxtoken)
+
+        # 使用Rich库将结果显示为Markdown
+        md = Markdown("")
+        with Live(md, auto_refresh=True) as live:
+            tmp = ""
+            for r in response:
+                tmp += r
+                md = Markdown(tmp)
+                live.update(md, refresh=True)
+    else:
+        click.echo(result.stdout)
     
         
     
     
 
      
     
@@ -226,10 +292,11 @@
 
 dxr.add_command(hello)
 dxr.add_command(bash)
 dxr.add_command(chat)
 dxr.add_command(git)
 dxr.add_command(python)
 dxr.add_command(python3)
+dxr.add_command(run)
 
 if __name__ == '__main__':
     dxr()
```

### Comparing `DXR-1.8.6/dxr_cli/code_execution.py` & `DXR-1.8.7/dxr_cli/code_execution.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/dxr_cli/utils.py` & `DXR-1.8.7/dxr_cli/utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.6/setup.py` & `DXR-1.8.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='DXR',
-    version='1.8.6',
-    packages=['Dxr_mqtt', 'Dxr_log', 'Dxr_bytes', 'Dxr_utils', 'Dxr_video', 'Dxr_serial', 'Dxr_yaml', 'Dxr_file', 'Dxr_grpc', 'Dxr_isapi', 'Dxr_voice', 'Dxr_Chat', 'dxr_cli'],
+    version='1.8.7',
+    packages=['Dxr_mqtt', 'Dxr_log', 'Dxr_bytes', 'Dxr_utils', 'Dxr_video', 'Dxr_serial', 'Dxr_yaml', 'Dxr_file', 'Dxr_grpc', 'Dxr_isapi', 'Dxr_voice', 'Dxr_Chat', 'Dxr_redis', 'dxr_cli'],
     install_requires=['paho-mqtt', 'pyyaml', 'pyserial', 'loguru','tabulate', 'pymysql', 'sqlalchemy', 'oss2', 'imagezmq', 'simplejpeg', 'pexpect', 'aiortsp'],
     author='luzhipeng',
     author_email='402087139@qq.com',
     license='MIT',
     url='http://pycn.me',
     description='DXR is a python library for DXR_mqtt',
     entry_points={
```

