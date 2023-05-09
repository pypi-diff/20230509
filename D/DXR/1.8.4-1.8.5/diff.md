# Comparing `tmp/DXR-1.8.4.tar.gz` & `tmp/DXR-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DXR-1.8.4.tar", last modified: Fri May  5 09:46:47 2023, max compression
+gzip compressed data, was "DXR-1.8.5.tar", last modified: Mon May  8 23:55:53 2023, max compression
```

## Comparing `DXR-1.8.4.tar` & `DXR-1.8.5.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-05 09:46:47.982684 DXR-1.8.4/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-05 09:46:47.897806 DXR-1.8.4/DXR.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-05-05 09:46:47.000000 DXR-1.8.4/DXR.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1417 2023-05-05 09:46:47.000000 DXR-1.8.4/DXR.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-05 09:46:47.000000 DXR-1.8.4/DXR.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       40 2023-05-05 09:46:47.000000 DXR-1.8.4/DXR.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-05-05 09:46:47.000000 DXR-1.8.4/DXR.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      122 2023-05-05 09:46:47.000000 DXR-1.8.4/DXR.egg-info/top_level.txt
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-05 09:46:47.900049 DXR-1.8.4/Dxr_Chat/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7852 2023-05-05 09:46:26.000000 DXR-1.8.4/Dxr_Chat/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.8.4/Dxr_Chat/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.8.4/Dxr_Chat/utils.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-05 09:46:47.904338 DXR-1.8.4/Dxr_bytes/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.8.4/Dxr_bytes/Dxr_bytes.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_bytes/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-05 09:46:47.910549 DXR-1.8.4/Dxr_file/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.8.4/Dxr_file/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.8.4/Dxr_file/dxr_file.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3364 2023-04-24 05:32:08.000000 DXR-1.8.4/Dxr_file/dxr_request.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2427 2023-04-28 02:39:04.000000 DXR-1.8.4/Dxr_file/dxr_request_ros.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3427 2023-04-24 05:40:55.000000 DXR-1.8.4/Dxr_file/dxr_requests.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.8.4/Dxr_file/dxr_ssh.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-05 09:46:47.923016 DXR-1.8.4/Dxr_grpc/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.8.4/Dxr_grpc/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.8.4/Dxr_grpc/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.8.4/Dxr_grpc/audios_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.8.4/Dxr_grpc/audios_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.8.4/Dxr_grpc/dxr_grpc_audio_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.8.4/Dxr_grpc/dxr_grpc_audio_server.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.8.4/Dxr_grpc/dxr_grpc_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.8.4/Dxr_grpc/dxr_grpc_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-05 09:46:47.930699 DXR-1.8.4/Dxr_isapi/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.8.4/Dxr_isapi/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    29134 2023-04-25 05:13:27.000000 DXR-1.8.4/Dxr_isapi/api.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.8.4/Dxr_isapi/constants.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.8.4/Dxr_isapi/error.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.8.4/Dxr_isapi/ir_client.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-05 09:46:47.937221 DXR-1.8.4/Dxr_log/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_log/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_log/log.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-05 09:46:47.944353 DXR-1.8.4/Dxr_mqtt/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_mqtt/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_mqtt/dxr_log.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    14253 2023-04-14 07:14:34.000000 DXR-1.8.4/Dxr_mqtt/dxr_mqtt.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_mqtt/dxr_mqtt_2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.8.4/Dxr_mqtt/msg.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-05 09:46:47.947227 DXR-1.8.4/Dxr_serial/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.8.4/Dxr_serial/Dxr_serial.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_serial/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-05 09:46:47.952118 DXR-1.8.4/Dxr_utils/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_utils/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_utils/dxr_ftp.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_utils/dxr_utils.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_utils/gvalues.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-05 09:46:47.967813 DXR-1.8.4/Dxr_video/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_video/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_video/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_video/HCNetSDK.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_video/PlayCtrl.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_video/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_video/global_values.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_video/test_main.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_video/video.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_video/video_hk.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_video/video_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-05 09:46:47.971546 DXR-1.8.4/Dxr_voice/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.8.4/Dxr_voice/dxr_tts.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.8.4/Dxr_voice/dxr_whisper.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-05 09:46:47.974574 DXR-1.8.4/Dxr_yaml/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.8.4/Dxr_yaml/Dxr_yaml.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.8.4/Dxr_yaml/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-05-05 09:46:47.982165 DXR-1.8.4/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.8.4/README.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-05 09:46:47.981037 DXR-1.8.4/dxr_cli/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7933 2023-05-05 08:48:13.000000 DXR-1.8.4/dxr_cli/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-24 09:19:18.000000 DXR-1.8.4/dxr_cli/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     5079 2023-05-05 08:44:03.000000 DXR-1.8.4/dxr_cli/cli.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-04 13:36:41.000000 DXR-1.8.4/dxr_cli/utils.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-05 09:46:47.982945 DXR-1.8.4/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      675 2023-05-05 09:46:41.000000 DXR-1.8.4/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-08 23:55:53.249339 DXR-1.8.5/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-08 23:55:53.178772 DXR-1.8.5/DXR.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-05-08 23:55:53.000000 DXR-1.8.5/DXR.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1443 2023-05-08 23:55:53.000000 DXR-1.8.5/DXR.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-08 23:55:53.000000 DXR-1.8.5/DXR.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       40 2023-05-08 23:55:53.000000 DXR-1.8.5/DXR.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-05-08 23:55:53.000000 DXR-1.8.5/DXR.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      122 2023-05-08 23:55:53.000000 DXR-1.8.5/DXR.egg-info/top_level.txt
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-08 23:55:53.180824 DXR-1.8.5/Dxr_Chat/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7881 2023-05-08 11:48:13.000000 DXR-1.8.5/Dxr_Chat/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.8.5/Dxr_Chat/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.8.5/Dxr_Chat/utils.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-08 23:55:53.183744 DXR-1.8.5/Dxr_bytes/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.8.5/Dxr_bytes/Dxr_bytes.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_bytes/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-08 23:55:53.188930 DXR-1.8.5/Dxr_file/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.8.5/Dxr_file/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.8.5/Dxr_file/dxr_file.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3364 2023-05-08 06:51:48.000000 DXR-1.8.5/Dxr_file/dxr_request.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2427 2023-04-28 02:39:04.000000 DXR-1.8.5/Dxr_file/dxr_request_ros.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3427 2023-04-24 05:40:55.000000 DXR-1.8.5/Dxr_file/dxr_requests.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.8.5/Dxr_file/dxr_ssh.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-08 23:55:53.198987 DXR-1.8.5/Dxr_grpc/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.8.5/Dxr_grpc/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.8.5/Dxr_grpc/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.8.5/Dxr_grpc/audios_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.8.5/Dxr_grpc/audios_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.8.5/Dxr_grpc/dxr_grpc_audio_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.8.5/Dxr_grpc/dxr_grpc_audio_server.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.8.5/Dxr_grpc/dxr_grpc_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.8.5/Dxr_grpc/dxr_grpc_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-08 23:55:53.203556 DXR-1.8.5/Dxr_isapi/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.8.5/Dxr_isapi/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    29134 2023-05-08 05:52:49.000000 DXR-1.8.5/Dxr_isapi/api.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.8.5/Dxr_isapi/constants.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.8.5/Dxr_isapi/error.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.8.5/Dxr_isapi/ir_client.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-08 23:55:53.205872 DXR-1.8.5/Dxr_log/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_log/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_log/log.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-08 23:55:53.213142 DXR-1.8.5/Dxr_mqtt/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_mqtt/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_mqtt/dxr_log.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    14253 2023-04-14 07:14:34.000000 DXR-1.8.5/Dxr_mqtt/dxr_mqtt.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_mqtt/dxr_mqtt_2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.8.5/Dxr_mqtt/msg.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-08 23:55:53.216228 DXR-1.8.5/Dxr_serial/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.8.5/Dxr_serial/Dxr_serial.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_serial/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-08 23:55:53.221320 DXR-1.8.5/Dxr_utils/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_utils/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_utils/dxr_ftp.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_utils/dxr_utils.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_utils/gvalues.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-08 23:55:53.235705 DXR-1.8.5/Dxr_video/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_video/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_video/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_video/HCNetSDK.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_video/PlayCtrl.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_video/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_video/global_values.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_video/test_main.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_video/video.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_video/video_hk.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_video/video_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-08 23:55:53.238405 DXR-1.8.5/Dxr_voice/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.8.5/Dxr_voice/dxr_tts.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.8.5/Dxr_voice/dxr_whisper.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-08 23:55:53.240136 DXR-1.8.5/Dxr_yaml/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.8.5/Dxr_yaml/Dxr_yaml.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.8.5/Dxr_yaml/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-05-08 23:55:53.248875 DXR-1.8.5/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.8.5/README.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-08 23:55:53.246449 DXR-1.8.5/dxr_cli/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7902 2023-05-08 16:46:33.000000 DXR-1.8.5/dxr_cli/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-24 09:19:18.000000 DXR-1.8.5/dxr_cli/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7478 2023-05-08 23:55:40.000000 DXR-1.8.5/dxr_cli/cli.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8176 2023-05-08 23:51:46.000000 DXR-1.8.5/dxr_cli/code_execution.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-04 13:36:41.000000 DXR-1.8.5/dxr_cli/utils.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-08 23:55:53.250625 DXR-1.8.5/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      675 2023-05-08 23:55:47.000000 DXR-1.8.5/setup.py
```

### Comparing `DXR-1.8.4/DXR.egg-info/SOURCES.txt` & `DXR-1.8.5/DXR.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -56,8 +56,9 @@
 Dxr_voice/dxr_tts.py
 Dxr_voice/dxr_whisper.py
 Dxr_yaml/Dxr_yaml.py
 Dxr_yaml/__init__.py
 dxr_cli/ChatGPT.py
 dxr_cli/__init__.py
 dxr_cli/cli.py
+dxr_cli/code_execution.py
 dxr_cli/utils.py
```

### Comparing `DXR-1.8.4/Dxr_Chat/ChatGPT.py` & `DXR-1.8.5/dxr_cli/ChatGPT.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     """
     Official ChatGPT API
     """
 
     def __init__(
         self,
         api_key: str,
+        base_url: str = None,
         engine: str = None,
         proxy: str = None,
         max_tokens: int = 4095,
         temperature: float = 0.5,
         top_p: float = 1.0,
         reply_count: int = 1,
         system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
@@ -37,15 +38,16 @@
         """
         Initialize Chatbot with API key (from https://platform.openai.com/account/api-keys)
         """
         self.engine = engine or ENGINE
         self.session = requests.Session()
         self.api_key = api_key
         openai.api_key = self.api_key
-        openai.api_base = 'https://api.open-ai.repl.co/v1'
+        if base_url is not None:
+            openai.api_base = base_url + 'v1'
         self.proxy = proxy
         if self.proxy:
             proxies = {
                 "http": self.proxy,
                 "https": self.proxy,
             }
             self.session.proxies = proxies
```

### Comparing `DXR-1.8.4/Dxr_Chat/utils.py` & `DXR-1.8.5/Dxr_Chat/utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_bytes/Dxr_bytes.py` & `DXR-1.8.5/Dxr_bytes/Dxr_bytes.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_file/dxr_file.py` & `DXR-1.8.5/Dxr_file/dxr_file.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_file/dxr_request.py` & `DXR-1.8.5/Dxr_file/dxr_request.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_file/dxr_request_ros.py` & `DXR-1.8.5/Dxr_file/dxr_request_ros.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_file/dxr_requests.py` & `DXR-1.8.5/Dxr_file/dxr_requests.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_file/dxr_ssh.py` & `DXR-1.8.5/Dxr_file/dxr_ssh.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_grpc/Datas_pb2.py` & `DXR-1.8.5/Dxr_grpc/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_grpc/Datas_pb2_grpc.py` & `DXR-1.8.5/Dxr_grpc/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_grpc/audios_pb2.py` & `DXR-1.8.5/Dxr_grpc/audios_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_grpc/audios_pb2_grpc.py` & `DXR-1.8.5/Dxr_grpc/audios_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_grpc/dxr_grpc_audio_client.py` & `DXR-1.8.5/Dxr_grpc/dxr_grpc_audio_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_grpc/dxr_grpc_audio_server.py` & `DXR-1.8.5/Dxr_grpc/dxr_grpc_audio_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_grpc/dxr_grpc_client.py` & `DXR-1.8.5/Dxr_grpc/dxr_grpc_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_grpc/dxr_grpc_server.py` & `DXR-1.8.5/Dxr_grpc/dxr_grpc_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_isapi/api.py` & `DXR-1.8.5/Dxr_isapi/api.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_isapi/error.py` & `DXR-1.8.5/Dxr_isapi/error.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_isapi/ir_client.py` & `DXR-1.8.5/Dxr_isapi/ir_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_log/log.py` & `DXR-1.8.5/Dxr_log/log.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_mqtt/dxr_mqtt.py` & `DXR-1.8.5/Dxr_mqtt/dxr_mqtt.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_mqtt/dxr_mqtt_2.py` & `DXR-1.8.5/Dxr_mqtt/dxr_mqtt_2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_mqtt/msg.py` & `DXR-1.8.5/Dxr_mqtt/msg.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_serial/Dxr_serial.py` & `DXR-1.8.5/Dxr_serial/Dxr_serial.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_utils/dxr_ftp.py` & `DXR-1.8.5/Dxr_utils/dxr_ftp.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_utils/dxr_utils.py` & `DXR-1.8.5/Dxr_utils/dxr_utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_video/Datas_pb2.py` & `DXR-1.8.5/Dxr_video/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_video/Datas_pb2_grpc.py` & `DXR-1.8.5/Dxr_video/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_video/HCNetSDK.py` & `DXR-1.8.5/Dxr_video/HCNetSDK.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_video/PlayCtrl.py` & `DXR-1.8.5/Dxr_video/PlayCtrl.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_video/test_main.py` & `DXR-1.8.5/Dxr_video/test_main.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_video/video.py` & `DXR-1.8.5/Dxr_video/video.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_video/video_hk.py` & `DXR-1.8.5/Dxr_video/video_hk.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_video/video_server.py` & `DXR-1.8.5/Dxr_video/video_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_voice/dxr_tts.py` & `DXR-1.8.5/Dxr_voice/dxr_tts.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/Dxr_yaml/Dxr_yaml.py` & `DXR-1.8.5/Dxr_yaml/Dxr_yaml.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/README.md` & `DXR-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/dxr_cli/ChatGPT.py` & `DXR-1.8.5/Dxr_Chat/ChatGPT.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,33 +22,31 @@
     """
     Official ChatGPT API
     """
 
     def __init__(
         self,
         api_key: str,
-        base_url: str = None,
         engine: str = None,
         proxy: str = None,
         max_tokens: int = 4095,
         temperature: float = 0.5,
         top_p: float = 1.0,
         reply_count: int = 1,
         system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
+        base_url: str = "https://api.openai.com/v1",
     ) -> None:
         """
         Initialize Chatbot with API key (from https://platform.openai.com/account/api-keys)
         """
         self.engine = engine or ENGINE
         self.session = requests.Session()
         self.api_key = api_key
         openai.api_key = self.api_key
-        if base_url is not None:
-            openai.api_base = base_url + 'v1'
-        print(openai.api_base)
+        openai.api_base = base_url
         self.proxy = proxy
         if self.proxy:
             proxies = {
                 "http": self.proxy,
                 "https": self.proxy,
             }
             self.session.proxies = proxies
```

### Comparing `DXR-1.8.4/dxr_cli/utils.py` & `DXR-1.8.5/dxr_cli/utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.8.4/setup.py` & `DXR-1.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='DXR',
-    version='1.8.4',
+    version='1.8.5',
     packages=['Dxr_mqtt', 'Dxr_log', 'Dxr_bytes', 'Dxr_utils', 'Dxr_video', 'Dxr_serial', 'Dxr_yaml', 'Dxr_file', 'Dxr_grpc', 'Dxr_isapi', 'Dxr_voice', 'Dxr_Chat', 'dxr_cli'],
     install_requires=['paho-mqtt', 'pyyaml', 'pyserial', 'loguru','tabulate', 'pymysql', 'sqlalchemy', 'oss2', 'imagezmq', 'simplejpeg', 'pexpect', 'aiortsp'],
     author='luzhipeng',
     author_email='402087139@qq.com',
     license='MIT',
     url='http://pycn.me',
     description='DXR is a python library for DXR_mqtt',
```

