# Comparing `tmp/nanosurf-1.6.1.tar.gz` & `tmp/nanosurf-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanosurf-1.6.1.tar", last modified: Thu May  4 07:50:21 2023, max compression
+gzip compressed data, was "nanosurf-1.6.2.tar", last modified: Tue May  9 09:44:59 2023, max compression
```

## Comparing `nanosurf-1.6.1.tar` & `nanosurf-1.6.2.tar`

### file list

```diff
@@ -1,269 +1,269 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.501716 nanosurf-1.6.1/
--rw-rw-rw-   0        0        0     1067 2022-02-08 08:13:22.000000 nanosurf-1.6.1/LICENSE
--rw-rw-rw-   0        0        0     6686 2023-05-04 07:50:21.501716 nanosurf-1.6.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.313560 nanosurf-1.6.1/nanosurf/
--rw-rw-rw-   0        0        0     1774 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/__init__.py
--rw-rw-rw-   0        0        0       21 2023-05-04 07:46:30.000000 nanosurf-1.6.1/nanosurf/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.303562 nanosurf-1.6.1/nanosurf/app/
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.323562 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.323562 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/.vscode/
--rw-rw-rw-   0        0        0      566 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/.vscode/launch.json
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.334572 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/
--rw-rw-rw-   0        0        0     2294 2023-02-17 17:06:00.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_stm_addon.cpython-310.pyc
--rw-rw-rw-   0        0        0     2285 2023-04-14 11:38:45.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_stm_addon.cpython-39.pyc
--rw-rw-rw-   0        0        0     2364 2023-05-03 07:22:11.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_tip_current_addon.cpython-39.pyc
--rw-rw-rw-   0        0        0     1853 2023-02-17 16:53:51.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/gui.cpython-310.pyc
--rw-rw-rw-   0        0        0     1822 2023-05-03 07:22:11.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/gui.cpython-39.pyc
--rw-rw-rw-   0        0        0     1523 2023-02-17 17:00:32.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/settings.cpython-310.pyc
--rw-rw-rw-   0        0        0     1361 2023-05-03 07:22:11.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/settings.cpython-39.pyc
--rw-rw-rw-   0        0        0     3319 2023-02-17 17:12:09.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker.cpython-310.pyc
--rw-rw-rw-   0        0        0     3400 2023-05-03 07:22:11.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker.cpython-39.pyc
--rw-rw-rw-   0        0        0     2670 2023-02-16 15:52:16.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker_task.cpython-310.pyc
--rw-rw-rw-   0        0        0     2086 2023-05-03 07:19:15.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/device_tip_current_addon.py
--rw-rw-rw-   0        0        0     1843 2023-05-03 07:17:37.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/gui.py
--rw-rw-rw-   0        0        0      740 2023-05-03 07:16:24.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/main.py
--rw-rw-rw-   0        0        0      893 2023-05-03 07:17:37.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/settings.py
--rw-rw-rw-   0        0        0     4204 2023-05-03 07:20:07.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/worker.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.334572 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.334572 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/.vscode/
--rw-rw-rw-   0        0        0      566 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/.vscode/launch.json
--rw-rw-rw-   0        0        0     1462 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/main.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.344581 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/
--rw-rw-rw-   0        0        0        0 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.354580 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/
--rw-rw-rw-   0        0        0      195 2022-12-14 07:35:47.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      193 2022-09-19 09:03:09.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     9770 2023-03-09 15:52:53.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/gui.cpython-310.pyc
--rw-rw-rw-   0        0        0     9831 2023-04-14 09:26:40.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/gui.cpython-39.pyc
--rw-rw-rw-   0        0        0     5198 2023-03-09 15:52:53.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/imaging_task.cpython-310.pyc
--rw-rw-rw-   0        0        0     4006 2023-04-14 09:26:21.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/imaging_task.cpython-39.pyc
--rw-rw-rw-   0        0        0     5181 2023-02-03 08:34:04.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/module.cpython-310.pyc
--rw-rw-rw-   0        0        0     5236 2023-04-14 09:26:21.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     1930 2022-12-14 07:35:47.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/settings.cpython-310.pyc
--rw-rw-rw-   0        0        0     1768 2023-04-14 09:09:22.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/settings.cpython-39.pyc
--rw-rw-rw-   0        0        0    13848 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/gui.py
--rw-rw-rw-   0        0        0     4907 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/imaging_task.py
--rw-rw-rw-   0        0        0     5067 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/module.py
--rw-rw-rw-   0        0        0     1310 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.354580 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.354580 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/.vscode/
--rw-rw-rw-   0        0        0      566 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/.vscode/launch.json
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.354580 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/
--rw-rw-rw-   0        0        0        0 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.364580 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/
--rw-rw-rw-   0        0        0      194 2022-12-16 09:42:02.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      192 2022-09-16 14:32:05.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5443 2023-03-09 14:29:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_fit.cpython-310.pyc
--rw-rw-rw-   0        0        0     5291 2023-04-14 12:04:20.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_fit.cpython-39.pyc
--rw-rw-rw-   0        0        0     9703 2023-03-09 14:29:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_gui.cpython-310.pyc
--rw-rw-rw-   0        0        0     9667 2023-04-14 12:04:20.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_gui.cpython-39.pyc
--rw-rw-rw-   0        0        0     9829 2023-02-08 13:02:32.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_module.cpython-310.pyc
--rw-rw-rw-   0        0        0     9723 2023-04-14 12:06:14.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_module.cpython-39.pyc
--rw-rw-rw-   0        0        0     3005 2023-02-08 13:02:33.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_settings.cpython-310.pyc
--rw-rw-rw-   0        0        0     2991 2023-04-14 12:01:18.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_settings.cpython-39.pyc
--rw-rw-rw-   0        0        0     5067 2023-03-09 14:29:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_task.cpython-310.pyc
--rw-rw-rw-   0        0        0     3662 2023-04-14 12:04:20.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_task.cpython-39.pyc
--rw-rw-rw-   0        0        0     7030 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_fit.py
--rw-rw-rw-   0        0        0    13971 2023-05-03 08:56:03.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_gui.py
--rw-rw-rw-   0        0        0    10552 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_module.py
--rw-rw-rw-   0        0        0     2397 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_settings.py
--rw-rw-rw-   0        0        0     3943 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_task.py
--rw-rw-rw-   0        0        0     1580 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/main.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.364580 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.364580 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/.vscode/
--rw-rw-rw-   0        0        0      566 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/.vscode/launch.json
--rw-rw-rw-   0        0        0     1431 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/main.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.374582 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/
--rw-rw-rw-   0        0        0        0 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.384580 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/
--rw-rw-rw-   0        0        0      199 2022-12-16 13:29:49.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      197 2022-11-15 07:27:23.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     9252 2023-02-16 16:05:23.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/gui.cpython-310.pyc
--rw-rw-rw-   0        0        0     9276 2023-04-14 12:27:20.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/gui.cpython-39.pyc
--rw-rw-rw-   0        0        0     6662 2023-02-16 16:05:23.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/module.cpython-310.pyc
--rw-rw-rw-   0        0        0     6564 2023-04-14 12:24:00.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     2314 2023-01-25 08:22:47.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/settings.cpython-310.pyc
--rw-rw-rw-   0        0        0     2322 2023-04-14 12:24:00.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/settings.cpython-39.pyc
--rw-rw-rw-   0        0        0     4594 2023-03-13 14:19:52.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/worker_task.cpython-310.pyc
--rw-rw-rw-   0        0        0     3455 2023-04-14 12:24:00.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/worker_task.cpython-39.pyc
--rw-rw-rw-   0        0        0    13358 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/gui.py
--rw-rw-rw-   0        0        0     7055 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/module.py
--rw-rw-rw-   0        0        0     1949 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/settings.py
--rw-rw-rw-   0        0        0     4533 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/worker_task.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.384580 nanosurf-1.6.1/nanosurf/app/app_template/
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.384580 nanosurf-1.6.1/nanosurf/app/app_template/.vscode/
--rw-rw-rw-   0        0        0      566 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/app/app_template/.vscode/launch.json
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.384580 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/
--rw-rw-rw-   0        0        0        0 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.397103 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/
--rw-rw-rw-   0        0        0      176 2022-12-16 15:19:50.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      192 2023-01-25 09:01:50.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      174 2022-09-19 08:10:48.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     6384 2023-02-07 10:44:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-310.pyc
--rw-rw-rw-   0        0        0    13859 2023-01-25 09:01:50.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-311.pyc
--rw-rw-rw-   0        0        0     6336 2023-04-14 08:47:57.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-39.pyc
--rw-rw-rw-   0        0        0     5392 2023-02-09 07:59:12.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-310.pyc
--rw-rw-rw-   0        0        0     9403 2023-01-25 09:01:50.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0     5327 2023-04-14 08:43:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     1797 2022-12-16 15:19:50.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-310.pyc
--rw-rw-rw-   0        0        0     2652 2023-01-25 09:01:50.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-311.pyc
--rw-rw-rw-   0        0        0     1634 2023-04-14 08:43:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-39.pyc
--rw-rw-rw-   0        0        0     2896 2023-02-07 10:44:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-310.pyc
--rw-rw-rw-   0        0        0     5326 2023-01-25 09:01:50.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-311.pyc
--rw-rw-rw-   0        0        0     2570 2023-04-14 08:47:57.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-39.pyc
--rw-rw-rw-   0        0        0     7820 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/gui.py
--rw-rw-rw-   0        0        0     5134 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/module.py
--rw-rw-rw-   0        0        0     1160 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/settings.py
--rw-rw-rw-   0        0        0     2617 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/worker_task.py
--rw-rw-rw-   0        0        0     1673 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/main.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.397103 nanosurf-1.6.1/nanosurf/app/demo_creating_spec_pos_table_with_smiley/
--rw-rw-rw-   0        0        0     4446 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/app/demo_creating_spec_pos_table_with_smiley/spectroscopy_demo_creating_a_smiley.ipynb
--rw-rw-rw-   0        0        0     2457 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/demo_creating_spec_pos_table_with_smiley/spectroscopy_demo_creating_a_smiley.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.397103 nanosurf-1.6.1/nanosurf/app/demo_lateral_force_signal_calibration/
--rw-rw-rw-   0        0        0    54597 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/app/demo_lateral_force_signal_calibration/demo_lfm_calibration.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.397103 nanosurf-1.6.1/nanosurf/app/demo_move_sample_stage/
--rw-rw-rw-   0        0        0     7665 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/app/demo_move_sample_stage/demo_move_sample_stage.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.407112 nanosurf-1.6.1/nanosurf/app/demo_spec_setup_and_data_plotting/
--rw-rw-rw-   0        0        0   121398 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/app/demo_spec_setup_and_data_plotting/spec_demo.ipynb
--rw-rw-rw-   0        0        0     2294 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/app/demo_spec_setup_and_data_plotting/spec_demo.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.407112 nanosurf-1.6.1/nanosurf/app/demo_studio_scripting/
--rw-rw-rw-   0        0        0     4735 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/demo_studio_scripting/studio_demo_data_sampling.py
--rw-rw-rw-   0        0        0     1817 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/app/demo_studio_scripting/studio_scripting_demo.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.407112 nanosurf-1.6.1/nanosurf/app/spm_template/
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.407112 nanosurf-1.6.1/nanosurf/app/spm_template/.vscode/
--rw-rw-rw-   0        0        0      566 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/spm_template/.vscode/launch.json
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.417110 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/
--rw-rw-rw-   0        0        0     7537 2023-03-22 08:49:37.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/gui.cpython-310.pyc
--rw-rw-rw-   0        0        0     7506 2023-04-14 11:57:53.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/gui.cpython-39.pyc
--rw-rw-rw-   0        0        0     3307 2023-03-22 08:30:27.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/measure_task.cpython-310.pyc
--rw-rw-rw-   0        0        0     3320 2023-04-14 09:59:56.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/measure_task.cpython-39.pyc
--rw-rw-rw-   0        0        0     6030 2023-03-22 08:48:33.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/module.cpython-310.pyc
--rw-rw-rw-   0        0        0     5992 2023-04-14 12:53:50.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     1702 2023-03-22 08:30:27.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/settings.cpython-310.pyc
--rw-rw-rw-   0        0        0     1690 2023-04-14 09:52:09.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/settings.cpython-39.pyc
--rw-rw-rw-   0        0        0     5903 2023-03-21 09:02:18.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/worker.cpython-310.pyc
--rw-rw-rw-   0        0        0     3297 2023-03-22 08:21:12.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/worker_task.cpython-310.pyc
--rw-rw-rw-   0        0        0     9589 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/spm_template/gui.py
--rw-rw-rw-   0        0        0      698 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/spm_template/main.py
--rw-rw-rw-   0        0        0     3962 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/spm_template/measure_task.py
--rw-rw-rw-   0        0        0     7804 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/spm_template/module.py
--rw-rw-rw-   0        0        0     1210 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/spm_template/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.417110 nanosurf-1.6.1/nanosurf/doc/
--rw-rw-rw-   0        0        0   797639 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/doc/Nanosurf Python Library Overview.pdf
--rw-rw-rw-   0        0        0     6267 2023-05-04 07:47:12.000000 nanosurf-1.6.1/nanosurf/doc/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.427110 nanosurf-1.6.1/nanosurf/lib/
--rw-rw-rw-   0        0        0        0 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.427110 nanosurf-1.6.1/nanosurf/lib/datatypes/
--rw-rw-rw-   0        0        0       52 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/datatypes/__init__.py
--rw-rw-rw-   0        0        0     6982 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/datatypes/prop_val.py
--rw-rw-rw-   0        0        0      856 2023-05-02 06:53:23.000000 nanosurf-1.6.1/nanosurf/lib/datatypes/sci_channel.py
--rw-rw-rw-   0        0        0     5185 2023-05-03 06:11:08.000000 nanosurf-1.6.1/nanosurf/lib/datatypes/sci_stream.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.427110 nanosurf-1.6.1/nanosurf/lib/datatypes/sci_val/
--rw-rw-rw-   0        0        0     8641 2023-03-30 14:33:28.000000 nanosurf-1.6.1/nanosurf/lib/datatypes/sci_val/__init__.py
--rw-rw-rw-   0        0        0     9607 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/lib/datatypes/sci_val/convert.py
--rw-rw-rw-   0        0        0     4102 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/lib/datatypes/sci_val/unit_prefix.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.427110 nanosurf-1.6.1/nanosurf/lib/devices/
--rw-rw-rw-   0        0        0      192 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/devices/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.427110 nanosurf-1.6.1/nanosurf/lib/devices/accessory_interface/
--rw-rw-rw-   0        0        0    13063 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/devices/accessory_interface/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.437112 nanosurf-1.6.1/nanosurf/lib/devices/i2c/
--rw-rw-rw-   0        0        0      469 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/devices/i2c/__init__.py
--rw-rw-rw-   0        0        0     7187 2022-11-08 07:40:33.000000 nanosurf-1.6.1/nanosurf/lib/devices/i2c/bus_master.py
--rw-rw-rw-   0        0        0     2375 2022-11-08 07:40:33.000000 nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_24LC32A.py
--rw-rw-rw-   0        0        0     1123 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_PCA9534.py
--rw-rw-rw-   0        0        0     2830 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_TCN75.py
--rw-rw-rw-   0        0        0    14497 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_TMC5031.py
--rw-rw-rw-   0        0        0     3543 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_TMP42x.py
--rw-rw-rw-   0        0        0     8324 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/lib/devices/trinamic_motor_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.437112 nanosurf-1.6.1/nanosurf/lib/frameworks/
--rw-rw-rw-   0        0        0      225 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.447111 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/
--rw-rw-rw-   0        0        0      225 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.457113 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/
--rw-rw-rw-   0        0        0      405 2023-03-21 09:02:18.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      443 2023-04-17 12:02:23.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     7123 2023-03-21 09:02:18.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/app_base.cpython-310.pyc
--rw-rw-rw-   0        0        0     7469 2023-04-17 12:02:23.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/app_base.cpython-39.pyc
--rw-rw-rw-   0        0        0      509 2023-03-21 09:02:18.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/app_common.cpython-310.pyc
--rw-rw-rw-   0        0        0      505 2023-03-27 12:29:07.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/app_common.cpython-39.pyc
--rw-rw-rw-   0        0        0     7873 2023-03-21 09:02:18.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/app_gui.cpython-310.pyc
--rw-rw-rw-   0        0        0     7979 2023-04-17 12:02:23.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/app_gui.cpython-39.pyc
--rw-rw-rw-   0        0        0     3149 2023-03-21 09:02:18.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/module_base.cpython-310.pyc
--rw-rw-rw-   0        0        0     3341 2023-04-17 12:02:23.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/module_base.cpython-39.pyc
--rw-rw-rw-   0        0        0    12941 2023-03-23 07:32:45.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/nsf_thread.cpython-310.pyc
--rw-rw-rw-   0        0        0    12980 2023-03-27 12:29:07.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/nsf_thread.cpython-39.pyc
--rw-rw-rw-   0        0        0     6750 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/app_base.py
--rw-rw-rw-   0        0        0      195 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/app_common.py
--rw-rw-rw-   0        0        0     7474 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/app_gui.py
--rw-rw-rw-   0        0        0   166135 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/app_icon.ico
--rw-rw-rw-   0        0        0     6279 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/app_stylesheet.qss
--rw-rw-rw-   0        0        0     2271 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/module_base.py
--rw-rw-rw-   0        0        0    13694 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/nsf_thread.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.459619 nanosurf-1.6.1/nanosurf/lib/gui/
--rw-rw-rw-   0        0        0      781 2023-01-23 12:51:02.000000 nanosurf-1.6.1/nanosurf/lib/gui/__init__.py
--rw-rw-rw-   0        0        0     4528 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/gui/bind_gui.py
--rw-rw-rw-   0        0        0     1224 2023-02-02 07:32:08.000000 nanosurf-1.6.1/nanosurf/lib/gui/import_helper.py
--rw-rw-rw-   0        0        0      301 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/lib/gui/nsf_colors.py
--rw-rw-rw-   0        0        0     5545 2023-02-02 07:32:08.000000 nanosurf-1.6.1/nanosurf/lib/gui/nsf_combobox.py
--rw-rw-rw-   0        0        0     5287 2023-02-02 07:32:08.000000 nanosurf-1.6.1/nanosurf/lib/gui/nsf_edit.py
--rw-rw-rw-   0        0        0     1710 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/gui/nsf_info_box.py
--rw-rw-rw-   0        0        0    16496 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/gui/nsf_plots.py
--rw-rw-rw-   0        0        0    26594 2023-02-02 07:32:08.000000 nanosurf-1.6.1/nanosurf/lib/gui/nsf_sci_edit.py
--rw-rw-rw-   0        0        0     6083 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/gui/nsf_tables.py
--rw-rw-rw-   0        0        0      282 2022-12-14 14:12:12.000000 nanosurf-1.6.1/nanosurf/lib/gui/nsf_widgets_common.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.469626 nanosurf-1.6.1/nanosurf/lib/math/
--rw-rw-rw-   0        0        0       56 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/math/__init__.py
--rw-rw-rw-   0        0        0     5577 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/math/iir_filter.py
--rw-rw-rw-   0        0        0    19882 2023-05-03 06:11:08.000000 nanosurf-1.6.1/nanosurf/lib/math/sci_math.py
--rw-rw-rw-   0        0        0    12709 2023-05-03 06:11:08.000000 nanosurf-1.6.1/nanosurf/lib/plot.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.469626 nanosurf-1.6.1/nanosurf/lib/spm/
--rw-rw-rw-   0        0        0      943 2023-02-24 14:35:46.000000 nanosurf-1.6.1/nanosurf/lib/spm/__init__.py
--rw-rw-rw-   0        0        0    17724 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/spm/com_proxy.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.469626 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/
--rw-rw-rw-   0        0        0     4755 2023-03-10 16:14:57.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/__init__.py
--rw-rw-rw-   0        0        0      808 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/check.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.479626 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/
--rw-rw-rw-   0        0        0     1777 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/__init__.py
--rw-rw-rw-   0        0        0     2342 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/adc.py
--rw-rw-rw-   0        0        0     6090 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/analyzer.py
--rw-rw-rw-   0        0        0     6502 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/capture.py
--rw-rw-rw-   0        0        0     1260 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/channelmux.py
--rw-rw-rw-   0        0        0     4528 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/dac.py
--rw-rw-rw-   0        0        0     6009 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/factory.py
--rw-rw-rw-   0        0        0     5016 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/sampler.py
--rw-rw-rw-   0        0        0     7234 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/data_buffer.py
--rw-rw-rw-   0        0        0     5943 2023-05-03 08:56:03.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/data_buffer_interface.py
--rw-rw-rw-   0        0        0     3516 2023-04-12 16:19:57.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/iir_filter.py
--rw-rw-rw-   0        0        0    10920 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/logical_unit_interface.py
--rw-rw-rw-   0        0        0     6353 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/logical_unit_interface_parser.py
--rw-rw-rw-   0        0        0     4227 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/manager_mock.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.479626 nanosurf-1.6.1/nanosurf/lib/spm/scanhead/
--rw-rw-rw-   0        0        0     1698 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/scanhead/__init__.py
--rw-rw-rw-   0        0        0     8222 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/spm/scanhead/drive_afm.py
--rw-rw-rw-   0        0        0    18954 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/spm/scanhead/motor_control.py
--rw-rw-rw-   0        0        0    12254 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/spm/scanhead/studio_motor_control.py
--rw-rw-rw-   0        0        0     1634 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/spm/spm_app.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.479626 nanosurf-1.6.1/nanosurf/lib/spm/studio/
--rw-rw-rw-   0        0        0    22149 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/spm/studio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.489626 nanosurf-1.6.1/nanosurf/lib/spm/studio/wrapper/
--rw-rw-rw-   0        0        0    21945 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/spm/studio/wrapper/__init__.py
--rw-rw-rw-   0        0        0  2934958 2023-04-14 08:23:25.000000 nanosurf-1.6.1/nanosurf/lib/spm/studio/wrapper/cmd_tree_main.py
--rw-rw-rw-   0        0        0  2796278 2023-04-14 08:23:25.000000 nanosurf-1.6.1/nanosurf/lib/spm/studio/wrapper/cmd_tree_spm.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.489626 nanosurf-1.6.1/nanosurf/lib/spm/workflow/
--rw-rw-rw-   0        0        0      129 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/workflow/__init__.py
--rw-rw-rw-   0        0        0    56054 2023-05-03 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/spm/workflow/frequency_sweep.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.499627 nanosurf-1.6.1/nanosurf/lib/util/
--rw-rw-rw-   0        0        0      177 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/util/__init__.py
--rw-rw-rw-   0        0        0     2140 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/lib/util/dataexport.py
--rw-rw-rw-   0        0        0     2561 2022-12-14 14:12:12.000000 nanosurf-1.6.1/nanosurf/lib/util/fileutil.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.323562 nanosurf-1.6.1/nanosurf.egg-info/
--rw-rw-rw-   0        0        0     6686 2023-05-04 07:50:21.000000 nanosurf-1.6.1/nanosurf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12618 2023-05-04 07:50:21.000000 nanosurf-1.6.1/nanosurf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 07:50:21.000000 nanosurf-1.6.1/nanosurf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-04 07:50:21.000000 nanosurf-1.6.1/nanosurf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-04 07:50:20.000000 nanosurf-1.6.1/nanosurf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       78 2023-05-04 07:50:21.000000 nanosurf-1.6.1/nanosurf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 07:50:21.000000 nanosurf-1.6.1/nanosurf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-09-05 14:31:09.000000 nanosurf-1.6.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 07:50:21.501716 nanosurf-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0     2126 2023-05-04 07:42:37.000000 nanosurf-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.870727 nanosurf-1.6.2/
+-rw-rw-rw-   0        0        0     1067 2022-02-08 08:13:22.000000 nanosurf-1.6.2/LICENSE
+-rw-rw-rw-   0        0        0     6808 2023-05-09 09:44:59.862693 nanosurf-1.6.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.680930 nanosurf-1.6.2/nanosurf/
+-rw-rw-rw-   0        0        0     1774 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-05-09 09:42:18.000000 nanosurf-1.6.2/nanosurf/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.669012 nanosurf-1.6.2/nanosurf/app/
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.691028 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.691028 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/.vscode/
+-rw-rw-rw-   0        0        0      566 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/.vscode/launch.json
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.701132 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/
+-rw-rw-rw-   0        0        0     2294 2023-02-17 17:06:00.000000 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_stm_addon.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2285 2023-04-14 11:38:45.000000 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_stm_addon.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2364 2023-05-03 07:22:11.000000 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_tip_current_addon.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1853 2023-02-17 16:53:51.000000 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/gui.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1822 2023-05-03 07:22:11.000000 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/gui.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1523 2023-02-17 17:00:32.000000 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/settings.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1543 2023-05-09 08:48:26.000000 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/settings.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3319 2023-02-17 17:12:09.000000 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3400 2023-05-03 07:22:11.000000 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2670 2023-02-16 15:52:16.000000 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker_task.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2086 2023-05-03 07:19:15.000000 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/device_tip_current_addon.py
+-rw-rw-rw-   0        0        0     1843 2023-05-03 07:17:37.000000 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/gui.py
+-rw-rw-rw-   0        0        0      740 2023-05-03 07:16:24.000000 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/main.py
+-rw-rw-rw-   0        0        0      951 2023-05-09 08:31:37.000000 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/settings.py
+-rw-rw-rw-   0        0        0     4204 2023-05-03 07:20:07.000000 nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/worker.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.701132 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.701132 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/.vscode/
+-rw-rw-rw-   0        0        0      566 2022-09-05 14:31:09.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/.vscode/launch.json
+-rw-rw-rw-   0        0        0     1462 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.709190 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/
+-rw-rw-rw-   0        0        0        0 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.711233 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/
+-rw-rw-rw-   0        0        0      195 2022-12-14 07:35:47.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      185 2023-05-09 07:46:59.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9770 2023-03-09 15:52:53.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/gui.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9831 2023-05-09 08:47:11.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/gui.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5198 2023-03-09 15:52:53.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/imaging_task.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4006 2023-05-09 07:46:59.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/imaging_task.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5181 2023-02-03 08:34:04.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/module.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5236 2023-05-09 07:46:59.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1930 2022-12-14 07:35:47.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/settings.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2083 2023-05-09 08:40:30.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/settings.cpython-39.pyc
+-rw-rw-rw-   0        0        0    13848 2023-05-09 08:47:07.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/gui.py
+-rw-rw-rw-   0        0        0     4907 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/imaging_task.py
+-rw-rw-rw-   0        0        0     5067 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/module.py
+-rw-rw-rw-   0        0        0     1452 2023-05-09 08:39:24.000000 nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.719277 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.719277 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/.vscode/
+-rw-rw-rw-   0        0        0      566 2022-09-05 14:31:09.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/.vscode/launch.json
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.721315 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/
+-rw-rw-rw-   0        0        0        0 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.731387 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/
+-rw-rw-rw-   0        0        0      194 2022-12-16 09:42:02.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      184 2023-05-09 08:48:48.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5443 2023-03-09 14:29:54.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_fit.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5291 2023-05-09 08:48:48.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_fit.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9703 2023-03-09 14:29:54.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_gui.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9635 2023-05-09 08:48:48.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_gui.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9829 2023-02-08 13:02:32.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_module.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9723 2023-05-09 08:48:48.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3005 2023-02-08 13:02:33.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_settings.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3096 2023-05-09 08:48:48.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_settings.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5067 2023-03-09 14:29:54.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_task.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3662 2023-05-09 08:48:48.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_task.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7030 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_fit.py
+-rw-rw-rw-   0        0        0    13971 2023-05-03 08:56:03.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_gui.py
+-rw-rw-rw-   0        0        0    10552 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_module.py
+-rw-rw-rw-   0        0        0     2445 2023-05-09 08:37:36.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_settings.py
+-rw-rw-rw-   0        0        0     3943 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_task.py
+-rw-rw-rw-   0        0        0     1580 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.731387 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.731387 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/.vscode/
+-rw-rw-rw-   0        0        0      566 2022-11-08 07:07:44.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/.vscode/launch.json
+-rw-rw-rw-   0        0        0     1431 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.741516 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/
+-rw-rw-rw-   0        0        0        0 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.749570 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/
+-rw-rw-rw-   0        0        0      199 2022-12-16 13:29:49.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      189 2023-05-09 08:49:32.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9252 2023-02-16 16:05:23.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/gui.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9334 2023-05-09 08:51:15.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/gui.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6662 2023-02-16 16:05:23.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/module.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6564 2023-05-09 08:49:32.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2314 2023-01-25 08:22:47.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/settings.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2322 2023-05-09 08:49:32.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/settings.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4594 2023-03-13 14:19:52.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/worker_task.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3455 2023-05-09 08:49:32.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/worker_task.cpython-39.pyc
+-rw-rw-rw-   0        0        0    13403 2023-05-09 08:51:33.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/gui.py
+-rw-rw-rw-   0        0        0     7055 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/module.py
+-rw-rw-rw-   0        0        0     1949 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/settings.py
+-rw-rw-rw-   0        0        0     4533 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/worker_task.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.751611 nanosurf-1.6.2/nanosurf/app/app_template/
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.751611 nanosurf-1.6.2/nanosurf/app/app_template/.vscode/
+-rw-rw-rw-   0        0        0      566 2022-09-05 14:31:09.000000 nanosurf-1.6.2/nanosurf/app/app_template/.vscode/launch.json
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.751611 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/
+-rw-rw-rw-   0        0        0        0 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.761705 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/
+-rw-rw-rw-   0        0        0      176 2022-12-16 15:19:50.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      192 2023-01-25 09:01:50.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      166 2023-05-09 07:49:12.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6384 2023-02-07 10:44:54.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-310.pyc
+-rw-rw-rw-   0        0        0    13859 2023-01-25 09:01:50.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6336 2023-05-09 08:51:50.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5392 2023-02-09 07:59:12.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9403 2023-01-25 09:01:50.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5327 2023-05-09 08:51:50.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1797 2022-12-16 15:19:50.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2652 2023-01-25 09:01:50.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1904 2023-05-09 08:51:50.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2896 2023-02-07 10:44:54.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5326 2023-01-25 09:01:50.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2593 2023-05-09 08:51:50.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7820 2023-05-09 08:29:37.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/gui.py
+-rw-rw-rw-   0        0        0     5134 2023-05-09 08:29:43.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/module.py
+-rw-rw-rw-   0        0        0     1267 2023-05-09 08:36:42.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/settings.py
+-rw-rw-rw-   0        0        0     2631 2023-05-09 08:35:35.000000 nanosurf-1.6.2/nanosurf/app/app_template/demo_module/worker_task.py
+-rw-rw-rw-   0        0        0     1673 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/app_template/main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.771801 nanosurf-1.6.2/nanosurf/app/demo_creating_spec_pos_table_with_smiley/
+-rw-rw-rw-   0        0        0     4446 2022-11-08 07:07:44.000000 nanosurf-1.6.2/nanosurf/app/demo_creating_spec_pos_table_with_smiley/spectroscopy_demo_creating_a_smiley.ipynb
+-rw-rw-rw-   0        0        0     2457 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/demo_creating_spec_pos_table_with_smiley/spectroscopy_demo_creating_a_smiley.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.771801 nanosurf-1.6.2/nanosurf/app/demo_lateral_force_signal_calibration/
+-rw-rw-rw-   0        0        0    54597 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/app/demo_lateral_force_signal_calibration/demo_lfm_calibration.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.771801 nanosurf-1.6.2/nanosurf/app/demo_move_sample_stage/
+-rw-rw-rw-   0        0        0     7665 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/app/demo_move_sample_stage/demo_move_sample_stage.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.771801 nanosurf-1.6.2/nanosurf/app/demo_spec_setup_and_data_plotting/
+-rw-rw-rw-   0        0        0   121398 2022-11-08 07:07:44.000000 nanosurf-1.6.2/nanosurf/app/demo_spec_setup_and_data_plotting/spec_demo.ipynb
+-rw-rw-rw-   0        0        0     2294 2022-12-20 08:45:27.000000 nanosurf-1.6.2/nanosurf/app/demo_spec_setup_and_data_plotting/spec_demo.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.771801 nanosurf-1.6.2/nanosurf/app/demo_studio_scripting/
+-rw-rw-rw-   0        0        0     4735 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/demo_studio_scripting/studio_demo_data_sampling.py
+-rw-rw-rw-   0        0        0     1817 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/app/demo_studio_scripting/studio_scripting_demo.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.779854 nanosurf-1.6.2/nanosurf/app/spm_template/
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.781896 nanosurf-1.6.2/nanosurf/app/spm_template/.vscode/
+-rw-rw-rw-   0        0        0      566 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/spm_template/.vscode/launch.json
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.781896 nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/
+-rw-rw-rw-   0        0        0     7537 2023-03-22 08:49:37.000000 nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/gui.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7506 2023-05-09 08:52:20.000000 nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/gui.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3307 2023-03-22 08:30:27.000000 nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/measure_task.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3404 2023-05-09 08:52:20.000000 nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/measure_task.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6030 2023-03-22 08:48:33.000000 nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/module.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5992 2023-05-09 08:52:20.000000 nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1702 2023-03-22 08:30:27.000000 nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/settings.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1966 2023-05-09 08:52:20.000000 nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/settings.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5903 2023-03-21 09:02:18.000000 nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/worker.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3297 2023-03-22 08:21:12.000000 nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/worker_task.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9589 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/spm_template/gui.py
+-rw-rw-rw-   0        0        0      698 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/spm_template/main.py
+-rw-rw-rw-   0        0        0     4005 2023-05-09 08:40:06.000000 nanosurf-1.6.2/nanosurf/app/spm_template/measure_task.py
+-rw-rw-rw-   0        0        0     7804 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/app/spm_template/module.py
+-rw-rw-rw-   0        0        0     1354 2023-05-09 08:33:38.000000 nanosurf-1.6.2/nanosurf/app/spm_template/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.791990 nanosurf-1.6.2/nanosurf/doc/
+-rw-rw-rw-   0        0        0   797639 2022-09-05 14:31:09.000000 nanosurf-1.6.2/nanosurf/doc/Nanosurf Python Library Overview.pdf
+-rw-rw-rw-   0        0        0     6389 2023-05-09 09:43:56.000000 nanosurf-1.6.2/nanosurf/doc/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.791990 nanosurf-1.6.2/nanosurf/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-05 14:31:09.000000 nanosurf-1.6.2/nanosurf/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.791990 nanosurf-1.6.2/nanosurf/lib/datatypes/
+-rw-rw-rw-   0        0        0       52 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/lib/datatypes/__init__.py
+-rw-rw-rw-   0        0        0     6982 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/lib/datatypes/prop_val.py
+-rw-rw-rw-   0        0        0      856 2023-05-02 06:53:23.000000 nanosurf-1.6.2/nanosurf/lib/datatypes/sci_channel.py
+-rw-rw-rw-   0        0        0     5185 2023-05-03 06:11:08.000000 nanosurf-1.6.2/nanosurf/lib/datatypes/sci_stream.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.791990 nanosurf-1.6.2/nanosurf/lib/datatypes/sci_val/
+-rw-rw-rw-   0        0        0     8641 2023-03-30 14:33:28.000000 nanosurf-1.6.2/nanosurf/lib/datatypes/sci_val/__init__.py
+-rw-rw-rw-   0        0        0     9607 2022-09-05 14:31:09.000000 nanosurf-1.6.2/nanosurf/lib/datatypes/sci_val/convert.py
+-rw-rw-rw-   0        0        0     4102 2022-09-05 14:31:09.000000 nanosurf-1.6.2/nanosurf/lib/datatypes/sci_val/unit_prefix.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.800048 nanosurf-1.6.2/nanosurf/lib/devices/
+-rw-rw-rw-   0        0        0      192 2022-11-08 07:07:44.000000 nanosurf-1.6.2/nanosurf/lib/devices/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.802092 nanosurf-1.6.2/nanosurf/lib/devices/accessory_interface/
+-rw-rw-rw-   0        0        0    13063 2022-11-08 07:07:44.000000 nanosurf-1.6.2/nanosurf/lib/devices/accessory_interface/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.802092 nanosurf-1.6.2/nanosurf/lib/devices/i2c/
+-rw-rw-rw-   0        0        0      469 2022-11-08 07:07:44.000000 nanosurf-1.6.2/nanosurf/lib/devices/i2c/__init__.py
+-rw-rw-rw-   0        0        0     7187 2022-11-08 07:40:33.000000 nanosurf-1.6.2/nanosurf/lib/devices/i2c/bus_master.py
+-rw-rw-rw-   0        0        0     2375 2022-11-08 07:40:33.000000 nanosurf-1.6.2/nanosurf/lib/devices/i2c/chip_24LC32A.py
+-rw-rw-rw-   0        0        0     1123 2022-11-08 07:07:44.000000 nanosurf-1.6.2/nanosurf/lib/devices/i2c/chip_PCA9534.py
+-rw-rw-rw-   0        0        0     2830 2022-11-08 07:07:44.000000 nanosurf-1.6.2/nanosurf/lib/devices/i2c/chip_TCN75.py
+-rw-rw-rw-   0        0        0    14497 2022-11-08 07:07:44.000000 nanosurf-1.6.2/nanosurf/lib/devices/i2c/chip_TMC5031.py
+-rw-rw-rw-   0        0        0     3543 2022-11-08 07:07:44.000000 nanosurf-1.6.2/nanosurf/lib/devices/i2c/chip_TMP42x.py
+-rw-rw-rw-   0        0        0     8324 2022-09-05 14:31:09.000000 nanosurf-1.6.2/nanosurf/lib/devices/trinamic_motor_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.802092 nanosurf-1.6.2/nanosurf/lib/frameworks/
+-rw-rw-rw-   0        0        0      225 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.812186 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/
+-rw-rw-rw-   0        0        0      225 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.822278 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/
+-rw-rw-rw-   0        0        0      405 2023-03-21 09:02:18.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      443 2023-04-17 12:02:23.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7123 2023-03-21 09:02:18.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/app_base.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7776 2023-05-09 08:40:30.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/app_base.cpython-39.pyc
+-rw-rw-rw-   0        0        0      509 2023-03-21 09:02:18.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/app_common.cpython-310.pyc
+-rw-rw-rw-   0        0        0      505 2023-03-27 12:29:07.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/app_common.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7873 2023-03-21 09:02:18.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/app_gui.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8457 2023-05-09 08:03:09.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/app_gui.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3149 2023-03-21 09:02:18.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/module_base.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3299 2023-05-09 08:40:30.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/module_base.cpython-39.pyc
+-rw-rw-rw-   0        0        0    12941 2023-03-23 07:32:45.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/nsf_thread.cpython-310.pyc
+-rw-rw-rw-   0        0        0    12980 2023-03-27 12:29:07.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/nsf_thread.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7095 2023-05-09 08:27:12.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/app_base.py
+-rw-rw-rw-   0        0        0      195 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/app_common.py
+-rw-rw-rw-   0        0        0     7731 2023-05-09 08:01:43.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/app_gui.py
+-rw-rw-rw-   0        0        0   166135 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/app_icon.ico
+-rw-rw-rw-   0        0        0     6279 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/app_stylesheet.qss
+-rw-rw-rw-   0        0        0     2202 2023-05-09 08:26:51.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/module_base.py
+-rw-rw-rw-   0        0        0    13694 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/nsf_thread.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.832410 nanosurf-1.6.2/nanosurf/lib/gui/
+-rw-rw-rw-   0        0        0      781 2023-01-23 12:51:02.000000 nanosurf-1.6.2/nanosurf/lib/gui/__init__.py
+-rw-rw-rw-   0        0        0     4528 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/lib/gui/bind_gui.py
+-rw-rw-rw-   0        0        0     1224 2023-02-02 07:32:08.000000 nanosurf-1.6.2/nanosurf/lib/gui/import_helper.py
+-rw-rw-rw-   0        0        0      301 2022-09-05 14:31:09.000000 nanosurf-1.6.2/nanosurf/lib/gui/nsf_colors.py
+-rw-rw-rw-   0        0        0     5545 2023-02-02 07:32:08.000000 nanosurf-1.6.2/nanosurf/lib/gui/nsf_combobox.py
+-rw-rw-rw-   0        0        0     5287 2023-02-02 07:32:08.000000 nanosurf-1.6.2/nanosurf/lib/gui/nsf_edit.py
+-rw-rw-rw-   0        0        0     1710 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/lib/gui/nsf_info_box.py
+-rw-rw-rw-   0        0        0    16496 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/lib/gui/nsf_plots.py
+-rw-rw-rw-   0        0        0    26594 2023-02-02 07:32:08.000000 nanosurf-1.6.2/nanosurf/lib/gui/nsf_sci_edit.py
+-rw-rw-rw-   0        0        0     6083 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/lib/gui/nsf_tables.py
+-rw-rw-rw-   0        0        0      282 2022-12-14 14:12:12.000000 nanosurf-1.6.2/nanosurf/lib/gui/nsf_widgets_common.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.832410 nanosurf-1.6.2/nanosurf/lib/math/
+-rw-rw-rw-   0        0        0       56 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/lib/math/__init__.py
+-rw-rw-rw-   0        0        0     5577 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/lib/math/iir_filter.py
+-rw-rw-rw-   0        0        0    19882 2023-05-03 06:11:08.000000 nanosurf-1.6.2/nanosurf/lib/math/sci_math.py
+-rw-rw-rw-   0        0        0    12709 2023-05-03 06:11:08.000000 nanosurf-1.6.2/nanosurf/lib/plot.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.832410 nanosurf-1.6.2/nanosurf/lib/spm/
+-rw-rw-rw-   0        0        0      943 2023-02-24 14:35:46.000000 nanosurf-1.6.2/nanosurf/lib/spm/__init__.py
+-rw-rw-rw-   0        0        0    17724 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/lib/spm/com_proxy.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.842513 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/
+-rw-rw-rw-   0        0        0     4755 2023-03-10 16:14:57.000000 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/__init__.py
+-rw-rw-rw-   0        0        0      808 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/check.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.852600 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/
+-rw-rw-rw-   0        0        0     1777 2022-12-20 08:45:27.000000 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/__init__.py
+-rw-rw-rw-   0        0        0     2342 2022-12-20 08:45:27.000000 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/adc.py
+-rw-rw-rw-   0        0        0     6090 2022-12-20 08:45:27.000000 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/analyzer.py
+-rw-rw-rw-   0        0        0     6502 2022-12-20 08:45:27.000000 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/capture.py
+-rw-rw-rw-   0        0        0     1260 2022-12-20 08:45:27.000000 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/channelmux.py
+-rw-rw-rw-   0        0        0     4528 2022-12-20 08:45:27.000000 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/dac.py
+-rw-rw-rw-   0        0        0     6009 2022-12-20 08:45:27.000000 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/factory.py
+-rw-rw-rw-   0        0        0     5016 2022-12-20 08:45:27.000000 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/sampler.py
+-rw-rw-rw-   0        0        0     7234 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/data_buffer.py
+-rw-rw-rw-   0        0        0     5943 2023-05-03 08:56:03.000000 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/data_buffer_interface.py
+-rw-rw-rw-   0        0        0     3516 2023-04-12 16:19:57.000000 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/iir_filter.py
+-rw-rw-rw-   0        0        0    10920 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/logical_unit_interface.py
+-rw-rw-rw-   0        0        0     6353 2022-09-05 14:31:09.000000 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/logical_unit_interface_parser.py
+-rw-rw-rw-   0        0        0     4227 2022-09-05 14:31:09.000000 nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/manager_mock.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.852600 nanosurf-1.6.2/nanosurf/lib/spm/scanhead/
+-rw-rw-rw-   0        0        0     1698 2022-12-20 08:45:27.000000 nanosurf-1.6.2/nanosurf/lib/spm/scanhead/__init__.py
+-rw-rw-rw-   0        0        0     8222 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/lib/spm/scanhead/drive_afm.py
+-rw-rw-rw-   0        0        0    18954 2022-11-08 07:07:44.000000 nanosurf-1.6.2/nanosurf/lib/spm/scanhead/motor_control.py
+-rw-rw-rw-   0        0        0    12254 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/lib/spm/scanhead/studio_motor_control.py
+-rw-rw-rw-   0        0        0     1634 2023-04-14 12:55:54.000000 nanosurf-1.6.2/nanosurf/lib/spm/spm_app.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.852600 nanosurf-1.6.2/nanosurf/lib/spm/studio/
+-rw-rw-rw-   0        0        0    22149 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/lib/spm/studio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.862693 nanosurf-1.6.2/nanosurf/lib/spm/studio/wrapper/
+-rw-rw-rw-   0        0        0    21945 2023-03-27 12:25:59.000000 nanosurf-1.6.2/nanosurf/lib/spm/studio/wrapper/__init__.py
+-rw-rw-rw-   0        0        0  2934958 2023-04-14 08:23:25.000000 nanosurf-1.6.2/nanosurf/lib/spm/studio/wrapper/cmd_tree_main.py
+-rw-rw-rw-   0        0        0  2796278 2023-04-14 08:23:25.000000 nanosurf-1.6.2/nanosurf/lib/spm/studio/wrapper/cmd_tree_spm.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.862693 nanosurf-1.6.2/nanosurf/lib/spm/workflow/
+-rw-rw-rw-   0        0        0      129 2022-12-20 08:45:27.000000 nanosurf-1.6.2/nanosurf/lib/spm/workflow/__init__.py
+-rw-rw-rw-   0        0        0    56054 2023-05-03 07:07:44.000000 nanosurf-1.6.2/nanosurf/lib/spm/workflow/frequency_sweep.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.862693 nanosurf-1.6.2/nanosurf/lib/util/
+-rw-rw-rw-   0        0        0      177 2022-11-08 07:07:44.000000 nanosurf-1.6.2/nanosurf/lib/util/__init__.py
+-rw-rw-rw-   0        0        0     2140 2022-09-05 14:31:09.000000 nanosurf-1.6.2/nanosurf/lib/util/dataexport.py
+-rw-rw-rw-   0        0        0     2561 2022-12-14 14:12:12.000000 nanosurf-1.6.2/nanosurf/lib/util/fileutil.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:44:59.688989 nanosurf-1.6.2/nanosurf.egg-info/
+-rw-rw-rw-   0        0        0     6808 2023-05-09 09:44:59.000000 nanosurf-1.6.2/nanosurf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    12618 2023-05-09 09:44:59.000000 nanosurf-1.6.2/nanosurf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 09:44:59.000000 nanosurf-1.6.2/nanosurf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-09 09:44:59.000000 nanosurf-1.6.2/nanosurf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-09 09:44:59.000000 nanosurf-1.6.2/nanosurf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       78 2023-05-09 09:44:59.000000 nanosurf-1.6.2/nanosurf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-09 09:44:59.000000 nanosurf-1.6.2/nanosurf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-09-05 14:31:09.000000 nanosurf-1.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 09:44:59.870727 nanosurf-1.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     2126 2023-05-04 07:42:37.000000 nanosurf-1.6.2/setup.py
```

### Comparing `nanosurf-1.6.1/LICENSE` & `nanosurf-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/PKG-INFO` & `nanosurf-1.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanosurf
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python API for Nanosurf controllers
 Author: Nanosurf AG
 Author-email: scripting@nanosurf.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -145,14 +145,18 @@
 
 Full list of objects and methods can be found in the Scripting Manual
 in Nanosurf controller software under Help tab:
 Help -> Manuals -> Script Programmers Manual, or [here](https://www.nanosurf.com/downloads/programmers-manual.pdf).
 
 ## Library Version History
 
+* v1.6.2
+  * New: qt_app_framwork supports multi screen modules
+  * Bugfix: settings should not be of dataclass type
+
 * v1.6.1
   * Bugfix: pip packaging did not copy framework files
 
 * v1.6.0
   * New: spm_template: A new template to demonstrate simple connection to CX/Studio and measure some data
   * New: app_DriveAFM_Tip_Current_Addon this app controls the amplifier of the Tip-Current Addon
   * New: demo_move_sample_stage. This demo shows basic stage movements
```

### Comparing `nanosurf-1.6.1/nanosurf/__init__.py` & `nanosurf-1.6.2/nanosurf/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/.vscode/launch.json` & `nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_stm_addon.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_stm_addon.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_stm_addon.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_stm_addon.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_tip_current_addon.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_tip_current_addon.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/gui.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/gui.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/gui.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/gui.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/settings.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/settings.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/settings.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed May  3 07:17:37 2023 UTC, .py size: 893 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,86 +1,97 @@
-00000000: 610d 0d0a 0000 0000 910a 5264 7d03 0000  a.........Rd}...
+00000000: 610d 0d0a 0000 0000 e904 5a64 b703 0000  a.........Zd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
+00000020: 0004 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a05 4700  m.Z...d.d.l.Z.G.
 00000050: 6404 6405 8400 6405 6501 6a06 8303 5a07  d.d...d.e.j...Z.
-00000060: 6503 4700 6406 6407 8400 6407 6505 6a08  e.G.d.d...d.e.j.
-00000070: 8303 8301 5a09 6503 4700 6408 6409 8400  ....Z.e.G.d.d...
-00000080: 6409 8302 8301 5a0a 6402 5300 290a 7abc  d.....Z.d.S.).z.
-00000090: 2044 6566 696e 6573 2074 6865 2063 6f6e   Defines the con
-000000a0: 6669 6775 7261 7469 6f6e 2076 616c 7565  figuration value
-000000b0: 7320 6f66 2074 6865 206d 6f64 756c 652e  s of the module.
-000000c0: 0a20 2020 2056 616c 7565 7320 696e 2074  .    Values in t
-000000d0: 6865 2050 726f 5374 6f72 6520 6172 6520  he ProStore are 
-000000e0: 7361 7665 6420 616e 6420 6c6f 6164 6564  saved and loaded
-000000f0: 2064 7572 696e 6720 6170 706c 6963 6174   during applicat
-00000100: 696f 6e20 7374 6172 7475 702f 7368 7574  ion startup/shut
-00000110: 646f 776e 2061 7574 6f6d 6174 6963 616c  down automatical
-00000120: 6c79 0a43 6f70 7972 6967 6874 204e 616e  ly.Copyright Nan
-00000130: 6f73 7572 6620 4147 2032 3032 310a 4c69  osurf AG 2021.Li
-00000140: 6365 6e73 6520 2d20 4d49 540a e900 0000  cense - MIT.....
-00000150: 004e 2901 da09 6461 7461 636c 6173 7363  .N)...dataclassc
-00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000170: 0100 0000 4000 0000 7318 0000 0065 005a  ....@...s....e.Z
-00000180: 0164 005a 0264 015a 0364 025a 0464 035a  .d.Z.d.Z.d.Z.d.Z
-00000190: 0564 0453 0029 05da 0f41 6d70 6c69 6669  .d.S.)...Amplifi
-000001a0: 6572 4761 696e 4944 e901 0000 00e9 0200  erGainID........
-000001b0: 0000 e903 0000 004e 2906 da08 5f5f 6e61  .......N)...__na
-000001c0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000001d0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0a  ..__qualname__..
-000001e0: 4761 696e 5f35 3030 7541 da08 4761 696e  Gain_500uA..Gain
-000001f0: 5f35 7541 da09 4761 696e 5f35 306e 41a9  _5uA..Gain_50nA.
-00000200: 0072 0d00 0000 720d 0000 00fa 5143 3a5c  .r....r.....QC:\
-00000210: 4769 745c 7363 7269 7074 735f 7079 7468  Git\scripts_pyth
-00000220: 6f6e 5f6c 6962 5c6e 616e 6f73 7572 665c  on_lib\nanosurf\
-00000230: 6170 705c 6170 705f 4472 6976 6541 464d  app\app_DriveAFM
-00000240: 5f54 6970 5f43 7572 7265 6e74 5f41 6464  _Tip_Current_Add
-00000250: 6f6e 5c73 6574 7469 6e67 732e 7079 7203  on\settings.pyr.
-00000260: 0000 000c 0000 0073 0600 0000 0801 0401  .......s........
-00000270: 0401 7203 0000 0063 0000 0000 0000 0000  ..r....c........
-00000280: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
-00000290: 7320 0000 0065 005a 0164 005a 0264 015a  s ...e.Z.d.Z.d.Z
-000002a0: 0365 04a0 0565 0665 076a 0883 01a1 015a  .e...e.e.j.....Z
-000002b0: 0964 0253 0029 03da 0853 6574 7469 6e67  .d.S.)...Setting
-000002c0: 737a ad20 7365 7474 696e 6773 2064 6566  sz. settings def
-000002d0: 696e 6564 2068 6572 6520 6173 2050 726f  ined here as Pro
-000002e0: 7056 616c 2061 7265 2073 746f 7265 6420  pVal are stored 
-000002f0: 7065 7273 6973 7465 6e74 6c79 2069 6e20  persistently in 
-00000300: 6120 696e 692d 6669 6c65 200a 2020 2020  a ini-file .    
-00000310: 2020 2020 436f 756c 6420 6265 2063 6f6e      Could be con
-00000320: 6e65 6374 6564 2061 6c73 6f20 746f 2047  nected also to G
-00000330: 5549 2065 6c65 6d65 6e74 7320 2865 2e67  UI elements (e.g
-00000340: 2e3a 206c 6f6f 6b20 696e 746f 2062 696e  .: look into bin
-00000350: 645f 6775 695f 656c 656d 656e 7473 2829  d_gui_elements()
-00000360: 2069 6e20 6775 692e 7079 290a 2020 2020   in gui.py).    
-00000370: 4e29 0a72 0700 0000 7208 0000 0072 0900  N).r....r....r..
-00000380: 0000 da07 5f5f 646f 635f 5fda 036e 7366  ....__doc__..nsf
-00000390: da07 5072 6f70 5661 6cda 0369 6e74 7203  ..PropVal..intr.
-000003a0: 0000 0072 0a00 0000 da07 6761 696e 5f69  ...r......gain_i
-000003b0: 6472 0d00 0000 720d 0000 0072 0d00 0000  dr....r....r....
-000003c0: 720e 0000 0072 0f00 0000 1100 0000 7304  r....r........s.
-000003d0: 0000 0008 0204 0372 0f00 0000 6300 0000  .......r....c...
-000003e0: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-000003f0: 0040 0000 0073 1000 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000400: 5a02 6401 5a03 6402 5300 2903 da0d 576f  Z.d.Z.d.S.)...Wo
-00000410: 726b 6572 5265 7375 6c74 737a 6a20 5468  rkerResultszj Th
-00000420: 6973 2063 6c61 7373 2073 6176 6573 2074  is class saves t
-00000430: 6865 2077 6f72 6b65 7220 6d6f 6475 6c65  he worker module
-00000440: 2072 6573 756c 7420 2865 2e67 2e3a 2062   result (e.g.: b
-00000450: 6520 7265 6164 2062 7920 6775 6920 656c  e read by gui el
-00000460: 656d 656e 7473 206c 696b 6520 4e53 4643  ements like NSFC
-00000470: 6861 7274 206f 7220 7361 7665 6420 746f  hart or saved to
-00000480: 2066 696c 6529 204e 2904 7207 0000 0072   file) N).r....r
-00000490: 0800 0000 7209 0000 0072 1000 0000 720d  ....r....r....r.
-000004a0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-000004b0: 0000 7215 0000 0018 0000 0073 0400 0000  ..r........s....
-000004c0: 0802 0401 7215 0000 0029 0b72 1000 0000  ....r....).r....
-000004d0: da04 656e 756d da0b 6461 7461 636c 6173  ..enum..dataclas
-000004e0: 7365 7372 0200 0000 da08 6e61 6e6f 7375  sesr......nanosu
-000004f0: 7266 7211 0000 00da 0749 6e74 456e 756d  rfr......IntEnum
-00000500: 7203 0000 00da 0950 726f 7053 746f 7265  r......PropStore
-00000510: 720f 0000 0072 1500 0000 720d 0000 0072  r....r....r....r
-00000520: 0d00 0000 720d 0000 0072 0e00 0000 da08  ....r....r......
-00000530: 3c6d 6f64 756c 653e 0100 0000 7310 0000  <module>....s...
-00000540: 0004 0608 010c 0108 0312 0502 0114 0602  ................
-00000550: 01                                       .
+00000060: 4700 6406 6407 8400 6407 6505 6a08 8303  G.d.d...d.e.j...
+00000070: 5a09 6503 4700 6408 6409 8400 6409 8302  Z.e.G.d.d...d...
+00000080: 8301 5a0a 6402 5300 290a 7abc 2044 6566  ..Z.d.S.).z. Def
+00000090: 696e 6573 2074 6865 2063 6f6e 6669 6775  ines the configu
+000000a0: 7261 7469 6f6e 2076 616c 7565 7320 6f66  ration values of
+000000b0: 2074 6865 206d 6f64 756c 652e 0a20 2020   the module..   
+000000c0: 2056 616c 7565 7320 696e 2074 6865 2050   Values in the P
+000000d0: 726f 5374 6f72 6520 6172 6520 7361 7665  roStore are save
+000000e0: 6420 616e 6420 6c6f 6164 6564 2064 7572  d and loaded dur
+000000f0: 696e 6720 6170 706c 6963 6174 696f 6e20  ing application 
+00000100: 7374 6172 7475 702f 7368 7574 646f 776e  startup/shutdown
+00000110: 2061 7574 6f6d 6174 6963 616c 6c79 0a43   automatically.C
+00000120: 6f70 7972 6967 6874 204e 616e 6f73 7572  opyright Nanosur
+00000130: 6620 4147 2032 3032 310a 4c69 6365 6e73  f AG 2021.Licens
+00000140: 6520 2d20 4d49 540a e900 0000 004e 2901  e - MIT......N).
+00000150: da09 6461 7461 636c 6173 7363 0000 0000  ..dataclassc....
+00000160: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+00000170: 4000 0000 7318 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00000180: 0264 015a 0364 025a 0464 035a 0564 0453  .d.Z.d.Z.d.Z.d.S
+00000190: 0029 05da 0f41 6d70 6c69 6669 6572 4761  .)...AmplifierGa
+000001a0: 696e 4944 e901 0000 00e9 0200 0000 e903  inID............
+000001b0: 0000 004e 2906 da08 5f5f 6e61 6d65 5f5f  ...N)...__name__
+000001c0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+000001d0: 7175 616c 6e61 6d65 5f5f da0a 4761 696e  qualname__..Gain
+000001e0: 5f35 3030 7541 da08 4761 696e 5f35 7541  _500uA..Gain_5uA
+000001f0: da09 4761 696e 5f35 306e 41a9 0072 0d00  ..Gain_50nA..r..
+00000200: 0000 720d 0000 00fa 5143 3a5c 4769 745c  ..r.....QC:\Git\
+00000210: 7363 7269 7074 735f 7079 7468 6f6e 5f6c  scripts_python_l
+00000220: 6962 5c6e 616e 6f73 7572 665c 6170 705c  ib\nanosurf\app\
+00000230: 6170 705f 4472 6976 6541 464d 5f54 6970  app_DriveAFM_Tip
+00000240: 5f43 7572 7265 6e74 5f41 6464 6f6e 5c73  _Current_Addon\s
+00000250: 6574 7469 6e67 732e 7079 7203 0000 000c  ettings.pyr.....
+00000260: 0000 0073 0600 0000 0801 0401 0401 7203  ...s..........r.
+00000270: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000280: 0000 0000 0400 0000 0000 0000 7326 0000  ............s&..
+00000290: 0065 005a 0164 005a 0264 015a 0364 0264  .e.Z.d.Z.d.Z.d.d
+000002a0: 039c 0187 0066 0164 0464 0584 0c5a 0487  .....f.d.d...Z..
+000002b0: 0004 005a 0553 0029 06da 0853 6574 7469  ...Z.S.)...Setti
+000002c0: 6e67 737a ad20 7365 7474 696e 6773 2064  ngsz. settings d
+000002d0: 6566 696e 6564 2068 6572 6520 6173 2050  efined here as P
+000002e0: 726f 7056 616c 2061 7265 2073 746f 7265  ropVal are store
+000002f0: 6420 7065 7273 6973 7465 6e74 6c79 2069  d persistently i
+00000300: 6e20 6120 696e 692d 6669 6c65 200a 2020  n a ini-file .  
+00000310: 2020 2020 2020 436f 756c 6420 6265 2063        Could be c
+00000320: 6f6e 6e65 6374 6564 2061 6c73 6f20 746f  onnected also to
+00000330: 2047 5549 2065 6c65 6d65 6e74 7320 2865   GUI elements (e
+00000340: 2e67 2e3a 206c 6f6f 6b20 696e 746f 2062  .g.: look into b
+00000350: 696e 645f 6775 695f 656c 656d 656e 7473  ind_gui_elements
+00000360: 2829 2069 6e20 6775 692e 7079 290a 2020  () in gui.py).  
+00000370: 2020 4e29 01da 0672 6574 7572 6e63 0100    N)...returnc..
+00000380: 0000 0000 0000 0000 0000 0100 0000 0400  ................
+00000390: 0000 0300 0000 7320 0000 0074 0083 00a0  ......s ...t....
+000003a0: 01a1 0001 0074 02a0 0374 0474 056a 0683  .....t...t.t.j..
+000003b0: 01a1 017c 005f 0764 0053 0029 014e 2908  ...|._.d.S.).N).
+000003c0: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
+000003d0: 5fda 036e 7366 da07 5072 6f70 5661 6cda  _..nsf..PropVal.
+000003e0: 0369 6e74 7203 0000 0072 0a00 0000 da07  .intr....r......
+000003f0: 6761 696e 5f69 6429 01da 0473 656c 66a9  gain_id)...self.
+00000400: 01da 095f 5f63 6c61 7373 5f5f 720d 0000  ...__class__r...
+00000410: 0072 0e00 0000 7212 0000 0015 0000 0073  .r....r........s
+00000420: 0400 0000 0001 0a01 7a11 5365 7474 696e  ........z.Settin
+00000430: 6773 2e5f 5f69 6e69 745f 5f29 0672 0700  gs.__init__).r..
+00000440: 0000 7208 0000 0072 0900 0000 da07 5f5f  ..r....r......__
+00000450: 646f 635f 5f72 1200 0000 da0d 5f5f 636c  doc__r......__cl
+00000460: 6173 7363 656c 6c5f 5f72 0d00 0000 720d  asscell__r....r.
+00000470: 0000 0072 1800 0000 720e 0000 0072 0f00  ...r....r....r..
+00000480: 0000 1100 0000 7304 0000 0008 0104 0372  ......s........r
+00000490: 0f00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+000004a0: 0000 0000 0001 0000 0040 0000 0073 1000  .........@...s..
+000004b0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+000004c0: 5300 2903 da0d 576f 726b 6572 5265 7375  S.)...WorkerResu
+000004d0: 6c74 737a 6a20 5468 6973 2063 6c61 7373  ltszj This class
+000004e0: 2073 6176 6573 2074 6865 2077 6f72 6b65   saves the worke
+000004f0: 7220 6d6f 6475 6c65 2072 6573 756c 7420  r module result 
+00000500: 2865 2e67 2e3a 2062 6520 7265 6164 2062  (e.g.: be read b
+00000510: 7920 6775 6920 656c 656d 656e 7473 206c  y gui elements l
+00000520: 696b 6520 4e53 4643 6861 7274 206f 7220  ike NSFChart or 
+00000530: 7361 7665 6420 746f 2066 696c 6529 204e  saved to file) N
+00000540: 2904 7207 0000 0072 0800 0000 7209 0000  ).r....r....r...
+00000550: 0072 1a00 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00000560: 720d 0000 0072 0e00 0000 721c 0000 0019  r....r....r.....
+00000570: 0000 0073 0400 0000 0802 0401 721c 0000  ...s........r...
+00000580: 0029 0b72 1a00 0000 da04 656e 756d da0b  .).r......enum..
+00000590: 6461 7461 636c 6173 7365 7372 0200 0000  dataclassesr....
+000005a0: da08 6e61 6e6f 7375 7266 7213 0000 00da  ..nanosurfr.....
+000005b0: 0749 6e74 456e 756d 7203 0000 00da 0950  .IntEnumr......P
+000005c0: 726f 7053 746f 7265 720f 0000 0072 1c00  ropStorer....r..
+000005d0: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+000005e0: 0072 0e00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000005f0: 0100 0000 730e 0000 0004 0608 010c 0108  ....s...........
+00000600: 0312 0512 0802 01                        .......
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker_task.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker_task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/device_tip_current_addon.py` & `nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/device_tip_current_addon.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/gui.py` & `nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/gui.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/main.py` & `nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/main.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/settings.py` & `nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 
 """ Available monitoring channels defined by the worker task"""
 class AmplifierGainID(enum.IntEnum):
     Gain_500uA = 1
     Gain_5uA = 2
     Gain_50nA = 3
 
-@dataclass
 class Settings(nsf.PropStore):
     """ settings defined here as PropVal are stored persistently in a ini-file 
         Could be connected also to GUI elements (e.g.: look into bind_gui_elements() in gui.py)
     """
-    gain_id = nsf.PropVal(int(AmplifierGainID.Gain_500uA))
+    def __init__(self) -> None:
+        super().__init__()
+        self.gain_id = nsf.PropVal(int(AmplifierGainID.Gain_500uA))
 
 @dataclass
 class WorkerResults():
     """ This class saves the worker module result (e.g.: be read by gui elements like NSFChart or saved to file) """
     pass
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/worker.py` & `nanosurf-1.6.2/nanosurf/app/app_DriveAFM_Tip_Current_Addon/worker.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/.vscode/launch.json` & `nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/main.py` & `nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/main.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/gui.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/gui.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/gui.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/gui.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 09:26:35 2023 UTC, .py size: 13848 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 4b1c 3964 1836 0000  a.......K.9d.6..
+00000000: 610d 0d0a 0000 0000 8b08 5a64 1836 0000  a.........Zd.6..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 ea00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 0100 6504 8300 722c 6401 6404  m.Z...e...r,d.d.
 00000050: 6c05 6d06 5a06 0100 6e0c 6401 6404 6c07  l.m.Z...n.d.d.l.
 00000060: 6d06 5a06 0100 6401 6402 6c08 5a09 6401  m.Z...d.d.l.Z.d.
 00000070: 6405 6c0a 6d0b 5a0b 6d0c 5a0c 0100 4700  d.l.m.Z.m.Z...G.
@@ -92,48 +92,48 @@
 000005b0: 0201 0074 016a 02a0 1374 1464 0ba1 027c  ...t.j...t.d...|
 000005c0: 005f 1574 16a0 1764 0ca1 017c 005f 1874  ._.t...d...|._.t
 000005d0: 16a0 19a1 007c 005f 1a7c 006a 1aa0 1b7c  .....|._.|.j...|
 000005e0: 006a 04a1 0101 007c 006a 1aa0 1b7c 006a  .j.....|.j...|.j
 000005f0: 0ea1 0101 007c 006a 1aa0 1b7c 006a 11a1  .....|.j...|.j..
 00000600: 0101 007c 006a 1aa0 1b7c 006a 15a1 0101  ...|.j...|.j....
 00000610: 007c 006a 1aa0 1ca1 0001 007c 006a 1aa0  .|.j.......|.j..
-00000620: 1b7c 006a 18a1 0101 0074 016a 02a0 1da1  .|.j.....t.j....
-00000630: 007c 005f 1e74 016a 02a0 1fa1 007c 005f  .|._.t.j.....|._
-00000640: 2074 016a 026a 1d64 0d64 0d64 0e8d 027c   t.j.j.d.d.d...|
-00000650: 005f 2174 16a0 2264 0fa1 017c 005f 2374  ._!t.."d...|._#t
-00000660: 16a0 2264 10a1 017c 005f 2474 16a0 2264  .."d...|._$t.."d
-00000670: 11a1 017c 005f 2574 16a0 2264 12a1 017c  ...|._%t.."d...|
-00000680: 005f 2674 016a 02a0 2774 28a1 017c 005f  ._&t.j..'t(..|._
-00000690: 297c 006a 29a0 2a74 286a 2b64 13a1 0201  )|.j).*t(j+d....
-000006a0: 007c 006a 29a0 2a74 286a 2c64 14a1 0201  .|.j).*t(j,d....
-000006b0: 007c 006a 29a0 2a74 286a 2d64 15a1 0201  .|.j).*t(j-d....
-000006c0: 007c 006a 29a0 2a74 286a 2e64 16a1 0201  .|.j).*t(j.d....
-000006d0: 0074 16a0 19a1 007c 005f 2f74 16a0 30a1  .t.....|._/t..0.
-000006e0: 007c 005f 317c 006a 31a0 1b7c 006a 20a1  .|._1|.j1..|.j .
-000006f0: 0101 007c 006a 31a0 1b7c 006a 206a 32a1  ...|.j1..|.j j2.
-00000700: 0101 0074 16a0 19a1 007c 005f 337c 006a  ...t.....|._3|.j
-00000710: 33a0 347c 006a 31a1 0101 007c 006a 33a0  3.4|.j1....|.j3.
-00000720: 1b7c 006a 23a1 0101 0074 16a0 19a1 007c  .|.j#....t.....|
-00000730: 005f 357c 006a 35a0 1b7c 006a 1ea1 0101  ._5|.j5..|.j....
-00000740: 007c 006a 35a0 1b7c 006a 24a1 0101 0074  .|.j5..|.j$....t
-00000750: 16a0 19a1 007c 005f 367c 006a 36a0 1b7c  .....|._6|.j6..|
-00000760: 006a 21a1 0101 007c 006a 36a0 1b7c 006a  .j!....|.j6..|.j
-00000770: 25a1 0101 007c 006a 36a0 1b7c 006a 26a1  %....|.j6..|.j&.
-00000780: 0101 0074 16a0 19a1 007c 005f 377c 006a  ...t.....|._7|.j
-00000790: 37a0 347c 006a 35a1 0101 007c 006a 37a0  7.4|.j5....|.j7.
-000007a0: 347c 006a 36a1 0101 0074 16a0 30a1 007c  4|.j6....t..0..|
-000007b0: 005f 387c 006a 38a0 347c 006a 33a1 0101  ._8|.j8.4|.j3...
-000007c0: 007c 006a 38a0 347c 006a 37a1 0101 007c  .|.j8.4|.j7....|
-000007d0: 006a 2fa0 347c 006a 38a1 0101 007c 006a  .j/.4|.j8....|.j
-000007e0: 2fa0 1b7c 006a 29a1 0101 007c 006a 1aa0  /..|.j)....|.j..
-000007f0: 3974 016a 3a6a 3b6a 3ca0 3da1 00a1 0101  9t.j:j;j<.=.....
-00000800: 0074 16a0 19a1 007c 005f 3e74 16a0 30a1  .t.....|._>t..0.
-00000810: 007c 005f 3f7c 006a 3fa0 347c 006a 1a64  .|._?|.j?.4|.j.d
-00000820: 17a1 0201 007c 006a 3fa0 347c 006a 2f64  .....|.j?.4|.j/d
-00000830: 02a1 0201 007c 006a 3fa0 347c 006a 3e64  .....|.j?.4|.j>d
+00000620: 1d74 016a 1e6a 1f6a 20a0 21a1 00a1 0101  .t.j.j.j .!.....
+00000630: 007c 006a 1aa0 1b7c 006a 18a1 0101 0074  .|.j...|.j.....t
+00000640: 016a 02a0 22a1 007c 005f 2374 016a 02a0  .j.."..|._#t.j..
+00000650: 24a1 007c 005f 2574 016a 026a 2264 0d64  $..|._%t.j.j"d.d
+00000660: 0d64 0e8d 027c 005f 2674 16a0 2764 0fa1  .d...|._&t..'d..
+00000670: 017c 005f 2874 16a0 2764 10a1 017c 005f  .|._(t..'d...|._
+00000680: 2974 16a0 2764 11a1 017c 005f 2a74 16a0  )t..'d...|._*t..
+00000690: 2764 12a1 017c 005f 2b74 016a 02a0 2c74  'd...|._+t.j..,t
+000006a0: 2da1 017c 005f 2e7c 006a 2ea0 2f74 2d6a  -..|._.|.j../t-j
+000006b0: 3064 13a1 0201 007c 006a 2ea0 2f74 2d6a  0d.....|.j../t-j
+000006c0: 3164 14a1 0201 007c 006a 2ea0 2f74 2d6a  1d.....|.j../t-j
+000006d0: 3264 15a1 0201 007c 006a 2ea0 2f74 2d6a  2d.....|.j../t-j
+000006e0: 3364 16a1 0201 0074 16a0 19a1 007c 005f  3d.....t.....|._
+000006f0: 3474 16a0 35a1 007c 005f 367c 006a 36a0  4t..5..|._6|.j6.
+00000700: 1b7c 006a 25a1 0101 007c 006a 36a0 1b7c  .|.j%....|.j6..|
+00000710: 006a 256a 37a1 0101 0074 16a0 19a1 007c  .j%j7....t.....|
+00000720: 005f 387c 006a 38a0 397c 006a 36a1 0101  ._8|.j8.9|.j6...
+00000730: 007c 006a 38a0 1b7c 006a 28a1 0101 0074  .|.j8..|.j(....t
+00000740: 16a0 19a1 007c 005f 3a7c 006a 3aa0 1b7c  .....|._:|.j:..|
+00000750: 006a 23a1 0101 007c 006a 3aa0 1b7c 006a  .j#....|.j:..|.j
+00000760: 29a1 0101 0074 16a0 19a1 007c 005f 3b7c  )....t.....|._;|
+00000770: 006a 3ba0 1b7c 006a 26a1 0101 007c 006a  .j;..|.j&....|.j
+00000780: 3ba0 1b7c 006a 2aa1 0101 007c 006a 3ba0  ;..|.j*....|.j;.
+00000790: 1b7c 006a 2ba1 0101 0074 16a0 19a1 007c  .|.j+....t.....|
+000007a0: 005f 3c7c 006a 3ca0 397c 006a 3aa1 0101  ._<|.j<.9|.j:...
+000007b0: 007c 006a 3ca0 397c 006a 3ba1 0101 0074  .|.j<.9|.j;....t
+000007c0: 16a0 35a1 007c 005f 3d7c 006a 3da0 397c  ..5..|._=|.j=.9|
+000007d0: 006a 38a1 0101 007c 006a 3da0 397c 006a  .j8....|.j=.9|.j
+000007e0: 3ca1 0101 007c 006a 34a0 397c 006a 3da1  <....|.j4.9|.j=.
+000007f0: 0101 007c 006a 34a0 1b7c 006a 2ea1 0101  ...|.j4..|.j....
+00000800: 0074 16a0 19a1 007c 005f 3e74 16a0 35a1  .t.....|._>t..5.
+00000810: 007c 005f 3f7c 006a 3fa0 397c 006a 1a64  .|._?|.j?.9|.j.d
+00000820: 09a1 0201 007c 006a 3fa0 397c 006a 3464  .....|.j?.9|.j4d
+00000830: 17a1 0201 007c 006a 3fa0 397c 006a 3e64  .....|.j?.9|.j>d
 00000840: 09a1 0201 007c 00a0 407c 006a 3fa1 0101  .....|..@|.j?...
 00000850: 007c 00a0 41a1 0001 007c 00a0 42a1 0001  .|..A....|..B...
 00000860: 007c 00a0 43a1 0001 0064 1853 0029 197a  .|..C....d.S.).z
 00000870: 3820 6372 6561 7465 2068 6572 6520 796f  8 create here yo
 00000880: 7572 2067 7569 2077 6974 6820 616c 6c20  ur gui with all 
 00000890: 636f 6e74 726f 6c73 2061 6e64 2074 6865  controls and the
 000008a0: 6972 206c 6179 6f75 747a 0a49 6d61 6765  ir layoutz.Image
@@ -173,59 +173,59 @@
 00000ac0: 6e65 6c45 6e74 7269 6573 da11 636f 6d62  nelEntries..comb
 00000ad0: 6f5f 6368 616e 6e65 6c5f 6469 7272 0300  o_channel_dirr..
 00000ae0: 0000 da0b 5150 7573 6842 7574 746f 6eda  ....QPushButton.
 00000af0: 1162 7574 746f 6e5f 7374 6172 745f 7374  .button_start_st
 00000b00: 6f70 da0b 5156 426f 784c 6179 6f75 745a  op..QVBoxLayoutZ
 00000b10: 0b6c 6179 6f75 745f 6c65 6674 da09 6164  .layout_left..ad
 00000b20: 6457 6964 6765 74da 0a61 6464 5374 7265  dWidget..addStre
-00000b30: 7463 68da 084e 5346 4368 6172 74da 0a63  tch..NSFChart..c
-00000b40: 6861 7274 5f70 6c6f 74da 0b4e 5346 436f  hart_plot..NSFCo
-00000b50: 6c6f 726d 6170 da0d 636f 6c6f 726d 6170  lormap..colormap
-00000b60: 5f70 6c6f 74da 0973 7065 635f 706c 6f74  _plot..spec_plot
-00000b70: da09 5143 6865 636b 426f 78da 1463 6865  ..QCheckBox..che
-00000b80: 636b 5f73 686f 775f 6869 7374 6f67 7261  ck_show_histogra
-00000b90: 6dda 1363 6865 636b 5f73 686f 775f 6261  m..check_show_ba
-00000ba0: 636b 7761 7264 da15 6368 6563 6b5f 7368  ckward..check_sh
-00000bb0: 6f77 5f70 6f77 6572 5f73 7065 63da 1a63  ow_power_spec..c
-00000bc0: 6865 636b 5f73 686f 775f 636f 6d70 7265  heck_show_compre
-00000bd0: 7373 6564 5f73 7065 63da 114e 5346 4e61  ssed_spec..NSFNa
-00000be0: 6d65 5661 6c75 6554 6162 6c65 7206 0000  meValueTabler...
-00000bf0: 00da 0c74 6162 6c65 5265 7375 6c74 73da  ...tableResults.
-00000c00: 0c64 6566 696e 655f 656e 7472 7972 0e00  .define_entryr..
-00000c10: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00000c20: 005a 0a6c 6179 6f75 745f 6d69 64da 0b51  .Z.layout_mid..Q
-00000c30: 4842 6f78 4c61 796f 7574 5a11 6c61 796f  HBoxLayoutZ.layo
-00000c40: 7574 5f63 6f6c 6f72 5f70 6c6f 74da 0968  ut_color_plot..h
-00000c50: 6973 746f 6772 616d 5a0f 6c61 796f 7574  istogramZ.layout
-00000c60: 5f63 6f6c 6f72 6d61 70da 0961 6464 4c61  _colormap..addLa
-00000c70: 796f 7574 5a11 6c61 796f 7574 5f6c 696e  youtZ.layout_lin
-00000c80: 655f 6368 6172 745a 116c 6179 6f75 745f  e_chartZ.layout_
-00000c90: 7370 6563 5f63 6861 7274 5a0d 6c61 796f  spec_chartZ.layo
-00000ca0: 7574 5f63 6861 7274 735a 0c6c 6179 6f75  ut_chartsZ.layou
-00000cb0: 745f 706c 6f74 73da 0d61 6464 5370 6163  t_plots..addSpac
-00000cc0: 6572 4974 656d da0a 6672 616d 6577 6f72  erItem..framewor
-00000cd0: 6b73 da06 7174 5f61 7070 da07 6170 705f  ks..qt_app..app_
-00000ce0: 6775 69da 0a53 7464 5653 7061 6365 725a  gui..StdVSpacerZ
+00000b30: 7463 68da 0d61 6464 5370 6163 6572 4974  tch..addSpacerIt
+00000b40: 656d da0a 6672 616d 6577 6f72 6b73 da06  em..frameworks..
+00000b50: 7174 5f61 7070 da07 6170 705f 6775 69da  qt_app..app_gui.
+00000b60: 0a53 7464 5653 7061 6365 72da 084e 5346  .StdVSpacer..NSF
+00000b70: 4368 6172 74da 0a63 6861 7274 5f70 6c6f  Chart..chart_plo
+00000b80: 74da 0b4e 5346 436f 6c6f 726d 6170 da0d  t..NSFColormap..
+00000b90: 636f 6c6f 726d 6170 5f70 6c6f 74da 0973  colormap_plot..s
+00000ba0: 7065 635f 706c 6f74 da09 5143 6865 636b  pec_plot..QCheck
+00000bb0: 426f 78da 1463 6865 636b 5f73 686f 775f  Box..check_show_
+00000bc0: 6869 7374 6f67 7261 6dda 1363 6865 636b  histogram..check
+00000bd0: 5f73 686f 775f 6261 636b 7761 7264 da15  _show_backward..
+00000be0: 6368 6563 6b5f 7368 6f77 5f70 6f77 6572  check_show_power
+00000bf0: 5f73 7065 63da 1a63 6865 636b 5f73 686f  _spec..check_sho
+00000c00: 775f 636f 6d70 7265 7373 6564 5f73 7065  w_compressed_spe
+00000c10: 63da 114e 5346 4e61 6d65 5661 6c75 6554  c..NSFNameValueT
+00000c20: 6162 6c65 7206 0000 00da 0c74 6162 6c65  abler......table
+00000c30: 5265 7375 6c74 73da 0c64 6566 696e 655f  Results..define_
+00000c40: 656e 7472 7972 0e00 0000 720f 0000 0072  entryr....r....r
+00000c50: 1000 0000 7211 0000 005a 0a6c 6179 6f75  ....r....Z.layou
+00000c60: 745f 6d69 64da 0b51 4842 6f78 4c61 796f  t_mid..QHBoxLayo
+00000c70: 7574 5a11 6c61 796f 7574 5f63 6f6c 6f72  utZ.layout_color
+00000c80: 5f70 6c6f 74da 0968 6973 746f 6772 616d  _plot..histogram
+00000c90: 5a0f 6c61 796f 7574 5f63 6f6c 6f72 6d61  Z.layout_colorma
+00000ca0: 70da 0961 6464 4c61 796f 7574 5a11 6c61  p..addLayoutZ.la
+00000cb0: 796f 7574 5f6c 696e 655f 6368 6172 745a  yout_line_chartZ
+00000cc0: 116c 6179 6f75 745f 7370 6563 5f63 6861  .layout_spec_cha
+00000cd0: 7274 5a0d 6c61 796f 7574 5f63 6861 7274  rtZ.layout_chart
+00000ce0: 735a 0c6c 6179 6f75 745f 706c 6f74 735a  sZ.layout_plotsZ
 00000cf0: 0c6c 6179 6f75 745f 7269 6768 745a 0d73  .layout_rightZ.s
 00000d00: 6372 6565 6e5f 6c61 796f 7574 da09 7365  creen_layout..se
 00000d10: 744c 6179 6f75 74da 1162 696e 645f 6775  tLayout..bind_gu
 00000d20: 695f 656c 656d 656e 7473 da09 696e 6974  i_elements..init
 00000d30: 5f70 6c6f 74da 1465 6e74 6572 5f67 7569  _plot..enter_gui
 00000d40: 5f73 7461 7465 5f69 646c 6529 0272 1b00  _state_idle).r..
 00000d50: 0000 7204 0000 0072 1200 0000 7212 0000  ..r....r....r...
 00000d60: 0072 1300 0000 da0f 646f 5f73 6574 7570  .r......do_setup
 00000d70: 5f73 6372 6565 6e26 0000 0073 8a00 0000  _screen&...s....
 00000d80: 0002 0604 0e01 0c01 1401 0c01 0e02 0e01  ................
 00000d90: 0c01 1401 0c01 0e02 0e01 0c01 1401 0c01  ................
 00000da0: 0e02 1002 0c02 0a01 0e01 0e01 0e01 0e01  ................
-00000db0: 0a01 0e03 0c01 0c01 1202 0c01 0c01 0c01  ................
-00000dc0: 0c01 0e01 1001 1001 1001 1002 0a01 0a01  ................
-00000dd0: 0e01 1001 0a01 0e01 0e02 0a01 0e01 0e01  ................
-00000de0: 0a01 0e01 0e01 0e01 0a01 0e01 0e01 0a01  ................
-00000df0: 0e01 0e01 0e01 0e02 1604 0a03 0a02 1001  ................
+00000db0: 0a01 1601 0e03 0c01 0c01 1202 0c01 0c01  ................
+00000dc0: 0c01 0c01 0e01 1001 1001 1001 1002 0a01  ................
+00000dd0: 0a01 0e01 1001 0a01 0e01 0e02 0a01 0e01  ................
+00000de0: 0e01 0a01 0e01 0e01 0e01 0a01 0e01 0e01  ................
+00000df0: 0a01 0e01 0e01 0e01 0e05 0a03 0a02 1001  ................
 00000e00: 1001 1001 0c02 0801 0801 7a1a 5363 616e  ..........z.Scan
 00000e10: 5363 7265 656e 2e64 6f5f 7365 7475 705f  Screen.do_setup_
 00000e20: 7363 7265 656e 6301 0000 0000 0000 0000  screenc.........
 00000e30: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
 00000e40: 4e01 0000 7400 6a01 a002 7c00 6a03 7c00  N...t.j...|.j.|.
 00000e50: 6a04 6a05 6a06 a102 0100 7400 6a01 a002  j.j.j.....t.j...
 00000e60: 7c00 6a07 7c00 6a04 6a05 6a08 a102 0100  |.j.|.j.j.j.....
@@ -255,19 +255,19 @@
 00000fe0: 654e 2928 7221 0000 0072 2200 0000 da13  eN)(r!...r".....
 00000ff0: 636f 6e6e 6563 745f 746f 5f70 726f 7065  connect_to_prope
 00001000: 7274 7972 3500 0000 7204 0000 0072 0500  rtyr5...r....r..
 00001010: 0000 da0a 6368 616e 6e65 6c5f 6964 7224  ....channel_idr$
 00001020: 0000 00da 0a69 6d61 6765 5f73 697a 6572  .....image_sizer
 00001030: 2e00 0000 da0d 7469 6d65 5f70 6572 5f6c  ......time_per_l
 00001040: 696e 6572 3100 0000 da0f 706f 696e 7473  iner1.....points
-00001050: 5f70 6572 5f6c 696e 6572 4200 0000 da0d  _per_linerB.....
-00001060: 7368 6f77 5f62 6163 6b77 6172 6472 4300  show_backwardrC.
+00001050: 5f70 6572 5f6c 696e 6572 4700 0000 da0d  _per_linerG.....
+00001060: 7368 6f77 5f62 6163 6b77 6172 6472 4800  show_backwardrH.
 00001070: 0000 da0f 7368 6f77 5f70 6f77 6572 5f73  ....show_power_s
-00001080: 7065 6372 4400 0000 da12 7368 6f77 5f63  pecrD.....show_c
-00001090: 6f6d 7072 6573 735f 7370 6563 7241 0000  ompress_specrA..
+00001080: 7065 6372 4900 0000 da12 7368 6f77 5f63  pecrI.....show_c
+00001090: 6f6d 7072 6573 735f 7370 6563 7246 0000  ompress_specrF..
 000010a0: 00da 0c73 7461 7465 4368 616e 6765 64da  ...stateChanged.
 000010b0: 0763 6f6e 6e65 6374 da17 5f73 686f 775f  .connect.._show_
 000010c0: 6869 7374 6f67 7261 6d5f 636c 6963 6b65  histogram_clicke
 000010d0: 64da 165f 7368 6f77 5f62 6163 6b77 6172  d.._show_backwar
 000010e0: 645f 636c 6963 6b65 64da 185f 7368 6f77  d_clicked.._show
 000010f0: 5f70 6f77 6572 5f73 7065 635f 636c 6963  _power_spec_clic
 00001100: 6b65 64da 1d5f 7368 6f77 5f63 6f6d 7072  ked.._show_compr
@@ -331,26 +331,26 @@
 000014a0: 7a06 592d 4178 6973 7201 0000 007a 1543  z.Y-Axisr....z.C
 000014b0: 7572 7265 6e74 206c 696e 6520 6368 6172  urrent line char
 000014c0: 7420 2d20 da04 4461 7461 7a0e 5370 6563  t - ..Dataz.Spec
 000014d0: 7472 756d 206f 6620 2d20 5a03 4672 71da  trum of - Z.Frq.
 000014e0: 0248 7ada 0941 6d70 6c69 7475 6465 da00  .Hz..Amplitude..
 000014f0: 291d 7235 0000 00da 0a65 6e74 7279 5f6e  ).r5.....entry_n
 00001500: 616d 6572 0400 0000 7205 0000 0072 5600  amer....r....rV.
-00001510: 0000 da05 7661 6c75 6572 3e00 0000 da09  ....valuer>.....
+00001510: 0000 da05 7661 6c75 6572 4300 0000 da09  ....valuerC.....
 00001520: 7365 745f 7469 746c 65da 0973 6574 5f6c  set_title..set_l
-00001530: 6162 656c 7221 0000 0072 2200 0000 723d  abelr!...r"...r=
+00001530: 6162 656c 7221 0000 0072 2200 0000 7242  abelr!...r"...rB
 00001540: 0000 00da 0441 7869 73da 0662 6f74 746f  .....Axis..botto
 00001550: 6dda 0873 6574 5f75 6e69 74da 046c 6566  m..set_unit..lef
 00001560: 74da 017a da02 6e70 da08 6c69 6e73 7061  t..z..np..linspa
 00001570: 6365 7257 0000 0072 5900 0000 da0c 7365  cerW...rY.....se
 00001580: 745f 7879 5f72 616e 6765 da0f 7365 745f  t_xy_range..set_
-00001590: 6461 7461 5f70 6f69 6e74 7372 3c00 0000  data_pointsr<...
-000015a0: 723b 0000 00da 0470 6c6f 74da 0973 6574  r;.....plot..set
+00001590: 6461 7461 5f70 6f69 6e74 7372 4100 0000  data_pointsrA...
+000015a0: 7240 0000 00da 0470 6c6f 74da 0973 6574  r@.....plot..set
 000015b0: 5852 616e 6765 da0b 636c 6561 725f 706c  XRange..clear_pl
-000015c0: 6f74 7372 3f00 0000 2903 721b 0000 005a  otsr?...).r....Z
+000015c0: 6f74 7372 4400 0000 2903 721b 0000 005a  otsrD...).r....Z
 000015d0: 0c63 6861 6e6e 656c 5f6e 616d 655a 0973  .channel_nameZ.s
 000015e0: 6361 6e5f 6c69 6e65 7212 0000 0072 1200  can_liner....r..
 000015f0: 0000 7213 0000 0072 5200 0000 9f00 0000  ..r....rR.......
 00001600: 732e 0000 0000 0114 0212 0116 0116 0116  s...............
 00001610: 0116 0116 021e 010e 011e 0212 0116 0116  ................
 00001620: 0116 0116 0118 010a 0212 0116 0116 0116  ................
 00001630: 0116 017a 1453 6361 6e53 6372 6565 6e2e  ...z.ScanScreen.
@@ -368,16 +368,16 @@
 000016f0: 5363 7265 656e 2e6f 6e5f 6275 7474 6f6e  Screen.on_button
 00001700: 5f73 7461 7274 5f73 746f 705f 636c 6963  _start_stop_clic
 00001710: 6b65 6463 0100 0000 0000 0000 0000 0000  kedc............
 00001720: 0100 0000 0200 0000 4300 0000 7328 0000  ........C...s(..
 00001730: 007c 006a 00a0 01a1 0072 187c 006a 026a  .|.j.....r.|.j.j
 00001740: 03a0 04a1 0001 006e 0c7c 006a 026a 03a0  .......n.|.j.j..
 00001750: 05a1 0001 0064 0053 0072 1700 0000 2906  .....d.S.r....).
-00001760: 7241 0000 00da 0969 7343 6865 636b 6564  rA.....isChecked
-00001770: 723e 0000 0072 4900 0000 da04 7368 6f77  r>...rI.....show
+00001760: 7246 0000 00da 0969 7343 6865 636b 6564  rF.....isChecked
+00001770: 7243 0000 0072 4e00 0000 da04 7368 6f77  rC...rN.....show
 00001780: da04 6869 6465 721a 0000 0072 1200 0000  ..hider....r....
 00001790: 7212 0000 0072 1300 0000 725f 0000 00c2  r....r....r_....
 000017a0: 0000 0073 0600 0000 0001 0a01 0e02 7a22  ...s..........z"
 000017b0: 5363 616e 5363 7265 656e 2e5f 7368 6f77  ScanScreen._show
 000017c0: 5f68 6973 746f 6772 616d 5f63 6c69 636b  _histogram_click
 000017d0: 6564 6301 0000 0000 0000 0000 0000 0001  edc.............
 000017e0: 0000 0002 0000 0043 0000 0073 0c00 0000  .......C...s....
@@ -478,28 +478,28 @@
 00001dd0: 0072 1300 0000 726c 0000 00ec 0000 0073  .r....rl.......s
 00001de0: 0400 0000 0001 0801 7a18 5363 616e 5363  ........z.ScanSc
 00001df0: 7265 656e 2e73 686f 775f 6e65 775f 6461  reen.show_new_da
 00001e00: 7461 6301 0000 0000 0000 0000 0000 0001  tac.............
 00001e10: 0000 0002 0000 0043 0000 0073 1800 0000  .......C...s....
 00001e20: 7c00 6a00 a001 a100 0100 7c00 6a02 a003  |.j.......|.j...
 00001e30: a100 0100 6400 5300 7217 0000 0029 0472  ....d.S.r....).r
-00001e40: 3c00 0000 7283 0000 0072 4600 0000 da0c  <...r....rF.....
+00001e40: 4100 0000 7283 0000 0072 4b00 0000 da0c  A...r....rK.....
 00001e50: 636c 6561 725f 7661 6c75 6573 721a 0000  clear_valuesr...
 00001e60: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
 00001e70: 726e 0000 00f0 0000 0073 0400 0000 0001  rn.......s......
 00001e80: 0a01 7a1b 5363 616e 5363 7265 656e 2e73  ..z.ScanScreen.s
 00001e90: 6574 5f64 6174 615f 696e 7661 6c69 6463  et_data_invalidc
 00001ea0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
 00001eb0: 0600 0000 4300 0000 7326 0000 007c 006a  ....C...s&...|.j
 00001ec0: 00a0 01a1 007d 017c 006a 026a 0374 046a  .....}.|.j.j.t.j
 00001ed0: 057c 016a 0664 0164 0264 038d 0401 0064  .|.j.d.d.d.....d
 00001ee0: 0053 0029 044e 7273 0000 0072 0100 0000  .S.).Nrs...r....
 00001ef0: 2901 da09 7072 6563 6973 696f 6e29 0772  )...precision).r
 00001f00: 0400 0000 da11 6765 745f 776f 726b 6572  ......get_worker
-00001f10: 5f72 6573 756c 7472 4600 0000 da09 7365  _resultrF.....se
+00001f10: 5f72 6573 756c 7472 4b00 0000 da09 7365  _resultrK.....se
 00001f20: 745f 7661 6c75 6572 0600 0000 720e 0000  t_valuer....r...
 00001f30: 00da 0f73 6361 6e5f 6c69 6e65 5f69 6e64  ...scan_line_ind
 00001f40: 6578 2902 721b 0000 00da 0372 6573 7212  ex).r......resr.
 00001f50: 0000 0072 1200 0000 7213 0000 0072 9600  ...r....r....r..
 00001f60: 0000 f400 0000 7304 0000 0000 010a 017a  ......s........z
 00001f70: 1853 6361 6e53 6372 6565 6e2e 7570 6461  .ScanScreen.upda
 00001f80: 7465 5f72 6573 756c 7463 0100 0000 0000  te_resultc......
@@ -544,24 +544,24 @@
 000021f0: 7374 636f 6d70 3e15 0100 00f3 0000 0000  stcomp>.........
 00002200: 7a2a 5363 616e 5363 7265 656e 2e75 7064  z*ScanScreen.upd
 00002210: 6174 655f 706c 6f74 2e3c 6c6f 6361 6c73  ate_plot.<locals
 00002220: 3e2e 3c6c 6973 7463 6f6d 703e 2903 da01  >.<listcomp>)...
 00002230: 79da 0178 729d 0000 0029 2472 0400 0000  y..xr....)$r....
 00002240: 7299 0000 00da 0673 7472 6561 6dda 1167  r......stream..g
 00002250: 6574 5f73 7472 6561 6d5f 6c65 6e67 7468  et_stream_length
-00002260: 723e 0000 00da 0c70 6c6f 745f 6368 616e  r>.....plot_chan
+00002260: 7243 0000 00da 0c70 6c6f 745f 6368 616e  rC.....plot_chan
 00002270: 6e65 6cda 0b67 6574 5f63 6861 6e6e 656c  nel..get_channel
-00002280: 729b 0000 0072 3c00 0000 da0b 706c 6f74  r....r<.....plot
+00002280: 729b 0000 0072 4100 0000 da0b 706c 6f74  r....rA.....plot
 00002290: 5f73 7472 6561 6d72 0500 0000 725a 0000  _streamr....rZ..
 000022a0: 0072 7500 0000 da09 706c 6f74 5f64 6174  .ru.....plot_dat
 000022b0: 6172 5b00 0000 725c 0000 0072 5800 0000  ar[...r\...rX...
 000022c0: 7221 0000 00da 0873 6369 5f6d 6174 68da  r!.....sci_math.
 000022d0: 0863 616c 635f 6666 74da 1166 696e 645f  .calc_fft..find_
-000022e0: 6869 6768 6573 745f 7065 616b 723f 0000  highest_peakr?..
-000022f0: 00da 0a73 6574 5f6d 6172 6b65 7272 4600  ...set_markerrF.
+000022e0: 6869 6768 6573 745f 7065 616b 7244 0000  highest_peakrD..
+000022f0: 00da 0a73 6574 5f6d 6172 6b65 7272 4b00  ...set_markerrK.
 00002300: 0000 729a 0000 0072 0600 0000 720f 0000  ..r....r....r...
 00002310: 00da 0f67 6574 5f73 7472 6561 6d5f 756e  ...get_stream_un
 00002320: 6974 7210 0000 00da 0475 6e69 74da 0c63  itr......unit..c
 00002330: 6c65 6172 5f6d 6172 6b65 72da 0b63 6c65  lear_marker..cle
 00002340: 6172 5f76 616c 7565 da0f 6765 745f 6e6f  ar_value..get_no
 00002350: 6973 655f 666c 6f6f 72da 0572 616e 6765  ise_floor..range
 00002360: da10 6765 745f 7374 7265 616d 5f72 616e  ..get_stream_ran
@@ -602,14 +602,14 @@
 00002590: 2200 0000 da0d 5461 626c 6545 6e74 7279  ".....TableEntry
 000025a0: 4944 7372 0600 0000 da0d 4e53 4643 6f6d  IDsr......NSFCom
 000025b0: 626f 456e 7472 79da 0843 6861 6e6e 656c  boEntry..Channel
 000025c0: 4472 1400 0000 7215 0000 0072 3400 0000  Dr....r....r4...
 000025d0: 7228 0000 0072 2900 0000 722a 0000 0072  r(...r)...r*...r
 000025e0: 3000 0000 7232 0000 00da 056d 696c 6c69  0...r2.....milli
 000025f0: 722f 0000 0072 2b00 0000 da04 6e61 6e6f  r/...r+.....nano
-00002600: 7226 0000 0072 4c00 0000 724d 0000 00da  r&...rL...rM....
+00002600: 7226 0000 0072 3c00 0000 723d 0000 00da  r&...r<...r=....
 00002610: 0c4d 6f64 756c 6553 6372 6565 6e72 1600  .ModuleScreenr..
 00002620: 0000 7212 0000 0072 1200 0000 7212 0000  ..r....r....r...
 00002630: 0072 1300 0000 da08 3c6d 6f64 756c 653e  .r......<module>
 00002640: 0100 0000 731e 0000 0004 0408 020c 0106  ....s...........
 00002650: 010e 020c 0208 0110 0214 0810 0110 fe04  ................
 00002660: 060e 0118 0122 02                        .....".
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/imaging_task.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/imaging_task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/imaging_task.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/imaging_task.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 09:25:17 2023 UTC, .py size: 4907 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 fd1b 3964 2b13 0000  a.........9d+...
+00000000: 610d 0d0a 0000 0000 5a4d 3964 2b13 0000  a.......ZM9d+...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6505 8300 7238 6401 6405 6c06 6d07  ..e...r8d.d.l.m.
 00000060: 5a07 0100 6e0c 6401 6405 6c08 6d07 5a07  Z...n.d.d.l.m.Z.
 00000070: 0100 6401 6402 6c09 5a0a 6401 6406 6c0b  ..d.d.l.Z.d.d.l.
@@ -29,15 +29,15 @@
 000001c0: 4461 7461 e902 0000 0029 01da 0863 6861  Data.....)...cha
 000001d0: 6e6e 656c 73e9 ffff ffff 4e29 07da 085f  nnels.....N)..._
 000001e0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
 000001f0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
 00000200: 5fda 036e 7366 da09 5363 6953 7472 6561  _..nsf..SciStrea
 00000210: 6dda 0673 7472 6561 6dda 0f73 6361 6e5f  m..stream..scan_
 00000220: 6c69 6e65 5f69 6e64 6578 a900 7211 0000  line_index..r...
-00000230: 0072 1100 0000 fa62 633a 5c47 6974 5c73  .r.....bc:\Git\s
+00000230: 0072 1100 0000 fa62 433a 5c47 6974 5c73  .r.....bC:\Git\s
 00000240: 6372 6970 7473 5f70 7974 686f 6e5f 6c69  cripts_python_li
 00000250: 625c 6e61 6e6f 7375 7266 5c61 7070 5c61  b\nanosurf\app\a
 00000260: 7070 5f64 656d 6f5f 7363 616e 6e69 6e67  pp_demo_scanning
 00000270: 5f61 6e64 5f6c 6962 5f75 7361 6765 5c73  _and_lib_usage\s
 00000280: 6361 6e5f 6d6f 6475 6c65 5c69 6d61 6769  can_module\imagi
 00000290: 6e67 5f74 6173 6b2e 7079 7206 0000 0010  ng_task.pyr.....
 000002a0: 0000 0073 0400 0000 0802 0c01 7206 0000  ...s........r...
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/module.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/module.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/module.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/module.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 09:26:11 2023 UTC, .py size: 5067 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 331c 3964 cb13 0000  a.......3.9d....
+00000000: 610d 0d0a 0000 0000 5a4d 3964 cb13 0000  a.......ZM9d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6502  Z.d.d.l.m.Z...e.
 00000040: 8300 7224 6401 6403 6c03 6d04 5a04 0100  ..r$d.d.l.m.Z...
 00000050: 6e0c 6401 6403 6c05 6d04 5a04 0100 6401  n.d.d.l.m.Z...d.
 00000060: 6404 6c06 5a07 6401 6405 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 6d0a 5a0a 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
@@ -40,15 +40,15 @@
 00000270: 0100 7402 a003 a100 7c00 5f02 7402 a004  ..t.....|._.t...
 00000280: a100 7c00 5f05 6400 5300 a901 4e29 06da  ..|._.d.S...N)..
 00000290: 0573 7570 6572 da08 5f5f 696e 6974 5f5f  .super..__init__
 000002a0: 7205 0000 005a 0c53 6361 6e53 6574 7469  r....Z.ScanSetti
 000002b0: 6e67 73da 0b53 6361 6e52 6573 756c 7473  ngs..ScanResults
 000002c0: da06 7265 7375 6c74 2903 da04 7365 6c66  ..result)...self
 000002d0: 7207 0000 00da 0367 7569 a901 da09 5f5f  r......gui....__
-000002e0: 636c 6173 735f 5fa9 00fa 5c63 3a5c 4769  class__...\c:\Gi
+000002e0: 636c 6173 735f 5fa9 00fa 5c43 3a5c 4769  class__...\C:\Gi
 000002f0: 745c 7363 7269 7074 735f 7079 7468 6f6e  t\scripts_python
 00000300: 5f6c 6962 5c6e 616e 6f73 7572 665c 6170  _lib\nanosurf\ap
 00000310: 705c 6170 705f 6465 6d6f 5f73 6361 6e6e  p\app_demo_scann
 00000320: 696e 675f 616e 645f 6c69 625f 7573 6167  ing_and_lib_usag
 00000330: 655c 7363 616e 5f6d 6f64 756c 655c 6d6f  e\scan_module\mo
 00000340: 6475 6c65 2e70 7972 0a00 0000 1a00 0000  dule.pyr........
 00000350: 7308 0000 0000 010e 0204 010a 017a 1353  s............z.S
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/settings.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/settings.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/settings.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 08:58:56 2023 UTC, .py size: 1310 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,111 +1,131 @@
-00000000: 610d 0d0a 0000 0000 d015 3964 1e05 0000  a.........9d....
+00000000: 610d 0d0a 0000 0000 bc06 5a64 ac05 0000  a.........Zd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a04 6401  m.Z...d.d.l.Z.d.
 00000050: 6402 6c05 6d06 0200 0100 6d07 0200 0100  d.l.m.....m.....
 00000060: 6d08 5a08 0100 6401 6402 6c09 6d06 0200  m.Z...d.d.l.m...
-00000070: 0100 6d07 0200 0100 6d0a 5a0a 0100 6503  ..m.....m.Z...e.
-00000080: 4700 6404 6405 8400 6405 650a 6a0b 8303  G.d.d...d.e.j...
-00000090: 8301 5a0c 6503 4700 6406 6407 8400 6407  ..Z.e.G.d.d...d.
-000000a0: 8302 8301 5a0d 4700 6408 6409 8400 6409  ....Z.G.d.d...d.
-000000b0: 6501 6a0e 8303 5a0f 6402 5300 290a 7abc  e.j...Z.d.S.).z.
-000000c0: 2044 6566 696e 6573 2074 6865 2063 6f6e   Defines the con
-000000d0: 6669 6775 7261 7469 6f6e 2076 616c 7565  figuration value
-000000e0: 7320 6f66 2074 6865 206d 6f64 756c 652e  s of the module.
-000000f0: 0a20 2020 2056 616c 7565 7320 696e 2074  .    Values in t
-00000100: 6865 2050 726f 5374 6f72 6520 6172 6520  he ProStore are 
-00000110: 7361 7665 6420 616e 6420 6c6f 6164 6564  saved and loaded
-00000120: 2064 7572 696e 6720 6170 706c 6963 6174   during applicat
-00000130: 696f 6e20 7374 6172 7475 702f 7368 7574  ion startup/shut
-00000140: 646f 776e 2061 7574 6f6d 6174 6963 616c  down automatical
-00000150: 6c79 0a43 6f70 7972 6967 6874 204e 616e  ly.Copyright Nan
-00000160: 6f73 7572 6620 4147 2032 3032 310a 4c69  osurf AG 2021.Li
-00000170: 6365 6e73 6520 2d20 4d49 540a e900 0000  cense - MIT.....
-00000180: 004e 2901 da09 6461 7461 636c 6173 7363  .N)...dataclassc
-00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001a0: 0600 0000 4000 0000 7380 0000 0065 005a  ....@...s....e.Z
-000001b0: 0164 005a 0264 015a 0365 04a0 0565 06a0  .d.Z.d.Z.e...e..
-000001c0: 0764 0264 03a1 02a1 015a 0865 04a0 0565  .d.d.....Z.e...e
-000001d0: 06a0 0764 0464 05a1 02a1 015a 0965 04a0  ...d.d.....Z.e..
-000001e0: 0565 0a64 0683 01a1 015a 0b65 04a0 0565  .e.d.....Z.e...e
-000001f0: 0a65 0c6a 0d6a 0e6a 0f83 01a1 015a 1065  .e.j.j.j.....Z.e
-00000200: 04a0 0565 1164 0783 01a1 015a 1265 04a0  ...e.d.....Z.e..
-00000210: 0565 1164 0783 01a1 015a 1365 04a0 0565  .e.d.....Z.e...e
-00000220: 1164 0883 01a1 015a 1464 0953 0029 0ada  .d.....Z.d.S.)..
-00000230: 0c53 6361 6e53 6574 7469 6e67 737a 8520  .ScanSettingsz. 
-00000240: 7365 7474 696e 6773 2064 6566 696e 6564  settings defined
-00000250: 2068 6572 6520 6173 2050 726f 7056 616c   here as PropVal
-00000260: 2061 7265 2073 746f 7265 6420 7065 7273   are stored pers
-00000270: 6973 7465 6e74 6c79 2069 6e20 6120 696e  istently in a in
-00000280: 692d 6669 6c65 0a20 2020 2020 2020 2073  i-file.        s
-00000290: 6574 7469 6e67 7320 7769 7468 2061 2027  ettings with a '
-000002a0: 5f27 2061 7320 6669 7273 7420 6368 6172  _' as first char
-000002b0: 2061 7265 206e 6f74 2073 746f 7265 640a   are not stored.
-000002c0: 2020 2020 67f1 68e3 88b5 f8e4 3eda 016d      g.h.....>..m
-000002d0: 679a 9999 9999 99c9 3fda 0173 e900 0100  g.......?..s....
-000002e0: 0054 464e 2915 da08 5f5f 6e61 6d65 5f5f  .TFN)...__name__
-000002f0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000300: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
-00000310: 635f 5fda 0870 726f 705f 7661 6cda 0750  c__..prop_val..P
-00000320: 726f 7056 616c da07 7363 695f 7661 6cda  ropVal..sci_val.
-00000330: 0653 6369 5661 6cda 0a69 6d61 6765 5f73  .SciVal..image_s
-00000340: 697a 65da 0d74 696d 655f 7065 725f 6c69  ize..time_per_li
-00000350: 6e65 da03 696e 74da 0f70 6f69 6e74 735f  ne..int..points_
-00000360: 7065 725f 6c69 6e65 da08 6e61 6e6f 7375  per_line..nanosu
-00000370: 7266 da03 5370 6dda 0b53 6361 6e43 6861  rf..Spm..ScanCha
-00000380: 6e6e 656c da15 4465 666c 6563 7469 6f6e  nnel..Deflection
-00000390: 5f6f 725f 5a43 7472 6c49 6eda 0a63 6861  _or_ZCtrlIn..cha
-000003a0: 6e6e 656c 5f69 64da 0462 6f6f 6cda 0d73  nnel_id..bool..s
-000003b0: 686f 775f 6261 636b 7761 7264 5a0f 7368  how_backwardZ.sh
-000003c0: 6f77 5f70 6f77 6572 5f73 7065 635a 1273  ow_power_specZ.s
-000003d0: 686f 775f 636f 6d70 7265 7373 5f73 7065  how_compress_spe
-000003e0: 63a9 0072 1a00 0000 721a 0000 00fa 5e43  c..r....r.....^C
-000003f0: 3a5c 4769 745c 7363 7269 7074 735f 7079  :\Git\scripts_py
-00000400: 7468 6f6e 5f6c 6962 5c6e 616e 6f73 7572  thon_lib\nanosur
-00000410: 665c 6170 705c 6170 705f 6465 6d6f 5f73  f\app\app_demo_s
-00000420: 6361 6e6e 696e 675f 616e 645f 6c69 625f  canning_and_lib_
-00000430: 7573 6167 655c 7363 616e 5f6d 6f64 756c  usage\scan_modul
-00000440: 655c 7365 7474 696e 6773 2e70 7972 0300  e\settings.pyr..
-00000450: 0000 0d00 0000 7310 0000 0008 0204 0312  ......s.........
-00000460: 0112 010e 0114 010e 010e 0172 0300 0000  ...........r....
-00000470: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000480: 0001 0000 0040 0000 0073 1400 0000 6500  .....@...s....e.
-00000490: 5a01 6400 5a02 6401 5a03 6402 5a04 6403  Z.d.Z.d.Z.d.Z.d.
-000004a0: 5300 2904 da0b 5363 616e 5265 7375 6c74  S.)...ScanResult
-000004b0: 737a 5720 5468 6973 2063 6c61 7373 2073  szW This class s
-000004c0: 6176 6573 2074 6865 2077 6f72 6b65 7220  aves the worker 
-000004d0: 7461 736b 2072 6573 756c 7420 2865 2e67  task result (e.g
-000004e0: 2062 6520 7265 6164 2062 7920 6775 6920   be read by gui 
-000004f0: 656c 656d 656e 7473 206f 7220 7361 7665  elements or save
-00000500: 6420 746f 2066 696c 6520 7201 0000 004e  d to file r....N
-00000510: 2905 7207 0000 0072 0800 0000 7209 0000  ).r....r....r...
-00000520: 0072 0a00 0000 5a17 6375 7272 656e 745f  .r....Z.current_
-00000530: 7363 616e 5f6c 696e 655f 696e 6465 7872  scan_line_indexr
-00000540: 1a00 0000 721a 0000 0072 1a00 0000 721b  ....r....r....r.
-00000550: 0000 0072 1c00 0000 1a00 0000 7304 0000  ...r........s...
-00000560: 0008 0204 0172 1c00 0000 6300 0000 0000  .....r....c.....
-00000570: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-00000580: 0000 0073 1400 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00000590: 6401 5a03 6402 5a04 6403 5300 2904 da08  d.Z.d.Z.d.S.)...
-000005a0: 4368 616e 6e65 6c44 2901 7201 0000 0029  ChannelD).r....)
-000005b0: 01e9 0100 0000 4e29 0572 0700 0000 7208  ......N).r....r.
-000005c0: 0000 0072 0900 0000 da0a 4465 666c 6563  ...r......Deflec
-000005d0: 7469 6f6e da0a 546f 706f 6772 6170 6879  tion..Topography
-000005e0: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
-000005f0: 1b00 0000 721d 0000 0020 0000 0073 0400  ....r.... ...s..
-00000600: 0000 0801 0401 721d 0000 0029 1072 0a00  ......r....).r..
-00000610: 0000 da04 656e 756d da0b 6461 7461 636c  ....enum..datacl
-00000620: 6173 7365 7372 0200 0000 7213 0000 00da  assesr....r.....
-00000630: 1e6e 616e 6f73 7572 662e 6c69 622e 6461  .nanosurf.lib.da
-00000640: 7461 7479 7065 732e 7363 695f 7661 6cda  tatypes.sci_val.
-00000650: 036c 6962 da09 6461 7461 7479 7065 7372  .lib..datatypesr
-00000660: 0d00 0000 da1f 6e61 6e6f 7375 7266 2e6c  ......nanosurf.l
-00000670: 6962 2e64 6174 6174 7970 6573 2e70 726f  ib.datatypes.pro
-00000680: 705f 7661 6c72 0b00 0000 da09 5072 6f70  p_valr......Prop
-00000690: 5374 6f72 6572 0300 0000 721c 0000 00da  Storer....r.....
-000006a0: 0749 6e74 456e 756d 721d 0000 0072 1a00  .IntEnumr....r..
-000006b0: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-000006c0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000006d0: 1400 0000 0406 0801 0c01 0801 1801 1802  ................
-000006e0: 0201 140c 0201 1005                      ........
+00000070: 0100 6d07 0200 0100 6d0a 5a0a 0100 4700  ..m.....m.Z...G.
+00000080: 6404 6405 8400 6405 650a 6a0b 8303 5a0c  d.d...d.e.j...Z.
+00000090: 4700 6406 6407 8400 6407 8302 5a0d 4700  G.d.d...d...Z.G.
+000000a0: 6408 6409 8400 6409 6501 6a0e 8303 5a0f  d.d...d.e.j...Z.
+000000b0: 6402 5300 290a 7abc 2044 6566 696e 6573  d.S.).z. Defines
+000000c0: 2074 6865 2063 6f6e 6669 6775 7261 7469   the configurati
+000000d0: 6f6e 2076 616c 7565 7320 6f66 2074 6865  on values of the
+000000e0: 206d 6f64 756c 652e 0a20 2020 2056 616c   module..    Val
+000000f0: 7565 7320 696e 2074 6865 2050 726f 5374  ues in the ProSt
+00000100: 6f72 6520 6172 6520 7361 7665 6420 616e  ore are saved an
+00000110: 6420 6c6f 6164 6564 2064 7572 696e 6720  d loaded during 
+00000120: 6170 706c 6963 6174 696f 6e20 7374 6172  application star
+00000130: 7475 702f 7368 7574 646f 776e 2061 7574  tup/shutdown aut
+00000140: 6f6d 6174 6963 616c 6c79 0a43 6f70 7972  omatically.Copyr
+00000150: 6967 6874 204e 616e 6f73 7572 6620 4147  ight Nanosurf AG
+00000160: 2032 3032 310a 4c69 6365 6e73 6520 2d20   2021.License - 
+00000170: 4d49 540a e900 0000 004e 2901 da09 6461  MIT......N)...da
+00000180: 7461 636c 6173 7363 0000 0000 0000 0000  taclassc........
+00000190: 0000 0000 0000 0000 0400 0000 0000 0000  ................
+000001a0: 7326 0000 0065 005a 0164 005a 0264 015a  s&...e.Z.d.Z.d.Z
+000001b0: 0364 0264 039c 0187 0066 0164 0464 0584  .d.d.....f.d.d..
+000001c0: 0c5a 0487 0004 005a 0553 0029 06da 0c53  .Z.....Z.S.)...S
+000001d0: 6361 6e53 6574 7469 6e67 737a 8520 7365  canSettingsz. se
+000001e0: 7474 696e 6773 2064 6566 696e 6564 2068  ttings defined h
+000001f0: 6572 6520 6173 2050 726f 7056 616c 2061  ere as PropVal a
+00000200: 7265 2073 746f 7265 6420 7065 7273 6973  re stored persis
+00000210: 7465 6e74 6c79 2069 6e20 6120 696e 692d  tently in a ini-
+00000220: 6669 6c65 0a20 2020 2020 2020 2073 6574  file.        set
+00000230: 7469 6e67 7320 7769 7468 2061 2027 5f27  tings with a '_'
+00000240: 2061 7320 6669 7273 7420 6368 6172 2061   as first char a
+00000250: 7265 206e 6f74 2073 746f 7265 640a 2020  re not stored.  
+00000260: 2020 4ea9 01da 0672 6574 7572 6e63 0100    N....returnc..
+00000270: 0000 0000 0000 0000 0000 0100 0000 0600  ................
+00000280: 0000 0300 0000 738c 0000 0074 0083 00a0  ......s....t....
+00000290: 01a1 0001 0074 02a0 0374 04a0 0564 0164  .....t...t...d.d
+000002a0: 02a1 02a1 017c 005f 0674 02a0 0374 04a0  .....|._.t...t..
+000002b0: 0564 0364 04a1 02a1 017c 005f 0774 02a0  .d.d.....|._.t..
+000002c0: 0374 0864 0583 01a1 017c 005f 0974 02a0  .t.d.....|._.t..
+000002d0: 0374 0874 0a6a 0b6a 0c6a 0d83 01a1 017c  .t.t.j.j.j.....|
+000002e0: 005f 0e74 02a0 0374 0f64 0683 01a1 017c  ._.t...t.d.....|
+000002f0: 005f 1074 02a0 0374 0f64 0683 01a1 017c  ._.t...t.d.....|
+00000300: 005f 1174 02a0 0374 0f64 0783 01a1 017c  ._.t...t.d.....|
+00000310: 005f 1264 0053 0029 084e 67f1 68e3 88b5  ._.d.S.).Ng.h...
+00000320: f8e4 3eda 016d 679a 9999 9999 99c9 3fda  ..>..mg.......?.
+00000330: 0173 e900 0100 0054 4629 13da 0573 7570  .s.....TF)...sup
+00000340: 6572 da08 5f5f 696e 6974 5f5f da08 7072  er..__init__..pr
+00000350: 6f70 5f76 616c da07 5072 6f70 5661 6cda  op_val..PropVal.
+00000360: 0773 6369 5f76 616c da06 5363 6956 616c  .sci_val..SciVal
+00000370: da0a 696d 6167 655f 7369 7a65 da0d 7469  ..image_size..ti
+00000380: 6d65 5f70 6572 5f6c 696e 65da 0369 6e74  me_per_line..int
+00000390: da0f 706f 696e 7473 5f70 6572 5f6c 696e  ..points_per_lin
+000003a0: 65da 086e 616e 6f73 7572 66da 0353 706d  e..nanosurf..Spm
+000003b0: da0b 5363 616e 4368 616e 6e65 6cda 1544  ..ScanChannel..D
+000003c0: 6566 6c65 6374 696f 6e5f 6f72 5f5a 4374  eflection_or_ZCt
+000003d0: 726c 496e da0a 6368 616e 6e65 6c5f 6964  rlIn..channel_id
+000003e0: da04 626f 6f6c da0d 7368 6f77 5f62 6163  ..bool..show_bac
+000003f0: 6b77 6172 645a 0f73 686f 775f 706f 7765  kwardZ.show_powe
+00000400: 725f 7370 6563 5a12 7368 6f77 5f63 6f6d  r_specZ.show_com
+00000410: 7072 6573 735f 7370 6563 a901 da04 7365  press_spec....se
+00000420: 6c66 a901 da09 5f5f 636c 6173 735f 5fa9  lf....__class__.
+00000430: 00fa 5e43 3a5c 4769 745c 7363 7269 7074  ..^C:\Git\script
+00000440: 735f 7079 7468 6f6e 5f6c 6962 5c6e 616e  s_python_lib\nan
+00000450: 6f73 7572 665c 6170 705c 6170 705f 6465  osurf\app\app_de
+00000460: 6d6f 5f73 6361 6e6e 696e 675f 616e 645f  mo_scanning_and_
+00000470: 6c69 625f 7573 6167 655c 7363 616e 5f6d  lib_usage\scan_m
+00000480: 6f64 756c 655c 7365 7474 696e 6773 2e70  odule\settings.p
+00000490: 7972 0a00 0000 1100 0000 7310 0000 0000  yr........s.....
+000004a0: 010a 0114 0114 0110 0116 0110 0110 017a  ...............z
+000004b0: 1553 6361 6e53 6574 7469 6e67 732e 5f5f  .ScanSettings.__
+000004c0: 696e 6974 5f5f 2906 da08 5f5f 6e61 6d65  init__)...__name
+000004d0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+000004e0: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
+000004f0: 646f 635f 5f72 0a00 0000 da0d 5f5f 636c  doc__r......__cl
+00000500: 6173 7363 656c 6c5f 5f72 1e00 0000 721e  asscell__r....r.
+00000510: 0000 0072 1c00 0000 721f 0000 0072 0300  ...r....r....r..
+00000520: 0000 0d00 0000 7304 0000 0008 0104 0372  ......s........r
+00000530: 0300 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000540: 0000 0000 0003 0000 0040 0000 0073 1e00  .........@...s..
+00000550: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+00000560: 6403 9c01 6404 6405 8404 5a04 6402 5300  d...d.d...Z.d.S.
+00000570: 2906 da0b 5363 616e 5265 7375 6c74 737a  )...ScanResultsz
+00000580: 5720 5468 6973 2063 6c61 7373 2073 6176  W This class sav
+00000590: 6573 2074 6865 2077 6f72 6b65 7220 7461  es the worker ta
+000005a0: 736b 2072 6573 756c 7420 2865 2e67 2062  sk result (e.g b
+000005b0: 6520 7265 6164 2062 7920 6775 6920 656c  e read by gui el
+000005c0: 656d 656e 7473 206f 7220 7361 7665 6420  ements or saved 
+000005d0: 746f 2066 696c 6520 4e72 0400 0000 6301  to file Nr....c.
+000005e0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+000005f0: 0000 0043 0000 0073 0a00 0000 6401 7c00  ...C...s....d.|.
+00000600: 5f00 6400 5300 2902 4e72 0100 0000 2901  _.d.S.).Nr....).
+00000610: 5a17 6375 7272 656e 745f 7363 616e 5f6c  Z.current_scan_l
+00000620: 696e 655f 696e 6465 7872 1a00 0000 721e  ine_indexr....r.
+00000630: 0000 0072 1e00 0000 721f 0000 0072 0a00  ...r....r....r..
+00000640: 0000 1d00 0000 7302 0000 0000 017a 1453  ......s......z.S
+00000650: 6361 6e52 6573 756c 7473 2e5f 5f69 6e69  canResults.__ini
+00000660: 745f 5f29 0572 2000 0000 7221 0000 0072  t__).r ...r!...r
+00000670: 2200 0000 7223 0000 0072 0a00 0000 721e  "...r#...r....r.
+00000680: 0000 0072 1e00 0000 721e 0000 0072 1f00  ...r....r....r..
+00000690: 0000 7225 0000 001b 0000 0073 0400 0000  ..r%.......s....
+000006a0: 0801 0401 7225 0000 0063 0000 0000 0000  ....r%...c......
+000006b0: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+000006c0: 0000 7314 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+000006d0: 015a 0364 025a 0464 0353 0029 04da 0843  .Z.d.Z.d.S.)...C
+000006e0: 6861 6e6e 656c 4429 0172 0100 0000 2901  hannelD).r....).
+000006f0: e901 0000 004e 2905 7220 0000 0072 2100  .....N).r ...r!.
+00000700: 0000 7222 0000 00da 0a44 6566 6c65 6374  ..r".....Deflect
+00000710: 696f 6eda 0a54 6f70 6f67 7261 7068 7972  ion..Topographyr
+00000720: 1e00 0000 721e 0000 0072 1e00 0000 721f  ....r....r....r.
+00000730: 0000 0072 2600 0000 2100 0000 7304 0000  ...r&...!...s...
+00000740: 0008 0104 0172 2600 0000 2910 7223 0000  .....r&...).r#..
+00000750: 00da 0465 6e75 6dda 0b64 6174 6163 6c61  ...enum..datacla
+00000760: 7373 6573 7202 0000 0072 1300 0000 da1e  ssesr....r......
+00000770: 6e61 6e6f 7375 7266 2e6c 6962 2e64 6174  nanosurf.lib.dat
+00000780: 6174 7970 6573 2e73 6369 5f76 616c da03  atypes.sci_val..
+00000790: 6c69 62da 0964 6174 6174 7970 6573 720d  lib..datatypesr.
+000007a0: 0000 00da 1f6e 616e 6f73 7572 662e 6c69  .....nanosurf.li
+000007b0: 622e 6461 7461 7479 7065 732e 7072 6f70  b.datatypes.prop
+000007c0: 5f76 616c 720b 0000 00da 0950 726f 7053  _valr......PropS
+000007d0: 746f 7265 7203 0000 0072 2500 0000 da07  torer....r%.....
+000007e0: 496e 7445 6e75 6d72 2600 0000 721e 0000  IntEnumr&...r...
+000007f0: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00000800: da08 3c6d 6f64 756c 653e 0100 0000 7310  ..<module>....s.
+00000810: 0000 0004 0608 010c 0108 0118 0118 0212  ................
+00000820: 0e0e 06                                  ...
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/gui.py` & `nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 
         self.layout_left = QtWidgets.QVBoxLayout()
         self.layout_left.addWidget(self.scival_image_size)
         self.layout_left.addWidget(self.scival_time_per_line)
         self.layout_left.addWidget(self.scival_points)
         self.layout_left.addWidget(self.combo_channel_dir)
         self.layout_left.addStretch()
+        self.layout_left.addSpacerItem(nsf.frameworks.qt_app.app_gui.StdVSpacer())
         self.layout_left.addWidget(self.button_start_stop)
 
         # mid layout - plots and result ---------------------------------------------------------
         self.chart_plot = nsf.gui.NSFChart()
         self.colormap_plot = nsf.gui.NSFColormap()
         self.spec_plot = nsf.gui.NSFChart(logmodex=True, logmodey=True)
 
@@ -106,25 +107,24 @@
         self.layout_charts.addLayout(self.layout_spec_chart)
         self.layout_plots  = QtWidgets.QHBoxLayout()
         self.layout_plots.addLayout(self.layout_colormap)
         self.layout_plots.addLayout(self.layout_charts)
         self.layout_mid.addLayout(self.layout_plots)
         self.layout_mid.addWidget(self.tableResults)
 
-        self.layout_left.addSpacerItem(nsf.frameworks.qt_app.app_gui.StdVSpacer())
 
         # right layout - additional user inputs
 
         self.layout_right= QtWidgets.QVBoxLayout()
 
         # set GUI controls
         self.screen_layout = QtWidgets.QHBoxLayout()
         # stretch only plot area and keep controls fix in size
-        self.screen_layout.addLayout(self.layout_left, 1)
-        self.screen_layout.addLayout(self.layout_mid,  2) 
+        self.screen_layout.addLayout(self.layout_left, 0)
+        self.screen_layout.addLayout(self.layout_mid,  1) 
         self.screen_layout.addLayout(self.layout_right,0)
         self.setLayout(self.screen_layout)
 
         self.bind_gui_elements()
         self.init_plot()
         self.enter_gui_state_idle()
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/imaging_task.py` & `nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/imaging_task.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/module.py` & `nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/module.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/settings.py` & `nanosurf-1.6.2/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,30 +6,31 @@
 
 import enum
 from dataclasses import dataclass
 import nanosurf
 import nanosurf.lib.datatypes.sci_val as sci_val
 import nanosurf.lib.datatypes.prop_val as prop_val
 
-@dataclass
 class ScanSettings(prop_val.PropStore):
     """ settings defined here as PropVal are stored persistently in a ini-file
         settings with a '_' as first char are not stored
     """
-    image_size = prop_val.PropVal(sci_val.SciVal(10e-6, "m"))
-    time_per_line = prop_val.PropVal(sci_val.SciVal(0.2, "s"))
-    points_per_line = prop_val.PropVal(int(256))
-    channel_id = prop_val.PropVal(int(nanosurf.Spm.ScanChannel.Deflection_or_ZCtrlIn))
-    show_backward = prop_val.PropVal(bool(True))
-    show_power_spec = prop_val.PropVal(bool(True))
-    show_compress_spec = prop_val.PropVal(bool(False))
+    def __init__(self) -> None:
+        super().__init__()
+        self.image_size = prop_val.PropVal(sci_val.SciVal(10e-6, "m"))
+        self.time_per_line = prop_val.PropVal(sci_val.SciVal(0.2, "s"))
+        self.points_per_line = prop_val.PropVal(int(256))
+        self.channel_id = prop_val.PropVal(int(nanosurf.Spm.ScanChannel.Deflection_or_ZCtrlIn))
+        self.show_backward = prop_val.PropVal(bool(True))
+        self.show_power_spec = prop_val.PropVal(bool(True))
+        self.show_compress_spec = prop_val.PropVal(bool(False))
 
-@dataclass
 class ScanResults():
     """ This class saves the worker task result (e.g be read by gui elements or saved to file """
-    current_scan_line_index = 0
+    def __init__(self) -> None:
+        self.current_scan_line_index = 0
 
 """ Combo boxes show entries with IDs and the names in second list"""
 class ChannelD(enum.IntEnum):
     Deflection = 0,
     Topography = 1,
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/.vscode/launch.json` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_fit.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_fit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_fit.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_fit.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 12:01:03 2023 UTC, .py size: 7030 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7f40 3964 761b 0000  a........@9dv...
+00000000: 610d 0d0a 0000 0000 5a4d 3964 761b 0000  a.......ZM9dv...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6402 6c05 5a06 6401 6404 6c07 6d08 5a09  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6401 6405 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0c 5a0c 0100 6504 4700 6407  d.l.m.Z...e.G.d.
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_gui.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_gui.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_gui.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_gui.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 11:56:46 2023 UTC, .py size: 13967 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7e3f 3964 8f36 0000  a.......~?9d.6..
+00000000: 610d 0d0a 0000 0000 a321 5264 9336 0000  a........!Rd.6..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5601 0000 6400  .....@...sV...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a04 6401 6403 6c05 6d06 0200  d.l.Z.d.d.l.m...
 00000050: 0100 6d07 0200 0100 6d08 0200 0100 6d09  ..m.....m.....m.
 00000060: 5a0a 0100 6401 6404 6c0b 6d0c 5a0c 6d0d  Z...d.d.l.m.Z.m.
 00000070: 5a0d 0100 4700 6405 6406 8400 6406 6504  Z...G.d.d...d.e.
@@ -77,15 +77,15 @@
 000004c0: 02da 0573 7570 6572 da08 5f5f 696e 6974  ...super..__init
 000004d0: 5f5f a901 da04 7365 6c66 a901 da09 5f5f  __....self....__
 000004e0: 636c 6173 735f 5f72 0f00 0000 7210 0000  class__r....r...
 000004f0: 0072 1700 0000 2400 0000 7304 0000 0000  .r....$...s.....
 00000500: 0104 017a 1453 7765 6570 5363 7265 656e  ...z.SweepScreen
 00000510: 2e5f 5f69 6e69 745f 5f29 01da 066d 6f64  .__init__)...mod
 00000520: 756c 6563 0200 0000 0000 0000 0000 0000  ulec............
-00000530: 0200 0000 0400 0000 4300 0000 73f6 0300  ........C...s...
+00000530: 0200 0000 0400 0000 4300 0000 73da 0300  ........C...s...
 00000540: 007c 017c 005f 0074 01a0 0264 01a1 017c  .|.|._.t...d...|
 00000550: 005f 0374 01a0 04a1 007c 005f 057c 00a0  ._.t.....|._.|..
 00000560: 06a1 0001 0074 076a 08a0 0974 0a64 02a1  .....t.j...t.d..
 00000570: 027c 005f 0b74 076a 086a 09a0 0c74 0d6a  .|._.t.j.j...t.j
 00000580: 0e6a 0fa1 017c 005f 1074 076a 08a0 097c  .j...|._.t.j...|
 00000590: 006a 1064 03a1 027c 005f 1174 076a 086a  .j.d...|._.t.j.j
 000005a0: 09a0 0c74 0d6a 0e6a 12a1 017c 005f 1374  ...t.j.j...|._.t
@@ -110,496 +110,494 @@
 000006d0: 0101 007c 006a 25a0 1c74 076a 1d6a 1e6a  ...|.j%..t.j.j.j
 000006e0: 1f6a 20a1 0101 007c 006a 25a0 2164 0ba1  .j ....|.j%.!d..
 000006f0: 0101 007c 006a 25a0 2264 07a1 0101 007c  ...|.j%."d.....|
 00000700: 006a 25a0 2764 0ca1 0101 0074 01a0 2864  .j%.'d.....t..(d
 00000710: 0da1 017c 005f 2974 01a0 2a64 0ea1 017c  ...|._)t..*d...|
 00000720: 005f 2b74 01a0 2a64 0fa1 017c 005f 2c74  ._+t..*d...|._,t
 00000730: 01a0 2a64 10a1 017c 005f 2d74 01a0 2ea1  ..*d...|._-t....
-00000740: 007c 005f 2f7c 006a 2fa0 307c 006a 03a1  .|._/|.j/.0|.j..
-00000750: 0101 007c 006a 2fa0 307c 006a 05a1 0101  ...|.j/.0|.j....
-00000760: 007c 006a 2fa0 307c 006a 0ba1 0101 007c  .|.j/.0|.j.....|
-00000770: 006a 2fa0 307c 006a 11a1 0101 007c 006a  .j/.0|.j.....|.j
-00000780: 2fa0 307c 006a 14a1 0101 007c 006a 2fa0  /.0|.j.....|.j/.
-00000790: 307c 006a 17a1 0101 007c 006a 2fa0 307c  0|.j.....|.j/.0|
-000007a0: 006a 19a1 0101 007c 006a 2fa0 307c 006a  .j.....|.j/.0|.j
-000007b0: 23a1 0101 007c 006a 2fa0 307c 006a 24a1  #....|.j/.0|.j$.
-000007c0: 0101 007c 006a 2fa0 307c 006a 25a1 0101  ...|.j/.0|.j%...
-000007d0: 007c 006a 2fa0 31a1 0001 007c 006a 2fa0  .|.j/.1....|.j/.
-000007e0: 307c 006a 2ca1 0101 007c 006a 2fa0 3274  0|.j,....|.j/.2t
-000007f0: 076a 336a 346a 35a0 36a1 00a1 0101 0074  .j3j4j5.6......t
-00000800: 076a 08a0 37a1 007c 005f 3874 076a 08a0  .j..7..|._8t.j..
-00000810: 37a1 007c 005f 3974 076a 08a0 3a74 3ba1  7..|._9t.j..:t;.
-00000820: 017c 005f 3c7c 006a 3ca0 3d74 3b6a 3e64  .|._<|.j<.=t;j>d
-00000830: 11a1 0201 007c 006a 3ca0 3d74 3b6a 3f64  .....|.j<.=t;j?d
-00000840: 12a1 0201 0074 01a0 2ea1 007c 005f 407c  .....t.....|._@|
-00000850: 006a 40a0 307c 006a 38a1 0101 007c 006a  .j@.0|.j8....|.j
-00000860: 40a0 307c 006a 39a1 0101 007c 006a 40a0  @.0|.j9....|.j@.
-00000870: 307c 006a 3ca1 0101 007c 006a 40a0 3274  0|.j<....|.j@.2t
-00000880: 076a 336a 346a 35a0 36a1 00a1 0101 0074  .j3j4j5.6......t
-00000890: 076a 08a0 0974 4164 13a1 027c 005f 4274  .j...tAd...|._Bt
-000008a0: 01a0 2ea1 007c 005f 437c 006a 43a0 307c  .....|._C|.jC.0|
-000008b0: 006a 42a1 0101 007c 006a 43a0 3274 076a  .jB....|.jC.2t.j
-000008c0: 336a 346a 35a0 36a1 00a1 0101 0074 01a0  3j4j5.6......t..
-000008d0: 44a1 007c 005f 457c 006a 45a0 467c 006a  D..|._E|.jE.F|.j
-000008e0: 2f64 07a1 0201 007c 006a 45a0 467c 006a  /d.....|.jE.F|.j
-000008f0: 4064 0ba1 0201 007c 006a 45a0 467c 006a  @d.....|.jE.F|.j
-00000900: 4364 07a1 0201 007c 00a0 477c 006a 45a1  Cd.....|..G|.jE.
-00000910: 0101 007c 00a0 48a1 0001 007c 00a0 49a1  ...|..H....|..I.
-00000920: 0001 007c 00a0 4aa1 0001 007c 00a0 4ba1  ...|..J....|..K.
-00000930: 0001 0064 1453 0029 157a 3820 6372 6561  ...d.S.).z8 crea
-00000940: 7465 2068 6572 6520 796f 7572 2067 7569  te here your gui
-00000950: 2077 6974 6820 616c 6c20 636f 6e74 726f   with all contro
-00000960: 6c73 2061 6e64 2074 6865 6972 206c 6179  ls and their lay
-00000970: 6f75 74da 0a43 616e 7469 6c65 7665 727a  out..Cantileverz
-00000980: 1145 7863 6974 6174 696f 6e20 4d65 7468  .Excitation Meth
-00000990: 6f64 7a0c 496e 7075 7420 536f 7572 6365  odz.Input Source
-000009a0: 7a0d 4f75 7470 7574 2053 6f75 7263 655a  z.Output SourceZ
-000009b0: 0942 616e 6477 6964 7468 7a10 4365 6e74  .Bandwidthz.Cent
-000009c0: 6572 2046 7265 7175 656e 6379 7201 0000  er Frequencyr...
-000009d0: 007a 0f46 7265 7175 656e 6379 2052 616e  .z.Frequency Ran
-000009e0: 6765 7a0f 4672 6571 7565 6e63 7920 5374  gez.Frequency St
-000009f0: 6570 737a 1445 7863 6974 6174 696f 6e20  epsz.Excitation 
-00000a00: 416d 706c 6974 7564 6572 0600 0000 7207  Amplituder....r.
-00000a10: 0000 007a 0a45 6d69 7420 5469 636b 73da  ...z.Emit Ticks.
-00000a20: 0841 7070 726f 6163 68fa 0b53 7461 7274  .Approach..Start
-00000a30: 2053 7765 6570 da04 5361 7665 7a13 5265   Sweep..Savez.Re
-00000a40: 736f 6e61 6e63 6520 4672 6571 7565 6e63  sonance Frequenc
-00000a50: 797a 0851 2d46 6163 746f 727a 0a50 6c6f  yz.Q-Factorz.Plo
-00000a60: 7420 5374 796c 654e 294c 721c 0000 0072  t StyleN)Lr....r
-00000a70: 0200 0000 da06 514c 6162 656c 5a10 6c61  ......QLabelZ.la
-00000a80: 6265 6c5f 6361 6e74 696c 6576 6572 da09  bel_cantilever..
-00000a90: 5143 6f6d 626f 426f 78da 1063 6f6d 626f  QComboBox..combo
-00000aa0: 5f63 616e 7469 6c65 7665 72da 1675 7064  _cantilever..upd
-00000ab0: 6174 655f 6361 6e74 696c 6576 6572 5f6c  ate_cantilever_l
-00000ac0: 6973 74da 036e 7366 da03 6775 69da 0b4e  ist..nsf..gui..N
-00000ad0: 5346 436f 6d62 6f42 6f78 da16 436f 6d62  SFComboBox..Comb
-00000ae0: 6f45 7863 6974 6174 696f 6e4d 6574 686f  oExcitationMetho
-00000af0: 6473 da17 636f 6d62 6f5f 6578 6369 7461  ds..combo_excita
-00000b00: 7469 6f6e 5f6d 6574 686f 64da 1b63 7265  tion_method..cre
-00000b10: 6174 655f 656e 7472 795f 6c69 7374 5f66  ate_entry_list_f
-00000b20: 726f 6d5f 6469 6374 da0a 6672 6571 5f73  rom_dict..freq_s
-00000b30: 7765 6570 da0e 4672 6571 7565 6e63 7953  weep..FrequencyS
-00000b40: 7765 6570 da13 696e 7075 745f 736f 7572  weep..input_sour
-00000b50: 6365 735f 6e61 6d65 735a 1863 6f6d 626f  ces_namesZ.combo
-00000b60: 5f69 6e70 7574 5f73 6f75 7263 655f 6974  _input_source_it
-00000b70: 656d 73da 1263 6f6d 626f 5f69 6e70 7574  ems..combo_input
-00000b80: 5f73 6f75 7263 65da 0c6f 7574 7075 745f  _source..output_
-00000b90: 6e61 6d65 735a 1963 6f6d 626f 5f6f 7574  namesZ.combo_out
-00000ba0: 7075 745f 736f 7572 6365 5f69 7465 6d73  put_source_items
-00000bb0: da13 636f 6d62 6f5f 6f75 7470 7574 5f73  ..combo_output_s
-00000bc0: 6f75 7263 65da 1062 616e 6477 6964 7468  ource..bandwidth
-00000bd0: 735f 6e61 6d65 735a 1563 6f6d 626f 5f62  s_namesZ.combo_b
-00000be0: 616e 6477 6964 7468 5f69 7465 6d73 da0f  andwidth_items..
-00000bf0: 636f 6d62 6f5f 6261 6e64 7769 6474 68da  combo_bandwidth.
-00000c00: 0a4e 5346 5363 6945 6469 74da 1773 6369  .NSFSciEdit..sci
-00000c10: 7661 6c5f 6365 6e74 6572 5f66 7265 7175  val_center_frequ
-00000c20: 656e 6379 da16 7365 745f 616c 6c6f 7765  ency..set_allowe
-00000c30: 645f 7072 6566 6978 5f69 6473 da17 616c  d_prefix_ids..al
-00000c40: 6c6f 7765 645f 6672 6571 7565 6e63 795f  lowed_frequency_
-00000c50: 756e 6974 73da 0d73 6574 5f70 7265 6669  units..set_prefi
-00000c60: 785f 6964 da07 7363 695f 7661 6cda 0275  x_id..sci_val..u
-00000c70: 70da 0650 7265 6669 78da 0561 7574 6f5f  p..Prefix..auto_
-00000c80: da0d 7365 745f 7072 6563 6973 696f 6eda  ..set_precision.
-00000c90: 0d73 6574 5f76 616c 7565 5f6d 696e da16  .set_value_min..
-00000ca0: 7363 6976 616c 5f66 7265 7175 656e 6379  scival_frequency
-00000cb0: 5f72 616e 6765 da16 7363 6976 616c 5f66  _range..scival_f
-00000cc0: 7265 7175 656e 6379 5f73 7465 7073 da1b  requency_steps..
-00000cd0: 7363 6976 616c 5f65 7863 6974 6174 696f  scival_excitatio
-00000ce0: 6e5f 616d 706c 6974 7564 65da 1561 6c6c  n_amplitude..all
-00000cf0: 6f77 6564 5f76 6f6c 7461 6765 5f75 6e69  owed_voltage_uni
-00000d00: 7473 da0d 7365 745f 7661 6c75 655f 6d61  ts..set_value_ma
-00000d10: 78da 0951 4368 6563 6b42 6f78 5a10 6368  x..QCheckBoxZ.ch
-00000d20: 6563 6b5f 656d 6974 5f74 6963 6b73 da0b  eck_emit_ticks..
-00000d30: 5150 7573 6842 7574 746f 6e5a 0f62 7574  QPushButtonZ.but
-00000d40: 746f 6e5f 6170 7072 6f61 6368 da11 6275  ton_approach..bu
-00000d50: 7474 6f6e 5f73 7461 7274 5f73 746f 705a  tton_start_stopZ
-00000d60: 0b62 7574 746f 6e5f 7361 7665 da0b 5156  .button_save..QV
-00000d70: 426f 784c 6179 6f75 745a 0b6c 6179 6f75  BoxLayoutZ.layou
-00000d80: 745f 6c65 6674 da09 6164 6457 6964 6765  t_left..addWidge
-00000d90: 74da 0a61 6464 5374 7265 7463 68da 0d61  t..addStretch..a
-00000da0: 6464 5370 6163 6572 4974 656d da0a 6672  ddSpacerItem..fr
-00000db0: 616d 6577 6f72 6b73 da06 7174 5f61 7070  ameworks..qt_app
-00000dc0: da07 6170 705f 6775 69da 0a53 7464 5653  ..app_gui..StdVS
-00000dd0: 7061 6365 72da 084e 5346 4368 6172 74da  pacer..NSFChart.
-00000de0: 0e61 6d70 6c69 7475 6465 5f70 6c6f 74da  .amplitude_plot.
-00000df0: 0a70 6861 7365 5f70 6c6f 74da 114e 5346  .phase_plot..NSF
-00000e00: 4e61 6d65 5661 6c75 6554 6162 6c65 7205  NameValueTabler.
-00000e10: 0000 00da 0c74 6162 6c65 5265 7375 6c74  .....tableResult
-00000e20: 73da 0c64 6566 696e 655f 656e 7472 7972  s..define_entryr
-00000e30: 0c00 0000 720d 0000 005a 0a6c 6179 6f75  ....r....Z.layou
-00000e40: 745f 6d69 64da 0f43 6f6d 626f 506c 6f74  t_mid..ComboPlot
-00000e50: 5374 796c 6573 da10 636f 6d62 6f5f 706c  Styles..combo_pl
-00000e60: 6f74 5f73 7479 6c65 5a0c 6c61 796f 7574  ot_styleZ.layout
-00000e70: 5f72 6967 6874 da0b 5148 426f 784c 6179  _right..QHBoxLay
-00000e80: 6f75 745a 0d73 6372 6565 6e5f 6c61 796f  outZ.screen_layo
-00000e90: 7574 da09 6164 644c 6179 6f75 74da 0973  ut..addLayout..s
-00000ea0: 6574 4c61 796f 7574 da11 6269 6e64 5f67  etLayout..bind_g
-00000eb0: 7569 5f65 6c65 6d65 6e74 73da 0969 6e69  ui_elements..ini
-00000ec0: 745f 706c 6f74 da14 656e 7465 725f 6775  t_plot..enter_gu
-00000ed0: 695f 7374 6174 655f 6964 6c65 da0b 7570  i_state_idle..up
-00000ee0: 6461 7465 5f70 6c6f 7429 0272 1900 0000  date_plot).r....
-00000ef0: 721c 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00000f00: 1000 0000 da0f 646f 5f73 6574 7570 5f73  ......do_setup_s
-00000f10: 6372 6565 6e28 0000 0073 9200 0000 0002  creen(...s......
-00000f20: 0603 0c01 0a01 0802 1002 1401 1202 1401  ................
-00000f30: 1202 1401 1202 0e01 0c01 1401 0c01 0c02  ................
-00000f40: 0e01 0c01 1401 0c01 0c02 0e01 0c01 1401  ................
-00000f50: 0c01 0c02 0e01 0c01 1401 0c01 0c01 0c02  ................
-00000f60: 0c01 0c01 0c01 0c02 0a01 0e01 0e01 0e01  ................
-00000f70: 0e01 0e01 0e01 0e01 0e01 0e01 0e01 0a01  ................
-00000f80: 0e01 1603 0c01 0c01 0e01 1001 1002 0a01  ................
-00000f90: 0e01 0e01 0e01 1603 1002 0a01 0e01 1603  ................
-00000fa0: 0a02 1001 1001 1002 0c02 0801 0801 0801  ................
-00000fb0: 7a1b 5377 6565 7053 6372 6565 6e2e 646f  z.SweepScreen.do
-00000fc0: 5f73 6574 7570 5f73 6372 6565 6e63 0100  _setup_screenc..
-00000fd0: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00000fe0: 0000 4300 0000 735e 0100 0074 006a 01a0  ..C...s^...t.j..
-00000ff0: 027c 006a 037c 006a 046a 056a 06a1 0201  .|.j.|.j.j.j....
-00001000: 0074 006a 01a0 027c 006a 077c 006a 046a  .t.j...|.j.|.j.j
-00001010: 056a 08a1 0201 0074 006a 01a0 027c 006a  .j.....t.j...|.j
-00001020: 097c 006a 046a 056a 0aa1 0201 0074 006a  .|.j.j.j.....t.j
-00001030: 01a0 027c 006a 0b7c 006a 046a 056a 0ca1  ...|.j.|.j.j.j..
-00001040: 0201 0074 006a 01a0 027c 006a 0d7c 006a  ...t.j...|.j.|.j
-00001050: 046a 056a 0ea1 0201 0074 006a 01a0 027c  .j.j.....t.j...|
-00001060: 006a 0f7c 006a 046a 056a 10a1 0201 0074  .j.|.j.j.j.....t
-00001070: 006a 01a0 027c 006a 117c 006a 046a 056a  .j...|.j.|.j.j.j
-00001080: 12a1 0201 0074 006a 01a0 027c 006a 137c  .....t.j...|.j.|
-00001090: 006a 046a 056a 14a1 0201 0074 006a 01a0  .j.j.j.....t.j..
-000010a0: 027c 006a 157c 006a 046a 056a 16a1 0201  .|.j.|.j.j.j....
-000010b0: 007c 006a 176a 18a0 197c 006a 1aa1 0101  .|.j.j...|.j....
-000010c0: 007c 006a 046a 056a 066a 1ba0 197c 006a  .|.j.j.j.j...|.j
-000010d0: 1ca1 0101 007c 006a 1d6a 1ea0 197c 006a  .....|.j.j...|.j
-000010e0: 1fa1 0101 007c 006a 046a 20a0 197c 006a  .....|.j.j ..|.j
-000010f0: 21a1 0101 007c 006a 046a 22a0 197c 006a  !....|.j.j"..|.j
-00001100: 21a1 0101 007c 006a 046a 23a0 197c 006a  !....|.j.j#..|.j
-00001110: 24a1 0101 007c 006a 046a 25a0 197c 006a  $....|.j.j%..|.j
-00001120: 26a1 0101 007c 006a 046a 27a0 197c 006a  &....|.j.j'..|.j
-00001130: 28a1 0101 007c 006a 046a 29a0 197c 006a  (....|.j.j)..|.j
-00001140: 2aa1 0101 0064 0153 0029 027a 4b20 636f  *....d.S.).zK co
-00001150: 6e6e 6563 7420 6865 7265 2061 6c6c 2067  nnect here all g
-00001160: 7569 2077 6964 6765 7473 2074 6f20 7365  ui widgets to se
-00001170: 7474 696e 6773 206f 6620 7468 6520 6d6f  ttings of the mo
-00001180: 6475 6c65 206f 7220 616e 7920 6f74 6865  dule or any othe
-00001190: 7220 736f 7572 6365 4e29 2b72 2500 0000  r sourceN)+r%...
-000011a0: 7226 0000 00da 1363 6f6e 6e65 6374 5f74  r&.....connect_t
-000011b0: 6f5f 7072 6f70 6572 7479 7255 0000 0072  o_propertyrU...r
-000011c0: 1c00 0000 da08 7365 7474 696e 6773 da0d  ......settings..
-000011d0: 706c 6f74 5f73 7479 6c65 5f69 6472 2900  plot_style_idr).
-000011e0: 0000 da11 6578 6369 7461 7469 6f6e 5f6d  ....excitation_m
-000011f0: 6574 686f 6472 2e00 0000 da0c 696e 7075  ethodr......inpu
-00001200: 745f 736f 7572 6365 7230 0000 00da 0d6f  t_sourcer0.....o
-00001210: 7574 7075 745f 736f 7572 6365 7232 0000  utput_sourcer2..
-00001220: 00da 0962 616e 6477 6964 7468 7234 0000  ...bandwidthr4..
-00001230: 00da 1063 656e 7465 725f 6672 6571 7565  ...center_freque
-00001240: 6e63 7972 3e00 0000 da0f 6672 6571 7565  ncyr>.....freque
-00001250: 6e63 795f 7261 6e67 6572 3f00 0000 da0f  ncy_ranger?.....
-00001260: 6672 6571 7565 6e63 795f 7374 6570 7372  frequency_stepsr
-00001270: 4000 0000 da14 6578 6369 7461 7469 6f6e  @.....excitation
-00001280: 5f61 6d70 6c69 7475 6465 7223 0000 00da  _amplituder#....
-00001290: 0961 6374 6976 6174 6564 da07 636f 6e6e  .activated..conn
-000012a0: 6563 74da 1175 7064 6174 655f 6361 6e74  ect..update_cant
-000012b0: 696c 6576 6572 da11 7369 675f 7661 6c75  ilever..sig_valu
-000012c0: 655f 6368 616e 6765 6472 5c00 0000 7245  e_changedr\...rE
-000012d0: 0000 00da 0763 6c69 636b 6564 da1c 6f6e  .....clicked..on
-000012e0: 5f62 7574 746f 6e5f 7374 6172 745f 7374  _button_start_st
-000012f0: 6f70 5f63 6c69 636b 6564 da18 7369 675f  op_clicked..sig_
-00001300: 776f 726b 5f73 7461 7274 5f72 6571 7565  work_start_reque
-00001310: 7374 6564 da14 656e 7465 725f 6775 695f  sted..enter_gui_
-00001320: 7374 6174 655f 7761 6974 da17 7369 675f  state_wait..sig_
-00001330: 776f 726b 5f73 746f 705f 7265 7175 6573  work_stop_reques
-00001340: 7465 64da 0f73 6967 5f77 6f72 6b5f 6163  ted..sig_work_ac
-00001350: 7469 7665 da16 656e 7465 725f 6775 695f  tive..enter_gui_
-00001360: 7374 6174 655f 6163 7469 7665 da0d 7369  state_active..si
-00001370: 675f 776f 726b 5f64 6f6e 6572 5b00 0000  g_work_doner[...
-00001380: da16 7369 675f 6e65 775f 6461 7461 5f61  ..sig_new_data_a
-00001390: 7661 696c 6162 6c65 da0d 7368 6f77 5f6e  vailable..show_n
-000013a0: 6577 5f64 6174 61da 1073 6967 5f64 6174  ew_data..sig_dat
-000013b0: 615f 696e 7661 6c69 64da 1073 6574 5f64  a_invalid..set_d
-000013c0: 6174 615f 696e 7661 6c69 6472 1800 0000  ata_invalidr....
-000013d0: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-000013e0: 5900 0000 8b00 0000 7324 0000 0000 0416  Y.......s$......
-000013f0: 0116 0116 0116 0116 0116 0116 0116 0116  ................
-00001400: 0310 0114 0310 0310 0110 0110 0110 0110  ................
-00001410: 017a 1d53 7765 6570 5363 7265 656e 2e62  .z.SweepScreen.b
-00001420: 696e 645f 6775 695f 656c 656d 656e 7473  ind_gui_elements
-00001430: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001440: 0004 0000 0043 0000 0073 e000 0000 7c00  .....C...s....|.
-00001450: 6a00 a001 6401 a101 0100 7c00 6a00 a002  j...d.....|.j...
-00001460: 7403 6a04 6a05 6a06 6a07 6402 a102 0100  t.j.j.j.j.d.....
-00001470: 7c00 6a00 a008 7403 6a04 6a05 6a06 6a07  |.j...t.j.j.j.j.
-00001480: 6403 a102 0100 7c00 6a00 a002 7403 6a04  d.....|.j...t.j.
-00001490: 6a05 6a06 6a09 6404 a102 0100 7c00 6a00  j.j.j.d.....|.j.
-000014a0: a008 7403 6a04 6a05 6a06 6a09 6405 a102  ..t.j.j.j.j.d...
-000014b0: 0100 7c00 6a00 a00a a100 0100 7c00 6a0b  ..|.j.......|.j.
-000014c0: a001 6406 a101 0100 7c00 6a0b a002 7403  ..d.....|.j...t.
-000014d0: 6a04 6a05 6a06 6a07 6402 a102 0100 7c00  j.j.j.j.d.....|.
-000014e0: 6a0b a008 7403 6a04 6a05 6a06 6a07 6403  j...t.j.j.j.j.d.
-000014f0: a102 0100 7c00 6a0b a002 7403 6a04 6a05  ....|.j...t.j.j.
-00001500: 6a06 6a09 6407 a102 0100 7c00 6a0b a008  j.j.d.....|.j...
-00001510: 7403 6a04 6a05 6a06 6a09 6408 a102 0100  t.j.j.j.j.d.....
-00001520: 7c00 6a0b a00a a100 0100 6400 5300 2909  |.j.......d.S.).
-00001530: 4e7a 1241 6d70 6c69 7475 6465 2053 7065  Nz.Amplitude Spe
-00001540: 6374 7275 6dda 0946 7265 7175 656e 6379  ctrum..Frequency
-00001550: da02 487a da09 416d 706c 6974 7564 65da  ..Hz..Amplitude.
-00001560: 0156 7a0e 5068 6173 6520 5370 6563 7472  .Vz.Phase Spectr
-00001570: 756d da05 5068 6173 65da 0364 6567 290c  um..Phase..deg).
-00001580: 724f 0000 00da 0973 6574 5f74 6974 6c65  rO.....set_title
-00001590: da09 7365 745f 6c61 6265 6c72 2500 0000  ..set_labelr%...
-000015a0: 7226 0000 0072 4e00 0000 da04 4178 6973  r&...rN.....Axis
-000015b0: da06 626f 7474 6f6d da08 7365 745f 756e  ..bottom..set_un
-000015c0: 6974 da04 6c65 6674 da0b 636c 6561 725f  it..left..clear_
-000015d0: 706c 6f74 7372 5000 0000 7218 0000 0072  plotsrP...r....r
-000015e0: 0f00 0000 720f 0000 0072 1000 0000 725a  ....r....r....rZ
-000015f0: 0000 00a8 0000 0073 1800 0000 0001 0c01  .......s........
-00001600: 1601 1601 1601 1601 0a02 0c01 1601 1601  ................
-00001610: 1601 1601 7a15 5377 6565 7053 6372 6565  ....z.SweepScree
-00001620: 6e2e 696e 6974 5f70 6c6f 7463 0100 0000  n.init_plotc....
-00001630: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00001640: 4300 0000 7330 0000 007c 006a 00a0 01a1  C...s0...|.j....
-00001650: 0072 227c 006a 00a0 02a1 0001 007c 006a  .r"|.j.......|.j
-00001660: 0364 0164 028d 0101 006e 0a7c 006a 00a0  .d.d.....n.|.j..
-00001670: 04a1 0001 0064 0053 0029 034e 54a9 01da  .....d.S.).NT...
-00001680: 0477 6169 7429 0572 1c00 0000 da0d 6973  .wait).r......is
-00001690: 5f73 7765 6570 5f62 7573 79da 0a73 746f  _sweep_busy..sto
-000016a0: 705f 7377 6565 70da 1773 7461 7274 5f73  p_sweep..start_s
-000016b0: 746f 705f 6275 7474 6f6e 5f73 7461 7465  top_button_state
-000016c0: da0b 7374 6172 745f 7377 6565 7072 1800  ..start_sweepr..
-000016d0: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-000016e0: 0072 6e00 0000 b700 0000 7308 0000 0000  .rn.......s.....
-000016f0: 010a 010a 010e 027a 2853 7765 6570 5363  .......z(SweepSc
-00001700: 7265 656e 2e6f 6e5f 6275 7474 6f6e 5f73  reen.on_button_s
-00001710: 7461 7274 5f73 746f 705f 636c 6963 6b65  tart_stop_clicke
-00001720: 6463 0100 0000 0000 0000 0000 0000 0100  dc..............
-00001730: 0000 0300 0000 4300 0000 731c 0000 007c  ......C...s....|
-00001740: 006a 0064 0164 028d 0101 007c 006a 0164  .j.d.d.....|.j.d
-00001750: 0364 048d 0101 0064 0053 0029 054e 46a9  .d.....d.S.).NF.
-00001760: 01da 0765 6e61 626c 6564 5472 8600 0000  ...enabledTr....
-00001770: 2902 da21 7365 745f 7061 7261 6d65 7465  )..!set_paramete
-00001780: 725f 7769 6467 6574 5f65 6e61 626c 655f  r_widget_enable_
-00001790: 7374 6174 6572 8a00 0000 7218 0000 0072  stater....r....r
-000017a0: 0f00 0000 720f 0000 0072 1000 0000 7270  ....r....r....rp
-000017b0: 0000 00be 0000 0073 0400 0000 0001 0c01  .......s........
-000017c0: 7a20 5377 6565 7053 6372 6565 6e2e 656e  z SweepScreen.en
-000017d0: 7465 725f 6775 695f 7374 6174 655f 7761  ter_gui_state_wa
-000017e0: 6974 6301 0000 0000 0000 0000 0000 0001  itc.............
-000017f0: 0000 0004 0000 0043 0000 0073 2c00 0000  .......C...s,...
-00001800: 7c00 6a00 6401 6402 8d01 0100 7c00 6a01  |.j.d.d.....|.j.
-00001810: 6401 7c00 6a02 a003 a100 6403 8d02 0100  d.|.j.....d.....
-00001820: 7c00 a004 a100 0100 6400 5300 2904 4e46  |.......d.S.).NF
-00001830: 728c 0000 00a9 0272 8700 0000 da0a 7374  r......r......st
-00001840: 6f70 5f73 7461 7465 2905 728e 0000 0072  op_state).r....r
-00001850: 8a00 0000 721c 0000 0072 8800 0000 725a  ....r....r....rZ
-00001860: 0000 0072 1800 0000 720f 0000 0072 0f00  ...r....r....r..
-00001870: 0000 7210 0000 0072 7300 0000 c200 0000  ..r....rs.......
-00001880: 7306 0000 0000 010c 0114 017a 2253 7765  s..........z"Swe
-00001890: 6570 5363 7265 656e 2e65 6e74 6572 5f67  epScreen.enter_g
-000018a0: 7569 5f73 7461 7465 5f61 6374 6976 6563  ui_state_activec
-000018b0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000018c0: 0400 0000 4300 0000 7324 0000 007c 006a  ....C...s$...|.j
-000018d0: 0064 0164 028d 0101 007c 006a 0164 037c  .d.d.....|.j.d.|
-000018e0: 006a 02a0 03a1 0064 048d 0201 0064 0053  .j.....d.....d.S
-000018f0: 0029 054e 5472 8c00 0000 4672 8f00 0000  .).NTr....Fr....
-00001900: 2904 728e 0000 0072 8a00 0000 721c 0000  ).r....r....r...
-00001910: 0072 8800 0000 7218 0000 0072 0f00 0000  .r....r....r....
-00001920: 720f 0000 0072 1000 0000 725b 0000 00c7  r....r....r[....
-00001930: 0000 0073 0400 0000 0001 0c01 7a20 5377  ...s........z Sw
-00001940: 6565 7053 6372 6565 6e2e 656e 7465 725f  eepScreen.enter_
-00001950: 6775 695f 7374 6174 655f 6964 6c65 5472  gui_state_idleTr
-00001960: 8c00 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00001970: 0002 0000 0003 0000 0043 0000 0073 7000  .........C...sp.
-00001980: 0000 7c00 6a00 a001 7c01 a101 0100 7c00  ..|.j...|.....|.
-00001990: 6a02 a001 7c01 a101 0100 7c00 6a03 a001  j...|.....|.j...
-000019a0: 7c01 a101 0100 7c00 6a04 a001 7c01 a101  |.....|.j...|...
-000019b0: 0100 7c00 6a05 a001 7c01 a101 0100 7c00  ..|.j...|.....|.
-000019c0: 6a06 a001 7c01 a101 0100 7c00 6a07 a001  j...|.....|.j...
-000019d0: 7c01 a101 0100 7c00 6a08 a001 7c01 a101  |.....|.j...|...
-000019e0: 0100 7c00 6a09 a001 7c01 a101 0100 6400  ..|.j...|.....d.
-000019f0: 5300 7215 0000 0029 0a72 2300 0000 da0a  S.r....).r#.....
-00001a00: 7365 7445 6e61 626c 6564 7229 0000 0072  setEnabledr)...r
-00001a10: 2e00 0000 7230 0000 0072 3200 0000 7234  ....r0...r2...r4
-00001a20: 0000 0072 3e00 0000 723f 0000 0072 4000  ...r>...r?...r@.
-00001a30: 0000 2902 7219 0000 0072 8d00 0000 720f  ..).r....r....r.
-00001a40: 0000 0072 0f00 0000 7210 0000 0072 8e00  ...r....r....r..
-00001a50: 0000 cb00 0000 7312 0000 0000 010c 010c  ......s.........
-00001a60: 010c 010c 010c 010c 010c 010c 017a 2d53  .............z-S
-00001a70: 7765 6570 5363 7265 656e 2e73 6574 5f70  weepScreen.set_p
-00001a80: 6172 616d 6574 6572 5f77 6964 6765 745f  arameter_widget_
-00001a90: 656e 6162 6c65 5f73 7461 7465 4672 8f00  enable_stateFr..
-00001aa0: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
-00001ab0: 0000 0003 0000 0043 0000 0073 4200 0000  .......C...sB...
-00001ac0: 7c01 721e 7c00 6a00 a001 6401 a101 0100  |.r.|.j...d.....
-00001ad0: 7c00 6a00 a002 6402 a101 0100 6e20 7c00  |.j...d.....n |.
-00001ae0: 6a00 a001 6403 a101 0100 7c00 6a00 a002  j...d.....|.j...
-00001af0: 7c02 7238 6404 6e02 6405 a101 0100 6400  |.r8d.n.d.....d.
-00001b00: 5300 2906 4e46 7a07 5761 6974 2e2e 2e54  S.).NFz.Wait...T
-00001b10: 7a0a 5374 6f70 2053 7765 6570 721f 0000  z.Stop Sweepr...
-00001b20: 0029 0372 4500 0000 7291 0000 00da 0773  .).rE...r......s
-00001b30: 6574 5465 7874 2903 7219 0000 0072 8700  etText).r....r..
-00001b40: 0000 7290 0000 0072 0f00 0000 720f 0000  ..r....r....r...
-00001b50: 0072 1000 0000 728a 0000 00d6 0000 0073  .r....r........s
-00001b60: 0a00 0000 0001 0401 0c01 0e02 0c01 7a23  ..............z#
-00001b70: 5377 6565 7053 6372 6565 6e2e 7374 6172  SweepScreen.star
-00001b80: 745f 7374 6f70 5f62 7574 746f 6e5f 7374  t_stop_button_st
-00001b90: 6174 6563 0100 0000 0000 0000 0000 0000  atec............
-00001ba0: 0100 0000 0200 0000 4300 0000 7314 0000  ........C...s...
-00001bb0: 007c 00a0 00a1 0001 007c 00a0 01a1 0001  .|.......|......
-00001bc0: 0064 0053 0072 1500 0000 2902 725c 0000  .d.S.r....).r\..
-00001bd0: 00da 1375 7064 6174 655f 7265 7375 6c74  ...update_result
-00001be0: 5f74 6162 6c65 7218 0000 0072 0f00 0000  _tabler....r....
-00001bf0: 720f 0000 0072 1000 0000 7276 0000 00de  r....r....rv....
-00001c00: 0000 0073 0400 0000 0001 0801 7a19 5377  ...s........z.Sw
-00001c10: 6565 7053 6372 6565 6e2e 7368 6f77 5f6e  eepScreen.show_n
-00001c20: 6577 5f64 6174 6163 0100 0000 0000 0000  ew_datac........
-00001c30: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00001c40: 7318 0000 007c 006a 00a0 01a1 0001 007c  s....|.j.......|
-00001c50: 006a 02a0 01a1 0001 0064 0053 0072 1500  .j.......d.S.r..
-00001c60: 0000 2903 724f 0000 0072 8500 0000 7250  ..).rO...r....rP
-00001c70: 0000 0072 1800 0000 720f 0000 0072 0f00  ...r....r....r..
-00001c80: 0000 7210 0000 0072 7800 0000 e200 0000  ..r....rx.......
-00001c90: 7304 0000 0000 010a 017a 1c53 7765 6570  s........z.Sweep
-00001ca0: 5363 7265 656e 2e73 6574 5f64 6174 615f  Screen.set_data_
-00001cb0: 696e 7661 6c69 6463 0100 0000 0000 0000  invalidc........
-00001cc0: 0000 0000 0200 0000 0600 0000 4300 0000  ............C...
-00001cd0: 733e 0000 007c 006a 00a0 01a1 007d 017c  s>...|.j.....}.|
-00001ce0: 006a 026a 0374 046a 057c 016a 0564 0164  .j.j.t.j.|.j.d.d
-00001cf0: 0264 038d 0401 007c 006a 026a 0374 046a  .d.....|.j.j.t.j
-00001d00: 067c 016a 0664 0464 0264 038d 0401 0064  .|.j.d.d.d.....d
-00001d10: 0053 0029 054e 727a 0000 00e9 0300 0000  .S.).Nrz........
-00001d20: 2901 da09 7072 6563 6973 696f 6eda 0029  )...precision..)
-00001d30: 0772 1c00 0000 da0a 6765 745f 7265 7375  .r......get_resu
-00001d40: 6c74 7252 0000 00da 0973 6574 5f76 616c  ltrR.....set_val
-00001d50: 7565 7205 0000 0072 0c00 0000 720d 0000  uer....r....r...
-00001d60: 0029 0272 1900 0000 da03 7265 7372 0f00  .).r......resr..
-00001d70: 0000 720f 0000 0072 1000 0000 7293 0000  ..r....r....r...
-00001d80: 00e6 0000 0073 0600 0000 0001 0a01 1801  .....s..........
-00001d90: 7a1f 5377 6565 7053 6372 6565 6e2e 7570  z.SweepScreen.up
-00001da0: 6461 7465 5f72 6573 756c 745f 7461 626c  date_result_tabl
-00001db0: 6563 0100 0000 0000 0000 0000 0000 0400  ec..............
-00001dc0: 0000 0500 0000 4300 0000 73c8 0000 007c  ......C...s....|
-00001dd0: 006a 006a 016a 026a 0374 046a 056a 066b  .j.j.j.j.t.j.j.k
-00001de0: 027d 017c 006a 07a0 087c 01a1 0101 007c  .}.|.j...|.....|
-00001df0: 006a 07a0 097c 01a1 0101 007c 006a 0aa0  .j...|.....|.j..
-00001e00: 087c 01a1 0101 007c 006a 00a0 0ba1 007d  .|.....|.j.....}
-00001e10: 027c 006a 00a0 0ca1 007d 037c 006a 07a0  .|.j.....}.|.j..
-00001e20: 0da1 0001 007c 006a 0aa0 0da1 0001 007c  .....|.j.......|
-00001e30: 026a 0e72 927c 006a 076a 0f7c 026a 107c  .j.r.|.j.j.|.j.|
-00001e40: 026a 1164 0164 028d 0301 007c 006a 0a6a  .j.d.d.....|.j.j
-00001e50: 0f7c 026a 107c 026a 1264 0164 028d 0301  .|.j.|.j.d.d....
-00001e60: 007c 036a 0e72 c47c 006a 076a 0f7c 036a  .|.j.r.|.j.j.|.j
-00001e70: 137c 036a 1464 0364 028d 0301 007c 006a  .|.j.d.d.....|.j
-00001e80: 0a6a 0f7c 036a 137c 036a 1564 0364 028d  .j.|.j.|.j.d.d..
-00001e90: 0301 0064 0053 0029 044e 7201 0000 0029  ...d.S.).Nr....)
-00001ea0: 03da 0178 da01 79da 0b6c 6179 6572 5f69  ...x..y..layer_i
-00001eb0: 6e64 6578 7206 0000 0029 1672 1c00 0000  ndexr....).r....
-00001ec0: 725f 0000 0072 6000 0000 da05 7661 6c75  r_...r`.....valu
-00001ed0: 6572 0400 0000 da0b 506c 6f74 5374 796c  er......PlotStyl
-00001ee0: 6549 4472 1200 0000 724f 0000 00da 0e73  eIDr....rO.....s
-00001ef0: 6574 5f6c 6f67 5f6d 6f64 655f 78da 0e73  et_log_mode_x..s
-00001f00: 6574 5f6c 6f67 5f6d 6f64 655f 7972 5000  et_log_mode_yrP.
-00001f10: 0000 da10 6765 745f 7377 6565 705f 7265  ....get_sweep_re
-00001f20: 7375 6c74 da0e 6765 745f 6669 745f 7265  sult..get_fit_re
-00001f30: 7375 6c74 7285 0000 00da 0972 6573 756c  sultr......resul
-00001f40: 745f 6f6b da09 706c 6f74 5f64 6174 61da  t_ok..plot_data.
-00001f50: 0b72 6573 756c 745f 6672 6571 da10 7265  .result_freq..re
-00001f60: 7375 6c74 5f61 6d70 6c69 7475 6465 da0c  sult_amplitude..
-00001f70: 7265 7375 6c74 5f70 6861 7365 da0f 7265  result_phase..re
-00001f80: 7375 6c74 5f66 6974 5f66 7265 71da 1472  sult_fit_freq..r
-00001f90: 6573 756c 745f 6669 745f 616d 706c 6974  esult_fit_amplit
-00001fa0: 7564 65da 1072 6573 756c 745f 6669 745f  ude..result_fit_
-00001fb0: 7068 6173 6529 0472 1900 0000 5a09 6c6f  phase).r....Z.lo
-00001fc0: 675f 7374 796c 655a 1563 7572 7265 6e74  g_styleZ.current
-00001fd0: 5f6d 6561 7375 7265 645f 6461 7461 5a13  _measured_dataZ.
-00001fe0: 6375 7272 656e 745f 6669 7474 6564 5f64  current_fitted_d
-00001ff0: 6174 6172 0f00 0000 720f 0000 0072 1000  atar....r....r..
-00002000: 0000 725c 0000 00eb 0000 0073 1c00 0000  ..r\.......s....
-00002010: 0001 1401 0c01 0c01 0c01 0a01 0a02 0a01  ................
-00002020: 0a01 0601 1601 1601 0601 1601 7a17 5377  ............z.Sw
-00002030: 6565 7053 6372 6565 6e2e 7570 6461 7465  eepScreen.update
-00002040: 5f70 6c6f 7463 0100 0000 0000 0000 0000  _plotc..........
-00002050: 0000 0200 0000 0300 0000 4300 0000 7324  ..........C...s$
-00002060: 0000 007c 006a 00a0 01a1 0001 007c 006a  ...|.j.......|.j
-00002070: 02a0 03a1 007d 017c 006a 00a0 047c 01a1  .....}.|.j...|..
-00002080: 0101 0064 0053 0072 1500 0000 2905 7223  ...d.S.r....).r#
-00002090: 0000 00da 0563 6c65 6172 721c 0000 00da  .....clearr.....
-000020a0: 1367 6574 5f63 616e 7469 6c65 7665 725f  .get_cantilever_
-000020b0: 6c69 7374 da08 6164 6449 7465 6d73 2902  list..addItems).
-000020c0: 7219 0000 00da 0f63 616e 7469 6c65 7665  r......cantileve
-000020d0: 725f 6c69 7374 720f 0000 0072 0f00 0000  r_listr....r....
-000020e0: 7210 0000 0072 2400 0000 fc00 0000 7306  r....r$.......s.
-000020f0: 0000 0000 010a 010a 017a 2253 7765 6570  .........z"Sweep
-00002100: 5363 7265 656e 2e75 7064 6174 655f 6361  Screen.update_ca
-00002110: 6e74 696c 6576 6572 5f6c 6973 7463 0100  ntilever_listc..
-00002120: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00002130: 0000 4300 0000 732e 0000 007c 006a 00a0  ..C...s....|.j..
-00002140: 01a1 007c 006a 026a 035f 047c 006a 00a0  ...|.j.j._.|.j..
-00002150: 05a1 007c 006a 026a 035f 067c 006a 02a0  ...|.j.j._.|.j..
-00002160: 07a1 0001 0064 0053 0072 1500 0000 2908  .....d.S.r....).
-00002170: 7223 0000 00da 0b63 7572 7265 6e74 5465  r#.....currentTe
-00002180: 7874 721c 0000 00da 0a63 616e 7469 6c65  xtr......cantile
-00002190: 7665 72da 046e 616d 65da 0c63 7572 7265  ver..name..curre
-000021a0: 6e74 496e 6465 78da 0569 6e64 6578 da11  ntIndex..index..
-000021b0: 7365 6c65 6374 5f63 616e 7469 6c65 7665  select_cantileve
-000021c0: 7272 1800 0000 720f 0000 0072 0f00 0000  rr....r....r....
-000021d0: 7210 0000 0072 6b00 0000 0101 0000 7306  r....rk.......s.
-000021e0: 0000 0000 0110 0110 017a 1d53 7765 6570  .........z.Sweep
-000021f0: 5363 7265 656e 2e75 7064 6174 655f 6361  Screen.update_ca
-00002200: 6e74 696c 6576 6572 6301 0000 0000 0000  ntileverc.......
-00002210: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-00002220: 0073 1a00 0000 7c00 6a00 a001 a100 7d01  .s....|.j.....}.
-00002230: 7c00 6a02 a003 7c01 a101 0100 6400 5300  |.j...|.....d.S.
-00002240: 7215 0000 0029 0472 2900 0000 729d 0000  r....).r)...r...
-00002250: 0072 1c00 0000 da18 7365 6c65 6374 5f65  .r......select_e
-00002260: 7863 6974 6174 696f 6e5f 6d65 7468 6f64  xcitation_method
-00002270: 2902 7219 0000 0072 6100 0000 720f 0000  ).r....ra...r...
-00002280: 0072 0f00 0000 7210 0000 00da 1875 7064  .r....r......upd
-00002290: 6174 655f 6578 6369 7461 7469 6f6e 5f6d  ate_excitation_m
-000022a0: 6574 686f 6406 0100 0073 0400 0000 0001  ethod....s......
-000022b0: 0a01 7a24 5377 6565 7053 6372 6565 6e2e  ..z$SweepScreen.
-000022c0: 7570 6461 7465 5f65 7863 6974 6174 696f  update_excitatio
-000022d0: 6e5f 6d65 7468 6f64 2901 5429 0246 4629  n_method).T).FF)
-000022e0: 1872 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
-000022f0: 7217 0000 0072 0300 0000 da14 4672 6571  r....r......Freq
-00002300: 7565 6e63 7953 7765 6570 4d6f 6475 6c65  uencySweepModule
-00002310: 725d 0000 0072 5900 0000 725a 0000 0072  r]...rY...rZ...r
-00002320: 6e00 0000 7270 0000 0072 7300 0000 725b  n...rp...rs...r[
-00002330: 0000 00da 0462 6f6f 6c72 8e00 0000 728a  .....boolr....r.
-00002340: 0000 0072 7600 0000 7278 0000 0072 9300  ...rv...rx...r..
-00002350: 0000 725c 0000 0072 2400 0000 726b 0000  ..r\...r$...rk..
-00002360: 0072 b600 0000 da0d 5f5f 636c 6173 7363  .r......__classc
-00002370: 656c 6c5f 5f72 0f00 0000 720f 0000 0072  ell__r....r....r
-00002380: 1a00 0000 7210 0000 0072 1400 0000 2300  ....r....r....#.
-00002390: 0000 7322 0000 0008 010c 0410 6308 1d08  ..s"........c...
-000023a0: 0f08 0708 0408 0508 0410 0b12 0808 0408  ................
-000023b0: 0408 0508 1108 0508 0572 1400 0000 292d  .........r....)-
-000023c0: 720b 0000 00da 0750 7953 6964 6536 7202  r......PySide6r.
-000023d0: 0000 00da 086e 616e 6f73 7572 6672 2500  .....nanosurfr%.
-000023e0: 0000 da29 6e61 6e6f 7375 7266 2e6c 6962  ...)nanosurf.lib
-000023f0: 2e73 706d 2e77 6f72 6b66 6c6f 772e 6672  .spm.workflow.fr
-00002400: 6571 7565 6e63 795f 7377 6565 70da 036c  equency_sweep..l
-00002410: 6962 da03 7370 6dda 0877 6f72 6b66 6c6f  ib..spm..workflo
-00002420: 77da 0f66 7265 7175 656e 6379 5f73 7765  w..frequency_swe
-00002430: 6570 722b 0000 00da 1666 7265 7175 656e  epr+.....frequen
-00002440: 6379 5f73 7765 6570 5f6d 6f64 756c 6572  cy_sweep_moduler
-00002450: 0300 0000 7204 0000 0072 2600 0000 da0d  ....r....r&.....
-00002460: 5461 626c 6545 6e74 7279 4944 7372 0500  TableEntryIDsr..
-00002470: 0000 da0d 4e53 4643 6f6d 626f 456e 7472  ....NSFComboEntr
-00002480: 7972 9e00 0000 7211 0000 0072 1200 0000  yr....r....r....
-00002490: 7254 0000 00da 1245 7863 6974 6174 696f  rT.....Excitatio
-000024a0: 6e4d 6574 686f 6449 4472 1300 0000 da0a  nMethodIDr......
-000024b0: 5069 657a 6f44 7269 7665 7228 0000 0072  PiezoDriver(...r
-000024c0: 3800 0000 7239 0000 0072 3a00 0000 da04  8...r9...r:.....
-000024d0: 6261 7365 5a13 616c 6c6f 7765 645f 636f  baseZ.allowed_co
-000024e0: 756e 745f 756e 6974 73da 056d 696c 6c69  unt_units..milli
-000024f0: 5a12 616c 6c6f 7765 645f 7469 6d65 5f75  Z.allowed_time_u
-00002500: 6e69 7473 da05 6d69 6372 6fda 046e 616e  nits..micro..nan
-00002510: 6f5a 1361 6c6c 6f77 6564 5f6d 6574 6572  oZ.allowed_meter
-00002520: 5f75 6e69 7473 da04 6d65 6761 da04 6b69  _units..mega..ki
-00002530: 6c6f 7236 0000 0072 4100 0000 5a1d 616c  lor6...rA...Z.al
-00002540: 6c6f 7765 645f 7370 7269 6e67 5f63 6f6e  lowed_spring_con
-00002550: 7374 616e 745f 756e 6974 7372 4a00 0000  stant_unitsrJ...
-00002560: 724b 0000 00da 0c4d 6f64 756c 6553 6372  rK.....ModuleScr
-00002570: 6565 6e72 1400 0000 720f 0000 0072 0f00  eenr....r....r..
-00002580: 0000 720f 0000 0072 1000 0000 da08 3c6d  ..r....r......<m
-00002590: 6f64 756c 653e 0100 0000 7324 0000 0004  odule>....s$....
-000025a0: 050c 0108 011e 0110 0214 0710 0110 fe04  ................
-000025b0: 0610 0110 fe04 060e 0118 0122 0122 0122  ..........."."."
-000025c0: 010e 02                                  ...
+00000740: 007c 005f 2f7c 006a 2fa0 307c 006a 0ba1  .|._/|.j/.0|.j..
+00000750: 0101 007c 006a 2fa0 307c 006a 11a1 0101  ...|.j/.0|.j....
+00000760: 007c 006a 2fa0 307c 006a 14a1 0101 007c  .|.j/.0|.j.....|
+00000770: 006a 2fa0 307c 006a 17a1 0101 007c 006a  .j/.0|.j.....|.j
+00000780: 2fa0 307c 006a 19a1 0101 007c 006a 2fa0  /.0|.j.....|.j/.
+00000790: 307c 006a 23a1 0101 007c 006a 2fa0 307c  0|.j#....|.j/.0|
+000007a0: 006a 24a1 0101 007c 006a 2fa0 307c 006a  .j$....|.j/.0|.j
+000007b0: 25a1 0101 007c 006a 2fa0 31a1 0001 007c  %....|.j/.1....|
+000007c0: 006a 2fa0 307c 006a 2ca1 0101 007c 006a  .j/.0|.j,....|.j
+000007d0: 2fa0 3274 076a 336a 346a 35a0 36a1 00a1  /.2t.j3j4j5.6...
+000007e0: 0101 0074 076a 08a0 37a1 007c 005f 3874  ...t.j..7..|._8t
+000007f0: 076a 08a0 37a1 007c 005f 3974 076a 08a0  .j..7..|._9t.j..
+00000800: 3a74 3ba1 017c 005f 3c7c 006a 3ca0 3d74  :t;..|._<|.j<.=t
+00000810: 3b6a 3e64 11a1 0201 007c 006a 3ca0 3d74  ;j>d.....|.j<.=t
+00000820: 3b6a 3f64 12a1 0201 0074 01a0 2ea1 007c  ;j?d.....t.....|
+00000830: 005f 407c 006a 40a0 307c 006a 38a1 0101  ._@|.j@.0|.j8...
+00000840: 007c 006a 40a0 307c 006a 39a1 0101 007c  .|.j@.0|.j9....|
+00000850: 006a 40a0 307c 006a 3ca1 0101 007c 006a  .j@.0|.j<....|.j
+00000860: 40a0 3274 076a 336a 346a 35a0 36a1 00a1  @.2t.j3j4j5.6...
+00000870: 0101 0074 076a 08a0 0974 4164 13a1 027c  ...t.j...tAd...|
+00000880: 005f 4274 01a0 2ea1 007c 005f 437c 006a  ._Bt.....|._C|.j
+00000890: 43a0 307c 006a 42a1 0101 007c 006a 43a0  C.0|.jB....|.jC.
+000008a0: 3274 076a 336a 346a 35a0 36a1 00a1 0101  2t.j3j4j5.6.....
+000008b0: 0074 01a0 44a1 007c 005f 457c 006a 45a0  .t..D..|._E|.jE.
+000008c0: 467c 006a 2f64 07a1 0201 007c 006a 45a0  F|.j/d.....|.jE.
+000008d0: 467c 006a 4064 0ba1 0201 007c 006a 45a0  F|.j@d.....|.jE.
+000008e0: 467c 006a 4364 07a1 0201 007c 00a0 477c  F|.jCd.....|..G|
+000008f0: 006a 45a1 0101 007c 00a0 48a1 0001 007c  .jE....|..H....|
+00000900: 00a0 49a1 0001 007c 00a0 4aa1 0001 007c  ..I....|..J....|
+00000910: 00a0 4ba1 0001 0064 1453 0029 157a 3820  ..K....d.S.).z8 
+00000920: 6372 6561 7465 2068 6572 6520 796f 7572  create here your
+00000930: 2067 7569 2077 6974 6820 616c 6c20 636f   gui with all co
+00000940: 6e74 726f 6c73 2061 6e64 2074 6865 6972  ntrols and their
+00000950: 206c 6179 6f75 74da 0a43 616e 7469 6c65   layout..Cantile
+00000960: 7665 727a 1145 7863 6974 6174 696f 6e20  verz.Excitation 
+00000970: 4d65 7468 6f64 7a0c 496e 7075 7420 536f  Methodz.Input So
+00000980: 7572 6365 7a0d 4f75 7470 7574 2053 6f75  urcez.Output Sou
+00000990: 7263 655a 0942 616e 6477 6964 7468 7a10  rceZ.Bandwidthz.
+000009a0: 4365 6e74 6572 2046 7265 7175 656e 6379  Center Frequency
+000009b0: 7201 0000 007a 0f46 7265 7175 656e 6379  r....z.Frequency
+000009c0: 2052 616e 6765 7a0f 4672 6571 7565 6e63   Rangez.Frequenc
+000009d0: 7920 5374 6570 737a 1445 7863 6974 6174  y Stepsz.Excitat
+000009e0: 696f 6e20 416d 706c 6974 7564 6572 0600  ion Amplituder..
+000009f0: 0000 7207 0000 007a 0a45 6d69 7420 5469  ..r....z.Emit Ti
+00000a00: 636b 73da 0841 7070 726f 6163 68fa 0b53  cks..Approach..S
+00000a10: 7461 7274 2053 7765 6570 da04 5361 7665  tart Sweep..Save
+00000a20: 7a13 5265 736f 6e61 6e63 6520 4672 6571  z.Resonance Freq
+00000a30: 7565 6e63 797a 0851 2d46 6163 746f 727a  uencyz.Q-Factorz
+00000a40: 0a50 6c6f 7420 5374 796c 654e 294c 721c  .Plot StyleN)Lr.
+00000a50: 0000 0072 0200 0000 da06 514c 6162 656c  ...r......QLabel
+00000a60: 5a10 6c61 6265 6c5f 6361 6e74 696c 6576  Z.label_cantilev
+00000a70: 6572 da09 5143 6f6d 626f 426f 78da 1063  er..QComboBox..c
+00000a80: 6f6d 626f 5f63 616e 7469 6c65 7665 72da  ombo_cantilever.
+00000a90: 1675 7064 6174 655f 6361 6e74 696c 6576  .update_cantilev
+00000aa0: 6572 5f6c 6973 74da 036e 7366 da03 6775  er_list..nsf..gu
+00000ab0: 69da 0b4e 5346 436f 6d62 6f42 6f78 da16  i..NSFComboBox..
+00000ac0: 436f 6d62 6f45 7863 6974 6174 696f 6e4d  ComboExcitationM
+00000ad0: 6574 686f 6473 da17 636f 6d62 6f5f 6578  ethods..combo_ex
+00000ae0: 6369 7461 7469 6f6e 5f6d 6574 686f 64da  citation_method.
+00000af0: 1b63 7265 6174 655f 656e 7472 795f 6c69  .create_entry_li
+00000b00: 7374 5f66 726f 6d5f 6469 6374 da0a 6672  st_from_dict..fr
+00000b10: 6571 5f73 7765 6570 da0e 4672 6571 7565  eq_sweep..Freque
+00000b20: 6e63 7953 7765 6570 da13 696e 7075 745f  ncySweep..input_
+00000b30: 736f 7572 6365 735f 6e61 6d65 735a 1863  sources_namesZ.c
+00000b40: 6f6d 626f 5f69 6e70 7574 5f73 6f75 7263  ombo_input_sourc
+00000b50: 655f 6974 656d 73da 1263 6f6d 626f 5f69  e_items..combo_i
+00000b60: 6e70 7574 5f73 6f75 7263 65da 0c6f 7574  nput_source..out
+00000b70: 7075 745f 6e61 6d65 735a 1963 6f6d 626f  put_namesZ.combo
+00000b80: 5f6f 7574 7075 745f 736f 7572 6365 5f69  _output_source_i
+00000b90: 7465 6d73 da13 636f 6d62 6f5f 6f75 7470  tems..combo_outp
+00000ba0: 7574 5f73 6f75 7263 65da 1062 616e 6477  ut_source..bandw
+00000bb0: 6964 7468 735f 6e61 6d65 735a 1563 6f6d  idths_namesZ.com
+00000bc0: 626f 5f62 616e 6477 6964 7468 5f69 7465  bo_bandwidth_ite
+00000bd0: 6d73 da0f 636f 6d62 6f5f 6261 6e64 7769  ms..combo_bandwi
+00000be0: 6474 68da 0a4e 5346 5363 6945 6469 74da  dth..NSFSciEdit.
+00000bf0: 1773 6369 7661 6c5f 6365 6e74 6572 5f66  .scival_center_f
+00000c00: 7265 7175 656e 6379 da16 7365 745f 616c  requency..set_al
+00000c10: 6c6f 7765 645f 7072 6566 6978 5f69 6473  lowed_prefix_ids
+00000c20: da17 616c 6c6f 7765 645f 6672 6571 7565  ..allowed_freque
+00000c30: 6e63 795f 756e 6974 73da 0d73 6574 5f70  ncy_units..set_p
+00000c40: 7265 6669 785f 6964 da07 7363 695f 7661  refix_id..sci_va
+00000c50: 6cda 0275 70da 0650 7265 6669 78da 0561  l..up..Prefix..a
+00000c60: 7574 6f5f da0d 7365 745f 7072 6563 6973  uto_..set_precis
+00000c70: 696f 6eda 0d73 6574 5f76 616c 7565 5f6d  ion..set_value_m
+00000c80: 696e da16 7363 6976 616c 5f66 7265 7175  in..scival_frequ
+00000c90: 656e 6379 5f72 616e 6765 da16 7363 6976  ency_range..sciv
+00000ca0: 616c 5f66 7265 7175 656e 6379 5f73 7465  al_frequency_ste
+00000cb0: 7073 da1b 7363 6976 616c 5f65 7863 6974  ps..scival_excit
+00000cc0: 6174 696f 6e5f 616d 706c 6974 7564 65da  ation_amplitude.
+00000cd0: 1561 6c6c 6f77 6564 5f76 6f6c 7461 6765  .allowed_voltage
+00000ce0: 5f75 6e69 7473 da0d 7365 745f 7661 6c75  _units..set_valu
+00000cf0: 655f 6d61 78da 0951 4368 6563 6b42 6f78  e_max..QCheckBox
+00000d00: 5a10 6368 6563 6b5f 656d 6974 5f74 6963  Z.check_emit_tic
+00000d10: 6b73 da0b 5150 7573 6842 7574 746f 6e5a  ks..QPushButtonZ
+00000d20: 0f62 7574 746f 6e5f 6170 7072 6f61 6368  .button_approach
+00000d30: da11 6275 7474 6f6e 5f73 7461 7274 5f73  ..button_start_s
+00000d40: 746f 705a 0b62 7574 746f 6e5f 7361 7665  topZ.button_save
+00000d50: da0b 5156 426f 784c 6179 6f75 745a 0b6c  ..QVBoxLayoutZ.l
+00000d60: 6179 6f75 745f 6c65 6674 da09 6164 6457  ayout_left..addW
+00000d70: 6964 6765 74da 0a61 6464 5374 7265 7463  idget..addStretc
+00000d80: 68da 0d61 6464 5370 6163 6572 4974 656d  h..addSpacerItem
+00000d90: da0a 6672 616d 6577 6f72 6b73 da06 7174  ..frameworks..qt
+00000da0: 5f61 7070 da07 6170 705f 6775 69da 0a53  _app..app_gui..S
+00000db0: 7464 5653 7061 6365 72da 084e 5346 4368  tdVSpacer..NSFCh
+00000dc0: 6172 74da 0e61 6d70 6c69 7475 6465 5f70  art..amplitude_p
+00000dd0: 6c6f 74da 0a70 6861 7365 5f70 6c6f 74da  lot..phase_plot.
+00000de0: 114e 5346 4e61 6d65 5661 6c75 6554 6162  .NSFNameValueTab
+00000df0: 6c65 7205 0000 00da 0c74 6162 6c65 5265  ler......tableRe
+00000e00: 7375 6c74 73da 0c64 6566 696e 655f 656e  sults..define_en
+00000e10: 7472 7972 0c00 0000 720d 0000 005a 0a6c  tryr....r....Z.l
+00000e20: 6179 6f75 745f 6d69 64da 0f43 6f6d 626f  ayout_mid..Combo
+00000e30: 506c 6f74 5374 796c 6573 da10 636f 6d62  PlotStyles..comb
+00000e40: 6f5f 706c 6f74 5f73 7479 6c65 5a0c 6c61  o_plot_styleZ.la
+00000e50: 796f 7574 5f72 6967 6874 da0b 5148 426f  yout_right..QHBo
+00000e60: 784c 6179 6f75 745a 0d73 6372 6565 6e5f  xLayoutZ.screen_
+00000e70: 6c61 796f 7574 da09 6164 644c 6179 6f75  layout..addLayou
+00000e80: 74da 0973 6574 4c61 796f 7574 da11 6269  t..setLayout..bi
+00000e90: 6e64 5f67 7569 5f65 6c65 6d65 6e74 73da  nd_gui_elements.
+00000ea0: 0969 6e69 745f 706c 6f74 da14 656e 7465  .init_plot..ente
+00000eb0: 725f 6775 695f 7374 6174 655f 6964 6c65  r_gui_state_idle
+00000ec0: da0b 7570 6461 7465 5f70 6c6f 7429 0272  ..update_plot).r
+00000ed0: 1900 0000 721c 0000 0072 0f00 0000 720f  ....r....r....r.
+00000ee0: 0000 0072 1000 0000 da0f 646f 5f73 6574  ...r......do_set
+00000ef0: 7570 5f73 6372 6565 6e28 0000 0073 8e00  up_screen(...s..
+00000f00: 0000 0002 0603 0c01 0a01 0802 1002 1401  ................
+00000f10: 1202 1401 1202 1401 1202 0e01 0c01 1401  ................
+00000f20: 0c01 0c02 0e01 0c01 1401 0c01 0c02 0e01  ................
+00000f30: 0c01 1401 0c01 0c02 0e01 0c01 1401 0c01  ................
+00000f40: 0c01 0c02 0c01 0c01 0c01 0c02 0a03 0e01  ................
+00000f50: 0e01 0e01 0e01 0e01 0e01 0e01 0e01 0a01  ................
+00000f60: 0e01 1603 0c01 0c01 0e01 1001 1002 0a01  ................
+00000f70: 0e01 0e01 0e01 1603 1002 0a01 0e01 1603  ................
+00000f80: 0a02 1001 1001 1002 0c02 0801 0801 0801  ................
+00000f90: 7a1b 5377 6565 7053 6372 6565 6e2e 646f  z.SweepScreen.do
+00000fa0: 5f73 6574 7570 5f73 6372 6565 6e63 0100  _setup_screenc..
+00000fb0: 0000 0000 0000 0000 0000 0100 0000 0400  ................
+00000fc0: 0000 4300 0000 735e 0100 0074 006a 01a0  ..C...s^...t.j..
+00000fd0: 027c 006a 037c 006a 046a 056a 06a1 0201  .|.j.|.j.j.j....
+00000fe0: 0074 006a 01a0 027c 006a 077c 006a 046a  .t.j...|.j.|.j.j
+00000ff0: 056a 08a1 0201 0074 006a 01a0 027c 006a  .j.....t.j...|.j
+00001000: 097c 006a 046a 056a 0aa1 0201 0074 006a  .|.j.j.j.....t.j
+00001010: 01a0 027c 006a 0b7c 006a 046a 056a 0ca1  ...|.j.|.j.j.j..
+00001020: 0201 0074 006a 01a0 027c 006a 0d7c 006a  ...t.j...|.j.|.j
+00001030: 046a 056a 0ea1 0201 0074 006a 01a0 027c  .j.j.....t.j...|
+00001040: 006a 0f7c 006a 046a 056a 10a1 0201 0074  .j.|.j.j.j.....t
+00001050: 006a 01a0 027c 006a 117c 006a 046a 056a  .j...|.j.|.j.j.j
+00001060: 12a1 0201 0074 006a 01a0 027c 006a 137c  .....t.j...|.j.|
+00001070: 006a 046a 056a 14a1 0201 0074 006a 01a0  .j.j.j.....t.j..
+00001080: 027c 006a 157c 006a 046a 056a 16a1 0201  .|.j.|.j.j.j....
+00001090: 007c 006a 176a 18a0 197c 006a 1aa1 0101  .|.j.j...|.j....
+000010a0: 007c 006a 046a 056a 066a 1ba0 197c 006a  .|.j.j.j.j...|.j
+000010b0: 1ca1 0101 007c 006a 1d6a 1ea0 197c 006a  .....|.j.j...|.j
+000010c0: 1fa1 0101 007c 006a 046a 20a0 197c 006a  .....|.j.j ..|.j
+000010d0: 21a1 0101 007c 006a 046a 22a0 197c 006a  !....|.j.j"..|.j
+000010e0: 21a1 0101 007c 006a 046a 23a0 197c 006a  !....|.j.j#..|.j
+000010f0: 24a1 0101 007c 006a 046a 25a0 197c 006a  $....|.j.j%..|.j
+00001100: 26a1 0101 007c 006a 046a 27a0 197c 006a  &....|.j.j'..|.j
+00001110: 28a1 0101 007c 006a 046a 29a0 197c 006a  (....|.j.j)..|.j
+00001120: 2aa1 0101 0064 0153 0029 027a 4b20 636f  *....d.S.).zK co
+00001130: 6e6e 6563 7420 6865 7265 2061 6c6c 2067  nnect here all g
+00001140: 7569 2077 6964 6765 7473 2074 6f20 7365  ui widgets to se
+00001150: 7474 696e 6773 206f 6620 7468 6520 6d6f  ttings of the mo
+00001160: 6475 6c65 206f 7220 616e 7920 6f74 6865  dule or any othe
+00001170: 7220 736f 7572 6365 4e29 2b72 2500 0000  r sourceN)+r%...
+00001180: 7226 0000 00da 1363 6f6e 6e65 6374 5f74  r&.....connect_t
+00001190: 6f5f 7072 6f70 6572 7479 7255 0000 0072  o_propertyrU...r
+000011a0: 1c00 0000 da08 7365 7474 696e 6773 da0d  ......settings..
+000011b0: 706c 6f74 5f73 7479 6c65 5f69 6472 2900  plot_style_idr).
+000011c0: 0000 da11 6578 6369 7461 7469 6f6e 5f6d  ....excitation_m
+000011d0: 6574 686f 6472 2e00 0000 da0c 696e 7075  ethodr......inpu
+000011e0: 745f 736f 7572 6365 7230 0000 00da 0d6f  t_sourcer0.....o
+000011f0: 7574 7075 745f 736f 7572 6365 7232 0000  utput_sourcer2..
+00001200: 00da 0962 616e 6477 6964 7468 7234 0000  ...bandwidthr4..
+00001210: 00da 1063 656e 7465 725f 6672 6571 7565  ...center_freque
+00001220: 6e63 7972 3e00 0000 da0f 6672 6571 7565  ncyr>.....freque
+00001230: 6e63 795f 7261 6e67 6572 3f00 0000 da0f  ncy_ranger?.....
+00001240: 6672 6571 7565 6e63 795f 7374 6570 7372  frequency_stepsr
+00001250: 4000 0000 da14 6578 6369 7461 7469 6f6e  @.....excitation
+00001260: 5f61 6d70 6c69 7475 6465 7223 0000 00da  _amplituder#....
+00001270: 0961 6374 6976 6174 6564 da07 636f 6e6e  .activated..conn
+00001280: 6563 74da 1175 7064 6174 655f 6361 6e74  ect..update_cant
+00001290: 696c 6576 6572 da11 7369 675f 7661 6c75  ilever..sig_valu
+000012a0: 655f 6368 616e 6765 6472 5c00 0000 7245  e_changedr\...rE
+000012b0: 0000 00da 0763 6c69 636b 6564 da1c 6f6e  .....clicked..on
+000012c0: 5f62 7574 746f 6e5f 7374 6172 745f 7374  _button_start_st
+000012d0: 6f70 5f63 6c69 636b 6564 da18 7369 675f  op_clicked..sig_
+000012e0: 776f 726b 5f73 7461 7274 5f72 6571 7565  work_start_reque
+000012f0: 7374 6564 da14 656e 7465 725f 6775 695f  sted..enter_gui_
+00001300: 7374 6174 655f 7761 6974 da17 7369 675f  state_wait..sig_
+00001310: 776f 726b 5f73 746f 705f 7265 7175 6573  work_stop_reques
+00001320: 7465 64da 0f73 6967 5f77 6f72 6b5f 6163  ted..sig_work_ac
+00001330: 7469 7665 da16 656e 7465 725f 6775 695f  tive..enter_gui_
+00001340: 7374 6174 655f 6163 7469 7665 da0d 7369  state_active..si
+00001350: 675f 776f 726b 5f64 6f6e 6572 5b00 0000  g_work_doner[...
+00001360: da16 7369 675f 6e65 775f 6461 7461 5f61  ..sig_new_data_a
+00001370: 7661 696c 6162 6c65 da0d 7368 6f77 5f6e  vailable..show_n
+00001380: 6577 5f64 6174 61da 1073 6967 5f64 6174  ew_data..sig_dat
+00001390: 615f 696e 7661 6c69 64da 1073 6574 5f64  a_invalid..set_d
+000013a0: 6174 615f 696e 7661 6c69 6472 1800 0000  ata_invalidr....
+000013b0: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+000013c0: 5900 0000 8b00 0000 7324 0000 0000 0416  Y.......s$......
+000013d0: 0116 0116 0116 0116 0116 0116 0116 0116  ................
+000013e0: 0310 0114 0310 0310 0110 0110 0110 0110  ................
+000013f0: 017a 1d53 7765 6570 5363 7265 656e 2e62  .z.SweepScreen.b
+00001400: 696e 645f 6775 695f 656c 656d 656e 7473  ind_gui_elements
+00001410: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001420: 0004 0000 0043 0000 0073 e000 0000 7c00  .....C...s....|.
+00001430: 6a00 a001 6401 a101 0100 7c00 6a00 a002  j...d.....|.j...
+00001440: 7403 6a04 6a05 6a06 6a07 6402 a102 0100  t.j.j.j.j.d.....
+00001450: 7c00 6a00 a008 7403 6a04 6a05 6a06 6a07  |.j...t.j.j.j.j.
+00001460: 6403 a102 0100 7c00 6a00 a002 7403 6a04  d.....|.j...t.j.
+00001470: 6a05 6a06 6a09 6404 a102 0100 7c00 6a00  j.j.j.d.....|.j.
+00001480: a008 7403 6a04 6a05 6a06 6a09 6405 a102  ..t.j.j.j.j.d...
+00001490: 0100 7c00 6a00 a00a a100 0100 7c00 6a0b  ..|.j.......|.j.
+000014a0: a001 6406 a101 0100 7c00 6a0b a002 7403  ..d.....|.j...t.
+000014b0: 6a04 6a05 6a06 6a07 6402 a102 0100 7c00  j.j.j.j.d.....|.
+000014c0: 6a0b a008 7403 6a04 6a05 6a06 6a07 6403  j...t.j.j.j.j.d.
+000014d0: a102 0100 7c00 6a0b a002 7403 6a04 6a05  ....|.j...t.j.j.
+000014e0: 6a06 6a09 6407 a102 0100 7c00 6a0b a008  j.j.d.....|.j...
+000014f0: 7403 6a04 6a05 6a06 6a09 6408 a102 0100  t.j.j.j.j.d.....
+00001500: 7c00 6a0b a00a a100 0100 6400 5300 2909  |.j.......d.S.).
+00001510: 4e7a 1241 6d70 6c69 7475 6465 2053 7065  Nz.Amplitude Spe
+00001520: 6374 7275 6dda 0946 7265 7175 656e 6379  ctrum..Frequency
+00001530: da02 487a da09 416d 706c 6974 7564 65da  ..Hz..Amplitude.
+00001540: 0156 7a0e 5068 6173 6520 5370 6563 7472  .Vz.Phase Spectr
+00001550: 756d da05 5068 6173 65da 0364 6567 290c  um..Phase..deg).
+00001560: 724f 0000 00da 0973 6574 5f74 6974 6c65  rO.....set_title
+00001570: da09 7365 745f 6c61 6265 6c72 2500 0000  ..set_labelr%...
+00001580: 7226 0000 0072 4e00 0000 da04 4178 6973  r&...rN.....Axis
+00001590: da06 626f 7474 6f6d da08 7365 745f 756e  ..bottom..set_un
+000015a0: 6974 da04 6c65 6674 da0b 636c 6561 725f  it..left..clear_
+000015b0: 706c 6f74 7372 5000 0000 7218 0000 0072  plotsrP...r....r
+000015c0: 0f00 0000 720f 0000 0072 1000 0000 725a  ....r....r....rZ
+000015d0: 0000 00a8 0000 0073 1800 0000 0001 0c01  .......s........
+000015e0: 1601 1601 1601 1601 0a02 0c01 1601 1601  ................
+000015f0: 1601 1601 7a15 5377 6565 7053 6372 6565  ....z.SweepScree
+00001600: 6e2e 696e 6974 5f70 6c6f 7463 0100 0000  n.init_plotc....
+00001610: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00001620: 4300 0000 7330 0000 007c 006a 00a0 01a1  C...s0...|.j....
+00001630: 0072 227c 006a 00a0 02a1 0001 007c 006a  .r"|.j.......|.j
+00001640: 0364 0164 028d 0101 006e 0a7c 006a 00a0  .d.d.....n.|.j..
+00001650: 04a1 0001 0064 0053 0029 034e 54a9 01da  .....d.S.).NT...
+00001660: 0477 6169 7429 0572 1c00 0000 da0d 6973  .wait).r......is
+00001670: 5f73 7765 6570 5f62 7573 79da 0a73 746f  _sweep_busy..sto
+00001680: 705f 7377 6565 70da 1773 7461 7274 5f73  p_sweep..start_s
+00001690: 746f 705f 6275 7474 6f6e 5f73 7461 7465  top_button_state
+000016a0: da0b 7374 6172 745f 7377 6565 7072 1800  ..start_sweepr..
+000016b0: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+000016c0: 0072 6e00 0000 b700 0000 7308 0000 0000  .rn.......s.....
+000016d0: 010a 010a 010e 027a 2853 7765 6570 5363  .......z(SweepSc
+000016e0: 7265 656e 2e6f 6e5f 6275 7474 6f6e 5f73  reen.on_button_s
+000016f0: 7461 7274 5f73 746f 705f 636c 6963 6b65  tart_stop_clicke
+00001700: 6463 0100 0000 0000 0000 0000 0000 0100  dc..............
+00001710: 0000 0300 0000 4300 0000 731c 0000 007c  ......C...s....|
+00001720: 006a 0064 0164 028d 0101 007c 006a 0164  .j.d.d.....|.j.d
+00001730: 0364 048d 0101 0064 0053 0029 054e 46a9  .d.....d.S.).NF.
+00001740: 01da 0765 6e61 626c 6564 5472 8600 0000  ...enabledTr....
+00001750: 2902 da21 7365 745f 7061 7261 6d65 7465  )..!set_paramete
+00001760: 725f 7769 6467 6574 5f65 6e61 626c 655f  r_widget_enable_
+00001770: 7374 6174 6572 8a00 0000 7218 0000 0072  stater....r....r
+00001780: 0f00 0000 720f 0000 0072 1000 0000 7270  ....r....r....rp
+00001790: 0000 00be 0000 0073 0400 0000 0001 0c01  .......s........
+000017a0: 7a20 5377 6565 7053 6372 6565 6e2e 656e  z SweepScreen.en
+000017b0: 7465 725f 6775 695f 7374 6174 655f 7761  ter_gui_state_wa
+000017c0: 6974 6301 0000 0000 0000 0000 0000 0001  itc.............
+000017d0: 0000 0004 0000 0043 0000 0073 2c00 0000  .......C...s,...
+000017e0: 7c00 6a00 6401 6402 8d01 0100 7c00 6a01  |.j.d.d.....|.j.
+000017f0: 6401 7c00 6a02 a003 a100 6403 8d02 0100  d.|.j.....d.....
+00001800: 7c00 a004 a100 0100 6400 5300 2904 4e46  |.......d.S.).NF
+00001810: 728c 0000 00a9 0272 8700 0000 da0a 7374  r......r......st
+00001820: 6f70 5f73 7461 7465 2905 728e 0000 0072  op_state).r....r
+00001830: 8a00 0000 721c 0000 0072 8800 0000 725a  ....r....r....rZ
+00001840: 0000 0072 1800 0000 720f 0000 0072 0f00  ...r....r....r..
+00001850: 0000 7210 0000 0072 7300 0000 c200 0000  ..r....rs.......
+00001860: 7306 0000 0000 010c 0114 017a 2253 7765  s..........z"Swe
+00001870: 6570 5363 7265 656e 2e65 6e74 6572 5f67  epScreen.enter_g
+00001880: 7569 5f73 7461 7465 5f61 6374 6976 6563  ui_state_activec
+00001890: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000018a0: 0400 0000 4300 0000 7324 0000 007c 006a  ....C...s$...|.j
+000018b0: 0064 0164 028d 0101 007c 006a 0164 037c  .d.d.....|.j.d.|
+000018c0: 006a 02a0 03a1 0064 048d 0201 0064 0053  .j.....d.....d.S
+000018d0: 0029 054e 5472 8c00 0000 4672 8f00 0000  .).NTr....Fr....
+000018e0: 2904 728e 0000 0072 8a00 0000 721c 0000  ).r....r....r...
+000018f0: 0072 8800 0000 7218 0000 0072 0f00 0000  .r....r....r....
+00001900: 720f 0000 0072 1000 0000 725b 0000 00c7  r....r....r[....
+00001910: 0000 0073 0400 0000 0001 0c01 7a20 5377  ...s........z Sw
+00001920: 6565 7053 6372 6565 6e2e 656e 7465 725f  eepScreen.enter_
+00001930: 6775 695f 7374 6174 655f 6964 6c65 5472  gui_state_idleTr
+00001940: 8c00 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00001950: 0002 0000 0003 0000 0043 0000 0073 7000  .........C...sp.
+00001960: 0000 7c00 6a00 a001 7c01 a101 0100 7c00  ..|.j...|.....|.
+00001970: 6a02 a001 7c01 a101 0100 7c00 6a03 a001  j...|.....|.j...
+00001980: 7c01 a101 0100 7c00 6a04 a001 7c01 a101  |.....|.j...|...
+00001990: 0100 7c00 6a05 a001 7c01 a101 0100 7c00  ..|.j...|.....|.
+000019a0: 6a06 a001 7c01 a101 0100 7c00 6a07 a001  j...|.....|.j...
+000019b0: 7c01 a101 0100 7c00 6a08 a001 7c01 a101  |.....|.j...|...
+000019c0: 0100 7c00 6a09 a001 7c01 a101 0100 6400  ..|.j...|.....d.
+000019d0: 5300 7215 0000 0029 0a72 2300 0000 da0a  S.r....).r#.....
+000019e0: 7365 7445 6e61 626c 6564 7229 0000 0072  setEnabledr)...r
+000019f0: 2e00 0000 7230 0000 0072 3200 0000 7234  ....r0...r2...r4
+00001a00: 0000 0072 3e00 0000 723f 0000 0072 4000  ...r>...r?...r@.
+00001a10: 0000 2902 7219 0000 0072 8d00 0000 720f  ..).r....r....r.
+00001a20: 0000 0072 0f00 0000 7210 0000 0072 8e00  ...r....r....r..
+00001a30: 0000 cb00 0000 7312 0000 0000 010c 010c  ......s.........
+00001a40: 010c 010c 010c 010c 010c 010c 017a 2d53  .............z-S
+00001a50: 7765 6570 5363 7265 656e 2e73 6574 5f70  weepScreen.set_p
+00001a60: 6172 616d 6574 6572 5f77 6964 6765 745f  arameter_widget_
+00001a70: 656e 6162 6c65 5f73 7461 7465 4672 8f00  enable_stateFr..
+00001a80: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
+00001a90: 0000 0003 0000 0043 0000 0073 4200 0000  .......C...sB...
+00001aa0: 7c01 721e 7c00 6a00 a001 6401 a101 0100  |.r.|.j...d.....
+00001ab0: 7c00 6a00 a002 6402 a101 0100 6e20 7c00  |.j...d.....n |.
+00001ac0: 6a00 a001 6403 a101 0100 7c00 6a00 a002  j...d.....|.j...
+00001ad0: 7c02 7238 6404 6e02 6405 a101 0100 6400  |.r8d.n.d.....d.
+00001ae0: 5300 2906 4e46 7a07 5761 6974 2e2e 2e54  S.).NFz.Wait...T
+00001af0: 7a0a 5374 6f70 2053 7765 6570 721f 0000  z.Stop Sweepr...
+00001b00: 0029 0372 4500 0000 7291 0000 00da 0773  .).rE...r......s
+00001b10: 6574 5465 7874 2903 7219 0000 0072 8700  etText).r....r..
+00001b20: 0000 7290 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+00001b30: 0072 1000 0000 728a 0000 00d6 0000 0073  .r....r........s
+00001b40: 0a00 0000 0001 0401 0c01 0e02 0c01 7a23  ..............z#
+00001b50: 5377 6565 7053 6372 6565 6e2e 7374 6172  SweepScreen.star
+00001b60: 745f 7374 6f70 5f62 7574 746f 6e5f 7374  t_stop_button_st
+00001b70: 6174 6563 0100 0000 0000 0000 0000 0000  atec............
+00001b80: 0100 0000 0200 0000 4300 0000 7314 0000  ........C...s...
+00001b90: 007c 00a0 00a1 0001 007c 00a0 01a1 0001  .|.......|......
+00001ba0: 0064 0053 0072 1500 0000 2902 725c 0000  .d.S.r....).r\..
+00001bb0: 00da 1375 7064 6174 655f 7265 7375 6c74  ...update_result
+00001bc0: 5f74 6162 6c65 7218 0000 0072 0f00 0000  _tabler....r....
+00001bd0: 720f 0000 0072 1000 0000 7276 0000 00de  r....r....rv....
+00001be0: 0000 0073 0400 0000 0001 0801 7a19 5377  ...s........z.Sw
+00001bf0: 6565 7053 6372 6565 6e2e 7368 6f77 5f6e  eepScreen.show_n
+00001c00: 6577 5f64 6174 6163 0100 0000 0000 0000  ew_datac........
+00001c10: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00001c20: 7318 0000 007c 006a 00a0 01a1 0001 007c  s....|.j.......|
+00001c30: 006a 02a0 01a1 0001 0064 0053 0072 1500  .j.......d.S.r..
+00001c40: 0000 2903 724f 0000 0072 8500 0000 7250  ..).rO...r....rP
+00001c50: 0000 0072 1800 0000 720f 0000 0072 0f00  ...r....r....r..
+00001c60: 0000 7210 0000 0072 7800 0000 e200 0000  ..r....rx.......
+00001c70: 7304 0000 0000 010a 017a 1c53 7765 6570  s........z.Sweep
+00001c80: 5363 7265 656e 2e73 6574 5f64 6174 615f  Screen.set_data_
+00001c90: 696e 7661 6c69 6463 0100 0000 0000 0000  invalidc........
+00001ca0: 0000 0000 0200 0000 0600 0000 4300 0000  ............C...
+00001cb0: 733e 0000 007c 006a 00a0 01a1 007d 017c  s>...|.j.....}.|
+00001cc0: 006a 026a 0374 046a 057c 016a 0564 0164  .j.j.t.j.|.j.d.d
+00001cd0: 0264 038d 0401 007c 006a 026a 0374 046a  .d.....|.j.j.t.j
+00001ce0: 067c 016a 0664 0464 0264 038d 0401 0064  .|.j.d.d.d.....d
+00001cf0: 0053 0029 054e 727a 0000 00e9 0300 0000  .S.).Nrz........
+00001d00: 2901 da09 7072 6563 6973 696f 6eda 0029  )...precision..)
+00001d10: 0772 1c00 0000 da0a 6765 745f 7265 7375  .r......get_resu
+00001d20: 6c74 7252 0000 00da 0973 6574 5f76 616c  ltrR.....set_val
+00001d30: 7565 7205 0000 0072 0c00 0000 720d 0000  uer....r....r...
+00001d40: 0029 0272 1900 0000 da03 7265 7372 0f00  .).r......resr..
+00001d50: 0000 720f 0000 0072 1000 0000 7293 0000  ..r....r....r...
+00001d60: 00e6 0000 0073 0600 0000 0001 0a01 1801  .....s..........
+00001d70: 7a1f 5377 6565 7053 6372 6565 6e2e 7570  z.SweepScreen.up
+00001d80: 6461 7465 5f72 6573 756c 745f 7461 626c  date_result_tabl
+00001d90: 6563 0100 0000 0000 0000 0000 0000 0400  ec..............
+00001da0: 0000 0500 0000 4300 0000 73c8 0000 007c  ......C...s....|
+00001db0: 006a 006a 016a 026a 0374 046a 056a 066b  .j.j.j.j.t.j.j.k
+00001dc0: 027d 017c 006a 07a0 087c 01a1 0101 007c  .}.|.j...|.....|
+00001dd0: 006a 07a0 097c 01a1 0101 007c 006a 0aa0  .j...|.....|.j..
+00001de0: 087c 01a1 0101 007c 006a 00a0 0ba1 007d  .|.....|.j.....}
+00001df0: 027c 006a 00a0 0ca1 007d 037c 006a 07a0  .|.j.....}.|.j..
+00001e00: 0da1 0001 007c 006a 0aa0 0da1 0001 007c  .....|.j.......|
+00001e10: 026a 0e72 927c 006a 076a 0f7c 026a 107c  .j.r.|.j.j.|.j.|
+00001e20: 026a 1164 0164 028d 0301 007c 006a 0a6a  .j.d.d.....|.j.j
+00001e30: 0f7c 026a 107c 026a 1264 0164 028d 0301  .|.j.|.j.d.d....
+00001e40: 007c 036a 0e72 c47c 006a 076a 0f7c 036a  .|.j.r.|.j.j.|.j
+00001e50: 137c 036a 1464 0364 028d 0301 007c 006a  .|.j.d.d.....|.j
+00001e60: 0a6a 0f7c 036a 137c 036a 1564 0364 028d  .j.|.j.|.j.d.d..
+00001e70: 0301 0064 0053 0029 044e 7201 0000 0029  ...d.S.).Nr....)
+00001e80: 03da 0178 da01 79da 0b6c 6179 6572 5f69  ...x..y..layer_i
+00001e90: 6e64 6578 7206 0000 0029 1672 1c00 0000  ndexr....).r....
+00001ea0: 725f 0000 0072 6000 0000 da05 7661 6c75  r_...r`.....valu
+00001eb0: 6572 0400 0000 da0b 506c 6f74 5374 796c  er......PlotStyl
+00001ec0: 6549 4472 1200 0000 724f 0000 00da 0e73  eIDr....rO.....s
+00001ed0: 6574 5f6c 6f67 5f6d 6f64 655f 78da 0e73  et_log_mode_x..s
+00001ee0: 6574 5f6c 6f67 5f6d 6f64 655f 7972 5000  et_log_mode_yrP.
+00001ef0: 0000 da10 6765 745f 7377 6565 705f 7265  ....get_sweep_re
+00001f00: 7375 6c74 da0e 6765 745f 6669 745f 7265  sult..get_fit_re
+00001f10: 7375 6c74 7285 0000 00da 0972 6573 756c  sultr......resul
+00001f20: 745f 6f6b da09 706c 6f74 5f64 6174 61da  t_ok..plot_data.
+00001f30: 0b72 6573 756c 745f 6672 6571 da10 7265  .result_freq..re
+00001f40: 7375 6c74 5f61 6d70 6c69 7475 6465 da0c  sult_amplitude..
+00001f50: 7265 7375 6c74 5f70 6861 7365 da0f 7265  result_phase..re
+00001f60: 7375 6c74 5f66 6974 5f66 7265 71da 1472  sult_fit_freq..r
+00001f70: 6573 756c 745f 6669 745f 616d 706c 6974  esult_fit_amplit
+00001f80: 7564 65da 1072 6573 756c 745f 6669 745f  ude..result_fit_
+00001f90: 7068 6173 6529 0472 1900 0000 5a09 6c6f  phase).r....Z.lo
+00001fa0: 675f 7374 796c 655a 1563 7572 7265 6e74  g_styleZ.current
+00001fb0: 5f6d 6561 7375 7265 645f 6461 7461 5a13  _measured_dataZ.
+00001fc0: 6375 7272 656e 745f 6669 7474 6564 5f64  current_fitted_d
+00001fd0: 6174 6172 0f00 0000 720f 0000 0072 1000  atar....r....r..
+00001fe0: 0000 725c 0000 00eb 0000 0073 1c00 0000  ..r\.......s....
+00001ff0: 0001 1401 0c01 0c01 0c01 0a01 0a02 0a01  ................
+00002000: 0a01 0601 1601 1601 0601 1601 7a17 5377  ............z.Sw
+00002010: 6565 7053 6372 6565 6e2e 7570 6461 7465  eepScreen.update
+00002020: 5f70 6c6f 7463 0100 0000 0000 0000 0000  _plotc..........
+00002030: 0000 0200 0000 0300 0000 4300 0000 7324  ..........C...s$
+00002040: 0000 007c 006a 00a0 01a1 0001 007c 006a  ...|.j.......|.j
+00002050: 02a0 03a1 007d 017c 006a 00a0 047c 01a1  .....}.|.j...|..
+00002060: 0101 0064 0053 0072 1500 0000 2905 7223  ...d.S.r....).r#
+00002070: 0000 00da 0563 6c65 6172 721c 0000 00da  .....clearr.....
+00002080: 1367 6574 5f63 616e 7469 6c65 7665 725f  .get_cantilever_
+00002090: 6c69 7374 da08 6164 6449 7465 6d73 2902  list..addItems).
+000020a0: 7219 0000 00da 0f63 616e 7469 6c65 7665  r......cantileve
+000020b0: 725f 6c69 7374 720f 0000 0072 0f00 0000  r_listr....r....
+000020c0: 7210 0000 0072 2400 0000 fc00 0000 7306  r....r$.......s.
+000020d0: 0000 0000 010a 010a 017a 2253 7765 6570  .........z"Sweep
+000020e0: 5363 7265 656e 2e75 7064 6174 655f 6361  Screen.update_ca
+000020f0: 6e74 696c 6576 6572 5f6c 6973 7463 0100  ntilever_listc..
+00002100: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00002110: 0000 4300 0000 732e 0000 007c 006a 00a0  ..C...s....|.j..
+00002120: 01a1 007c 006a 026a 035f 047c 006a 00a0  ...|.j.j._.|.j..
+00002130: 05a1 007c 006a 026a 035f 067c 006a 02a0  ...|.j.j._.|.j..
+00002140: 07a1 0001 0064 0053 0072 1500 0000 2908  .....d.S.r....).
+00002150: 7223 0000 00da 0b63 7572 7265 6e74 5465  r#.....currentTe
+00002160: 7874 721c 0000 00da 0a63 616e 7469 6c65  xtr......cantile
+00002170: 7665 72da 046e 616d 65da 0c63 7572 7265  ver..name..curre
+00002180: 6e74 496e 6465 78da 0569 6e64 6578 da11  ntIndex..index..
+00002190: 7365 6c65 6374 5f63 616e 7469 6c65 7665  select_cantileve
+000021a0: 7272 1800 0000 720f 0000 0072 0f00 0000  rr....r....r....
+000021b0: 7210 0000 0072 6b00 0000 0101 0000 7306  r....rk.......s.
+000021c0: 0000 0000 0110 0110 017a 1d53 7765 6570  .........z.Sweep
+000021d0: 5363 7265 656e 2e75 7064 6174 655f 6361  Screen.update_ca
+000021e0: 6e74 696c 6576 6572 6301 0000 0000 0000  ntileverc.......
+000021f0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00002200: 0073 1a00 0000 7c00 6a00 a001 a100 7d01  .s....|.j.....}.
+00002210: 7c00 6a02 a003 7c01 a101 0100 6400 5300  |.j...|.....d.S.
+00002220: 7215 0000 0029 0472 2900 0000 729d 0000  r....).r)...r...
+00002230: 0072 1c00 0000 da18 7365 6c65 6374 5f65  .r......select_e
+00002240: 7863 6974 6174 696f 6e5f 6d65 7468 6f64  xcitation_method
+00002250: 2902 7219 0000 0072 6100 0000 720f 0000  ).r....ra...r...
+00002260: 0072 0f00 0000 7210 0000 00da 1875 7064  .r....r......upd
+00002270: 6174 655f 6578 6369 7461 7469 6f6e 5f6d  ate_excitation_m
+00002280: 6574 686f 6406 0100 0073 0400 0000 0001  ethod....s......
+00002290: 0a01 7a24 5377 6565 7053 6372 6565 6e2e  ..z$SweepScreen.
+000022a0: 7570 6461 7465 5f65 7863 6974 6174 696f  update_excitatio
+000022b0: 6e5f 6d65 7468 6f64 2901 5429 0246 4629  n_method).T).FF)
+000022c0: 1872 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
+000022d0: 7217 0000 0072 0300 0000 da14 4672 6571  r....r......Freq
+000022e0: 7565 6e63 7953 7765 6570 4d6f 6475 6c65  uencySweepModule
+000022f0: 725d 0000 0072 5900 0000 725a 0000 0072  r]...rY...rZ...r
+00002300: 6e00 0000 7270 0000 0072 7300 0000 725b  n...rp...rs...r[
+00002310: 0000 00da 0462 6f6f 6c72 8e00 0000 728a  .....boolr....r.
+00002320: 0000 0072 7600 0000 7278 0000 0072 9300  ...rv...rx...r..
+00002330: 0000 725c 0000 0072 2400 0000 726b 0000  ..r\...r$...rk..
+00002340: 0072 b600 0000 da0d 5f5f 636c 6173 7363  .r......__classc
+00002350: 656c 6c5f 5f72 0f00 0000 720f 0000 0072  ell__r....r....r
+00002360: 1a00 0000 7210 0000 0072 1400 0000 2300  ....r....r....#.
+00002370: 0000 7322 0000 0008 010c 0410 6308 1d08  ..s"........c...
+00002380: 0f08 0708 0408 0508 0410 0b12 0808 0408  ................
+00002390: 0408 0508 1108 0508 0572 1400 0000 292d  .........r....)-
+000023a0: 720b 0000 00da 0750 7953 6964 6536 7202  r......PySide6r.
+000023b0: 0000 00da 086e 616e 6f73 7572 6672 2500  .....nanosurfr%.
+000023c0: 0000 da29 6e61 6e6f 7375 7266 2e6c 6962  ...)nanosurf.lib
+000023d0: 2e73 706d 2e77 6f72 6b66 6c6f 772e 6672  .spm.workflow.fr
+000023e0: 6571 7565 6e63 795f 7377 6565 70da 036c  equency_sweep..l
+000023f0: 6962 da03 7370 6dda 0877 6f72 6b66 6c6f  ib..spm..workflo
+00002400: 77da 0f66 7265 7175 656e 6379 5f73 7765  w..frequency_swe
+00002410: 6570 722b 0000 00da 1666 7265 7175 656e  epr+.....frequen
+00002420: 6379 5f73 7765 6570 5f6d 6f64 756c 6572  cy_sweep_moduler
+00002430: 0300 0000 7204 0000 0072 2600 0000 da0d  ....r....r&.....
+00002440: 5461 626c 6545 6e74 7279 4944 7372 0500  TableEntryIDsr..
+00002450: 0000 da0d 4e53 4643 6f6d 626f 456e 7472  ....NSFComboEntr
+00002460: 7972 9e00 0000 7211 0000 0072 1200 0000  yr....r....r....
+00002470: 7254 0000 00da 1245 7863 6974 6174 696f  rT.....Excitatio
+00002480: 6e4d 6574 686f 6449 4472 1300 0000 da0a  nMethodIDr......
+00002490: 5069 657a 6f44 7269 7665 7228 0000 0072  PiezoDriver(...r
+000024a0: 3800 0000 7239 0000 0072 3a00 0000 da04  8...r9...r:.....
+000024b0: 6261 7365 5a13 616c 6c6f 7765 645f 636f  baseZ.allowed_co
+000024c0: 756e 745f 756e 6974 73da 056d 696c 6c69  unt_units..milli
+000024d0: 5a12 616c 6c6f 7765 645f 7469 6d65 5f75  Z.allowed_time_u
+000024e0: 6e69 7473 da05 6d69 6372 6fda 046e 616e  nits..micro..nan
+000024f0: 6f5a 1361 6c6c 6f77 6564 5f6d 6574 6572  oZ.allowed_meter
+00002500: 5f75 6e69 7473 da04 6d65 6761 da04 6b69  _units..mega..ki
+00002510: 6c6f 7236 0000 0072 4100 0000 5a1d 616c  lor6...rA...Z.al
+00002520: 6c6f 7765 645f 7370 7269 6e67 5f63 6f6e  lowed_spring_con
+00002530: 7374 616e 745f 756e 6974 7372 4a00 0000  stant_unitsrJ...
+00002540: 724b 0000 00da 0c4d 6f64 756c 6553 6372  rK.....ModuleScr
+00002550: 6565 6e72 1400 0000 720f 0000 0072 0f00  eenr....r....r..
+00002560: 0000 720f 0000 0072 1000 0000 da08 3c6d  ..r....r......<m
+00002570: 6f64 756c 653e 0100 0000 7324 0000 0004  odule>....s$....
+00002580: 050c 0108 011e 0110 0214 0710 0110 fe04  ................
+00002590: 0610 0110 fe04 060e 0118 0122 0122 0122  ..........."."."
+000025a0: 010e 02                                  ...
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_module.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_module.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_module.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_module.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 12:06:00 2023 UTC, .py size: 10552 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 a841 3964 3829 0000  a........A9d8)..
+00000000: 610d 0d0a 0000 0000 5a4d 3964 3829 0000  a.......ZM9d8)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 0200 0100 6d05 0200 0100 6d06 0200  m.....m.....m...
 00000050: 0100 6d07 5a08 0100 6401 6403 6c09 6d0a  ..m.Z...d.d.l.m.
 00000060: 5a0a 0100 6401 6404 6c0b 6d0c 5a0c 6d0d  Z...d.d.l.m.Z.m.
 00000070: 5a0d 6d0e 5a0e 0100 4700 6405 6406 8400  Z.m.Z...G.d.d...
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_settings.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_settings.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_settings.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 11:50:20 2023 UTC, .py size: 2397 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,187 +1,194 @@
-00000000: 610d 0d0a 0000 0000 fc3d 3964 5d09 0000  a........=9d]...
+00000000: 610d 0d0a 0000 0000 5006 5a64 8d09 0000  a.......P.Zd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a05 6401  m.Z...d.d.l.Z.d.
 00000050: 6402 6c06 6d07 0200 0100 6d08 0200 0100  d.l.m.....m.....
 00000060: 6d09 0200 0100 6d0a 5a0b 0100 4700 6404  m.....m.Z...G.d.
-00000070: 6405 8400 6405 6505 6a0c 8303 5a0d 6503  d...d.e.j...Z.e.
-00000080: 4700 6406 6407 8400 6407 8302 8301 5a0e  G.d.d...d.....Z.
-00000090: 4700 6408 6409 8400 6409 6501 6a0f 8303  G.d.d...d.e.j...
-000000a0: 5a10 4700 640a 640b 8400 640b 6501 6a0f  Z.G.d.d...d.e.j.
-000000b0: 8303 5a11 4700 640c 640d 8400 640d 8302  ..Z.G.d.d...d...
-000000c0: 5a12 6402 5300 290e 7abc 2044 6566 696e  Z.d.S.).z. Defin
-000000d0: 6573 2074 6865 2063 6f6e 6669 6775 7261  es the configura
-000000e0: 7469 6f6e 2076 616c 7565 7320 6f66 2074  tion values of t
-000000f0: 6865 206d 6f64 756c 652e 0a20 2020 2056  he module..    V
-00000100: 616c 7565 7320 696e 2074 6865 2050 726f  alues in the Pro
-00000110: 5374 6f72 6520 6172 6520 7361 7665 6420  Store are saved 
-00000120: 616e 6420 6c6f 6164 6564 2064 7572 696e  and loaded durin
-00000130: 6720 6170 706c 6963 6174 696f 6e20 7374  g application st
-00000140: 6172 7475 702f 7368 7574 646f 776e 2061  artup/shutdown a
-00000150: 7574 6f6d 6174 6963 616c 6c79 0a43 6f70  utomatically.Cop
-00000160: 7972 6967 6874 204e 616e 6f73 7572 6620  yright Nanosurf 
-00000170: 4147 2032 3032 310a 4c69 6365 6e73 6520  AG 2021.License 
-00000180: 2d20 4d49 540a e900 0000 004e 2901 da09  - MIT......N)...
-00000190: 6461 7461 636c 6173 7363 0000 0000 0000  dataclassc......
-000001a0: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-000001b0: 0000 7318 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-000001c0: 015a 0364 0264 0384 005a 0464 0453 0029  .Z.d.d...Z.d.S.)
-000001d0: 05da 0d53 7765 6570 5365 7474 696e 6773  ...SweepSettings
-000001e0: 7a85 2073 6574 7469 6e67 7320 6465 6669  z. settings defi
-000001f0: 6e65 6420 6865 7265 2061 7320 5072 6f70  ned here as Prop
-00000200: 5661 6c20 6172 6520 7374 6f72 6564 2070  Val are stored p
-00000210: 6572 7369 7374 656e 746c 7920 696e 2061  ersistently in a
-00000220: 2069 6e69 2d66 696c 650a 2020 2020 2020   ini-file.      
-00000230: 2020 7365 7474 696e 6773 2077 6974 6820    settings with 
-00000240: 6120 275f 2720 6173 2066 6972 7374 2063  a '_' as first c
-00000250: 6861 7220 6172 6520 6e6f 7420 7374 6f72  har are not stor
-00000260: 6564 0a20 2020 2063 0100 0000 0000 0000  ed.    c........
-00000270: 0000 0000 0100 0000 0600 0000 4300 0000  ............C...
-00000280: 73d0 0000 0074 0083 007c 005f 0174 02a0  s....t...|._.t..
-00000290: 0374 0474 056a 066a 0783 01a1 017c 005f  .t.t.j.j.....|._
-000002a0: 0874 02a0 0374 0474 056a 096a 0a83 01a1  .t...t.t.j.j....
-000002b0: 017c 005f 0b74 02a0 0374 0474 056a 0c6a  .|._.t...t.t.j.j
-000002c0: 0d83 01a1 017c 005f 0e74 02a0 0374 02a0  .....|._.t...t..
-000002d0: 0f64 0164 02a1 02a1 017c 005f 1074 02a0  .d.d.....|._.t..
-000002e0: 0374 02a0 0f64 0364 02a1 02a1 017c 005f  .t...d.d.....|._
-000002f0: 1174 02a0 0374 02a0 0f64 0464 02a1 02a1  .t...t...d.d....
-00000300: 017c 005f 1274 02a0 0374 02a0 0f64 0564  .|._.t...t...d.d
-00000310: 06a1 02a1 017c 005f 1374 02a0 0374 02a0  .....|._.t...t..
-00000320: 0f64 0764 06a1 02a1 017c 005f 1474 02a0  .d.d.....|._.t..
-00000330: 0374 0474 156a 1683 01a1 017c 005f 1774  .t.t.j.....|._.t
-00000340: 02a0 0374 0474 186a 1983 01a1 017c 005f  ...t.t.j.....|._
-00000350: 1a64 0053 0029 084e 6988 1300 00da 0248  .d.S.).Ni......H
-00000360: 7ae9 c800 0000 e90a 0000 0067 9a99 9999  z..........g....
-00000370: 9999 c93f da01 5672 0100 0000 291b da0a  ...?..Vr....)...
-00000380: 4361 6e74 696c 6576 6572 da0a 6361 6e74  Cantilever..cant
-00000390: 696c 6576 6572 da03 6e73 66da 0750 726f  ilever..nsf..Pro
-000003a0: 7056 616c da03 696e 74da 0a66 7265 715f  pVal..int..freq_
-000003b0: 7377 6565 70da 0a42 616e 6477 6964 7468  sweep..Bandwidth
-000003c0: 73da 0648 7a5f 3336 30da 0962 616e 6477  s..Hz_360..bandw
-000003d0: 6964 7468 da0b 496e 7075 7453 6f75 7263  idth..InputSourc
-000003e0: 65da 0a44 6566 6c65 6374 696f 6eda 0c69  e..Deflection..i
-000003f0: 6e70 7574 5f73 6f75 7263 65da 1446 7265  nput_source..Fre
-00000400: 7175 656e 6379 5377 6565 704f 7574 7075  quencySweepOutpu
-00000410: 74da 114e 6f72 6d61 6c5f 4578 6369 7461  t..Normal_Excita
-00000420: 7469 6f6e da0d 6f75 7470 7574 5f73 6f75  tion..output_sou
-00000430: 7263 65da 0653 6369 5661 6cda 1063 656e  rce..SciVal..cen
-00000440: 7465 725f 6672 6571 7565 6e63 79da 0f66  ter_frequency..f
-00000450: 7265 7175 656e 6379 5f72 616e 6765 da0f  requency_range..
-00000460: 6672 6571 7565 6e63 795f 7374 6570 73da  frequency_steps.
-00000470: 1465 7863 6974 6174 696f 6e5f 616d 706c  .excitation_ampl
-00000480: 6974 7564 65da 1364 6566 6c65 6374 696f  itude..deflectio
-00000490: 6e5f 7365 7470 6f69 6e74 da0b 506c 6f74  n_setpoint..Plot
-000004a0: 5374 796c 6549 44da 064c 696e 6561 72da  StyleID..Linear.
-000004b0: 0d70 6c6f 745f 7374 796c 655f 6964 da12  .plot_style_id..
-000004c0: 4578 6369 7461 7469 6f6e 4d65 7468 6f64  ExcitationMethod
-000004d0: 4944 da0a 436c 6561 6e44 7269 7665 da11  ID..CleanDrive..
-000004e0: 6578 6369 7461 7469 6f6e 5f6d 6574 686f  excitation_metho
-000004f0: 64a9 01da 0473 656c 66a9 0072 2500 0000  d....self..r%...
-00000500: fa63 433a 5c47 6974 5c73 6372 6970 7473  .cC:\Git\scripts
-00000510: 5f70 7974 686f 6e5f 6c69 625c 6e61 6e6f  _python_lib\nano
-00000520: 7375 7266 5c61 7070 5c61 7070 5f66 7265  surf\app\app_fre
-00000530: 7175 656e 6379 5f73 7765 6570 5c66 7265  quency_sweep\fre
-00000540: 7175 656e 6379 5f73 7765 6570 5f6d 6f64  quency_sweep_mod
-00000550: 756c 655c 7377 6565 705f 7365 7474 696e  ule\sweep_settin
-00000560: 6773 2e70 79da 085f 5f69 6e69 745f 5f10  gs.py..__init__.
-00000570: 0000 0073 1600 0000 0001 0801 1401 1401  ...s............
-00000580: 1401 1401 1401 1401 1401 1402 1201 7a16  ..............z.
-00000590: 5377 6565 7053 6574 7469 6e67 732e 5f5f  SweepSettings.__
-000005a0: 696e 6974 5f5f 4e29 05da 085f 5f6e 616d  init__N)...__nam
-000005b0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-000005c0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
-000005d0: 5f64 6f63 5f5f 7227 0000 0072 2500 0000  _doc__r'...r%...
-000005e0: 7225 0000 0072 2500 0000 7226 0000 0072  r%...r%...r&...r
-000005f0: 0300 0000 0c00 0000 7304 0000 0008 0104  ........s.......
-00000600: 0372 0300 0000 6300 0000 0000 0000 0000  .r....c.........
-00000610: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
-00000620: 1c00 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
-00000630: 6402 5a04 6402 5a05 6402 5a06 6403 5300  d.Z.d.Z.d.Z.d.S.
-00000640: 2904 da0c 5377 6565 7052 6573 756c 7473  )...SweepResults
-00000650: 7a57 2054 6869 7320 636c 6173 7320 7361  zW This class sa
-00000660: 7665 7320 7468 6520 776f 726b 6572 2074  ves the worker t
-00000670: 6173 6b20 7265 7375 6c74 2028 652e 6720  ask result (e.g 
-00000680: 6265 2072 6561 6420 6279 2067 7569 2065  be read by gui e
-00000690: 6c65 6d65 6e74 7320 6f72 2073 6176 6564  lements or saved
-000006a0: 2074 6f20 6669 6c65 2067 0000 0000 0000   to file g......
-000006b0: 0000 4e29 0772 2800 0000 7229 0000 0072  ..N).r(...r)...r
-000006c0: 2a00 0000 722b 0000 00da 1372 6573 6f6e  *...r+.....reson
-000006d0: 616e 6365 5f66 7265 7175 656e 6379 da08  ance_frequency..
-000006e0: 715f 6661 6374 6f72 da0f 7370 7269 6e67  q_factor..spring
-000006f0: 5f63 6f6e 7374 616e 7472 2500 0000 7225  _constantr%...r%
-00000700: 0000 0072 2500 0000 7226 0000 0072 2c00  ...r%...r&...r,.
-00000710: 0000 1e00 0000 7308 0000 0008 0204 0104  ......s.........
-00000720: 0104 0172 2c00 0000 6300 0000 0000 0000  ...r,...c.......
-00000730: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-00000740: 0073 1400 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-00000750: 5a03 6402 5a04 6403 5300 2904 721d 0000  Z.d.Z.d.S.).r...
-00000760: 00a9 0172 0100 0000 a901 e901 0000 004e  ...r...........N
-00000770: 2905 7228 0000 0072 2900 0000 722a 0000  ).r(...r)...r*..
-00000780: 0072 1e00 0000 5a0b 4c6f 6761 7269 7468  .r....Z.Logarith
-00000790: 6d69 6372 2500 0000 7225 0000 0072 2500  micr%...r%...r%.
-000007a0: 0000 7226 0000 0072 1d00 0000 2500 0000  ..r&...r....%...
-000007b0: 7304 0000 0008 0104 0172 1d00 0000 6300  s........r....c.
-000007c0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-000007d0: 0000 0040 0000 0073 1400 0000 6500 5a01  ...@...s....e.Z.
-000007e0: 6400 5a02 6401 5a03 6402 5a04 6403 5300  d.Z.d.Z.d.Z.d.S.
-000007f0: 2904 7220 0000 0072 3000 0000 7231 0000  ).r ...r0...r1..
-00000800: 004e 2905 7228 0000 0072 2900 0000 722a  .N).r(...r)...r*
-00000810: 0000 0072 2100 0000 5a0a 5069 657a 6f44  ...r!...Z.PiezoD
-00000820: 7269 7665 7225 0000 0072 2500 0000 7225  river%...r%...r%
-00000830: 0000 0072 2600 0000 7220 0000 0029 0000  ...r&...r ...)..
-00000840: 0073 0400 0000 0801 0401 7220 0000 0063  .s........r ...c
-00000850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000860: 0200 0000 4000 0000 7314 0000 0065 005a  ....@...s....e.Z
-00000870: 0164 005a 0264 0164 0284 005a 0364 0353  .d.Z.d.d...Z.d.S
-00000880: 0029 0472 0800 0000 6301 0000 0000 0000  .).r....c.......
-00000890: 0000 0000 0001 0000 0006 0000 0043 0000  .............C..
-000008a0: 0073 ca00 0000 6401 7c00 5f00 6402 7c00  .s....d.|._.d.|.
-000008b0: 5f01 7402 a003 7402 a004 6401 6403 a102  _.t...t...d.d...
-000008c0: a101 7c00 5f05 7402 a003 7402 a004 6401  ..|._.t...t...d.
-000008d0: 6403 a102 a101 7c00 5f06 7402 a003 7402  d.....|._.t...t.
-000008e0: a004 6401 6404 a102 a101 7c00 5f07 7402  ..d.d.....|._.t.
-000008f0: a003 7402 a004 6401 6405 a102 a101 7c00  ..t...d.d.....|.
-00000900: 5f08 7402 a003 7402 a004 6401 6402 a102  _.t...t...d.d...
-00000910: a101 7c00 5f09 7402 a003 7402 a004 6401  ..|._.t...t...d.
-00000920: 6405 a102 a101 7c00 5f0a 7402 a003 7402  d.....|._.t...t.
-00000930: a004 6401 6402 a102 a101 7c00 5f0b 6402  ..d.d.....|._.d.
-00000940: 7c00 5f0c 7402 a003 7402 a004 6401 6406  |._.t...t...d.d.
-00000950: a102 a101 7c00 5f0d 7402 a003 7402 a004  ....|._.t...t...
-00000960: 6401 6403 a102 a101 7c00 5f0e 6400 5300  d.d.....|._.d.S.
-00000970: 2907 4e72 0100 0000 da00 da01 6d7a 034e  ).Nr........mz.N
-00000980: 2f6d 7204 0000 00da 0364 6567 290f da05  /mr......deg)...
-00000990: 696e 6465 78da 046e 616d 6572 0a00 0000  index..namer....
-000009a0: 720b 0000 0072 1700 0000 da06 6c65 6e67  r....r......leng
-000009b0: 7468 da05 7769 6474 6872 2f00 0000 da17  th..widthr/.....
-000009c0: 7265 736f 6e61 6e63 655f 6672 6571 7565  resonance_freque
-000009d0: 6e63 795f 6169 72da 0c71 5f66 6163 746f  ncy_air..q_facto
-000009e0: 725f 6169 72da 1a72 6573 6f6e 616e 6365  r_air..resonance
-000009f0: 5f66 7265 7175 656e 6379 5f6c 6971 7569  _frequency_liqui
-00000a00: 64da 0f71 5f66 6163 746f 725f 6c69 7175  d..q_factor_liqu
-00000a10: 6964 da05 7368 6170 65da 0e74 6970 5f68  id..shape..tip_h
-00000a20: 616c 665f 616e 676c 65da 0a74 6970 5f72  alf_angle..tip_r
-00000a30: 6164 6975 7372 2300 0000 7225 0000 0072  adiusr#...r%...r
-00000a40: 2500 0000 7226 0000 0072 2700 0000 2e00  %...r&...r'.....
-00000a50: 0000 7318 0000 0000 0106 0106 0114 0114  ..s.............
-00000a60: 0114 0114 0114 0114 0114 0106 0114 017a  ...............z
-00000a70: 1343 616e 7469 6c65 7665 722e 5f5f 696e  .Cantilever.__in
-00000a80: 6974 5f5f 4e29 0472 2800 0000 7229 0000  it__N).r(...r)..
-00000a90: 0072 2a00 0000 7227 0000 0072 2500 0000  .r*...r'...r%...
-00000aa0: 7225 0000 0072 2500 0000 7226 0000 0072  r%...r%...r&...r
-00000ab0: 0800 0000 2d00 0000 7302 0000 0008 0172  ....-...s......r
-00000ac0: 0800 0000 2913 722b 0000 00da 0465 6e75  ....).r+.....enu
-00000ad0: 6dda 0b64 6174 6163 6c61 7373 6573 7202  m..dataclassesr.
-00000ae0: 0000 00da 086e 616e 6f73 7572 6672 0a00  .....nanosurfr..
-00000af0: 0000 da29 6e61 6e6f 7375 7266 2e6c 6962  ...)nanosurf.lib
-00000b00: 2e73 706d 2e77 6f72 6b66 6c6f 772e 6672  .spm.workflow.fr
-00000b10: 6571 7565 6e63 795f 7377 6565 70da 036c  equency_sweep..l
-00000b20: 6962 da03 7370 6dda 0877 6f72 6b66 6c6f  ib..spm..workflo
-00000b30: 77da 0f66 7265 7175 656e 6379 5f73 7765  w..frequency_swe
-00000b40: 6570 720d 0000 00da 0950 726f 7053 746f  epr......PropSto
-00000b50: 7265 7203 0000 0072 2c00 0000 da07 496e  rer....r,.....In
-00000b60: 7445 6e75 6d72 1d00 0000 7220 0000 0072  tEnumr....r ...r
-00000b70: 0800 0000 7225 0000 0072 2500 0000 7225  ....r%...r%...r%
-00000b80: 0000 0072 2600 0000 da08 3c6d 6f64 756c  ...r&.....<modul
-00000b90: 653e 0100 0000 7314 0000 0004 0608 010c  e>....s.........
-00000ba0: 0108 011e 0212 1202 0110 0612 0412 04    ...............
+00000070: 6405 8400 6405 6505 6a0c 8303 5a0d 4700  d...d.e.j...Z.G.
+00000080: 6406 6407 8400 6407 8302 5a0e 4700 6408  d.d...d...Z.G.d.
+00000090: 6409 8400 6409 6501 6a0f 8303 5a10 4700  d...d.e.j...Z.G.
+000000a0: 640a 640b 8400 640b 6501 6a0f 8303 5a11  d.d...d.e.j...Z.
+000000b0: 4700 640c 640d 8400 640d 8302 5a12 6402  G.d.d...d...Z.d.
+000000c0: 5300 290e 7abc 2044 6566 696e 6573 2074  S.).z. Defines t
+000000d0: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
+000000e0: 2076 616c 7565 7320 6f66 2074 6865 206d   values of the m
+000000f0: 6f64 756c 652e 0a20 2020 2056 616c 7565  odule..    Value
+00000100: 7320 696e 2074 6865 2050 726f 5374 6f72  s in the ProStor
+00000110: 6520 6172 6520 7361 7665 6420 616e 6420  e are saved and 
+00000120: 6c6f 6164 6564 2064 7572 696e 6720 6170  loaded during ap
+00000130: 706c 6963 6174 696f 6e20 7374 6172 7475  plication startu
+00000140: 702f 7368 7574 646f 776e 2061 7574 6f6d  p/shutdown autom
+00000150: 6174 6963 616c 6c79 0a43 6f70 7972 6967  atically.Copyrig
+00000160: 6874 204e 616e 6f73 7572 6620 4147 2032  ht Nanosurf AG 2
+00000170: 3032 310a 4c69 6365 6e73 6520 2d20 4d49  021.License - MI
+00000180: 540a e900 0000 004e 2901 da09 6461 7461  T......N)...data
+00000190: 636c 6173 7363 0000 0000 0000 0000 0000  classc..........
+000001a0: 0000 0000 0000 0200 0000 4000 0000 7318  ..........@...s.
+000001b0: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+000001c0: 0264 0384 005a 0464 0453 0029 05da 0d53  .d...Z.d.S.)...S
+000001d0: 7765 6570 5365 7474 696e 6773 7a85 2073  weepSettingsz. s
+000001e0: 6574 7469 6e67 7320 6465 6669 6e65 6420  ettings defined 
+000001f0: 6865 7265 2061 7320 5072 6f70 5661 6c20  here as PropVal 
+00000200: 6172 6520 7374 6f72 6564 2070 6572 7369  are stored persi
+00000210: 7374 656e 746c 7920 696e 2061 2069 6e69  stently in a ini
+00000220: 2d66 696c 650a 2020 2020 2020 2020 7365  -file.        se
+00000230: 7474 696e 6773 2077 6974 6820 6120 275f  ttings with a '_
+00000240: 2720 6173 2066 6972 7374 2063 6861 7220  ' as first char 
+00000250: 6172 6520 6e6f 7420 7374 6f72 6564 0a20  are not stored. 
+00000260: 2020 2063 0100 0000 0000 0000 0000 0000     c............
+00000270: 0100 0000 0600 0000 4300 0000 73d0 0000  ........C...s...
+00000280: 0074 0083 007c 005f 0174 02a0 0374 0474  .t...|._.t...t.t
+00000290: 056a 066a 0783 01a1 017c 005f 0874 02a0  .j.j.....|._.t..
+000002a0: 0374 0474 056a 096a 0a83 01a1 017c 005f  .t.t.j.j.....|._
+000002b0: 0b74 02a0 0374 0474 056a 0c6a 0d83 01a1  .t...t.t.j.j....
+000002c0: 017c 005f 0e74 02a0 0374 02a0 0f64 0164  .|._.t...t...d.d
+000002d0: 02a1 02a1 017c 005f 1074 02a0 0374 02a0  .....|._.t...t..
+000002e0: 0f64 0364 02a1 02a1 017c 005f 1174 02a0  .d.d.....|._.t..
+000002f0: 0374 02a0 0f64 0464 02a1 02a1 017c 005f  .t...d.d.....|._
+00000300: 1274 02a0 0374 02a0 0f64 0564 06a1 02a1  .t...t...d.d....
+00000310: 017c 005f 1374 02a0 0374 02a0 0f64 0764  .|._.t...t...d.d
+00000320: 06a1 02a1 017c 005f 1474 02a0 0374 0474  .....|._.t...t.t
+00000330: 156a 1683 01a1 017c 005f 1774 02a0 0374  .j.....|._.t...t
+00000340: 0474 186a 1983 01a1 017c 005f 1a64 0053  .t.j.....|._.d.S
+00000350: 0029 084e 6988 1300 00da 0248 7ae9 c800  .).Ni......Hz...
+00000360: 0000 e90a 0000 0067 9a99 9999 9999 c93f  .......g.......?
+00000370: da01 5672 0100 0000 291b da0a 4361 6e74  ..Vr....)...Cant
+00000380: 696c 6576 6572 da0a 6361 6e74 696c 6576  ilever..cantilev
+00000390: 6572 da03 6e73 66da 0750 726f 7056 616c  er..nsf..PropVal
+000003a0: da03 696e 74da 0a66 7265 715f 7377 6565  ..int..freq_swee
+000003b0: 70da 0a42 616e 6477 6964 7468 73da 0648  p..Bandwidths..H
+000003c0: 7a5f 3336 30da 0962 616e 6477 6964 7468  z_360..bandwidth
+000003d0: da0b 496e 7075 7453 6f75 7263 65da 0a44  ..InputSource..D
+000003e0: 6566 6c65 6374 696f 6eda 0c69 6e70 7574  eflection..input
+000003f0: 5f73 6f75 7263 65da 1446 7265 7175 656e  _source..Frequen
+00000400: 6379 5377 6565 704f 7574 7075 74da 114e  cySweepOutput..N
+00000410: 6f72 6d61 6c5f 4578 6369 7461 7469 6f6e  ormal_Excitation
+00000420: da0d 6f75 7470 7574 5f73 6f75 7263 65da  ..output_source.
+00000430: 0653 6369 5661 6cda 1063 656e 7465 725f  .SciVal..center_
+00000440: 6672 6571 7565 6e63 79da 0f66 7265 7175  frequency..frequ
+00000450: 656e 6379 5f72 616e 6765 da0f 6672 6571  ency_range..freq
+00000460: 7565 6e63 795f 7374 6570 73da 1465 7863  uency_steps..exc
+00000470: 6974 6174 696f 6e5f 616d 706c 6974 7564  itation_amplitud
+00000480: 65da 1364 6566 6c65 6374 696f 6e5f 7365  e..deflection_se
+00000490: 7470 6f69 6e74 da0b 506c 6f74 5374 796c  tpoint..PlotStyl
+000004a0: 6549 44da 064c 696e 6561 72da 0d70 6c6f  eID..Linear..plo
+000004b0: 745f 7374 796c 655f 6964 da12 4578 6369  t_style_id..Exci
+000004c0: 7461 7469 6f6e 4d65 7468 6f64 4944 da0a  tationMethodID..
+000004d0: 436c 6561 6e44 7269 7665 da11 6578 6369  CleanDrive..exci
+000004e0: 7461 7469 6f6e 5f6d 6574 686f 64a9 01da  tation_method...
+000004f0: 0473 656c 66a9 0072 2500 0000 fa63 433a  .self..r%....cC:
+00000500: 5c47 6974 5c73 6372 6970 7473 5f70 7974  \Git\scripts_pyt
+00000510: 686f 6e5f 6c69 625c 6e61 6e6f 7375 7266  hon_lib\nanosurf
+00000520: 5c61 7070 5c61 7070 5f66 7265 7175 656e  \app\app_frequen
+00000530: 6379 5f73 7765 6570 5c66 7265 7175 656e  cy_sweep\frequen
+00000540: 6379 5f73 7765 6570 5f6d 6f64 756c 655c  cy_sweep_module\
+00000550: 7377 6565 705f 7365 7474 696e 6773 2e70  sweep_settings.p
+00000560: 79da 085f 5f69 6e69 745f 5f10 0000 0073  y..__init__....s
+00000570: 1600 0000 0001 0801 1401 1401 1401 1401  ................
+00000580: 1401 1401 1401 1402 1201 7a16 5377 6565  ..........z.Swee
+00000590: 7053 6574 7469 6e67 732e 5f5f 696e 6974  pSettings.__init
+000005a0: 5f5f 4ea9 05da 085f 5f6e 616d 655f 5fda  __N....__name__.
+000005b0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+000005c0: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
+000005d0: 5f5f 7227 0000 0072 2500 0000 7225 0000  __r'...r%...r%..
+000005e0: 0072 2500 0000 7226 0000 0072 0300 0000  .r%...r&...r....
+000005f0: 0c00 0000 7304 0000 0008 0104 0372 0300  ....s........r..
+00000600: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000610: 0000 0003 0000 0040 0000 0073 1e00 0000  .......@...s....
+00000620: 6500 5a01 6400 5a02 6401 5a03 6402 6403  e.Z.d.Z.d.Z.d.d.
+00000630: 9c01 6404 6405 8404 5a04 6402 5300 2906  ..d.d...Z.d.S.).
+00000640: da0c 5377 6565 7052 6573 756c 7473 7a57  ..SweepResultszW
+00000650: 2054 6869 7320 636c 6173 7320 7361 7665   This class save
+00000660: 7320 7468 6520 776f 726b 6572 2074 6173  s the worker tas
+00000670: 6b20 7265 7375 6c74 2028 652e 6720 6265  k result (e.g be
+00000680: 2072 6561 6420 6279 2067 7569 2065 6c65   read by gui ele
+00000690: 6d65 6e74 7320 6f72 2073 6176 6564 2074  ments or saved t
+000006a0: 6f20 6669 6c65 204e 2901 da06 7265 7475  o file N)...retu
+000006b0: 726e 6301 0000 0000 0000 0000 0000 0001  rnc.............
+000006c0: 0000 0002 0000 0043 0000 0073 1600 0000  .......C...s....
+000006d0: 6401 7c00 5f00 6401 7c00 5f01 6401 7c00  d.|._.d.|._.d.|.
+000006e0: 5f02 6400 5300 2902 4e67 0000 0000 0000  _.d.S.).Ng......
+000006f0: 0000 2903 da13 7265 736f 6e61 6e63 655f  ..)...resonance_
+00000700: 6672 6571 7565 6e63 79da 0871 5f66 6163  frequency..q_fac
+00000710: 746f 72da 0f73 7072 696e 675f 636f 6e73  tor..spring_cons
+00000720: 7461 6e74 7223 0000 0072 2500 0000 7225  tantr#...r%...r%
+00000730: 0000 0072 2600 0000 7227 0000 0020 0000  ...r&...r'... ..
+00000740: 0073 0600 0000 0001 0601 0601 7a15 5377  .s..........z.Sw
+00000750: 6565 7052 6573 756c 7473 2e5f 5f69 6e69  eepResults.__ini
+00000760: 745f 5f72 2800 0000 7225 0000 0072 2500  t__r(...r%...r%.
+00000770: 0000 7225 0000 0072 2600 0000 722d 0000  ..r%...r&...r-..
+00000780: 001e 0000 0073 0400 0000 0801 0401 722d  .....s........r-
+00000790: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000007a0: 0000 0000 0100 0000 4000 0000 7314 0000  ........@...s...
+000007b0: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
+000007c0: 0464 0353 0029 0472 1d00 0000 a901 7201  .d.S.).r......r.
+000007d0: 0000 00a9 01e9 0100 0000 4e29 0572 2900  ..........N).r).
+000007e0: 0000 722a 0000 0072 2b00 0000 721e 0000  ..r*...r+...r...
+000007f0: 005a 0b4c 6f67 6172 6974 686d 6963 7225  .Z.Logarithmicr%
+00000800: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
+00000810: 0000 721d 0000 0025 0000 0073 0400 0000  ..r....%...s....
+00000820: 0801 0401 721d 0000 0063 0000 0000 0000  ....r....c......
+00000830: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+00000840: 0000 7314 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00000850: 015a 0364 025a 0464 0353 0029 0472 2000  .Z.d.Z.d.S.).r .
+00000860: 0000 7232 0000 0072 3300 0000 4e29 0572  ..r2...r3...N).r
+00000870: 2900 0000 722a 0000 0072 2b00 0000 7221  )...r*...r+...r!
+00000880: 0000 005a 0a50 6965 7a6f 4472 6976 6572  ...Z.PiezoDriver
+00000890: 2500 0000 7225 0000 0072 2500 0000 7226  %...r%...r%...r&
+000008a0: 0000 0072 2000 0000 2900 0000 7304 0000  ...r ...)...s...
+000008b0: 0008 0104 0172 2000 0000 6300 0000 0000  .....r ...c.....
+000008c0: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
+000008d0: 0000 0073 1400 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+000008e0: 6401 6402 8400 5a03 6403 5300 2904 7208  d.d...Z.d.S.).r.
+000008f0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000900: 0100 0000 0600 0000 4300 0000 73ca 0000  ........C...s...
+00000910: 0064 017c 005f 0064 027c 005f 0174 02a0  .d.|._.d.|._.t..
+00000920: 0374 02a0 0464 0164 03a1 02a1 017c 005f  .t...d.d.....|._
+00000930: 0574 02a0 0374 02a0 0464 0164 03a1 02a1  .t...t...d.d....
+00000940: 017c 005f 0674 02a0 0374 02a0 0464 0164  .|._.t...t...d.d
+00000950: 04a1 02a1 017c 005f 0774 02a0 0374 02a0  .....|._.t...t..
+00000960: 0464 0164 05a1 02a1 017c 005f 0874 02a0  .d.d.....|._.t..
+00000970: 0374 02a0 0464 0164 02a1 02a1 017c 005f  .t...d.d.....|._
+00000980: 0974 02a0 0374 02a0 0464 0164 05a1 02a1  .t...t...d.d....
+00000990: 017c 005f 0a74 02a0 0374 02a0 0464 0164  .|._.t...t...d.d
+000009a0: 02a1 02a1 017c 005f 0b64 027c 005f 0c74  .....|._.d.|._.t
+000009b0: 02a0 0374 02a0 0464 0164 06a1 02a1 017c  ...t...d.d.....|
+000009c0: 005f 0d74 02a0 0374 02a0 0464 0164 03a1  ._.t...t...d.d..
+000009d0: 02a1 017c 005f 0e64 0053 0029 074e 7201  ...|._.d.S.).Nr.
+000009e0: 0000 00da 00da 016d 7a03 4e2f 6d72 0400  .......mz.N/mr..
+000009f0: 0000 da03 6465 6729 0fda 0569 6e64 6578  ....deg)...index
+00000a00: da04 6e61 6d65 720a 0000 0072 0b00 0000  ..namer....r....
+00000a10: 7217 0000 00da 066c 656e 6774 68da 0577  r......length..w
+00000a20: 6964 7468 7231 0000 00da 1772 6573 6f6e  idthr1.....reson
+00000a30: 616e 6365 5f66 7265 7175 656e 6379 5f61  ance_frequency_a
+00000a40: 6972 da0c 715f 6661 6374 6f72 5f61 6972  ir..q_factor_air
+00000a50: da1a 7265 736f 6e61 6e63 655f 6672 6571  ..resonance_freq
+00000a60: 7565 6e63 795f 6c69 7175 6964 da0f 715f  uency_liquid..q_
+00000a70: 6661 6374 6f72 5f6c 6971 7569 64da 0573  factor_liquid..s
+00000a80: 6861 7065 da0e 7469 705f 6861 6c66 5f61  hape..tip_half_a
+00000a90: 6e67 6c65 da0a 7469 705f 7261 6469 7573  ngle..tip_radius
+00000aa0: 7223 0000 0072 2500 0000 7225 0000 0072  r#...r%...r%...r
+00000ab0: 2600 0000 7227 0000 002e 0000 0073 1800  &...r'.......s..
+00000ac0: 0000 0001 0601 0601 1401 1401 1401 1401  ................
+00000ad0: 1401 1401 1401 0601 1401 7a13 4361 6e74  ..........z.Cant
+00000ae0: 696c 6576 6572 2e5f 5f69 6e69 745f 5f4e  ilever.__init__N
+00000af0: 2904 7229 0000 0072 2a00 0000 722b 0000  ).r)...r*...r+..
+00000b00: 0072 2700 0000 7225 0000 0072 2500 0000  .r'...r%...r%...
+00000b10: 7225 0000 0072 2600 0000 7208 0000 002d  r%...r&...r....-
+00000b20: 0000 0073 0200 0000 0801 7208 0000 0029  ...s......r....)
+00000b30: 1372 2c00 0000 da04 656e 756d da0b 6461  .r,.....enum..da
+00000b40: 7461 636c 6173 7365 7372 0200 0000 da08  taclassesr......
+00000b50: 6e61 6e6f 7375 7266 720a 0000 00da 296e  nanosurfr.....)n
+00000b60: 616e 6f73 7572 662e 6c69 622e 7370 6d2e  anosurf.lib.spm.
+00000b70: 776f 726b 666c 6f77 2e66 7265 7175 656e  workflow.frequen
+00000b80: 6379 5f73 7765 6570 da03 6c69 62da 0373  cy_sweep..lib..s
+00000b90: 706d da08 776f 726b 666c 6f77 da0f 6672  pm..workflow..fr
+00000ba0: 6571 7565 6e63 795f 7377 6565 7072 0d00  equency_sweepr..
+00000bb0: 0000 da09 5072 6f70 5374 6f72 6572 0300  ....PropStorer..
+00000bc0: 0000 722d 0000 00da 0749 6e74 456e 756d  ..r-.....IntEnum
+00000bd0: 721d 0000 0072 2000 0000 7208 0000 0072  r....r ...r....r
+00000be0: 2500 0000 7225 0000 0072 2500 0000 7226  %...r%...r%...r&
+00000bf0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000c00: 0073 1200 0000 0406 0801 0c01 0801 1e02  .s..............
+00000c10: 1212 0e07 1204 1204                      ........
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_task.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_task.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_task.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 12:04:15 2023 UTC, .py size: 3943 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3f41 3964 670f 0000  a.......?A9dg...
+00000000: 610d 0d0a 0000 0000 5a4d 3964 670f 0000  a.......ZM9dg...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6403 6c04 6d05 5a05 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6402 6c06 5a07 6401 6402 6c08 6d09 0200  d.l.Z.d.d.l.m...
 00000060: 0100 6d0a 0200 0100 6d0b 0200 0100 6d0c  ..m.....m.....m.
 00000070: 5a0d 0100 6401 6404 6c0e 6d0f 5a0f 6d10  Z...d.d.l.m.Z.m.
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_fit.py` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_fit.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_gui.py` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_gui.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_module.py` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_module.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_settings.py` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
         self.frequency_steps = nsf.PropVal(nsf.SciVal(10, "Hz"))
         self.excitation_amplitude = nsf.PropVal(nsf.SciVal(0.2, "V"))
         self.deflection_setpoint = nsf.PropVal(nsf.SciVal(0, "V"))
 
         self.plot_style_id = nsf.PropVal(int(PlotStyleID.Linear))
         self.excitation_method = nsf.PropVal(int(ExcitationMethodID.CleanDrive))
 
-@dataclass
 class SweepResults():
     """ This class saves the worker task result (e.g be read by gui elements or saved to file """
-    resonance_frequency = 0.0
-    q_factor = 0.0
-    spring_constant = 0.0
+    def __init__(self) -> None:
+        self.resonance_frequency = 0.0
+        self.q_factor = 0.0
+        self.spring_constant = 0.0
 
 class PlotStyleID(enum.IntEnum):
     Linear = 0,
     Logarithmic = 1,
 
 class ExcitationMethodID(enum.IntEnum):
     CleanDrive = 0,
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_task.py` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_task.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/main.py` & `nanosurf-1.6.2/nanosurf/app/app_frequency_sweep/main.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/.vscode/launch.json` & `nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/main.py` & `nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/main.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/gui.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/gui.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/gui.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/gui.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 12:26:54 2023 UTC, .py size: 13358 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8e46 3964 2e34 0000  a........F9d.4..
+00000000: 610d 0d0a 0000 0000 8009 5a64 8434 0000  a.........Zd.4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 0a01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6402 6c06 5a07 6401 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 4700 6406 6407  m.Z.m.Z...G.d.d.
 00000070: 8400 6407 6507 6a0b 6a0c 6a0d 8303 5a0e  ..d.e.j.j.j...Z.
@@ -70,15 +70,15 @@
 00000450: 7375 7065 72da 085f 5f69 6e69 745f 5fa9  super..__init__.
 00000460: 01da 0473 656c 66a9 01da 095f 5f63 6c61  ...self....__cla
 00000470: 7373 5f5f 720d 0000 0072 0e00 0000 7212  ss__r....r....r.
 00000480: 0000 0020 0000 0073 0400 0000 0001 0a01  ... ...s........
 00000490: 7a1c 5377 6974 6368 696e 6753 7065 6353  z.SwitchingSpecS
 000004a0: 6372 6565 6e2e 5f5f 696e 6974 5f5f 2901  creen.__init__).
 000004b0: 7204 0000 0063 0200 0000 0000 0000 0000  r....c..........
-000004c0: 0000 0200 0000 0400 0000 4300 0000 7300  ..........C...s.
+000004c0: 0000 0200 0000 0400 0000 4300 0000 730c  ..........C...s.
 000004d0: 0400 007c 017c 005f 0074 016a 02a0 0374  ...|.|._.t.j...t
 000004e0: 0464 01a1 027c 005f 0574 016a 02a0 0664  .d...|._.t.j...d
 000004f0: 02a1 017c 005f 077c 006a 07a0 0874 09a1  ...|._.|.j...t..
 00000500: 0101 007c 006a 07a0 0a74 016a 0b6a 0c6a  ...|.j...t.j.j.j
 00000510: 0d6a 0ea1 0101 007c 006a 07a0 0f64 03a1  .j.....|.j...d..
 00000520: 0101 007c 006a 07a0 1064 0464 05a1 0201  ...|.j...d.d....
 00000530: 0074 016a 02a0 0664 06a1 017c 005f 117c  .t.j...d...|._.|
@@ -110,471 +110,475 @@
 000006d0: 25a0 267c 006a 07a1 0101 007c 006a 25a0  %.&|.j.....|.j%.
 000006e0: 267c 006a 11a1 0101 007c 006a 25a0 267c  &|.j.....|.j%.&|
 000006f0: 006a 12a1 0101 007c 006a 25a0 267c 006a  .j.....|.j%.&|.j
 00000700: 14a1 0101 007c 006a 25a0 2764 19a1 0101  .....|.j%.'d....
 00000710: 007c 006a 25a0 267c 006a 1ba1 0101 007c  .|.j%.&|.j.....|
 00000720: 006a 25a0 2764 19a1 0101 007c 006a 25a0  .j%.'d.....|.j%.
 00000730: 267c 006a 1aa1 0101 007c 006a 25a0 28a1  &|.j.....|.j%.(.
-00000740: 0001 007c 006a 25a0 267c 006a 21a1 0101  ...|.j%.&|.j!...
-00000750: 007c 006a 25a0 28a1 0001 0074 016a 026a  .|.j%.(....t.j.j
-00000760: 2964 1a64 1b8d 017c 005f 2a74 016a 026a  )d.d...|._*t.j.j
-00000770: 2964 1a64 1b8d 017c 005f 2b74 18a0 24a1  )d.d...|._+t..$.
-00000780: 007c 005f 2c7c 006a 2ca0 267c 006a 2aa1  .|._,|.j,.&|.j*.
-00000790: 0101 007c 006a 2ca0 267c 006a 2ba1 0101  ...|.j,.&|.j+...
-000007a0: 0074 18a0 2da1 007c 005f 2e7c 006a 2ea0  .t..-..|._.|.j..
-000007b0: 267c 006a 1ea1 0101 007c 006a 2e6a 267c  &|.j.....|.j.j&|
-000007c0: 006a 2274 2f6a 306a 3164 1c8d 0201 007c  .j"t/j0j1d.....|
-000007d0: 006a 2ca0 327c 006a 2ea1 0101 0074 18a0  .j,.2|.j.....t..
-000007e0: 2da1 007c 005f 3374 18a0 24a1 007c 005f  -..|._3t..$..|._
-000007f0: 347c 006a 34a0 267c 006a 1da1 0101 007c  4|.j4.&|.j.....|
-00000800: 006a 33a0 327c 006a 34a1 0101 007c 006a  .j3.2|.j4....|.j
-00000810: 336a 267c 006a 1674 2f6a 306a 3564 1c8d  3j&|.j.t/j0j5d..
-00000820: 0201 007c 006a 336a 267c 006a 1f74 2f6a  ...|.j3j&|.j.t/j
-00000830: 306a 3564 1c8d 0201 007c 006a 33a0 28a1  0j5d.....|.j3.(.
-00000840: 0001 007c 006a 336a 267c 006a 2374 2f6a  ...|.j3j&|.j#t/j
-00000850: 306a 3564 1c8d 0201 007c 006a 2ca0 327c  0j5d.....|.j,.2|
-00000860: 006a 33a1 0101 0074 18a0 24a1 007c 005f  .j3....t..$..|._
-00000870: 3674 18a0 2da1 007c 005f 377c 006a 37a0  6t..-..|._7|.j7.
-00000880: 327c 006a 2564 0aa1 0201 007c 006a 37a0  2|.j%d.....|.j7.
-00000890: 327c 006a 2c64 0fa1 0201 007c 006a 37a0  2|.j,d.....|.j7.
-000008a0: 327c 006a 3664 0aa1 0201 007c 00a0 387c  2|.j6d.....|..8|
-000008b0: 006a 37a1 0101 007c 00a0 39a1 0001 007c  .j7....|..9....|
-000008c0: 00a0 3aa1 0001 007c 00a0 3ba1 0001 0064  ..:....|..;....d
-000008d0: 1d53 0029 1e7a 3820 6372 6561 7465 2068  .S.).z8 create h
-000008e0: 6572 6520 796f 7572 2067 7569 2077 6974  ere your gui wit
-000008f0: 6820 616c 6c20 636f 6e74 726f 6c73 2061  h all controls a
-00000900: 6e64 2074 6865 6972 206c 6179 6f75 74da  nd their layout.
-00000910: 064f 7574 7075 747a 0d56 6f6c 7461 6765  .Outputz.Voltage
-00000920: 2072 616e 6765 7208 0000 0067 0000 0000   ranger....g....
-00000930: 0000 0000 6700 0000 0000 409f 407a 0d43  ....g.....@.@z.C
-00000940: 656e 7465 7220 6f66 6673 6574 6700 0000  enter offsetg...
-00000950: 0000 408f c067 0000 0000 0040 8f40 7a0f  ..@..g.....@.@z.
-00000960: 4e75 6d62 6572 206f 6620 7374 6570 7372  Number of stepsr
-00000970: 0100 0000 69e8 0300 007a 1554 696d 6520  ....i....z.Time 
-00000980: 6465 6c61 7920 6166 7465 7220 7374 6570  delay after step
-00000990: 6700 0000 0000 00f0 3f7a 0a46 696c 6520  g.......?z.File 
-000009a0: 696e 6465 7872 0700 0000 6910 2700 007a  indexr....i.'..z
-000009b0: 0e53 686f 7720 276f 6e27 2064 6174 617a  .Show 'on' dataz
-000009c0: 0e42 6163 6b77 6172 6420 6669 7273 747a  .Backward firstz
-000009d0: 0e46 696c 6520 6e61 6d65 206d 6173 6b7a  .File name maskz
-000009e0: 1044 6573 7469 6e61 7469 6f6e 2070 6174  .Destination pat
-000009f0: 687a 0e41 7574 6f20 7361 7665 2064 6174  hz.Auto save dat
-00000a00: 61da 0553 7461 7274 5a06 4272 6f77 7365  a..StartZ.Browse
-00000a10: 7a09 5361 7665 2064 6174 61e9 0a00 0000  z.Save data.....
-00000a20: 4629 01da 086c 6f67 6d6f 6465 7829 01da  F)...logmodex)..
-00000a30: 0961 6c69 676e 6d65 6e74 4e29 3c72 0400  .alignmentN)<r..
-00000a40: 0000 da03 6e73 66da 0367 7569 da0b 4e53  ....nsf..gui..NS
-00000a50: 4643 6f6d 626f 426f 78da 1343 6f6d 626f  FComboBox..Combo
-00000a60: 4f75 7470 7574 4368 616e 6e65 6c73 da0f  OutputChannels..
-00000a70: 636f 6d62 6f5f 6f75 7470 7574 5f69 64da  combo_output_id.
-00000a80: 0a4e 5346 5363 6945 6469 74da 1273 6369  .NSFSciEdit..sci
-00000a90: 7661 6c5f 6f75 7470 7574 5f73 7061 6eda  val_output_span.
-00000aa0: 1673 6574 5f61 6c6c 6f77 6564 5f70 7265  .set_allowed_pre
-00000ab0: 6669 785f 6964 73da 1261 6c6c 6f77 6564  fix_ids..allowed
-00000ac0: 5f76 6f6c 745f 756e 6974 73da 0d73 6574  _volt_units..set
-00000ad0: 5f70 7265 6669 785f 6964 da07 7363 695f  _prefix_id..sci_
-00000ae0: 7661 6cda 0275 70da 0650 7265 6669 78da  val..up..Prefix.
-00000af0: 0462 6173 65da 0d73 6574 5f70 7265 6369  .base..set_preci
-00000b00: 7369 6f6e da11 7365 745f 7661 6c75 655f  sion..set_value_
-00000b10: 6d69 6e5f 6d61 78da 1473 6369 7661 6c5f  min_max..scival_
-00000b20: 6f75 7470 7574 5f63 656e 7465 72da 1073  output_center..s
-00000b30: 6369 7661 6c5f 6e75 6d5f 7374 6570 73da  cival_num_steps.
-00000b40: 1361 6c6c 6f77 6564 5f6d 6574 6572 5f75  .allowed_meter_u
-00000b50: 6e69 7473 da11 7363 6976 616c 5f74 696d  nits..scival_tim
-00000b60: 655f 6465 6c61 79da 1261 6c6c 6f77 6564  e_delay..allowed
-00000b70: 5f74 696d 655f 756e 6974 73da 1173 6369  _time_units..sci
-00000b80: 7661 6c5f 6669 6c65 5f69 6e64 6578 da13  val_file_index..
-00000b90: 616c 6c6f 7765 645f 636f 756e 745f 756e  allowed_count_un
-00000ba0: 6974 7372 0200 0000 da09 5143 6865 636b  itsr......QCheck
-00000bb0: 426f 78da 1263 6865 636b 5f73 686f 775f  Box..check_show_
-00000bc0: 6f6e 5f64 6174 61da 1463 6865 636b 5f64  on_data..check_d
-00000bd0: 6f5f 7265 7665 7273 5f72 616d 70da 074e  o_revers_ramp..N
-00000be0: 5346 4564 6974 da0e 6564 6974 5f66 696c  SFEdit..edit_fil
-00000bf0: 655f 6d61 736b da0e 6564 6974 5f66 696c  e_mask..edit_fil
-00000c00: 655f 7061 7468 da0f 6368 6563 6b5f 6175  e_path..check_au
-00000c10: 746f 5f73 6176 65da 0b51 5075 7368 4275  to_save..QPushBu
-00000c20: 7474 6f6e da11 6275 7474 6f6e 5f73 7461  tton..button_sta
-00000c30: 7274 5f73 746f 70da 0d62 7574 746f 6e5f  rt_stop..button_
-00000c40: 6272 6f77 7365 da0d 6275 7474 6f6e 5f65  browse..button_e
-00000c50: 7870 6f72 74da 0b51 5642 6f78 4c61 796f  xport..QVBoxLayo
-00000c60: 7574 5a0b 6c61 796f 7574 5f6c 6566 74da  utZ.layout_left.
-00000c70: 0961 6464 5769 6467 6574 da0a 6164 6453  .addWidget..addS
-00000c80: 7061 6369 6e67 da0a 6164 6453 7472 6574  pacing..addStret
-00000c90: 6368 da08 4e53 4643 6861 7274 da09 6368  ch..NSFChart..ch
-00000ca0: 6172 745f 616d 70da 0b63 6861 7274 5f70  art_amp..chart_p
-00000cb0: 6861 7365 5a0a 6c61 796f 7574 5f6d 6964  haseZ.layout_mid
-00000cc0: da0b 5148 426f 784c 6179 6f75 745a 0b6c  ..QHBoxLayoutZ.l
-00000cd0: 6179 6f75 745f 7061 7468 7203 0000 00da  ayout_pathr.....
-00000ce0: 0d41 6c69 676e 6d65 6e74 466c 6167 da0d  .AlignmentFlag..
-00000cf0: 416c 6967 6e42 6173 656c 696e 65da 0961  AlignBaseline..a
-00000d00: 6464 4c61 796f 7574 5a0b 6c61 796f 7574  ddLayoutZ.layout
-00000d10: 5f66 696c 655a 106c 6179 6f75 745f 6669  _fileZ.layout_fi
-00000d20: 6c65 5f6d 6173 6bda 0c41 6c69 676e 5643  le_mask..AlignVC
-00000d30: 656e 7465 725a 0c6c 6179 6f75 745f 7269  enterZ.layout_ri
-00000d40: 6768 745a 0d73 6372 6565 6e5f 6c61 796f  ghtZ.screen_layo
-00000d50: 7574 da09 7365 744c 6179 6f75 74da 1162  ut..setLayout..b
-00000d60: 696e 645f 6775 695f 656c 656d 656e 7473  ind_gui_elements
-00000d70: da09 696e 6974 5f70 6c6f 74da 1465 6e74  ..init_plot..ent
-00000d80: 6572 5f67 7569 5f73 7461 7465 5f69 646c  er_gui_state_idl
-00000d90: 6529 0272 1400 0000 7204 0000 0072 0d00  e).r....r....r..
-00000da0: 0000 720d 0000 0072 0e00 0000 da0f 646f  ..r....r......do
-00000db0: 5f73 6574 7570 5f73 6372 6565 6e24 0000  _setup_screen$..
-00000dc0: 0073 9600 0000 0002 0604 1002 0e01 0c01  .s..............
-00000dd0: 1401 0c01 0e02 0e01 0c01 1401 0c01 0e02  ................
-00000de0: 0e01 0c01 1401 0c01 0e02 0e01 0c01 1401  ................
-00000df0: 0c01 0e02 0e01 0c01 1401 0c01 0e02 0c01  ................
-00000e00: 0c02 0e01 0e02 0c01 0c01 0c01 0c02 0a01  ................
-00000e10: 0e01 0e01 0e01 0e01 0e01 0c01 0e01 0c01  ................
-00000e20: 0e01 0a01 0e01 0a03 1001 1002 0a01 0e01  ................
-00000e30: 0e01 0a01 0e01 1601 0e01 0a01 0a01 0e01  ................
-00000e40: 0e01 1601 1601 0a01 1601 0e04 0a03 0a02  ................
-00000e50: 1001 1001 1001 0c02 0801 0801 7a23 5377  ............z#Sw
-00000e60: 6974 6368 696e 6753 7065 6353 6372 6565  itchingSpecScree
-00000e70: 6e2e 646f 5f73 6574 7570 5f73 6372 6565  n.do_setup_scree
-00000e80: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
-00000e90: 0000 0400 0000 4300 0000 73ae 0100 0074  ......C...s....t
-00000ea0: 006a 01a0 027c 006a 037c 006a 046a 056a  .j...|.j.|.j.j.j
-00000eb0: 06a1 0201 0074 006a 01a0 027c 006a 077c  .....t.j...|.j.|
-00000ec0: 006a 046a 056a 08a1 0201 0074 006a 01a0  .j.j.j.....t.j..
-00000ed0: 027c 006a 097c 006a 046a 056a 0aa1 0201  .|.j.|.j.j.j....
-00000ee0: 0074 006a 01a0 027c 006a 0b7c 006a 046a  .t.j...|.j.|.j.j
-00000ef0: 056a 0ca1 0201 0074 006a 01a0 027c 006a  .j.....t.j...|.j
-00000f00: 0d7c 006a 046a 056a 0ea1 0201 0074 006a  .|.j.j.j.....t.j
-00000f10: 01a0 027c 006a 0f7c 006a 046a 056a 10a1  ...|.j.|.j.j.j..
-00000f20: 0201 0074 006a 01a0 027c 006a 117c 006a  ...t.j...|.j.|.j
-00000f30: 046a 056a 12a1 0201 0074 006a 01a0 027c  .j.j.....t.j...|
-00000f40: 006a 137c 006a 046a 056a 14a1 0201 0074  .j.|.j.j.j.....t
-00000f50: 006a 01a0 027c 006a 157c 006a 046a 056a  .j...|.j.|.j.j.j
-00000f60: 16a1 0201 0074 006a 01a0 027c 006a 177c  .....t.j...|.j.|
-00000f70: 006a 046a 056a 18a1 0201 0074 006a 01a0  .j.j.j.....t.j..
-00000f80: 027c 006a 197c 006a 046a 056a 1aa1 0201  .|.j.|.j.j.j....
-00000f90: 007c 006a 1b6a 1ca0 1d7c 006a 1ea1 0101  .|.j.j...|.j....
-00000fa0: 007c 006a 1f6a 1ca0 1d7c 006a 20a1 0101  .|.j.j...|.j ...
-00000fb0: 007c 006a 216a 1ca0 1d7c 006a 22a1 0101  .|.j!j...|.j"...
-00000fc0: 007c 006a 046a 23a0 1d7c 006a 24a1 0101  .|.j.j#..|.j$...
-00000fd0: 007c 006a 046a 25a0 1d7c 006a 24a1 0101  .|.j.j%..|.j$...
-00000fe0: 007c 006a 046a 26a0 1d7c 006a 27a1 0101  .|.j.j&..|.j'...
-00000ff0: 007c 006a 046a 28a0 1d7c 006a 29a1 0101  .|.j.j(..|.j)...
-00001000: 007c 006a 046a 2aa0 1d7c 006a 2ba1 0101  .|.j.j*..|.j+...
-00001010: 007c 006a 046a 2ca0 1d7c 006a 2da1 0101  .|.j.j,..|.j-...
-00001020: 007c 006a 046a 056a 1a6a 2ea0 1d7c 006a  .|.j.j.j.j...|.j
-00001030: 2fa1 0101 007c 006a 046a 056a 066a 2ea0  /....|.j.j.j.j..
-00001040: 1d7c 006a 30a1 0101 0064 0153 0029 027a  .|.j0....d.S.).z
-00001050: 4020 636f 6e6e 6563 7420 616c 6c20 6775  @ connect all gu
-00001060: 6920 7769 6467 6574 7320 746f 206d 6f64  i widgets to mod
-00001070: 756c 6520 7365 7474 696e 6773 206f 7220  ule settings or 
-00001080: 616e 7920 6f74 6865 7220 736f 7572 6365  any other source
-00001090: 204e 2931 721c 0000 0072 1d00 0000 da13   N)1r....r......
-000010a0: 636f 6e6e 6563 745f 746f 5f70 726f 7065  connect_to_prope
-000010b0: 7274 7972 2000 0000 7204 0000 0072 0500  rtyr ...r....r..
-000010c0: 0000 da09 6f75 7470 7574 5f69 6472 2200  ....output_idr".
-000010d0: 0000 da0b 6f75 7470 7574 5f73 7061 6e72  ....output_spanr
-000010e0: 2c00 0000 da0d 6f75 7470 7574 5f63 656e  ,.....output_cen
-000010f0: 7465 7272 2d00 0000 da0f 6e75 6d62 6572  terr-.....number
-00001100: 5f6f 665f 7374 6570 7372 2f00 0000 da15  _of_stepsr/.....
-00001110: 7469 6d65 5f64 656c 6179 5f61 6674 6572  time_delay_after
-00001120: 5f73 7465 7072 3800 0000 da0b 666f 6c64  _stepr8.....fold
-00001130: 6572 5f6e 616d 6572 3700 0000 da0e 6669  er_namer7.....fi
-00001140: 6c65 5f6e 616d 655f 6d61 736b 7231 0000  le_name_maskr1..
-00001150: 00da 0a66 696c 655f 696e 6465 7872 3900  ...file_indexr9.
-00001160: 0000 da0e 6175 746f 5f73 6176 655f 6461  ....auto_save_da
-00001170: 7461 7235 0000 00da 0b72 6576 6572 735f  tar5.....revers_
-00001180: 7261 6d70 7234 0000 00da 1373 686f 775f  rampr4.....show_
-00001190: 6f6e 5f64 6174 615f 7661 6c75 6573 723b  on_data_valuesr;
-000011a0: 0000 00da 0763 6c69 636b 6564 da07 636f  .....clicked..co
-000011b0: 6e6e 6563 74da 1c6f 6e5f 6275 7474 6f6e  nnect..on_button
-000011c0: 5f73 7461 7274 5f73 746f 705f 636c 6963  _start_stop_clic
-000011d0: 6b65 6472 3d00 0000 da18 6f6e 5f62 7574  kedr=.....on_but
-000011e0: 746f 6e5f 6578 706f 7274 5f63 6c69 636b  ton_export_click
-000011f0: 6564 723c 0000 00da 186f 6e5f 6275 7474  edr<.....on_butt
-00001200: 6f6e 5f62 726f 7773 655f 636c 6963 6b65  on_browse_clicke
-00001210: 64da 1873 6967 5f77 6f72 6b5f 7374 6172  d..sig_work_star
-00001220: 745f 7265 7175 6573 7465 64da 1465 6e74  t_requested..ent
-00001230: 6572 5f67 7569 5f73 7461 7465 5f77 6169  er_gui_state_wai
-00001240: 74da 1773 6967 5f77 6f72 6b5f 7374 6f70  t..sig_work_stop
-00001250: 5f72 6571 7565 7374 6564 da0f 7369 675f  _requested..sig_
-00001260: 776f 726b 5f61 6374 6976 65da 1665 6e74  work_active..ent
-00001270: 6572 5f67 7569 5f73 7461 7465 5f61 6374  er_gui_state_act
-00001280: 6976 65da 0d73 6967 5f77 6f72 6b5f 646f  ive..sig_work_do
-00001290: 6e65 724d 0000 00da 1673 6967 5f6e 6577  nerM.....sig_new
-000012a0: 5f64 6174 615f 6176 6169 6c61 626c 65da  _data_available.
-000012b0: 0d73 686f 775f 6e65 775f 6461 7461 da10  .show_new_data..
-000012c0: 7369 675f 6461 7461 5f69 6e76 616c 6964  sig_data_invalid
-000012d0: da10 7365 745f 6461 7461 5f69 6e76 616c  ..set_data_inval
-000012e0: 6964 da11 7369 675f 7661 6c75 655f 6368  id..sig_value_ch
-000012f0: 616e 6765 64da 1063 6861 6e67 655f 706c  anged..change_pl
-00001300: 6f74 5f76 6965 7772 4c00 0000 7213 0000  ot_viewrL...r...
-00001310: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
-00001320: 724b 0000 0088 0000 0073 2c00 0000 0004  rK.......s,.....
-00001330: 1601 1601 1601 1601 1601 1601 1601 1601  ................
-00001340: 1601 1601 1603 1001 1001 1003 1001 1001  ................
-00001350: 1001 1001 1001 1002 1401 7a25 5377 6974  ..........z%Swit
-00001360: 6368 696e 6753 7065 6353 6372 6565 6e2e  chingSpecScreen.
-00001370: 6269 6e64 5f67 7569 5f65 6c65 6d65 6e74  bind_gui_element
-00001380: 7363 0100 0000 0000 0000 0000 0000 0100  sc..............
-00001390: 0000 0600 0000 4300 0000 7312 0100 007c  ......C...s....|
-000013a0: 006a 00a0 0164 01a1 0101 007c 006a 00a0  .j...d.....|.j..
-000013b0: 0274 036a 046a 056a 066a 0764 027c 006a  .t.j.j.j.j.d.|.j
-000013c0: 08a0 09a1 009b 0064 039d 03a1 0201 007c  .......d.......|
-000013d0: 006a 00a0 0a74 036a 046a 056a 066a 0764  .j...t.j.j.j.j.d
-000013e0: 04a1 0201 007c 006a 00a0 0a74 036a 046a  .....|.j...t.j.j
-000013f0: 056a 066a 0b64 04a1 0201 007c 006a 00a0  .j.j.d.....|.j..
-00001400: 0274 036a 046a 056a 066a 0b64 01a1 0201  .t.j.j.j.j.d....
-00001410: 007c 006a 00a0 0a74 036a 046a 056a 066a  .|.j...t.j.j.j.j
-00001420: 0b64 05a1 0201 007c 006a 00a0 0ca1 0001  .d.....|.j......
-00001430: 007c 006a 0da0 0164 06a1 0101 007c 006a  .|.j...d.....|.j
-00001440: 0da0 0274 036a 046a 056a 066a 0764 027c  ...t.j.j.j.j.d.|
-00001450: 006a 08a0 09a1 009b 0064 039d 03a1 0201  .j.......d......
-00001460: 007c 006a 0da0 0a74 036a 046a 056a 066a  .|.j...t.j.j.j.j
-00001470: 0764 04a1 0201 007c 006a 0da0 0274 036a  .d.....|.j...t.j
-00001480: 046a 056a 066a 0b64 06a1 0201 007c 006a  .j.j.j.d.....|.j
-00001490: 0da0 0a74 036a 046a 056a 066a 0b64 07a1  ...t.j.j.j.j.d..
-000014a0: 0201 007c 006a 0da0 0ca1 0001 0064 0053  ...|.j.......d.S
-000014b0: 0029 084e da09 416d 706c 6974 7564 657a  .).N..Amplitudez
-000014c0: 084f 7574 7075 7420 27fa 0127 da00 da01  .Output '..'....
-000014d0: 56da 0550 6861 7365 f502 0000 00c2 b029  V..Phase.......)
-000014e0: 0e72 4300 0000 da09 7365 745f 7469 746c  .rC.....set_titl
-000014f0: 65da 0973 6574 5f6c 6162 656c 721c 0000  e..set_labelr...
-00001500: 0072 1d00 0000 7242 0000 00da 0441 7869  .r....rB.....Axi
-00001510: 73da 0662 6f74 746f 6d72 2000 0000 da12  s..bottomr .....
-00001520: 6375 7272 656e 745f 656e 7472 795f 6e61  current_entry_na
-00001530: 6d65 da08 7365 745f 756e 6974 da04 6c65  me..set_unit..le
-00001540: 6674 da0b 636c 6561 725f 706c 6f74 7372  ft..clear_plotsr
-00001550: 4400 0000 7213 0000 0072 0d00 0000 720d  D...r....r....r.
-00001560: 0000 0072 0e00 0000 724c 0000 00a8 0000  ...r....rL......
-00001570: 0073 1a00 0000 0001 0c01 2401 1601 1601  .s........$.....
-00001580: 1601 1601 0a01 0c01 2401 1601 1601 1601  ........$.......
-00001590: 7a1d 5377 6974 6368 696e 6753 7065 6353  z.SwitchingSpecS
-000015a0: 6372 6565 6e2e 696e 6974 5f70 6c6f 7463  creen.init_plotc
-000015b0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000015c0: 0200 0000 4300 0000 7324 0000 007c 006a  ....C...s$...|.j
-000015d0: 00a0 01a1 0072 167c 006a 00a0 02a1 0001  .....r.|.j......
-000015e0: 006e 0a7c 006a 00a0 03a1 0001 0064 0053  .n.|.j.......d.S
-000015f0: 0072 1000 0000 2904 7204 0000 00da 0e69  .r....).r......i
-00001600: 735f 776f 726b 6572 5f62 7573 79da 0b73  s_worker_busy..s
-00001610: 746f 705f 776f 726b 6572 da0c 7374 6172  top_worker..star
-00001620: 745f 776f 726b 6572 7213 0000 0072 0d00  t_workerr....r..
-00001630: 0000 720d 0000 0072 0e00 0000 725d 0000  ..r....r....r]..
-00001640: 00b7 0000 0073 0600 0000 0001 0a01 0c02  .....s..........
-00001650: 7a30 5377 6974 6368 696e 6753 7065 6353  z0SwitchingSpecS
-00001660: 6372 6565 6e2e 6f6e 5f62 7574 746f 6e5f  creen.on_button_
-00001670: 7374 6172 745f 7374 6f70 5f63 6c69 636b  start_stop_click
-00001680: 6564 6301 0000 0000 0000 0000 0000 0001  edc.............
-00001690: 0000 0002 0000 0043 0000 0073 0e00 0000  .......C...s....
-000016a0: 7c00 6a00 a001 a100 0100 6400 5300 7210  |.j.......d.S.r.
-000016b0: 0000 0029 0272 0400 0000 da09 7361 7665  ...).r......save
-000016c0: 5f64 6174 6172 1300 0000 720d 0000 0072  _datar....r....r
-000016d0: 0d00 0000 720e 0000 0072 5e00 0000 bd00  ....r....r^.....
-000016e0: 0000 7302 0000 0000 017a 2c53 7769 7463  ..s......z,Switc
-000016f0: 6869 6e67 5370 6563 5363 7265 656e 2e6f  hingSpecScreen.o
-00001700: 6e5f 6275 7474 6f6e 5f65 7870 6f72 745f  n_button_export_
-00001710: 636c 6963 6b65 6463 0100 0000 0000 0000  clickedc........
-00001720: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-00001730: 7358 0000 0074 00a0 01a1 007d 017c 01a0  sX...t.....}.|..
-00001740: 0274 006a 016a 036a 04a1 0101 007c 01a0  .t.j.j.j.....|..
-00001750: 0574 067c 006a 076a 086a 096a 0a83 01a1  .t.|.j.j.j.j....
-00001760: 0101 007c 01a0 0ba1 0072 547c 01a0 0ca1  ...|.....rT|....
-00001770: 007d 0274 0da0 0e7c 0264 0119 00a1 017c  .}.t...|.d.....|
-00001780: 006a 076a 086a 095f 0a64 0053 0029 024e  .j.j.j._.d.S.).N
-00001790: 7201 0000 0029 0f72 0200 0000 da0b 5146  r....).r......QF
-000017a0: 696c 6544 6961 6c6f 67da 0b73 6574 4669  ileDialog..setFi
-000017b0: 6c65 4d6f 6465 da08 4669 6c65 4d6f 6465  leMode..FileMode
-000017c0: da09 4469 7265 6374 6f72 79da 0c73 6574  ..Directory..set
-000017d0: 4469 7265 6374 6f72 79da 0373 7472 7204  Directory..strr.
-000017e0: 0000 0072 0500 0000 7255 0000 00da 0576  ...r....rU.....v
-000017f0: 616c 7565 da05 6578 6563 5fda 0d73 656c  alue..exec_..sel
-00001800: 6563 7465 6446 696c 6573 da07 7061 7468  ectedFiles..path
-00001810: 6c69 62da 0450 6174 6829 0372 1400 0000  lib..Path).r....
-00001820: da03 646c 675a 0966 696c 654e 616d 6573  ..dlgZ.fileNames
-00001830: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-00001840: 5f00 0000 c000 0000 730c 0000 0000 0108  _.......s.......
-00001850: 0110 0116 0108 0108 017a 2c53 7769 7463  .........z,Switc
-00001860: 6869 6e67 5370 6563 5363 7265 656e 2e6f  hingSpecScreen.o
-00001870: 6e5f 6275 7474 6f6e 5f62 726f 7773 655f  n_button_browse_
-00001880: 636c 6963 6b65 6463 0100 0000 0000 0000  clickedc........
-00001890: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
-000018a0: 731c 0000 007c 006a 0064 0164 028d 0101  s....|.j.d.d....
-000018b0: 007c 006a 0164 0364 048d 0101 0064 0053  .|.j.d.d.....d.S
-000018c0: 0029 054e 46a9 01da 0765 6e61 626c 6564  .).NF....enabled
-000018d0: 5429 01da 0477 6169 7429 02da 2173 6574  T)...wait)..!set
-000018e0: 5f70 6172 616d 6574 6572 5f77 6964 6765  _parameter_widge
-000018f0: 745f 656e 6162 6c65 5f73 7461 7465 da17  t_enable_state..
-00001900: 7374 6172 745f 7374 6f70 5f62 7574 746f  start_stop_butto
-00001910: 6e5f 7374 6174 6572 1300 0000 720d 0000  n_stater....r...
-00001920: 0072 0d00 0000 720e 0000 0072 6100 0000  .r....r....ra...
-00001930: c800 0000 7304 0000 0000 010c 017a 2853  ....s........z(S
-00001940: 7769 7463 6869 6e67 5370 6563 5363 7265  witchingSpecScre
-00001950: 656e 2e65 6e74 6572 5f67 7569 5f73 7461  en.enter_gui_sta
-00001960: 7465 5f77 6169 7463 0100 0000 0000 0000  te_waitc........
-00001970: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-00001980: 732c 0000 007c 006a 0064 0164 028d 0101  s,...|.j.d.d....
-00001990: 007c 006a 0164 017c 006a 02a0 03a1 0064  .|.j.d.|.j.....d
-000019a0: 038d 0201 007c 00a0 04a1 0001 0064 0053  .....|.......d.S
-000019b0: 0029 044e 4672 8a00 0000 a902 728c 0000  .).NFr......r...
-000019c0: 00da 0a73 746f 705f 7374 6174 6529 0572  ...stop_state).r
-000019d0: 8d00 0000 728e 0000 0072 0400 0000 727a  ....r....r....rz
-000019e0: 0000 0072 4c00 0000 7213 0000 0072 0d00  ...rL...r....r..
-000019f0: 0000 720d 0000 0072 0e00 0000 7264 0000  ..r....r....rd..
-00001a00: 00cc 0000 0073 0600 0000 0001 0c01 1401  .....s..........
-00001a10: 7a2a 5377 6974 6368 696e 6753 7065 6353  z*SwitchingSpecS
-00001a20: 6372 6565 6e2e 656e 7465 725f 6775 695f  creen.enter_gui_
-00001a30: 7374 6174 655f 6163 7469 7665 6301 0000  state_activec...
-00001a40: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00001a50: 0043 0000 0073 2400 0000 7c00 6a00 6401  .C...s$...|.j.d.
-00001a60: 6402 8d01 0100 7c00 6a01 6403 7c00 6a02  d.....|.j.d.|.j.
-00001a70: a003 a100 6404 8d02 0100 6400 5300 2905  ....d.....d.S.).
-00001a80: 4e54 728a 0000 0046 728f 0000 0029 0472  NTr....Fr....).r
-00001a90: 8d00 0000 728e 0000 0072 0400 0000 727a  ....r....r....rz
-00001aa0: 0000 0072 1300 0000 720d 0000 0072 0d00  ...r....r....r..
-00001ab0: 0000 720e 0000 0072 4d00 0000 d100 0000  ..r....rM.......
-00001ac0: 7304 0000 0000 010c 017a 2853 7769 7463  s........z(Switc
-00001ad0: 6869 6e67 5370 6563 5363 7265 656e 2e65  hingSpecScreen.e
-00001ae0: 6e74 6572 5f67 7569 5f73 7461 7465 5f69  nter_gui_state_i
-00001af0: 646c 6554 728a 0000 0063 0200 0000 0000  dleTr....c......
-00001b00: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-00001b10: 0000 7340 0000 007c 006a 00a0 017c 01a1  ..s@...|.j...|..
-00001b20: 0101 007c 006a 02a0 017c 01a1 0101 007c  ...|.j...|.....|
-00001b30: 006a 03a0 017c 01a1 0101 007c 006a 04a0  .j...|.....|.j..
-00001b40: 017c 01a1 0101 007c 006a 05a0 017c 01a1  .|.....|.j...|..
-00001b50: 0101 0064 0053 0072 1000 0000 2906 7222  ...d.S.r....).r"
-00001b60: 0000 00da 0a73 6574 456e 6162 6c65 6472  .....setEnabledr
-00001b70: 2c00 0000 722d 0000 0072 2f00 0000 7235  ,...r-...r/...r5
-00001b80: 0000 0029 0272 1400 0000 728b 0000 0072  ...).r....r....r
-00001b90: 0d00 0000 720d 0000 0072 0e00 0000 728d  ....r....r....r.
-00001ba0: 0000 00d5 0000 0073 0a00 0000 0001 0c01  .......s........
-00001bb0: 0c01 0c01 0c01 7a35 5377 6974 6368 696e  ......z5Switchin
-00001bc0: 6753 7065 6353 6372 6565 6e2e 7365 745f  gSpecScreen.set_
-00001bd0: 7061 7261 6d65 7465 725f 7769 6467 6574  parameter_widget
-00001be0: 5f65 6e61 626c 655f 7374 6174 6546 728f  _enable_stateFr.
-00001bf0: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-00001c00: 0300 0000 0300 0000 4300 0000 7342 0000  ........C...sB..
-00001c10: 007c 0172 1e7c 006a 00a0 0164 01a1 0101  .|.r.|.j...d....
-00001c20: 007c 006a 00a0 0264 02a1 0101 006e 207c  .|.j...d.....n |
-00001c30: 006a 00a0 0164 03a1 0101 007c 006a 00a0  .j...d.....|.j..
-00001c40: 027c 0272 3864 046e 0264 05a1 0101 0064  .|.r8d.n.d.....d
-00001c50: 0053 0029 064e 467a 0757 6169 742e 2e2e  .S.).NFz.Wait...
-00001c60: 545a 0453 746f 7072 1800 0000 2903 723b  TZ.Stopr....).r;
-00001c70: 0000 0072 9100 0000 da07 7365 7454 6578  ...r......setTex
-00001c80: 7429 0372 1400 0000 728c 0000 0072 9000  t).r....r....r..
-00001c90: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-00001ca0: 0072 8e00 0000 dc00 0000 730a 0000 0000  .r........s.....
-00001cb0: 0104 010c 010e 020c 017a 2b53 7769 7463  .........z+Switc
-00001cc0: 6869 6e67 5370 6563 5363 7265 656e 2e73  hingSpecScreen.s
-00001cd0: 7461 7274 5f73 746f 705f 6275 7474 6f6e  tart_stop_button
-00001ce0: 5f73 7461 7465 6301 0000 0000 0000 0000  _statec.........
-00001cf0: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
-00001d00: 1400 0000 7c00 a000 a100 0100 7c00 a001  ....|.......|...
-00001d10: a100 0100 6400 5300 7210 0000 0029 02da  ....d.S.r....)..
-00001d20: 0b75 7064 6174 655f 706c 6f74 da0d 7570  .update_plot..up
-00001d30: 6461 7465 5f72 6573 756c 7472 1300 0000  date_resultr....
-00001d40: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-00001d50: 6700 0000 e400 0000 7304 0000 0000 0108  g.......s.......
-00001d60: 017a 2153 7769 7463 6869 6e67 5370 6563  .z!SwitchingSpec
-00001d70: 5363 7265 656e 2e73 686f 775f 6e65 775f  Screen.show_new_
-00001d80: 6461 7461 6301 0000 0000 0000 0000 0000  datac...........
-00001d90: 0004 0000 0004 0000 0043 0000 0073 6400  .........C...sd.
-00001da0: 0000 7c00 6a00 6a01 6a02 6a03 6401 1b00  ..|.j.j.j.j.d...
-00001db0: 7d01 7c00 6a00 6a01 6a04 6a03 7c01 1800  }.|.j.j.j.j.|...
-00001dc0: 7d02 7c00 6a00 6a01 6a04 6a03 7c01 1700  }.|.j.j.j.j.|...
-00001dd0: 7d03 7c00 6a05 a006 a100 0100 7c00 6a05  }.|.j.......|.j.
-00001de0: a007 7c02 7c03 a102 0100 7c00 6a08 a006  ..|.|.....|.j...
-00001df0: a100 0100 7c00 6a08 a007 7c02 7c03 a102  ....|.j...|.|...
-00001e00: 0100 6400 5300 2902 4e67 0000 0000 0000  ..d.S.).Ng......
-00001e10: 0040 2909 7204 0000 0072 0500 0000 7251  .@).r....r....rQ
-00001e20: 0000 0072 8400 0000 7252 0000 0072 4300  ...r....rR...rC.
-00001e30: 0000 7279 0000 00da 0b73 6574 5f72 616e  ..ry.....set_ran
-00001e40: 6765 5f78 7244 0000 0029 0472 1400 0000  ge_xrD...).r....
-00001e50: 5a0a 6861 6c66 5f72 616e 6765 5a05 6d69  Z.half_rangeZ.mi
-00001e60: 6e5f 765a 056d 6178 5f76 720d 0000 0072  n_vZ.max_vr....r
-00001e70: 0d00 0000 720e 0000 0072 6900 0000 e800  ....r....ri.....
-00001e80: 0000 730e 0000 0000 0110 0110 0110 010a  ..s.............
-00001e90: 010e 010a 017a 2453 7769 7463 6869 6e67  .....z$Switching
-00001ea0: 5370 6563 5363 7265 656e 2e73 6574 5f64  SpecScreen.set_d
-00001eb0: 6174 615f 696e 7661 6c69 6463 0100 0000  ata_invalidc....
-00001ec0: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00001ed0: 4300 0000 730e 0000 007c 006a 00a0 01a1  C...s....|.j....
-00001ee0: 007d 0164 0053 0072 1000 0000 2902 7204  .}.d.S.r....).r.
-00001ef0: 0000 00da 0a67 6574 5f72 6573 756c 7429  .....get_result)
-00001f00: 0272 1400 0000 da03 7265 7372 0d00 0000  .r......resr....
-00001f10: 720d 0000 0072 0e00 0000 7294 0000 00f1  r....r....r.....
-00001f20: 0000 0073 0200 0000 0001 7a21 5377 6974  ...s......z!Swit
-00001f30: 6368 696e 6753 7065 6353 6372 6565 6e2e  chingSpecScreen.
-00001f40: 7570 6461 7465 5f72 6573 756c 7463 0100  update_resultc..
-00001f50: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00001f60: 0000 4300 0000 73ba 0000 007c 006a 00a0  ..C...s....|.j..
-00001f70: 01a1 007d 017c 006a 02a0 0374 046a 056a  ...}.|.j...t.j.j
-00001f80: 066a 076a 087c 016a 09a1 0201 007c 006a  .j.j.|.j.....|.j
-00001f90: 0aa0 0374 046a 056a 066a 076a 087c 016a  ...t.j.j.j.j.|.j
-00001fa0: 09a1 0201 007c 006a 02a0 0374 046a 056a  .....|.j...t.j.j
-00001fb0: 066a 076a 0b7c 016a 0ca1 0201 007c 006a  .j.j.|.j.....|.j
-00001fc0: 026a 0d7c 016a 0e7c 016a 0f64 0164 028d  .j.|.j.|.j.d.d..
-00001fd0: 0301 007c 006a 0a6a 0d7c 016a 0e7c 016a  ...|.j.j.|.j.|.j
-00001fe0: 1064 0164 028d 0301 007c 006a 006a 116a  .d.d.....|.j.j.j
-00001ff0: 126a 1372 b67c 006a 026a 0d7c 016a 0e7c  .j.r.|.j.j.|.j.|
-00002000: 016a 1464 0364 028d 0301 007c 006a 0a6a  .j.d.d.....|.j.j
-00002010: 0d7c 016a 0e7c 016a 1564 0364 028d 0301  .|.j.|.j.d.d....
-00002020: 0064 0053 0029 044e 7201 0000 0029 03da  .d.S.).Nr....)..
-00002030: 0178 da01 79da 0b6c 6179 6572 5f69 6e64  .x..y..layer_ind
-00002040: 6578 7207 0000 0029 1672 0400 0000 7296  exr....).r....r.
-00002050: 0000 0072 4300 0000 7277 0000 0072 1c00  ...rC...rw...r..
-00002060: 0000 721d 0000 0072 4200 0000 7274 0000  ..r....rB...rt..
-00002070: 0072 7500 0000 da0c 6f75 7470 7574 735f  .ru.....outputs_
-00002080: 756e 6974 7244 0000 0072 7800 0000 da0f  unitrD...rx.....
-00002090: 616d 706c 6974 7564 6573 5f75 6e69 74da  amplitudes_unit.
-000020a0: 0970 6c6f 745f 6461 7461 da07 6f75 7470  .plot_data..outp
-000020b0: 7574 73da 0e61 6d70 6c69 7475 6465 735f  uts..amplitudes_
-000020c0: 6f66 66da 0a70 6861 7365 735f 6f66 6672  off..phases_offr
-000020d0: 0500 0000 725a 0000 0072 8400 0000 da0d  ....rZ...r......
-000020e0: 616d 706c 6974 7564 6573 5f6f 6eda 0970  amplitudes_on..p
-000020f0: 6861 7365 735f 6f6e 2902 7214 0000 00da  hases_on).r.....
-00002100: 0c63 7572 7265 6e74 5f64 6174 6172 0d00  .current_datar..
-00002110: 0000 720d 0000 0072 0e00 0000 7293 0000  ..r....r....r...
-00002120: 00f7 0000 0073 1200 0000 0001 0a01 1801  .....s..........
-00002130: 1801 1801 1601 1601 0c01 1601 7a1f 5377  ............z.Sw
-00002140: 6974 6368 696e 6753 7065 6353 6372 6565  itchingSpecScree
-00002150: 6e2e 7570 6461 7465 5f70 6c6f 7463 0100  n.update_plotc..
-00002160: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00002170: 0000 4300 0000 7314 0000 007c 00a0 00a1  ..C...s....|....
-00002180: 0001 007c 00a0 01a1 0001 0064 0053 0072  ...|.......d.S.r
-00002190: 1000 0000 2902 724c 0000 0072 9300 0000  ....).rL...r....
-000021a0: 7213 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-000021b0: 0e00 0000 726b 0000 0002 0100 0073 0400  ....rk.......s..
-000021c0: 0000 0001 0801 7a24 5377 6974 6368 696e  ......z$Switchin
-000021d0: 6753 7065 6353 6372 6565 6e2e 6368 616e  gSpecScreen.chan
-000021e0: 6765 5f70 6c6f 745f 7669 6577 2901 5429  ge_plot_view).T)
-000021f0: 0246 4629 1872 0900 0000 720a 0000 0072  .FF).r....r....r
-00002200: 0b00 0000 7212 0000 0072 0400 0000 da13  ....r....r......
-00002210: 5377 6974 6368 696e 6753 7065 634d 6f64  SwitchingSpecMod
-00002220: 756c 6572 4e00 0000 724b 0000 0072 4c00  ulerN...rK...rL.
-00002230: 0000 725d 0000 0072 5e00 0000 725f 0000  ..r]...r^...r_..
-00002240: 0072 6100 0000 7264 0000 0072 4d00 0000  .ra...rd...rM...
-00002250: da04 626f 6f6c 728d 0000 0072 8e00 0000  ..boolr....r....
-00002260: 7267 0000 0072 6900 0000 7294 0000 0072  rg...ri...r....r
-00002270: 9300 0000 726b 0000 00da 0d5f 5f63 6c61  ....rk.....__cla
-00002280: 7373 6365 6c6c 5f5f 720d 0000 0072 0d00  sscell__r....r..
-00002290: 0000 7215 0000 0072 0e00 0000 720f 0000  ..r....r....r...
-000022a0: 001f 0000 0073 2200 0000 0801 0c04 1064  .....s"........d
-000022b0: 0820 080f 0806 0803 0808 0804 0805 0804  . ..............
-000022c0: 1007 1208 0804 0809 0806 080b 720f 0000  ............r...
-000022d0: 0029 2472 0c00 0000 7287 0000 00da 0750  .)$r....r......P
-000022e0: 7953 6964 6536 7202 0000 00da 0e50 7953  ySide6r......PyS
-000022f0: 6964 6536 2e51 7443 6f72 6572 0300 0000  ide6.QtCorer....
-00002300: da08 6e61 6e6f 7375 7266 721c 0000 00da  ..nanosurfr.....
-00002310: 1573 7769 7463 6869 6e67 5f73 7065 635f  .switching_spec_
-00002320: 6d6f 6475 6c65 7204 0000 0072 0500 0000  moduler....r....
-00002330: 721d 0000 00da 0a6e 7366 5f74 6162 6c65  r......nsf_table
-00002340: 73da 0d54 6162 6c65 456e 7472 7949 4473  s..TableEntryIDs
-00002350: 7206 0000 00da 0d4e 5346 436f 6d62 6f45  r......NSFComboE
-00002360: 6e74 7279 da0f 4f75 7470 7574 4368 616e  ntry..OutputChan
-00002370: 6e65 6c49 44da 0555 7365 7231 da05 5573  nelID..User1..Us
-00002380: 6572 32da 0a54 6970 566f 6c74 6167 6572  er2..TipVoltager
-00002390: 1f00 0000 7226 0000 0072 2700 0000 7228  ....r&...r'...r(
-000023a0: 0000 0072 2900 0000 7232 0000 00da 056d  ...r)...r2.....m
-000023b0: 696c 6c69 7230 0000 00da 056d 6963 726f  illir0.....micro
-000023c0: da04 6e61 6e6f 722e 0000 0072 2400 0000  ..nanor....r$...
-000023d0: da0a 6672 616d 6577 6f72 6b73 da06 7174  ..frameworks..qt
-000023e0: 5f61 7070 da0c 4d6f 6475 6c65 5363 7265  _app..ModuleScre
-000023f0: 656e 720f 0000 0072 0d00 0000 720d 0000  enr....r....r...
-00002400: 0072 0d00 0000 720e 0000 00da 083c 6d6f  .r....r......<mo
-00002410: 6475 6c65 3e01 0000 0073 1e00 0000 0405  dule>....s......
-00002420: 0801 0c01 0c01 0802 1002 1607 1001 1001  ................
-00002430: 10fd 0407 0e01 1801 2201 2202            ........".".
+00000740: 0001 007c 006a 25a0 2974 016a 2a6a 2b6a  ...|.j%.)t.j*j+j
+00000750: 2ca0 2da1 00a1 0101 007c 006a 25a0 267c  ,.-......|.j%.&|
+00000760: 006a 21a1 0101 0074 016a 026a 2e64 1a64  .j!....t.j.j.d.d
+00000770: 1b8d 017c 005f 2f74 016a 026a 2e64 1a64  ...|._/t.j.j.d.d
+00000780: 1b8d 017c 005f 3074 18a0 24a1 007c 005f  ...|._0t..$..|._
+00000790: 317c 006a 31a0 267c 006a 2fa1 0101 007c  1|.j1.&|.j/....|
+000007a0: 006a 31a0 267c 006a 30a1 0101 0074 18a0  .j1.&|.j0....t..
+000007b0: 32a1 007c 005f 337c 006a 33a0 267c 006a  2..|._3|.j3.&|.j
+000007c0: 1ea1 0101 007c 006a 336a 267c 006a 2274  .....|.j3j&|.j"t
+000007d0: 346a 356a 3664 1c8d 0201 007c 006a 31a0  4j5j6d.....|.j1.
+000007e0: 377c 006a 33a1 0101 0074 18a0 32a1 007c  7|.j3....t..2..|
+000007f0: 005f 3874 18a0 24a1 007c 005f 397c 006a  ._8t..$..|._9|.j
+00000800: 39a0 267c 006a 1da1 0101 007c 006a 38a0  9.&|.j.....|.j8.
+00000810: 377c 006a 39a1 0101 007c 006a 386a 267c  7|.j9....|.j8j&|
+00000820: 006a 1674 346a 356a 3a64 1c8d 0201 007c  .j.t4j5j:d.....|
+00000830: 006a 386a 267c 006a 1f74 346a 356a 3a64  .j8j&|.j.t4j5j:d
+00000840: 1c8d 0201 007c 006a 38a0 28a1 0001 007c  .....|.j8.(....|
+00000850: 006a 386a 267c 006a 2374 346a 356a 3a64  .j8j&|.j#t4j5j:d
+00000860: 1c8d 0201 007c 006a 31a0 377c 006a 38a1  .....|.j1.7|.j8.
+00000870: 0101 0074 18a0 24a1 007c 005f 3b74 18a0  ...t..$..|._;t..
+00000880: 32a1 007c 005f 3c7c 006a 3ca0 377c 006a  2..|._<|.j<.7|.j
+00000890: 2564 0aa1 0201 007c 006a 3ca0 377c 006a  %d.....|.j<.7|.j
+000008a0: 3164 0fa1 0201 007c 006a 3ca0 377c 006a  1d.....|.j<.7|.j
+000008b0: 3b64 0aa1 0201 007c 00a0 3d7c 006a 3ca1  ;d.....|..=|.j<.
+000008c0: 0101 007c 00a0 3ea1 0001 007c 00a0 3fa1  ...|..>....|..?.
+000008d0: 0001 007c 00a0 40a1 0001 0064 1d53 0029  ...|..@....d.S.)
+000008e0: 1e7a 3820 6372 6561 7465 2068 6572 6520  .z8 create here 
+000008f0: 796f 7572 2067 7569 2077 6974 6820 616c  your gui with al
+00000900: 6c20 636f 6e74 726f 6c73 2061 6e64 2074  l controls and t
+00000910: 6865 6972 206c 6179 6f75 74da 064f 7574  heir layout..Out
+00000920: 7075 747a 0d56 6f6c 7461 6765 2072 616e  putz.Voltage ran
+00000930: 6765 7208 0000 0067 0000 0000 0000 0000  ger....g........
+00000940: 6700 0000 0000 409f 407a 0d43 656e 7465  g.....@.@z.Cente
+00000950: 7220 6f66 6673 6574 6700 0000 0000 408f  r offsetg.....@.
+00000960: c067 0000 0000 0040 8f40 7a0f 4e75 6d62  .g.....@.@z.Numb
+00000970: 6572 206f 6620 7374 6570 7372 0100 0000  er of stepsr....
+00000980: 69e8 0300 007a 1554 696d 6520 6465 6c61  i....z.Time dela
+00000990: 7920 6166 7465 7220 7374 6570 6700 0000  y after stepg...
+000009a0: 0000 00f0 3f7a 0a46 696c 6520 696e 6465  ....?z.File inde
+000009b0: 7872 0700 0000 6910 2700 007a 0e53 686f  xr....i.'..z.Sho
+000009c0: 7720 276f 6e27 2064 6174 617a 0e42 6163  w 'on' dataz.Bac
+000009d0: 6b77 6172 6420 6669 7273 747a 0e46 696c  kward firstz.Fil
+000009e0: 6520 6e61 6d65 206d 6173 6b7a 1044 6573  e name maskz.Des
+000009f0: 7469 6e61 7469 6f6e 2070 6174 687a 0e41  tination pathz.A
+00000a00: 7574 6f20 7361 7665 2064 6174 61da 0553  uto save data..S
+00000a10: 7461 7274 5a06 4272 6f77 7365 7a09 5361  tartZ.Browsez.Sa
+00000a20: 7665 2064 6174 61e9 0a00 0000 4629 01da  ve data.....F)..
+00000a30: 086c 6f67 6d6f 6465 7829 01da 0961 6c69  .logmodex)...ali
+00000a40: 676e 6d65 6e74 4e29 4172 0400 0000 da03  gnmentN)Ar......
+00000a50: 6e73 66da 0367 7569 da0b 4e53 4643 6f6d  nsf..gui..NSFCom
+00000a60: 626f 426f 78da 1343 6f6d 626f 4f75 7470  boBox..ComboOutp
+00000a70: 7574 4368 616e 6e65 6c73 da0f 636f 6d62  utChannels..comb
+00000a80: 6f5f 6f75 7470 7574 5f69 64da 0a4e 5346  o_output_id..NSF
+00000a90: 5363 6945 6469 74da 1273 6369 7661 6c5f  SciEdit..scival_
+00000aa0: 6f75 7470 7574 5f73 7061 6eda 1673 6574  output_span..set
+00000ab0: 5f61 6c6c 6f77 6564 5f70 7265 6669 785f  _allowed_prefix_
+00000ac0: 6964 73da 1261 6c6c 6f77 6564 5f76 6f6c  ids..allowed_vol
+00000ad0: 745f 756e 6974 73da 0d73 6574 5f70 7265  t_units..set_pre
+00000ae0: 6669 785f 6964 da07 7363 695f 7661 6cda  fix_id..sci_val.
+00000af0: 0275 70da 0650 7265 6669 78da 0462 6173  .up..Prefix..bas
+00000b00: 65da 0d73 6574 5f70 7265 6369 7369 6f6e  e..set_precision
+00000b10: da11 7365 745f 7661 6c75 655f 6d69 6e5f  ..set_value_min_
+00000b20: 6d61 78da 1473 6369 7661 6c5f 6f75 7470  max..scival_outp
+00000b30: 7574 5f63 656e 7465 72da 1073 6369 7661  ut_center..sciva
+00000b40: 6c5f 6e75 6d5f 7374 6570 73da 1361 6c6c  l_num_steps..all
+00000b50: 6f77 6564 5f6d 6574 6572 5f75 6e69 7473  owed_meter_units
+00000b60: da11 7363 6976 616c 5f74 696d 655f 6465  ..scival_time_de
+00000b70: 6c61 79da 1261 6c6c 6f77 6564 5f74 696d  lay..allowed_tim
+00000b80: 655f 756e 6974 73da 1173 6369 7661 6c5f  e_units..scival_
+00000b90: 6669 6c65 5f69 6e64 6578 da13 616c 6c6f  file_index..allo
+00000ba0: 7765 645f 636f 756e 745f 756e 6974 7372  wed_count_unitsr
+00000bb0: 0200 0000 da09 5143 6865 636b 426f 78da  ......QCheckBox.
+00000bc0: 1263 6865 636b 5f73 686f 775f 6f6e 5f64  .check_show_on_d
+00000bd0: 6174 61da 1463 6865 636b 5f64 6f5f 7265  ata..check_do_re
+00000be0: 7665 7273 5f72 616d 70da 074e 5346 4564  vers_ramp..NSFEd
+00000bf0: 6974 da0e 6564 6974 5f66 696c 655f 6d61  it..edit_file_ma
+00000c00: 736b da0e 6564 6974 5f66 696c 655f 7061  sk..edit_file_pa
+00000c10: 7468 da0f 6368 6563 6b5f 6175 746f 5f73  th..check_auto_s
+00000c20: 6176 65da 0b51 5075 7368 4275 7474 6f6e  ave..QPushButton
+00000c30: da11 6275 7474 6f6e 5f73 7461 7274 5f73  ..button_start_s
+00000c40: 746f 70da 0d62 7574 746f 6e5f 6272 6f77  top..button_brow
+00000c50: 7365 da0d 6275 7474 6f6e 5f65 7870 6f72  se..button_expor
+00000c60: 74da 0b51 5642 6f78 4c61 796f 7574 5a0b  t..QVBoxLayoutZ.
+00000c70: 6c61 796f 7574 5f6c 6566 74da 0961 6464  layout_left..add
+00000c80: 5769 6467 6574 da0a 6164 6453 7061 6369  Widget..addSpaci
+00000c90: 6e67 da0a 6164 6453 7472 6574 6368 da0d  ng..addStretch..
+00000ca0: 6164 6453 7061 6365 7249 7465 6dda 0a66  addSpacerItem..f
+00000cb0: 7261 6d65 776f 726b 73da 0671 745f 6170  rameworks..qt_ap
+00000cc0: 70da 0761 7070 5f67 7569 da0a 5374 6456  p..app_gui..StdV
+00000cd0: 5370 6163 6572 da08 4e53 4643 6861 7274  Spacer..NSFChart
+00000ce0: da09 6368 6172 745f 616d 70da 0b63 6861  ..chart_amp..cha
+00000cf0: 7274 5f70 6861 7365 5a0a 6c61 796f 7574  rt_phaseZ.layout
+00000d00: 5f6d 6964 da0b 5148 426f 784c 6179 6f75  _mid..QHBoxLayou
+00000d10: 745a 0b6c 6179 6f75 745f 7061 7468 7203  tZ.layout_pathr.
+00000d20: 0000 00da 0d41 6c69 676e 6d65 6e74 466c  .....AlignmentFl
+00000d30: 6167 da0d 416c 6967 6e42 6173 656c 696e  ag..AlignBaselin
+00000d40: 65da 0961 6464 4c61 796f 7574 5a0b 6c61  e..addLayoutZ.la
+00000d50: 796f 7574 5f66 696c 655a 106c 6179 6f75  yout_fileZ.layou
+00000d60: 745f 6669 6c65 5f6d 6173 6bda 0c41 6c69  t_file_mask..Ali
+00000d70: 676e 5643 656e 7465 725a 0c6c 6179 6f75  gnVCenterZ.layou
+00000d80: 745f 7269 6768 745a 0d73 6372 6565 6e5f  t_rightZ.screen_
+00000d90: 6c61 796f 7574 da09 7365 744c 6179 6f75  layout..setLayou
+00000da0: 74da 1162 696e 645f 6775 695f 656c 656d  t..bind_gui_elem
+00000db0: 656e 7473 da09 696e 6974 5f70 6c6f 74da  ents..init_plot.
+00000dc0: 1465 6e74 6572 5f67 7569 5f73 7461 7465  .enter_gui_state
+00000dd0: 5f69 646c 6529 0272 1400 0000 7204 0000  _idle).r....r...
+00000de0: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+00000df0: da0f 646f 5f73 6574 7570 5f73 6372 6565  ..do_setup_scree
+00000e00: 6e24 0000 0073 9600 0000 0002 0604 1002  n$...s..........
+00000e10: 0e01 0c01 1401 0c01 0e02 0e01 0c01 1401  ................
+00000e20: 0c01 0e02 0e01 0c01 1401 0c01 0e02 0e01  ................
+00000e30: 0c01 1401 0c01 0e02 0e01 0c01 1401 0c01  ................
+00000e40: 0e02 0c01 0c02 0e01 0e02 0c01 0c01 0c01  ................
+00000e50: 0c02 0a01 0e01 0e01 0e01 0e01 0e01 0c01  ................
+00000e60: 0e01 0c01 0e01 0a01 1601 0e04 1001 1002  ................
+00000e70: 0a01 0e01 0e01 0a01 0e01 1601 0e01 0a01  ................
+00000e80: 0a01 0e01 0e01 1601 1601 0a01 1601 0e04  ................
+00000e90: 0a03 0a02 1001 1001 1001 0c02 0801 0801  ................
+00000ea0: 7a23 5377 6974 6368 696e 6753 7065 6353  z#SwitchingSpecS
+00000eb0: 6372 6565 6e2e 646f 5f73 6574 7570 5f73  creen.do_setup_s
+00000ec0: 6372 6565 6e63 0100 0000 0000 0000 0000  creenc..........
+00000ed0: 0000 0100 0000 0400 0000 4300 0000 73ae  ..........C...s.
+00000ee0: 0100 0074 006a 01a0 027c 006a 037c 006a  ...t.j...|.j.|.j
+00000ef0: 046a 056a 06a1 0201 0074 006a 01a0 027c  .j.j.....t.j...|
+00000f00: 006a 077c 006a 046a 056a 08a1 0201 0074  .j.|.j.j.j.....t
+00000f10: 006a 01a0 027c 006a 097c 006a 046a 056a  .j...|.j.|.j.j.j
+00000f20: 0aa1 0201 0074 006a 01a0 027c 006a 0b7c  .....t.j...|.j.|
+00000f30: 006a 046a 056a 0ca1 0201 0074 006a 01a0  .j.j.j.....t.j..
+00000f40: 027c 006a 0d7c 006a 046a 056a 0ea1 0201  .|.j.|.j.j.j....
+00000f50: 0074 006a 01a0 027c 006a 0f7c 006a 046a  .t.j...|.j.|.j.j
+00000f60: 056a 10a1 0201 0074 006a 01a0 027c 006a  .j.....t.j...|.j
+00000f70: 117c 006a 046a 056a 12a1 0201 0074 006a  .|.j.j.j.....t.j
+00000f80: 01a0 027c 006a 137c 006a 046a 056a 14a1  ...|.j.|.j.j.j..
+00000f90: 0201 0074 006a 01a0 027c 006a 157c 006a  ...t.j...|.j.|.j
+00000fa0: 046a 056a 16a1 0201 0074 006a 01a0 027c  .j.j.....t.j...|
+00000fb0: 006a 177c 006a 046a 056a 18a1 0201 0074  .j.|.j.j.j.....t
+00000fc0: 006a 01a0 027c 006a 197c 006a 046a 056a  .j...|.j.|.j.j.j
+00000fd0: 1aa1 0201 007c 006a 1b6a 1ca0 1d7c 006a  .....|.j.j...|.j
+00000fe0: 1ea1 0101 007c 006a 1f6a 1ca0 1d7c 006a  .....|.j.j...|.j
+00000ff0: 20a1 0101 007c 006a 216a 1ca0 1d7c 006a   ....|.j!j...|.j
+00001000: 22a1 0101 007c 006a 046a 23a0 1d7c 006a  "....|.j.j#..|.j
+00001010: 24a1 0101 007c 006a 046a 25a0 1d7c 006a  $....|.j.j%..|.j
+00001020: 24a1 0101 007c 006a 046a 26a0 1d7c 006a  $....|.j.j&..|.j
+00001030: 27a1 0101 007c 006a 046a 28a0 1d7c 006a  '....|.j.j(..|.j
+00001040: 29a1 0101 007c 006a 046a 2aa0 1d7c 006a  )....|.j.j*..|.j
+00001050: 2ba1 0101 007c 006a 046a 2ca0 1d7c 006a  +....|.j.j,..|.j
+00001060: 2da1 0101 007c 006a 046a 056a 1a6a 2ea0  -....|.j.j.j.j..
+00001070: 1d7c 006a 2fa1 0101 007c 006a 046a 056a  .|.j/....|.j.j.j
+00001080: 066a 2ea0 1d7c 006a 30a1 0101 0064 0153  .j...|.j0....d.S
+00001090: 0029 027a 4020 636f 6e6e 6563 7420 616c  .).z@ connect al
+000010a0: 6c20 6775 6920 7769 6467 6574 7320 746f  l gui widgets to
+000010b0: 206d 6f64 756c 6520 7365 7474 696e 6773   module settings
+000010c0: 206f 7220 616e 7920 6f74 6865 7220 736f   or any other so
+000010d0: 7572 6365 204e 2931 721c 0000 0072 1d00  urce N)1r....r..
+000010e0: 0000 da13 636f 6e6e 6563 745f 746f 5f70  ....connect_to_p
+000010f0: 726f 7065 7274 7972 2000 0000 7204 0000  ropertyr ...r...
+00001100: 0072 0500 0000 da09 6f75 7470 7574 5f69  .r......output_i
+00001110: 6472 2200 0000 da0b 6f75 7470 7574 5f73  dr".....output_s
+00001120: 7061 6e72 2c00 0000 da0d 6f75 7470 7574  panr,.....output
+00001130: 5f63 656e 7465 7272 2d00 0000 da0f 6e75  _centerr-.....nu
+00001140: 6d62 6572 5f6f 665f 7374 6570 7372 2f00  mber_of_stepsr/.
+00001150: 0000 da15 7469 6d65 5f64 656c 6179 5f61  ....time_delay_a
+00001160: 6674 6572 5f73 7465 7072 3800 0000 da0b  fter_stepr8.....
+00001170: 666f 6c64 6572 5f6e 616d 6572 3700 0000  folder_namer7...
+00001180: da0e 6669 6c65 5f6e 616d 655f 6d61 736b  ..file_name_mask
+00001190: 7231 0000 00da 0a66 696c 655f 696e 6465  r1.....file_inde
+000011a0: 7872 3900 0000 da0e 6175 746f 5f73 6176  xr9.....auto_sav
+000011b0: 655f 6461 7461 7235 0000 00da 0b72 6576  e_datar5.....rev
+000011c0: 6572 735f 7261 6d70 7234 0000 00da 1373  ers_rampr4.....s
+000011d0: 686f 775f 6f6e 5f64 6174 615f 7661 6c75  how_on_data_valu
+000011e0: 6573 723b 0000 00da 0763 6c69 636b 6564  esr;.....clicked
+000011f0: da07 636f 6e6e 6563 74da 1c6f 6e5f 6275  ..connect..on_bu
+00001200: 7474 6f6e 5f73 7461 7274 5f73 746f 705f  tton_start_stop_
+00001210: 636c 6963 6b65 6472 3d00 0000 da18 6f6e  clickedr=.....on
+00001220: 5f62 7574 746f 6e5f 6578 706f 7274 5f63  _button_export_c
+00001230: 6c69 636b 6564 723c 0000 00da 186f 6e5f  lickedr<.....on_
+00001240: 6275 7474 6f6e 5f62 726f 7773 655f 636c  button_browse_cl
+00001250: 6963 6b65 64da 1873 6967 5f77 6f72 6b5f  icked..sig_work_
+00001260: 7374 6172 745f 7265 7175 6573 7465 64da  start_requested.
+00001270: 1465 6e74 6572 5f67 7569 5f73 7461 7465  .enter_gui_state
+00001280: 5f77 6169 74da 1773 6967 5f77 6f72 6b5f  _wait..sig_work_
+00001290: 7374 6f70 5f72 6571 7565 7374 6564 da0f  stop_requested..
+000012a0: 7369 675f 776f 726b 5f61 6374 6976 65da  sig_work_active.
+000012b0: 1665 6e74 6572 5f67 7569 5f73 7461 7465  .enter_gui_state
+000012c0: 5f61 6374 6976 65da 0d73 6967 5f77 6f72  _active..sig_wor
+000012d0: 6b5f 646f 6e65 7252 0000 00da 1673 6967  k_donerR.....sig
+000012e0: 5f6e 6577 5f64 6174 615f 6176 6169 6c61  _new_data_availa
+000012f0: 626c 65da 0d73 686f 775f 6e65 775f 6461  ble..show_new_da
+00001300: 7461 da10 7369 675f 6461 7461 5f69 6e76  ta..sig_data_inv
+00001310: 616c 6964 da10 7365 745f 6461 7461 5f69  alid..set_data_i
+00001320: 6e76 616c 6964 da11 7369 675f 7661 6c75  nvalid..sig_valu
+00001330: 655f 6368 616e 6765 64da 1063 6861 6e67  e_changed..chang
+00001340: 655f 706c 6f74 5f76 6965 7772 5100 0000  e_plot_viewrQ...
+00001350: 7213 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00001360: 0e00 0000 7250 0000 0089 0000 0073 2c00  ....rP.......s,.
+00001370: 0000 0004 1601 1601 1601 1601 1601 1601  ................
+00001380: 1601 1601 1601 1601 1603 1001 1001 1003  ................
+00001390: 1001 1001 1001 1001 1001 1002 1401 7a25  ..............z%
+000013a0: 5377 6974 6368 696e 6753 7065 6353 6372  SwitchingSpecScr
+000013b0: 6565 6e2e 6269 6e64 5f67 7569 5f65 6c65  een.bind_gui_ele
+000013c0: 6d65 6e74 7363 0100 0000 0000 0000 0000  mentsc..........
+000013d0: 0000 0100 0000 0600 0000 4300 0000 7312  ..........C...s.
+000013e0: 0100 007c 006a 00a0 0164 01a1 0101 007c  ...|.j...d.....|
+000013f0: 006a 00a0 0274 036a 046a 056a 066a 0764  .j...t.j.j.j.j.d
+00001400: 027c 006a 08a0 09a1 009b 0064 039d 03a1  .|.j.......d....
+00001410: 0201 007c 006a 00a0 0a74 036a 046a 056a  ...|.j...t.j.j.j
+00001420: 066a 0764 04a1 0201 007c 006a 00a0 0a74  .j.d.....|.j...t
+00001430: 036a 046a 056a 066a 0b64 04a1 0201 007c  .j.j.j.j.d.....|
+00001440: 006a 00a0 0274 036a 046a 056a 066a 0b64  .j...t.j.j.j.j.d
+00001450: 01a1 0201 007c 006a 00a0 0a74 036a 046a  .....|.j...t.j.j
+00001460: 056a 066a 0b64 05a1 0201 007c 006a 00a0  .j.j.d.....|.j..
+00001470: 0ca1 0001 007c 006a 0da0 0164 06a1 0101  .....|.j...d....
+00001480: 007c 006a 0da0 0274 036a 046a 056a 066a  .|.j...t.j.j.j.j
+00001490: 0764 027c 006a 08a0 09a1 009b 0064 039d  .d.|.j.......d..
+000014a0: 03a1 0201 007c 006a 0da0 0a74 036a 046a  .....|.j...t.j.j
+000014b0: 056a 066a 0764 04a1 0201 007c 006a 0da0  .j.j.d.....|.j..
+000014c0: 0274 036a 046a 056a 066a 0b64 06a1 0201  .t.j.j.j.j.d....
+000014d0: 007c 006a 0da0 0a74 036a 046a 056a 066a  .|.j...t.j.j.j.j
+000014e0: 0b64 07a1 0201 007c 006a 0da0 0ca1 0001  .d.....|.j......
+000014f0: 0064 0053 0029 084e da09 416d 706c 6974  .d.S.).N..Amplit
+00001500: 7564 657a 084f 7574 7075 7420 27fa 0127  udez.Output '..'
+00001510: da00 da01 56da 0550 6861 7365 f502 0000  ....V..Phase....
+00001520: 00c2 b029 0e72 4800 0000 da09 7365 745f  ...).rH.....set_
+00001530: 7469 746c 65da 0973 6574 5f6c 6162 656c  title..set_label
+00001540: 721c 0000 0072 1d00 0000 7247 0000 00da  r....r....rG....
+00001550: 0441 7869 73da 0662 6f74 746f 6d72 2000  .Axis..bottomr .
+00001560: 0000 da12 6375 7272 656e 745f 656e 7472  ....current_entr
+00001570: 795f 6e61 6d65 da08 7365 745f 756e 6974  y_name..set_unit
+00001580: da04 6c65 6674 da0b 636c 6561 725f 706c  ..left..clear_pl
+00001590: 6f74 7372 4900 0000 7213 0000 0072 0d00  otsrI...r....r..
+000015a0: 0000 720d 0000 0072 0e00 0000 7251 0000  ..r....r....rQ..
+000015b0: 00a9 0000 0073 1a00 0000 0001 0c01 2401  .....s........$.
+000015c0: 1601 1601 1601 1601 0a01 0c01 2401 1601  ............$...
+000015d0: 1601 1601 7a1d 5377 6974 6368 696e 6753  ....z.SwitchingS
+000015e0: 7065 6353 6372 6565 6e2e 696e 6974 5f70  pecScreen.init_p
+000015f0: 6c6f 7463 0100 0000 0000 0000 0000 0000  lotc............
+00001600: 0100 0000 0200 0000 4300 0000 7324 0000  ........C...s$..
+00001610: 007c 006a 00a0 01a1 0072 167c 006a 00a0  .|.j.....r.|.j..
+00001620: 02a1 0001 006e 0a7c 006a 00a0 03a1 0001  .....n.|.j......
+00001630: 0064 0053 0072 1000 0000 2904 7204 0000  .d.S.r....).r...
+00001640: 00da 0e69 735f 776f 726b 6572 5f62 7573  ...is_worker_bus
+00001650: 79da 0b73 746f 705f 776f 726b 6572 da0c  y..stop_worker..
+00001660: 7374 6172 745f 776f 726b 6572 7213 0000  start_workerr...
+00001670: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+00001680: 7262 0000 00b8 0000 0073 0600 0000 0001  rb.......s......
+00001690: 0a01 0c02 7a30 5377 6974 6368 696e 6753  ....z0SwitchingS
+000016a0: 7065 6353 6372 6565 6e2e 6f6e 5f62 7574  pecScreen.on_but
+000016b0: 746f 6e5f 7374 6172 745f 7374 6f70 5f63  ton_start_stop_c
+000016c0: 6c69 636b 6564 6301 0000 0000 0000 0000  lickedc.........
+000016d0: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+000016e0: 0e00 0000 7c00 6a00 a001 a100 0100 6400  ....|.j.......d.
+000016f0: 5300 7210 0000 0029 0272 0400 0000 da09  S.r....).r......
+00001700: 7361 7665 5f64 6174 6172 1300 0000 720d  save_datar....r.
+00001710: 0000 0072 0d00 0000 720e 0000 0072 6300  ...r....r....rc.
+00001720: 0000 be00 0000 7302 0000 0000 017a 2c53  ......s......z,S
+00001730: 7769 7463 6869 6e67 5370 6563 5363 7265  witchingSpecScre
+00001740: 656e 2e6f 6e5f 6275 7474 6f6e 5f65 7870  en.on_button_exp
+00001750: 6f72 745f 636c 6963 6b65 6463 0100 0000  ort_clickedc....
+00001760: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00001770: 4300 0000 7358 0000 0074 00a0 01a1 007d  C...sX...t.....}
+00001780: 017c 01a0 0274 006a 016a 036a 04a1 0101  .|...t.j.j.j....
+00001790: 007c 01a0 0574 067c 006a 076a 086a 096a  .|...t.|.j.j.j.j
+000017a0: 0a83 01a1 0101 007c 01a0 0ba1 0072 547c  .......|.....rT|
+000017b0: 01a0 0ca1 007d 0274 0da0 0e7c 0264 0119  .....}.t...|.d..
+000017c0: 00a1 017c 006a 076a 086a 095f 0a64 0053  ...|.j.j.j._.d.S
+000017d0: 0029 024e 7201 0000 0029 0f72 0200 0000  .).Nr....).r....
+000017e0: da0b 5146 696c 6544 6961 6c6f 67da 0b73  ..QFileDialog..s
+000017f0: 6574 4669 6c65 4d6f 6465 da08 4669 6c65  etFileMode..File
+00001800: 4d6f 6465 da09 4469 7265 6374 6f72 79da  Mode..Directory.
+00001810: 0c73 6574 4469 7265 6374 6f72 79da 0373  .setDirectory..s
+00001820: 7472 7204 0000 0072 0500 0000 725a 0000  trr....r....rZ..
+00001830: 00da 0576 616c 7565 da05 6578 6563 5fda  ...value..exec_.
+00001840: 0d73 656c 6563 7465 6446 696c 6573 da07  .selectedFiles..
+00001850: 7061 7468 6c69 62da 0450 6174 6829 0372  pathlib..Path).r
+00001860: 1400 0000 da03 646c 675a 0966 696c 654e  ......dlgZ.fileN
+00001870: 616d 6573 720d 0000 0072 0d00 0000 720e  amesr....r....r.
+00001880: 0000 0072 6400 0000 c100 0000 730c 0000  ...rd.......s...
+00001890: 0000 0108 0110 0116 0108 0108 017a 2c53  .............z,S
+000018a0: 7769 7463 6869 6e67 5370 6563 5363 7265  witchingSpecScre
+000018b0: 656e 2e6f 6e5f 6275 7474 6f6e 5f62 726f  en.on_button_bro
+000018c0: 7773 655f 636c 6963 6b65 6463 0100 0000  wse_clickedc....
+000018d0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+000018e0: 4300 0000 731c 0000 007c 006a 0064 0164  C...s....|.j.d.d
+000018f0: 028d 0101 007c 006a 0164 0364 048d 0101  .....|.j.d.d....
+00001900: 0064 0053 0029 054e 46a9 01da 0765 6e61  .d.S.).NF....ena
+00001910: 626c 6564 5429 01da 0477 6169 7429 02da  bledT)...wait)..
+00001920: 2173 6574 5f70 6172 616d 6574 6572 5f77  !set_parameter_w
+00001930: 6964 6765 745f 656e 6162 6c65 5f73 7461  idget_enable_sta
+00001940: 7465 da17 7374 6172 745f 7374 6f70 5f62  te..start_stop_b
+00001950: 7574 746f 6e5f 7374 6174 6572 1300 0000  utton_stater....
+00001960: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+00001970: 6600 0000 c900 0000 7304 0000 0000 010c  f.......s.......
+00001980: 017a 2853 7769 7463 6869 6e67 5370 6563  .z(SwitchingSpec
+00001990: 5363 7265 656e 2e65 6e74 6572 5f67 7569  Screen.enter_gui
+000019a0: 5f73 7461 7465 5f77 6169 7463 0100 0000  _state_waitc....
+000019b0: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+000019c0: 4300 0000 732c 0000 007c 006a 0064 0164  C...s,...|.j.d.d
+000019d0: 028d 0101 007c 006a 0164 017c 006a 02a0  .....|.j.d.|.j..
+000019e0: 03a1 0064 038d 0201 007c 00a0 04a1 0001  ...d.....|......
+000019f0: 0064 0053 0029 044e 4672 8f00 0000 a902  .d.S.).NFr......
+00001a00: 7291 0000 00da 0a73 746f 705f 7374 6174  r......stop_stat
+00001a10: 6529 0572 9200 0000 7293 0000 0072 0400  e).r....r....r..
+00001a20: 0000 727f 0000 0072 5100 0000 7213 0000  ..r....rQ...r...
+00001a30: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+00001a40: 7269 0000 00cd 0000 0073 0600 0000 0001  ri.......s......
+00001a50: 0c01 1401 7a2a 5377 6974 6368 696e 6753  ....z*SwitchingS
+00001a60: 7065 6353 6372 6565 6e2e 656e 7465 725f  pecScreen.enter_
+00001a70: 6775 695f 7374 6174 655f 6163 7469 7665  gui_state_active
+00001a80: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001a90: 0004 0000 0043 0000 0073 2400 0000 7c00  .....C...s$...|.
+00001aa0: 6a00 6401 6402 8d01 0100 7c00 6a01 6403  j.d.d.....|.j.d.
+00001ab0: 7c00 6a02 a003 a100 6404 8d02 0100 6400  |.j.....d.....d.
+00001ac0: 5300 2905 4e54 728f 0000 0046 7294 0000  S.).NTr....Fr...
+00001ad0: 0029 0472 9200 0000 7293 0000 0072 0400  .).r....r....r..
+00001ae0: 0000 727f 0000 0072 1300 0000 720d 0000  ..r....r....r...
+00001af0: 0072 0d00 0000 720e 0000 0072 5200 0000  .r....r....rR...
+00001b00: d200 0000 7304 0000 0000 010c 017a 2853  ....s........z(S
+00001b10: 7769 7463 6869 6e67 5370 6563 5363 7265  witchingSpecScre
+00001b20: 656e 2e65 6e74 6572 5f67 7569 5f73 7461  en.enter_gui_sta
+00001b30: 7465 5f69 646c 6554 728f 0000 0063 0200  te_idleTr....c..
+00001b40: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00001b50: 0000 4300 0000 7340 0000 007c 006a 00a0  ..C...s@...|.j..
+00001b60: 017c 01a1 0101 007c 006a 02a0 017c 01a1  .|.....|.j...|..
+00001b70: 0101 007c 006a 03a0 017c 01a1 0101 007c  ...|.j...|.....|
+00001b80: 006a 04a0 017c 01a1 0101 007c 006a 05a0  .j...|.....|.j..
+00001b90: 017c 01a1 0101 0064 0053 0072 1000 0000  .|.....d.S.r....
+00001ba0: 2906 7222 0000 00da 0a73 6574 456e 6162  ).r".....setEnab
+00001bb0: 6c65 6472 2c00 0000 722d 0000 0072 2f00  ledr,...r-...r/.
+00001bc0: 0000 7235 0000 0029 0272 1400 0000 7290  ..r5...).r....r.
+00001bd0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00001be0: 0000 7292 0000 00d6 0000 0073 0a00 0000  ..r........s....
+00001bf0: 0001 0c01 0c01 0c01 0c01 7a35 5377 6974  ..........z5Swit
+00001c00: 6368 696e 6753 7065 6353 6372 6565 6e2e  chingSpecScreen.
+00001c10: 7365 745f 7061 7261 6d65 7465 725f 7769  set_parameter_wi
+00001c20: 6467 6574 5f65 6e61 626c 655f 7374 6174  dget_enable_stat
+00001c30: 6546 7294 0000 0063 0300 0000 0000 0000  eFr....c........
+00001c40: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
+00001c50: 7342 0000 007c 0172 1e7c 006a 00a0 0164  sB...|.r.|.j...d
+00001c60: 01a1 0101 007c 006a 00a0 0264 02a1 0101  .....|.j...d....
+00001c70: 006e 207c 006a 00a0 0164 03a1 0101 007c  .n |.j...d.....|
+00001c80: 006a 00a0 027c 0272 3864 046e 0264 05a1  .j...|.r8d.n.d..
+00001c90: 0101 0064 0053 0029 064e 467a 0757 6169  ...d.S.).NFz.Wai
+00001ca0: 742e 2e2e 545a 0453 746f 7072 1800 0000  t...TZ.Stopr....
+00001cb0: 2903 723b 0000 0072 9600 0000 da07 7365  ).r;...r......se
+00001cc0: 7454 6578 7429 0372 1400 0000 7291 0000  tText).r....r...
+00001cd0: 0072 9500 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00001ce0: 720e 0000 0072 9300 0000 dd00 0000 730a  r....r........s.
+00001cf0: 0000 0000 0104 010c 010e 020c 017a 2b53  .............z+S
+00001d00: 7769 7463 6869 6e67 5370 6563 5363 7265  witchingSpecScre
+00001d10: 656e 2e73 7461 7274 5f73 746f 705f 6275  en.start_stop_bu
+00001d20: 7474 6f6e 5f73 7461 7465 6301 0000 0000  tton_statec.....
+00001d30: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00001d40: 0000 0073 1400 0000 7c00 a000 a100 0100  ...s....|.......
+00001d50: 7c00 a001 a100 0100 6400 5300 7210 0000  |.......d.S.r...
+00001d60: 0029 02da 0b75 7064 6174 655f 706c 6f74  .)...update_plot
+00001d70: da0d 7570 6461 7465 5f72 6573 756c 7472  ..update_resultr
+00001d80: 1300 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
+00001d90: 0000 0072 6c00 0000 e500 0000 7304 0000  ...rl.......s...
+00001da0: 0000 0108 017a 2153 7769 7463 6869 6e67  .....z!Switching
+00001db0: 5370 6563 5363 7265 656e 2e73 686f 775f  SpecScreen.show_
+00001dc0: 6e65 775f 6461 7461 6301 0000 0000 0000  new_datac.......
+00001dd0: 0000 0000 0004 0000 0004 0000 0043 0000  .............C..
+00001de0: 0073 6400 0000 7c00 6a00 6a01 6a02 6a03  .sd...|.j.j.j.j.
+00001df0: 6401 1b00 7d01 7c00 6a00 6a01 6a04 6a03  d...}.|.j.j.j.j.
+00001e00: 7c01 1800 7d02 7c00 6a00 6a01 6a04 6a03  |...}.|.j.j.j.j.
+00001e10: 7c01 1700 7d03 7c00 6a05 a006 a100 0100  |...}.|.j.......
+00001e20: 7c00 6a05 a007 7c02 7c03 a102 0100 7c00  |.j...|.|.....|.
+00001e30: 6a08 a006 a100 0100 7c00 6a08 a007 7c02  j.......|.j...|.
+00001e40: 7c03 a102 0100 6400 5300 2902 4e67 0000  |.....d.S.).Ng..
+00001e50: 0000 0000 0040 2909 7204 0000 0072 0500  .....@).r....r..
+00001e60: 0000 7256 0000 0072 8900 0000 7257 0000  ..rV...r....rW..
+00001e70: 0072 4800 0000 727e 0000 00da 0b73 6574  .rH...r~.....set
+00001e80: 5f72 616e 6765 5f78 7249 0000 0029 0472  _range_xrI...).r
+00001e90: 1400 0000 5a0a 6861 6c66 5f72 616e 6765  ....Z.half_range
+00001ea0: 5a05 6d69 6e5f 765a 056d 6178 5f76 720d  Z.min_vZ.max_vr.
+00001eb0: 0000 0072 0d00 0000 720e 0000 0072 6e00  ...r....r....rn.
+00001ec0: 0000 e900 0000 730e 0000 0000 0110 0110  ......s.........
+00001ed0: 0110 010a 010e 010a 017a 2453 7769 7463  .........z$Switc
+00001ee0: 6869 6e67 5370 6563 5363 7265 656e 2e73  hingSpecScreen.s
+00001ef0: 6574 5f64 6174 615f 696e 7661 6c69 6463  et_data_invalidc
+00001f00: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001f10: 0200 0000 4300 0000 730e 0000 007c 006a  ....C...s....|.j
+00001f20: 00a0 01a1 007d 0164 0053 0072 1000 0000  .....}.d.S.r....
+00001f30: 2902 7204 0000 00da 0a67 6574 5f72 6573  ).r......get_res
+00001f40: 756c 7429 0272 1400 0000 da03 7265 7372  ult).r......resr
+00001f50: 0d00 0000 720d 0000 0072 0e00 0000 7299  ....r....r....r.
+00001f60: 0000 00f2 0000 0073 0200 0000 0001 7a21  .......s......z!
+00001f70: 5377 6974 6368 696e 6753 7065 6353 6372  SwitchingSpecScr
+00001f80: 6565 6e2e 7570 6461 7465 5f72 6573 756c  een.update_resul
+00001f90: 7463 0100 0000 0000 0000 0000 0000 0200  tc..............
+00001fa0: 0000 0500 0000 4300 0000 73ba 0000 007c  ......C...s....|
+00001fb0: 006a 00a0 01a1 007d 017c 006a 02a0 0374  .j.....}.|.j...t
+00001fc0: 046a 056a 066a 076a 087c 016a 09a1 0201  .j.j.j.j.|.j....
+00001fd0: 007c 006a 0aa0 0374 046a 056a 066a 076a  .|.j...t.j.j.j.j
+00001fe0: 087c 016a 09a1 0201 007c 006a 02a0 0374  .|.j.....|.j...t
+00001ff0: 046a 056a 066a 076a 0b7c 016a 0ca1 0201  .j.j.j.j.|.j....
+00002000: 007c 006a 026a 0d7c 016a 0e7c 016a 0f64  .|.j.j.|.j.|.j.d
+00002010: 0164 028d 0301 007c 006a 0a6a 0d7c 016a  .d.....|.j.j.|.j
+00002020: 0e7c 016a 1064 0164 028d 0301 007c 006a  .|.j.d.d.....|.j
+00002030: 006a 116a 126a 1372 b67c 006a 026a 0d7c  .j.j.j.r.|.j.j.|
+00002040: 016a 0e7c 016a 1464 0364 028d 0301 007c  .j.|.j.d.d.....|
+00002050: 006a 0a6a 0d7c 016a 0e7c 016a 1564 0364  .j.j.|.j.|.j.d.d
+00002060: 028d 0301 0064 0053 0029 044e 7201 0000  .....d.S.).Nr...
+00002070: 0029 03da 0178 da01 79da 0b6c 6179 6572  .)...x..y..layer
+00002080: 5f69 6e64 6578 7207 0000 0029 1672 0400  _indexr....).r..
+00002090: 0000 729b 0000 0072 4800 0000 727c 0000  ..r....rH...r|..
+000020a0: 0072 1c00 0000 721d 0000 0072 4700 0000  .r....r....rG...
+000020b0: 7279 0000 0072 7a00 0000 da0c 6f75 7470  ry...rz.....outp
+000020c0: 7574 735f 756e 6974 7249 0000 0072 7d00  uts_unitrI...r}.
+000020d0: 0000 da0f 616d 706c 6974 7564 6573 5f75  ....amplitudes_u
+000020e0: 6e69 74da 0970 6c6f 745f 6461 7461 da07  nit..plot_data..
+000020f0: 6f75 7470 7574 73da 0e61 6d70 6c69 7475  outputs..amplitu
+00002100: 6465 735f 6f66 66da 0a70 6861 7365 735f  des_off..phases_
+00002110: 6f66 6672 0500 0000 725f 0000 0072 8900  offr....r_...r..
+00002120: 0000 da0d 616d 706c 6974 7564 6573 5f6f  ....amplitudes_o
+00002130: 6eda 0970 6861 7365 735f 6f6e 2902 7214  n..phases_on).r.
+00002140: 0000 00da 0c63 7572 7265 6e74 5f64 6174  .....current_dat
+00002150: 6172 0d00 0000 720d 0000 0072 0e00 0000  ar....r....r....
+00002160: 7298 0000 00f8 0000 0073 1200 0000 0001  r........s......
+00002170: 0a01 1801 1801 1801 1601 1601 0c01 1601  ................
+00002180: 7a1f 5377 6974 6368 696e 6753 7065 6353  z.SwitchingSpecS
+00002190: 6372 6565 6e2e 7570 6461 7465 5f70 6c6f  creen.update_plo
+000021a0: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
+000021b0: 0000 0200 0000 4300 0000 7314 0000 007c  ......C...s....|
+000021c0: 00a0 00a1 0001 007c 00a0 01a1 0001 0064  .......|.......d
+000021d0: 0053 0072 1000 0000 2902 7251 0000 0072  .S.r....).rQ...r
+000021e0: 9800 0000 7213 0000 0072 0d00 0000 720d  ....r....r....r.
+000021f0: 0000 0072 0e00 0000 7270 0000 0003 0100  ...r....rp......
+00002200: 0073 0400 0000 0001 0801 7a24 5377 6974  .s........z$Swit
+00002210: 6368 696e 6753 7065 6353 6372 6565 6e2e  chingSpecScreen.
+00002220: 6368 616e 6765 5f70 6c6f 745f 7669 6577  change_plot_view
+00002230: 2901 5429 0246 4629 1872 0900 0000 720a  ).T).FF).r....r.
+00002240: 0000 0072 0b00 0000 7212 0000 0072 0400  ...r....r....r..
+00002250: 0000 da13 5377 6974 6368 696e 6753 7065  ....SwitchingSpe
+00002260: 634d 6f64 756c 6572 5300 0000 7250 0000  cModulerS...rP..
+00002270: 0072 5100 0000 7262 0000 0072 6300 0000  .rQ...rb...rc...
+00002280: 7264 0000 0072 6600 0000 7269 0000 0072  rd...rf...ri...r
+00002290: 5200 0000 da04 626f 6f6c 7292 0000 0072  R.....boolr....r
+000022a0: 9300 0000 726c 0000 0072 6e00 0000 7299  ....rl...rn...r.
+000022b0: 0000 0072 9800 0000 7270 0000 00da 0d5f  ...r....rp....._
+000022c0: 5f63 6c61 7373 6365 6c6c 5f5f 720d 0000  _classcell__r...
+000022d0: 0072 0d00 0000 7215 0000 0072 0e00 0000  .r....r....r....
+000022e0: 720f 0000 001f 0000 0073 2200 0000 0801  r........s".....
+000022f0: 0c04 1065 0820 080f 0806 0803 0808 0804  ...e. ..........
+00002300: 0805 0804 1007 1208 0804 0809 0806 080b  ................
+00002310: 720f 0000 0029 2472 0c00 0000 728c 0000  r....)$r....r...
+00002320: 00da 0750 7953 6964 6536 7202 0000 00da  ...PySide6r.....
+00002330: 0e50 7953 6964 6536 2e51 7443 6f72 6572  .PySide6.QtCorer
+00002340: 0300 0000 da08 6e61 6e6f 7375 7266 721c  ......nanosurfr.
+00002350: 0000 00da 1573 7769 7463 6869 6e67 5f73  .....switching_s
+00002360: 7065 635f 6d6f 6475 6c65 7204 0000 0072  pec_moduler....r
+00002370: 0500 0000 721d 0000 00da 0a6e 7366 5f74  ....r......nsf_t
+00002380: 6162 6c65 73da 0d54 6162 6c65 456e 7472  ables..TableEntr
+00002390: 7949 4473 7206 0000 00da 0d4e 5346 436f  yIDsr......NSFCo
+000023a0: 6d62 6f45 6e74 7279 da0f 4f75 7470 7574  mboEntry..Output
+000023b0: 4368 616e 6e65 6c49 44da 0555 7365 7231  ChannelID..User1
+000023c0: da05 5573 6572 32da 0a54 6970 566f 6c74  ..User2..TipVolt
+000023d0: 6167 6572 1f00 0000 7226 0000 0072 2700  ager....r&...r'.
+000023e0: 0000 7228 0000 0072 2900 0000 7232 0000  ..r(...r)...r2..
+000023f0: 00da 056d 696c 6c69 7230 0000 00da 056d  ...millir0.....m
+00002400: 6963 726f da04 6e61 6e6f 722e 0000 0072  icro..nanor....r
+00002410: 2400 0000 7243 0000 0072 4400 0000 da0c  $...rC...rD.....
+00002420: 4d6f 6475 6c65 5363 7265 656e 720f 0000  ModuleScreenr...
+00002430: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00002440: 720e 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00002450: 0000 0073 1e00 0000 0405 0801 0c01 0c01  ...s............
+00002460: 0802 1002 1607 1001 1001 10fd 0407 0e01  ................
+00002470: 1801 2201 2202                           ..".".
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/module.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/module.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/module.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/module.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 12:11:49 2023 UTC, .py size: 7055 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 0543 3964 8f1b 0000  a........C9d....
+00000000: 610d 0d0a 0000 0000 5a4d 3964 8f1b 0000  a.......ZM9d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6403 6c04 6d05 5a05 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6402 6c06 5a07 6401 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000060: 6d0a 5a0a 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000070: 6507 6a0b 6a0c 6a0d 8303 5a0e 6402 5300  e.j.j.j...Z.d.S.
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/settings.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/settings.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/settings.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Dec 20 08:45:27 2022 UTC, .py size: 1949 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2776 a163 9d07 0000  a.......'v.c....
+00000000: 610d 0d0a 0000 0000 5a4d 3964 9d07 0000  a.......ZM9d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6402 6c04 5a04 6401 6402 6c05  Z.d.d.l.Z.d.d.l.
 00000050: 6d06 0200 0100 6d07 0200 0100 6d08 5a08  m.....m.....m.Z.
 00000060: 0100 6401 6402 6c09 6d06 0200 0100 6d07  ..d.d.l.m.....m.
 00000070: 0200 0100 6d0a 5a0a 0100 4700 6403 6404  ....m.Z...G.d.d.
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/worker_task.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/worker_task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/worker_task.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/worker_task.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 12:14:29 2023 UTC, .py size: 4533 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 a543 3964 b511 0000  a........C9d....
+00000000: 610d 0d0a 0000 0000 5a4d 3964 b511 0000  a.......ZM9d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6402 6c05 5a06 6401 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6401 6402 6c09 6d0a 0200 0100 6d0b  ..d.d.l.m.....m.
 00000070: 0200 0100 6d0c 0200 0100 6d0d 5a0e 0100  ....m.....m.Z...
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/gui.py` & `nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,16 +89,16 @@
         self.layout_left.addWidget(self.scival_num_steps)
         self.layout_left.addWidget(self.scival_time_delay)
         self.layout_left.addSpacing(10)
         self.layout_left.addWidget(self.check_do_revers_ramp)
         self.layout_left.addSpacing(10)
         self.layout_left.addWidget(self.check_show_on_data)
         self.layout_left.addStretch()
+        self.layout_left.addSpacerItem(nsf.frameworks.qt_app.app_gui.StdVSpacer())
         self.layout_left.addWidget(self.button_start_stop)
-        self.layout_left.addStretch()
 
         # mid layout - plots and result ---------------------------------------------------------
         self.chart_amp = nsf.gui.NSFChart(logmodex=False)
         self.chart_phase = nsf.gui.NSFChart(logmodex=False)
 
         self.layout_mid = QtWidgets.QVBoxLayout()
         self.layout_mid.addWidget(self.chart_amp)
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/module.py` & `nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/module.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/settings.py` & `nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/settings.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/worker_task.py` & `nanosurf-1.6.2/nanosurf/app/app_switching_spectrocopy/switching_spec_module/worker_task.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/.vscode/launch.json` & `nanosurf-1.6.2/nanosurf/app/app_template/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-311.pyc` & `nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 08:43:42 2023 UTC, .py size: 7820 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3e12 3964 8c1e 0000  a.......>.9d....
+00000000: 610d 0d0a 0000 0000 7104 5a64 8c1e 0000  a.......q.Zd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a04 6401 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 6d07 5a07 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000060: 6504 6a08 6a09 6a0a 8303 5a0b 6504 6a08  e.j.j.j...Z.e.j.
 00000070: a00c 6507 6a0d 6a0e 6407 a102 6504 6a08  ..e.j.j.d...e.j.
@@ -30,15 +30,15 @@
 000001d0: 6120 6e73 665f 7461 626c 6520 7769 6467  a nsf_table widg
 000001e0: 6574 7201 0000 00e9 0100 0000 e902 0000  etr.............
 000001f0: 004e 2907 da08 5f5f 6e61 6d65 5f5f da0a  .N)...__name__..
 00000200: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 00000210: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
 00000220: 5fda 0549 7465 6d73 da09 6c61 7374 5f64  _..Items..last_d
 00000230: 6174 61da 0a6d 6561 6e5f 7661 6c75 65a9  ata..mean_value.
-00000240: 0072 0f00 0000 720f 0000 00fa 4663 3a5c  .r....r.....Fc:\
+00000240: 0072 0f00 0000 720f 0000 00fa 4643 3a5c  .r....r.....FC:\
 00000250: 4769 745c 7363 7269 7074 735f 7079 7468  Git\scripts_pyth
 00000260: 6f6e 5f6c 6962 5c6e 616e 6f73 7572 665c  on_lib\nanosurf\
 00000270: 6170 705c 6170 705f 7465 6d70 6c61 7465  app\app_template
 00000280: 5c64 656d 6f5f 6d6f 6475 6c65 5c67 7569  \demo_module\gui
 00000290: 2e70 7972 0500 0000 0a00 0000 7308 0000  .pyr........s...
 000002a0: 0008 0104 0104 0104 0172 0500 0000 7a08  .........r....z.
 000002b0: 5369 6e2d 506c 6f74 7a08 436f 732d 506c  Sin-Plotz.Cos-Pl
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-311.pyc` & `nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 08:39:14 2023 UTC, .py size: 5134 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3211 3964 0e14 0000  a.......2.9d....
+00000000: 610d 0d0a 0000 0000 7704 5a64 0e14 0000  a.......w.Zd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 0100 6401 6402 6c05 5a06 6401  m.Z...d.d.l.Z.d.
 00000050: 6404 6c07 6d08 5a08 6d09 5a09 0100 4700  d.l.m.Z.m.Z...G.
 00000060: 6405 6406 8400 6406 6506 6a0a 6a0b 6a0c  d.d...d.e.j.j.j.
 00000070: 8303 5a0d 6402 5300 2907 7a5d 2054 6865  ..Z.d.S.).z] The
@@ -37,15 +37,15 @@
 00000240: 02a0 03a1 007c 005f 0274 02a0 04a1 007c  .....|._.t.....|
 00000250: 005f 0564 0053 00a9 014e 2906 da05 7375  ._.d.S...N)...su
 00000260: 7065 72da 085f 5f69 6e69 745f 5f72 0300  per..__init__r..
 00000270: 0000 5a0c 4465 6d6f 5365 7474 696e 6773  ..Z.DemoSettings
 00000280: da0b 4465 6d6f 5265 7375 6c74 73da 0672  ..DemoResults..r
 00000290: 6573 756c 7429 03da 0473 656c 6672 0600  esult)...selfr..
 000002a0: 0000 da03 6775 69a9 01da 095f 5f63 6c61  ....gui....__cla
-000002b0: 7373 5f5f a900 fa49 633a 5c47 6974 5c73  ss__...Ic:\Git\s
+000002b0: 7373 5f5f a900 fa49 433a 5c47 6974 5c73  ss__...IC:\Git\s
 000002c0: 6372 6970 7473 5f70 7974 686f 6e5f 6c69  cripts_python_li
 000002d0: 625c 6e61 6e6f 7375 7266 5c61 7070 5c61  b\nanosurf\app\a
 000002e0: 7070 5f74 656d 706c 6174 655c 6465 6d6f  pp_template\demo
 000002f0: 5f6d 6f64 756c 655c 6d6f 6475 6c65 2e70  _module\module.p
 00000300: 7972 0900 0000 1500 0000 7308 0000 0000  yr........s.....
 00000310: 010e 0104 020a 017a 1344 656d 6f4d 6f64  .......z.DemoMod
 00000320: 756c 652e 5f5f 696e 6974 5f5f 6301 0000  ule.__init__c...
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-311.pyc` & `nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/settings.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 08:34:12 2023 UTC, .py size: 1160 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,103 +1,107 @@
-00000000: 610d 0d0a 0000 0000 0410 3964 8804 0000  a.........9d....
+00000000: 6f0d 0d0a 0000 0000 aebb 1a64 ba04 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
-00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
-00000040: 6403 6c03 5a03 6401 6403 6c04 6d05 0200  d.l.Z.d.d.l.m...
-00000050: 0100 6d06 0200 0100 6d07 5a07 0100 6401  ..m.....m.Z...d.
-00000060: 6403 6c08 6d05 0200 0100 6d06 0200 0100  d.l.m.....m.....
-00000070: 6d09 5a09 0100 6502 4700 6404 6405 8400  m.Z...e.G.d.d...
-00000080: 6405 6509 6a0a 8303 8301 5a0b 6502 4700  d.e.j.....Z.e.G.
-00000090: 6406 6407 8400 6407 8302 8301 5a0c 4700  d.d...d.....Z.G.
-000000a0: 6408 6409 8400 6409 6503 6a0d 8303 5a0e  d.d...d.e.j...Z.
-000000b0: 6403 5300 290a 7abc 2044 6566 696e 6573  d.S.).z. Defines
-000000c0: 2074 6865 2063 6f6e 6669 6775 7261 7469   the configurati
-000000d0: 6f6e 2076 616c 7565 7320 6f66 2074 6865  on values of the
-000000e0: 206d 6f64 756c 652e 0a20 2020 2056 616c   module..    Val
-000000f0: 7565 7320 696e 2074 6865 2050 726f 5374  ues in the ProSt
-00000100: 6f72 6520 6172 6520 7361 7665 6420 616e  ore are saved an
-00000110: 6420 6c6f 6164 6564 2064 7572 696e 6720  d loaded during 
-00000120: 6170 706c 6963 6174 696f 6e20 7374 6172  application star
-00000130: 7475 702f 7368 7574 646f 776e 2061 7574  tup/shutdown aut
-00000140: 6f6d 6174 6963 616c 6c79 0a43 6f70 7972  omatically.Copyr
-00000150: 6967 6874 204e 616e 6f73 7572 6620 4147  ight Nanosurf AG
-00000160: 2032 3032 310a 4c69 6365 6e73 6520 2d20   2021.License - 
-00000170: 4d49 540a e900 0000 0029 01da 0964 6174  MIT......)...dat
-00000180: 6163 6c61 7373 4e63 0000 0000 0000 0000  aclassNc........
-00000190: 0000 0000 0000 0000 0600 0000 4000 0000  ............@...
-000001a0: 7356 0000 0065 005a 0164 005a 0264 015a  sV...e.Z.d.Z.d.Z
-000001b0: 0365 04a0 0565 0664 0283 01a1 015a 0765  .e...e.d.....Z.e
-000001c0: 04a0 0565 08a0 0964 0364 04a1 02a1 015a  ...e...d.d.....Z
-000001d0: 0a65 04a0 0564 05a1 015a 0b65 04a0 0565  .e...d...Z.e...e
-000001e0: 0664 0683 01a1 015a 0c65 04a0 0565 0664  .d.....Z.e...e.d
-000001f0: 0683 01a1 015a 0d64 0753 0029 08da 0c44  .....Z.d.S.)...D
-00000200: 656d 6f53 6574 7469 6e67 737a 8520 7365  emoSettingsz. se
-00000210: 7474 696e 6773 2064 6566 696e 6564 2068  ttings defined h
-00000220: 6572 6520 6173 2050 726f 7056 616c 2061  ere as PropVal a
-00000230: 7265 2073 746f 7265 6420 7065 7273 6973  re stored persis
-00000240: 7465 6e74 6c79 2069 6e20 6120 696e 692d  tently in a ini-
-00000250: 6669 6c65 0a20 2020 2020 2020 2073 6574  file.        set
-00000260: 7469 6e67 7320 7769 7468 2061 2027 5f27  tings with a '_'
-00000270: 2061 7320 6669 7273 7420 6368 6172 2061   as first char a
-00000280: 7265 206e 6f74 2073 746f 7265 640a 2020  re not stored.  
-00000290: 2020 692c 0100 0067 9a99 9999 9999 b93f    i,...g.......?
-000002a0: da01 7346 7201 0000 004e 290e da08 5f5f  ..sFr....N)...__
-000002b0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-000002c0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-000002d0: da07 5f5f 646f 635f 5fda 0870 726f 705f  ..__doc__..prop_
-000002e0: 7661 6cda 0750 726f 7056 616c da03 696e  val..PropVal..in
-000002f0: 74da 0b72 6570 6574 6974 696f 6e73 da07  t..repetitions..
-00000300: 7363 695f 7661 6cda 0653 6369 5661 6cda  sci_val..SciVal.
-00000310: 1374 696d 655f 7065 725f 7265 7065 7469  .time_per_repeti
-00000320: 7469 6f6e da0a 7365 6e64 5f74 6963 6b73  tion..send_ticks
-00000330: da0c 706c 6f74 5f66 756e 635f 6964 5a12  ..plot_func_idZ.
-00000340: 7468 6973 5f69 735f 6e6f 745f 7374 6f72  this_is_not_stor
-00000350: 6564 a900 7212 0000 0072 1200 0000 fa4b  ed..r....r.....K
-00000360: 633a 5c47 6974 5c73 6372 6970 7473 5f70  c:\Git\scripts_p
-00000370: 7974 686f 6e5f 6c69 625c 6e61 6e6f 7375  ython_lib\nanosu
-00000380: 7266 5c61 7070 5c61 7070 5f74 656d 706c  rf\app\app_templ
-00000390: 6174 655c 6465 6d6f 5f6d 6f64 756c 655c  ate\demo_module\
-000003a0: 7365 7474 696e 6773 2e70 7972 0300 0000  settings.pyr....
-000003b0: 0c00 0000 730c 0000 0008 0204 030e 0112  ....s...........
-000003c0: 010a 010e 0172 0300 0000 6300 0000 0000  .....r....c.....
-000003d0: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-000003e0: 0000 0073 1c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-000003f0: 6401 5a03 6402 5a04 6403 5a05 6403 5a06  d.Z.d.Z.d.Z.d.Z.
-00000400: 6404 5300 2905 da0b 4465 6d6f 5265 7375  d.S.)...DemoResu
-00000410: 6c74 737a 5720 5468 6973 2063 6c61 7373  ltszW This class
-00000420: 2073 6176 6573 2074 6865 2077 6f72 6b65   saves the worke
-00000430: 7220 7461 736b 2072 6573 756c 7420 2865  r task result (e
-00000440: 2e67 2062 6520 7265 6164 2062 7920 6775  .g be read by gu
-00000450: 6920 656c 656d 656e 7473 206f 7220 7361  i elements or sa
-00000460: 7665 6420 746f 2066 696c 6520 7201 0000  ved to file r...
-00000470: 0067 0000 0000 0000 0000 4e29 0772 0500  .g........N).r..
-00000480: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
-00000490: 00da 156e 756d 6265 725f 6f66 5f64 6174  ...number_of_dat
-000004a0: 615f 706f 696e 7473 da09 6c61 7374 5f64  a_points..last_d
-000004b0: 6174 61da 0a6d 6561 6e5f 7661 6c75 6572  ata..mean_valuer
-000004c0: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-000004d0: 0000 0072 1400 0000 1700 0000 7308 0000  ...r........s...
-000004e0: 0008 0204 0104 0104 0172 1400 0000 6300  .........r....c.
-000004f0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00000500: 0000 0040 0000 0073 1400 0000 6500 5a01  ...@...s....e.Z.
-00000510: 6400 5a02 6401 5a03 6402 5a04 6403 5300  d.Z.d.Z.d.Z.d.S.
-00000520: 2904 da0b 506c 6f74 5374 796c 6549 4429  )...PlotStyleID)
-00000530: 0172 0100 0000 2901 e901 0000 004e 2905  .r....)......N).
-00000540: 7205 0000 0072 0600 0000 7207 0000 005a  r....r....r....Z
-00000550: 0750 6c6f 7453 696e 5a07 506c 6f74 436f  .PlotSinZ.PlotCo
-00000560: 7372 1200 0000 7212 0000 0072 1200 0000  sr....r....r....
-00000570: 7213 0000 0072 1800 0000 1f00 0000 7304  r....r........s.
-00000580: 0000 0008 0104 0172 1800 0000 290f 7208  .......r....).r.
-00000590: 0000 00da 0b64 6174 6163 6c61 7373 6573  .....dataclasses
-000005a0: 7202 0000 00da 0465 6e75 6dda 1e6e 616e  r......enum..nan
-000005b0: 6f73 7572 662e 6c69 622e 6461 7461 7479  osurf.lib.dataty
-000005c0: 7065 732e 7363 695f 7661 6cda 036c 6962  pes.sci_val..lib
-000005d0: da09 6461 7461 7479 7065 7372 0d00 0000  ..datatypesr....
-000005e0: da1f 6e61 6e6f 7375 7266 2e6c 6962 2e64  ..nanosurf.lib.d
-000005f0: 6174 6174 7970 6573 2e70 726f 705f 7661  atatypes.prop_va
-00000600: 6c72 0900 0000 da09 5072 6f70 5374 6f72  lr......PropStor
-00000610: 6572 0300 0000 7214 0000 00da 0749 6e74  er....r......Int
-00000620: 456e 756d 7218 0000 0072 1200 0000 7212  Enumr....r....r.
-00000630: 0000 0072 1200 0000 7213 0000 00da 083c  ...r....r......<
-00000640: 6d6f 6475 6c65 3e01 0000 0073 1200 0000  module>....s....
-00000650: 0406 0c01 0801 1801 1802 0201 140a 0201  ................
-00000660: 1007                                     ..
+00000020: 0005 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
+00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
+00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
+00000050: 6d05 5a05 0100 6401 6402 6c06 5a07 0900  m.Z...d.d.l.Z...
+00000060: 4700 6404 6405 8400 6405 6501 6a08 8303  G.d.d...d.e.j...
+00000070: 5a09 6505 4700 6406 6407 8400 6407 6507  Z.e.G.d.d...d.e.
+00000080: 6a0a 8303 8301 5a0b 6505 4700 6408 6409  j.....Z.e.G.d.d.
+00000090: 8400 6409 8302 8301 5a0c 6402 5300 290a  ..d.....Z.d.S.).
+000000a0: 7abc 2044 6566 696e 6573 2074 6865 2063  z. Defines the c
+000000b0: 6f6e 6669 6775 7261 7469 6f6e 2076 616c  onfiguration val
+000000c0: 7565 7320 6f66 2074 6865 206d 6f64 756c  ues of the modul
+000000d0: 652e 0a20 2020 2056 616c 7565 7320 696e  e..    Values in
+000000e0: 2074 6865 2050 726f 5374 6f72 6520 6172   the ProStore ar
+000000f0: 6520 7361 7665 6420 616e 6420 6c6f 6164  e saved and load
+00000100: 6564 2064 7572 696e 6720 6170 706c 6963  ed during applic
+00000110: 6174 696f 6e20 7374 6172 7475 702f 7368  ation startup/sh
+00000120: 7574 646f 776e 2061 7574 6f6d 6174 6963  utdown automatic
+00000130: 616c 6c79 0a43 6f70 7972 6967 6874 204e  ally.Copyright N
+00000140: 616e 6f73 7572 6620 4147 2032 3032 310a  anosurf AG 2021.
+00000150: 4c69 6365 6e73 6520 2d20 4d49 540a e900  License - MIT...
+00000160: 0000 004e 2901 da09 6461 7461 636c 6173  ...N)...dataclas
+00000170: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
+00000180: 0000 0100 0000 4000 0000 7314 0000 0065  ......@...s....e
+00000190: 005a 0164 005a 0264 015a 0364 025a 0464  .Z.d.Z.d.Z.d.Z.d
+000001a0: 0353 0029 04da 104d 6f6e 6974 6f72 4368  .S.)...MonitorCh
+000001b0: 616e 6e65 6c49 4429 0172 0100 0000 2901  annelID).r....).
+000001c0: e901 0000 004e 2905 da08 5f5f 6e61 6d65  .....N)...__name
+000001d0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+000001e0: 5f5f 7175 616c 6e61 6d65 5f5f 5a0a 5573  __qualname__Z.Us
+000001f0: 6572 3149 6e70 7574 da0a 4465 666c 6563  er1Input..Deflec
+00000200: 7469 6f6e a900 7209 0000 0072 0900 0000  tion..r....r....
+00000210: fa3f 433a 5c47 6974 5c73 6372 6970 7473  .?C:\Git\scripts
+00000220: 5f70 7974 686f 6e5f 6c69 625c 6e61 6e6f  _python_lib\nano
+00000230: 7375 7266 5c61 7070 5c67 7569 5f74 656d  surf\app\gui_tem
+00000240: 706c 6174 655c 7365 7474 696e 6773 2e70  plate\settings.p
+00000250: 7972 0300 0000 0e00 0000 7306 0000 0008  yr........s.....
+00000260: 0004 0108 0172 0300 0000 6300 0000 0000  .....r....c.....
+00000270: 0000 0000 0000 0000 0000 0007 0000 0040  ...............@
+00000280: 0000 0073 5a00 0000 6500 5a01 6400 5a02  ...sZ...e.Z.d.Z.
+00000290: 6401 5a03 6504 a005 6506 6402 8301 a101  d.Z.e...e.d.....
+000002a0: 5a07 6504 a005 6504 a008 6403 6404 a102  Z.e...e...d.d...
+000002b0: a101 5a09 6504 a005 6506 650a 6a0b 8301  ..Z.e...e.e.j...
+000002c0: a101 5a0c 6504 a005 650d a00e 650f a010  ..Z.e...e...e...
+000002d0: 6405 a101 a101 6406 1b00 a101 5a11 6407  d.....d.....Z.d.
+000002e0: 5300 2908 da08 5365 7474 696e 6773 7aad  S.)...Settingsz.
+000002f0: 2073 6574 7469 6e67 7320 6465 6669 6e65   settings define
+00000300: 6420 6865 7265 2061 7320 5072 6f70 5661  d here as PropVa
+00000310: 6c20 6172 6520 7374 6f72 6564 2070 6572  l are stored per
+00000320: 7369 7374 656e 746c 7920 696e 2061 2069  sistently in a i
+00000330: 6e69 2d66 696c 6520 0a20 2020 2020 2020  ni-file .       
+00000340: 2043 6f75 6c64 2062 6520 636f 6e6e 6563   Could be connec
+00000350: 7465 6420 616c 736f 2074 6f20 4755 4920  ted also to GUI 
+00000360: 656c 656d 656e 7473 2028 652e 672e 3a20  elements (e.g.: 
+00000370: 6c6f 6f6b 2069 6e74 6f20 6269 6e64 5f67  look into bind_g
+00000380: 7569 5f65 6c65 6d65 6e74 7328 2920 696e  ui_elements() in
+00000390: 2067 7569 2e70 7929 0a20 2020 2069 2c01   gui.py).    i,.
+000003a0: 0000 679a 9999 9999 99b9 3fda 0173 5a0b  ..g.......?..sZ.
+000003b0: 5573 6572 5072 6f66 696c 65da 0744 6573  UserProfile..Des
+000003c0: 6b74 6f70 4e29 1272 0500 0000 7206 0000  ktopN).r....r...
+000003d0: 0072 0700 0000 da07 5f5f 646f 635f 5fda  .r......__doc__.
+000003e0: 036e 7366 da07 5072 6f70 5661 6cda 0369  .nsf..PropVal..i
+000003f0: 6e74 da0b 7265 7065 7469 7469 6f6e 73da  nt..repetitions.
+00000400: 0653 6369 5661 6cda 1374 696d 655f 7065  .SciVal..time_pe
+00000410: 725f 7265 7065 7469 7469 6f6e 7203 0000  r_repetitionr...
+00000420: 0072 0800 0000 da0a 6368 616e 6e65 6c5f  .r......channel_
+00000430: 6964 da07 7061 7468 6c69 62da 0450 6174  id..pathlib..Pat
+00000440: 68da 026f 73da 0667 6574 656e 765a 0973  h..os..getenvZ.s
+00000450: 6176 655f 7061 7468 7209 0000 0072 0900  ave_pathr....r..
+00000460: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00000470: 0012 0000 0073 0c00 0000 0800 0402 0e03  .....s..........
+00000480: 1201 1001 1e01 720b 0000 0063 0000 0000  ......r....c....
+00000490: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+000004a0: 4000 0000 7336 0000 0065 005a 0164 005a  @...s6...e.Z.d.Z
+000004b0: 0255 0064 015a 0365 04a0 05a1 005a 0665  .U.d.Z.e.....Z.e
+000004c0: 04a0 07a1 005a 0865 04a0 07a1 005a 0964  .....Z.e.....Z.d
+000004d0: 025a 0a65 0b65 0c64 033c 0064 0453 0029  .Z.e.e.d.<.d.S.)
+000004e0: 05da 0d4d 6f64 756c 6552 6573 756c 7473  ...ModuleResults
+000004f0: 7a6a 2054 6869 7320 636c 6173 7320 7361  zj This class sa
+00000500: 7665 7320 7468 6520 776f 726b 6572 206d  ves the worker m
+00000510: 6f64 756c 6520 7265 7375 6c74 2028 652e  odule result (e.
+00000520: 672e 3a20 6265 2072 6561 6420 6279 2067  g.: be read by g
+00000530: 7569 2065 6c65 6d65 6e74 7320 6c69 6b65  ui elements like
+00000540: 204e 5346 4368 6172 7420 6f72 2073 6176   NSFChart or sav
+00000550: 6564 2074 6f20 6669 6c65 2920 e9ff ffff  ed to file) ....
+00000560: ffda 0a6c 6173 745f 696e 6465 784e 290d  ...last_indexN).
+00000570: 7205 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
+00000580: 0e00 0000 720f 0000 00da 0953 6369 5374  ....r......SciSt
+00000590: 7265 616d da0b 6461 7461 5f73 7472 6561  ream..data_strea
+000005a0: 6d72 1300 0000 da0a 6d65 616e 5f76 616c  mr......mean_val
+000005b0: 7565 da0a 6c61 7374 5f76 616c 7565 721c  ue..last_valuer.
+000005c0: 0000 0072 1100 0000 da0f 5f5f 616e 6e6f  ...r......__anno
+000005d0: 7461 7469 6f6e 735f 5f72 0900 0000 7209  tations__r....r.
+000005e0: 0000 0072 0900 0000 720a 0000 0072 1a00  ...r....r....r..
+000005f0: 0000 1c00 0000 730c 0000 000a 0004 0208  ......s.........
+00000600: 0108 0108 0110 0172 1a00 0000 290d 720e  .......r....).r.
+00000610: 0000 00da 0465 6e75 6d72 1600 0000 7218  .....enumr....r.
+00000620: 0000 00da 0b64 6174 6163 6c61 7373 6573  .....dataclasses
+00000630: 7202 0000 00da 086e 616e 6f73 7572 6672  r......nanosurfr
+00000640: 0f00 0000 da07 496e 7445 6e75 6d72 0300  ......IntEnumr..
+00000650: 0000 da09 5072 6f70 5374 6f72 6572 0b00  ....PropStorer..
+00000660: 0000 721a 0000 0072 0900 0000 7209 0000  ..r....r....r...
+00000670: 0072 0900 0000 720a 0000 00da 083c 6d6f  .r....r......<mo
+00000680: 6475 6c65 3e01 0000 0073 1800 0000 0400  dule>....s......
+00000690: 0806 0801 0801 0c01 0801 0202 1201 0204  ................
+000006a0: 1401 0209 1401                           ......
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-311.pyc` & `nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 08:47:50 2023 UTC, .py size: 2617 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,161 +1,163 @@
-00000000: 610d 0d0a 0000 0000 3613 3964 390a 0000  a.......6.9d9...
+00000000: 610d 0d0a 0000 0000 d705 5a64 470a 0000  a.........ZdG...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
+00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6401 6404 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6402 6c08 5a09 6401 6405 6c0a 6d0b 5a0b  d.l.Z.d.d.l.m.Z.
-00000070: 0100 6504 4700 6406 6407 8400 6407 8302  ..e.G.d.d...d...
-00000080: 8301 5a0c 4700 6408 6409 8400 6409 6509  ..Z.G.d.d...d.e.
-00000090: 6a0d 6a0e 6a0f 6a10 8303 5a11 6402 5300  j.j.j.j...Z.d.S.
-000000a0: 290a 7a84 2054 6865 206c 6f6e 6720 6c61  ).z. The long la
-000000b0: 7374 696e 6720 776f 726b 6572 2074 6872  sting worker thr
-000000c0: 6561 6420 6173 2064 656d 6f20 2d20 6a75  ead as demo - ju
-000000d0: 7374 2077 6169 7420 736f 6d65 2074 696d  st wait some tim
-000000e0: 6520 616e 6420 6372 6561 7465 2064 6174  e and create dat
-000000f0: 6120 7065 7269 6f64 6963 616c 6c79 0a43  a periodically.C
-00000100: 6f70 7972 6967 6874 204e 616e 6f73 7572  opyright Nanosur
-00000110: 6620 4147 2032 3032 310a 4c69 6365 6e73  f AG 2021.Licens
-00000120: 6520 2d20 4d49 540a e900 0000 004e 2902  e - MIT......N).
-00000130: da09 6461 7461 636c 6173 73da 0566 6965  ..dataclass..fie
-00000140: 6c64 2901 da06 5369 676e 616c 2901 da08  ld)...Signal)...
-00000150: 7365 7474 696e 6773 6300 0000 0000 0000  settingsc.......
-00000160: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000170: 0073 3000 0000 6500 5a01 6400 5a02 5500  .s0...e.Z.d.Z.U.
-00000180: 6503 6504 6401 8d01 5a05 6504 6506 1900  e.e.d...Z.e.e...
-00000190: 6507 6402 3c00 6403 5a08 6509 6507 6404  e.d.<.d.Z.e.e.d.
-000001a0: 3c00 6405 5300 2906 da0c 4d79 576f 726b  <.d.S.)...MyWork
-000001b0: 6572 4461 7461 2901 da0f 6465 6661 756c  erData)...defaul
-000001c0: 745f 6661 6374 6f72 79da 0576 616c 7565  t_factory..value
-000001d0: e9ff ffff ffda 0a6c 6173 745f 696e 6465  .......last_inde
-000001e0: 784e 290a da08 5f5f 6e61 6d65 5f5f da0a  xN)...__name__..
-000001f0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000200: 616c 6e61 6d65 5f5f 7203 0000 00da 046c  alname__r......l
-00000210: 6973 7472 0800 0000 da05 666c 6f61 74da  istr......float.
-00000220: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
-00000230: 720a 0000 00da 0369 6e74 a900 7212 0000  r......int..r...
-00000240: 0072 1200 0000 fa4e 633a 5c47 6974 5c73  .r.....Nc:\Git\s
-00000250: 6372 6970 7473 5f70 7974 686f 6e5f 6c69  cripts_python_li
-00000260: 625c 6e61 6e6f 7375 7266 5c61 7070 5c61  b\nanosurf\app\a
-00000270: 7070 5f74 656d 706c 6174 655c 6465 6d6f  pp_template\demo
-00000280: 5f6d 6f64 756c 655c 776f 726b 6572 5f74  _module\worker_t
-00000290: 6173 6b2e 7079 7206 0000 000c 0000 0073  ask.pyr........s
-000002a0: 0400 0000 0a02 1601 7206 0000 0063 0000  ........r....c..
-000002b0: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-000002c0: 0000 0000 0000 7370 0000 0065 005a 0164  ......sp...e.Z.d
-000002d0: 005a 0264 015a 0365 0483 005a 0565 0483  .Z.d.Z.e...Z.e..
-000002e0: 005a 0664 025a 0764 035a 0864 045a 0964  .Z.d.Z.d.Z.d.Z.d
-000002f0: 055a 0a65 0b6a 0c6a 0d5a 0e65 0465 0f65  .Z.e.j.j.Z.e.e.e
-00000300: 1083 025a 1165 126a 136a 146a 1564 069c  ...Z.e.j.j.j.d..
-00000310: 0187 0066 0164 0764 0884 0c5a 1664 0964  ...f.d.d...Z.d.d
-00000320: 0a84 005a 1765 1864 0b9c 0164 0c64 0d84  ...Z.e.d...d.d..
-00000330: 045a 1987 0004 005a 1a53 0029 0eda 084d  .Z.....Z.S.)...M
-00000340: 7957 6f72 6b65 727a 5920 5468 6973 2063  yWorkerzY This c
-00000350: 6c61 7373 2069 6d70 6c65 6d65 6e74 7320  lass implements 
-00000360: 7468 6520 6c6f 6e67 206c 6173 7469 6e67  the long lasting
-00000370: 2061 6374 6976 6974 7920 696e 2074 6865   activity in the
-00000380: 2062 6163 6b67 726f 756e 6420 746f 206e   background to n
-00000390: 6f74 2066 7265 657a 6520 7468 6520 6775  ot freeze the gu
-000003a0: 6920 e90a 0000 0067 0000 0000 0000 0040  i .....g.......@
-000003b0: 5467 9a99 9999 9999 b93f 2901 da09 6d79  Tg.......?)...my
-000003c0: 5f6d 6f64 756c 6563 0200 0000 0000 0000  _modulec........
-000003d0: 0000 0000 0200 0000 0200 0000 0300 0000  ................
-000003e0: 731c 0000 007c 017c 005f 0074 0183 007c  s....|.|._.t...|
-000003f0: 005f 0274 0383 00a0 04a1 0001 0064 0053  ._.t.........d.S
-00000400: 00a9 014e 2905 da06 6d6f 6475 6c65 7206  ...N)...moduler.
-00000410: 0000 00da 0672 6573 756c 74da 0573 7570  .....result..sup
-00000420: 6572 da08 5f5f 696e 6974 5f5f 2902 da04  er..__init__)...
-00000430: 7365 6c66 7216 0000 00a9 01da 095f 5f63  selfr........__c
-00000440: 6c61 7373 5f5f 7212 0000 0072 1300 0000  lass__r....r....
-00000450: 721b 0000 0020 0000 0073 0600 0000 0001  r.... ...s......
-00000460: 0601 0801 7a11 4d79 576f 726b 6572 2e5f  ....z.MyWorker._
-00000470: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-00000480: 0000 0000 0100 0000 0600 0000 4300 0000  ............C...
-00000490: 7334 0100 0074 0083 007c 005f 0164 017c  s4...t...|._.d.|
-000004a0: 005f 027c 006a 027c 006a 036b 0090 0172  ._.|.j.|.j.k...r
-000004b0: 307c 00a0 04a1 0090 0173 307c 0004 006a  0|.......s0|...j
-000004c0: 0264 0237 0002 005f 027c 006a 0572 9464  .d.7..._.|.j.r.d
-000004d0: 037c 005f 067c 006a 067c 006a 076b 0072  .|._.|.j.|.j.k.r
-000004e0: a07c 00a0 04a1 0073 a07c 0004 006a 067c  .|.....s.|...j.|
-000004f0: 006a 0837 0002 005f 0674 09a0 0a7c 006a  .j.7..._.t...|.j
-00000500: 08a1 0101 007c 006a 0ba0 0ca1 0001 007c  .....|.j.......|
-00000510: 00a0 0d64 047c 006a 0664 059b 0464 069d  ...d.|.j.d...d..
-00000520: 03a1 0101 0071 406e 0c74 09a0 0a7c 006a  .....q@n.t...|.j
-00000530: 07a1 0101 007c 006a 0e6a 0f74 106a 116a  .....|.j.j.t.j.j
-00000540: 126b 0272 d47c 006a 016a 0fa0 1374 14a0  .k.r.|.j.j...t..
-00000550: 157c 006a 027c 006a 031b 0074 146a 1614  .|.j.|.j...t.j..
-00000560: 00a1 01a1 0101 006e 407c 006a 0e6a 0f74  .......n@|.j.j.t
-00000570: 106a 116a 176b 0290 0172 0a7c 006a 016a  .j.j.k...r.|.j.j
-00000580: 0fa0 1374 14a0 187c 006a 027c 006a 031b  ...t...|.j.|.j..
-00000590: 0074 146a 1614 00a1 01a1 0101 006e 0a7c  .t.j.........n.|
-000005a0: 00a0 1964 07a1 0101 007c 006a 0104 006a  ...d.....|.j...j
-000005b0: 1a64 0237 0002 005f 1a7c 006a 1ba0 0ca1  .d.7..._.|.j....
-000005c0: 0001 0071 0e64 0853 0029 097a 2f20 5468  ...q.d.S.).z/ Th
-000005d0: 6973 2069 7320 7468 6520 776f 726b 696e  is is the workin
-000005e0: 6720 6675 6e63 7469 6f6e 2066 6f72 2074  g function for t
-000005f0: 6865 206c 6f6e 6720 7461 736b 7201 0000  he long taskr...
-00000600: 00e9 0100 0000 6700 0000 0000 0000 007a  ......g........z
-00000610: 0654 6963 6b3a 207a 032e 3266 da01 737a  .Tick: z..2f..sz
-00000620: 1255 6e6b 6e6f 776e 2070 6c6f 7420 7374  .Unknown plot st
-00000630: 796c 654e 291c 7206 0000 0072 1900 0000  yleN).r....r....
-00000640: da05 636f 756e 74da 0e70 6172 5f72 6570  ..count..par_rep
-00000650: 6574 6974 696f 6eda 1769 735f 7374 6f70  etition..is_stop
-00000660: 5f72 6571 7565 7374 5f70 656e 6469 6e67  _request_pending
-00000670: da0e 7061 725f 7365 6e64 5f74 6963 6b73  ..par_send_ticks
-00000680: 5a09 7469 636b 5f74 696d 65da 1770 6172  Z.tick_time..par
-00000690: 5f74 696d 655f 7065 725f 7265 7065 7469  _time_per_repeti
-000006a0: 7469 6f6e da16 7061 725f 7469 6d65 5f62  tion..par_time_b
-000006b0: 6574 7765 656e 5f74 6963 6b73 da04 7469  etween_ticks..ti
-000006c0: 6d65 da05 736c 6565 70da 0873 6967 5f74  me..sleep..sig_t
-000006d0: 6963 6bda 0465 6d69 74da 1173 656e 645f  ick..emit..send_
-000006e0: 696e 666f 5f6d 6573 7361 6765 da10 7061  info_message..pa
-000006f0: 725f 706c 6f74 5f66 756e 635f 6964 7208  r_plot_func_idr.
-00000700: 0000 0072 0500 0000 da0b 506c 6f74 5374  ...r......PlotSt
-00000710: 796c 6549 44da 0750 6c6f 7453 696e da06  yleID..PlotSin..
-00000720: 6170 7065 6e64 da04 6d61 7468 da03 7369  append..math..si
-00000730: 6eda 0270 69da 0750 6c6f 7443 6f73 da03  n..pi..PlotCos..
-00000740: 636f 73da 1273 656e 645f 6572 726f 725f  cos..send_error_
-00000750: 6d65 7373 6167 6572 0a00 0000 da0c 7369  messager......si
-00000760: 675f 6e65 775f 6461 7461 a901 721c 0000  g_new_data..r...
-00000770: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-00000780: da07 646f 5f77 6f72 6b25 0000 0073 2600  ..do_work%...s&.
-00000790: 0000 0003 0802 0601 1801 0e02 0601 0601  ................
-000007a0: 1401 1001 0c01 0a01 1a02 0c02 1001 2401  ..............$.
-000007b0: 1201 2402 0a02 1001 7a10 4d79 576f 726b  ..$.....z.MyWork
-000007c0: 6572 2e64 6f5f 776f 726b 2901 da06 7265  er.do_work)...re
-000007d0: 7475 726e 6301 0000 0000 0000 0000 0000  turnc...........
-000007e0: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-000007f0: 0000 7c00 6a00 5300 7217 0000 0029 0172  ..|.j.S.r....).r
-00000800: 1900 0000 7237 0000 0072 1200 0000 7212  ....r7...r....r.
-00000810: 0000 0072 1300 0000 da0f 6765 745f 7461  ...r......get_ta
-00000820: 736b 5f72 6573 756c 7442 0000 0073 0200  sk_resultB...s..
-00000830: 0000 0001 7a18 4d79 576f 726b 6572 2e67  ....z.MyWorker.g
-00000840: 6574 5f74 6173 6b5f 7265 7375 6c74 291b  et_task_result).
-00000850: 720b 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00000860: 075f 5f64 6f63 5f5f 7204 0000 0072 2900  .__doc__r....r).
-00000870: 0000 7236 0000 0072 2200 0000 7225 0000  ..r6...r"...r%..
-00000880: 0072 2400 0000 7226 0000 0072 0500 0000  .r$...r&...r....
-00000890: 722d 0000 0072 2e00 0000 722c 0000 00da  r-...r....r,....
-000008a0: 0373 7472 7211 0000 005a 0c5f 7369 675f  .strr....Z._sig_
-000008b0: 6d65 7373 6167 65da 036e 7366 da0a 6672  message..nsf..fr
-000008c0: 616d 6577 6f72 6b73 da06 7174 5f61 7070  ameworks..qt_app
-000008d0: da0a 4d6f 6475 6c65 4261 7365 721b 0000  ..ModuleBaser...
-000008e0: 0072 3800 0000 7206 0000 0072 3a00 0000  .r8...r....r:...
-000008f0: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
-00000900: 1200 0000 7212 0000 0072 1d00 0000 7213  ....r....r....r.
-00000910: 0000 0072 1400 0000 1100 0000 7318 0000  ...r........s...
-00000920: 0008 0104 0206 0106 0304 0104 0104 0104  ................
-00000930: 0108 020a 0218 0508 1d72 1400 0000 2912  .........r....).
-00000940: 723b 0000 0072 2700 0000 7230 0000 00da  r;...r'...r0....
-00000950: 0b64 6174 6163 6c61 7373 6573 7202 0000  .dataclassesr...
-00000960: 0072 0300 0000 da0e 5079 5369 6465 362e  .r......PySide6.
-00000970: 5174 436f 7265 7204 0000 00da 086e 616e  QtCorer......nan
-00000980: 6f73 7572 6672 3d00 0000 da0b 6465 6d6f  osurfr=.....demo
-00000990: 5f6d 6f64 756c 6572 0500 0000 7206 0000  _moduler....r...
-000009a0: 0072 3e00 0000 723f 0000 00da 0a6e 7366  .r>...r?.....nsf
-000009b0: 5f74 6872 6561 64da 134e 5346 4261 636b  _thread..NSFBack
-000009c0: 6772 6f75 6e64 576f 726b 6572 7214 0000  groundWorkerr...
-000009d0: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
-000009e0: 7213 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000009f0: 0000 0073 1200 0000 0404 0801 0801 1001  ...s............
-00000a00: 0c01 0801 0c02 0201 1004                 ..........
+00000070: 0100 4700 6406 6407 8400 6407 8302 5a0c  ..G.d.d...d...Z.
+00000080: 4700 6408 6409 8400 6409 6509 6a0d 6a0e  G.d.d...d.e.j.j.
+00000090: 6a0f 6a10 8303 5a11 6402 5300 290a 7a84  j.j...Z.d.S.).z.
+000000a0: 2054 6865 206c 6f6e 6720 6c61 7374 696e   The long lastin
+000000b0: 6720 776f 726b 6572 2074 6872 6561 6420  g worker thread 
+000000c0: 6173 2064 656d 6f20 2d20 6a75 7374 2077  as demo - just w
+000000d0: 6169 7420 736f 6d65 2074 696d 6520 616e  ait some time an
+000000e0: 6420 6372 6561 7465 2064 6174 6120 7065  d create data pe
+000000f0: 7269 6f64 6963 616c 6c79 0a43 6f70 7972  riodically.Copyr
+00000100: 6967 6874 204e 616e 6f73 7572 6620 4147  ight Nanosurf AG
+00000110: 2032 3032 310a 4c69 6365 6e73 6520 2d20   2021.License - 
+00000120: 4d49 540a e900 0000 004e 2902 da09 6461  MIT......N)...da
+00000130: 7461 636c 6173 73da 0566 6965 6c64 2901  taclass..field).
+00000140: da06 5369 676e 616c 2901 da08 7365 7474  ..Signal)...sett
+00000150: 696e 6773 6300 0000 0000 0000 0000 0000  ingsc...........
+00000160: 0000 0000 0003 0000 0040 0000 0073 1a00  .........@...s..
+00000170: 0000 6500 5a01 6400 5a02 6401 6402 9c01  ..e.Z.d.Z.d.d...
+00000180: 6403 6404 8404 5a03 6401 5300 2905 da0c  d.d...Z.d.S.)...
+00000190: 4d79 576f 726b 6572 4461 7461 4ea9 01da  MyWorkerDataN...
+000001a0: 0672 6574 7572 6e63 0100 0000 0000 0000  .returnc........
+000001b0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+000001c0: 7310 0000 0067 007c 005f 0064 017c 005f  s....g.|._.d.|._
+000001d0: 0164 0053 0029 024e e9ff ffff ff29 02da  .d.S.).N.....)..
+000001e0: 0576 616c 7565 da0a 6c61 7374 5f69 6e64  .value..last_ind
+000001f0: 6578 a901 da04 7365 6c66 a900 720e 0000  ex....self..r...
+00000200: 00fa 4e43 3a5c 4769 745c 7363 7269 7074  ..NC:\Git\script
+00000210: 735f 7079 7468 6f6e 5f6c 6962 5c6e 616e  s_python_lib\nan
+00000220: 6f73 7572 665c 6170 705c 6170 705f 7465  osurf\app\app_te
+00000230: 6d70 6c61 7465 5c64 656d 6f5f 6d6f 6475  mplate\demo_modu
+00000240: 6c65 5c77 6f72 6b65 725f 7461 736b 2e70  le\worker_task.p
+00000250: 79da 085f 5f69 6e69 745f 5f0d 0000 0073  y..__init__....s
+00000260: 0400 0000 0001 0601 7a15 4d79 576f 726b  ........z.MyWork
+00000270: 6572 4461 7461 2e5f 5f69 6e69 745f 5f29  erData.__init__)
+00000280: 04da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000290: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000002a0: 616d 655f 5f72 1000 0000 720e 0000 0072  ame__r....r....r
+000002b0: 0e00 0000 720e 0000 0072 0f00 0000 7206  ....r....r....r.
+000002c0: 0000 000c 0000 0073 0200 0000 0801 7206  .......s......r.
+000002d0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000002e0: 0000 0000 0400 0000 0000 0000 7370 0000  ............sp..
+000002f0: 0065 005a 0164 005a 0264 015a 0365 0483  .e.Z.d.Z.d.Z.e..
+00000300: 005a 0565 0483 005a 0664 025a 0764 035a  .Z.e...Z.d.Z.d.Z
+00000310: 0864 045a 0964 055a 0a65 0b6a 0c6a 0d5a  .d.Z.d.Z.e.j.j.Z
+00000320: 0e65 0465 0f65 1083 025a 1165 126a 136a  .e.e.e...Z.e.j.j
+00000330: 146a 1564 069c 0187 0066 0164 0764 0884  .j.d.....f.d.d..
+00000340: 0c5a 1664 0964 0a84 005a 1765 1864 0b9c  .Z.d.d...Z.e.d..
+00000350: 0164 0c64 0d84 045a 1987 0004 005a 1a53  .d.d...Z.....Z.S
+00000360: 0029 0eda 084d 7957 6f72 6b65 727a 5920  .)...MyWorkerzY 
+00000370: 5468 6973 2063 6c61 7373 2069 6d70 6c65  This class imple
+00000380: 6d65 6e74 7320 7468 6520 6c6f 6e67 206c  ments the long l
+00000390: 6173 7469 6e67 2061 6374 6976 6974 7920  asting activity 
+000003a0: 696e 2074 6865 2062 6163 6b67 726f 756e  in the backgroun
+000003b0: 6420 746f 206e 6f74 2066 7265 657a 6520  d to not freeze 
+000003c0: 7468 6520 6775 6920 e90a 0000 0067 0000  the gui .....g..
+000003d0: 0000 0000 0040 5467 9a99 9999 9999 b93f  .....@Tg.......?
+000003e0: 2901 da09 6d79 5f6d 6f64 756c 6563 0200  )...my_modulec..
+000003f0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00000400: 0000 0300 0000 731c 0000 007c 017c 005f  ......s....|.|._
+00000410: 0074 0183 007c 005f 0274 0383 00a0 04a1  .t...|._.t......
+00000420: 0001 0064 0053 00a9 014e 2905 da06 6d6f  ...d.S...N)...mo
+00000430: 6475 6c65 7206 0000 00da 0672 6573 756c  duler......resul
+00000440: 74da 0573 7570 6572 7210 0000 0029 0272  t..superr....).r
+00000450: 0d00 0000 7216 0000 00a9 01da 095f 5f63  ....r........__c
+00000460: 6c61 7373 5f5f 720e 0000 0072 0f00 0000  lass__r....r....
+00000470: 7210 0000 0020 0000 0073 0600 0000 0001  r.... ...s......
+00000480: 0601 0801 7a11 4d79 576f 726b 6572 2e5f  ....z.MyWorker._
+00000490: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+000004a0: 0000 0000 0100 0000 0600 0000 4300 0000  ............C...
+000004b0: 7334 0100 0074 0083 007c 005f 0164 017c  s4...t...|._.d.|
+000004c0: 005f 027c 006a 027c 006a 036b 0090 0172  ._.|.j.|.j.k...r
+000004d0: 307c 00a0 04a1 0090 0173 307c 0004 006a  0|.......s0|...j
+000004e0: 0264 0237 0002 005f 027c 006a 0572 9464  .d.7..._.|.j.r.d
+000004f0: 037c 005f 067c 006a 067c 006a 076b 0072  .|._.|.j.|.j.k.r
+00000500: a07c 00a0 04a1 0073 a07c 0004 006a 067c  .|.....s.|...j.|
+00000510: 006a 0837 0002 005f 0674 09a0 0a7c 006a  .j.7..._.t...|.j
+00000520: 08a1 0101 007c 006a 0ba0 0ca1 0001 007c  .....|.j.......|
+00000530: 00a0 0d64 047c 006a 0664 059b 0464 069d  ...d.|.j.d...d..
+00000540: 03a1 0101 0071 406e 0c74 09a0 0a7c 006a  .....q@n.t...|.j
+00000550: 07a1 0101 007c 006a 0e6a 0f74 106a 116a  .....|.j.j.t.j.j
+00000560: 126b 0272 d47c 006a 016a 0fa0 1374 14a0  .k.r.|.j.j...t..
+00000570: 157c 006a 027c 006a 031b 0074 146a 1614  .|.j.|.j...t.j..
+00000580: 00a1 01a1 0101 006e 407c 006a 0e6a 0f74  .......n@|.j.j.t
+00000590: 106a 116a 176b 0290 0172 0a7c 006a 016a  .j.j.k...r.|.j.j
+000005a0: 0fa0 1374 14a0 187c 006a 027c 006a 031b  ...t...|.j.|.j..
+000005b0: 0074 146a 1614 00a1 01a1 0101 006e 0a7c  .t.j.........n.|
+000005c0: 00a0 1964 07a1 0101 007c 006a 0104 006a  ...d.....|.j...j
+000005d0: 1a64 0237 0002 005f 1a7c 006a 1ba0 0ca1  .d.7..._.|.j....
+000005e0: 0001 0071 0e64 0853 0029 097a 2f20 5468  ...q.d.S.).z/ Th
+000005f0: 6973 2069 7320 7468 6520 776f 726b 696e  is is the workin
+00000600: 6720 6675 6e63 7469 6f6e 2066 6f72 2074  g function for t
+00000610: 6865 206c 6f6e 6720 7461 736b 7201 0000  he long taskr...
+00000620: 00e9 0100 0000 6700 0000 0000 0000 007a  ......g........z
+00000630: 0654 6963 6b3a 207a 032e 3266 da01 737a  .Tick: z..2f..sz
+00000640: 1255 6e6b 6e6f 776e 2070 6c6f 7420 7374  .Unknown plot st
+00000650: 796c 654e 291c 7206 0000 0072 1900 0000  yleN).r....r....
+00000660: da05 636f 756e 74da 0e70 6172 5f72 6570  ..count..par_rep
+00000670: 6574 6974 696f 6eda 1769 735f 7374 6f70  etition..is_stop
+00000680: 5f72 6571 7565 7374 5f70 656e 6469 6e67  _request_pending
+00000690: da0e 7061 725f 7365 6e64 5f74 6963 6b73  ..par_send_ticks
+000006a0: 5a09 7469 636b 5f74 696d 65da 1770 6172  Z.tick_time..par
+000006b0: 5f74 696d 655f 7065 725f 7265 7065 7469  _time_per_repeti
+000006c0: 7469 6f6e da16 7061 725f 7469 6d65 5f62  tion..par_time_b
+000006d0: 6574 7765 656e 5f74 6963 6b73 da04 7469  etween_ticks..ti
+000006e0: 6d65 da05 736c 6565 70da 0873 6967 5f74  me..sleep..sig_t
+000006f0: 6963 6bda 0465 6d69 74da 1173 656e 645f  ick..emit..send_
+00000700: 696e 666f 5f6d 6573 7361 6765 da10 7061  info_message..pa
+00000710: 725f 706c 6f74 5f66 756e 635f 6964 720a  r_plot_func_idr.
+00000720: 0000 0072 0500 0000 da0b 506c 6f74 5374  ...r......PlotSt
+00000730: 796c 6549 44da 0750 6c6f 7453 696e da06  yleID..PlotSin..
+00000740: 6170 7065 6e64 da04 6d61 7468 da03 7369  append..math..si
+00000750: 6eda 0270 69da 0750 6c6f 7443 6f73 da03  n..pi..PlotCos..
+00000760: 636f 73da 1273 656e 645f 6572 726f 725f  cos..send_error_
+00000770: 6d65 7373 6167 6572 0b00 0000 da0c 7369  messager......si
+00000780: 675f 6e65 775f 6461 7461 720c 0000 0072  g_new_datar....r
+00000790: 0e00 0000 720e 0000 0072 0f00 0000 da07  ....r....r......
+000007a0: 646f 5f77 6f72 6b25 0000 0073 2600 0000  do_work%...s&...
+000007b0: 0003 0802 0601 1801 0e02 0601 0601 1401  ................
+000007c0: 1001 0c01 0a01 1a02 0c02 1001 2401 1201  ............$...
+000007d0: 2402 0a02 1001 7a10 4d79 576f 726b 6572  $.....z.MyWorker
+000007e0: 2e64 6f5f 776f 726b 7207 0000 0063 0100  .do_workr....c..
+000007f0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00000800: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
+00000810: 0072 1700 0000 2901 7219 0000 0072 0c00  .r....).r....r..
+00000820: 0000 720e 0000 0072 0e00 0000 720f 0000  ..r....r....r...
+00000830: 00da 0f67 6574 5f74 6173 6b5f 7265 7375  ...get_task_resu
+00000840: 6c74 4200 0000 7302 0000 0000 017a 184d  ltB...s......z.M
+00000850: 7957 6f72 6b65 722e 6765 745f 7461 736b  yWorker.get_task
+00000860: 5f72 6573 756c 7429 1b72 1100 0000 7212  _result).r....r.
+00000870: 0000 0072 1300 0000 da07 5f5f 646f 635f  ...r......__doc_
+00000880: 5f72 0400 0000 7227 0000 0072 3400 0000  _r....r'...r4...
+00000890: 7220 0000 0072 2300 0000 7222 0000 0072  r ...r#...r"...r
+000008a0: 2400 0000 7205 0000 0072 2b00 0000 722c  $...r....r+...r,
+000008b0: 0000 0072 2a00 0000 da03 7374 72da 0369  ...r*.....str..i
+000008c0: 6e74 5a0c 5f73 6967 5f6d 6573 7361 6765  ntZ._sig_message
+000008d0: da03 6e73 66da 0a66 7261 6d65 776f 726b  ..nsf..framework
+000008e0: 73da 0671 745f 6170 70da 0a4d 6f64 756c  s..qt_app..Modul
+000008f0: 6542 6173 6572 1000 0000 7235 0000 0072  eBaser....r5...r
+00000900: 0600 0000 7236 0000 00da 0d5f 5f63 6c61  ....r6.....__cla
+00000910: 7373 6365 6c6c 5f5f 720e 0000 0072 0e00  sscell__r....r..
+00000920: 0000 721b 0000 0072 0f00 0000 7214 0000  ..r....r....r...
+00000930: 0011 0000 0073 1800 0000 0801 0402 0601  .....s..........
+00000940: 0603 0401 0401 0401 0401 0802 0a02 1805  ................
+00000950: 081d 7214 0000 0029 1272 3700 0000 7225  ..r....).r7...r%
+00000960: 0000 0072 2e00 0000 da0b 6461 7461 636c  ...r......datacl
+00000970: 6173 7365 7372 0200 0000 7203 0000 00da  assesr....r.....
+00000980: 0e50 7953 6964 6536 2e51 7443 6f72 6572  .PySide6.QtCorer
+00000990: 0400 0000 da08 6e61 6e6f 7375 7266 723a  ......nanosurfr:
+000009a0: 0000 00da 0b64 656d 6f5f 6d6f 6475 6c65  .....demo_module
+000009b0: 7205 0000 0072 0600 0000 723b 0000 0072  r....r....r;...r
+000009c0: 3c00 0000 da0a 6e73 665f 7468 7265 6164  <.....nsf_thread
+000009d0: da13 4e53 4642 6163 6b67 726f 756e 6457  ..NSFBackgroundW
+000009e0: 6f72 6b65 7272 1400 0000 720e 0000 0072  orkerr....r....r
+000009f0: 0e00 0000 720e 0000 0072 0f00 0000 da08  ....r....r......
+00000a00: 3c6d 6f64 756c 653e 0100 0000 7310 0000  <module>....s...
+00000a10: 0004 0408 0108 0110 010c 0108 010c 020e  ................
+00000a20: 05                                       .
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/gui.py` & `nanosurf-1.6.2/nanosurf/app/app_template/demo_module/gui.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/module.py` & `nanosurf-1.6.2/nanosurf/app/app_template/demo_module/module.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/settings.py` & `nanosurf-1.6.2/nanosurf/app/app_template/demo_module/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """ Defines the configuration values of the module.
     Values in the ProStore are saved and loaded during application startup/shutdown automatically
 Copyright Nanosurf AG 2021
 License - MIT
 """
 
-from dataclasses import dataclass
 import enum
 import nanosurf.lib.datatypes.sci_val as sci_val
 import nanosurf.lib.datatypes.prop_val as prop_val
 
-@dataclass
 class DemoSettings(prop_val.PropStore):
     """ settings defined here as PropVal are stored persistently in a ini-file
         settings with a '_' as first char are not stored
     """
-    repetitions = prop_val.PropVal(int(300))
-    time_per_repetition = prop_val.PropVal(sci_val.SciVal(0.1, "s"))
-    send_ticks = prop_val.PropVal(False)
-    plot_func_id = prop_val.PropVal(int(0))
-    this_is_not_stored = prop_val.PropVal(int(0))
+    def __init__(self) -> None:
+        super().__init__()
+        self.repetitions = prop_val.PropVal(int(300))
+        self.time_per_repetition = prop_val.PropVal(sci_val.SciVal(0.1, "s"))
+        self.send_ticks = prop_val.PropVal(False)
+        self.plot_func_id = prop_val.PropVal(int(0))
+        self.this_is_not_stored = prop_val.PropVal(int(0))
 
-@dataclass
 class DemoResults():
     """ This class saves the worker task result (e.g be read by gui elements or saved to file """
-    number_of_data_points = 0
-    last_data = 0.0
-    mean_value = 0.0
+    def __init__(self) -> None:
+        self.number_of_data_points = 0
+        self.last_data = 0.0
+        self.mean_value = 0.0
 
 """ Combo boxes show entries with IDs and the names in second list"""
 class PlotStyleID(enum.IntEnum):
     PlotSin = 0,
     PlotCos = 1,
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/worker_task.py` & `nanosurf-1.6.2/nanosurf/app/app_template/demo_module/worker_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import time
 import math
 from dataclasses import dataclass, field
 from PySide6.QtCore import Signal
 import nanosurf as nsf
 from demo_module import settings
 
-@dataclass
 class MyWorkerData():
-    value:list[float] = field(default_factory=list)
-    last_index:int = -1
+    def __init__(self) -> None:
+        self.value:list[float] = []
+        self.last_index:int = -1
 
 class MyWorker(nsf.frameworks.qt_app.nsf_thread.NSFBackgroundWorker):
     """ This class implements the long lasting activity in the background to not freeze the gui """
 
     sig_tick = Signal() # is emitted if par_send_tick is True
     sig_new_data = Signal() # is emitted each time new data are available . Result is read by self.get_result()
```

### Comparing `nanosurf-1.6.1/nanosurf/app/app_template/main.py` & `nanosurf-1.6.2/nanosurf/app/app_template/main.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/demo_creating_spec_pos_table_with_smiley/spectroscopy_demo_creating_a_smiley.ipynb` & `nanosurf-1.6.2/nanosurf/app/demo_creating_spec_pos_table_with_smiley/spectroscopy_demo_creating_a_smiley.ipynb`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/demo_creating_spec_pos_table_with_smiley/spectroscopy_demo_creating_a_smiley.py` & `nanosurf-1.6.2/nanosurf/app/demo_creating_spec_pos_table_with_smiley/spectroscopy_demo_creating_a_smiley.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/demo_lateral_force_signal_calibration/demo_lfm_calibration.ipynb` & `nanosurf-1.6.2/nanosurf/app/demo_lateral_force_signal_calibration/demo_lfm_calibration.ipynb`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/demo_move_sample_stage/demo_move_sample_stage.py` & `nanosurf-1.6.2/nanosurf/app/demo_move_sample_stage/demo_move_sample_stage.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/demo_spec_setup_and_data_plotting/spec_demo.ipynb` & `nanosurf-1.6.2/nanosurf/app/demo_spec_setup_and_data_plotting/spec_demo.ipynb`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/demo_spec_setup_and_data_plotting/spec_demo.py` & `nanosurf-1.6.2/nanosurf/app/demo_spec_setup_and_data_plotting/spec_demo.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/demo_studio_scripting/studio_demo_data_sampling.py` & `nanosurf-1.6.2/nanosurf/app/demo_studio_scripting/studio_demo_data_sampling.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/demo_studio_scripting/studio_scripting_demo.py` & `nanosurf-1.6.2/nanosurf/app/demo_studio_scripting/studio_scripting_demo.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/spm_template/.vscode/launch.json` & `nanosurf-1.6.2/nanosurf/app/spm_template/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/gui.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/gui.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/gui.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/gui.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 10:03:33 2023 UTC, .py size: 9589 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 f524 3964 7525 0000  a........$9du%..
+00000000: 610d 0d0a 0000 0000 5a4d 3964 7525 0000  a.......ZM9du%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6401 6402 6c05  m.Z.m.Z...d.d.l.
 00000050: 5a06 6401 6402 6c07 5a07 6401 6402 6c08  Z.d.d.l.Z.d.d.l.
 00000060: 5a08 4700 6404 6405 8400 6405 6506 6a09  Z.G.d.d...d.e.j.
 00000070: 6a0a 6a0b 8303 5a0c 6506 6a09 a00d 6508  j.j...Z.e.j...e.
@@ -33,15 +33,15 @@
 00000200: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
 00000210: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
 00000220: da0d 4375 7272 656e 7453 616d 706c 65da  ..CurrentSample.
 00000230: 094c 6173 7456 616c 7565 da09 4d65 616e  .LastValue..Mean
 00000240: 5661 6c75 65a9 0072 0e00 0000 720e 0000  Value..r....r...
 00000250: 00fa 3a43 3a5c 4769 745c 7363 7269 7074  ..:C:\Git\script
 00000260: 735f 7079 7468 6f6e 5f6c 6962 5c6e 616e  s_python_lib\nan
-00000270: 6f73 7572 665c 6170 705c 6775 695f 7465  osurf\app\gui_te
+00000270: 6f73 7572 665c 6170 705c 7370 6d5f 7465  osurf\app\spm_te
 00000280: 6d70 6c61 7465 5c67 7569 2e70 7972 0400  mplate\gui.pyr..
 00000290: 0000 0c00 0000 7308 0000 0008 0104 0104  ......s.........
 000002a0: 0104 0172 0400 0000 7a0c 5573 6572 2031  ...r....z.User 1
 000002b0: 2049 6e70 7574 7a10 4465 666c 6563 7469   Inputz.Deflecti
 000002c0: 6f6e 2049 6e70 7574 6300 0000 0000 0000  on Inputc.......
 000002d0: 0000 0000 0000 0000 0004 0000 0000 0000  ................
 000002e0: 0073 ae00 0000 6500 5a01 6400 5a02 8700  .s....e.Z.d.Z...
```

### Comparing `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/measure_task.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/measure_task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/measure_task.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/measure_task.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 09:59:17 2023 UTC, .py size: 3962 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,208 +1,213 @@
-00000000: 610d 0d0a 0000 0000 f523 3964 7a0f 0000  a........#9dz...
+00000000: 610d 0d0a 0000 0000 e606 5a64 a50f 0000  a.........Zd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
+00000020: 0008 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a05 6401  m.Z...d.d.l.Z.d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6402 6c08  d.l.m.Z...d.d.l.
 00000060: 5a09 7a14 6401 6405 6c0a 6d0b 5a0b 6d0c  Z.z.d.d.l.m.Z.m.
 00000070: 5a0c 0100 5700 6e12 0400 650d 795a 0100  Z...W.n...e.yZ..
 00000080: 0100 0100 5900 6e02 3000 6401 6402 6c0e  ....Y.n.0.d.d.l.
-00000090: 5a0e 6503 4700 6406 6407 8400 6407 8302  Z.e.G.d.d...d...
-000000a0: 8301 5a0f 4700 6408 6409 8400 6409 6509  ..Z.G.d.d...d.e.
-000000b0: 6a10 6a11 6a12 6a13 8303 5a14 6402 5300  j.j.j.j...Z.d.S.
-000000c0: 290a 7a84 2054 6865 206c 6f6e 6720 6c61  ).z. The long la
-000000d0: 7374 696e 6720 776f 726b 6572 2074 6872  sting worker thr
-000000e0: 6561 6420 6173 2064 656d 6f20 2d20 6a75  ead as demo - ju
-000000f0: 7374 2077 6169 7420 736f 6d65 2074 696d  st wait some tim
-00000100: 6520 616e 6420 6372 6561 7465 2064 6174  e and create dat
-00000110: 6120 7065 7269 6f64 6963 616c 6c79 0a43  a periodically.C
-00000120: 6f70 7972 6967 6874 204e 616e 6f73 7572  opyright Nanosur
-00000130: 6620 4147 2032 3032 310a 4c69 6365 6e73  f AG 2021.Licens
-00000140: 6520 2d20 4d49 540a e900 0000 004e 2901  e - MIT......N).
-00000150: da09 6461 7461 636c 6173 7329 01da 0653  ..dataclass)...S
-00000160: 6967 6e61 6c29 02da 0452 6f6f 74da 0652  ignal)...Root..R
-00000170: 6f6f 744c 7563 0000 0000 0000 0000 0000  ootLuc..........
-00000180: 0000 0000 0000 0300 0000 4000 0000 7322  ..........@...s"
-00000190: 0000 0065 005a 0164 005a 0255 0065 03a0  ...e.Z.d.Z.U.e..
-000001a0: 04a1 005a 0564 015a 0665 0765 0864 023c  ...Z.d.Z.e.e.d.<
-000001b0: 0064 0353 0029 04da 0d4d 6561 7375 7265  .d.S.)...Measure
-000001c0: 5265 7375 6c74 e9ff ffff ffda 0a6c 6173  Result.......las
-000001d0: 745f 696e 6465 784e 2909 da08 5f5f 6e61  t_indexN)...__na
-000001e0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000001f0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da03  ..__qualname__..
-00000200: 6e73 66da 0953 6369 5374 7265 616d da0e  nsf..SciStream..
-00000210: 6d6f 6e69 746f 725f 7374 7265 616d 7208  monitor_streamr.
-00000220: 0000 00da 0369 6e74 da0f 5f5f 616e 6e6f  .....int..__anno
-00000230: 7461 7469 6f6e 735f 5fa9 0072 1100 0000  tations__..r....
-00000240: 7211 0000 00fa 4343 3a5c 4769 745c 7363  r.....CC:\Git\sc
-00000250: 7269 7074 735f 7079 7468 6f6e 5f6c 6962  ripts_python_lib
-00000260: 5c6e 616e 6f73 7572 665c 6170 705c 6775  \nanosurf\app\gu
-00000270: 695f 7465 6d70 6c61 7465 5c6d 6561 7375  i_template\measu
-00000280: 7265 5f74 6173 6b2e 7079 7206 0000 0011  re_task.pyr.....
-00000290: 0000 0073 0400 0000 0a02 0801 7206 0000  ...s........r...
-000002a0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000002b0: 0000 0400 0000 0000 0000 7368 0000 0065  ..........sh...e
-000002c0: 005a 0164 005a 0264 015a 0364 025a 0464  .Z.d.Z.d.Z.d.Z.d
-000002d0: 035a 0565 066a 076a 085a 0965 0a83 005a  .Z.e.j.j.Z.e...Z
-000002e0: 0b65 0c6a 0d6a 0e6a 0f64 049c 0187 0066  .e.j.j.j.d.....f
-000002f0: 0164 0564 0684 0c5a 1065 1164 079c 0164  .d.d...Z.e.d...d
-00000300: 0864 0984 045a 1264 0a64 0b84 005a 1364  .d...Z.d.d...Z.d
-00000310: 0c64 0d84 005a 1464 0e64 0f84 005a 1587  .d...Z.d.d...Z..
-00000320: 0004 005a 1653 0029 10da 0b4d 6561 7375  ...Z.S.)...Measu
-00000330: 7265 5461 736b 7a58 2054 6869 7320 636c  reTaskzX This cl
-00000340: 6173 7320 696d 706c 656d 656e 7473 2074  ass implements t
-00000350: 6865 2062 6163 6b67 726f 756e 6420 6d65  he background me
-00000360: 6173 7572 656d 656e 7420 7461 736b 2075  asurement task u
-00000370: 7369 6e67 2061 204e 616e 6f73 7572 6620  sing a Nanosurf 
-00000380: 5350 4d20 436f 6e74 726f 6c6c 6572 2020  SPM Controller  
-00000390: e90a 0000 0067 0000 0000 0000 0040 2901  .....g.......@).
-000003a0: da06 6d6f 6475 6c65 6302 0000 0000 0000  ..modulec.......
-000003b0: 0000 0000 0002 0000 0003 0000 0003 0000  ................
-000003c0: 0073 1e00 0000 7c01 7c00 5f00 7401 8300  .s....|.|._.t...
-000003d0: 7c00 5f02 7403 8300 a004 7c01 a101 0100  |._.t.....|.....
-000003e0: 6400 5300 a901 4e29 0572 1500 0000 7206  d.S...N).r....r.
-000003f0: 0000 00da 0672 6573 756c 74da 0573 7570  .....result..sup
-00000400: 6572 da08 5f5f 696e 6974 5f5f 2902 da04  er..__init__)...
-00000410: 7365 6c66 7215 0000 00a9 01da 095f 5f63  selfr........__c
-00000420: 6c61 7373 5f5f 7211 0000 0072 1200 0000  lass__r....r....
-00000430: 7219 0000 0023 0000 0073 0600 0000 0001  r....#...s......
-00000440: 0601 0801 7a14 4d65 6173 7572 6554 6173  ....z.MeasureTas
-00000450: 6b2e 5f5f 696e 6974 5f5f 2901 da06 7265  k.__init__)...re
-00000460: 7475 726e 6301 0000 0000 0000 0000 0000  turnc...........
-00000470: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-00000480: 0000 7c00 6a00 5300 7216 0000 0029 0172  ..|.j.S.r....).r
-00000490: 1700 0000 a901 721a 0000 0072 1100 0000  ......r....r....
-000004a0: 7211 0000 0072 1200 0000 da0f 6765 745f  r....r......get_
-000004b0: 7461 736b 5f72 6573 756c 7428 0000 0073  task_result(...s
-000004c0: 0200 0000 0001 7a1b 4d65 6173 7572 6554  ......z.MeasureT
-000004d0: 6173 6b2e 6765 745f 7461 736b 5f72 6573  ask.get_task_res
-000004e0: 756c 7463 0100 0000 0000 0000 0000 0000  ultc............
-000004f0: 0100 0000 0200 0000 4300 0000 7358 0000  ........C...sX..
-00000500: 007c 0001 007c 0001 007c 006a 0074 016a  .|...|...|.j.t.j
-00000510: 026a 036b 0272 247c 006a 046a 056a 067c  .j.k.r$|.j.j.j.|
-00000520: 005f 076e 307c 006a 0074 016a 026a 086b  ._.n0|.j.t.j.j.k
-00000530: 0272 4c7c 006a 046a 056a 097c 005f 077c  .rL|.j.j.j.|._.|
-00000540: 006a 046a 0a6a 067c 005f 0b6e 0874 0c64  .j.j.j.|._.n.t.d
-00000550: 0183 0182 0164 0053 00a9 024e 7a20 556e  .....d.S...Nz Un
-00000560: 6b6e 6f77 6e20 6d6f 6e69 746f 7220 6368  known monitor ch
-00000570: 616e 6e65 6c20 7365 6c65 6374 6564 290d  annel selected).
-00000580: da0e 7061 725f 6d6f 6e69 746f 725f 6964  ..par_monitor_id
-00000590: da08 7365 7474 696e 6773 da10 4d6f 6e69  ..settings..Moni
-000005a0: 746f 7243 6861 6e6e 656c 4944 da0a 5573  torChannelID..Us
-000005b0: 6572 3149 6e70 7574 da02 6c75 da10 616e  er1Input..lu..an
-000005c0: 616c 6f67 5f68 695f 7265 735f 696e da05  alog_hi_res_in..
-000005d0: 7573 6572 31da 096c 755f 6164 635f 696e  user1..lu_adc_in
-000005e0: da0a 4465 666c 6563 7469 6f6e da0a 6465  ..Deflection..de
-000005f0: 666c 6563 7469 6f6e da0e 7261 6d70 5f67  flection..ramp_g
-00000600: 656e 6572 6174 6f72 da0b 6c75 5f72 616d  enerator..lu_ram
-00000610: 705f 6765 6eda 0a56 616c 7565 4572 726f  p_gen..ValueErro
-00000620: 7272 1e00 0000 7211 0000 0072 1100 0000  rr....r....r....
-00000630: 7212 0000 00da 0b69 6e69 745f 7374 7564  r......init_stud
-00000640: 696f 2b00 0000 7310 0000 0000 0104 0104  io+...s.........
-00000650: 010e 010e 010e 010c 010e 027a 174d 6561  ...........z.Mea
-00000660: 7375 7265 5461 736b 2e69 6e69 745f 7374  sureTask.init_st
-00000670: 7564 696f 6301 0000 0000 0000 0000 0000  udioc...........
-00000680: 0001 0000 0003 0000 0043 0000 0073 6e00  .........C...sn.
-00000690: 0000 7c00 6a00 7401 6a02 6a03 6b02 7226  ..|.j.t.j.j.k.r&
-000006a0: 7c00 6a04 a005 7c00 6a04 6a05 6a06 6a07  |.j...|.j.j.j.j.
-000006b0: a101 7c00 5f08 6e44 7c00 6a00 7401 6a02  ..|._.nD|.j.t.j.
-000006c0: 6a09 6b02 7262 7c00 6a04 a005 7c00 6a04  j.k.rb|.j...|.j.
-000006d0: 6a05 6a06 6a0a a101 7c00 5f08 7c00 6a04  j.j.j...|._.|.j.
-000006e0: a00b 7c00 6a04 6a0b 6a06 6a07 a101 7c00  ..|.j.j.j.j...|.
-000006f0: 5f0c 6e08 740d 6401 8301 8201 6400 5300  _.n.t.d.....d.S.
-00000700: 7220 0000 0029 0e72 2100 0000 7222 0000  r ...).r!...r"..
-00000710: 0072 2300 0000 7224 0000 0072 2500 0000  .r#...r$...r%...
-00000720: da0d 416e 616c 6f67 4869 5265 7349 6eda  ..AnalogHiResIn.
-00000730: 0849 6e73 7461 6e63 65da 0555 5345 5231  .Instance..USER1
-00000740: 7228 0000 0072 2900 0000 da0a 4445 464c  r(...r).....DEFL
-00000750: 4543 5449 4f4e 5a0d 5261 6d70 4765 6e65  ECTIONZ.RampGene
-00000760: 7261 746f 7272 2c00 0000 722d 0000 0072  ratorr,...r-...r
-00000770: 1e00 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-00000780: 0000 00da 0869 6e69 745f 7370 6d36 0000  .....init_spm6..
-00000790: 0073 0c00 0000 0001 0e01 1801 0e01 1601  .s..............
-000007a0: 1802 7a14 4d65 6173 7572 6554 6173 6b2e  ..z.MeasureTask.
-000007b0: 696e 6974 5f73 706d 6301 0000 0000 0000  init_spmc.......
-000007c0: 0000 0000 0003 0000 0007 0000 0043 0000  .............C..
-000007d0: 0073 0401 0000 7400 8300 7c00 5f01 7c00  .s....t...|._.|.
-000007e0: a002 a100 72f8 7403 6a04 7405 6a06 6401  ....r.t.j.t.j.d.
-000007f0: 7c00 6a07 7c00 6a08 1400 7c00 6a07 6402  |.j.|.j...|.j.d.
-00000800: 6403 8d04 6404 6405 6406 8d03 7c00 6a01  d...d.d.d...|.j.
-00000810: 5f09 7c00 6a0a 6a0b 724e 7c00 a00c a100  _.|.j.j.rN|.....
-00000820: 0100 6e08 7c00 a00d a100 0100 7c00 6a0e  ..n.|.......|.j.
-00000830: 6a0f 6a10 6a11 7d01 7c00 6a01 6a09 a012  j.j.j.}.|.j.j...
-00000840: 6401 7413 a014 7c00 6a15 a101 6a16 a102  d.t...|.j...j...
-00000850: 0100 7c00 6a01 6a09 a017 6401 7c01 a102  ..|.j.j...d.|...
-00000860: 0100 6401 7c00 5f18 7c00 6a18 7c00 6a07  ..d.|._.|.j.|.j.
-00000870: 6b00 72f8 7c00 a019 a100 73f8 7c00 6a0e  k.r.|.....s.|.j.
-00000880: 6a0f 6a10 6a1a 7d02 7c02 7c00 6a01 6a09  j.j.j.}.|.|.j.j.
-00000890: 6a1b 6401 1900 6a1a 7c00 6a18 3c00 7c00  j.d...j.|.j.<.|.
-000008a0: 6a18 7c00 6a01 5f1c 7c00 6a1d a01e a100  j.|.j._.|.j.....
-000008b0: 0100 741f a020 7c00 6a08 a101 0100 7c00  ..t.. |.j.....|.
-000008c0: 0400 6a18 6407 3700 0200 5f18 7192 7c00  ..j.d.7..._.q.|.
-000008d0: a021 a100 0100 6408 5300 2909 7a2f 2054  .!....d.S.).z/ T
-000008e0: 6869 7320 6973 2074 6865 2077 6f72 6b69  his is the worki
-000008f0: 6e67 2066 756e 6374 696f 6e20 666f 7220  ng function for 
-00000900: 7468 6520 6c6f 6e67 2074 6173 6b72 0100  the long taskr..
-00000910: 0000 4629 01da 0865 6e64 706f 696e 74da  ..F)...endpoint.
-00000920: 0173 da04 5469 6d65 2903 da06 736f 7572  .s..Time)...sour
-00000930: 6365 da06 785f 756e 6974 da06 785f 6e61  ce..x_unit..x_na
-00000940: 6d65 e901 0000 004e 2922 7206 0000 0072  me.....N)"r....r
-00000950: 1700 0000 da15 636f 6e6e 6563 745f 746f  ......connect_to
-00000960: 5f63 6f6e 7472 6f6c 6c65 7272 0c00 0000  _controllerr....
-00000970: 720d 0000 00da 026e 70da 086c 696e 7370  r......np..linsp
-00000980: 6163 65da 1170 6172 5f73 616d 706c 655f  ace..par_sample_
-00000990: 706f 696e 7473 da13 7061 725f 7469 6d65  points..par_time
-000009a0: 5f70 6572 5f73 616d 706c 6572 0e00 0000  _per_sampler....
-000009b0: da03 7370 6dda 0969 735f 7374 7564 696f  ..spm..is_studio
-000009c0: 722e 0000 0072 3300 0000 7228 0000 00da  r....r3...r(....
-000009d0: 0961 7474 7269 6275 7465 da13 6375 7272  .attribute..curr
-000009e0: 656e 745f 696e 7075 745f 7661 6c75 65da  ent_input_value.
-000009f0: 0475 6e69 74da 1073 6574 5f63 6861 6e6e  .unit..set_chann
-00000a00: 656c 5f6e 616d 6572 2200 0000 7223 0000  el_namer"...r#..
-00000a10: 0072 2100 0000 da04 6e61 6d65 da10 7365  .r!.....name..se
-00000a20: 745f 6368 616e 6e65 6c5f 756e 6974 da05  t_channel_unit..
-00000a30: 636f 756e 74da 1769 735f 7374 6f70 5f72  count..is_stop_r
-00000a40: 6571 7565 7374 5f70 656e 6469 6e67 da05  equest_pending..
-00000a50: 7661 6c75 65da 0863 6861 6e6e 656c 7372  value..channelsr
-00000a60: 0800 0000 da0e 7369 675f 6e65 775f 7265  ......sig_new_re
-00000a70: 7375 6c74 da04 656d 6974 da04 7469 6d65  sult..emit..time
-00000a80: da05 736c 6565 70da 1a64 6973 636f 6e6e  ..sleep..disconn
-00000a90: 6563 745f 6672 6f6d 5f63 6f6e 7472 6f6c  ect_from_control
-00000aa0: 6c65 7229 0372 1a00 0000 5a0c 6368 616e  ler).r....Z.chan
-00000ab0: 6e65 6c5f 756e 6974 da09 6e65 775f 7661  nel_unit..new_va
-00000ac0: 6c75 6572 1100 0000 7211 0000 0072 1200  luer....r....r..
-00000ad0: 0000 da07 646f 5f77 6f72 6b3f 0000 0073  ....do_work?...s
-00000ae0: 2c00 0000 0002 0801 0803 0401 1a01 0201  ,...............
-00000af0: 02fd 0a06 0801 0a02 0802 0c01 1a01 1003  ................
-00000b00: 0601 1401 0c02 1601 0a01 0a02 0c01 1002  ................
-00000b10: 7a13 4d65 6173 7572 6554 6173 6b2e 646f  z.MeasureTask.do
-00000b20: 5f77 6f72 6b29 1772 0900 0000 720a 0000  _work).r....r...
-00000b30: 0072 0b00 0000 da07 5f5f 646f 635f 5f72  .r......__doc__r
-00000b40: 3e00 0000 723f 0000 0072 2200 0000 7223  >...r?...r"...r#
-00000b50: 0000 0072 2400 0000 7221 0000 0072 0300  ...r$...r!...r..
-00000b60: 0000 724c 0000 0072 0c00 0000 da0a 6672  ..rL...r......fr
-00000b70: 616d 6577 6f72 6b73 da06 7174 5f61 7070  ameworks..qt_app
-00000b80: da0a 4d6f 6475 6c65 4261 7365 7219 0000  ..ModuleBaser...
-00000b90: 0072 0600 0000 721f 0000 0072 2e00 0000  .r....r....r....
-00000ba0: 7233 0000 0072 5200 0000 da0d 5f5f 636c  r3...rR.....__cl
-00000bb0: 6173 7363 656c 6c5f 5f72 1100 0000 7211  asscell__r....r.
-00000bc0: 0000 0072 1b00 0000 7212 0000 0072 1300  ...r....r....r..
-00000bd0: 0000 1700 0000 7314 0000 0008 0104 0404  ......s.........
-00000be0: 0104 0108 0306 0218 050e 0308 0b08 0972  ...............r
-00000bf0: 1300 0000 2915 7253 0000 0072 4e00 0000  ....).rS...rN...
-00000c00: da0b 6461 7461 636c 6173 7365 7372 0200  ..dataclassesr..
-00000c10: 0000 da05 6e75 6d70 7972 3c00 0000 da0e  ....numpyr<.....
-00000c20: 5079 5369 6465 362e 5174 436f 7265 7203  PySide6.QtCorer.
-00000c30: 0000 00da 086e 616e 6f73 7572 6672 0c00  .....nanosurfr..
-00000c40: 0000 da2c 6e61 6e6f 7375 7266 2e6c 6962  ...,nanosurf.lib
-00000c50: 2e73 706d 2e73 7475 6469 6f2e 7772 6170  .spm.studio.wrap
-00000c60: 7065 722e 636d 645f 7472 6565 5f73 706d  per.cmd_tree_spm
-00000c70: 7204 0000 0072 0500 0000 da0b 496d 706f  r....r......Impo
-00000c80: 7274 4572 726f 7272 2200 0000 7206 0000  rtErrorr"...r...
-00000c90: 0072 5400 0000 7255 0000 00da 0a6e 7366  .rT...rU.....nsf
-00000ca0: 5f74 6872 6561 64da 0953 504d 576f 726b  _thread..SPMWork
-00000cb0: 6572 7213 0000 0072 1100 0000 7211 0000  err....r....r...
-00000cc0: 0072 1100 0000 7212 0000 00da 083c 6d6f  .r....r......<mo
-00000cd0: 6475 6c65 3e01 0000 0073 1a00 0000 0404  dule>....s......
-00000ce0: 0801 0c01 0801 0c02 0801 0201 1401 0c01  ................
-00000cf0: 0601 0802 0201 1005                      ........
+00000090: 5a0e 4700 6406 6407 8400 6407 8302 5a0f  Z.G.d.d...d...Z.
+000000a0: 4700 6408 6409 8400 6409 6509 6a10 6a11  G.d.d...d.e.j.j.
+000000b0: 6a12 6a13 8303 5a14 6402 5300 290a 7a84  j.j...Z.d.S.).z.
+000000c0: 2054 6865 206c 6f6e 6720 6c61 7374 696e   The long lastin
+000000d0: 6720 776f 726b 6572 2074 6872 6561 6420  g worker thread 
+000000e0: 6173 2064 656d 6f20 2d20 6a75 7374 2077  as demo - just w
+000000f0: 6169 7420 736f 6d65 2074 696d 6520 616e  ait some time an
+00000100: 6420 6372 6561 7465 2064 6174 6120 7065  d create data pe
+00000110: 7269 6f64 6963 616c 6c79 0a43 6f70 7972  riodically.Copyr
+00000120: 6967 6874 204e 616e 6f73 7572 6620 4147  ight Nanosurf AG
+00000130: 2032 3032 310a 4c69 6365 6e73 6520 2d20   2021.License - 
+00000140: 4d49 540a e900 0000 004e 2901 da09 6461  MIT......N)...da
+00000150: 7461 636c 6173 7329 01da 0653 6967 6e61  taclass)...Signa
+00000160: 6c29 02da 0452 6f6f 74da 0652 6f6f 744c  l)...Root..RootL
+00000170: 7563 0000 0000 0000 0000 0000 0000 0000  uc..............
+00000180: 0000 0300 0000 4000 0000 731a 0000 0065  ......@...s....e
+00000190: 005a 0164 005a 0264 0164 029c 0164 0364  .Z.d.Z.d.d...d.d
+000001a0: 0484 045a 0364 0153 0029 05da 0d4d 6561  ...Z.d.S.)...Mea
+000001b0: 7375 7265 5265 7375 6c74 4ea9 01da 0672  sureResultN....r
+000001c0: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
+000001d0: 0000 0100 0000 0200 0000 4300 0000 7314  ..........C...s.
+000001e0: 0000 0074 00a0 01a1 007c 005f 0264 017c  ...t.....|._.d.|
+000001f0: 005f 0364 0053 0029 024e e9ff ffff ff29  ._.d.S.).N.....)
+00000200: 04da 036e 7366 da09 5363 6953 7472 6561  ...nsf..SciStrea
+00000210: 6dda 0e6d 6f6e 6974 6f72 5f73 7472 6561  m..monitor_strea
+00000220: 6dda 0a6c 6173 745f 696e 6465 78a9 01da  m..last_index...
+00000230: 0473 656c 66a9 0072 1000 0000 fa43 433a  .self..r.....CC:
+00000240: 5c47 6974 5c73 6372 6970 7473 5f70 7974  \Git\scripts_pyt
+00000250: 686f 6e5f 6c69 625c 6e61 6e6f 7375 7266  hon_lib\nanosurf
+00000260: 5c61 7070 5c73 706d 5f74 656d 706c 6174  \app\spm_templat
+00000270: 655c 6d65 6173 7572 655f 7461 736b 2e70  e\measure_task.p
+00000280: 79da 085f 5f69 6e69 745f 5f12 0000 0073  y..__init__....s
+00000290: 0400 0000 0001 0a01 7a16 4d65 6173 7572  ........z.Measur
+000002a0: 6552 6573 756c 742e 5f5f 696e 6974 5f5f  eResult.__init__
+000002b0: 2904 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+000002c0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+000002d0: 6e61 6d65 5f5f 7212 0000 0072 1000 0000  name__r....r....
+000002e0: 7210 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
+000002f0: 0600 0000 1100 0000 7302 0000 0008 0172  ........s......r
+00000300: 0600 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000310: 0000 0000 0004 0000 0000 0000 0073 6800  .............sh.
+00000320: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+00000330: 5a04 6403 5a05 6506 6a07 6a08 5a09 650a  Z.d.Z.e.j.j.Z.e.
+00000340: 8300 5a0b 650c 6a0d 6a0e 6a0f 6404 9c01  ..Z.e.j.j.j.d...
+00000350: 8700 6601 6405 6406 840c 5a10 6511 6407  ..f.d.d...Z.e.d.
+00000360: 9c01 6408 6409 8404 5a12 640a 640b 8400  ..d.d...Z.d.d...
+00000370: 5a13 640c 640d 8400 5a14 640e 640f 8400  Z.d.d...Z.d.d...
+00000380: 5a15 8700 0400 5a16 5300 2910 da0b 4d65  Z.....Z.S.)...Me
+00000390: 6173 7572 6554 6173 6b7a 5820 5468 6973  asureTaskzX This
+000003a0: 2063 6c61 7373 2069 6d70 6c65 6d65 6e74   class implement
+000003b0: 7320 7468 6520 6261 636b 6772 6f75 6e64  s the background
+000003c0: 206d 6561 7375 7265 6d65 6e74 2074 6173   measurement tas
+000003d0: 6b20 7573 696e 6720 6120 4e61 6e6f 7375  k using a Nanosu
+000003e0: 7266 2053 504d 2043 6f6e 7472 6f6c 6c65  rf SPM Controlle
+000003f0: 7220 20e9 0a00 0000 6700 0000 0000 0000  r  .....g.......
+00000400: 4029 01da 066d 6f64 756c 6563 0200 0000  @)...modulec....
+00000410: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00000420: 0300 0000 731e 0000 007c 017c 005f 0074  ....s....|.|._.t
+00000430: 0183 007c 005f 0274 0383 00a0 047c 01a1  ...|._.t.....|..
+00000440: 0101 0064 0053 00a9 014e 2905 7218 0000  ...d.S...N).r...
+00000450: 0072 0600 0000 da06 7265 7375 6c74 da05  .r......result..
+00000460: 7375 7065 7272 1200 0000 2902 720f 0000  superr....).r...
+00000470: 0072 1800 0000 a901 da09 5f5f 636c 6173  .r........__clas
+00000480: 735f 5f72 1000 0000 7211 0000 0072 1200  s__r....r....r..
+00000490: 0000 2300 0000 7306 0000 0000 0106 0108  ..#...s.........
+000004a0: 017a 144d 6561 7375 7265 5461 736b 2e5f  .z.MeasureTask._
+000004b0: 5f69 6e69 745f 5f72 0700 0000 6301 0000  _init__r....c...
+000004c0: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+000004d0: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
+000004e0: 7219 0000 0029 0172 1a00 0000 720e 0000  r....).r....r...
+000004f0: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
+00000500: da0f 6765 745f 7461 736b 5f72 6573 756c  ..get_task_resul
+00000510: 7428 0000 0073 0200 0000 0001 7a1b 4d65  t(...s......z.Me
+00000520: 6173 7572 6554 6173 6b2e 6765 745f 7461  asureTask.get_ta
+00000530: 736b 5f72 6573 756c 7463 0100 0000 0000  sk_resultc......
+00000540: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00000550: 0000 7358 0000 007c 0001 007c 0001 007c  ..sX...|...|...|
+00000560: 006a 0074 016a 026a 036b 0272 247c 006a  .j.t.j.j.k.r$|.j
+00000570: 046a 056a 067c 005f 076e 307c 006a 0074  .j.j.|._.n0|.j.t
+00000580: 016a 026a 086b 0272 4c7c 006a 046a 056a  .j.j.k.rL|.j.j.j
+00000590: 097c 005f 077c 006a 046a 0a6a 067c 005f  .|._.|.j.j.j.|._
+000005a0: 0b6e 0874 0c64 0183 0182 0164 0053 00a9  .n.t.d.....d.S..
+000005b0: 024e 7a20 556e 6b6e 6f77 6e20 6d6f 6e69  .Nz Unknown moni
+000005c0: 746f 7220 6368 616e 6e65 6c20 7365 6c65  tor channel sele
+000005d0: 6374 6564 290d da0e 7061 725f 6d6f 6e69  cted)...par_moni
+000005e0: 746f 725f 6964 da08 7365 7474 696e 6773  tor_id..settings
+000005f0: da10 4d6f 6e69 746f 7243 6861 6e6e 656c  ..MonitorChannel
+00000600: 4944 da0a 5573 6572 3149 6e70 7574 da02  ID..User1Input..
+00000610: 6c75 da10 616e 616c 6f67 5f68 695f 7265  lu..analog_hi_re
+00000620: 735f 696e da05 7573 6572 31da 096c 755f  s_in..user1..lu_
+00000630: 6164 635f 696e da0a 4465 666c 6563 7469  adc_in..Deflecti
+00000640: 6f6e da0a 6465 666c 6563 7469 6f6e da0e  on..deflection..
+00000650: 7261 6d70 5f67 656e 6572 6174 6f72 da0b  ramp_generator..
+00000660: 6c75 5f72 616d 705f 6765 6eda 0a56 616c  lu_ramp_gen..Val
+00000670: 7565 4572 726f 7272 0e00 0000 7210 0000  ueErrorr....r...
+00000680: 0072 1000 0000 7211 0000 00da 0b69 6e69  .r....r......ini
+00000690: 745f 7374 7564 696f 2b00 0000 7310 0000  t_studio+...s...
+000006a0: 0000 0104 0104 010e 010e 010e 010c 010e  ................
+000006b0: 027a 174d 6561 7375 7265 5461 736b 2e69  .z.MeasureTask.i
+000006c0: 6e69 745f 7374 7564 696f 6301 0000 0000  nit_studioc.....
+000006d0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+000006e0: 0000 0073 6e00 0000 7c00 6a00 7401 6a02  ...sn...|.j.t.j.
+000006f0: 6a03 6b02 7226 7c00 6a04 a005 7c00 6a04  j.k.r&|.j...|.j.
+00000700: 6a05 6a06 6a07 a101 7c00 5f08 6e44 7c00  j.j.j...|._.nD|.
+00000710: 6a00 7401 6a02 6a09 6b02 7262 7c00 6a04  j.t.j.j.k.rb|.j.
+00000720: a005 7c00 6a04 6a05 6a06 6a0a a101 7c00  ..|.j.j.j.j...|.
+00000730: 5f08 7c00 6a04 a00b 7c00 6a04 6a0b 6a06  _.|.j...|.j.j.j.
+00000740: 6a07 a101 7c00 5f0c 6e08 740d 6401 8301  j...|._.n.t.d...
+00000750: 8201 6400 5300 721f 0000 0029 0e72 2000  ..d.S.r....).r .
+00000760: 0000 7221 0000 0072 2200 0000 7223 0000  ..r!...r"...r#..
+00000770: 0072 2400 0000 da0d 416e 616c 6f67 4869  .r$.....AnalogHi
+00000780: 5265 7349 6eda 0849 6e73 7461 6e63 65da  ResIn..Instance.
+00000790: 0555 5345 5231 7227 0000 0072 2800 0000  .USER1r'...r(...
+000007a0: da0a 4445 464c 4543 5449 4f4e 5a0d 5261  ..DEFLECTIONZ.Ra
+000007b0: 6d70 4765 6e65 7261 746f 7272 2b00 0000  mpGeneratorr+...
+000007c0: 722c 0000 0072 0e00 0000 7210 0000 0072  r,...r....r....r
+000007d0: 1000 0000 7211 0000 00da 0869 6e69 745f  ....r......init_
+000007e0: 7370 6d36 0000 0073 0c00 0000 0001 0e01  spm6...s........
+000007f0: 1801 0e01 1601 1802 7a14 4d65 6173 7572  ........z.Measur
+00000800: 6554 6173 6b2e 696e 6974 5f73 706d 6301  eTask.init_spmc.
+00000810: 0000 0000 0000 0000 0000 0003 0000 0007  ................
+00000820: 0000 0043 0000 0073 0401 0000 7400 8300  ...C...s....t...
+00000830: 7c00 5f01 7c00 a002 a100 72f8 7403 6a04  |._.|.....r.t.j.
+00000840: 7405 6a06 6401 7c00 6a07 7c00 6a08 1400  t.j.d.|.j.|.j...
+00000850: 7c00 6a07 6402 6403 8d04 6404 6405 6406  |.j.d.d...d.d.d.
+00000860: 8d03 7c00 6a01 5f09 7c00 6a0a 6a0b 724e  ..|.j._.|.j.j.rN
+00000870: 7c00 a00c a100 0100 6e08 7c00 a00d a100  |.......n.|.....
+00000880: 0100 7c00 6a0e 6a0f 6a10 6a11 7d01 7c00  ..|.j.j.j.j.}.|.
+00000890: 6a01 6a09 a012 6401 7413 a014 7c00 6a15  j.j...d.t...|.j.
+000008a0: a101 6a16 a102 0100 7c00 6a01 6a09 a017  ..j.....|.j.j...
+000008b0: 6401 7c01 a102 0100 6401 7c00 5f18 7c00  d.|.....d.|._.|.
+000008c0: 6a18 7c00 6a07 6b00 72f8 7c00 a019 a100  j.|.j.k.r.|.....
+000008d0: 73f8 7c00 6a0e 6a0f 6a10 6a1a 7d02 7c02  s.|.j.j.j.j.}.|.
+000008e0: 7c00 6a01 6a09 6a1b 6401 1900 6a1a 7c00  |.j.j.j.d...j.|.
+000008f0: 6a18 3c00 7c00 6a18 7c00 6a01 5f1c 7c00  j.<.|.j.|.j._.|.
+00000900: 6a1d a01e a100 0100 741f a020 7c00 6a08  j.......t.. |.j.
+00000910: a101 0100 7c00 0400 6a18 6407 3700 0200  ....|...j.d.7...
+00000920: 5f18 7192 7c00 a021 a100 0100 6408 5300  _.q.|..!....d.S.
+00000930: 2909 7a2f 2054 6869 7320 6973 2074 6865  ).z/ This is the
+00000940: 2077 6f72 6b69 6e67 2066 756e 6374 696f   working functio
+00000950: 6e20 666f 7220 7468 6520 6c6f 6e67 2074  n for the long t
+00000960: 6173 6b72 0100 0000 4629 01da 0865 6e64  askr....F)...end
+00000970: 706f 696e 74da 0173 da04 5469 6d65 2903  point..s..Time).
+00000980: da06 736f 7572 6365 da06 785f 756e 6974  ..source..x_unit
+00000990: da06 785f 6e61 6d65 e901 0000 004e 2922  ..x_name.....N)"
+000009a0: 7206 0000 0072 1a00 0000 da15 636f 6e6e  r....r......conn
+000009b0: 6563 745f 746f 5f63 6f6e 7472 6f6c 6c65  ect_to_controlle
+000009c0: 7272 0a00 0000 720b 0000 00da 026e 70da  rr....r......np.
+000009d0: 086c 696e 7370 6163 65da 1170 6172 5f73  .linspace..par_s
+000009e0: 616d 706c 655f 706f 696e 7473 da13 7061  ample_points..pa
+000009f0: 725f 7469 6d65 5f70 6572 5f73 616d 706c  r_time_per_sampl
+00000a00: 6572 0c00 0000 da03 7370 6dda 0969 735f  er......spm..is_
+00000a10: 7374 7564 696f 722d 0000 0072 3200 0000  studior-...r2...
+00000a20: 7227 0000 00da 0961 7474 7269 6275 7465  r'.....attribute
+00000a30: da13 6375 7272 656e 745f 696e 7075 745f  ..current_input_
+00000a40: 7661 6c75 65da 0475 6e69 74da 1073 6574  value..unit..set
+00000a50: 5f63 6861 6e6e 656c 5f6e 616d 6572 2100  _channel_namer!.
+00000a60: 0000 7222 0000 0072 2000 0000 da04 6e61  ..r"...r .....na
+00000a70: 6d65 da10 7365 745f 6368 616e 6e65 6c5f  me..set_channel_
+00000a80: 756e 6974 da05 636f 756e 74da 1769 735f  unit..count..is_
+00000a90: 7374 6f70 5f72 6571 7565 7374 5f70 656e  stop_request_pen
+00000aa0: 6469 6e67 da05 7661 6c75 65da 0863 6861  ding..value..cha
+00000ab0: 6e6e 656c 7372 0d00 0000 da0e 7369 675f  nnelsr......sig_
+00000ac0: 6e65 775f 7265 7375 6c74 da04 656d 6974  new_result..emit
+00000ad0: da04 7469 6d65 da05 736c 6565 70da 1a64  ..time..sleep..d
+00000ae0: 6973 636f 6e6e 6563 745f 6672 6f6d 5f63  isconnect_from_c
+00000af0: 6f6e 7472 6f6c 6c65 7229 0372 0f00 0000  ontroller).r....
+00000b00: 5a0c 6368 616e 6e65 6c5f 756e 6974 da09  Z.channel_unit..
+00000b10: 6e65 775f 7661 6c75 6572 1000 0000 7210  new_valuer....r.
+00000b20: 0000 0072 1100 0000 da07 646f 5f77 6f72  ...r......do_wor
+00000b30: 6b3f 0000 0073 2c00 0000 0002 0801 0803  k?...s,.........
+00000b40: 0401 1a01 0201 02fd 0a06 0801 0a02 0802  ................
+00000b50: 0c01 1a01 1003 0601 1401 0c02 1601 0a01  ................
+00000b60: 0a02 0c01 1002 7a13 4d65 6173 7572 6554  ......z.MeasureT
+00000b70: 6173 6b2e 646f 5f77 6f72 6b29 1772 1300  ask.do_work).r..
+00000b80: 0000 7214 0000 0072 1500 0000 da07 5f5f  ..r....r......__
+00000b90: 646f 635f 5f72 3d00 0000 723e 0000 0072  doc__r=...r>...r
+00000ba0: 2100 0000 7222 0000 0072 2300 0000 7220  !...r"...r#...r 
+00000bb0: 0000 0072 0300 0000 724b 0000 0072 0a00  ...r....rK...r..
+00000bc0: 0000 da0a 6672 616d 6577 6f72 6b73 da06  ....frameworks..
+00000bd0: 7174 5f61 7070 da0a 4d6f 6475 6c65 4261  qt_app..ModuleBa
+00000be0: 7365 7212 0000 0072 0600 0000 721e 0000  ser....r....r...
+00000bf0: 0072 2d00 0000 7232 0000 0072 5100 0000  .r-...r2...rQ...
+00000c00: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
+00000c10: 1000 0000 7210 0000 0072 1c00 0000 7211  ....r....r....r.
+00000c20: 0000 0072 1600 0000 1700 0000 7314 0000  ...r........s...
+00000c30: 0008 0104 0404 0104 0108 0306 0218 050e  ................
+00000c40: 0308 0b08 0972 1600 0000 2915 7252 0000  .....r....).rR..
+00000c50: 0072 4d00 0000 da0b 6461 7461 636c 6173  .rM.....dataclas
+00000c60: 7365 7372 0200 0000 da05 6e75 6d70 7972  sesr......numpyr
+00000c70: 3b00 0000 da0e 5079 5369 6465 362e 5174  ;.....PySide6.Qt
+00000c80: 436f 7265 7203 0000 00da 086e 616e 6f73  Corer......nanos
+00000c90: 7572 6672 0a00 0000 da2c 6e61 6e6f 7375  urfr.....,nanosu
+00000ca0: 7266 2e6c 6962 2e73 706d 2e73 7475 6469  rf.lib.spm.studi
+00000cb0: 6f2e 7772 6170 7065 722e 636d 645f 7472  o.wrapper.cmd_tr
+00000cc0: 6565 5f73 706d 7204 0000 0072 0500 0000  ee_spmr....r....
+00000cd0: da0b 496d 706f 7274 4572 726f 7272 2100  ..ImportErrorr!.
+00000ce0: 0000 7206 0000 0072 5300 0000 7254 0000  ..r....rS...rT..
+00000cf0: 00da 0a6e 7366 5f74 6872 6561 64da 0953  ...nsf_thread..S
+00000d00: 504d 576f 726b 6572 7216 0000 0072 1000  PMWorkerr....r..
+00000d10: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
+00000d20: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000d30: 1800 0000 0404 0801 0c01 0801 0c02 0801  ................
+00000d40: 0201 1401 0c01 0601 0802 0e06            ............
```

### Comparing `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/module.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/module.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/module.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/module.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 12:52:48 2023 UTC, .py size: 7804 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 a04c 3964 7c1e 0000  a........L9d|...
+00000000: 610d 0d0a 0000 0000 5a4d 3964 7c1e 0000  a.......ZM9d|...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6403 6c04 6d05 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c07 6d08 5a08 0100 6401 6405 6c09  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6401 6402 6c0b 5a0c 6401  m.Z...d.d.l.Z.d.
 00000070: 6406 6c0d 6d0e 5a0e 0100 6401 6402 6c0f  d.l.m.Z...d.d.l.
```

### Comparing `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/settings.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/settings.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Mar 22 08:26:22 2023 UTC, .py size: 1210 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,123 @@
-00000000: 6f0d 0d0a 0000 0000 aebb 1a64 ba04 0000  o..........d....
+00000000: 610d 0d0a 0000 0000 6205 5a64 4a05 0000  a.......b.ZdJ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
+00000020: 0004 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
-00000050: 6d05 5a05 0100 6401 6402 6c06 5a07 0900  m.Z...d.d.l.Z...
-00000060: 4700 6404 6405 8400 6405 6501 6a08 8303  G.d.d...d.e.j...
-00000070: 5a09 6505 4700 6406 6407 8400 6407 6507  Z.e.G.d.d...d.e.
-00000080: 6a0a 8303 8301 5a0b 6505 4700 6408 6409  j.....Z.e.G.d.d.
-00000090: 8400 6409 8302 8301 5a0c 6402 5300 290a  ..d.....Z.d.S.).
-000000a0: 7abc 2044 6566 696e 6573 2074 6865 2063  z. Defines the c
-000000b0: 6f6e 6669 6775 7261 7469 6f6e 2076 616c  onfiguration val
-000000c0: 7565 7320 6f66 2074 6865 206d 6f64 756c  ues of the modul
-000000d0: 652e 0a20 2020 2056 616c 7565 7320 696e  e..    Values in
-000000e0: 2074 6865 2050 726f 5374 6f72 6520 6172   the ProStore ar
-000000f0: 6520 7361 7665 6420 616e 6420 6c6f 6164  e saved and load
-00000100: 6564 2064 7572 696e 6720 6170 706c 6963  ed during applic
-00000110: 6174 696f 6e20 7374 6172 7475 702f 7368  ation startup/sh
-00000120: 7574 646f 776e 2061 7574 6f6d 6174 6963  utdown automatic
-00000130: 616c 6c79 0a43 6f70 7972 6967 6874 204e  ally.Copyright N
-00000140: 616e 6f73 7572 6620 4147 2032 3032 310a  anosurf AG 2021.
-00000150: 4c69 6365 6e73 6520 2d20 4d49 540a e900  License - MIT...
-00000160: 0000 004e 2901 da09 6461 7461 636c 6173  ...N)...dataclas
-00000170: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
-00000180: 0000 0100 0000 4000 0000 7314 0000 0065  ......@...s....e
-00000190: 005a 0164 005a 0264 015a 0364 025a 0464  .Z.d.Z.d.Z.d.Z.d
-000001a0: 0353 0029 04da 104d 6f6e 6974 6f72 4368  .S.)...MonitorCh
-000001b0: 616e 6e65 6c49 4429 0172 0100 0000 2901  annelID).r....).
-000001c0: e901 0000 004e 2905 da08 5f5f 6e61 6d65  .....N)...__name
-000001d0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-000001e0: 5f5f 7175 616c 6e61 6d65 5f5f 5a0a 5573  __qualname__Z.Us
-000001f0: 6572 3149 6e70 7574 da0a 4465 666c 6563  er1Input..Deflec
-00000200: 7469 6f6e a900 7209 0000 0072 0900 0000  tion..r....r....
-00000210: fa3f 433a 5c47 6974 5c73 6372 6970 7473  .?C:\Git\scripts
-00000220: 5f70 7974 686f 6e5f 6c69 625c 6e61 6e6f  _python_lib\nano
-00000230: 7375 7266 5c61 7070 5c67 7569 5f74 656d  surf\app\gui_tem
-00000240: 706c 6174 655c 7365 7474 696e 6773 2e70  plate\settings.p
-00000250: 7972 0300 0000 0e00 0000 7306 0000 0008  yr........s.....
-00000260: 0004 0108 0172 0300 0000 6300 0000 0000  .....r....c.....
-00000270: 0000 0000 0000 0000 0000 0007 0000 0040  ...............@
-00000280: 0000 0073 5a00 0000 6500 5a01 6400 5a02  ...sZ...e.Z.d.Z.
-00000290: 6401 5a03 6504 a005 6506 6402 8301 a101  d.Z.e...e.d.....
-000002a0: 5a07 6504 a005 6504 a008 6403 6404 a102  Z.e...e...d.d...
-000002b0: a101 5a09 6504 a005 6506 650a 6a0b 8301  ..Z.e...e.e.j...
-000002c0: a101 5a0c 6504 a005 650d a00e 650f a010  ..Z.e...e...e...
-000002d0: 6405 a101 a101 6406 1b00 a101 5a11 6407  d.....d.....Z.d.
-000002e0: 5300 2908 da08 5365 7474 696e 6773 7aad  S.)...Settingsz.
-000002f0: 2073 6574 7469 6e67 7320 6465 6669 6e65   settings define
-00000300: 6420 6865 7265 2061 7320 5072 6f70 5661  d here as PropVa
-00000310: 6c20 6172 6520 7374 6f72 6564 2070 6572  l are stored per
-00000320: 7369 7374 656e 746c 7920 696e 2061 2069  sistently in a i
-00000330: 6e69 2d66 696c 6520 0a20 2020 2020 2020  ni-file .       
-00000340: 2043 6f75 6c64 2062 6520 636f 6e6e 6563   Could be connec
-00000350: 7465 6420 616c 736f 2074 6f20 4755 4920  ted also to GUI 
-00000360: 656c 656d 656e 7473 2028 652e 672e 3a20  elements (e.g.: 
-00000370: 6c6f 6f6b 2069 6e74 6f20 6269 6e64 5f67  look into bind_g
-00000380: 7569 5f65 6c65 6d65 6e74 7328 2920 696e  ui_elements() in
-00000390: 2067 7569 2e70 7929 0a20 2020 2069 2c01   gui.py).    i,.
-000003a0: 0000 679a 9999 9999 99b9 3fda 0173 5a0b  ..g.......?..sZ.
-000003b0: 5573 6572 5072 6f66 696c 65da 0744 6573  UserProfile..Des
-000003c0: 6b74 6f70 4e29 1272 0500 0000 7206 0000  ktopN).r....r...
-000003d0: 0072 0700 0000 da07 5f5f 646f 635f 5fda  .r......__doc__.
-000003e0: 036e 7366 da07 5072 6f70 5661 6cda 0369  .nsf..PropVal..i
-000003f0: 6e74 da0b 7265 7065 7469 7469 6f6e 73da  nt..repetitions.
-00000400: 0653 6369 5661 6cda 1374 696d 655f 7065  .SciVal..time_pe
-00000410: 725f 7265 7065 7469 7469 6f6e 7203 0000  r_repetitionr...
-00000420: 0072 0800 0000 da0a 6368 616e 6e65 6c5f  .r......channel_
-00000430: 6964 da07 7061 7468 6c69 62da 0450 6174  id..pathlib..Pat
-00000440: 68da 026f 73da 0667 6574 656e 765a 0973  h..os..getenvZ.s
-00000450: 6176 655f 7061 7468 7209 0000 0072 0900  ave_pathr....r..
-00000460: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
-00000470: 0012 0000 0073 0c00 0000 0800 0402 0e03  .....s..........
-00000480: 1201 1001 1e01 720b 0000 0063 0000 0000  ......r....c....
-00000490: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-000004a0: 4000 0000 7336 0000 0065 005a 0164 005a  @...s6...e.Z.d.Z
-000004b0: 0255 0064 015a 0365 04a0 05a1 005a 0665  .U.d.Z.e.....Z.e
-000004c0: 04a0 07a1 005a 0865 04a0 07a1 005a 0964  .....Z.e.....Z.d
-000004d0: 025a 0a65 0b65 0c64 033c 0064 0453 0029  .Z.e.e.d.<.d.S.)
-000004e0: 05da 0d4d 6f64 756c 6552 6573 756c 7473  ...ModuleResults
-000004f0: 7a6a 2054 6869 7320 636c 6173 7320 7361  zj This class sa
-00000500: 7665 7320 7468 6520 776f 726b 6572 206d  ves the worker m
-00000510: 6f64 756c 6520 7265 7375 6c74 2028 652e  odule result (e.
-00000520: 672e 3a20 6265 2072 6561 6420 6279 2067  g.: be read by g
-00000530: 7569 2065 6c65 6d65 6e74 7320 6c69 6b65  ui elements like
-00000540: 204e 5346 4368 6172 7420 6f72 2073 6176   NSFChart or sav
-00000550: 6564 2074 6f20 6669 6c65 2920 e9ff ffff  ed to file) ....
-00000560: ffda 0a6c 6173 745f 696e 6465 784e 290d  ...last_indexN).
-00000570: 7205 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
-00000580: 0e00 0000 720f 0000 00da 0953 6369 5374  ....r......SciSt
-00000590: 7265 616d da0b 6461 7461 5f73 7472 6561  ream..data_strea
-000005a0: 6d72 1300 0000 da0a 6d65 616e 5f76 616c  mr......mean_val
-000005b0: 7565 da0a 6c61 7374 5f76 616c 7565 721c  ue..last_valuer.
-000005c0: 0000 0072 1100 0000 da0f 5f5f 616e 6e6f  ...r......__anno
-000005d0: 7461 7469 6f6e 735f 5f72 0900 0000 7209  tations__r....r.
-000005e0: 0000 0072 0900 0000 720a 0000 0072 1a00  ...r....r....r..
-000005f0: 0000 1c00 0000 730c 0000 000a 0004 0208  ......s.........
-00000600: 0108 0108 0110 0172 1a00 0000 290d 720e  .......r....).r.
-00000610: 0000 00da 0465 6e75 6d72 1600 0000 7218  .....enumr....r.
-00000620: 0000 00da 0b64 6174 6163 6c61 7373 6573  .....dataclasses
-00000630: 7202 0000 00da 086e 616e 6f73 7572 6672  r......nanosurfr
-00000640: 0f00 0000 da07 496e 7445 6e75 6d72 0300  ......IntEnumr..
-00000650: 0000 da09 5072 6f70 5374 6f72 6572 0b00  ....PropStorer..
-00000660: 0000 721a 0000 0072 0900 0000 7209 0000  ..r....r....r...
-00000670: 0072 0900 0000 720a 0000 00da 083c 6d6f  .r....r......<mo
-00000680: 6475 6c65 3e01 0000 0073 1800 0000 0400  dule>....s......
-00000690: 0806 0801 0801 0c01 0801 0202 1201 0204  ................
-000006a0: 1401 0209 1401                           ......
+00000050: 6d05 5a05 0100 6401 6402 6c06 5a07 4700  m.Z...d.d.l.Z.G.
+00000060: 6404 6405 8400 6405 6501 6a08 8303 5a09  d.d...d.e.j...Z.
+00000070: 4700 6406 6407 8400 6407 6507 6a0a 8303  G.d.d...d.e.j...
+00000080: 5a0b 4700 6408 6409 8400 6409 8302 5a0c  Z.G.d.d...d...Z.
+00000090: 6402 5300 290a 7abc 2044 6566 696e 6573  d.S.).z. Defines
+000000a0: 2074 6865 2063 6f6e 6669 6775 7261 7469   the configurati
+000000b0: 6f6e 2076 616c 7565 7320 6f66 2074 6865  on values of the
+000000c0: 206d 6f64 756c 652e 0a20 2020 2056 616c   module..    Val
+000000d0: 7565 7320 696e 2074 6865 2050 726f 5374  ues in the ProSt
+000000e0: 6f72 6520 6172 6520 7361 7665 6420 616e  ore are saved an
+000000f0: 6420 6c6f 6164 6564 2064 7572 696e 6720  d loaded during 
+00000100: 6170 706c 6963 6174 696f 6e20 7374 6172  application star
+00000110: 7475 702f 7368 7574 646f 776e 2061 7574  tup/shutdown aut
+00000120: 6f6d 6174 6963 616c 6c79 0a43 6f70 7972  omatically.Copyr
+00000130: 6967 6874 204e 616e 6f73 7572 6620 4147  ight Nanosurf AG
+00000140: 2032 3032 310a 4c69 6365 6e73 6520 2d20   2021.License - 
+00000150: 4d49 540a e900 0000 004e 2901 da09 6461  MIT......N)...da
+00000160: 7461 636c 6173 7363 0000 0000 0000 0000  taclassc........
+00000170: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
+00000180: 7314 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
+00000190: 0364 025a 0464 0353 0029 04da 104d 6f6e  .d.Z.d.S.)...Mon
+000001a0: 6974 6f72 4368 616e 6e65 6c49 4429 0172  itorChannelID).r
+000001b0: 0100 0000 2901 e901 0000 004e 2905 da08  ....)......N)...
+000001c0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+000001d0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000001e0: 5f5f 5a0a 5573 6572 3149 6e70 7574 da0a  __Z.User1Input..
+000001f0: 4465 666c 6563 7469 6f6e a900 7209 0000  Deflection..r...
+00000200: 0072 0900 0000 fa3f 433a 5c47 6974 5c73  .r.....?C:\Git\s
+00000210: 6372 6970 7473 5f70 7974 686f 6e5f 6c69  cripts_python_li
+00000220: 625c 6e61 6e6f 7375 7266 5c61 7070 5c73  b\nanosurf\app\s
+00000230: 706d 5f74 656d 706c 6174 655c 7365 7474  pm_template\sett
+00000240: 696e 6773 2e70 7972 0300 0000 0e00 0000  ings.pyr........
+00000250: 7304 0000 0008 0104 0172 0300 0000 6300  s........r....c.
+00000260: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+00000270: 0000 0000 0000 0073 2600 0000 6500 5a01  .......s&...e.Z.
+00000280: 6400 5a02 6401 5a03 6402 6403 9c01 8700  d.Z.d.Z.d.d.....
+00000290: 6601 6404 6405 840c 5a04 8700 0400 5a05  f.d.d...Z.....Z.
+000002a0: 5300 2906 da08 5365 7474 696e 6773 7aad  S.)...Settingsz.
+000002b0: 2073 6574 7469 6e67 7320 6465 6669 6e65   settings define
+000002c0: 6420 6865 7265 2061 7320 5072 6f70 5661  d here as PropVa
+000002d0: 6c20 6172 6520 7374 6f72 6564 2070 6572  l are stored per
+000002e0: 7369 7374 656e 746c 7920 696e 2061 2069  sistently in a i
+000002f0: 6e69 2d66 696c 6520 0a20 2020 2020 2020  ni-file .       
+00000300: 2043 6f75 6c64 2062 6520 636f 6e6e 6563   Could be connec
+00000310: 7465 6420 616c 736f 2074 6f20 4755 4920  ted also to GUI 
+00000320: 656c 656d 656e 7473 2028 652e 672e 3a20  elements (e.g.: 
+00000330: 6c6f 6f6b 2069 6e74 6f20 6269 6e64 5f67  look into bind_g
+00000340: 7569 5f65 6c65 6d65 6e74 7328 2920 696e  ui_elements() in
+00000350: 2067 7569 2e70 7929 0a20 2020 204e a901   gui.py).    N..
+00000360: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
+00000370: 0000 0000 0001 0000 0007 0000 0003 0000  ................
+00000380: 0073 6000 0000 7400 8300 a001 a100 0100  .s`...t.........
+00000390: 7402 a003 7404 6401 8301 a101 7c00 5f05  t...t.d.....|._.
+000003a0: 7402 a003 7402 a006 6402 6403 a102 a101  t...t...d.d.....
+000003b0: 7c00 5f07 7402 a003 7404 7408 6a09 8301  |._.t...t.t.j...
+000003c0: a101 7c00 5f0a 7402 a003 740b a00c 740d  ..|._.t...t...t.
+000003d0: a00e 6404 a101 a101 6405 1b00 a101 7c00  ..d.....d.....|.
+000003e0: 5f0f 6400 5300 2906 4e69 2c01 0000 679a  _.d.S.).Ni,...g.
+000003f0: 9999 9999 99b9 3fda 0173 5a0b 5573 6572  ......?..sZ.User
+00000400: 5072 6f66 696c 65da 0744 6573 6b74 6f70  Profile..Desktop
+00000410: 2910 da05 7375 7065 72da 085f 5f69 6e69  )...super..__ini
+00000420: 745f 5fda 036e 7366 da07 5072 6f70 5661  t__..nsf..PropVa
+00000430: 6cda 0369 6e74 da0b 7265 7065 7469 7469  l..int..repetiti
+00000440: 6f6e 73da 0653 6369 5661 6cda 1374 696d  ons..SciVal..tim
+00000450: 655f 7065 725f 7265 7065 7469 7469 6f6e  e_per_repetition
+00000460: 7203 0000 0072 0800 0000 da0a 6368 616e  r....r......chan
+00000470: 6e65 6c5f 6964 da07 7061 7468 6c69 62da  nel_id..pathlib.
+00000480: 0450 6174 68da 026f 73da 0667 6574 656e  .Path..os..geten
+00000490: 765a 0973 6176 655f 7061 7468 a901 da04  vZ.save_path....
+000004a0: 7365 6c66 a901 da09 5f5f 636c 6173 735f  self....__class_
+000004b0: 5f72 0900 0000 720a 0000 0072 1100 0000  _r....r....r....
+000004c0: 1700 0000 730a 0000 0000 010a 0110 0114  ....s...........
+000004d0: 0112 017a 1153 6574 7469 6e67 732e 5f5f  ...z.Settings.__
+000004e0: 696e 6974 5f5f 2906 7205 0000 0072 0600  init__).r....r..
+000004f0: 0000 7207 0000 00da 075f 5f64 6f63 5f5f  ..r......__doc__
+00000500: 7211 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
+00000510: 6c6c 5f5f 7209 0000 0072 0900 0000 721f  ll__r....r....r.
+00000520: 0000 0072 0a00 0000 720b 0000 0013 0000  ...r....r.......
+00000530: 0073 0400 0000 0801 0403 720b 0000 0063  .s........r....c
+00000540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000550: 0300 0000 4000 0000 731e 0000 0065 005a  ....@...s....e.Z
+00000560: 0164 005a 0264 015a 0364 0264 039c 0164  .d.Z.d.Z.d.d...d
+00000570: 0464 0584 045a 0464 0253 0029 06da 0d4d  .d...Z.d.S.)...M
+00000580: 6f64 756c 6552 6573 756c 7473 7a6a 2054  oduleResultszj T
+00000590: 6869 7320 636c 6173 7320 7361 7665 7320  his class saves 
+000005a0: 7468 6520 776f 726b 6572 206d 6f64 756c  the worker modul
+000005b0: 6520 7265 7375 6c74 2028 652e 672e 3a20  e result (e.g.: 
+000005c0: 6265 2072 6561 6420 6279 2067 7569 2065  be read by gui e
+000005d0: 6c65 6d65 6e74 7320 6c69 6b65 204e 5346  lements like NSF
+000005e0: 4368 6172 7420 6f72 2073 6176 6564 2074  Chart or saved t
+000005f0: 6f20 6669 6c65 2920 4e72 0c00 0000 6301  o file) Nr....c.
+00000600: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00000610: 0000 0043 0000 0073 2800 0000 7400 a001  ...C...s(...t...
+00000620: a100 7c00 5f02 7400 a003 a100 7c00 5f04  ..|._.t.....|._.
+00000630: 7400 a003 a100 7c00 5f05 6401 7c00 5f06  t.....|._.d.|._.
+00000640: 6400 5300 2902 4ee9 ffff ffff 2907 7212  d.S.).N.....).r.
+00000650: 0000 00da 0953 6369 5374 7265 616d da0b  .....SciStream..
+00000660: 6461 7461 5f73 7472 6561 6d72 1600 0000  data_streamr....
+00000670: da0a 6d65 616e 5f76 616c 7565 da0a 6c61  ..mean_value..la
+00000680: 7374 5f76 616c 7565 da0a 6c61 7374 5f69  st_value..last_i
+00000690: 6e64 6578 721d 0000 0072 0900 0000 7209  ndexr....r....r.
+000006a0: 0000 0072 0a00 0000 7211 0000 0020 0000  ...r....r.... ..
+000006b0: 0073 0800 0000 0001 0a01 0a01 0a01 7a16  .s............z.
+000006c0: 4d6f 6475 6c65 5265 7375 6c74 732e 5f5f  ModuleResults.__
+000006d0: 696e 6974 5f5f 2905 7205 0000 0072 0600  init__).r....r..
+000006e0: 0000 7207 0000 0072 2100 0000 7211 0000  ..r....r!...r...
+000006f0: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
+00000700: 720a 0000 0072 2300 0000 1e00 0000 7304  r....r#.......s.
+00000710: 0000 0008 0104 0172 2300 0000 290d 7221  .......r#...).r!
+00000720: 0000 00da 0465 6e75 6d72 1900 0000 721b  .....enumr....r.
+00000730: 0000 00da 0b64 6174 6163 6c61 7373 6573  .....dataclasses
+00000740: 7202 0000 00da 086e 616e 6f73 7572 6672  r......nanosurfr
+00000750: 1200 0000 da07 496e 7445 6e75 6d72 0300  ......IntEnumr..
+00000760: 0000 da09 5072 6f70 5374 6f72 6572 0b00  ....PropStorer..
+00000770: 0000 7223 0000 0072 0900 0000 7209 0000  ..r#...r....r...
+00000780: 0072 0900 0000 720a 0000 00da 083c 6d6f  .r....r......<mo
+00000790: 6475 6c65 3e01 0000 0073 1000 0000 0406  dule>....s......
+000007a0: 0801 0801 0801 0c01 0803 1205 120b       ..............
```

### Comparing `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/worker.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/worker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/worker_task.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/app/spm_template/__pycache__/worker_task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/spm_template/gui.py` & `nanosurf-1.6.2/nanosurf/app/spm_template/gui.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/spm_template/main.py` & `nanosurf-1.6.2/nanosurf/app/spm_template/main.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/spm_template/measure_task.py` & `nanosurf-1.6.2/nanosurf/app/spm_template/measure_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 import nanosurf as nsf
 try:
     from nanosurf.lib.spm.studio.wrapper.cmd_tree_spm import Root, RootLu
 except ImportError: 
     pass
 import settings
 
-@dataclass
 class MeasureResult:
-    monitor_stream = nsf.SciStream()
-    last_index : int = -1
-    # add more or different results 
+    def __init__(self) -> None:
+        self.monitor_stream = nsf.SciStream()
+        self.last_index : int = -1
+        # add more or different results 
 
 class MeasureTask(nsf.frameworks.qt_app.nsf_thread.SPMWorker):
     """ This class implements the background measurement task using a Nanosurf SPM Controller  """
 
     """ Parameter for the background work with initial parameters. 
         Should be set to desired values by worker.start_background_task() """
     par_sample_points   = 10
```

### Comparing `nanosurf-1.6.1/nanosurf/app/spm_template/module.py` & `nanosurf-1.6.2/nanosurf/app/spm_template/module.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/app/spm_template/settings.py` & `nanosurf-1.6.2/nanosurf/app/spm_template/settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 import nanosurf as nsf
 
 """ Available monitoring channels defined by the worker task"""
 class MonitorChannelID(enum.IntEnum):
     User1Input = 0,
     Deflection = 1,
 
-@dataclass
+
 class Settings(nsf.PropStore):
     """ settings defined here as PropVal are stored persistently in a ini-file 
         Could be connected also to GUI elements (e.g.: look into bind_gui_elements() in gui.py)
     """
-    repetitions = nsf.PropVal(int(300))
-    time_per_repetition = nsf.PropVal(nsf.SciVal(0.1, "s"))
-    channel_id = nsf.PropVal(int(MonitorChannelID.Deflection))
-    save_path = nsf.PropVal(pathlib.Path(os.getenv(r"UserProfile")) / "Desktop")
+    def __init__(self) -> None:
+        super().__init__()
+        self.repetitions = nsf.PropVal(int(300))
+        self.time_per_repetition = nsf.PropVal(nsf.SciVal(0.1, "s"))
+        self.channel_id = nsf.PropVal(int(MonitorChannelID.Deflection))
+        self.save_path = nsf.PropVal(pathlib.Path(os.getenv(r"UserProfile")) / "Desktop")
 
-@dataclass
 class ModuleResults:
     """ This class saves the worker module result (e.g.: be read by gui elements like NSFChart or saved to file) """
-    data_stream = nsf.SciStream()
-    mean_value = nsf.SciVal()
-    last_value = nsf.SciVal()
-    last_index : int = -1
+    def __init__(self) -> None:
+        self.data_stream = nsf.SciStream()
+        self.mean_value = nsf.SciVal()
+        self.last_value = nsf.SciVal()
+        self.last_index : int = -1
```

### Comparing `nanosurf-1.6.1/nanosurf/doc/Nanosurf Python Library Overview.pdf` & `nanosurf-1.6.2/nanosurf/doc/Nanosurf Python Library Overview.pdf`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/doc/README.md` & `nanosurf-1.6.2/nanosurf/doc/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -131,14 +131,18 @@
 
 Full list of objects and methods can be found in the Scripting Manual
 in Nanosurf controller software under Help tab:
 Help -> Manuals -> Script Programmers Manual, or [here](https://www.nanosurf.com/downloads/programmers-manual.pdf).
 
 ## Library Version History
 
+* v1.6.2
+  * New: qt_app_framwork supports multi screen modules
+  * Bugfix: settings should not be of dataclass type
+
 * v1.6.1
   * Bugfix: pip packaging did not copy framework files
 
 * v1.6.0
   * New: spm_template: A new template to demonstrate simple connection to CX/Studio and measure some data
   * New: app_DriveAFM_Tip_Current_Addon this app controls the amplifier of the Tip-Current Addon
   * New: demo_move_sample_stage. This demo shows basic stage movements
```

### Comparing `nanosurf-1.6.1/nanosurf/lib/datatypes/prop_val.py` & `nanosurf-1.6.2/nanosurf/lib/datatypes/prop_val.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/datatypes/sci_channel.py` & `nanosurf-1.6.2/nanosurf/lib/datatypes/sci_channel.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/datatypes/sci_stream.py` & `nanosurf-1.6.2/nanosurf/lib/datatypes/sci_stream.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/datatypes/sci_val/__init__.py` & `nanosurf-1.6.2/nanosurf/lib/datatypes/sci_val/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/datatypes/sci_val/convert.py` & `nanosurf-1.6.2/nanosurf/lib/datatypes/sci_val/convert.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/datatypes/sci_val/unit_prefix.py` & `nanosurf-1.6.2/nanosurf/lib/datatypes/sci_val/unit_prefix.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/devices/accessory_interface/__init__.py` & `nanosurf-1.6.2/nanosurf/lib/devices/accessory_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/devices/i2c/bus_master.py` & `nanosurf-1.6.2/nanosurf/lib/devices/i2c/bus_master.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_24LC32A.py` & `nanosurf-1.6.2/nanosurf/lib/devices/i2c/chip_24LC32A.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_PCA9534.py` & `nanosurf-1.6.2/nanosurf/lib/devices/i2c/chip_PCA9534.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_TCN75.py` & `nanosurf-1.6.2/nanosurf/lib/devices/i2c/chip_TCN75.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_TMC5031.py` & `nanosurf-1.6.2/nanosurf/lib/devices/i2c/chip_TMC5031.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_TMP42x.py` & `nanosurf-1.6.2/nanosurf/lib/devices/i2c/chip_TMP42x.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/devices/trinamic_motor_controller.py` & `nanosurf-1.6.2/nanosurf/lib/devices/trinamic_motor_controller.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/app_base.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/app_base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/app_base.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/app_base.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 12:55:54 2023 UTC, .py size: 6750 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,467 +1,486 @@
-00000000: 610d 0d0a 0000 0000 5a4d 3964 5e1a 0000  a.......ZM9d^...
+00000000: 610d 0d0a 0000 0000 e003 5a64 b71b 0000  a.........Zd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 dc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6507 8300 7258 6401 6404  m.Z...e...rXd.d.
 00000070: 6c08 6d09 5a09 0100 6401 6405 6c0a 6d0b  l.m.Z...d.d.l.m.
 00000080: 5a0b 0100 6e18 6401 6404 6c0c 6d09 5a09  Z...n.d.d.l.m.Z.
 00000090: 0100 6401 6405 6c0d 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
 000000a0: 6402 6c0e 5a0f 6401 6406 6c10 6d11 5a11  d.l.Z.d.d.l.m.Z.
 000000b0: 0100 6401 6407 6c12 6d13 5a13 0100 6401  ..d.d.l.m.Z...d.
-000000c0: 6408 6c14 6d15 5a15 0100 6401 6409 6c16  d.l.m.Z...d.d.l.
-000000d0: 6d17 5a17 6d18 5a18 0100 640a 5a19 640b  m.Z.m.Z...d.Z.d.
-000000e0: 5a1a 4700 640c 640d 8400 640d 6517 8303  Z.G.d.d...d.e...
-000000f0: 5a1b 4700 640e 640f 8400 640f 6509 8303  Z.G.d.d...d.e...
-00000100: 5a1c 6402 5300 2910 7a62 2054 6865 2061  Z.d.S.).zb The a
-00000110: 7070 6c69 6361 7469 6f6e 2062 6173 6520  pplication base 
-00000120: 636c 6173 7320 6f66 2074 6865 2061 7070  class of the app
-00000130: 6c69 6361 7469 6f6e 2066 7261 6d65 776f  lication framewo
-00000140: 726b 0a43 6f70 7972 6967 6874 204e 616e  rk.Copyright Nan
-00000150: 6f73 7572 6620 4147 2032 3032 310a 4c69  osurf AG 2021.Li
-00000160: 6365 6e73 6520 2d20 4d49 540a e900 0000  cense - MIT.....
-00000170: 004e 2901 da22 696d 706f 7274 5f70 7973  .N).."import_pys
-00000180: 6964 6532 5f69 665f 6e6f 6e65 5f69 735f  ide2_if_none_is_
-00000190: 6465 7465 6374 6564 2901 da0c 5141 7070  detected)...QApp
-000001a0: 6c69 6361 7469 6f6e 2901 da09 5153 6574  lication)...QSet
-000001b0: 7469 6e67 7329 01da 0941 7070 5769 6e64  tings)...AppWind
-000001c0: 6f77 2901 da07 4d73 6754 7970 6529 01da  ow)...MsgType)..
-000001d0: 0a4d 6f64 756c 6542 6173 6529 02da 0950  .ModuleBase)...P
-000001e0: 726f 7053 746f 7265 da07 5072 6f70 5661  ropStore..PropVa
-000001f0: 6cda 036c 6f67 da06 636f 6e66 6967 6300  l..log..configc.
-00000200: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00000210: 0000 0040 0000 0073 2800 0000 6500 5a01  ...@...s(...e.Z.
-00000220: 6400 5a02 6503 6401 8301 5a04 6503 6401  d.Z.e.d...Z.e.d.
-00000230: 8301 5a05 6503 6506 6402 8301 8301 5a07  ..Z.e.e.d.....Z.
-00000240: 6403 5300 2904 da0b 4170 7053 6574 7469  d.S.)...AppSetti
-00000250: 6e67 7354 7201 0000 004e 2908 da08 5f5f  ngsTr....N)...__
-00000260: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000270: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000280: 7209 0000 00da 074c 6f67 6769 6e67 da10  r......Logging..
-00000290: 4c6f 6164 4c61 7374 5365 7474 696e 6773  LoadLastSettings
-000002a0: da03 696e 74da 1141 6374 6976 654d 6f64  ..int..ActiveMod
-000002b0: 756c 6549 6e64 6578 a900 7214 0000 0072  uleIndex..r....r
-000002c0: 1400 0000 fa44 633a 5c67 6974 5c73 6372  .....Dc:\git\scr
-000002d0: 6970 7473 5f70 7974 686f 6e5f 6c69 625c  ipts_python_lib\
-000002e0: 6e61 6e6f 7375 7266 5c6c 6962 5c66 7261  nanosurf\lib\fra
-000002f0: 6d65 776f 726b 735c 7174 5f61 7070 5c61  meworks\qt_app\a
-00000300: 7070 5f62 6173 652e 7079 720c 0000 001e  pp_base.pyr.....
-00000310: 0000 0073 0600 0000 0801 0801 0801 720c  ...s..........r.
-00000320: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000330: 0000 0000 0400 0000 0000 0000 730c 0100  ............s...
-00000340: 0065 005a 0164 005a 0265 0365 0365 046a  .e.Z.d.Z.e.e.e.j
-00000350: 0564 019c 0387 0066 0164 0264 0384 0c5a  .d.....f.d.d...Z
-00000360: 0664 0464 0584 005a 0764 0664 0784 005a  .d.d...Z.d.d...Z
-00000370: 0864 0864 0984 005a 0964 0a64 0b84 005a  .d.d...Z.d.d...Z
-00000380: 0a64 0c64 0d84 005a 0b65 0c64 0e9c 0164  .d.d...Z.e.d...d
-00000390: 0f64 1084 045a 0d65 0c64 0e9c 0164 1164  .d...Z.e.d...d.d
-000003a0: 1284 045a 0e65 04a0 0564 13a1 0166 0165  ...Z.e...d...f.e
-000003b0: 046a 0564 149c 0164 1564 1684 055a 0f65  .j.d...d.d...Z.e
-000003c0: 0364 179c 0164 1864 1984 045a 1065 0364  .d...d.d...Z.e.d
-000003d0: 179c 0164 1a64 1b84 045a 1165 0364 179c  ...d.d...Z.e.d..
-000003e0: 0164 1c64 1d84 045a 1264 1e64 1f84 005a  .d.d...Z.d.d...Z
-000003f0: 1365 146a 1566 0165 0365 1464 209c 0264  .e.j.f.e.e.d ..d
-00000400: 2164 2284 055a 1664 3165 0c65 0364 249c  !d"..Z.d1e.e.d$.
-00000410: 0264 2564 2684 055a 1765 1864 279c 0164  .d%d&..Z.e.d'..d
-00000420: 2864 2984 045a 1965 1864 2a9c 0164 2b64  (d)..Z.e.d*..d+d
-00000430: 2c84 045a 1a64 2d64 2e84 005a 1b64 2f64  ,..Z.d-d...Z.d/d
-00000440: 3084 005a 1c87 0004 005a 1d53 0029 32da  0..Z.....Z.S.)2.
-00000450: 0f41 7070 6c69 6361 7469 6f6e 4261 7365  .ApplicationBase
-00000460: 2903 da07 636f 6d70 616e 79da 0e61 7070  )...company..app
-00000470: 5f6e 616d 655f 7368 6f72 74da 096d 6169  _name_short..mai
-00000480: 6e5f 7061 7468 6304 0000 0000 0000 0000  n_pathc.........
-00000490: 0000 0006 0000 0005 0000 000f 0000 0073  ...............s
-000004a0: f600 0000 7400 8300 6a01 7c04 6900 7c05  ....t...j.|.i.|.
-000004b0: a401 8e01 0100 7c01 7c00 5f02 7c02 7c00  ......|.|._.|.|.
-000004c0: 5f03 7c02 a004 6401 6402 a102 7c00 5f05  _.|...d.d...|._.
-000004d0: 7406 6a07 6a08 a009 7c02 a101 0100 740a  t.j.j...|.....t.
-000004e0: 740b 6403 6404 6405 8400 8303 8300 6400  t.d.d.d.......d.
-000004f0: 7501 7c00 5f0c 740d 7c00 6a02 7c00 6a05  u.|._.t.|.j.|.j.
-00000500: 8302 7c00 5f0e 740f a010 7c03 a101 6a11  ..|._.t...|...j.
-00000510: 7c00 5f12 740f a010 7413 6a14 a015 7416  |._.t...t.j...t.
-00000520: a101 a101 6a11 7c00 5f17 740f a010 7413  ....j.|._.t...t.
-00000530: 6a14 a018 6406 a101 a101 740f a010 7c00  j...d.....t...|.
-00000540: 6a02 a101 1b00 740f a010 7c00 6a05 a101  j.....t...|.j...
-00000550: 1b00 7c00 5f19 7c00 6a19 741a 1b00 7c00  ..|._.|.j.t...|.
-00000560: 5f1b 7c00 6a19 741c 1b00 7c00 5f1d 7c00  _.|.j.t...|._.|.
-00000570: 6a1d 6407 1b00 7c00 5f1e 6408 7c00 5f1f  j.d...|._.d.|._.
-00000580: 7c00 6a17 7c00 5f20 7421 8300 7c00 5f22  |.j.|._ t!..|._"
-00000590: 6900 7c00 5f23 6400 5300 2909 4efa 0120  i.|._#d.S.).N.. 
-000005a0: da01 5fda 0867 6574 7472 6163 6563 0000  .._..gettracec..
-000005b0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-000005c0: 0000 5300 0000 7304 0000 0064 0053 00a9  ..S...s....d.S..
-000005d0: 014e 7214 0000 0072 1400 0000 7214 0000  .Nr....r....r...
-000005e0: 0072 1400 0000 7215 0000 00da 083c 6c61  .r....r......<la
-000005f0: 6d62 6461 3e2a 0000 00f3 0000 0000 7a2a  mbda>*........z*
-00000600: 4170 706c 6963 6174 696f 6e42 6173 652e  ApplicationBase.
-00000610: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
-00000620: 3e2e 3c6c 616d 6264 613e 7a0e 254c 4f43  >.<lambda>z.%LOC
-00000630: 414c 4150 5044 4154 4125 7a0f 6c61 7374  ALAPPDATA%z.last
-00000640: 5f63 6f6e 6669 672e 696e 69da 0b41 7070  _config.ini..App
-00000650: 6c69 6361 7469 6f6e 2924 da05 7375 7065  lication)$..supe
-00000660: 72da 085f 5f69 6e69 745f 5f72 1700 0000  r..__init__r....
-00000670: 5a0d 6170 705f 6e61 6d65 5f6c 6f6e 67da  Z.app_name_long.
-00000680: 0772 6570 6c61 6365 da08 6170 705f 6e61  .replace..app_na
-00000690: 6d65 da06 6374 7970 6573 da06 7769 6e64  me..ctypes..wind
-000006a0: 6c6c da07 7368 656c 6c33 325a 2753 6574  ll..shell32Z'Set
-000006b0: 4375 7272 656e 7450 726f 6365 7373 4578  CurrentProcessEx
-000006c0: 706c 6963 6974 4170 7055 7365 724d 6f64  plicitAppUserMod
-000006d0: 656c 4944 da07 6765 7461 7474 72da 0373  elID..getattr..s
-000006e0: 7973 da14 6973 5f69 6e5f 6465 6275 6767  ys..is_in_debugg
-000006f0: 696e 675f 6d6f 6465 7204 0000 00da 0872  ing_moder......r
-00000700: 6567 6973 7472 79da 0770 6174 686c 6962  egistry..pathlib
-00000710: da04 5061 7468 da06 7061 7265 6e74 7219  ..Path..parentr.
-00000720: 0000 00da 026f 73da 0470 6174 68da 0761  .....os..path..a
-00000730: 6273 7061 7468 da08 5f5f 6669 6c65 5f5f  bspath..__file__
-00000740: 5a0e 6672 616d 6577 6f72 6b5f 7061 7468  Z.framework_path
-00000750: da0a 6578 7061 6e64 7661 7273 5a0d 6170  ..expandvarsZ.ap
-00000760: 705f 6461 7461 5f70 6174 68da 0c64 6972  p_data_path..dir
-00000770: 5f6e 616d 655f 6c6f 67da 086c 6f67 5f70  _name_log..log_p
-00000780: 6174 68da 0f64 6972 5f6e 616d 655f 636f  ath..dir_name_co
-00000790: 6e66 6967 da0b 636f 6e66 6967 5f70 6174  nfig..config_pat
-000007a0: 68da 0b63 6f6e 6669 675f 6669 6c65 da0e  h..config_file..
-000007b0: 636f 6e66 6967 5f73 6563 7469 6f6e da0d  config_section..
-000007c0: 7265 736f 7572 6365 5f70 6174 6872 0c00  resource_pathr..
-000007d0: 0000 da08 7365 7474 696e 6773 da07 6d6f  ....settings..mo
-000007e0: 6475 6c65 7329 06da 0473 656c 6672 1700  dules)...selfr..
-000007f0: 0000 7218 0000 0072 1900 0000 da04 6172  ..r....r......ar
-00000800: 6773 da06 6b77 6172 6773 a901 da09 5f5f  gs..kwargs....__
-00000810: 636c 6173 735f 5f72 1400 0000 7215 0000  class__r....r...
-00000820: 0072 2200 0000 2400 0000 7322 0000 0000  .r"...$...s"....
-00000830: 0112 0106 0106 010e 010e 0118 0310 030e  ................
-00000840: 0116 012c 010c 010c 010c 0306 0108 0108  ...,............
-00000850: 017a 1841 7070 6c69 6361 7469 6f6e 4261  .z.ApplicationBa
-00000860: 7365 2e5f 5f69 6e69 745f 5f63 0100 0000  se.__init__c....
-00000870: 0000 0000 0000 0000 0100 0000 0500 0000  ................
-00000880: 4300 0000 7394 0000 0074 006a 016a 02a0  C...s....t.j.j..
-00000890: 037c 006a 04a1 0101 0074 006a 056a 06a0  .|.j.....t.j.j..
-000008a0: 077c 006a 087c 006a 097c 006a 0aa1 0301  .|.j.|.j.|.j....
-000008b0: 007c 00a0 0ba1 0001 0074 0c7c 0083 017c  .|.......t.|...|
-000008c0: 005f 0d7c 006a 0da0 0e7c 006a 0f64 011b  ._.|.j...|.j.d..
-000008d0: 007c 006a 0f64 021b 00a1 0201 007c 006a  .|.j.d.......|.j
-000008e0: 10a0 117c 006a 12a1 0101 007c 00a0 13a1  ...|.j.....|....
-000008f0: 0001 007c 00a0 147c 006a 086a 156a 16a1  ...|...|.j.j.j..
-00000900: 0101 007c 006a 0da0 17a1 0001 007c 006a  ...|.j.......|.j
-00000910: 18a0 1964 03a1 0101 0064 0053 0029 044e  ...d.....d.S.).N
-00000920: 7a12 6170 705f 7374 796c 6573 6865 6574  z.app_stylesheet
-00000930: 2e71 7373 7a0c 6170 705f 6963 6f6e 2e69  .qssz.app_icon.i
-00000940: 636f 7a0e 4170 7020 7275 6e6e 696e 672e  coz.App running.
-00000950: 2e2e 291a da03 6e73 66da 0475 7469 6cda  ..)...nsf..util.
-00000960: 0866 696c 6575 7469 6cda 0d63 7265 6174  .fileutil..creat
-00000970: 655f 666f 6c64 6572 7237 0000 00da 0964  e_folderr7.....d
-00000980: 6174 6174 7970 6573 da08 7072 6f70 5f76  atatypes..prop_v
-00000990: 616c da12 6c6f 6164 5f66 726f 6d5f 696e  al..load_from_in
-000009a0: 695f 6669 6c65 723b 0000 0072 3800 0000  i_filer;...r8...
-000009b0: 7239 0000 00da 0c73 6574 7570 5f6c 6f67  r9.....setup_log
-000009c0: 6765 7272 0500 0000 da09 6170 7077 696e  gerr......appwin
-000009d0: 646f 775a 0a63 7265 6174 655f 6775 6972  dowZ.create_guir
-000009e0: 3a00 0000 da10 6c61 7374 5769 6e64 6f77  :.....lastWindow
-000009f0: 436c 6f73 6564 da07 636f 6e6e 6563 74da  Closed..connect.
-00000a00: 0871 7569 745f 6170 70da 0a64 6f5f 7374  .quit_app..do_st
-00000a10: 6172 7475 70da 0f61 6374 6976 6174 655f  artup..activate_
-00000a20: 6d6f 6475 6c65 7213 0000 00da 0576 616c  moduler......val
-00000a30: 7565 da04 7368 6f77 da06 6c6f 6767 6572  ue..show..logger
-00000a40: da04 696e 666f a901 723d 0000 0072 1400  ..info..r=...r..
-00000a50: 0000 7214 0000 0072 1500 0000 da09 7374  ..r....r......st
-00000a60: 6172 745f 6170 703d 0000 0073 1400 0000  art_app=...s....
-00000a70: 0001 1001 1801 0801 0a01 1a01 0e01 0801  ................
-00000a80: 1001 0a01 7a19 4170 706c 6963 6174 696f  ....z.Applicatio
-00000a90: 6e42 6173 652e 7374 6172 745f 6170 7063  nBase.start_appc
-00000aa0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000ab0: 0500 0000 4300 0000 732c 0000 007c 00a0  ....C...s,...|..
-00000ac0: 00a1 0001 007c 00a0 01a1 0001 0074 026a  .....|.......t.j
-00000ad0: 036a 04a0 057c 006a 067c 006a 077c 006a  .j...|.j.|.j.|.j
-00000ae0: 08a1 0301 0064 0053 0072 1d00 0000 2909  .....d.S.r....).
-00000af0: da0c 7374 6f70 5f6d 6f64 756c 6573 da0b  ..stop_modules..
-00000b00: 646f 5f73 6875 7464 6f77 6e72 4200 0000  do_shutdownrB...
-00000b10: 7246 0000 0072 4700 0000 da10 7361 7665  rF...rG.....save
-00000b20: 5f74 6f5f 696e 695f 6669 6c65 723b 0000  _to_ini_filer;..
-00000b30: 0072 3800 0000 7239 0000 0072 5400 0000  .r8...r9...rT...
-00000b40: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
-00000b50: 4d00 0000 4900 0000 7306 0000 0000 0108  M...I...s.......
-00000b60: 0108 017a 1841 7070 6c69 6361 7469 6f6e  ...z.Application
-00000b70: 4261 7365 2e71 7569 745f 6170 7063 0100  Base.quit_appc..
-00000b80: 0000 0000 0000 0000 0000 0100 0000 0600  ................
-00000b90: 0000 4300 0000 7326 0000 0074 0064 017c  ..C...s&...t.d.|
-00000ba0: 006a 016a 029b 0064 0274 03a0 04a1 006a  .j.j...d.t.....j
-00000bb0: 056a 069b 0064 039d 0583 0182 0164 0053  .j...d.......d.S
-00000bc0: 0029 044e 7a0d 5375 6263 6c61 7373 206f  .).Nz.Subclass o
-00000bd0: 6620 277a 1427 2068 6173 2074 6f20 696d  f 'z.' has to im
-00000be0: 706c 656d 656e 7420 277a 0328 2927 2907  plement 'z.()').
-00000bf0: da13 4e6f 7449 6d70 6c65 6d65 6e74 6564  ..NotImplemented
-00000c00: 4572 726f 7272 4100 0000 720d 0000 0072  ErrorrA...r....r
-00000c10: 2900 0000 da09 5f67 6574 6672 616d 65da  )....._getframe.
-00000c20: 0666 5f63 6f64 65da 0763 6f5f 6e61 6d65  .f_code..co_name
-00000c30: 7254 0000 0072 1400 0000 7214 0000 0072  rT...r....r....r
-00000c40: 1500 0000 724e 0000 004e 0000 0073 0200  ....rN...N...s..
-00000c50: 0000 0001 7a1a 4170 706c 6963 6174 696f  ....z.Applicatio
-00000c60: 6e42 6173 652e 646f 5f73 7461 7274 7570  nBase.do_startup
-00000c70: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000c80: 0001 0000 0043 0000 0073 0400 0000 6400  .....C...s....d.
-00000c90: 5300 721d 0000 0072 1400 0000 7254 0000  S.r....r....rT..
-00000ca0: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
-00000cb0: 7257 0000 0051 0000 0073 0200 0000 0001  rW...Q...s......
-00000cc0: 7a1b 4170 706c 6963 6174 696f 6e42 6173  z.ApplicationBas
-00000cd0: 652e 646f 5f73 6875 7464 6f77 6e63 0100  e.do_shutdownc..
-00000ce0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000cf0: 0000 4300 0000 731c 0000 0074 0083 0072  ..C...s....t...r
-00000d00: 107c 00a0 01a1 0001 006e 087c 00a0 02a1  .|.......n.|....
-00000d10: 0001 0064 0053 0072 1d00 0000 2903 7202  ...d.S.r....).r.
-00000d20: 0000 00da 0565 7865 635f da04 6578 6563  .....exec_..exec
-00000d30: 7254 0000 0072 1400 0000 7214 0000 0072  rT...r....r....r
-00000d40: 1500 0000 da07 6578 6563 7574 6554 0000  ......executeT..
-00000d50: 0073 0600 0000 0001 0601 0a02 7a17 4170  .s..........z.Ap
-00000d60: 706c 6963 6174 696f 6e42 6173 652e 6578  plicationBase.ex
-00000d70: 6563 7574 6529 01da 066d 6f64 756c 6563  ecute)...modulec
-00000d80: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000d90: 0500 0000 4300 0000 7328 0000 0074 007c  ....C...s(...t.|
-00000da0: 016a 0174 0283 0272 2474 036a 046a 05a0  .j.t...r$t.j.j..
-00000db0: 067c 016a 017c 006a 077c 016a 08a1 0301  .|.j.|.j.|.j....
-00000dc0: 0064 0053 0072 1d00 0000 2909 da0a 6973  .d.S.r....)...is
-00000dd0: 696e 7374 616e 6365 723b 0000 0072 0800  instancer;...r..
-00000de0: 0000 7242 0000 0072 4600 0000 7247 0000  ..rB...rF...rG..
-00000df0: 0072 5800 0000 7238 0000 00da 046e 616d  .rX...r8.....nam
-00000e00: 65a9 0272 3d00 0000 7260 0000 0072 1400  e..r=...r`...r..
-00000e10: 0000 7214 0000 0072 1500 0000 da0d 7361  ..r....r......sa
-00000e20: 7665 5f73 6574 7469 6e67 735a 0000 0073  ve_settingsZ...s
-00000e30: 0400 0000 0001 0c01 7a1d 4170 706c 6963  ........z.Applic
-00000e40: 6174 696f 6e42 6173 652e 7361 7665 5f73  ationBase.save_s
-00000e50: 6574 7469 6e67 7363 0200 0000 0000 0000  ettingsc........
-00000e60: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
-00000e70: 7332 0000 0074 007c 016a 0174 0283 0272  s2...t.|.j.t...r
-00000e80: 2e7c 006a 016a 036a 0472 2e74 056a 066a  .|.j.j.j.r.t.j.j
-00000e90: 07a0 087c 016a 017c 006a 097c 016a 0aa1  ...|.j.|.j.|.j..
-00000ea0: 0301 0064 0053 0072 1d00 0000 290b 7261  ...d.S.r....).ra
-00000eb0: 0000 0072 3b00 0000 7208 0000 0072 1100  ...r;...r....r..
-00000ec0: 0000 7250 0000 0072 4200 0000 7246 0000  ..rP...rB...rF..
-00000ed0: 0072 4700 0000 7248 0000 0072 3800 0000  .rG...rH...r8...
-00000ee0: 7262 0000 0072 6300 0000 7214 0000 0072  rb...rc...r....r
-00000ef0: 1400 0000 7215 0000 00da 0d6c 6f61 645f  ....r......load_
-00000f00: 7365 7474 696e 6773 5e00 0000 7306 0000  settings^...s...
-00000f10: 0000 010c 010a 017a 1d41 7070 6c69 6361  .......z.Applica
-00000f20: 7469 6f6e 4261 7365 2e6c 6f61 645f 7365  tionBase.load_se
-00000f30: 7474 696e 6773 7a0a 6c61 7465 7374 2e6c  ttingsz.latest.l
-00000f40: 6f67 2901 da07 6c6f 6766 696c 6563 0200  og)...logfilec..
-00000f50: 0000 0000 0000 0000 0000 0500 0000 0700  ................
-00000f60: 0000 4300 0000 7394 0000 007c 006a 006a  ..C...s....|.j.j
-00000f70: 016a 0272 7674 036a 046a 05a0 067c 006a  .j.rvt.j.j...|.j
-00000f80: 07a1 0101 0074 087c 006a 077c 011b 0083  .....t.|.j.|....
-00000f90: 017d 0274 096a 0a74 096a 0b64 0164 027c  .}.t.j.t.j.d.d.|
-00000fa0: 0264 0364 048d 0501 0074 09a0 0ca1 007d  .d.d.....t.....}
-00000fb0: 037c 03a0 0d74 096a 0ea1 0101 0074 09a0  .|...t.j.....t..
-00000fc0: 0f64 05a1 017d 047c 03a0 107c 04a1 0101  .d...}.|...|....
-00000fd0: 0074 09a0 1164 06a1 01a0 127c 03a1 0101  .t...d.....|....
-00000fe0: 0074 09a0 1164 07a1 017c 005f 137c 006a  .t...d...|._.|.j
-00000ff0: 13a0 0d74 096a 0ba1 0101 0064 0853 0029  ...t.j.....d.S.)
-00001000: 097a cf0a 2020 2020 2020 2020 5365 7475  .z..        Setu
-00001010: 7020 4c6f 6767 6572 2069 6620 6e65 6564  p Logger if need
-00001020: 6564 2061 6e64 2064 6966 6665 7220 6265  ed and differ be
-00001030: 7477 6565 6e20 636f 6e73 6f6c 2061 6e64  tween consol and
-00001040: 2066 696c 6520 6f75 7470 7574 0a20 2020   file output.   
-00001050: 2020 2020 2073 6574 2075 7020 6c6f 6767       set up logg
-00001060: 696e 6720 746f 2066 696c 6520 616e 6420  ing to file and 
-00001070: 6368 6f6f 7365 206c 6f67 6765 7220 6c65  choose logger le
-00001080: 7665 6c20 2866 726f 6d20 6869 6768 6573  vel (from highes
-00001090: 7420 6c65 7665 6c20 746f 206c 6f77 6573  t level to lowes
-000010a0: 743a 2044 6562 7567 2c20 696e 666f 2c20  t: Debug, info, 
-000010b0: 7761 726e 696e 672c 2065 7272 6f72 2c20  warning, error, 
-000010c0: 6372 6974 6963 616c 290a 2020 2020 2020  critical).      
-000010d0: 2020 7a33 2528 6173 6374 696d 6529 7320    z3%(asctime)s 
-000010e0: 2528 6e61 6d65 292d 3132 7320 2528 6c65  %(name)-12s %(le
-000010f0: 7665 6c6e 616d 6529 2d38 7320 2528 6d65  velname)-8s %(me
-00001100: 7373 6167 6529 737a 0e25 6d2d 2564 2025  ssage)sz.%m-%d %
-00001110: 483a 254d 3a25 53da 0177 2905 da05 6c65  H:%M:%S..w)...le
-00001120: 7665 6cda 0666 6f72 6d61 74da 0764 6174  vel..format..dat
-00001130: 6566 6d74 da08 6669 6c65 6e61 6d65 da08  efmt..filename..
-00001140: 6669 6c65 6d6f 6465 7a27 2528 6e61 6d65  filemodez'%(name
-00001150: 292d 3132 7320 2528 6c65 7665 6c6e 616d  )-12s %(levelnam
-00001160: 6529 2d38 7320 2528 6d65 7373 6167 6529  e)-8s %(message)
-00001170: 73da 0072 2000 0000 4e29 1472 3b00 0000  s..r ...N).r;...
-00001180: 7210 0000 0072 5000 0000 7242 0000 0072  r....rP...rB...r
-00001190: 4300 0000 7244 0000 0072 4500 0000 7235  C...rD...rE...r5
-000011a0: 0000 00da 0373 7472 da07 6c6f 6767 696e  .....str..loggin
-000011b0: 67da 0b62 6173 6963 436f 6e66 6967 da05  g..basicConfig..
-000011c0: 4445 4255 47da 0d53 7472 6561 6d48 616e  DEBUG..StreamHan
-000011d0: 646c 6572 da08 7365 744c 6576 656c da04  dler..setLevel..
-000011e0: 494e 464f da09 466f 726d 6174 7465 72da  INFO..Formatter.
-000011f0: 0c73 6574 466f 726d 6174 7465 72da 0967  .setFormatter..g
-00001200: 6574 4c6f 6767 6572 da0a 6164 6448 616e  etLogger..addHan
-00001210: 646c 6572 7252 0000 0029 0572 3d00 0000  dlerrR...).r=...
-00001220: 7266 0000 005a 0b6c 6f67 6669 6c65 7061  rf...Z.logfilepa
-00001230: 7468 da07 636f 6e73 6f6c 65da 0966 6f72  th..console..for
-00001240: 6d61 7474 6572 7214 0000 0072 1400 0000  matterr....r....
-00001250: 7215 0000 0072 4900 0000 6300 0000 7320  r....rI...c...s 
-00001260: 0000 0000 050a 0110 010e 0108 0102 0102  ................
-00001270: 0102 0102 fc06 0508 010c 010a 010a 0110  ................
-00001280: 010c 017a 1c41 7070 6c69 6361 7469 6f6e  ...z.Application
-00001290: 4261 7365 2e73 6574 7570 5f6c 6f67 6765  Base.setup_logge
-000012a0: 7229 01da 036d 7367 6302 0000 0000 0000  r)...msgc.......
-000012b0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-000012c0: 0073 1200 0000 7c00 a000 7c01 7401 6a02  .s....|...|.t.j.
-000012d0: a102 0100 6400 5300 721d 0000 0029 03da  ....d.S.r....)..
-000012e0: 0c73 686f 775f 6d65 7373 6167 6572 0600  .show_messager..
-000012f0: 0000 da05 4572 726f 72a9 0272 3d00 0000  ....Error..r=...
-00001300: 727b 0000 0072 1400 0000 7214 0000 0072  r{...r....r....r
-00001310: 1500 0000 da12 7368 6f77 5f65 7272 6f72  ......show_error
-00001320: 5f6d 6573 7361 6765 7800 0000 7302 0000  _messagex...s...
-00001330: 0000 017a 2241 7070 6c69 6361 7469 6f6e  ...z"Application
-00001340: 4261 7365 2e73 686f 775f 6572 726f 725f  Base.show_error_
-00001350: 6d65 7373 6167 6563 0200 0000 0000 0000  messagec........
-00001360: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00001370: 7312 0000 007c 00a0 007c 0174 016a 02a1  s....|...|.t.j..
-00001380: 0201 0064 0053 0072 1d00 0000 2903 727c  ...d.S.r....).r|
-00001390: 0000 0072 0600 0000 5a04 5761 726e 727e  ...r....Z.Warnr~
-000013a0: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
-000013b0: 0000 da11 7368 6f77 5f77 6172 6e5f 6d65  ....show_warn_me
-000013c0: 7373 6167 657b 0000 0073 0200 0000 0001  ssage{...s......
-000013d0: 7a21 4170 706c 6963 6174 696f 6e42 6173  z!ApplicationBas
-000013e0: 652e 7368 6f77 5f77 6172 6e5f 6d65 7373  e.show_warn_mess
-000013f0: 6167 6563 0200 0000 0000 0000 0000 0000  agec............
-00001400: 0200 0000 0400 0000 4300 0000 7312 0000  ........C...s...
-00001410: 007c 00a0 007c 0174 016a 02a1 0201 0064  .|...|.t.j.....d
-00001420: 0053 0072 1d00 0000 2903 727c 0000 0072  .S.r....).r|...r
-00001430: 0600 0000 da04 496e 666f 727e 0000 0072  ......Infor~...r
-00001440: 1400 0000 7214 0000 0072 1500 0000 da11  ....r....r......
-00001450: 7368 6f77 5f69 6e66 6f5f 6d65 7373 6167  show_info_messag
-00001460: 657e 0000 0073 0200 0000 0001 7a21 4170  e~...s......z!Ap
-00001470: 706c 6963 6174 696f 6e42 6173 652e 7368  plicationBase.sh
-00001480: 6f77 5f69 6e66 6f5f 6d65 7373 6167 6563  ow_info_messagec
-00001490: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000014a0: 0200 0000 4300 0000 730e 0000 007c 006a  ....C...s....|.j
-000014b0: 00a0 01a1 0001 0064 0053 0072 1d00 0000  .......d.S.r....
-000014c0: 2902 724a 0000 005a 0c68 6964 655f 6d65  ).rJ...Z.hide_me
-000014d0: 7373 6167 6572 5400 0000 7214 0000 0072  ssagerT...r....r
-000014e0: 1400 0000 7215 0000 00da 0d63 6c65 6172  ....r......clear
-000014f0: 5f6d 6573 7361 6765 8100 0000 7302 0000  _message....s...
-00001500: 0000 017a 1d41 7070 6c69 6361 7469 6f6e  ...z.Application
-00001510: 4261 7365 2e63 6c65 6172 5f6d 6573 7361  Base.clear_messa
-00001520: 6765 2902 727b 0000 00da 086d 7367 5f74  ge).r{.....msg_t
-00001530: 7970 6563 0300 0000 0000 0000 0000 0000  ypec............
-00001540: 0300 0000 0400 0000 4300 0000 7312 0000  ........C...s...
-00001550: 007c 006a 00a0 017c 017c 02a1 0201 0064  .|.j...|.|.....d
-00001560: 0053 0072 1d00 0000 2902 724a 0000 0072  .S.r....).rJ...r
-00001570: 7c00 0000 2903 723d 0000 0072 7b00 0000  |...).r=...r{...
-00001580: 7284 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
-00001590: 1500 0000 727c 0000 0084 0000 0073 0200  ....r|.......s..
-000015a0: 0000 0001 7a1c 4170 706c 6963 6174 696f  ....z.Applicatio
-000015b0: 6e42 6173 652e 7368 6f77 5f6d 6573 7361  nBase.show_messa
-000015c0: 6765 da06 4d6f 6475 6c65 2902 da0a 6e65  ge..Module)...ne
-000015d0: 775f 6d6f 6475 6c65 7262 0000 0063 0300  w_modulerb...c..
-000015e0: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-000015f0: 0000 4300 0000 734c 0000 007c 027c 015f  ..C...sL...|.|._
-00001600: 007c 006a 01a0 0264 017c 016a 009b 009d  .|.j...d.|.j....
-00001610: 02a1 0101 007c 017c 006a 037c 016a 003c  .....|.|.j.|.j.<
-00001620: 007c 01a0 04a1 0001 007c 006a 05a0 067c  .|.......|.j...|
-00001630: 01a1 0101 007c 006a 05a0 077c 006a 03a1  .....|.j...|.j..
-00001640: 0101 0064 0053 0029 024e 7a0e 5374 6172  ...d.S.).Nz.Star
-00001650: 7420 6d6f 6475 6c65 3a20 2908 7262 0000  t module: ).rb..
-00001660: 0072 5200 0000 7253 0000 0072 3c00 0000  .rR...rS...r<...
-00001670: da05 7374 6172 7472 4a00 0000 5a0a 6164  ..startrJ...Z.ad
-00001680: 645f 7363 7265 656e 5a0b 7570 6461 7465  d_screenZ.update
-00001690: 5f6d 656e 7529 0372 3d00 0000 7286 0000  _menu).r=...r...
-000016a0: 0072 6200 0000 7214 0000 0072 1400 0000  .rb...r....r....
-000016b0: 7215 0000 00da 0a61 6464 5f6d 6f64 756c  r......add_modul
-000016c0: 6587 0000 0073 0c00 0000 0001 0601 1401  e....s..........
-000016d0: 0c01 0801 0c01 7a1a 4170 706c 6963 6174  ......z.Applicat
-000016e0: 696f 6e42 6173 652e 6164 645f 6d6f 6475  ionBase.add_modu
-000016f0: 6c65 2901 da06 7265 7475 726e 6301 0000  le)...returnc...
-00001700: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00001710: 0043 0000 0073 0a00 0000 7400 7c00 6a01  .C...s....t.|.j.
-00001720: 8301 5300 721d 0000 0029 02da 036c 656e  ..S.r....)...len
-00001730: 723c 0000 0072 5400 0000 7214 0000 0072  r<...rT...r....r
-00001740: 1400 0000 7215 0000 00da 1067 6574 5f6d  ....r......get_m
-00001750: 6f64 756c 655f 636f 756e 748f 0000 0073  odule_count....s
-00001760: 0200 0000 0001 7a20 4170 706c 6963 6174  ......z Applicat
-00001770: 696f 6e42 6173 652e 6765 745f 6d6f 6475  ionBase.get_modu
-00001780: 6c65 5f63 6f75 6e74 2901 da0c 6d6f 6475  le_count)...modu
-00001790: 6c65 5f69 6e64 6578 6302 0000 0000 0000  le_indexc.......
-000017a0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-000017b0: 0073 1a00 0000 7c01 7c00 6a00 6a01 5f02  .s....|.|.j.j._.
-000017c0: 7c00 6a03 a004 7c01 a101 0100 6400 5300  |.j...|.....d.S.
-000017d0: 721d 0000 0029 0572 3b00 0000 7213 0000  r....).r;...r...
-000017e0: 0072 5000 0000 724a 0000 005a 1a73 6574  .rP...rJ...Z.set
-000017f0: 5f61 6374 6976 655f 6d6f 6475 6c65 5f62  _active_module_b
-00001800: 795f 696e 6465 7829 0272 3d00 0000 728c  y_index).r=...r.
-00001810: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
-00001820: 0000 724f 0000 0092 0000 0073 0400 0000  ..rO.......s....
-00001830: 0001 0a01 7a1f 4170 706c 6963 6174 696f  ....z.Applicatio
-00001840: 6e42 6173 652e 6163 7469 7661 7465 5f6d  nBase.activate_m
-00001850: 6f64 756c 6563 0100 0000 0000 0000 0000  odulec..........
-00001860: 0000 0200 0000 0500 0000 4300 0000 7330  ..........C...s0
-00001870: 0000 007c 006a 00a0 01a1 0044 005d 207d  ...|.j.....D.] }
-00001880: 017c 006a 02a0 0364 017c 016a 049b 009d  .|.j...d.|.j....
-00001890: 02a1 0101 007c 01a0 05a1 0001 0071 0a64  .....|.......q.d
-000018a0: 0053 0029 024e 7a0d 5374 6f70 206d 6f64  .S.).Nz.Stop mod
-000018b0: 756c 653a 2029 0672 3c00 0000 da06 7661  ule: ).r<.....va
-000018c0: 6c75 6573 7252 0000 0072 5300 0000 7262  luesrR...rS...rb
-000018d0: 0000 00da 0473 746f 7029 0272 3d00 0000  .....stop).r=...
-000018e0: da03 6d6f 6472 1400 0000 7214 0000 0072  ..modr....r....r
-000018f0: 1500 0000 7256 0000 0096 0000 0073 0600  ....rV.......s..
-00001900: 0000 0001 0e01 1401 7a1c 4170 706c 6963  ........z.Applic
-00001910: 6174 696f 6e42 6173 652e 7374 6f70 5f6d  ationBase.stop_m
-00001920: 6f64 756c 6573 6301 0000 0000 0000 0000  odulesc.........
-00001930: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
-00001940: 1a00 0000 7c00 6a00 7216 6401 6402 6c01  ....|.j.r.d.d.l.
-00001950: 7d01 7c01 a002 a100 0100 6402 5300 2903  }.|.......d.S.).
-00001960: 7a58 2054 6869 7320 6675 6e63 7469 6f6e  zX This function
-00001970: 2068 6173 2074 6f20 6265 2063 616c 6c65   has to be calle
-00001980: 6420 6672 6f6d 2065 6163 6820 6e65 7720  d from each new 
-00001990: 7468 7265 6164 2074 6f20 6163 7469 7661  thread to activa
-000019a0: 7465 2064 6562 7567 6765 7220 7375 7070  te debugger supp
-000019b0: 6f72 7420 666f 7220 6974 7201 0000 004e  ort for itr....N
-000019c0: 2903 722a 0000 00da 0764 6562 7567 7079  ).r*.....debugpy
-000019d0: da11 6465 6275 675f 7468 6973 5f74 6872  ..debug_this_thr
-000019e0: 6561 6429 0272 3d00 0000 7290 0000 0072  ead).r=...r....r
-000019f0: 1400 0000 7214 0000 0072 1500 0000 da29  ....r....r.....)
-00001a00: 6163 7469 7661 7465 5f64 6562 7567 6765  activate_debugge
-00001a10: 725f 7375 7070 6f72 745f 666f 725f 7468  r_support_for_th
-00001a20: 6973 5f74 6872 6561 649b 0000 0073 0600  is_thread....s..
-00001a30: 0000 0002 0601 0801 7a39 4170 706c 6963  ........z9Applic
-00001a40: 6174 696f 6e42 6173 652e 6163 7469 7661  ationBase.activa
-00001a50: 7465 5f64 6562 7567 6765 725f 7375 7070  te_debugger_supp
-00001a60: 6f72 745f 666f 725f 7468 6973 5f74 6872  ort_for_this_thr
-00001a70: 6561 6429 0172 8500 0000 291e 720d 0000  ead).r....).r...
-00001a80: 0072 0e00 0000 720f 0000 0072 6e00 0000  .r....r....rn...
-00001a90: 722c 0000 0072 2d00 0000 7222 0000 0072  r,...r-...r"...r
-00001aa0: 5500 0000 724d 0000 0072 4e00 0000 7257  U...rM...rN...rW
-00001ab0: 0000 0072 5f00 0000 7207 0000 0072 6400  ...r_...r....rd.
-00001ac0: 0000 7265 0000 0072 4900 0000 727f 0000  ..re...rI...r...
-00001ad0: 0072 8000 0000 7282 0000 0072 8300 0000  .r....r....r....
-00001ae0: 7206 0000 0072 8100 0000 727c 0000 0072  r....r....r|...r
-00001af0: 8800 0000 7212 0000 0072 8b00 0000 724f  ....r....r....rO
-00001b00: 0000 0072 5600 0000 7292 0000 00da 0d5f  ...rV...r......_
-00001b10: 5f63 6c61 7373 6365 6c6c 5f5f 7214 0000  _classcell__r...
-00001b20: 0072 1400 0000 7240 0000 0072 1500 0000  .r....r@...r....
-00001b30: 7216 0000 0023 0000 0073 2600 0000 0801  r....#...s&.....
-00001b40: 1819 080c 0805 0803 0803 0806 0e04 0e05  ................
-00001b50: 1a15 0e03 0e03 0e03 0803 1603 1208 0e03  ................
-00001b60: 0e04 0805 7216 0000 0029 1dda 075f 5f64  ....r....)...__d
-00001b70: 6f63 5f5f 7229 0000 0072 2f00 0000 7225  oc__r)...r/...r%
-00001b80: 0000 0072 6f00 0000 722c 0000 00da 1e6e  ...ro...r,.....n
-00001b90: 616e 6f73 7572 662e 6c69 622e 6775 692e  anosurf.lib.gui.
-00001ba0: 696d 706f 7274 5f68 656c 7065 7272 0200  import_helperr..
-00001bb0: 0000 da11 5079 5369 6465 322e 5174 5769  ....PySide2.QtWi
-00001bc0: 6467 6574 7372 0300 0000 da0e 5079 5369  dgetsr......PySi
-00001bd0: 6465 322e 5174 436f 7265 7204 0000 00da  de2.QtCorer.....
-00001be0: 1150 7953 6964 6536 2e51 7457 6964 6765  .PySide6.QtWidge
-00001bf0: 7473 da0e 5079 5369 6465 362e 5174 436f  ts..PySide6.QtCo
-00001c00: 7265 da08 6e61 6e6f 7375 7266 7242 0000  re..nanosurfrB..
-00001c10: 005a 266e 616e 6f73 7572 662e 6c69 622e  .Z&nanosurf.lib.
-00001c20: 6672 616d 6577 6f72 6b73 2e71 745f 6170  frameworks.qt_ap
-00001c30: 702e 6170 705f 6775 6972 0500 0000 5a29  p.app_guir....Z)
-00001c40: 6e61 6e6f 7375 7266 2e6c 6962 2e66 7261  nanosurf.lib.fra
-00001c50: 6d65 776f 726b 732e 7174 5f61 7070 2e61  meworks.qt_app.a
-00001c60: 7070 5f63 6f6d 6d6f 6e72 0600 0000 da2a  pp_commonr.....*
-00001c70: 6e61 6e6f 7375 7266 2e6c 6962 2e66 7261  nanosurf.lib.fra
-00001c80: 6d65 776f 726b 732e 7174 5f61 7070 2e6d  meworks.qt_app.m
-00001c90: 6f64 756c 655f 6261 7365 7207 0000 00da  odule_baser.....
-00001ca0: 1f6e 616e 6f73 7572 662e 6c69 622e 6461  .nanosurf.lib.da
-00001cb0: 7461 7479 7065 732e 7072 6f70 5f76 616c  tatypes.prop_val
-00001cc0: 7208 0000 0072 0900 0000 7234 0000 0072  r....r....r4...r
-00001cd0: 3600 0000 720c 0000 0072 1600 0000 7214  6...r....r....r.
-00001ce0: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
-00001cf0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00001d00: 7328 0000 0004 0508 0108 0108 0108 0108  s(..............
-00001d10: 020c 0106 010c 010e 020c 010c 0308 010c  ................
-00001d20: 010c 010c 0110 0204 0104 0210 05         .............
+000000c0: 6408 6c14 6d15 5a15 6d16 5a16 0100 6401  d.l.m.Z.m.Z...d.
+000000d0: 6409 6c17 6d18 5a18 6d19 5a19 0100 640a  d.l.m.Z.m.Z...d.
+000000e0: 5a1a 640b 5a1b 4700 640c 640d 8400 640d  Z.d.Z.G.d.d...d.
+000000f0: 6518 8303 5a1c 4700 640e 640f 8400 640f  e...Z.G.d.d...d.
+00000100: 6509 8303 5a1d 6402 5300 2910 7a62 2054  e...Z.d.S.).zb T
+00000110: 6865 2061 7070 6c69 6361 7469 6f6e 2062  he application b
+00000120: 6173 6520 636c 6173 7320 6f66 2074 6865  ase class of the
+00000130: 2061 7070 6c69 6361 7469 6f6e 2066 7261   application fra
+00000140: 6d65 776f 726b 0a43 6f70 7972 6967 6874  mework.Copyright
+00000150: 204e 616e 6f73 7572 6620 4147 2032 3032   Nanosurf AG 202
+00000160: 310a 4c69 6365 6e73 6520 2d20 4d49 540a  1.License - MIT.
+00000170: e900 0000 004e 2901 da22 696d 706f 7274  .....N).."import
+00000180: 5f70 7973 6964 6532 5f69 665f 6e6f 6e65  _pyside2_if_none
+00000190: 5f69 735f 6465 7465 6374 6564 2901 da0c  _is_detected)...
+000001a0: 5141 7070 6c69 6361 7469 6f6e 2901 da09  QApplication)...
+000001b0: 5153 6574 7469 6e67 7329 01da 0941 7070  QSettings)...App
+000001c0: 5769 6e64 6f77 2901 da07 4d73 6754 7970  Window)...MsgTyp
+000001d0: 6529 02da 0a4d 6f64 756c 6542 6173 65da  e)...ModuleBase.
+000001e0: 0c4d 6f64 756c 6553 6372 6565 6e29 02da  .ModuleScreen)..
+000001f0: 0950 726f 7053 746f 7265 da07 5072 6f70  .PropStore..Prop
+00000200: 5661 6cda 036c 6f67 da06 636f 6e66 6967  Val..log..config
+00000210: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000220: 0003 0000 0040 0000 0073 2800 0000 6500  .....@...s(...e.
+00000230: 5a01 6400 5a02 6503 6401 8301 5a04 6503  Z.d.Z.e.d...Z.e.
+00000240: 6401 8301 5a05 6503 6506 6402 8301 8301  d...Z.e.e.d.....
+00000250: 5a07 6403 5300 2904 da0b 4170 7053 6574  Z.d.S.)...AppSet
+00000260: 7469 6e67 7354 7201 0000 004e 2908 da08  tingsTr....N)...
+00000270: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000280: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000290: 5f5f 720a 0000 00da 074c 6f67 6769 6e67  __r......Logging
+000002a0: da10 4c6f 6164 4c61 7374 5365 7474 696e  ..LoadLastSettin
+000002b0: 6773 da03 696e 74da 1141 6374 6976 654d  gs..int..ActiveM
+000002c0: 6f64 756c 6549 6e64 6578 a900 7215 0000  oduleIndex..r...
+000002d0: 0072 1500 0000 fa44 633a 5c67 6974 5c73  .r.....Dc:\git\s
+000002e0: 6372 6970 7473 5f70 7974 686f 6e5f 6c69  cripts_python_li
+000002f0: 625c 6e61 6e6f 7375 7266 5c6c 6962 5c66  b\nanosurf\lib\f
+00000300: 7261 6d65 776f 726b 735c 7174 5f61 7070  rameworks\qt_app
+00000310: 5c61 7070 5f62 6173 652e 7079 720d 0000  \app_base.pyr...
+00000320: 001e 0000 0073 0600 0000 0801 0801 0801  .....s..........
+00000330: 720d 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000340: 0000 0000 0000 0500 0000 0000 0000 7322  ..............s"
+00000350: 0100 0065 005a 0164 005a 0265 0365 0365  ...e.Z.d.Z.e.e.e
+00000360: 046a 0564 019c 0387 0066 0164 0264 0384  .j.d.....f.d.d..
+00000370: 0c5a 0664 0464 0584 005a 0764 0664 0784  .Z.d.d...Z.d.d..
+00000380: 005a 0864 0864 0984 005a 0964 0a64 0b84  .Z.d.d...Z.d.d..
+00000390: 005a 0a64 0c64 0d84 005a 0b65 0c64 0e9c  .Z.d.d...Z.e.d..
+000003a0: 0164 0f64 1084 045a 0d65 0c64 0e9c 0164  .d.d...Z.e.d...d
+000003b0: 1164 1284 045a 0e65 04a0 0564 13a1 0166  .d...Z.e...d...f
+000003c0: 0165 046a 0564 149c 0164 1564 1684 055a  .e.j.d...d.d...Z
+000003d0: 0f65 0364 179c 0164 1864 1984 045a 1065  .e.d...d.d...Z.e
+000003e0: 0364 179c 0164 1a64 1b84 045a 1165 0364  .d...d.d...Z.e.d
+000003f0: 179c 0164 1c64 1d84 045a 1264 1e64 1f84  ...d.d...Z.d.d..
+00000400: 005a 1365 146a 1566 0165 0365 1464 209c  .Z.e.j.f.e.e.d .
+00000410: 0264 2164 2284 055a 1664 3665 0c65 0365  .d!d"..Z.d6e.e.e
+00000420: 1764 259c 0364 2664 2784 055a 1864 3765  .d%..d&d'..Z.d7e
+00000430: 0c65 1765 0364 299c 0364 2a64 2b84 055a  .e.e.d)..d*d+..Z
+00000440: 1965 1a64 2c9c 0164 2d64 2e84 045a 1b65  .e.d,..d-d...Z.e
+00000450: 1a64 2f9c 0164 3064 3184 045a 1c64 3264  .d/..d0d1..Z.d2d
+00000460: 3384 005a 1d64 3464 3584 005a 1e87 0004  3..Z.d4d5..Z....
+00000470: 005a 1f53 0029 38da 0f41 7070 6c69 6361  .Z.S.)8..Applica
+00000480: 7469 6f6e 4261 7365 2903 da07 636f 6d70  tionBase)...comp
+00000490: 616e 79da 0e61 7070 5f6e 616d 655f 7368  any..app_name_sh
+000004a0: 6f72 74da 096d 6169 6e5f 7061 7468 6304  ort..main_pathc.
+000004b0: 0000 0000 0000 0000 0000 0006 0000 0005  ................
+000004c0: 0000 000f 0000 0073 f600 0000 7400 8300  .......s....t...
+000004d0: 6a01 7c04 6900 7c05 a401 8e01 0100 7c01  j.|.i.|.......|.
+000004e0: 7c00 5f02 7c02 7c00 5f03 7c02 a004 6401  |._.|.|._.|...d.
+000004f0: 6402 a102 7c00 5f05 7406 6a07 6a08 a009  d...|._.t.j.j...
+00000500: 7c02 a101 0100 740a 740b 6403 6404 6405  |.....t.t.d.d.d.
+00000510: 8400 8303 8300 6400 7501 7c00 5f0c 740d  ......d.u.|._.t.
+00000520: 7c00 6a02 7c00 6a05 8302 7c00 5f0e 740f  |.j.|.j...|._.t.
+00000530: a010 7c03 a101 6a11 7c00 5f12 740f a010  ..|...j.|._.t...
+00000540: 7413 6a14 a015 7416 a101 a101 6a11 7c00  t.j...t.....j.|.
+00000550: 5f17 740f a010 7413 6a14 a018 6406 a101  _.t...t.j...d...
+00000560: a101 740f a010 7c00 6a02 a101 1b00 740f  ..t...|.j.....t.
+00000570: a010 7c00 6a05 a101 1b00 7c00 5f19 7c00  ..|.j.....|._.|.
+00000580: 6a19 741a 1b00 7c00 5f1b 7c00 6a19 741c  j.t...|._.|.j.t.
+00000590: 1b00 7c00 5f1d 7c00 6a1d 6407 1b00 7c00  ..|._.|.j.d...|.
+000005a0: 5f1e 6408 7c00 5f1f 7c00 6a17 7c00 5f20  _.d.|._.|.j.|._ 
+000005b0: 7421 8300 7c00 5f22 6900 7c00 5f23 6400  t!..|._"i.|._#d.
+000005c0: 5300 2909 4efa 0120 da01 5fda 0867 6574  S.).N.. .._..get
+000005d0: 7472 6163 6563 0000 0000 0000 0000 0000  tracec..........
+000005e0: 0000 0000 0000 0100 0000 5300 0000 7304  ..........S...s.
+000005f0: 0000 0064 0053 00a9 014e 7215 0000 0072  ...d.S...Nr....r
+00000600: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+00000610: 0000 00da 083c 6c61 6d62 6461 3e2a 0000  .....<lambda>*..
+00000620: 00f3 0000 0000 7a2a 4170 706c 6963 6174  ......z*Applicat
+00000630: 696f 6e42 6173 652e 5f5f 696e 6974 5f5f  ionBase.__init__
+00000640: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00000650: 613e 7a0e 254c 4f43 414c 4150 5044 4154  a>z.%LOCALAPPDAT
+00000660: 4125 7a0f 6c61 7374 5f63 6f6e 6669 672e  A%z.last_config.
+00000670: 696e 69da 0b41 7070 6c69 6361 7469 6f6e  ini..Application
+00000680: 2924 da05 7375 7065 72da 085f 5f69 6e69  )$..super..__ini
+00000690: 745f 5f72 1800 0000 5a0d 6170 705f 6e61  t__r....Z.app_na
+000006a0: 6d65 5f6c 6f6e 67da 0772 6570 6c61 6365  me_long..replace
+000006b0: da08 6170 705f 6e61 6d65 da06 6374 7970  ..app_name..ctyp
+000006c0: 6573 da06 7769 6e64 6c6c da07 7368 656c  es..windll..shel
+000006d0: 6c33 325a 2753 6574 4375 7272 656e 7450  l32Z'SetCurrentP
+000006e0: 726f 6365 7373 4578 706c 6963 6974 4170  rocessExplicitAp
+000006f0: 7055 7365 724d 6f64 656c 4944 da07 6765  pUserModelID..ge
+00000700: 7461 7474 72da 0373 7973 da14 6973 5f69  tattr..sys..is_i
+00000710: 6e5f 6465 6275 6767 696e 675f 6d6f 6465  n_debugging_mode
+00000720: 7204 0000 00da 0872 6567 6973 7472 79da  r......registry.
+00000730: 0770 6174 686c 6962 da04 5061 7468 da06  .pathlib..Path..
+00000740: 7061 7265 6e74 721a 0000 00da 026f 73da  parentr......os.
+00000750: 0470 6174 68da 0761 6273 7061 7468 da08  .path..abspath..
+00000760: 5f5f 6669 6c65 5f5f 5a0e 6672 616d 6577  __file__Z.framew
+00000770: 6f72 6b5f 7061 7468 da0a 6578 7061 6e64  ork_path..expand
+00000780: 7661 7273 5a0d 6170 705f 6461 7461 5f70  varsZ.app_data_p
+00000790: 6174 68da 0c64 6972 5f6e 616d 655f 6c6f  ath..dir_name_lo
+000007a0: 67da 086c 6f67 5f70 6174 68da 0f64 6972  g..log_path..dir
+000007b0: 5f6e 616d 655f 636f 6e66 6967 da0b 636f  _name_config..co
+000007c0: 6e66 6967 5f70 6174 68da 0b63 6f6e 6669  nfig_path..confi
+000007d0: 675f 6669 6c65 da0e 636f 6e66 6967 5f73  g_file..config_s
+000007e0: 6563 7469 6f6e da0d 7265 736f 7572 6365  ection..resource
+000007f0: 5f70 6174 6872 0d00 0000 da08 7365 7474  _pathr......sett
+00000800: 696e 6773 da07 6d6f 6475 6c65 7329 06da  ings..modules)..
+00000810: 0473 656c 6672 1800 0000 7219 0000 0072  .selfr....r....r
+00000820: 1a00 0000 da04 6172 6773 da06 6b77 6172  ......args..kwar
+00000830: 6773 a901 da09 5f5f 636c 6173 735f 5f72  gs....__class__r
+00000840: 1500 0000 7216 0000 0072 2300 0000 2400  ....r....r#...$.
+00000850: 0000 7322 0000 0000 0112 0106 0106 010e  ..s"............
+00000860: 010e 0118 0310 030e 0116 012c 010c 010c  ...........,....
+00000870: 010c 0306 0108 0108 017a 1841 7070 6c69  .........z.Appli
+00000880: 6361 7469 6f6e 4261 7365 2e5f 5f69 6e69  cationBase.__ini
+00000890: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
+000008a0: 0100 0000 0500 0000 4300 0000 7396 0000  ........C...s...
+000008b0: 0074 006a 016a 02a0 037c 006a 04a1 0101  .t.j.j...|.j....
+000008c0: 0074 006a 056a 06a0 077c 006a 087c 006a  .t.j.j...|.j.|.j
+000008d0: 097c 006a 0aa1 0301 007c 00a0 0ba1 0001  .|.j.....|......
+000008e0: 0074 0c7c 0083 017c 005f 0d7c 006a 0da0  .t.|...|._.|.j..
+000008f0: 0e7c 006a 0f64 011b 007c 006a 0f64 021b  .|.j.d...|.j.d..
+00000900: 00a1 0201 007c 006a 10a0 117c 006a 12a1  .....|.j...|.j..
+00000910: 0101 007c 00a0 13a1 0001 007c 006a 0da0  ...|.......|.j..
+00000920: 147c 006a 086a 156a 16a1 0101 007c 006a  .|.j.j.j.....|.j
+00000930: 0da0 17a1 0001 007c 006a 18a0 1964 03a1  .......|.j...d..
+00000940: 0101 0064 0053 0029 044e 7a12 6170 705f  ...d.S.).Nz.app_
+00000950: 7374 796c 6573 6865 6574 2e71 7373 7a0c  stylesheet.qssz.
+00000960: 6170 705f 6963 6f6e 2e69 636f 7a0e 4170  app_icon.icoz.Ap
+00000970: 7020 7275 6e6e 696e 672e 2e2e 291a da03  p running...)...
+00000980: 6e73 66da 0475 7469 6cda 0866 696c 6575  nsf..util..fileu
+00000990: 7469 6cda 0d63 7265 6174 655f 666f 6c64  til..create_fold
+000009a0: 6572 7238 0000 00da 0964 6174 6174 7970  err8.....datatyp
+000009b0: 6573 da08 7072 6f70 5f76 616c da12 6c6f  es..prop_val..lo
+000009c0: 6164 5f66 726f 6d5f 696e 695f 6669 6c65  ad_from_ini_file
+000009d0: 723c 0000 0072 3900 0000 723a 0000 00da  r<...r9...r:....
+000009e0: 0c73 6574 7570 5f6c 6f67 6765 7272 0500  .setup_loggerr..
+000009f0: 0000 da09 6170 7077 696e 646f 775a 0a63  ....appwindowZ.c
+00000a00: 7265 6174 655f 6775 6972 3b00 0000 da10  reate_guir;.....
+00000a10: 6c61 7374 5769 6e64 6f77 436c 6f73 6564  lastWindowClosed
+00000a20: da07 636f 6e6e 6563 74da 0871 7569 745f  ..connect..quit_
+00000a30: 6170 70da 0a64 6f5f 7374 6172 7475 705a  app..do_startupZ
+00000a40: 0f61 6374 6976 6174 655f 7363 7265 656e  .activate_screen
+00000a50: 7214 0000 00da 0576 616c 7565 da04 7368  r......value..sh
+00000a60: 6f77 da06 6c6f 6767 6572 da04 696e 666f  ow..logger..info
+00000a70: a901 723e 0000 0072 1500 0000 7215 0000  ..r>...r....r...
+00000a80: 0072 1600 0000 da09 7374 6172 745f 6170  .r......start_ap
+00000a90: 703d 0000 0073 1400 0000 0001 1001 1801  p=...s..........
+00000aa0: 0801 0a01 1a01 0e01 0801 1201 0a01 7a19  ..............z.
+00000ab0: 4170 706c 6963 6174 696f 6e42 6173 652e  ApplicationBase.
+00000ac0: 7374 6172 745f 6170 7063 0100 0000 0000  start_appc......
+00000ad0: 0000 0000 0000 0100 0000 0500 0000 4300  ..............C.
+00000ae0: 0000 732c 0000 007c 00a0 00a1 0001 007c  ..s,...|.......|
+00000af0: 00a0 01a1 0001 0074 026a 036a 04a0 057c  .......t.j.j...|
+00000b00: 006a 067c 006a 077c 006a 08a1 0301 0064  .j.|.j.|.j.....d
+00000b10: 0053 0072 1e00 0000 2909 da0c 7374 6f70  .S.r....)...stop
+00000b20: 5f6d 6f64 756c 6573 da0b 646f 5f73 6875  _modules..do_shu
+00000b30: 7464 6f77 6e72 4300 0000 7247 0000 0072  tdownrC...rG...r
+00000b40: 4800 0000 da10 7361 7665 5f74 6f5f 696e  H.....save_to_in
+00000b50: 695f 6669 6c65 723c 0000 0072 3900 0000  i_filer<...r9...
+00000b60: 723a 0000 0072 5400 0000 7215 0000 0072  r:...rT...r....r
+00000b70: 1500 0000 7216 0000 0072 4e00 0000 4900  ....r....rN...I.
+00000b80: 0000 7306 0000 0000 0108 0108 017a 1841  ..s..........z.A
+00000b90: 7070 6c69 6361 7469 6f6e 4261 7365 2e71  pplicationBase.q
+00000ba0: 7569 745f 6170 7063 0100 0000 0000 0000  uit_appc........
+00000bb0: 0000 0000 0100 0000 0600 0000 4300 0000  ............C...
+00000bc0: 7326 0000 0074 0064 017c 006a 016a 029b  s&...t.d.|.j.j..
+00000bd0: 0064 0274 03a0 04a1 006a 056a 069b 0064  .d.t.....j.j...d
+00000be0: 039d 0583 0182 0164 0053 0029 044e 7a0d  .......d.S.).Nz.
+00000bf0: 5375 6263 6c61 7373 206f 6620 277a 1427  Subclass of 'z.'
+00000c00: 2068 6173 2074 6f20 696d 706c 656d 656e   has to implemen
+00000c10: 7420 277a 0328 2927 2907 da13 4e6f 7449  t 'z.()')...NotI
+00000c20: 6d70 6c65 6d65 6e74 6564 4572 726f 7272  mplementedErrorr
+00000c30: 4200 0000 720e 0000 0072 2a00 0000 da09  B...r....r*.....
+00000c40: 5f67 6574 6672 616d 65da 0666 5f63 6f64  _getframe..f_cod
+00000c50: 65da 0763 6f5f 6e61 6d65 7254 0000 0072  e..co_namerT...r
+00000c60: 1500 0000 7215 0000 0072 1600 0000 724f  ....r....r....rO
+00000c70: 0000 004e 0000 0073 0200 0000 0001 7a1a  ...N...s......z.
+00000c80: 4170 706c 6963 6174 696f 6e42 6173 652e  ApplicationBase.
+00000c90: 646f 5f73 7461 7274 7570 6301 0000 0000  do_startupc.....
+00000ca0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00000cb0: 0000 0073 0400 0000 6400 5300 721e 0000  ...s....d.S.r...
+00000cc0: 0072 1500 0000 7254 0000 0072 1500 0000  .r....rT...r....
+00000cd0: 7215 0000 0072 1600 0000 7257 0000 0051  r....r....rW...Q
+00000ce0: 0000 0073 0200 0000 0001 7a1b 4170 706c  ...s......z.Appl
+00000cf0: 6963 6174 696f 6e42 6173 652e 646f 5f73  icationBase.do_s
+00000d00: 6875 7464 6f77 6e63 0100 0000 0000 0000  hutdownc........
+00000d10: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00000d20: 731c 0000 0074 0083 0072 107c 00a0 01a1  s....t...r.|....
+00000d30: 0001 006e 087c 00a0 02a1 0001 0064 0053  ...n.|.......d.S
+00000d40: 0072 1e00 0000 2903 7202 0000 00da 0565  .r....).r......e
+00000d50: 7865 635f da04 6578 6563 7254 0000 0072  xec_..execrT...r
+00000d60: 1500 0000 7215 0000 0072 1600 0000 da07  ....r....r......
+00000d70: 6578 6563 7574 6554 0000 0073 0600 0000  executeT...s....
+00000d80: 0001 0601 0a02 7a17 4170 706c 6963 6174  ......z.Applicat
+00000d90: 696f 6e42 6173 652e 6578 6563 7574 6529  ionBase.execute)
+00000da0: 01da 066d 6f64 756c 6563 0200 0000 0000  ...modulec......
+00000db0: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
+00000dc0: 0000 7328 0000 0074 007c 016a 0174 0283  ..s(...t.|.j.t..
+00000dd0: 0272 2474 036a 046a 05a0 067c 016a 017c  .r$t.j.j...|.j.|
+00000de0: 006a 077c 016a 08a1 0301 0064 0053 0072  .j.|.j.....d.S.r
+00000df0: 1e00 0000 2909 da0a 6973 696e 7374 616e  ....)...isinstan
+00000e00: 6365 723c 0000 0072 0900 0000 7243 0000  cer<...r....rC..
+00000e10: 0072 4700 0000 7248 0000 0072 5800 0000  .rG...rH...rX...
+00000e20: 7239 0000 00da 046e 616d 65a9 0272 3e00  r9.....name..r>.
+00000e30: 0000 7260 0000 0072 1500 0000 7215 0000  ..r`...r....r...
+00000e40: 0072 1600 0000 da0d 7361 7665 5f73 6574  .r......save_set
+00000e50: 7469 6e67 735a 0000 0073 0400 0000 0001  tingsZ...s......
+00000e60: 0c01 7a1d 4170 706c 6963 6174 696f 6e42  ..z.ApplicationB
+00000e70: 6173 652e 7361 7665 5f73 6574 7469 6e67  ase.save_setting
+00000e80: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
+00000e90: 0000 0500 0000 4300 0000 7332 0000 0074  ......C...s2...t
+00000ea0: 007c 016a 0174 0283 0272 2e7c 006a 016a  .|.j.t...r.|.j.j
+00000eb0: 036a 0472 2e74 056a 066a 07a0 087c 016a  .j.r.t.j.j...|.j
+00000ec0: 017c 006a 097c 016a 0aa1 0301 0064 0053  .|.j.|.j.....d.S
+00000ed0: 0072 1e00 0000 290b 7261 0000 0072 3c00  .r....).ra...r<.
+00000ee0: 0000 7209 0000 0072 1200 0000 7250 0000  ..r....r....rP..
+00000ef0: 0072 4300 0000 7247 0000 0072 4800 0000  .rC...rG...rH...
+00000f00: 7249 0000 0072 3900 0000 7262 0000 0072  rI...r9...rb...r
+00000f10: 6300 0000 7215 0000 0072 1500 0000 7216  c...r....r....r.
+00000f20: 0000 00da 0d6c 6f61 645f 7365 7474 696e  .....load_settin
+00000f30: 6773 5e00 0000 7306 0000 0000 010c 010a  gs^...s.........
+00000f40: 017a 1d41 7070 6c69 6361 7469 6f6e 4261  .z.ApplicationBa
+00000f50: 7365 2e6c 6f61 645f 7365 7474 696e 6773  se.load_settings
+00000f60: 7a0a 6c61 7465 7374 2e6c 6f67 2901 da07  z.latest.log)...
+00000f70: 6c6f 6766 696c 6563 0200 0000 0000 0000  logfilec........
+00000f80: 0000 0000 0500 0000 0700 0000 4300 0000  ............C...
+00000f90: 7394 0000 007c 006a 006a 016a 0272 7674  s....|.j.j.j.rvt
+00000fa0: 036a 046a 05a0 067c 006a 07a1 0101 0074  .j.j...|.j.....t
+00000fb0: 087c 006a 077c 011b 0083 017d 0274 096a  .|.j.|.....}.t.j
+00000fc0: 0a74 096a 0b64 0164 027c 0264 0364 048d  .t.j.d.d.|.d.d..
+00000fd0: 0501 0074 09a0 0ca1 007d 037c 03a0 0d74  ...t.....}.|...t
+00000fe0: 096a 0ea1 0101 0074 09a0 0f64 05a1 017d  .j.....t...d...}
+00000ff0: 047c 03a0 107c 04a1 0101 0074 09a0 1164  .|...|.....t...d
+00001000: 06a1 01a0 127c 03a1 0101 0074 09a0 1164  .....|.....t...d
+00001010: 07a1 017c 005f 137c 006a 13a0 0d74 096a  ...|._.|.j...t.j
+00001020: 0ba1 0101 0064 0853 0029 097a cf0a 2020  .....d.S.).z..  
+00001030: 2020 2020 2020 5365 7475 7020 4c6f 6767        Setup Logg
+00001040: 6572 2069 6620 6e65 6564 6564 2061 6e64  er if needed and
+00001050: 2064 6966 6665 7220 6265 7477 6565 6e20   differ between 
+00001060: 636f 6e73 6f6c 2061 6e64 2066 696c 6520  consol and file 
+00001070: 6f75 7470 7574 0a20 2020 2020 2020 2073  output.        s
+00001080: 6574 2075 7020 6c6f 6767 696e 6720 746f  et up logging to
+00001090: 2066 696c 6520 616e 6420 6368 6f6f 7365   file and choose
+000010a0: 206c 6f67 6765 7220 6c65 7665 6c20 2866   logger level (f
+000010b0: 726f 6d20 6869 6768 6573 7420 6c65 7665  rom highest leve
+000010c0: 6c20 746f 206c 6f77 6573 743a 2044 6562  l to lowest: Deb
+000010d0: 7567 2c20 696e 666f 2c20 7761 726e 696e  ug, info, warnin
+000010e0: 672c 2065 7272 6f72 2c20 6372 6974 6963  g, error, critic
+000010f0: 616c 290a 2020 2020 2020 2020 7a33 2528  al).        z3%(
+00001100: 6173 6374 696d 6529 7320 2528 6e61 6d65  asctime)s %(name
+00001110: 292d 3132 7320 2528 6c65 7665 6c6e 616d  )-12s %(levelnam
+00001120: 6529 2d38 7320 2528 6d65 7373 6167 6529  e)-8s %(message)
+00001130: 737a 0e25 6d2d 2564 2025 483a 254d 3a25  sz.%m-%d %H:%M:%
+00001140: 53da 0177 2905 da05 6c65 7665 6cda 0666  S..w)...level..f
+00001150: 6f72 6d61 74da 0764 6174 6566 6d74 da08  ormat..datefmt..
+00001160: 6669 6c65 6e61 6d65 da08 6669 6c65 6d6f  filename..filemo
+00001170: 6465 7a27 2528 6e61 6d65 292d 3132 7320  dez'%(name)-12s 
+00001180: 2528 6c65 7665 6c6e 616d 6529 2d38 7320  %(levelname)-8s 
+00001190: 2528 6d65 7373 6167 6529 73da 0072 2100  %(message)s..r!.
+000011a0: 0000 4e29 1472 3c00 0000 7211 0000 0072  ..N).r<...r....r
+000011b0: 5000 0000 7243 0000 0072 4400 0000 7245  P...rC...rD...rE
+000011c0: 0000 0072 4600 0000 7236 0000 00da 0373  ...rF...r6.....s
+000011d0: 7472 da07 6c6f 6767 696e 67da 0b62 6173  tr..logging..bas
+000011e0: 6963 436f 6e66 6967 da05 4445 4255 47da  icConfig..DEBUG.
+000011f0: 0d53 7472 6561 6d48 616e 646c 6572 da08  .StreamHandler..
+00001200: 7365 744c 6576 656c da04 494e 464f da09  setLevel..INFO..
+00001210: 466f 726d 6174 7465 72da 0c73 6574 466f  Formatter..setFo
+00001220: 726d 6174 7465 72da 0967 6574 4c6f 6767  rmatter..getLogg
+00001230: 6572 da0a 6164 6448 616e 646c 6572 7252  er..addHandlerrR
+00001240: 0000 0029 0572 3e00 0000 7266 0000 005a  ...).r>...rf...Z
+00001250: 0b6c 6f67 6669 6c65 7061 7468 da07 636f  .logfilepath..co
+00001260: 6e73 6f6c 65da 0966 6f72 6d61 7474 6572  nsole..formatter
+00001270: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00001280: 4a00 0000 6300 0000 7320 0000 0000 050a  J...c...s ......
+00001290: 0110 010e 0108 0102 0102 0102 0102 fc06  ................
+000012a0: 0508 010c 010a 010a 0110 010c 017a 1c41  .............z.A
+000012b0: 7070 6c69 6361 7469 6f6e 4261 7365 2e73  pplicationBase.s
+000012c0: 6574 7570 5f6c 6f67 6765 7229 01da 036d  etup_logger)...m
+000012d0: 7367 6302 0000 0000 0000 0000 0000 0002  sgc.............
+000012e0: 0000 0004 0000 0043 0000 0073 1200 0000  .......C...s....
+000012f0: 7c00 a000 7c01 7401 6a02 a102 0100 6400  |...|.t.j.....d.
+00001300: 5300 721e 0000 0029 03da 0c73 686f 775f  S.r....)...show_
+00001310: 6d65 7373 6167 6572 0600 0000 da05 4572  messager......Er
+00001320: 726f 72a9 0272 3e00 0000 727b 0000 0072  ror..r>...r{...r
+00001330: 1500 0000 7215 0000 0072 1600 0000 da12  ....r....r......
+00001340: 7368 6f77 5f65 7272 6f72 5f6d 6573 7361  show_error_messa
+00001350: 6765 7800 0000 7302 0000 0000 017a 2241  gex...s......z"A
+00001360: 7070 6c69 6361 7469 6f6e 4261 7365 2e73  pplicationBase.s
+00001370: 686f 775f 6572 726f 725f 6d65 7373 6167  how_error_messag
+00001380: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
+00001390: 0000 0400 0000 4300 0000 7312 0000 007c  ......C...s....|
+000013a0: 00a0 007c 0174 016a 02a1 0201 0064 0053  ...|.t.j.....d.S
+000013b0: 0072 1e00 0000 2903 727c 0000 0072 0600  .r....).r|...r..
+000013c0: 0000 5a04 5761 726e 727e 0000 0072 1500  ..Z.Warnr~...r..
+000013d0: 0000 7215 0000 0072 1600 0000 da11 7368  ..r....r......sh
+000013e0: 6f77 5f77 6172 6e5f 6d65 7373 6167 657b  ow_warn_message{
+000013f0: 0000 0073 0200 0000 0001 7a21 4170 706c  ...s......z!Appl
+00001400: 6963 6174 696f 6e42 6173 652e 7368 6f77  icationBase.show
+00001410: 5f77 6172 6e5f 6d65 7373 6167 6563 0200  _warn_messagec..
+00001420: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00001430: 0000 4300 0000 7312 0000 007c 00a0 007c  ..C...s....|...|
+00001440: 0174 016a 02a1 0201 0064 0053 0072 1e00  .t.j.....d.S.r..
+00001450: 0000 2903 727c 0000 0072 0600 0000 da04  ..).r|...r......
+00001460: 496e 666f 727e 0000 0072 1500 0000 7215  Infor~...r....r.
+00001470: 0000 0072 1600 0000 da11 7368 6f77 5f69  ...r......show_i
+00001480: 6e66 6f5f 6d65 7373 6167 657e 0000 0073  nfo_message~...s
+00001490: 0200 0000 0001 7a21 4170 706c 6963 6174  ......z!Applicat
+000014a0: 696f 6e42 6173 652e 7368 6f77 5f69 6e66  ionBase.show_inf
+000014b0: 6f5f 6d65 7373 6167 6563 0100 0000 0000  o_messagec......
+000014c0: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+000014d0: 0000 730e 0000 007c 006a 00a0 01a1 0001  ..s....|.j......
+000014e0: 0064 0053 0072 1e00 0000 2902 724b 0000  .d.S.r....).rK..
+000014f0: 005a 0c68 6964 655f 6d65 7373 6167 6572  .Z.hide_messager
+00001500: 5400 0000 7215 0000 0072 1500 0000 7216  T...r....r....r.
+00001510: 0000 00da 0d63 6c65 6172 5f6d 6573 7361  .....clear_messa
+00001520: 6765 8100 0000 7302 0000 0000 017a 1d41  ge....s......z.A
+00001530: 7070 6c69 6361 7469 6f6e 4261 7365 2e63  pplicationBase.c
+00001540: 6c65 6172 5f6d 6573 7361 6765 2902 727b  lear_message).r{
+00001550: 0000 00da 086d 7367 5f74 7970 6563 0300  .....msg_typec..
+00001560: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00001570: 0000 4300 0000 7312 0000 007c 006a 00a0  ..C...s....|.j..
+00001580: 017c 017c 02a1 0201 0064 0053 0072 1e00  .|.|.....d.S.r..
+00001590: 0000 2902 724b 0000 0072 7c00 0000 2903  ..).rK...r|...).
+000015a0: 723e 0000 0072 7b00 0000 7284 0000 0072  r>...r{...r....r
+000015b0: 1500 0000 7215 0000 0072 1600 0000 727c  ....r....r....r|
+000015c0: 0000 0084 0000 0073 0200 0000 0001 7a1c  .......s......z.
+000015d0: 4170 706c 6963 6174 696f 6e42 6173 652e  ApplicationBase.
+000015e0: 7368 6f77 5f6d 6573 7361 6765 da06 4d6f  show_message..Mo
+000015f0: 6475 6c65 4e29 03da 0a6e 6577 5f6d 6f64  duleN)...new_mod
+00001600: 756c 6572 6200 0000 da0a 6e65 775f 7363  ulerb.....new_sc
+00001610: 7265 656e 6304 0000 0000 0000 0000 0000  reenc...........
+00001620: 0004 0000 0005 0000 0043 0000 0073 5a00  .........C...sZ.
+00001630: 0000 7c02 7c01 5f00 7c03 6400 7501 7214  ..|.|._.|.d.u.r.
+00001640: 7c03 7c01 5f01 7c00 6a02 a003 6401 7c01  |.|._.|.j...d.|.
+00001650: 6a00 9b00 9d02 a101 0100 7c01 7c00 6a04  j.........|.|.j.
+00001660: 7c01 6a00 3c00 7c01 a005 a100 0100 7c01  |.j.<.|.......|.
+00001670: 6a01 6400 7501 7256 7c00 a006 7c01 7c01  j.d.u.rV|...|.|.
+00001680: 6a01 7c02 a103 0100 6400 5300 2902 4e7a  j.|.....d.S.).Nz
+00001690: 0e53 7461 7274 206d 6f64 756c 653a 2029  .Start module: )
+000016a0: 0772 6200 0000 da02 7569 7252 0000 0072  .rb.....uirR...r
+000016b0: 5300 0000 723d 0000 00da 0573 7461 7274  S...r=.....start
+000016c0: da0a 6164 645f 7363 7265 656e 2904 723e  ..add_screen).r>
+000016d0: 0000 0072 8600 0000 7262 0000 0072 8700  ...r....rb...r..
+000016e0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+000016f0: 00da 0a61 6464 5f6d 6f64 756c 6587 0000  ...add_module...
+00001700: 0073 1000 0000 0001 0601 0801 0601 1401  .s..............
+00001710: 0c01 0801 0a01 7a1a 4170 706c 6963 6174  ......z.Applicat
+00001720: 696f 6e42 6173 652e 6164 645f 6d6f 6475  ionBase.add_modu
+00001730: 6c65 da06 5363 7265 656e 2903 7260 0000  le..Screen).r`..
+00001740: 0072 8700 0000 da0b 7363 7265 656e 5f6e  .r......screen_n
+00001750: 616d 6563 0400 0000 0000 0000 0000 0000  amec............
+00001760: 0400 0000 0400 0000 4300 0000 731c 0000  ........C...s...
+00001770: 007c 02a0 007c 01a1 0101 007c 006a 01a0  .|...|.....|.j..
+00001780: 027c 027c 03a1 0201 0064 0053 0072 1e00  .|.|.....d.S.r..
+00001790: 0000 2903 5a0d 6372 6561 7465 5f73 6372  ..).Z.create_scr
+000017a0: 6565 6e72 4b00 0000 728a 0000 0029 0472  eenrK...r....).r
+000017b0: 3e00 0000 7260 0000 0072 8700 0000 728d  >...r`...r....r.
+000017c0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+000017d0: 0000 728a 0000 0091 0000 0073 0400 0000  ..r........s....
+000017e0: 0001 0a01 7a1a 4170 706c 6963 6174 696f  ....z.Applicatio
+000017f0: 6e42 6173 652e 6164 645f 7363 7265 656e  nBase.add_screen
+00001800: 2901 da06 7265 7475 726e 6301 0000 0000  )...returnc.....
+00001810: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00001820: 0000 0073 0a00 0000 7400 7c00 6a01 8301  ...s....t.|.j...
+00001830: 5300 721e 0000 0029 02da 036c 656e 723d  S.r....)...lenr=
+00001840: 0000 0072 5400 0000 7215 0000 0072 1500  ...rT...r....r..
+00001850: 0000 7216 0000 00da 1067 6574 5f6d 6f64  ..r......get_mod
+00001860: 756c 655f 636f 756e 7495 0000 0073 0200  ule_count....s..
+00001870: 0000 0001 7a20 4170 706c 6963 6174 696f  ....z Applicatio
+00001880: 6e42 6173 652e 6765 745f 6d6f 6475 6c65  nBase.get_module
+00001890: 5f63 6f75 6e74 2901 da0c 6d6f 6475 6c65  _count)...module
+000018a0: 5f69 6e64 6578 6302 0000 0000 0000 0000  _indexc.........
+000018b0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+000018c0: 1a00 0000 7c01 7c00 6a00 6a01 5f02 7c00  ....|.|.j.j._.|.
+000018d0: 6a03 a004 7c01 a101 0100 6400 5300 721e  j...|.....d.S.r.
+000018e0: 0000 0029 0572 3c00 0000 7214 0000 0072  ...).r<...r....r
+000018f0: 5000 0000 724b 0000 005a 1a73 6574 5f61  P...rK...Z.set_a
+00001900: 6374 6976 655f 6d6f 6475 6c65 5f62 795f  ctive_module_by_
+00001910: 696e 6465 7829 0272 3e00 0000 7291 0000  index).r>...r...
+00001920: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+00001930: da0f 6163 7469 7661 7465 5f6d 6f64 756c  ..activate_modul
+00001940: 6598 0000 0073 0400 0000 0001 0a01 7a1f  e....s........z.
+00001950: 4170 706c 6963 6174 696f 6e42 6173 652e  ApplicationBase.
+00001960: 6163 7469 7661 7465 5f6d 6f64 756c 6563  activate_modulec
+00001970: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001980: 0500 0000 4300 0000 7330 0000 007c 006a  ....C...s0...|.j
+00001990: 00a0 01a1 0044 005d 207d 017c 006a 02a0  .....D.] }.|.j..
+000019a0: 0364 017c 016a 049b 009d 02a1 0101 007c  .d.|.j.........|
+000019b0: 01a0 05a1 0001 0071 0a64 0053 0029 024e  .......q.d.S.).N
+000019c0: 7a0d 5374 6f70 206d 6f64 756c 653a 2029  z.Stop module: )
+000019d0: 0672 3d00 0000 da06 7661 6c75 6573 7252  .r=.....valuesrR
+000019e0: 0000 0072 5300 0000 7262 0000 00da 0473  ...rS...rb.....s
+000019f0: 746f 7029 0272 3e00 0000 da03 6d6f 6472  top).r>.....modr
+00001a00: 1500 0000 7215 0000 0072 1600 0000 7256  ....r....r....rV
+00001a10: 0000 009c 0000 0073 0600 0000 0001 0e01  .......s........
+00001a20: 1401 7a1c 4170 706c 6963 6174 696f 6e42  ..z.ApplicationB
+00001a30: 6173 652e 7374 6f70 5f6d 6f64 756c 6573  ase.stop_modules
+00001a40: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00001a50: 0002 0000 0043 0000 0073 1a00 0000 7c00  .....C...s....|.
+00001a60: 6a00 7216 6401 6402 6c01 7d01 7c01 a002  j.r.d.d.l.}.|...
+00001a70: a100 0100 6402 5300 2903 7a58 2054 6869  ....d.S.).zX Thi
+00001a80: 7320 6675 6e63 7469 6f6e 2068 6173 2074  s function has t
+00001a90: 6f20 6265 2063 616c 6c65 6420 6672 6f6d  o be called from
+00001aa0: 2065 6163 6820 6e65 7720 7468 7265 6164   each new thread
+00001ab0: 2074 6f20 6163 7469 7661 7465 2064 6562   to activate deb
+00001ac0: 7567 6765 7220 7375 7070 6f72 7420 666f  ugger support fo
+00001ad0: 7220 6974 7201 0000 004e 2903 722b 0000  r itr....N).r+..
+00001ae0: 00da 0764 6562 7567 7079 da11 6465 6275  ...debugpy..debu
+00001af0: 675f 7468 6973 5f74 6872 6561 6429 0272  g_this_thread).r
+00001b00: 3e00 0000 7296 0000 0072 1500 0000 7215  >...r....r....r.
+00001b10: 0000 0072 1600 0000 da29 6163 7469 7661  ...r.....)activa
+00001b20: 7465 5f64 6562 7567 6765 725f 7375 7070  te_debugger_supp
+00001b30: 6f72 745f 666f 725f 7468 6973 5f74 6872  ort_for_this_thr
+00001b40: 6561 64a1 0000 0073 0600 0000 0002 0601  ead....s........
+00001b50: 0801 7a39 4170 706c 6963 6174 696f 6e42  ..z9ApplicationB
+00001b60: 6173 652e 6163 7469 7661 7465 5f64 6562  ase.activate_deb
+00001b70: 7567 6765 725f 7375 7070 6f72 745f 666f  ugger_support_fo
+00001b80: 725f 7468 6973 5f74 6872 6561 6429 0272  r_this_thread).r
+00001b90: 8500 0000 4e29 0172 8c00 0000 2920 720e  ....N).r....) r.
+00001ba0: 0000 0072 0f00 0000 7210 0000 0072 6e00  ...r....r....rn.
+00001bb0: 0000 722d 0000 0072 2e00 0000 7223 0000  ..r-...r....r#..
+00001bc0: 0072 5500 0000 724e 0000 0072 4f00 0000  .rU...rN...rO...
+00001bd0: 7257 0000 0072 5f00 0000 7207 0000 0072  rW...r_...r....r
+00001be0: 6400 0000 7265 0000 0072 4a00 0000 727f  d...re...rJ...r.
+00001bf0: 0000 0072 8000 0000 7282 0000 0072 8300  ...r....r....r..
+00001c00: 0000 7206 0000 0072 8100 0000 727c 0000  ..r....r....r|..
+00001c10: 0072 0800 0000 728b 0000 0072 8a00 0000  .r....r....r....
+00001c20: 7213 0000 0072 9000 0000 7292 0000 0072  r....r....r....r
+00001c30: 5600 0000 7298 0000 00da 0d5f 5f63 6c61  V...r......__cla
+00001c40: 7373 6365 6c6c 5f5f 7215 0000 0072 1500  sscell__r....r..
+00001c50: 0000 7241 0000 0072 1600 0000 7217 0000  ..rA...r....r...
+00001c60: 0023 0000 0073 2800 0000 0801 1819 080c  .#...s(.........
+00001c70: 0805 0803 0803 0806 0e04 0e05 1a15 0e03  ................
+00001c80: 0e03 0e03 0803 1603 140a 1404 0e03 0e04  ................
+00001c90: 0805 7217 0000 0029 1eda 075f 5f64 6f63  ..r....)...__doc
+00001ca0: 5f5f 722a 0000 0072 3000 0000 7226 0000  __r*...r0...r&..
+00001cb0: 0072 6f00 0000 722d 0000 00da 1e6e 616e  .ro...r-.....nan
+00001cc0: 6f73 7572 662e 6c69 622e 6775 692e 696d  osurf.lib.gui.im
+00001cd0: 706f 7274 5f68 656c 7065 7272 0200 0000  port_helperr....
+00001ce0: da11 5079 5369 6465 322e 5174 5769 6467  ..PySide2.QtWidg
+00001cf0: 6574 7372 0300 0000 da0e 5079 5369 6465  etsr......PySide
+00001d00: 322e 5174 436f 7265 7204 0000 00da 1150  2.QtCorer......P
+00001d10: 7953 6964 6536 2e51 7457 6964 6765 7473  ySide6.QtWidgets
+00001d20: da0e 5079 5369 6465 362e 5174 436f 7265  ..PySide6.QtCore
+00001d30: da08 6e61 6e6f 7375 7266 7243 0000 005a  ..nanosurfrC...Z
+00001d40: 266e 616e 6f73 7572 662e 6c69 622e 6672  &nanosurf.lib.fr
+00001d50: 616d 6577 6f72 6b73 2e71 745f 6170 702e  ameworks.qt_app.
+00001d60: 6170 705f 6775 6972 0500 0000 5a29 6e61  app_guir....Z)na
+00001d70: 6e6f 7375 7266 2e6c 6962 2e66 7261 6d65  nosurf.lib.frame
+00001d80: 776f 726b 732e 7174 5f61 7070 2e61 7070  works.qt_app.app
+00001d90: 5f63 6f6d 6d6f 6e72 0600 0000 da2a 6e61  _commonr.....*na
+00001da0: 6e6f 7375 7266 2e6c 6962 2e66 7261 6d65  nosurf.lib.frame
+00001db0: 776f 726b 732e 7174 5f61 7070 2e6d 6f64  works.qt_app.mod
+00001dc0: 756c 655f 6261 7365 7207 0000 0072 0800  ule_baser....r..
+00001dd0: 0000 da1f 6e61 6e6f 7375 7266 2e6c 6962  ....nanosurf.lib
+00001de0: 2e64 6174 6174 7970 6573 2e70 726f 705f  .datatypes.prop_
+00001df0: 7661 6c72 0900 0000 720a 0000 0072 3500  valr....r....r5.
+00001e00: 0000 7237 0000 0072 0d00 0000 7217 0000  ..r7...r....r...
+00001e10: 0072 1500 0000 7215 0000 0072 1500 0000  .r....r....r....
+00001e20: 7216 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00001e30: 0000 0073 2800 0000 0405 0801 0801 0801  ...s(...........
+00001e40: 0801 0802 0c01 0601 0c01 0e02 0c01 0c03  ................
+00001e50: 0801 0c01 0c01 1001 1002 0401 0402 1005  ................
```

### Comparing `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/app_gui.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/app_gui.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/app_gui.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/app_gui.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 12:55:54 2023 UTC, .py size: 7474 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,499 +1,529 @@
-00000000: 610d 0d0a 0000 0000 5a4d 3964 321d 0000  a.......ZM9d2...
+00000000: 610d 0d0a 0000 0000 e7fd 5964 331e 0000  a.........Yd3...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 de00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6502  Z.d.d.l.m.Z...e.
 00000040: 8300 7238 6401 6403 6c03 6d04 5a04 0100  ..r8d.d.l.m.Z...
 00000050: 6401 6404 6c03 6d05 5a05 6d04 5a04 6d06  d.d.l.m.Z.m.Z.m.
 00000060: 5a06 0100 6e20 6401 6403 6c07 6d04 5a04  Z...n d.d.l.m.Z.
 00000070: 0100 6401 6404 6c07 6d05 5a05 6d04 5a04  ..d.d.l.m.Z.m.Z.
-00000080: 6d06 5a06 0100 6401 6405 6c08 5a09 6406  m.Z...d.d.l.Z.d.
-00000090: 6407 6c0a 6d0b 5a0b 6d0c 5a0c 0100 6408  d.l.m.Z.m.Z...d.
-000000a0: 5a0d 4700 6409 640a 8400 640a 6504 6a0e  Z.G.d.d...d.e.j.
-000000b0: 8303 5a0f 4700 640b 640c 8400 640c 6504  ..Z.G.d.d...d.e.
-000000c0: 6a10 8303 5a11 4700 640d 640e 8400 640e  j...Z.G.d.d...d.
-000000d0: 6504 6a12 8303 5a13 4700 640f 6410 8400  e.j...Z.G.d.d...
-000000e0: 6410 6504 6a14 8303 5a15 6405 5300 2911  d.e.j...Z.d.S.).
-000000f0: 7a4f 2054 6865 2047 5549 206f 6620 7468  zO The GUI of th
-00000100: 6520 6170 706c 6963 6174 696f 6e20 6672  e application fr
-00000110: 616d 6577 6f72 6b0a 436f 7079 7269 6768  amework.Copyrigh
-00000120: 7420 4e61 6e6f 7375 7266 2041 4720 3230  t Nanosurf AG 20
-00000130: 3231 0a4c 6963 656e 7365 202d 204d 4954  21.License - MIT
-00000140: 0ae9 0000 0000 2901 da22 696d 706f 7274  ......).."import
-00000150: 5f70 7973 6964 6532 5f69 665f 6e6f 6e65  _pyside2_if_none
-00000160: 5f69 735f 6465 7465 6374 6564 2901 da09  _is_detected)...
-00000170: 5174 5769 6467 6574 7329 03da 0551 7447  QtWidgets)...QtG
-00000180: 7569 7203 0000 00da 0651 7443 6f72 654e  uir......QtCoreN
-00000190: e901 0000 0029 02da 0a61 7070 5f63 6f6d  .....)...app_com
-000001a0: 6d6f 6eda 0b6d 6f64 756c 655f 6261 7365  mon..module_base
-000001b0: e9c8 0000 0063 0000 0000 0000 0000 0000  .....c..........
-000001c0: 0000 0000 0000 0500 0000 0000 0000 7326  ..............s&
-000001d0: 0000 0065 005a 0164 005a 0264 0665 0365  ...e.Z.d.Z.d.e.e
-000001e0: 0464 039c 0287 0066 0164 0464 0584 0d5a  .d.....f.d.d...Z
-000001f0: 0587 0004 005a 0653 0029 07da 0d4d 656e  .....Z.S.)...Men
-00000200: 7553 6570 6172 6174 6f72 4672 0600 0000  uSeparatorFr....
-00000210: a902 da06 6869 6464 656e da06 6865 6967  ....hidden..heig
-00000220: 6874 6303 0000 0000 0000 0000 0000 0004  htc.............
-00000230: 0000 0005 0000 000b 0000 0073 5400 0000  ...........sT...
-00000240: 7400 8300 6a01 7c03 8e00 0100 7c00 a002  t...j.|.....|...
-00000250: 7403 6a04 6a05 7403 6a04 6a06 4200 a101  t.j.j.t.j.j.B...
-00000260: 0100 7c00 a007 6401 7408 6a09 6a0a 6a0b  ..|...d.t.j.j.j.
-00000270: 6a0c 9b00 6402 9d03 a101 0100 7c00 a00d  j...d.......|...
-00000280: 7c02 a101 0100 7c00 a00e 7c01 a101 0100  |.....|...|.....
-00000290: 6400 5300 a903 4e7a 1262 6163 6b67 726f  d.S...Nz.backgro
-000002a0: 756e 642d 636f 6c6f 723a 23fa 013b 290f  und-color:#..;).
-000002b0: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
-000002c0: 5fda 0d73 6574 4672 616d 6553 7479 6c65  _..setFrameStyle
-000002d0: 7203 0000 00da 0651 4672 616d 65da 0548  r......QFrame..H
-000002e0: 4c69 6e65 da05 506c 6169 6eda 0d73 6574  Line..Plain..set
-000002f0: 5374 796c 6553 6865 6574 da03 6e73 66da  StyleSheet..nsf.
-00000300: 0367 7569 da0a 6e73 665f 636f 6c6f 7273  .gui..nsf_colors
-00000310: da0e 4e53 4643 6f6c 6f72 4865 7853 7472  ..NSFColorHexStr
-00000320: da06 4f72 616e 6765 da0e 7365 7446 6978  ..Orange..setFix
-00000330: 6564 4865 6967 6874 da09 7365 7448 6964  edHeight..setHid
-00000340: 6465 6e29 04da 0473 656c 6672 0c00 0000  den)...selfr....
-00000350: 720d 0000 00da 056b 6172 6773 a901 da09  r......kargs....
-00000360: 5f5f 636c 6173 735f 5fa9 00fa 4363 3a5c  __class__...Cc:\
-00000370: 6769 745c 7363 7269 7074 735f 7079 7468  git\scripts_pyth
-00000380: 6f6e 5f6c 6962 5c6e 616e 6f73 7572 665c  on_lib\nanosurf\
-00000390: 6c69 625c 6672 616d 6577 6f72 6b73 5c71  lib\frameworks\q
-000003a0: 745f 6170 705c 6170 705f 6775 692e 7079  t_app\app_gui.py
-000003b0: 7211 0000 0015 0000 0073 0a00 0000 0001  r........s......
-000003c0: 0c01 1601 1a01 0a01 7a16 4d65 6e75 5365  ........z.MenuSe
-000003d0: 7061 7261 746f 722e 5f5f 696e 6974 5f5f  parator.__init__
-000003e0: 2902 4672 0600 0000 2907 da08 5f5f 6e61  ).Fr....)...__na
-000003f0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000400: da0c 5f5f 7175 616c 6e61 6d65 5f5f da04  ..__qualname__..
-00000410: 626f 6f6c da03 696e 7472 1100 0000 da0d  bool..intr......
-00000420: 5f5f 636c 6173 7363 656c 6c5f 5f72 2200  __classcell__r".
-00000430: 0000 7222 0000 0072 2000 0000 7223 0000  ..r"...r ...r#..
-00000440: 0072 0a00 0000 1400 0000 7302 0000 0008  .r........s.....
-00000450: 0172 0a00 0000 6300 0000 0000 0000 0000  .r....c.........
-00000460: 0000 0000 0000 0004 0000 0000 0000 0073  ...............s
-00000470: 5400 0000 6500 5a01 6400 5a02 6503 a004  T...e.Z.d.Z.e...
-00000480: 6505 a101 5a06 6507 6505 6401 9c02 8700  e...Z.e.e.d.....
-00000490: 6601 6402 6403 840c 5a08 640d 6509 6405  f.d.d...Z.d.e.d.
-000004a0: 9c01 6406 6407 8405 5a0a 6408 6409 8400  ..d.d...Z.d.d...
-000004b0: 5a0b 6507 640a 9c01 640b 640c 8404 5a0c  Z.e.d...d.d...Z.
-000004c0: 8700 0400 5a0d 5300 290e da0a 4d65 6e75  ....Z.S.)...Menu
-000004d0: 4275 7474 6f6e 2902 da08 6d65 6e75 7465  Button)...menute
-000004e0: 7874 da08 6d65 6e75 6974 656d 6303 0000  xt..menuitemc...
-000004f0: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-00000500: 0003 0000 0073 3800 0000 7400 8300 a001  .....s8...t.....
-00000510: a100 0100 7c00 a002 7c01 a101 0100 7c00  ....|...|.....|.
-00000520: a003 6401 a101 0100 7c02 7c00 5f04 7c00  ..d.....|.|._.|.
-00000530: 6a05 6a06 a007 7c00 6a08 a101 0100 6400  j.j...|.j.....d.
-00000540: 5300 2902 4e46 2909 7210 0000 0072 1100  S.).NF).r....r..
-00000550: 0000 da0e 5f73 6574 7570 5f77 6964 6765  ...._setup_widge
-00000560: 7473 da0d 7365 745f 6869 6768 6c69 6768  ts..set_highligh
-00000570: 7472 2c00 0000 da07 5f62 7574 746f 6eda  tr,....._button.
-00000580: 0763 6c69 636b 6564 da07 636f 6e6e 6563  .clicked..connec
-00000590: 74da 0b5f 6f6e 5f63 6c69 636b 6564 2903  t.._on_clicked).
-000005a0: 721e 0000 0072 2b00 0000 722c 0000 0072  r....r+...r,...r
-000005b0: 2000 0000 7222 0000 0072 2300 0000 7211   ...r"...r#...r.
-000005c0: 0000 0020 0000 0073 0a00 0000 0001 0a01  ... ...s........
-000005d0: 0a01 0a01 0601 7a13 4d65 6e75 4275 7474  ......z.MenuButt
-000005e0: 6f6e 2e5f 5f69 6e69 745f 5f46 2901 da09  on.__init__F)...
-000005f0: 6869 6768 6c69 6768 7463 0200 0000 0000  highlightc......
-00000600: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
-00000610: 0000 7334 0000 007c 0172 1074 006a 016a  ..s4...|.r.t.j.j
-00000620: 026a 036a 046e 0a74 006a 016a 026a 036a  .j.j.n.t.j.j.j.j
-00000630: 057d 027c 006a 06a0 0764 017c 029b 0064  .}.|.j...d.|...d
-00000640: 029d 03a1 0101 0064 0053 0072 0e00 0000  .......d.S.r....
-00000650: 2908 7217 0000 0072 1800 0000 7219 0000  ).r....r....r...
-00000660: 0072 1a00 0000 721b 0000 00da 0953 6f66  .r....r......Sof
-00000670: 745f 4772 6179 da0c 5f6d 6172 6b65 725f  t_Gray.._marker_
-00000680: 6c69 6e65 7216 0000 0029 0372 1e00 0000  liner....).r....
-00000690: 7233 0000 00da 0563 6f6c 6f72 7222 0000  r3.....colorr"..
-000006a0: 0072 2200 0000 7223 0000 0072 2e00 0000  .r"...r#...r....
-000006b0: 2700 0000 7304 0000 0000 011c 017a 184d  '...s........z.M
-000006c0: 656e 7542 7574 746f 6e2e 7365 745f 6869  enuButton.set_hi
-000006d0: 6768 6c69 6768 7463 0100 0000 0000 0000  ghlightc........
-000006e0: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
-000006f0: 7312 0000 007c 006a 00a0 017c 006a 02a1  s....|.j...|.j..
-00000700: 0101 0064 0053 00a9 014e 2903 da13 7369  ...d.S...N)...si
-00000710: 675f 6f6e 5f6d 656e 755f 636c 6963 6b65  g_on_menu_clicke
-00000720: 64da 0465 6d69 7472 2c00 0000 a901 721e  d..emitr,.....r.
-00000730: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
-00000740: 0000 7232 0000 002b 0000 0073 0200 0000  ..r2...+...s....
-00000750: 0001 7a16 4d65 6e75 4275 7474 6f6e 2e5f  ..z.MenuButton._
-00000760: 6f6e 5f63 6c69 636b 6564 2901 da09 6c61  on_clicked)...la
-00000770: 6265 6c5f 7374 7263 0200 0000 0000 0000  bel_strc........
-00000780: 0000 0000 0300 0000 0600 0000 4300 0000  ............C...
-00000790: 7362 0000 0074 00a0 01a1 007d 027c 02a0  sb...t.....}.|..
-000007a0: 0264 01a1 0101 007c 02a0 0364 0164 0164  .d.....|...d.d.d
-000007b0: 0164 01a1 0401 0074 00a0 047c 01a1 017c  .d.....t...|...|
-000007c0: 005f 0574 0664 0264 0364 048d 027c 005f  ._.t.d.d.d...|._
-000007d0: 077c 02a0 087c 006a 07a1 0101 007c 02a0  .|...|.j.....|..
-000007e0: 087c 006a 05a1 0101 007c 00a0 097c 02a1  .|.j.....|...|..
-000007f0: 0101 0064 0053 0029 054e 7201 0000 0046  ...d.S.).Nr....F
-00000800: e902 0000 0072 0b00 0000 290a 7203 0000  .....r....).r...
-00000810: 00da 0b51 5642 6f78 4c61 796f 7574 da0a  ...QVBoxLayout..
-00000820: 7365 7453 7061 6369 6e67 da12 7365 7443  setSpacing..setC
-00000830: 6f6e 7465 6e74 734d 6172 6769 6e73 da0b  ontentsMargins..
-00000840: 5150 7573 6842 7574 746f 6e72 2f00 0000  QPushButtonr/...
-00000850: 720a 0000 0072 3500 0000 da09 6164 6457  r....r5.....addW
-00000860: 6964 6765 74da 0973 6574 4c61 796f 7574  idget..setLayout
-00000870: 2903 721e 0000 0072 3b00 0000 da06 6c61  ).r....r;.....la
-00000880: 796f 7574 7222 0000 0072 2200 0000 7223  youtr"...r"...r#
-00000890: 0000 0072 2d00 0000 2e00 0000 7310 0000  ...r-.......s...
-000008a0: 0000 0108 010a 0110 010c 010e 010c 010c  ................
-000008b0: 017a 194d 656e 7542 7574 746f 6e2e 5f73  .z.MenuButton._s
-000008c0: 6574 7570 5f77 6964 6765 7473 2901 4629  etup_widgets).F)
-000008d0: 0e72 2400 0000 7225 0000 0072 2600 0000  .r$...r%...r&...
-000008e0: 7205 0000 00da 0653 6967 6e61 6c72 2800  r......Signalr(.
-000008f0: 0000 7238 0000 00da 0373 7472 7211 0000  ..r8.....strr...
-00000900: 0072 2700 0000 722e 0000 0072 3200 0000  .r'...r....r2...
-00000910: 722d 0000 0072 2900 0000 7222 0000 0072  r-...r)...r"...r
-00000920: 2200 0000 7220 0000 0072 2300 0000 722a  "...r ...r#...r*
-00000930: 0000 001c 0000 0073 0a00 0000 0802 0a02  .......s........
-00000940: 1407 1004 0803 722a 0000 0063 0000 0000  ......r*...c....
-00000950: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000960: 0000 0000 731c 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
-00000970: 0287 0066 0164 0164 0284 085a 0387 0004  ...f.d.d...Z....
-00000980: 005a 0453 0029 03da 0a53 7464 5653 7061  .Z.S.)...StdVSpa
-00000990: 6365 7263 0100 0000 0000 0000 0000 0000  cerc............
-000009a0: 0100 0000 0600 0000 0300 0000 731e 0000  ............s...
-000009b0: 0074 0083 00a0 0174 0264 0174 036a 046a  .t.....t.d.t.j.j
-000009c0: 0574 036a 046a 06a1 0401 0064 0053 0029  .t.j.j.....d.S.)
-000009d0: 024e e928 0000 0029 0772 1000 0000 7211  .N.(...).r....r.
-000009e0: 0000 00da 1463 6f6e 7472 6f6c 5f6c 6179  .....control_lay
-000009f0: 6f75 745f 7769 6474 6872 0300 0000 da0b  out_widthr......
-00000a00: 5153 697a 6550 6f6c 6963 79da 0546 6978  QSizePolicy..Fix
-00000a10: 6564 da10 4d69 6e69 6d75 6d45 7870 616e  ed..MinimumExpan
-00000a20: 6469 6e67 723a 0000 0072 2000 0000 7222  dingr:...r ...r"
-00000a30: 0000 0072 2300 0000 7211 0000 003a 0000  ...r#...r....:..
-00000a40: 0073 0200 0000 0001 7a13 5374 6456 5370  .s......z.StdVSp
-00000a50: 6163 6572 2e5f 5f69 6e69 745f 5f29 0572  acer.__init__).r
-00000a60: 2400 0000 7225 0000 0072 2600 0000 7211  $...r%...r&...r.
-00000a70: 0000 0072 2900 0000 7222 0000 0072 2200  ...r)...r"...r".
-00000a80: 0000 7220 0000 0072 2300 0000 7246 0000  ..r ...r#...rF..
-00000a90: 0039 0000 0073 0200 0000 0801 7246 0000  .9...s......rF..
-00000aa0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000ab0: 0000 0500 0000 0000 0000 73f2 0000 0065  ..........s....e
-00000ac0: 005a 0164 005a 0287 0066 0164 0164 0284  .Z.d.Z...f.d.d..
-00000ad0: 085a 0365 0465 0464 039c 0264 0464 0584  .Z.e.e.d...d.d..
-00000ae0: 045a 0565 066a 076a 0866 0165 0465 066a  .Z.e.j.j.f.e.e.j
-00000af0: 0764 069c 0264 0764 0884 055a 0964 0964  .d...d.d...Z.d.d
-00000b00: 0a84 005a 0a64 0b64 0c84 005a 0b64 0d64  ...Z.d.d...Z.d.d
-00000b10: 0e84 005a 0c65 0d6a 0e64 0f9c 0164 1064  ...Z.e.j.d...d.d
-00000b20: 1184 045a 0f65 1064 129c 0164 1364 1484  ...Z.e.d...d.d..
-00000b30: 045a 1165 1064 159c 0164 1664 1784 045a  .Z.e.d...d.d...Z
-00000b40: 1265 1364 129c 0164 1864 1984 045a 1465  .e.d...d.d...Z.e
-00000b50: 1564 1a9c 0164 1b64 1c84 045a 1687 0066  .d...d.d...Z...f
-00000b60: 0164 1d64 1e84 085a 1765 0464 1f9c 0164  .d.d...Z.e.d...d
-00000b70: 2064 2184 045a 1865 1064 159c 0164 2264   d!..Z.e.d...d"d
-00000b80: 2384 045a 1964 2464 2584 005a 1a64 2c65  #..Z.d$d%..Z.d,e
-00000b90: 0465 0465 0464 279c 0364 2864 2984 055a  .e.e.d'..d(d)..Z
-00000ba0: 1b64 2a64 2b84 005a 1c87 0004 005a 1d53  .d*d+..Z.....Z.S
-00000bb0: 0029 2dda 0941 7070 5769 6e64 6f77 6302  .)-..AppWindowc.
-00000bc0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-00000bd0: 0000 0003 0000 0073 1400 0000 7400 8300  .......s....t...
-00000be0: a001 a100 0100 7c01 7c00 5f02 6400 5300  ......|.|._.d.S.
-00000bf0: 7237 0000 0029 0372 1000 0000 7211 0000  r7...).r....r...
-00000c00: 00da 0361 7070 2902 721e 0000 0072 4d00  ...app).r....rM.
-00000c10: 0000 7220 0000 0072 2200 0000 7223 0000  ..r ...r"...r#..
-00000c20: 0072 1100 0000 3e00 0000 7304 0000 0000  .r....>...s.....
-00000c30: 010a 017a 1241 7070 5769 6e64 6f77 2e5f  ...z.AppWindow._
-00000c40: 5f69 6e69 745f 5f29 02da 0d75 695f 7374  _init__)...ui_st
-00000c50: 796c 655f 6669 6c65 da09 6963 6f6e 5f66  yle_file..icon_f
-00000c60: 696c 6563 0300 0000 0000 0000 0000 0000  ilec............
-00000c70: 0400 0000 0600 0000 4300 0000 731c 0100  ........C...s...
-00000c80: 007c 00a0 007c 01a1 017d 037c 00a0 017c  .|...|...}.|...|
-00000c90: 03a1 0101 007c 00a0 027c 006a 036a 04a1  .....|...|.j.j..
-00000ca0: 0101 007c 00a0 0574 06a0 0774 087c 0283  ...|...t...t.|..
-00000cb0: 01a1 01a1 0101 007c 00a0 09a1 00a0 0a64  .......|.......d
-00000cc0: 01a1 0101 0074 0ba0 0ca1 007c 005f 0d74  .....t.....|._.t
-00000cd0: 0ba0 0ea1 007c 005f 0f74 0ba0 10a1 007c  .....|._.t.....|
-00000ce0: 005f 1174 126a 136a 1464 0264 038d 017c  ._.t.j.j.d.d...|
-00000cf0: 005f 1574 0ba0 16a1 007c 005f 177c 006a  ._.t.....|._.|.j
-00000d00: 17a0 1874 0ba0 1964 04a1 01a1 0101 0074  ...t...d.......t
-00000d10: 1a64 0264 038d 017c 005f 1b74 1a64 0564  .d.d...|._.t.d.d
-00000d20: 038d 017c 005f 1c7c 006a 0fa0 1d7c 006a  ...|._.|.j...|.j
-00000d30: 1164 06a1 0201 007c 006a 0fa0 187c 006a  .d.....|.j...|.j
-00000d40: 1b64 07a1 0201 007c 006a 0fa0 187c 006a  .d.....|.j...|.j
-00000d50: 1564 08a1 0201 007c 006a 0fa0 1d7c 006a  .d.....|.j...|.j
-00000d60: 1764 09a1 0201 007c 006a 0fa0 187c 006a  .d.....|.j...|.j
-00000d70: 1c64 0aa1 0201 007c 006a 0da0 1e7c 006a  .d.....|.j...|.j
-00000d80: 0fa1 0101 007c 00a0 1f7c 006a 0da1 0101  .....|...|.j....
-00000d90: 007c 00a0 20a1 0001 0064 0053 0029 0b4e  .|.. ....d.S.).N
-00000da0: 5a05 5265 6164 7954 2901 720c 0000 007a  Z.ReadyT).r....z
-00000db0: 0b4d 6169 6e20 7363 7265 656e 4672 0100  .Main screenFr..
-00000dc0: 0000 7206 0000 0072 3c00 0000 e903 0000  ..r....r<.......
-00000dd0: 00e9 0400 0000 2921 da1a 5f72 6561 645f  ......)!.._read_
-00000de0: 7374 796c 655f 7368 6565 745f 696e 746f  style_sheet_into
-00000df0: 5f73 7472 7216 0000 00da 0e73 6574 5769  _strr......setWi
-00000e00: 6e64 6f77 5469 746c 6572 4d00 0000 da0d  ndowTitlerM.....
-00000e10: 6170 705f 6e61 6d65 5f6c 6f6e 67da 0d73  app_name_long..s
-00000e20: 6574 5769 6e64 6f77 4963 6f6e 7204 0000  etWindowIconr...
-00000e30: 00da 0551 4963 6f6e 7245 0000 00da 0973  ...QIconrE.....s
-00000e40: 7461 7475 7342 6172 da0b 7368 6f77 4d65  tatusBar..showMe
-00000e50: 7373 6167 6572 0300 0000 da07 5157 6964  ssager......QWid
-00000e60: 6765 745a 0a6d 6169 6e53 6372 6565 6e72  getZ.mainScreenr
-00000e70: 3d00 0000 5a0b 6d61 696e 5f6c 6179 6f75  =...Z.main_layou
-00000e80: 74da 0b51 4842 6f78 4c61 796f 7574 da09  t..QHBoxLayout..
-00000e90: 6d61 696e 5f6d 656e 7572 1700 0000 7218  main_menur....r.
-00000ea0: 0000 00da 0a4e 5346 496e 666f 426f 78da  .....NSFInfoBox.
-00000eb0: 0f6d 6169 6e5f 6d65 7373 6167 6562 6f78  .main_messagebox
-00000ec0: da0e 5153 7461 636b 6564 4c61 796f 7574  ..QStackedLayout
-00000ed0: da0a 6d61 696e 5f73 7461 636b 7241 0000  ..main_stackrA..
-00000ee0: 00da 0651 4c61 6265 6c72 0a00 0000 da08  ...QLabelr......
-00000ef0: 6d65 6e75 5f73 6570 5a0a 7374 6174 7573  menu_sepZ.status
-00000f00: 5f73 6570 da09 6164 644c 6179 6f75 7472  _sep..addLayoutr
-00000f10: 4200 0000 da10 7365 7443 656e 7472 616c  B.....setCentral
-00000f20: 5769 6467 6574 da10 6c6f 6164 5f77 696e  Widget..load_win
-00000f30: 646f 775f 7369 7a65 2904 721e 0000 0072  dow_size).r....r
-00000f40: 4e00 0000 724f 0000 005a 0f73 7479 6c65  N...rO...Z.style
-00000f50: 5f73 6865 6574 5f73 7472 7222 0000 0072  _sheet_strr"...r
-00000f60: 2200 0000 7223 0000 00da 0a63 7265 6174  "...r#.....creat
-00000f70: 655f 6775 6942 0000 0073 2a00 0000 0002  e_guiB...s*.....
-00000f80: 0a01 0a01 0e01 1401 0e04 0a01 0a01 0a01  ................
-00000f90: 1001 0a01 1202 0c01 0c01 1001 1001 1001  ................
-00000fa0: 1001 1002 0e01 0c01 7a14 4170 7057 696e  ........z.AppWin
-00000fb0: 646f 772e 6372 6561 7465 5f67 7569 2902  dow.create_gui).
-00000fc0: da03 6d73 67da 086d 7367 5f74 7970 6563  ..msg..msg_typec
-00000fd0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-00000fe0: 0400 0000 4300 0000 735a 0000 007c 0274  ....C...sZ...|.t
-00000ff0: 006a 016a 026b 0272 247c 006a 037c 0174  .j.j.k.r$|.j.|.t
-00001000: 046a 056a 066a 076a 0864 018d 0201 006e  .j.j.j.j.d.....n
-00001010: 327c 0274 006a 016a 096b 0272 487c 006a  2|.t.j.j.k.rH|.j
-00001020: 037c 0174 046a 056a 066a 076a 0864 018d  .|.t.j.j.j.j.d..
-00001030: 0201 006e 0e7c 00a0 0aa1 00a0 0b7c 01a1  ...n.|.......|..
-00001040: 0101 0064 0053 0029 024e 2901 da10 6261  ...d.S.).N)...ba
-00001050: 636b 6772 6f75 6e64 5f63 6f6c 6f72 290c  ckground_color).
-00001060: 7207 0000 00da 074d 7367 5479 7065 da05  r......MsgType..
-00001070: 4572 726f 72da 0d73 686f 775f 696e 666f  Error..show_info
-00001080: 5f62 6f78 7217 0000 0072 1800 0000 7219  _boxr....r....r.
-00001090: 0000 0072 1a00 0000 721b 0000 00da 0457  ...r....r......W
-000010a0: 6172 6e72 5700 0000 7258 0000 0029 0372  arnrW...rX...).r
-000010b0: 1e00 0000 7266 0000 0072 6700 0000 7222  ....rf...rg...r"
-000010c0: 0000 0072 2200 0000 7223 0000 00da 0c73  ...r"...r#.....s
-000010d0: 686f 775f 6d65 7373 6167 655f 0000 0073  how_message_...s
-000010e0: 0a00 0000 0001 0c01 1801 0c01 1802 7a16  ..............z.
-000010f0: 4170 7057 696e 646f 772e 7368 6f77 5f6d  AppWindow.show_m
-00001100: 6573 7361 6765 6301 0000 0000 0000 0000  essagec.........
-00001110: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-00001120: 1a00 0000 7c00 a000 a100 a001 6401 a101  ....|.......d...
-00001130: 0100 7c00 a002 a100 0100 6400 5300 a902  ..|.......d.S...
-00001140: 4eda 0029 0372 5700 0000 7258 0000 00da  N..).rW...rX....
-00001150: 0d68 6964 655f 696e 666f 5f62 6f78 723a  .hide_info_boxr:
-00001160: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
-00001170: 0000 da0c 6869 6465 5f6d 6573 7361 6765  ....hide_message
-00001180: 6700 0000 7304 0000 0000 010e 017a 1641  g...s........z.A
-00001190: 7070 5769 6e64 6f77 2e68 6964 655f 6d65  ppWindow.hide_me
-000011a0: 7373 6167 6563 0100 0000 0000 0000 0000  ssagec..........
-000011b0: 0000 0100 0000 0500 0000 4300 0000 732c  ..........C...s,
-000011c0: 0000 007c 006a 006a 01a0 0264 017c 00a0  ...|.j.j...d.|..
-000011d0: 03a1 00a1 0201 007c 006a 006a 01a0 0264  .......|.j.j...d
-000011e0: 027c 00a0 04a1 00a1 0201 0064 0053 00a9  .|.........d.S..
-000011f0: 034e da08 6765 6f6d 6574 7279 da0b 7769  .N..geometry..wi
-00001200: 6e64 6f77 5374 6174 6529 0572 4d00 0000  ndowState).rM...
-00001210: da08 7265 6769 7374 7279 da08 7365 7456  ..registry..setV
-00001220: 616c 7565 da0c 7361 7665 4765 6f6d 6574  alue..saveGeomet
-00001230: 7279 da09 7361 7665 5374 6174 6572 3a00  ry..saveStater:.
-00001240: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
-00001250: 00da 1073 6176 655f 7769 6e64 6f77 5f73  ...save_window_s
-00001260: 697a 656b 0000 0073 0400 0000 0001 1401  izek...s........
-00001270: 7a1a 4170 7057 696e 646f 772e 7361 7665  z.AppWindow.save
-00001280: 5f77 696e 646f 775f 7369 7a65 6301 0000  _window_sizec...
-00001290: 0000 0000 0000 0000 0001 0000 0005 0000  ................
-000012a0: 0043 0000 0073 2c00 0000 7c00 a000 7c00  .C...s,...|...|.
-000012b0: 6a01 6a02 a003 6401 a101 a101 0100 7c00  j.j...d.......|.
-000012c0: a004 7c00 6a01 6a02 a003 6402 a101 a101  ..|.j.j...d.....
-000012d0: 0100 6400 5300 7272 0000 0029 05da 0f72  ..d.S.rr...)...r
-000012e0: 6573 746f 7265 4765 6f6d 6574 7279 724d  estoreGeometryrM
-000012f0: 0000 0072 7500 0000 da05 7661 6c75 65da  ...ru.....value.
-00001300: 0c72 6573 746f 7265 5374 6174 6572 3a00  .restoreStater:.
-00001310: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
-00001320: 0072 6400 0000 6f00 0000 7304 0000 0000  .rd...o...s.....
-00001330: 0114 017a 1a41 7070 5769 6e64 6f77 2e6c  ...z.AppWindow.l
-00001340: 6f61 645f 7769 6e64 6f77 5f73 697a 6529  oad_window_size)
-00001350: 01da 066d 6f64 756c 6563 0200 0000 0000  ...modulec......
-00001360: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-00001370: 0000 733c 0000 007c 016a 007d 0274 017c  ..s<...|.j.}.t.|
-00001380: 0274 026a 0383 0272 387c 006a 04a0 057c  .t.j...r8|.j...|
-00001390: 02a1 0101 007c 006a 04a0 06a1 0064 016b  .....|.j.....d.k
-000013a0: 0272 387c 006a 04a0 077c 02a1 0101 0064  .r8|.j...|.....d
-000013b0: 0053 0029 024e 7201 0000 0029 0872 1800  .S.).Nr....).r..
-000013c0: 0000 da0a 6973 696e 7374 616e 6365 7203  ....isinstancer.
-000013d0: 0000 0072 5900 0000 725f 0000 0072 4100  ...rY...r_...rA.
-000013e0: 0000 da0c 6375 7272 656e 7449 6e64 6578  ....currentIndex
-000013f0: da10 7365 7443 7572 7265 6e74 5769 6467  ..setCurrentWidg
-00001400: 6574 2903 721e 0000 0072 7d00 0000 5a0a  et).r....r}...Z.
-00001410: 6d6f 6475 6c65 5f67 7569 7222 0000 0072  module_guir"...r
-00001420: 2200 0000 7223 0000 00da 0a61 6464 5f73  "...r#.....add_s
-00001430: 6372 6565 6e73 0000 0073 0a00 0000 0001  creens...s......
-00001440: 0601 0c01 0c02 0e01 7a14 4170 7057 696e  ........z.AppWin
-00001450: 646f 772e 6164 645f 7363 7265 656e 2901  dow.add_screen).
-00001460: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
-00001470: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00001480: 0073 0e00 0000 7c00 6a00 a001 a100 6401  .s....|.j.....d.
-00001490: 1800 5300 a902 4e72 0600 0000 2902 725f  ..S...Nr....).r_
-000014a0: 0000 0072 7f00 0000 723a 0000 0072 2200  ...r....r:...r".
-000014b0: 0000 7222 0000 0072 2300 0000 da17 6765  ..r"...r#.....ge
-000014c0: 745f 6163 7469 7665 5f6d 6f64 756c 655f  t_active_module_
-000014d0: 696e 6465 787b 0000 0073 0200 0000 0001  index{...s......
-000014e0: 7a21 4170 7057 696e 646f 772e 6765 745f  z!AppWindow.get_
-000014f0: 6163 7469 7665 5f6d 6f64 756c 655f 696e  active_module_in
-00001500: 6465 7829 01da 0569 6e64 6578 6302 0000  dex)...indexc...
-00001510: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00001520: 0043 0000 0073 1c00 0000 7c00 6a00 a001  .C...s....|.j...
-00001530: 7c01 6401 1700 a101 0100 7c00 a002 a100  |.d.......|.....
-00001540: 0100 6400 5300 7283 0000 0029 0372 5f00  ..d.S.r....).r_.
-00001550: 0000 da0f 7365 7443 7572 7265 6e74 496e  ....setCurrentIn
-00001560: 6465 78da 1d5f 7570 6461 7465 5f6d 656e  dex.._update_men
-00001570: 755f 6275 7474 6f6e 5f68 6967 686c 6967  u_button_highlig
-00001580: 6874 a902 721e 0000 0072 8500 0000 7222  ht..r....r....r"
-00001590: 0000 0072 2200 0000 7223 0000 00da 1a73  ...r"...r#.....s
-000015a0: 6574 5f61 6374 6976 655f 6d6f 6475 6c65  et_active_module
-000015b0: 5f62 795f 696e 6465 787e 0000 0073 0400  _by_index~...s..
-000015c0: 0000 0001 1001 7a24 4170 7057 696e 646f  ......z$AppWindo
-000015d0: 772e 7365 745f 6163 7469 7665 5f6d 6f64  w.set_active_mod
-000015e0: 756c 655f 6279 5f69 6e64 6578 6301 0000  ule_by_indexc...
-000015f0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00001600: 0043 0000 0073 0e00 0000 7c00 6a00 a001  .C...s....|.j...
-00001610: a100 6401 6b04 5300 7283 0000 0029 0272  ..d.k.S.r....).r
-00001620: 4d00 0000 da10 6765 745f 6d6f 6475 6c65  M.....get_module
-00001630: 5f63 6f75 6e74 723a 0000 0072 2200 0000  _countr:...r"...
-00001640: 7222 0000 0072 2300 0000 da0f 6973 5f6d  r"...r#.....is_m
-00001650: 656e 755f 7669 7369 626c 6582 0000 0073  enu_visible....s
-00001660: 0200 0000 0001 7a19 4170 7057 696e 646f  ......z.AppWindo
-00001670: 772e 6973 5f6d 656e 755f 7669 7369 626c  w.is_menu_visibl
-00001680: 6529 01da 076d 6f64 756c 6573 6302 0000  e)...modulesc...
-00001690: 0000 0000 0000 0000 0007 0000 0004 0000  ................
-000016a0: 0043 0000 0073 c400 0000 6401 7d02 7c01  .C...s....d.}.|.
-000016b0: a000 a100 4400 5d16 7d03 7c03 6a01 6400  ....D.].}.|.j.d.
-000016c0: 7501 720c 7c02 6402 3700 7d02 710c 7c02  u.r.|.d.7.}.q.|.
-000016d0: 6402 6b04 72b0 7c00 6a02 a003 a100 725c  d.k.r.|.j.....r\
-000016e0: 7c00 6a02 a004 6401 a101 7d04 7c04 a005  |.j...d...}.|...
-000016f0: a100 6400 7501 722c 7c04 a005 a100 a006  ..d.u.r,|.......
-00001700: a100 0100 712c 6401 7d05 7c01 a000 a100  ....q,d.}.|.....
-00001710: 4400 5d3c 7d03 7c03 6a01 6400 7501 7268  D.]<}.|.j.d.u.rh
-00001720: 7407 7c03 6a08 7c05 8302 7d06 7c06 6a09  t.|.j.|...}.|.j.
-00001730: a00a 7c00 6a0b a101 0100 7c00 6a02 a00c  ..|.j.....|.j...
-00001740: 7c06 a101 0100 7c05 6402 3700 7d05 7168  |.....|.d.7.}.qh
-00001750: 7c00 6a02 a00d a100 0100 7c00 6a0e a00f  |.j.......|.j...
-00001760: 7c02 6402 6b01 a101 0100 6400 5300 2903  |.d.k.....d.S.).
-00001770: 4e72 0100 0000 7206 0000 0029 10da 0676  Nr....r....)...v
-00001780: 616c 7565 7372 1800 0000 725b 0000 00da  aluesr....r[....
-00001790: 0563 6f75 6e74 da06 7461 6b65 4174 da06  .count..takeAt..
-000017a0: 7769 6467 6574 da0b 6465 6c65 7465 4c61  widget..deleteLa
-000017b0: 7465 7272 2a00 0000 da04 6e61 6d65 7238  terr*.....namer8
-000017c0: 0000 0072 3100 0000 da17 5f6f 6e5f 6d65  ...r1....._on_me
-000017d0: 6e75 5f62 7574 746f 6e5f 636c 6963 6b65  nu_button_clicke
-000017e0: 6472 4100 0000 da0a 6164 6453 7472 6574  drA.....addStret
-000017f0: 6368 7261 0000 0072 1d00 0000 2907 721e  chra...r....).r.
-00001800: 0000 0072 8c00 0000 5a0c 6d6f 645f 7769  ...r....Z.mod_wi
-00001810: 7468 5f67 7569 da03 6d6f 64da 0563 6869  th_gui..mod..chi
-00001820: 6c64 5a09 6d65 6e75 696e 6465 7872 2c00  ldZ.menuindexr,.
-00001830: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
-00001840: 00da 0b75 7064 6174 655f 6d65 6e75 8500  ...update_menu..
-00001850: 0000 7324 0000 0000 0104 010c 010a 010a  ..s$............
-00001860: 0308 020a 010c 010c 010e 0304 010c 010a  ................
-00001870: 010c 010e 010c 010a 010a 027a 1541 7070  ...........z.App
-00001880: 5769 6e64 6f77 2e75 7064 6174 655f 6d65  Window.update_me
-00001890: 6e75 6302 0000 0000 0000 0000 0000 0002  nuc.............
-000018a0: 0000 0003 0000 0003 0000 0073 1800 0000  ...........s....
-000018b0: 7c00 a000 a100 0100 7401 8300 a002 7c01  |.......t.....|.
-000018c0: a101 0100 6401 5300 2902 7a2d 2063 6170  ....d.S.).z- cap
-000018d0: 7475 7265 2063 6c6f 7365 2062 7574 746f  ture close butto
-000018e0: 6e20 6672 6f6d 2061 7070 6c69 6361 7469  n from applicati
-000018f0: 6f6e 2077 696e 646f 774e 2903 7279 0000  on windowN).ry..
-00001900: 0072 1000 0000 da0a 636c 6f73 6545 7665  .r......closeEve
-00001910: 6e74 2902 721e 0000 00da 0361 7267 7220  nt).r......argr 
-00001920: 0000 0072 2200 0000 7223 0000 0072 9800  ...r"...r#...r..
-00001930: 0000 a100 0000 7304 0000 0000 0208 017a  ......s........z
-00001940: 1441 7070 5769 6e64 6f77 2e63 6c6f 7365  .AppWindow.close
-00001950: 4576 656e 7429 01da 0a73 7479 6c65 5f66  Event)...style_f
-00001960: 696c 6563 0200 0000 0000 0000 0000 0000  ilec............
-00001970: 0400 0000 0800 0000 4300 0000 7338 0000  ........C...s8..
-00001980: 0064 017d 0274 007c 0183 018f 187d 037c  .d.}.t.|.....}.|
-00001990: 03a0 01a1 007d 0257 0064 0004 0004 0083  .....}.W.d......
-000019a0: 0301 006e 1031 0073 2a30 0001 0001 0001  ...n.1.s*0......
-000019b0: 0059 0001 007c 0253 0072 6e00 0000 2902  .Y...|.S.rn...).
-000019c0: da04 6f70 656e da04 7265 6164 2904 721e  ..open..read).r.
-000019d0: 0000 0072 9a00 0000 da05 7374 796c 65da  ...r......style.
-000019e0: 0166 7222 0000 0072 2200 0000 7223 0000  .fr"...r"...r#..
-000019f0: 0072 5200 0000 a600 0000 7308 0000 0000  .rR.......s.....
-00001a00: 0104 010a 0126 017a 2441 7070 5769 6e64  .....&.z$AppWind
-00001a10: 6f77 2e5f 7265 6164 5f73 7479 6c65 5f73  ow._read_style_s
-00001a20: 6865 6574 5f69 6e74 6f5f 7374 7263 0200  heet_into_strc..
-00001a30: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00001a40: 0000 4300 0000 7310 0000 007c 006a 00a0  ..C...s....|.j..
-00001a50: 017c 01a1 0101 0064 0053 0072 3700 0000  .|.....d.S.r7...
-00001a60: 2902 724d 0000 00da 0f61 6374 6976 6174  ).rM.....activat
-00001a70: 655f 6d6f 6475 6c65 7288 0000 0072 2200  e_moduler....r".
-00001a80: 0000 7222 0000 0072 2300 0000 7293 0000  ..r"...r#...r...
-00001a90: 00ac 0000 0073 0200 0000 0001 7a21 4170  .....s......z!Ap
-00001aa0: 7057 696e 646f 772e 5f6f 6e5f 6d65 6e75  pWindow._on_menu
-00001ab0: 5f62 7574 746f 6e5f 636c 6963 6b65 6463  _button_clickedc
-00001ac0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00001ad0: 0500 0000 4300 0000 7346 0000 007c 00a0  ....C...sF...|..
-00001ae0: 00a1 0072 427c 00a0 01a1 007d 0174 027c  ...rB|.....}.t.|
-00001af0: 006a 03a0 04a1 0064 0118 0083 0144 005d  .j.....d.....D.]
-00001b00: 1e7d 027c 006a 03a0 057c 02a1 01a0 06a1  .}.|.j...|......
-00001b10: 00a0 077c 027c 016b 02a1 0101 0071 2264  ...|.|.k.....q"d
-00001b20: 0053 0072 8300 0000 2908 728b 0000 0072  .S.r....).r....r
-00001b30: 8400 0000 da05 7261 6e67 6572 5b00 0000  ......ranger[...
-00001b40: 728e 0000 00da 0669 7465 6d41 7472 9000  r......itemAtr..
-00001b50: 0000 722e 0000 0029 0372 1e00 0000 5a0c  ..r....).r....Z.
-00001b60: 6163 7469 7665 5f69 6e64 6578 da01 6972  active_index..ir
-00001b70: 2200 0000 7222 0000 0072 2300 0000 7287  "...r"...r#...r.
-00001b80: 0000 00af 0000 0073 0800 0000 0001 0801  .......s........
-00001b90: 0801 1601 7a27 4170 7057 696e 646f 772e  ....z'AppWindow.
-00001ba0: 5f75 7064 6174 655f 6d65 6e75 5f62 7574  _update_menu_but
-00001bb0: 746f 6e5f 6869 6768 6c69 6768 7472 6f00  ton_highlightro.
-00001bc0: 0000 2903 7266 0000 0072 6800 0000 da0a  ..).rf...rh.....
-00001bd0: 7465 7874 5f63 6f6c 6f72 6304 0000 0000  text_colorc.....
-00001be0: 0000 0000 0000 0004 0000 0003 0000 0043  ...............C
-00001bf0: 0000 0073 3c00 0000 7c00 6a00 a001 7c02  ...s<...|.j...|.
-00001c00: a101 0100 7c03 6401 6b03 7220 7c00 6a00  ....|.d.k.r |.j.
-00001c10: a002 7c03 a101 0100 7c00 6a00 a003 7c01  ..|.....|.j...|.
-00001c20: a101 0100 7c00 6a00 a004 6402 a101 0100  ....|.j...d.....
-00001c30: 6400 5300 2903 4e72 6f00 0000 4629 0572  d.S.).Nro...F).r
-00001c40: 5d00 0000 da14 7365 745f 6261 636b 6772  ].....set_backgr
-00001c50: 6f75 6e64 5f63 6f6c 6f72 da0e 7365 745f  ound_color..set_
-00001c60: 7465 7874 5f63 6f6c 6f72 da0b 7365 745f  text_color..set_
-00001c70: 6d65 7373 6167 6572 1d00 0000 2904 721e  messager....).r.
-00001c80: 0000 0072 6600 0000 7268 0000 0072 a300  ...rf...rh...r..
-00001c90: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
-00001ca0: 0072 6b00 0000 b500 0000 730a 0000 0000  .rk.......s.....
-00001cb0: 010c 0108 010c 010c 017a 1741 7070 5769  .........z.AppWi
-00001cc0: 6e64 6f77 2e73 686f 775f 696e 666f 5f62  ndow.show_info_b
-00001cd0: 6f78 6301 0000 0000 0000 0000 0000 0001  oxc.............
-00001ce0: 0000 0003 0000 0043 0000 0073 1000 0000  .......C...s....
-00001cf0: 7c00 6a00 a001 6401 a101 0100 6400 5300  |.j...d.....d.S.
-00001d00: 2902 4e54 2902 725d 0000 0072 1d00 0000  ).NT).r]...r....
-00001d10: 723a 0000 0072 2200 0000 7222 0000 0072  r:...r"...r"...r
-00001d20: 2300 0000 7270 0000 00bc 0000 0073 0200  #...rp.......s..
-00001d30: 0000 0001 7a17 4170 7057 696e 646f 772e  ....z.AppWindow.
-00001d40: 6869 6465 5f69 6e66 6f5f 626f 7829 0172  hide_info_box).r
-00001d50: 6f00 0000 291e 7224 0000 0072 2500 0000  o...).r$...r%...
-00001d60: 7226 0000 0072 1100 0000 7245 0000 0072  r&...r....rE...r
-00001d70: 6500 0000 7207 0000 0072 6900 0000 da04  e...r....ri.....
-00001d80: 496e 666f 726d 0000 0072 7100 0000 7279  Inform...rq...ry
-00001d90: 0000 0072 6400 0000 7208 0000 00da 0a4d  ...rd...r......M
-00001da0: 6f64 756c 6542 6173 6572 8100 0000 7228  oduleBaser....r(
-00001db0: 0000 0072 8400 0000 7289 0000 0072 2700  ...r....r....r'.
-00001dc0: 0000 728b 0000 00da 0464 6963 7472 9700  ..r......dictr..
-00001dd0: 0000 7298 0000 0072 5200 0000 7293 0000  ..r....rR...r...
-00001de0: 0072 8700 0000 726b 0000 0072 7000 0000  .r....rk...rp...
-00001df0: 7229 0000 0072 2200 0000 7222 0000 0072  r)...r"...r"...r
-00001e00: 2000 0000 7223 0000 0072 4c00 0000 3d00   ...r#...rL...=.
-00001e10: 0000 7322 0000 0008 010c 0410 1d1a 0808  ..s"............
-00001e20: 0408 0408 0410 080e 030e 040e 030e 1c0c  ................
-00001e30: 050e 060e 0308 0614 0772 4c00 0000 2916  .........rL...).
-00001e40: da07 5f5f 646f 635f 5fda 1e6e 616e 6f73  ..__doc__..nanos
-00001e50: 7572 662e 6c69 622e 6775 692e 696d 706f  urf.lib.gui.impo
-00001e60: 7274 5f68 656c 7065 7272 0200 0000 da07  rt_helperr......
-00001e70: 5079 5369 6465 3272 0300 0000 7204 0000  PySide2r....r...
-00001e80: 0072 0500 0000 da07 5079 5369 6465 36da  .r......PySide6.
-00001e90: 086e 616e 6f73 7572 6672 1700 0000 726f  .nanosurfr....ro
-00001ea0: 0000 0072 0700 0000 7208 0000 0072 4800  ...r....r....rH.
-00001eb0: 0000 7213 0000 0072 0a00 0000 7259 0000  ..r....r....rY..
-00001ec0: 0072 2a00 0000 da0b 5153 7061 6365 7249  .r*.....QSpacerI
-00001ed0: 7465 6d72 4600 0000 da0b 514d 6169 6e57  temrF.....QMainW
-00001ee0: 696e 646f 7772 4c00 0000 7222 0000 0072  indowrL...r"...r
-00001ef0: 2200 0000 7222 0000 0072 2300 0000 da08  "...r"...r#.....
-00001f00: 3c6d 6f64 756c 653e 0100 0000 731a 0000  <module>....s...
-00001f10: 0004 050c 0106 010c 0116 020c 0114 0208  ................
-00001f20: 0210 0204 0212 0812 1d12 04              ...........
+00000080: 6d06 5a06 0100 6401 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
+00000090: 0100 6401 6406 6c0a 5a0b 6407 6408 6c0c  ..d.d.l.Z.d.d.l.
+000000a0: 6d0d 5a0d 6d0e 5a0e 0100 6409 5a0f 4700  m.Z.m.Z...d.Z.G.
+000000b0: 640a 640b 8400 640b 6504 6a10 8303 5a11  d.d...d.e.j...Z.
+000000c0: 4700 640c 640d 8400 640d 6504 6a12 8303  G.d.d...d.e.j...
+000000d0: 5a13 4700 640e 640f 8400 640f 6504 6a14  Z.G.d.d...d.e.j.
+000000e0: 8303 5a15 6509 4700 6410 6411 8400 6411  ..Z.e.G.d.d...d.
+000000f0: 8302 8301 5a16 4700 6412 6413 8400 6413  ....Z.G.d.d...d.
+00000100: 6504 6a17 8303 5a18 6406 5300 2914 7a4f  e.j...Z.d.S.).zO
+00000110: 2054 6865 2047 5549 206f 6620 7468 6520   The GUI of the 
+00000120: 6170 706c 6963 6174 696f 6e20 6672 616d  application fram
+00000130: 6577 6f72 6b0a 436f 7079 7269 6768 7420  ework.Copyright 
+00000140: 4e61 6e6f 7375 7266 2041 4720 3230 3231  Nanosurf AG 2021
+00000150: 0a4c 6963 656e 7365 202d 204d 4954 0ae9  .License - MIT..
+00000160: 0000 0000 2901 da22 696d 706f 7274 5f70  ....).."import_p
+00000170: 7973 6964 6532 5f69 665f 6e6f 6e65 5f69  yside2_if_none_i
+00000180: 735f 6465 7465 6374 6564 2901 da09 5174  s_detected)...Qt
+00000190: 5769 6467 6574 7329 03da 0551 7447 7569  Widgets)...QtGui
+000001a0: 7203 0000 00da 0651 7443 6f72 6529 01da  r......QtCore)..
+000001b0: 0964 6174 6163 6c61 7373 4ee9 0100 0000  .dataclassN.....
+000001c0: 2902 da0a 6170 705f 636f 6d6d 6f6e da0b  )...app_common..
+000001d0: 6d6f 6475 6c65 5f62 6173 65e9 c800 0000  module_base.....
+000001e0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000001f0: 0005 0000 0000 0000 0073 2600 0000 6500  .........s&...e.
+00000200: 5a01 6400 5a02 6406 6503 6504 6403 9c02  Z.d.Z.d.e.e.d...
+00000210: 8700 6601 6404 6405 840d 5a05 8700 0400  ..f.d.d...Z.....
+00000220: 5a06 5300 2907 da0d 4d65 6e75 5365 7061  Z.S.)...MenuSepa
+00000230: 7261 746f 7246 7207 0000 00a9 02da 0668  ratorFr........h
+00000240: 6964 6465 6eda 0668 6569 6768 7463 0300  idden..heightc..
+00000250: 0000 0000 0000 0000 0000 0400 0000 0500  ................
+00000260: 0000 0b00 0000 7354 0000 0074 0083 006a  ......sT...t...j
+00000270: 017c 038e 0001 007c 00a0 0274 036a 046a  .|.....|...t.j.j
+00000280: 0574 036a 046a 0642 00a1 0101 007c 00a0  .t.j.j.B.....|..
+00000290: 0764 0174 086a 096a 0a6a 0b6a 0c9b 0064  .d.t.j.j.j.j...d
+000002a0: 029d 03a1 0101 007c 00a0 0d7c 02a1 0101  .......|...|....
+000002b0: 007c 00a0 0e7c 01a1 0101 0064 0053 00a9  .|...|.....d.S..
+000002c0: 034e 7a12 6261 636b 6772 6f75 6e64 2d63  .Nz.background-c
+000002d0: 6f6c 6f72 3a23 fa01 3b29 0fda 0573 7570  olor:#..;)...sup
+000002e0: 6572 da08 5f5f 696e 6974 5f5f da0d 7365  er..__init__..se
+000002f0: 7446 7261 6d65 5374 796c 6572 0300 0000  tFrameStyler....
+00000300: da06 5146 7261 6d65 da05 484c 696e 65da  ..QFrame..HLine.
+00000310: 0550 6c61 696e da0d 7365 7453 7479 6c65  .Plain..setStyle
+00000320: 5368 6565 74da 036e 7366 da03 6775 69da  Sheet..nsf..gui.
+00000330: 0a6e 7366 5f63 6f6c 6f72 73da 0e4e 5346  .nsf_colors..NSF
+00000340: 436f 6c6f 7248 6578 5374 72da 064f 7261  ColorHexStr..Ora
+00000350: 6e67 65da 0e73 6574 4669 7865 6448 6569  nge..setFixedHei
+00000360: 6768 74da 0973 6574 4869 6464 656e 2904  ght..setHidden).
+00000370: da04 7365 6c66 720d 0000 0072 0e00 0000  ..selfr....r....
+00000380: da05 6b61 7267 73a9 01da 095f 5f63 6c61  ..kargs....__cla
+00000390: 7373 5f5f a900 fa43 633a 5c67 6974 5c73  ss__...Cc:\git\s
+000003a0: 6372 6970 7473 5f70 7974 686f 6e5f 6c69  cripts_python_li
+000003b0: 625c 6e61 6e6f 7375 7266 5c6c 6962 5c66  b\nanosurf\lib\f
+000003c0: 7261 6d65 776f 726b 735c 7174 5f61 7070  rameworks\qt_app
+000003d0: 5c61 7070 5f67 7569 2e70 7972 1200 0000  \app_gui.pyr....
+000003e0: 1500 0000 730a 0000 0000 010c 0116 011a  ....s...........
+000003f0: 010a 017a 164d 656e 7553 6570 6172 6174  ...z.MenuSeparat
+00000400: 6f72 2e5f 5f69 6e69 745f 5f29 0246 7207  or.__init__).Fr.
+00000410: 0000 0029 07da 085f 5f6e 616d 655f 5fda  ...)...__name__.
+00000420: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000430: 7561 6c6e 616d 655f 5fda 0462 6f6f 6cda  ualname__..bool.
+00000440: 0369 6e74 7212 0000 00da 0d5f 5f63 6c61  .intr......__cla
+00000450: 7373 6365 6c6c 5f5f 7223 0000 0072 2300  sscell__r#...r#.
+00000460: 0000 7221 0000 0072 2400 0000 720b 0000  ..r!...r$...r...
+00000470: 0014 0000 0073 0200 0000 0801 720b 0000  .....s......r...
+00000480: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000490: 0000 0400 0000 0000 0000 7354 0000 0065  ..........sT...e
+000004a0: 005a 0164 005a 0265 03a0 0465 05a1 015a  .Z.d.Z.e...e...Z
+000004b0: 0665 0765 0564 019c 0287 0066 0164 0264  .e.e.d.....f.d.d
+000004c0: 0384 0c5a 0864 0d65 0964 059c 0164 0664  ...Z.d.e.d...d.d
+000004d0: 0784 055a 0a64 0864 0984 005a 0b65 0764  ...Z.d.d...Z.e.d
+000004e0: 0a9c 0164 0b64 0c84 045a 0c87 0004 005a  ...d.d...Z.....Z
+000004f0: 0d53 0029 0eda 0a4d 656e 7542 7574 746f  .S.)...MenuButto
+00000500: 6e29 02da 086d 656e 7574 6578 74da 086d  n)...menutext..m
+00000510: 656e 7569 7465 6d63 0300 0000 0000 0000  enuitemc........
+00000520: 0000 0000 0300 0000 0300 0000 0300 0000  ................
+00000530: 7338 0000 0074 0083 00a0 01a1 0001 007c  s8...t.........|
+00000540: 00a0 027c 01a1 0101 007c 00a0 0364 01a1  ...|.....|...d..
+00000550: 0101 007c 027c 005f 047c 006a 056a 06a0  ...|.|._.|.j.j..
+00000560: 077c 006a 08a1 0101 0064 0053 0029 024e  .|.j.....d.S.).N
+00000570: 4629 0972 1100 0000 7212 0000 00da 0e5f  F).r....r......_
+00000580: 7365 7475 705f 7769 6467 6574 73da 0d73  setup_widgets..s
+00000590: 6574 5f68 6967 686c 6967 6874 722d 0000  et_highlightr-..
+000005a0: 00da 075f 6275 7474 6f6e da07 636c 6963  ..._button..clic
+000005b0: 6b65 64da 0763 6f6e 6e65 6374 da0b 5f6f  ked..connect.._o
+000005c0: 6e5f 636c 6963 6b65 6429 0372 1f00 0000  n_clicked).r....
+000005d0: 722c 0000 0072 2d00 0000 7221 0000 0072  r,...r-...r!...r
+000005e0: 2300 0000 7224 0000 0072 1200 0000 2000  #...r$...r.... .
+000005f0: 0000 730a 0000 0000 010a 010a 010a 0106  ..s.............
+00000600: 017a 134d 656e 7542 7574 746f 6e2e 5f5f  .z.MenuButton.__
+00000610: 696e 6974 5f5f 4629 01da 0968 6967 686c  init__F)...highl
+00000620: 6967 6874 6302 0000 0000 0000 0000 0000  ightc...........
+00000630: 0003 0000 0005 0000 0043 0000 0073 3400  .........C...s4.
+00000640: 0000 7c01 7210 7400 6a01 6a02 6a03 6a04  ..|.r.t.j.j.j.j.
+00000650: 6e0a 7400 6a01 6a02 6a03 6a05 7d02 7c00  n.t.j.j.j.j.}.|.
+00000660: 6a06 a007 6401 7c02 9b00 6402 9d03 a101  j...d.|...d.....
+00000670: 0100 6400 5300 720f 0000 0029 0872 1800  ..d.S.r....).r..
+00000680: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00000690: 0072 1c00 0000 da09 536f 6674 5f47 7261  .r......Soft_Gra
+000006a0: 79da 0c5f 6d61 726b 6572 5f6c 696e 6572  y.._marker_liner
+000006b0: 1700 0000 2903 721f 0000 0072 3400 0000  ....).r....r4...
+000006c0: da05 636f 6c6f 7272 2300 0000 7223 0000  ..colorr#...r#..
+000006d0: 0072 2400 0000 722f 0000 0027 0000 0073  .r$...r/...'...s
+000006e0: 0400 0000 0001 1c01 7a18 4d65 6e75 4275  ........z.MenuBu
+000006f0: 7474 6f6e 2e73 6574 5f68 6967 686c 6967  tton.set_highlig
+00000700: 6874 6301 0000 0000 0000 0000 0000 0001  htc.............
+00000710: 0000 0003 0000 0043 0000 0073 1200 0000  .......C...s....
+00000720: 7c00 6a00 a001 7c00 6a02 a101 0100 6400  |.j...|.j.....d.
+00000730: 5300 a901 4e29 03da 1373 6967 5f6f 6e5f  S...N)...sig_on_
+00000740: 6d65 6e75 5f63 6c69 636b 6564 da04 656d  menu_clicked..em
+00000750: 6974 722d 0000 00a9 0172 1f00 0000 7223  itr-.....r....r#
+00000760: 0000 0072 2300 0000 7224 0000 0072 3300  ...r#...r$...r3.
+00000770: 0000 2b00 0000 7302 0000 0000 017a 164d  ..+...s......z.M
+00000780: 656e 7542 7574 746f 6e2e 5f6f 6e5f 636c  enuButton._on_cl
+00000790: 6963 6b65 6429 01da 096c 6162 656c 5f73  icked)...label_s
+000007a0: 7472 6302 0000 0000 0000 0000 0000 0003  trc.............
+000007b0: 0000 0006 0000 0043 0000 0073 6200 0000  .......C...sb...
+000007c0: 7400 a001 a100 7d02 7c02 a002 6401 a101  t.....}.|...d...
+000007d0: 0100 7c02 a003 6401 6401 6401 6401 a104  ..|...d.d.d.d...
+000007e0: 0100 7400 a004 7c01 a101 7c00 5f05 7406  ..t...|...|._.t.
+000007f0: 6402 6403 6404 8d02 7c00 5f07 7c02 a008  d.d.d...|._.|...
+00000800: 7c00 6a07 a101 0100 7c02 a008 7c00 6a05  |.j.....|...|.j.
+00000810: a101 0100 7c00 a009 7c02 a101 0100 6400  ....|...|.....d.
+00000820: 5300 2905 4e72 0100 0000 46e9 0200 0000  S.).Nr....F.....
+00000830: 720c 0000 0029 0a72 0300 0000 da0b 5156  r....).r......QV
+00000840: 426f 784c 6179 6f75 74da 0a73 6574 5370  BoxLayout..setSp
+00000850: 6163 696e 67da 1273 6574 436f 6e74 656e  acing..setConten
+00000860: 7473 4d61 7267 696e 73da 0b51 5075 7368  tsMargins..QPush
+00000870: 4275 7474 6f6e 7230 0000 0072 0b00 0000  Buttonr0...r....
+00000880: 7236 0000 00da 0961 6464 5769 6467 6574  r6.....addWidget
+00000890: da09 7365 744c 6179 6f75 7429 0372 1f00  ..setLayout).r..
+000008a0: 0000 723c 0000 00da 066c 6179 6f75 7472  ..r<.....layoutr
+000008b0: 2300 0000 7223 0000 0072 2400 0000 722e  #...r#...r$...r.
+000008c0: 0000 002e 0000 0073 1000 0000 0001 0801  .......s........
+000008d0: 0a01 1001 0c01 0e01 0c01 0c01 7a19 4d65  ............z.Me
+000008e0: 6e75 4275 7474 6f6e 2e5f 7365 7475 705f  nuButton._setup_
+000008f0: 7769 6467 6574 7329 0146 290e 7225 0000  widgets).F).r%..
+00000900: 0072 2600 0000 7227 0000 0072 0500 0000  .r&...r'...r....
+00000910: da06 5369 676e 616c 7229 0000 0072 3900  ..Signalr)...r9.
+00000920: 0000 da03 7374 7272 1200 0000 7228 0000  ....strr....r(..
+00000930: 0072 2f00 0000 7233 0000 0072 2e00 0000  .r/...r3...r....
+00000940: 722a 0000 0072 2300 0000 7223 0000 0072  r*...r#...r#...r
+00000950: 2100 0000 7224 0000 0072 2b00 0000 1c00  !...r$...r+.....
+00000960: 0000 730a 0000 0008 020a 0214 0710 0408  ..s.............
+00000970: 0372 2b00 0000 6300 0000 0000 0000 0000  .r+...c.........
+00000980: 0000 0000 0000 0003 0000 0000 0000 0073  ...............s
+00000990: 1c00 0000 6500 5a01 6400 5a02 8700 6601  ....e.Z.d.Z...f.
+000009a0: 6401 6402 8408 5a03 8700 0400 5a04 5300  d.d...Z.....Z.S.
+000009b0: 2903 da0a 5374 6456 5370 6163 6572 6301  )...StdVSpacerc.
+000009c0: 0000 0000 0000 0000 0000 0001 0000 0006  ................
+000009d0: 0000 0003 0000 0073 1e00 0000 7400 8300  .......s....t...
+000009e0: a001 7402 6401 7403 6a04 6a05 7403 6a04  ..t.d.t.j.j.t.j.
+000009f0: 6a06 a104 0100 6400 5300 2902 4ee9 2800  j.....d.S.).N.(.
+00000a00: 0000 2907 7211 0000 0072 1200 0000 da14  ..).r....r......
+00000a10: 636f 6e74 726f 6c5f 6c61 796f 7574 5f77  control_layout_w
+00000a20: 6964 7468 7203 0000 00da 0b51 5369 7a65  idthr......QSize
+00000a30: 506f 6c69 6379 da05 4669 7865 64da 104d  Policy..Fixed..M
+00000a40: 696e 696d 756d 4578 7061 6e64 696e 6772  inimumExpandingr
+00000a50: 3b00 0000 7221 0000 0072 2300 0000 7224  ;...r!...r#...r$
+00000a60: 0000 0072 1200 0000 3a00 0000 7302 0000  ...r....:...s...
+00000a70: 0000 017a 1353 7464 5653 7061 6365 722e  ...z.StdVSpacer.
+00000a80: 5f5f 696e 6974 5f5f 2905 7225 0000 0072  __init__).r%...r
+00000a90: 2600 0000 7227 0000 0072 1200 0000 722a  &...r'...r....r*
+00000aa0: 0000 0072 2300 0000 7223 0000 0072 2100  ...r#...r#...r!.
+00000ab0: 0000 7224 0000 0072 4700 0000 3900 0000  ..r$...rG...9...
+00000ac0: 7302 0000 0008 0172 4700 0000 6300 0000  s......rG...c...
+00000ad0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000ae0: 0040 0000 0073 2800 0000 6500 5a01 6400  .@...s(...e.Z.d.
+00000af0: 5a02 5500 6401 5a03 6504 6a05 6506 6402  Z.U.d.Z.e.j.e.d.
+00000b00: 3c00 6403 5a07 6508 6506 6404 3c00 6401  <.d.Z.e.e.d.<.d.
+00000b10: 5300 2905 da09 5363 7265 656e 4465 664e  S.)...ScreenDefN
+00000b20: da06 7363 7265 656e da00 da04 6e61 6d65  ..screen....name
+00000b30: 2909 7225 0000 0072 2600 0000 7227 0000  ).r%...r&...r'..
+00000b40: 0072 4e00 0000 7209 0000 00da 0c4d 6f64  .rN...r......Mod
+00000b50: 756c 6553 6372 6565 6eda 0f5f 5f61 6e6e  uleScreen..__ann
+00000b60: 6f74 6174 696f 6e73 5f5f 7250 0000 0072  otations__rP...r
+00000b70: 4600 0000 7223 0000 0072 2300 0000 7223  F...r#...r#...r#
+00000b80: 0000 0072 2400 0000 724d 0000 003d 0000  ...r$...rM...=..
+00000b90: 0073 0400 0000 0a02 0e01 724d 0000 0063  .s........rM...c
+00000ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000bb0: 0500 0000 0000 0000 73fc 0000 0065 005a  ........s....e.Z
+00000bc0: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
+00000bd0: 0365 0465 0464 039c 0264 0464 0584 045a  .e.e.d...d.d...Z
+00000be0: 0565 066a 076a 0866 0165 0465 066a 0764  .e.j.j.f.e.e.j.d
+00000bf0: 069c 0264 0764 0884 055a 0964 0964 0a84  ...d.d...Z.d.d..
+00000c00: 005a 0a64 0b64 0c84 005a 0b64 0d64 0e84  .Z.d.d...Z.d.d..
+00000c10: 005a 0c65 0d6a 0e65 0464 0f9c 0264 1064  .Z.e.j.e.d...d.d
+00000c20: 1184 045a 0f65 1064 129c 0164 1364 1484  ...Z.e.d...d.d..
+00000c30: 045a 1165 1064 159c 0164 1664 1784 045a  .Z.e.d...d.d...Z
+00000c40: 1265 1364 129c 0164 1864 1984 045a 1464  .e.d...d.d...Z.d
+00000c50: 1a64 1b84 005a 1565 1064 1c9c 0164 1d64  .d...Z.e.d...d.d
+00000c60: 1e84 045a 1687 0066 0164 1f64 2084 085a  ...Z...f.d.d ..Z
+00000c70: 1765 0464 219c 0164 2264 2384 045a 1865  .e.d!..d"d#..Z.e
+00000c80: 1064 159c 0164 2464 2584 045a 1964 2664  .d...d$d%..Z.d&d
+00000c90: 2784 005a 1a64 2e65 0465 0465 0464 299c  '..Z.d.e.e.e.d).
+00000ca0: 0364 2a64 2b84 055a 1b64 2c64 2d84 005a  .d*d+..Z.d,d-..Z
+00000cb0: 1c87 0004 005a 1d53 0029 2fda 0941 7070  .....Z.S.)/..App
+00000cc0: 5769 6e64 6f77 6302 0000 0000 0000 0000  Windowc.........
+00000cd0: 0000 0002 0000 0002 0000 0003 0000 0073  ...............s
+00000ce0: 1a00 0000 7400 8300 a001 a100 0100 7c01  ....t.........|.
+00000cf0: 7c00 5f02 6700 7c00 5f03 6400 5300 7238  |._.g.|._.d.S.r8
+00000d00: 0000 0029 0472 1100 0000 7212 0000 00da  ...).r....r.....
+00000d10: 0361 7070 da0f 6c69 7374 5f6f 665f 7363  .app..list_of_sc
+00000d20: 7265 656e 7329 0272 1f00 0000 7254 0000  reens).r....rT..
+00000d30: 0072 2100 0000 7223 0000 0072 2400 0000  .r!...r#...r$...
+00000d40: 7212 0000 0043 0000 0073 0600 0000 0001  r....C...s......
+00000d50: 0a01 0601 7a12 4170 7057 696e 646f 772e  ....z.AppWindow.
+00000d60: 5f5f 696e 6974 5f5f 2902 da0d 7569 5f73  __init__)...ui_s
+00000d70: 7479 6c65 5f66 696c 65da 0969 636f 6e5f  tyle_file..icon_
+00000d80: 6669 6c65 6303 0000 0000 0000 0000 0000  filec...........
+00000d90: 0004 0000 0006 0000 0043 0000 0073 1c01  .........C...s..
+00000da0: 0000 7c00 a000 7c01 a101 7d03 7c00 a001  ..|...|...}.|...
+00000db0: 7c03 a101 0100 7c00 a002 7c00 6a03 6a04  |.....|...|.j.j.
+00000dc0: a101 0100 7c00 a005 7406 a007 7408 7c02  ....|...t...t.|.
+00000dd0: 8301 a101 a101 0100 7c00 a009 a100 a00a  ........|.......
+00000de0: 6401 a101 0100 740b a00c a100 7c00 5f0d  d.....t.....|._.
+00000df0: 740b a00e a100 7c00 5f0f 740b a010 a100  t.....|._.t.....
+00000e00: 7c00 5f11 7412 6a13 6a14 6402 6403 8d01  |._.t.j.j.d.d...
+00000e10: 7c00 5f15 740b a016 a100 7c00 5f17 7c00  |._.t.....|._.|.
+00000e20: 6a17 a018 740b a019 6404 a101 a101 0100  j...t...d.......
+00000e30: 741a 6402 6403 8d01 7c00 5f1b 741a 6405  t.d.d...|._.t.d.
+00000e40: 6403 8d01 7c00 5f1c 7c00 6a0f a01d 7c00  d...|._.|.j...|.
+00000e50: 6a11 6406 a102 0100 7c00 6a0f a018 7c00  j.d.....|.j...|.
+00000e60: 6a1b 6407 a102 0100 7c00 6a0f a018 7c00  j.d.....|.j...|.
+00000e70: 6a15 6408 a102 0100 7c00 6a0f a01d 7c00  j.d.....|.j...|.
+00000e80: 6a17 6409 a102 0100 7c00 6a0f a018 7c00  j.d.....|.j...|.
+00000e90: 6a1c 640a a102 0100 7c00 6a0d a01e 7c00  j.d.....|.j...|.
+00000ea0: 6a0f a101 0100 7c00 a01f 7c00 6a0d a101  j.....|...|.j...
+00000eb0: 0100 7c00 a020 a100 0100 6400 5300 290b  ..|.. ....d.S.).
+00000ec0: 4e5a 0552 6561 6479 5429 0172 0d00 0000  NZ.ReadyT).r....
+00000ed0: 7a0b 4d61 696e 2073 6372 6565 6e46 7201  z.Main screenFr.
+00000ee0: 0000 0072 0700 0000 723d 0000 00e9 0300  ...r....r=......
+00000ef0: 0000 e904 0000 0029 21da 1a5f 7265 6164  .......)!.._read
+00000f00: 5f73 7479 6c65 5f73 6865 6574 5f69 6e74  _style_sheet_int
+00000f10: 6f5f 7374 7272 1700 0000 da0e 7365 7457  o_strr......setW
+00000f20: 696e 646f 7754 6974 6c65 7254 0000 00da  indowTitlerT....
+00000f30: 0d61 7070 5f6e 616d 655f 6c6f 6e67 da0d  .app_name_long..
+00000f40: 7365 7457 696e 646f 7749 636f 6e72 0400  setWindowIconr..
+00000f50: 0000 da05 5149 636f 6e72 4600 0000 da09  ....QIconrF.....
+00000f60: 7374 6174 7573 4261 72da 0b73 686f 774d  statusBar..showM
+00000f70: 6573 7361 6765 7203 0000 00da 0751 5769  essager......QWi
+00000f80: 6467 6574 5a0a 6d61 696e 5363 7265 656e  dgetZ.mainScreen
+00000f90: 723e 0000 005a 0b6d 6169 6e5f 6c61 796f  r>...Z.main_layo
+00000fa0: 7574 da0b 5148 426f 784c 6179 6f75 74da  ut..QHBoxLayout.
+00000fb0: 096d 6169 6e5f 6d65 6e75 7218 0000 0072  .main_menur....r
+00000fc0: 1900 0000 da0a 4e53 4649 6e66 6f42 6f78  ......NSFInfoBox
+00000fd0: da0f 6d61 696e 5f6d 6573 7361 6765 626f  ..main_messagebo
+00000fe0: 78da 0e51 5374 6163 6b65 644c 6179 6f75  x..QStackedLayou
+00000ff0: 74da 0a6d 6169 6e5f 7374 6163 6b72 4200  t..main_stackrB.
+00001000: 0000 da06 514c 6162 656c 720b 0000 00da  ....QLabelr.....
+00001010: 086d 656e 755f 7365 705a 0a73 7461 7475  .menu_sepZ.statu
+00001020: 735f 7365 70da 0961 6464 4c61 796f 7574  s_sep..addLayout
+00001030: 7243 0000 00da 1073 6574 4365 6e74 7261  rC.....setCentra
+00001040: 6c57 6964 6765 74da 106c 6f61 645f 7769  lWidget..load_wi
+00001050: 6e64 6f77 5f73 697a 6529 0472 1f00 0000  ndow_size).r....
+00001060: 7256 0000 0072 5700 0000 5a0f 7374 796c  rV...rW...Z.styl
+00001070: 655f 7368 6565 745f 7374 7272 2300 0000  e_sheet_strr#...
+00001080: 7223 0000 0072 2400 0000 da0a 6372 6561  r#...r$.....crea
+00001090: 7465 5f67 7569 4800 0000 732a 0000 0000  te_guiH...s*....
+000010a0: 020a 010a 010e 0114 010e 040a 010a 010a  ................
+000010b0: 0110 010a 0112 020c 010c 0110 0110 0110  ................
+000010c0: 0110 0110 020e 010c 017a 1441 7070 5769  .........z.AppWi
+000010d0: 6e64 6f77 2e63 7265 6174 655f 6775 6929  ndow.create_gui)
+000010e0: 02da 036d 7367 da08 6d73 675f 7479 7065  ...msg..msg_type
+000010f0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00001100: 0004 0000 0043 0000 0073 5a00 0000 7c02  .....C...sZ...|.
+00001110: 7400 6a01 6a02 6b02 7224 7c00 6a03 7c01  t.j.j.k.r$|.j.|.
+00001120: 7404 6a05 6a06 6a07 6a08 6401 8d02 0100  t.j.j.j.j.d.....
+00001130: 6e32 7c02 7400 6a01 6a09 6b02 7248 7c00  n2|.t.j.j.k.rH|.
+00001140: 6a03 7c01 7404 6a05 6a06 6a07 6a08 6401  j.|.t.j.j.j.j.d.
+00001150: 8d02 0100 6e0e 7c00 a00a a100 a00b 7c01  ....n.|.......|.
+00001160: a101 0100 6400 5300 2902 4e29 01da 1062  ....d.S.).N)...b
+00001170: 6163 6b67 726f 756e 645f 636f 6c6f 7229  ackground_color)
+00001180: 0c72 0800 0000 da07 4d73 6754 7970 65da  .r......MsgType.
+00001190: 0545 7272 6f72 da0d 7368 6f77 5f69 6e66  .Error..show_inf
+000011a0: 6f5f 626f 7872 1800 0000 7219 0000 0072  o_boxr....r....r
+000011b0: 1a00 0000 721b 0000 0072 1c00 0000 da04  ....r....r......
+000011c0: 5761 726e 725f 0000 0072 6000 0000 2903  Warnr_...r`...).
+000011d0: 721f 0000 0072 6e00 0000 726f 0000 0072  r....rn...ro...r
+000011e0: 2300 0000 7223 0000 0072 2400 0000 da0c  #...r#...r$.....
+000011f0: 7368 6f77 5f6d 6573 7361 6765 6500 0000  show_messagee...
+00001200: 730a 0000 0000 010c 0118 010c 0118 027a  s..............z
+00001210: 1641 7070 5769 6e64 6f77 2e73 686f 775f  .AppWindow.show_
+00001220: 6d65 7373 6167 6563 0100 0000 0000 0000  messagec........
+00001230: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+00001240: 731a 0000 007c 00a0 00a1 00a0 0164 01a1  s....|.......d..
+00001250: 0101 007c 00a0 02a1 0001 0064 0053 00a9  ...|.......d.S..
+00001260: 024e 724f 0000 0029 0372 5f00 0000 7260  .NrO...).r_...r`
+00001270: 0000 00da 0d68 6964 655f 696e 666f 5f62  .....hide_info_b
+00001280: 6f78 723b 0000 0072 2300 0000 7223 0000  oxr;...r#...r#..
+00001290: 0072 2400 0000 da0c 6869 6465 5f6d 6573  .r$.....hide_mes
+000012a0: 7361 6765 6d00 0000 7304 0000 0000 010e  sagem...s.......
+000012b0: 017a 1641 7070 5769 6e64 6f77 2e68 6964  .z.AppWindow.hid
+000012c0: 655f 6d65 7373 6167 6563 0100 0000 0000  e_messagec......
+000012d0: 0000 0000 0000 0100 0000 0500 0000 4300  ..............C.
+000012e0: 0000 732c 0000 007c 006a 006a 01a0 0264  ..s,...|.j.j...d
+000012f0: 017c 00a0 03a1 00a1 0201 007c 006a 006a  .|.........|.j.j
+00001300: 01a0 0264 027c 00a0 04a1 00a1 0201 0064  ...d.|.........d
+00001310: 0053 00a9 034e da08 6765 6f6d 6574 7279  .S...N..geometry
+00001320: da0b 7769 6e64 6f77 5374 6174 6529 0572  ..windowState).r
+00001330: 5400 0000 da08 7265 6769 7374 7279 da08  T.....registry..
+00001340: 7365 7456 616c 7565 da0c 7361 7665 4765  setValue..saveGe
+00001350: 6f6d 6574 7279 da09 7361 7665 5374 6174  ometry..saveStat
+00001360: 6572 3b00 0000 7223 0000 0072 2300 0000  er;...r#...r#...
+00001370: 7224 0000 00da 1073 6176 655f 7769 6e64  r$.....save_wind
+00001380: 6f77 5f73 697a 6571 0000 0073 0400 0000  ow_sizeq...s....
+00001390: 0001 1401 7a1a 4170 7057 696e 646f 772e  ....z.AppWindow.
+000013a0: 7361 7665 5f77 696e 646f 775f 7369 7a65  save_window_size
+000013b0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000013c0: 0005 0000 0043 0000 0073 2c00 0000 7c00  .....C...s,...|.
+000013d0: a000 7c00 6a01 6a02 a003 6401 a101 a101  ..|.j.j...d.....
+000013e0: 0100 7c00 a004 7c00 6a01 6a02 a003 6402  ..|...|.j.j...d.
+000013f0: a101 a101 0100 6400 5300 7279 0000 0029  ......d.S.ry...)
+00001400: 05da 0f72 6573 746f 7265 4765 6f6d 6574  ...restoreGeomet
+00001410: 7279 7254 0000 0072 7c00 0000 da05 7661  ryrT...r|.....va
+00001420: 6c75 65da 0c72 6573 746f 7265 5374 6174  lue..restoreStat
+00001430: 6572 3b00 0000 7223 0000 0072 2300 0000  er;...r#...r#...
+00001440: 7224 0000 0072 6c00 0000 7500 0000 7304  r$...rl...u...s.
+00001450: 0000 0000 0114 017a 1a41 7070 5769 6e64  .......z.AppWind
+00001460: 6f77 2e6c 6f61 645f 7769 6e64 6f77 5f73  ow.load_window_s
+00001470: 697a 6529 0272 1900 0000 da0b 7363 7265  ize).r......scre
+00001480: 656e 5f6e 616d 6563 0300 0000 0000 0000  en_namec........
+00001490: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
+000014a0: 7350 0000 007c 006a 00a0 0174 027c 017c  sP...|.j...t.|.|
+000014b0: 0283 02a1 0101 0074 037c 0174 046a 0583  .......t.|.t.j..
+000014c0: 0272 447c 006a 06a0 077c 01a1 0101 007c  .rD|.j...|.....|
+000014d0: 006a 06a0 08a1 0064 016b 0272 447c 006a  .j.....d.k.rD|.j
+000014e0: 06a0 097c 01a1 0101 007c 00a0 0aa1 0001  ...|.....|......
+000014f0: 0064 0053 00a9 024e 7201 0000 0029 0b72  .d.S...Nr....).r
+00001500: 5500 0000 da06 6170 7065 6e64 724d 0000  U.....appendrM..
+00001510: 00da 0a69 7369 6e73 7461 6e63 6572 0300  ...isinstancer..
+00001520: 0000 7261 0000 0072 6700 0000 7242 0000  ..ra...rg...rB..
+00001530: 00da 0c63 7572 7265 6e74 496e 6465 78da  ...currentIndex.
+00001540: 1073 6574 4375 7272 656e 7457 6964 6765  .setCurrentWidge
+00001550: 74da 0b75 7064 6174 655f 6d65 6e75 2903  t..update_menu).
+00001560: 721f 0000 0072 1900 0000 7284 0000 0072  r....r....r....r
+00001570: 2300 0000 7223 0000 0072 2400 0000 da0a  #...r#...r$.....
+00001580: 6164 645f 7363 7265 656e 7900 0000 730c  add_screeny...s.
+00001590: 0000 0000 0112 010c 010c 020e 010c 017a  ...............z
+000015a0: 1441 7070 5769 6e64 6f77 2e61 6464 5f73  .AppWindow.add_s
+000015b0: 6372 6565 6e29 01da 0672 6574 7572 6e63  creen)...returnc
+000015c0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000015d0: 0200 0000 4300 0000 730e 0000 007c 006a  ....C...s....|.j
+000015e0: 00a0 01a1 0064 0118 0053 00a9 024e 7207  .....d...S...Nr.
+000015f0: 0000 0029 0272 6700 0000 7288 0000 0072  ...).rg...r....r
+00001600: 3b00 0000 7223 0000 0072 2300 0000 7224  ;...r#...r#...r$
+00001610: 0000 00da 1767 6574 5f61 6374 6976 655f  .....get_active_
+00001620: 6d6f 6475 6c65 5f69 6e64 6578 8200 0000  module_index....
+00001630: 7302 0000 0000 017a 2141 7070 5769 6e64  s......z!AppWind
+00001640: 6f77 2e67 6574 5f61 6374 6976 655f 6d6f  ow.get_active_mo
+00001650: 6475 6c65 5f69 6e64 6578 2901 da05 696e  dule_index)...in
+00001660: 6465 7863 0200 0000 0000 0000 0000 0000  dexc............
+00001670: 0200 0000 0400 0000 4300 0000 731c 0000  ........C...s...
+00001680: 007c 006a 00a0 017c 0164 0117 00a1 0101  .|.j...|.d......
+00001690: 007c 00a0 02a1 0001 0064 0053 0072 8d00  .|.......d.S.r..
+000016a0: 0000 2903 7267 0000 00da 0f73 6574 4375  ..).rg.....setCu
+000016b0: 7272 656e 7449 6e64 6578 da1d 5f75 7064  rrentIndex.._upd
+000016c0: 6174 655f 6d65 6e75 5f62 7574 746f 6e5f  ate_menu_button_
+000016d0: 6869 6768 6c69 6768 74a9 0272 1f00 0000  highlight..r....
+000016e0: 728f 0000 0072 2300 0000 7223 0000 0072  r....r#...r#...r
+000016f0: 2400 0000 da1a 7365 745f 6163 7469 7665  $.....set_active
+00001700: 5f6d 6f64 756c 655f 6279 5f69 6e64 6578  _module_by_index
+00001710: 8500 0000 7304 0000 0000 0110 017a 2441  ....s........z$A
+00001720: 7070 5769 6e64 6f77 2e73 6574 5f61 6374  ppWindow.set_act
+00001730: 6976 655f 6d6f 6475 6c65 5f62 795f 696e  ive_module_by_in
+00001740: 6465 7863 0100 0000 0000 0000 0000 0000  dexc............
+00001750: 0100 0000 0200 0000 4300 0000 730e 0000  ........C...s...
+00001760: 0074 007c 006a 0183 0164 016b 0453 0072  .t.|.j...d.k.S.r
+00001770: 8500 0000 2902 da03 6c65 6e72 5500 0000  ....)...lenrU...
+00001780: 723b 0000 0072 2300 0000 7223 0000 0072  r;...r#...r#...r
+00001790: 2400 0000 da0f 6973 5f6d 656e 755f 7669  $.....is_menu_vi
+000017a0: 7369 626c 6589 0000 0073 0200 0000 0001  sible....s......
+000017b0: 7a19 4170 7057 696e 646f 772e 6973 5f6d  z.AppWindow.is_m
+000017c0: 656e 755f 7669 7369 626c 6563 0100 0000  enu_visiblec....
+000017d0: 0000 0000 0000 0000 0600 0000 0400 0000  ................
+000017e0: 4300 0000 739a 0000 0074 007c 006a 0183  C...s....t.|.j..
+000017f0: 017d 017c 0164 016b 0472 867c 006a 02a0  .}.|.d.k.r.|.j..
+00001800: 03a1 0072 427c 006a 02a0 0464 02a1 017d  ...rB|.j...d...}
+00001810: 027c 02a0 05a1 0064 0075 0172 127c 02a0  .|.....d.u.r.|..
+00001820: 05a1 00a0 06a1 0001 0071 1274 077c 006a  .........q.t.|.j
+00001830: 0183 0144 005d 2e5c 027d 037d 0474 087c  ...D.].\.}.}.t.|
+00001840: 046a 097c 0383 027d 057c 056a 0aa0 0b7c  .j.|...}.|.j...|
+00001850: 006a 0ca1 0101 007c 006a 02a0 0d7c 05a1  .j.....|.j...|..
+00001860: 0101 0071 4c7c 006a 02a0 0ea1 0001 007c  ...qL|.j.......|
+00001870: 006a 0fa0 107c 0164 016b 01a1 0101 0064  .j...|.d.k.....d
+00001880: 0053 0029 034e 7207 0000 0072 0100 0000  .S.).Nr....r....
+00001890: 2911 7294 0000 0072 5500 0000 7263 0000  ).r....rU...rc..
+000018a0: 00da 0563 6f75 6e74 da06 7461 6b65 4174  ...count..takeAt
+000018b0: da06 7769 6467 6574 da0b 6465 6c65 7465  ..widget..delete
+000018c0: 4c61 7465 72da 0965 6e75 6d65 7261 7465  Later..enumerate
+000018d0: 722b 0000 0072 5000 0000 7239 0000 0072  r+...rP...r9...r
+000018e0: 3200 0000 da17 5f6f 6e5f 6d65 6e75 5f62  2....._on_menu_b
+000018f0: 7574 746f 6e5f 636c 6963 6b65 6472 4200  utton_clickedrB.
+00001900: 0000 da0a 6164 6453 7472 6574 6368 7269  ....addStretchri
+00001910: 0000 0072 1e00 0000 2906 721f 0000 005a  ...r....).r....Z
+00001920: 0e6e 756d 5f6f 665f 7363 7265 656e 73da  .num_of_screens.
+00001930: 0563 6869 6c64 5a09 6d65 6e75 696e 6465  .childZ.menuinde
+00001940: 785a 0973 6372 6565 6e64 6566 722d 0000  xZ.screendefr-..
+00001950: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
+00001960: 728a 0000 008c 0000 0073 1800 0000 0001  r........s......
+00001970: 0a02 0802 0a01 0c01 0c01 0e02 1201 0c01  ................
+00001980: 0e01 0e01 0a02 7a15 4170 7057 696e 646f  ......z.AppWindo
+00001990: 772e 7570 6461 7465 5f6d 656e 7529 01da  w.update_menu)..
+000019a0: 0c73 6372 6565 6e5f 696e 6465 7863 0200  .screen_indexc..
+000019b0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+000019c0: 0000 4300 0000 731a 0000 007c 017c 006a  ..C...s....|.|.j
+000019d0: 006a 016a 025f 037c 00a0 047c 01a1 0101  .j.j._.|...|....
+000019e0: 0064 0053 0072 3800 0000 2905 7254 0000  .d.S.r8...).rT..
+000019f0: 00da 0873 6574 7469 6e67 73da 1141 6374  ...settings..Act
+00001a00: 6976 654d 6f64 756c 6549 6e64 6578 7282  iveModuleIndexr.
+00001a10: 0000 0072 9300 0000 2902 721f 0000 0072  ...r....).r....r
+00001a20: 9e00 0000 7223 0000 0072 2300 0000 7224  ....r#...r#...r$
+00001a30: 0000 00da 0f61 6374 6976 6174 655f 7363  .....activate_sc
+00001a40: 7265 656e 9e00 0000 7304 0000 0000 010c  reen....s.......
+00001a50: 017a 1941 7070 5769 6e64 6f77 2e61 6374  .z.AppWindow.act
+00001a60: 6976 6174 655f 7363 7265 656e 6302 0000  ivate_screenc...
+00001a70: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00001a80: 0003 0000 0073 1800 0000 7c00 a000 a100  .....s....|.....
+00001a90: 0100 7401 8300 a002 7c01 a101 0100 6401  ..t.....|.....d.
+00001aa0: 5300 2902 7a2d 2063 6170 7475 7265 2063  S.).z- capture c
+00001ab0: 6c6f 7365 2062 7574 746f 6e20 6672 6f6d  lose button from
+00001ac0: 2061 7070 6c69 6361 7469 6f6e 2077 696e   application win
+00001ad0: 646f 774e 2903 7280 0000 0072 1100 0000  dowN).r....r....
+00001ae0: da0a 636c 6f73 6545 7665 6e74 2902 721f  ..closeEvent).r.
+00001af0: 0000 00da 0361 7267 7221 0000 0072 2300  .....argr!...r#.
+00001b00: 0000 7224 0000 0072 a200 0000 a400 0000  ..r$...r........
+00001b10: 7304 0000 0000 0208 017a 1441 7070 5769  s........z.AppWi
+00001b20: 6e64 6f77 2e63 6c6f 7365 4576 656e 7429  ndow.closeEvent)
+00001b30: 01da 0a73 7479 6c65 5f66 696c 6563 0200  ...style_filec..
+00001b40: 0000 0000 0000 0000 0000 0400 0000 0800  ................
+00001b50: 0000 4300 0000 7338 0000 0064 017d 0274  ..C...s8...d.}.t
+00001b60: 007c 0183 018f 187d 037c 03a0 01a1 007d  .|.....}.|.....}
+00001b70: 0257 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
+00001b80: 0073 2a30 0001 0001 0001 0059 0001 007c  .s*0.......Y...|
+00001b90: 0253 0072 7600 0000 2902 da04 6f70 656e  .S.rv...)...open
+00001ba0: da04 7265 6164 2904 721f 0000 0072 a400  ..read).r....r..
+00001bb0: 0000 da05 7374 796c 65da 0166 7223 0000  ....style..fr#..
+00001bc0: 0072 2300 0000 7224 0000 0072 5a00 0000  .r#...r$...rZ...
+00001bd0: a900 0000 7308 0000 0000 0104 010a 0126  ....s..........&
+00001be0: 017a 2441 7070 5769 6e64 6f77 2e5f 7265  .z$AppWindow._re
+00001bf0: 6164 5f73 7479 6c65 5f73 6865 6574 5f69  ad_style_sheet_i
+00001c00: 6e74 6f5f 7374 7263 0200 0000 0000 0000  nto_strc........
+00001c10: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
+00001c20: 730e 0000 007c 00a0 007c 01a1 0101 0064  s....|...|.....d
+00001c30: 0053 0072 3800 0000 2901 72a1 0000 0072  .S.r8...).r....r
+00001c40: 9200 0000 7223 0000 0072 2300 0000 7224  ....r#...r#...r$
+00001c50: 0000 0072 9b00 0000 af00 0000 7302 0000  ...r........s...
+00001c60: 0000 017a 2141 7070 5769 6e64 6f77 2e5f  ...z!AppWindow._
+00001c70: 6f6e 5f6d 656e 755f 6275 7474 6f6e 5f63  on_menu_button_c
+00001c80: 6c69 636b 6564 6301 0000 0000 0000 0000  lickedc.........
+00001c90: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
+00001ca0: 4600 0000 7c00 a000 a100 7242 7c00 a001  F...|.....rB|...
+00001cb0: a100 7d01 7402 7c00 6a03 a004 a100 6401  ..}.t.|.j.....d.
+00001cc0: 1800 8301 4400 5d1e 7d02 7c00 6a03 a005  ....D.].}.|.j...
+00001cd0: 7c02 a101 a006 a100 a007 7c02 7c01 6b02  |.........|.|.k.
+00001ce0: a101 0100 7122 6400 5300 728d 0000 0029  ....q"d.S.r....)
+00001cf0: 0872 9500 0000 728e 0000 00da 0572 616e  .r....r......ran
+00001d00: 6765 7263 0000 0072 9600 0000 da06 6974  gerc...r......it
+00001d10: 656d 4174 7298 0000 0072 2f00 0000 2903  emAtr....r/...).
+00001d20: 721f 0000 005a 0c61 6374 6976 655f 696e  r....Z.active_in
+00001d30: 6465 78da 0169 7223 0000 0072 2300 0000  dex..ir#...r#...
+00001d40: 7224 0000 0072 9100 0000 b200 0000 7308  r$...r........s.
+00001d50: 0000 0000 0108 0108 0116 017a 2741 7070  ...........z'App
+00001d60: 5769 6e64 6f77 2e5f 7570 6461 7465 5f6d  Window._update_m
+00001d70: 656e 755f 6275 7474 6f6e 5f68 6967 686c  enu_button_highl
+00001d80: 6967 6874 724f 0000 0029 0372 6e00 0000  ightrO...).rn...
+00001d90: 7270 0000 00da 0a74 6578 745f 636f 6c6f  rp.....text_colo
+00001da0: 7263 0400 0000 0000 0000 0000 0000 0400  rc..............
+00001db0: 0000 0300 0000 4300 0000 733c 0000 007c  ......C...s<...|
+00001dc0: 006a 00a0 017c 02a1 0101 007c 0364 016b  .j...|.....|.d.k
+00001dd0: 0372 207c 006a 00a0 027c 03a1 0101 007c  .r |.j...|.....|
+00001de0: 006a 00a0 037c 01a1 0101 007c 006a 00a0  .j...|.....|.j..
+00001df0: 0464 02a1 0101 0064 0053 0029 034e 724f  .d.....d.S.).NrO
+00001e00: 0000 0046 2905 7265 0000 00da 1473 6574  ...F).re.....set
+00001e10: 5f62 6163 6b67 726f 756e 645f 636f 6c6f  _background_colo
+00001e20: 72da 0e73 6574 5f74 6578 745f 636f 6c6f  r..set_text_colo
+00001e30: 72da 0b73 6574 5f6d 6573 7361 6765 721e  r..set_messager.
+00001e40: 0000 0029 0472 1f00 0000 726e 0000 0072  ...).r....rn...r
+00001e50: 7000 0000 72ac 0000 0072 2300 0000 7223  p...r....r#...r#
+00001e60: 0000 0072 2400 0000 7273 0000 00b8 0000  ...r$...rs......
+00001e70: 0073 0a00 0000 0001 0c01 0801 0c01 0c01  .s..............
+00001e80: 7a17 4170 7057 696e 646f 772e 7368 6f77  z.AppWindow.show
+00001e90: 5f69 6e66 6f5f 626f 7863 0100 0000 0000  _info_boxc......
+00001ea0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00001eb0: 0000 7310 0000 007c 006a 00a0 0164 01a1  ..s....|.j...d..
+00001ec0: 0101 0064 0053 0029 024e 5429 0272 6500  ...d.S.).NT).re.
+00001ed0: 0000 721e 0000 0072 3b00 0000 7223 0000  ..r....r;...r#..
+00001ee0: 0072 2300 0000 7224 0000 0072 7700 0000  .r#...r$...rw...
+00001ef0: bf00 0000 7302 0000 0000 017a 1741 7070  ....s......z.App
+00001f00: 5769 6e64 6f77 2e68 6964 655f 696e 666f  Window.hide_info
+00001f10: 5f62 6f78 2901 724f 0000 0029 1e72 2500  _box).rO...).r%.
+00001f20: 0000 7226 0000 0072 2700 0000 7212 0000  ..r&...r'...r...
+00001f30: 0072 4600 0000 726d 0000 0072 0800 0000  .rF...rm...r....
+00001f40: 7271 0000 00da 0449 6e66 6f72 7500 0000  rq.....Inforu...
+00001f50: 7278 0000 0072 8000 0000 726c 0000 0072  rx...r....rl...r
+00001f60: 0900 0000 7251 0000 0072 8b00 0000 7229  ....rQ...r....r)
+00001f70: 0000 0072 8e00 0000 7293 0000 0072 2800  ...r....r....r(.
+00001f80: 0000 7295 0000 0072 8a00 0000 72a1 0000  ..r....r....r...
+00001f90: 0072 a200 0000 725a 0000 0072 9b00 0000  .r....rZ...r....
+00001fa0: 7291 0000 0072 7300 0000 7277 0000 0072  r....rs...rw...r
+00001fb0: 2a00 0000 7223 0000 0072 2300 0000 7221  *...r#...r#...r!
+00001fc0: 0000 0072 2400 0000 7253 0000 0042 0000  ...r$...rS...B..
+00001fd0: 0073 2400 0000 0801 0c05 101d 1a08 0804  .s$.............
+00001fe0: 0804 0804 1209 0e03 0e04 0e03 0812 0e06  ................
+00001ff0: 0c05 0e06 0e03 0806 1407 7253 0000 0029  ..........rS...)
+00002000: 19da 075f 5f64 6f63 5f5f da1e 6e61 6e6f  ...__doc__..nano
+00002010: 7375 7266 2e6c 6962 2e67 7569 2e69 6d70  surf.lib.gui.imp
+00002020: 6f72 745f 6865 6c70 6572 7202 0000 00da  ort_helperr.....
+00002030: 0750 7953 6964 6532 7203 0000 0072 0400  .PySide2r....r..
+00002040: 0000 7205 0000 00da 0750 7953 6964 6536  ..r......PySide6
+00002050: da0b 6461 7461 636c 6173 7365 7372 0600  ..dataclassesr..
+00002060: 0000 da08 6e61 6e6f 7375 7266 7218 0000  ....nanosurfr...
+00002070: 0072 4f00 0000 7208 0000 0072 0900 0000  .rO...r....r....
+00002080: 7249 0000 0072 1400 0000 720b 0000 0072  rI...r....r....r
+00002090: 6100 0000 722b 0000 00da 0b51 5370 6163  a...r+.....QSpac
+000020a0: 6572 4974 656d 7247 0000 0072 4d00 0000  erItemrG...rM...
+000020b0: da0b 514d 6169 6e57 696e 646f 7772 5300  ..QMainWindowrS.
+000020c0: 0000 7223 0000 0072 2300 0000 7223 0000  ..r#...r#...r#..
+000020d0: 0072 2400 0000 da08 3c6d 6f64 756c 653e  .r$.....<module>
+000020e0: 0100 0000 7320 0000 0004 050c 0106 010c  ....s ..........
+000020f0: 0116 020c 0114 010c 0108 0210 0204 0212  ................
+00002100: 0812 1d12 0402 0110 04                   .........
```

### Comparing `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/module_base.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/module_base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/module_base.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/module_base.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Apr 14 12:55:54 2023 UTC, .py size: 2271 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 5a4d 3964 df08 0000  a.......ZM9d....
+00000000: 610d 0d0a 0000 0000 cb03 5a64 9a08 0000  a.........Zd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6504  Z.d.d.l.m.Z...e.
 00000050: 8300 7238 6401 6404 6c05 6d06 5a06 6d07  ..r8d.d.l.m.Z.m.
 00000060: 5a07 0100 6e10 6401 6404 6c08 6d06 5a06  Z...n.d.d.l.m.Z.
 00000070: 6d07 5a07 0100 6405 5a09 4700 6406 6407  m.Z...d.Z.G.d.d.
@@ -44,166 +44,164 @@
 000002b0: 745f 5f29 05da 085f 5f6e 616d 655f 5fda  t__)...__name__.
 000002c0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
 000002d0: 7561 6c6e 616d 655f 5f72 0900 0000 da0d  ualname__r......
 000002e0: 5f5f 636c 6173 7363 656c 6c5f 5f72 1200  __classcell__r..
 000002f0: 0000 7212 0000 0072 1000 0000 7213 0000  ..r....r....r...
 00000300: 0072 0600 0000 1100 0000 7302 0000 0008  .r........s.....
 00000310: 0172 0600 0000 6300 0000 0000 0000 0000  .r....c.........
-00000320: 0000 0000 0000 0004 0000 0000 0000 0073  ...............s
-00000330: 6a00 0000 6500 5a01 6400 5a02 6401 6402  j...e.Z.d.Z.d.d.
-00000340: 6403 9c02 8700 6601 6404 6405 840c 5a03  d.....f.d.d...Z.
+00000320: 0000 0000 0000 0005 0000 0000 0000 0073  ...............s
+00000330: 6a00 0000 6500 5a01 6400 5a02 6413 6402  j...e.Z.d.Z.d.d.
+00000340: 6403 9c01 8700 6601 6404 6405 840d 5a03  d.....f.d.d...Z.
 00000350: 6406 6407 8400 5a04 6505 6408 6409 8400  d.d...Z.e.d.d...
 00000360: 8301 5a06 6505 640a 640b 8400 8301 5a07  ..Z.e.d.d.....Z.
 00000370: 6507 6a08 640c 640b 8400 8301 5a07 640d  e.j.d.d.....Z.d.
 00000380: 640e 8400 5a09 640f 6410 8400 5a0a 6411  d...Z.d.d...Z.d.
-00000390: 6412 8400 5a0b 8700 0400 5a0c 5300 2913  d...Z.....Z.S.).
-000003a0: da0a 4d6f 6475 6c65 4261 7365 da0f 4170  ..ModuleBase..Ap
-000003b0: 706c 6963 6174 696f 6e42 6173 65da 0c4d  plicationBase..M
-000003c0: 6f64 756c 6553 6372 6565 6e29 02da 0361  oduleScreen)...a
-000003d0: 7070 da03 6775 6963 0300 0000 0000 0000  pp..guic........
-000003e0: 0000 0000 0300 0000 0300 0000 0300 0000  ................
-000003f0: 7334 0000 0074 0083 00a0 01a1 0001 007c  s4...t.........|
-00000400: 017c 005f 027c 027c 005f 0364 007c 005f  .|._.|.|._.d.|._
-00000410: 0464 017c 005f 0574 06a0 077c 006a 05a1  .d.|._.t...|.j..
-00000420: 017c 005f 0864 0053 0029 024e da00 2909  .|._.d.S.).N..).
-00000430: 7208 0000 0072 0900 0000 721b 0000 00da  r....r....r.....
-00000440: 0275 69da 0873 6574 7469 6e67 73da 115f  .ui..settings.._
-00000450: 4d6f 6475 6c65 4261 7365 5f5f 6e61 6d65  ModuleBase__name
-00000460: da07 6c6f 6767 696e 67da 0967 6574 4c6f  ..logging..getLo
-00000470: 6767 6572 da06 6c6f 6767 6572 2903 720f  gger..logger).r.
-00000480: 0000 0072 1b00 0000 721c 0000 0072 1000  ...r....r....r..
-00000490: 0000 7212 0000 0072 1300 0000 7209 0000  ..r....r....r...
-000004a0: 0016 0000 0073 0c00 0000 0001 0a01 0601  .....s..........
-000004b0: 0601 0601 0601 7a13 4d6f 6475 6c65 4261  ......z.ModuleBa
-000004c0: 7365 2e5f 5f69 6e69 745f 5f63 0100 0000  se.__init__c....
-000004d0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-000004e0: 4300 0000 732e 0000 007c 006a 00a0 017c  C...s....|.j...|
-000004f0: 00a1 0101 007c 00a0 02a1 0001 007c 006a  .....|.......|.j
-00000500: 0364 006b 0372 2a7c 006a 03a0 047c 00a1  .d.k.r*|.j...|..
-00000510: 0101 0064 0053 00a9 014e 2905 721b 0000  ...d.S...N).r...
-00000520: 00da 0d6c 6f61 645f 7365 7474 696e 6773  ...load_settings
-00000530: da08 646f 5f73 7461 7274 721e 0000 00da  ..do_startr.....
-00000540: 0d63 7265 6174 655f 7363 7265 656e 720e  .create_screenr.
-00000550: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-00000560: 0000 da05 7374 6172 741e 0000 0073 0800  ....start....s..
-00000570: 0000 0001 0c02 0801 0a01 7a10 4d6f 6475  ..........z.Modu
-00000580: 6c65 4261 7365 2e73 7461 7274 6301 0000  leBase.startc...
-00000590: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-000005a0: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
-000005b0: 7224 0000 0029 0172 1e00 0000 720e 0000  r$...).r....r...
-000005c0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-000005d0: 721c 0000 0025 0000 0073 0200 0000 0002  r....%...s......
-000005e0: 7a0e 4d6f 6475 6c65 4261 7365 2e67 7569  z.ModuleBase.gui
-000005f0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000600: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
-00000610: 6a00 5300 7224 0000 0029 0172 2000 0000  j.S.r$...).r ...
-00000620: 720e 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00000630: 1300 0000 da04 6e61 6d65 2900 0000 7302  ......name)...s.
-00000640: 0000 0000 027a 0f4d 6f64 756c 6542 6173  .....z.ModuleBas
-00000650: 652e 6e61 6d65 6302 0000 0000 0000 0000  e.namec.........
-00000660: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-00000670: 1800 0000 7c01 7c00 5f00 7401 a002 7c00  ....|.|._.t...|.
-00000680: 6a00 a101 7c00 5f03 6400 5300 7224 0000  j...|._.d.S.r$..
-00000690: 0029 0472 2000 0000 7221 0000 0072 2200  .).r ...r!...r".
-000006a0: 0000 7223 0000 0029 0272 0f00 0000 7229  ..r#...).r....r)
-000006b0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-000006c0: 0000 7229 0000 002d 0000 0073 0400 0000  ..r)...-...s....
-000006d0: 0002 0601 6301 0000 0000 0000 0000 0000  ....c...........
-000006e0: 0001 0000 0003 0000 0043 0000 0073 1800  .........C...s..
-000006f0: 0000 7c00 a000 a100 0100 7c00 6a01 a002  ..|.......|.j...
-00000700: 7c00 a101 0100 6400 5300 7224 0000 0029  |.....d.S.r$...)
-00000710: 03da 0764 6f5f 7374 6f70 721b 0000 00da  ...do_stopr.....
-00000720: 0d73 6176 655f 7365 7474 696e 6773 720e  .save_settingsr.
-00000730: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-00000740: 0000 da04 7374 6f70 3200 0000 7304 0000  ....stop2...s...
-00000750: 0000 0108 017a 0f4d 6f64 756c 6542 6173  .....z.ModuleBas
-00000760: 652e 7374 6f70 6301 0000 0000 0000 0000  e.stopc.........
-00000770: 0000 0001 0000 0006 0000 0043 0000 0073  ...........C...s
-00000780: 2600 0000 7400 6401 7c00 6a01 6a02 9b00  &...t.d.|.j.j...
-00000790: 6402 7403 a004 a100 6a05 6a06 9b00 6403  d.t.....j.j...d.
-000007a0: 9d05 8301 8201 6400 5300 a904 4e7a 0d53  ......d.S...Nz.S
-000007b0: 7562 636c 6173 7320 6f66 2027 7a14 2720  ubclass of 'z.' 
-000007c0: 6861 7320 746f 2069 6d70 6c65 6d65 6e74  has to implement
-000007d0: 2027 7a03 2829 27a9 07da 134e 6f74 496d   'z.()'....NotIm
-000007e0: 706c 656d 656e 7465 6445 7272 6f72 7211  plementedErrorr.
-000007f0: 0000 0072 1400 0000 da03 7379 73da 095f  ...r......sys.._
-00000800: 6765 7466 7261 6d65 da06 665f 636f 6465  getframe..f_code
-00000810: da07 636f 5f6e 616d 6572 0e00 0000 7212  ..co_namer....r.
-00000820: 0000 0072 1200 0000 7213 0000 0072 2600  ...r....r....r&.
-00000830: 0000 3600 0000 7302 0000 0000 017a 134d  ..6...s......z.M
-00000840: 6f64 756c 6542 6173 652e 646f 5f73 7461  oduleBase.do_sta
-00000850: 7274 6301 0000 0000 0000 0000 0000 0001  rtc.............
-00000860: 0000 0006 0000 0043 0000 0073 2600 0000  .......C...s&...
-00000870: 7400 6401 7c00 6a01 6a02 9b00 6402 7403  t.d.|.j.j...d.t.
-00000880: a004 a100 6a05 6a06 9b00 6403 9d05 8301  ....j.j...d.....
-00000890: 8201 6400 5300 722d 0000 0072 2e00 0000  ..d.S.r-...r....
-000008a0: 720e 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-000008b0: 1300 0000 722a 0000 0039 0000 0073 0200  ....r*...9...s..
-000008c0: 0000 0001 7a12 4d6f 6475 6c65 4261 7365  ....z.ModuleBase
-000008d0: 2e64 6f5f 7374 6f70 290d 7214 0000 0072  .do_stop).r....r
-000008e0: 1500 0000 7216 0000 0072 0900 0000 7228  ....r....r....r(
-000008f0: 0000 00da 0870 726f 7065 7274 7972 1c00  .....propertyr..
-00000900: 0000 7229 0000 00da 0673 6574 7465 7272  ..r).....setterr
-00000910: 2c00 0000 7226 0000 0072 2a00 0000 7217  ,...r&...r*...r.
-00000920: 0000 0072 1200 0000 7212 0000 0072 1000  ...r....r....r..
-00000930: 0000 7213 0000 0072 1800 0000 1500 0000  ..r....r........
-00000940: 7316 0000 0008 0114 0808 0702 010a 0302  s...............
-00000950: 010a 0304 010a 0408 0408 0372 1800 0000  ...........r....
-00000960: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000970: 0003 0000 0000 0000 0073 3800 0000 6500  .........s8...e.
-00000980: 5a01 6400 5a02 8700 6601 6401 6402 8408  Z.d.Z...f.d.d...
-00000990: 5a03 6504 6403 9c01 6404 6405 8404 5a05  Z.e.d...d.d...Z.
-000009a0: 6504 6403 9c01 6406 6407 8404 5a06 8700  e.d...d.d...Z...
-000009b0: 0400 5a07 5300 2908 721a 0000 0063 0100  ..Z.S.).r....c..
-000009c0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-000009d0: 0000 0300 0000 7314 0000 0064 007c 005f  ......s....d.|._
-000009e0: 0074 0183 00a0 02a1 0001 0064 0053 0072  .t.........d.S.r
-000009f0: 2400 0000 2903 da06 6d6f 6475 6c65 7208  $...)...moduler.
-00000a00: 0000 0072 0900 0000 720e 0000 0072 1000  ...r....r....r..
-00000a10: 0000 7212 0000 0072 1300 0000 7209 0000  ..r....r....r...
-00000a20: 003d 0000 0073 0400 0000 0001 0601 7a15  .=...s........z.
-00000a30: 4d6f 6475 6c65 5363 7265 656e 2e5f 5f69  ModuleScreen.__i
-00000a40: 6e69 745f 5f29 0172 3600 0000 6302 0000  nit__).r6...c...
-00000a50: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00000a60: 0043 0000 0073 1400 0000 7c01 7c00 5f00  .C...s....|.|._.
-00000a70: 7c00 a001 7c01 a101 0100 6401 5300 2902  |...|.....d.S.).
-00000a80: 7a7e 0a20 2020 2020 2020 206c 6574 7320  z~.        lets 
-00000a90: 6372 6561 7465 2074 6865 2067 7569 2e20  create the gui. 
-00000aa0: 4372 6561 7465 7320 616c 6c20 4755 4920  Creates all GUI 
-00000ab0: 656c 656d 656e 7473 2062 7574 206e 6f20  elements but no 
-00000ac0: 6163 7469 6f6e 2079 6574 2e20 0a20 2020  action yet. .   
-00000ad0: 2020 2020 2054 6869 7320 6973 2064 6f6e       This is don
-00000ae0: 6520 6c61 7465 7220 696e 2043 6f6e 6e65  e later in Conne
-00000af0: 6374 4755 4928 290a 2020 2020 2020 2020  ctGUI().        
-00000b00: 4e29 0272 3600 0000 da0f 646f 5f73 6574  N).r6.....do_set
-00000b10: 7570 5f73 6372 6565 6ea9 0272 0f00 0000  up_screen..r....
-00000b20: 7236 0000 0072 1200 0000 7212 0000 0072  r6...r....r....r
-00000b30: 1300 0000 7227 0000 0041 0000 0073 0400  ....r'...A...s..
-00000b40: 0000 0005 0601 7a1a 4d6f 6475 6c65 5363  ......z.ModuleSc
-00000b50: 7265 656e 2e63 7265 6174 655f 7363 7265  reen.create_scre
-00000b60: 656e 6302 0000 0000 0000 0000 0000 0002  enc.............
-00000b70: 0000 0006 0000 0043 0000 0073 2600 0000  .......C...s&...
-00000b80: 7400 6401 7c00 6a01 6a02 9b00 6402 7403  t.d.|.j.j...d.t.
-00000b90: a004 a100 6a05 6a06 9b00 6403 9d05 8301  ....j.j...d.....
-00000ba0: 8201 6400 5300 722d 0000 0072 2e00 0000  ..d.S.r-...r....
-00000bb0: 7238 0000 0072 1200 0000 7212 0000 0072  r8...r....r....r
-00000bc0: 1300 0000 7237 0000 0049 0000 0073 0200  ....r7...I...s..
-00000bd0: 0000 0001 7a1c 4d6f 6475 6c65 5363 7265  ....z.ModuleScre
-00000be0: 656e 2e64 6f5f 7365 7475 705f 7363 7265  en.do_setup_scre
-00000bf0: 656e 2908 7214 0000 0072 1500 0000 7216  en).r....r....r.
-00000c00: 0000 0072 0900 0000 7218 0000 0072 2700  ...r....r....r'.
-00000c10: 0000 7237 0000 0072 1700 0000 7212 0000  ..r7...r....r...
-00000c20: 0072 1200 0000 7210 0000 0072 1300 0000  .r....r....r....
-00000c30: 721a 0000 003c 0000 0073 0600 0000 0801  r....<...s......
-00000c40: 0c04 0e08 721a 0000 0029 10da 075f 5f64  ....r....)...__d
-00000c50: 6f63 5f5f 7230 0000 0072 2100 0000 da1e  oc__r0...r!.....
-00000c60: 6e61 6e6f 7375 7266 2e6c 6962 2e67 7569  nanosurf.lib.gui
-00000c70: 2e69 6d70 6f72 745f 6865 6c70 6572 7202  .import_helperr.
-00000c80: 0000 00da 0750 7953 6964 6532 7203 0000  .....PySide2r...
-00000c90: 0072 0400 0000 da07 5079 5369 6465 3672  .r......PySide6r
-00000ca0: 0a00 0000 da0b 5153 7061 6365 7249 7465  ......QSpacerIte
-00000cb0: 6d72 0600 0000 da07 514f 626a 6563 7472  mr......QObjectr
-00000cc0: 1800 0000 da07 5157 6964 6765 7472 1a00  ......QWidgetr..
-00000cd0: 0000 7212 0000 0072 1200 0000 7212 0000  ..r....r....r...
-00000ce0: 0072 1300 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000cf0: 0100 0000 7314 0000 0004 0408 0108 020c  ....s...........
-00000d00: 0106 0112 0210 0304 0212 0412 27         ............'
+00000390: 6412 8400 5a0b 8700 0400 5a0c 5300 2914  d...Z.....Z.S.).
+000003a0: da0a 4d6f 6475 6c65 4261 7365 4eda 0f41  ..ModuleBaseN..A
+000003b0: 7070 6c69 6361 7469 6f6e 4261 7365 2901  pplicationBase).
+000003c0: da03 6170 7063 0300 0000 0000 0000 0000  ..appc..........
+000003d0: 0000 0300 0000 0300 0000 0300 0000 7334  ..............s4
+000003e0: 0000 0074 0083 00a0 01a1 0001 007c 017c  ...t.........|.|
+000003f0: 005f 027c 027c 005f 0364 007c 005f 0464  ._.|.|._.d.|._.d
+00000400: 017c 005f 0574 06a0 077c 006a 05a1 017c  .|._.t...|.j...|
+00000410: 005f 0864 0053 0029 024e da00 2909 7208  ._.d.S.).N..).r.
+00000420: 0000 0072 0900 0000 721a 0000 00da 0275  ...r....r......u
+00000430: 69da 0873 6574 7469 6e67 73da 115f 4d6f  i..settings.._Mo
+00000440: 6475 6c65 4261 7365 5f5f 6e61 6d65 da07  duleBase__name..
+00000450: 6c6f 6767 696e 67da 0967 6574 4c6f 6767  logging..getLogg
+00000460: 6572 da06 6c6f 6767 6572 2903 720f 0000  er..logger).r...
+00000470: 0072 1a00 0000 da03 6775 6972 1000 0000  .r......guir....
+00000480: 7212 0000 0072 1300 0000 7209 0000 0016  r....r....r.....
+00000490: 0000 0073 0c00 0000 0001 0a01 0601 0601  ...s............
+000004a0: 0601 0601 7a13 4d6f 6475 6c65 4261 7365  ....z.ModuleBase
+000004b0: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
+000004c0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+000004d0: 0000 7318 0000 007c 006a 00a0 017c 00a1  ..s....|.j...|..
+000004e0: 0101 007c 00a0 02a1 0001 0064 0053 00a9  ...|.......d.S..
+000004f0: 014e 2903 721a 0000 00da 0d6c 6f61 645f  .N).r......load_
+00000500: 7365 7474 696e 6773 da08 646f 5f73 7461  settings..do_sta
+00000510: 7274 720e 0000 0072 1200 0000 7212 0000  rtr....r....r...
+00000520: 0072 1300 0000 da05 7374 6172 741e 0000  .r......start...
+00000530: 0073 0400 0000 0001 0c01 7a10 4d6f 6475  .s........z.Modu
+00000540: 6c65 4261 7365 2e73 7461 7274 6301 0000  leBase.startc...
+00000550: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+00000560: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
+00000570: 7223 0000 0029 0172 1c00 0000 720e 0000  r#...).r....r...
+00000580: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000590: 7222 0000 0022 0000 0073 0200 0000 0002  r"..."...s......
+000005a0: 7a0e 4d6f 6475 6c65 4261 7365 2e67 7569  z.ModuleBase.gui
+000005b0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000005c0: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
+000005d0: 6a00 5300 7223 0000 0029 0172 1e00 0000  j.S.r#...).r....
+000005e0: 720e 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+000005f0: 1300 0000 da04 6e61 6d65 2600 0000 7302  ......name&...s.
+00000600: 0000 0000 027a 0f4d 6f64 756c 6542 6173  .....z.ModuleBas
+00000610: 652e 6e61 6d65 6302 0000 0000 0000 0000  e.namec.........
+00000620: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+00000630: 1800 0000 7c01 7c00 5f00 7401 a002 7c00  ....|.|._.t...|.
+00000640: 6a00 a101 7c00 5f03 6400 5300 7223 0000  j...|._.d.S.r#..
+00000650: 0029 0472 1e00 0000 721f 0000 0072 2000  .).r....r....r .
+00000660: 0000 7221 0000 0029 0272 0f00 0000 7227  ..r!...).r....r'
+00000670: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
+00000680: 0000 7227 0000 002a 0000 0073 0400 0000  ..r'...*...s....
+00000690: 0002 0601 6301 0000 0000 0000 0000 0000  ....c...........
+000006a0: 0001 0000 0003 0000 0043 0000 0073 1800  .........C...s..
+000006b0: 0000 7c00 a000 a100 0100 7c00 6a01 a002  ..|.......|.j...
+000006c0: 7c00 a101 0100 6400 5300 7223 0000 0029  |.....d.S.r#...)
+000006d0: 03da 0764 6f5f 7374 6f70 721a 0000 00da  ...do_stopr.....
+000006e0: 0d73 6176 655f 7365 7474 696e 6773 720e  .save_settingsr.
+000006f0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
+00000700: 0000 da04 7374 6f70 2f00 0000 7304 0000  ....stop/...s...
+00000710: 0000 0108 017a 0f4d 6f64 756c 6542 6173  .....z.ModuleBas
+00000720: 652e 7374 6f70 6301 0000 0000 0000 0000  e.stopc.........
+00000730: 0000 0001 0000 0006 0000 0043 0000 0073  ...........C...s
+00000740: 2600 0000 7400 6401 7c00 6a01 6a02 9b00  &...t.d.|.j.j...
+00000750: 6402 7403 a004 a100 6a05 6a06 9b00 6403  d.t.....j.j...d.
+00000760: 9d05 8301 8201 6400 5300 a904 4e7a 0d53  ......d.S...Nz.S
+00000770: 7562 636c 6173 7320 6f66 2027 7a14 2720  ubclass of 'z.' 
+00000780: 6861 7320 746f 2069 6d70 6c65 6d65 6e74  has to implement
+00000790: 2027 7a03 2829 27a9 07da 134e 6f74 496d   'z.()'....NotIm
+000007a0: 706c 656d 656e 7465 6445 7272 6f72 7211  plementedErrorr.
+000007b0: 0000 0072 1400 0000 da03 7379 73da 095f  ...r......sys.._
+000007c0: 6765 7466 7261 6d65 da06 665f 636f 6465  getframe..f_code
+000007d0: da07 636f 5f6e 616d 6572 0e00 0000 7212  ..co_namer....r.
+000007e0: 0000 0072 1200 0000 7213 0000 0072 2500  ...r....r....r%.
+000007f0: 0000 3300 0000 7302 0000 0000 017a 134d  ..3...s......z.M
+00000800: 6f64 756c 6542 6173 652e 646f 5f73 7461  oduleBase.do_sta
+00000810: 7274 6301 0000 0000 0000 0000 0000 0001  rtc.............
+00000820: 0000 0006 0000 0043 0000 0073 2600 0000  .......C...s&...
+00000830: 7400 6401 7c00 6a01 6a02 9b00 6402 7403  t.d.|.j.j...d.t.
+00000840: a004 a100 6a05 6a06 9b00 6403 9d05 8301  ....j.j...d.....
+00000850: 8201 6400 5300 722b 0000 0072 2c00 0000  ..d.S.r+...r,...
+00000860: 720e 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00000870: 1300 0000 7228 0000 0036 0000 0073 0200  ....r(...6...s..
+00000880: 0000 0001 7a12 4d6f 6475 6c65 4261 7365  ....z.ModuleBase
+00000890: 2e64 6f5f 7374 6f70 2901 4e29 0d72 1400  .do_stop).N).r..
+000008a0: 0000 7215 0000 0072 1600 0000 7209 0000  ..r....r....r...
+000008b0: 0072 2600 0000 da08 7072 6f70 6572 7479  .r&.....property
+000008c0: 7222 0000 0072 2700 0000 da06 7365 7474  r"...r'.....sett
+000008d0: 6572 722a 0000 0072 2500 0000 7228 0000  err*...r%...r(..
+000008e0: 0072 1700 0000 7212 0000 0072 1200 0000  .r....r....r....
+000008f0: 7210 0000 0072 1300 0000 7218 0000 0015  r....r....r.....
+00000900: 0000 0073 1600 0000 0801 1408 0804 0201  ...s............
+00000910: 0a03 0201 0a03 0401 0a04 0804 0803 7218  ..............r.
+00000920: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000930: 0000 0000 0300 0000 0000 0000 7338 0000  ............s8..
+00000940: 0065 005a 0164 005a 0287 0066 0164 0164  .e.Z.d.Z...f.d.d
+00000950: 0284 085a 0365 0464 039c 0164 0464 0584  ...Z.e.d...d.d..
+00000960: 045a 0565 0464 039c 0164 0664 0784 045a  .Z.e.d...d.d...Z
+00000970: 0687 0004 005a 0753 0029 08da 0c4d 6f64  .....Z.S.)...Mod
+00000980: 756c 6553 6372 6565 6e63 0100 0000 0000  uleScreenc......
+00000990: 0000 0000 0000 0100 0000 0200 0000 0300  ................
+000009a0: 0000 7314 0000 0064 007c 005f 0074 0183  ..s....d.|._.t..
+000009b0: 00a0 02a1 0001 0064 0053 0072 2300 0000  .......d.S.r#...
+000009c0: 2903 da06 6d6f 6475 6c65 7208 0000 0072  )...moduler....r
+000009d0: 0900 0000 720e 0000 0072 1000 0000 7212  ....r....r....r.
+000009e0: 0000 0072 1300 0000 7209 0000 003a 0000  ...r....r....:..
+000009f0: 0073 0400 0000 0001 0601 7a15 4d6f 6475  .s........z.Modu
+00000a00: 6c65 5363 7265 656e 2e5f 5f69 6e69 745f  leScreen.__init_
+00000a10: 5f29 0172 3500 0000 6302 0000 0000 0000  _).r5...c.......
+00000a20: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00000a30: 0073 1400 0000 7c01 7c00 5f00 7c00 a001  .s....|.|._.|...
+00000a40: 7c01 a101 0100 6401 5300 2902 7a7e 0a20  |.....d.S.).z~. 
+00000a50: 2020 2020 2020 206c 6574 7320 6372 6561         lets crea
+00000a60: 7465 2074 6865 2067 7569 2e20 4372 6561  te the gui. Crea
+00000a70: 7465 7320 616c 6c20 4755 4920 656c 656d  tes all GUI elem
+00000a80: 656e 7473 2062 7574 206e 6f20 6163 7469  ents but no acti
+00000a90: 6f6e 2079 6574 2e20 0a20 2020 2020 2020  on yet. .       
+00000aa0: 2054 6869 7320 6973 2064 6f6e 6520 6c61   This is done la
+00000ab0: 7465 7220 696e 2043 6f6e 6e65 6374 4755  ter in ConnectGU
+00000ac0: 4928 290a 2020 2020 2020 2020 4e29 0272  I().        N).r
+00000ad0: 3500 0000 da0f 646f 5f73 6574 7570 5f73  5.....do_setup_s
+00000ae0: 6372 6565 6ea9 0272 0f00 0000 7235 0000  creen..r....r5..
+00000af0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000b00: da0d 6372 6561 7465 5f73 6372 6565 6e3e  ..create_screen>
+00000b10: 0000 0073 0400 0000 0005 0601 7a1a 4d6f  ...s........z.Mo
+00000b20: 6475 6c65 5363 7265 656e 2e63 7265 6174  duleScreen.creat
+00000b30: 655f 7363 7265 656e 6302 0000 0000 0000  e_screenc.......
+00000b40: 0000 0000 0002 0000 0006 0000 0043 0000  .............C..
+00000b50: 0073 2600 0000 7400 6401 7c00 6a01 6a02  .s&...t.d.|.j.j.
+00000b60: 9b00 6402 7403 a004 a100 6a05 6a06 9b00  ..d.t.....j.j...
+00000b70: 6403 9d05 8301 8201 6400 5300 722b 0000  d.......d.S.r+..
+00000b80: 0072 2c00 0000 7237 0000 0072 1200 0000  .r,...r7...r....
+00000b90: 7212 0000 0072 1300 0000 7236 0000 0046  r....r....r6...F
+00000ba0: 0000 0073 0200 0000 0001 7a1c 4d6f 6475  ...s......z.Modu
+00000bb0: 6c65 5363 7265 656e 2e64 6f5f 7365 7475  leScreen.do_setu
+00000bc0: 705f 7363 7265 656e 2908 7214 0000 0072  p_screen).r....r
+00000bd0: 1500 0000 7216 0000 0072 0900 0000 7218  ....r....r....r.
+00000be0: 0000 0072 3800 0000 7236 0000 0072 1700  ...r8...r6...r..
+00000bf0: 0000 7212 0000 0072 1200 0000 7210 0000  ..r....r....r...
+00000c00: 0072 1300 0000 7234 0000 0039 0000 0073  .r....r4...9...s
+00000c10: 0600 0000 0801 0c04 0e08 7234 0000 0029  ..........r4...)
+00000c20: 10da 075f 5f64 6f63 5f5f 722e 0000 0072  ...__doc__r....r
+00000c30: 1f00 0000 da1e 6e61 6e6f 7375 7266 2e6c  ......nanosurf.l
+00000c40: 6962 2e67 7569 2e69 6d70 6f72 745f 6865  ib.gui.import_he
+00000c50: 6c70 6572 7202 0000 00da 0750 7953 6964  lperr......PySid
+00000c60: 6532 7203 0000 0072 0400 0000 da07 5079  e2r....r......Py
+00000c70: 5369 6465 3672 0a00 0000 da0b 5153 7061  Side6r......QSpa
+00000c80: 6365 7249 7465 6d72 0600 0000 da07 514f  cerItemr......QO
+00000c90: 626a 6563 7472 1800 0000 da07 5157 6964  bjectr......QWid
+00000ca0: 6765 7472 3400 0000 7212 0000 0072 1200  getr4...r....r..
+00000cb0: 0000 7212 0000 0072 1300 0000 da08 3c6d  ..r....r......<m
+00000cc0: 6f64 756c 653e 0100 0000 7314 0000 0004  odule>....s.....
+00000cd0: 0408 0108 020c 0106 0112 0210 0304 0212  ................
+00000ce0: 0412 24                                  ..$
```

### Comparing `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/nsf_thread.cpython-310.pyc` & `nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/nsf_thread.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/nsf_thread.cpython-39.pyc` & `nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/__pycache__/nsf_thread.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/app_base.py` & `nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/app_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     from PySide6.QtWidgets import QApplication
     from PySide6.QtCore import QSettings
 
 
 import nanosurf as nsf
 from nanosurf.lib.frameworks.qt_app.app_gui import AppWindow
 from nanosurf.lib.frameworks.qt_app.app_common import MsgType
-from nanosurf.lib.frameworks.qt_app.module_base import ModuleBase
+from nanosurf.lib.frameworks.qt_app.module_base import ModuleBase, ModuleScreen
 from nanosurf.lib.datatypes.prop_val import PropStore, PropVal
 
 dir_name_log = "log"
 dir_name_config = "config"
 
 class AppSettings(PropStore):
     Logging  = PropVal(True)
@@ -62,15 +62,15 @@
         nsf.util.fileutil.create_folder(self.config_path)
         nsf.datatypes.prop_val.load_from_ini_file(self.settings, self.config_file, self.config_section)   
         self.setup_logger()
         self.appwindow = AppWindow(self)
         self.appwindow.create_gui(self.resource_path / "app_stylesheet.qss", self.resource_path / "app_icon.ico")
         self.lastWindowClosed.connect(self.quit_app)
         self.do_startup()
-        self.activate_module(self.settings.ActiveModuleIndex.value)
+        self.appwindow.activate_screen(self.settings.ActiveModuleIndex.value)
         self.appwindow.show()
         self.logger.info("App running...")
 
     def quit_app(self):
         self.stop_modules()
         self.do_shutdown()
         nsf.datatypes.prop_val.save_to_ini_file(self.settings, self.config_file, self.config_section)   
@@ -128,21 +128,27 @@
         
     def clear_message(self):
         self.appwindow.hide_message()
 
     def show_message(self, msg: str, msg_type: MsgType = MsgType.Info):
         self.appwindow.show_message(msg, msg_type)
 
-    def add_module(self, new_module: ModuleBase, name:str ="Module"):
+    def add_module(self, new_module: ModuleBase, name:str ="Module", new_screen:ModuleScreen = None):
         new_module.name = name
+        if new_screen is not None:
+            new_module.ui = new_screen
         self.logger.info(f"Start module: {new_module.name}")
         self.modules[new_module.name] = new_module
         new_module.start()
-        self.appwindow.add_screen(new_module)
-        self.appwindow.update_menu(self.modules)
+        if new_module.ui is not None:
+            self.add_screen(new_module, new_module.ui, name)
+      
+    def add_screen(self, module: ModuleBase, new_screen:ModuleScreen, screen_name:str ="Screen"):
+        new_screen.create_screen(module)
+        self.appwindow.add_screen(new_screen, screen_name)
 
     def get_module_count(self) -> int:
         return len(self.modules)     
 
     def activate_module(self, module_index: int):
         self.settings.ActiveModuleIndex.value = module_index
         self.appwindow.set_active_module_by_index(module_index)
```

### Comparing `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/app_gui.py` & `nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/app_gui.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from nanosurf.lib.gui.import_helper import import_pyside2_if_none_is_detected
 if import_pyside2_if_none_is_detected():
     from PySide2 import QtWidgets
     from PySide2 import QtGui, QtWidgets, QtCore
 else:
     from PySide6 import QtWidgets
     from PySide6 import QtGui, QtWidgets, QtCore
-
+from dataclasses import dataclass
 import nanosurf as nsf
 
 from . import app_common, module_base
 
 control_layout_width = 200
 
 class MenuSeparator(QtWidgets.QFrame):
@@ -54,18 +54,24 @@
         self.setLayout(layout)      
 
 
 class StdVSpacer(QtWidgets.QSpacerItem):
     def __init__(self):
         super().__init__(control_layout_width, 40, QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.MinimumExpanding)
 
+@dataclass
+class ScreenDef:
+    screen:module_base.ModuleScreen = None
+    name:str = ""
+
 class AppWindow(QtWidgets.QMainWindow):
     def __init__(self, app):
         super().__init__()
         self.app = app
+        self.list_of_screens:list[ScreenDef] = []
 
     def create_gui(self, ui_style_file : str, icon_file : str):
         # create main GUI layout
         style_sheet_str = self._read_style_sheet_into_str(ui_style_file)
         self.setStyleSheet(style_sheet_str)
         self.setWindowTitle(self.app.app_name_long)
         self.setWindowIcon(QtGui.QIcon(str(icon_file)))
@@ -108,73 +114,70 @@
         self.app.registry.setValue("geometry", self.saveGeometry())
         self.app.registry.setValue("windowState", self.saveState())
     
     def load_window_size(self):
         self.restoreGeometry(self.app.registry.value("geometry"))
         self.restoreState(self.app.registry.value("windowState"))
 
-    def add_screen(self, module: module_base.ModuleBase):
-        module_gui = module.gui
-        if isinstance(module_gui, QtWidgets.QWidget):
-            self.main_stack.addWidget(module_gui)
+    def add_screen(self, gui: module_base.ModuleScreen, screen_name:str):
+        self.list_of_screens.append(ScreenDef(gui, screen_name))
+        if isinstance(gui, QtWidgets.QWidget):
+            self.main_stack.addWidget(gui)
             # activate first screen 
             if self.main_stack.currentIndex() == 0:
-                self.main_stack.setCurrentWidget(module_gui)
+                self.main_stack.setCurrentWidget(gui)
+        self.update_menu()
 
     def get_active_module_index(self) -> int:
         return self.main_stack.currentIndex() - 1
 
     def set_active_module_by_index(self, index: int):
         self.main_stack.setCurrentIndex(index+1)
         self._update_menu_button_highlight()
 
     def is_menu_visible(self) -> bool:
-        return self.app.get_module_count() > 1
-
-    def update_menu(self, modules: dict):
-        mod_with_gui = 0
-        for mod in modules.values():
-            if mod.gui is not None:
-                mod_with_gui += 1
+        return len(self.list_of_screens) > 0
 
+    def update_menu(self):
+        num_of_screens = len(self.list_of_screens)
         # show menu only if there are more than one modules with gui present
-        if mod_with_gui > 1:
+        if num_of_screens > 1:
             #remove all menu items
             while self.main_menu.count():
                 child = self.main_menu.takeAt(0)
                 if child.widget() is not None:
                     child.widget().deleteLater()
-
             # add menu items
-            menuindex = 0
-            for mod in modules.values():
-                if mod.gui is not None:
-                    menuitem = MenuButton(mod.name, menuindex)
+            for menuindex, screendef in enumerate(self.list_of_screens):
+                    menuitem = MenuButton(screendef.name, menuindex)
                     menuitem.sig_on_menu_clicked.connect(self._on_menu_button_clicked)
                     self.main_menu.addWidget(menuitem)
-                    menuindex += 1
             self.main_menu.addStretch() 
 
-        self.menu_sep.setHidden(mod_with_gui <= 1)
+        self.menu_sep.setHidden(num_of_screens <= 1)
         
+    def activate_screen(self, screen_index: int):
+        self.app.settings.ActiveModuleIndex.value = screen_index
+        self.set_active_module_by_index(screen_index)   
+                
     # internal use only
 
     def closeEvent(self, arg):
         """ capture close button from application window"""
         self.save_window_size()
         super().closeEvent(arg)
 
     def _read_style_sheet_into_str(self, style_file: str):
         style = ""
         with open(style_file) as f:
             style = f.read()
         return style
     
     def _on_menu_button_clicked(self, index: int):
-        self.app.activate_module(index)
+        self.activate_screen(index)
 
     def _update_menu_button_highlight(self):
         if self.is_menu_visible():
             active_index = self.get_active_module_index()
             for i in range(self.main_menu.count()-1):
                 self.main_menu.itemAt(i).widget().set_highlight(i == active_index)
```

### Comparing `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/app_icon.ico` & `nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/app_icon.ico`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/app_stylesheet.qss` & `nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/app_stylesheet.qss`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/module_base.py` & `nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/module_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,28 +15,25 @@
 control_layout_width = 200
 
 class CtrlSpacer(QtWidgets.QSpacerItem):
     def __init__(self):
         super().__init__(control_layout_width,40, QtWidgets.QSizePolicy.Fixed,QtWidgets.QSizePolicy.MinimumExpanding)
 
 class ModuleBase(QtCore.QObject):
-    def __init__(self, app:'ApplicationBase', gui:'ModuleScreen'):
+    def __init__(self, app:'ApplicationBase', gui = None):
         super().__init__()
         self.app:ApplicationBase = app
         self.ui:ModuleScreen = gui
         self.settings = None
         self.__name = ""
         self.logger = logging.getLogger(self.__name)
  
     def start(self):
         self.app.load_settings(self)
-
         self.do_start()
-        if self.ui != None:
-            self.ui.create_screen(self)
 
     @property
     def gui(self):
         return self.ui
 
     @property
     def name(self):
@@ -55,15 +52,15 @@
         raise NotImplementedError(f"Subclass of '{self.__class__.__name__}' has to implement '{sys._getframe().f_code.co_name}()'")
 
     def do_stop(self):
         raise NotImplementedError(f"Subclass of '{self.__class__.__name__}' has to implement '{sys._getframe().f_code.co_name}()'")
 
 class ModuleScreen(QtWidgets.QWidget):
     def __init__(self):
-        self.module = None
+        self.module:ModuleBase = None
         super().__init__()
 
     def create_screen(self, module: ModuleBase):
         """
         lets create the gui. Creates all GUI elements but no action yet. 
         This is done later in ConnectGUI()
         """
```

### Comparing `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/nsf_thread.py` & `nanosurf-1.6.2/nanosurf/lib/frameworks/qt_app/nsf_thread.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/gui/__init__.py` & `nanosurf-1.6.2/nanosurf/lib/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/gui/bind_gui.py` & `nanosurf-1.6.2/nanosurf/lib/gui/bind_gui.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/gui/import_helper.py` & `nanosurf-1.6.2/nanosurf/lib/gui/import_helper.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/gui/nsf_combobox.py` & `nanosurf-1.6.2/nanosurf/lib/gui/nsf_combobox.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/gui/nsf_edit.py` & `nanosurf-1.6.2/nanosurf/lib/gui/nsf_edit.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/gui/nsf_info_box.py` & `nanosurf-1.6.2/nanosurf/lib/gui/nsf_info_box.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/gui/nsf_plots.py` & `nanosurf-1.6.2/nanosurf/lib/gui/nsf_plots.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/gui/nsf_sci_edit.py` & `nanosurf-1.6.2/nanosurf/lib/gui/nsf_sci_edit.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/gui/nsf_tables.py` & `nanosurf-1.6.2/nanosurf/lib/gui/nsf_tables.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/math/iir_filter.py` & `nanosurf-1.6.2/nanosurf/lib/math/iir_filter.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/math/sci_math.py` & `nanosurf-1.6.2/nanosurf/lib/math/sci_math.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/plot.py` & `nanosurf-1.6.2/nanosurf/lib/plot.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/__init__.py` & `nanosurf-1.6.2/nanosurf/lib/spm/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/com_proxy.py` & `nanosurf-1.6.2/nanosurf/lib/spm/com_proxy.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/__init__.py` & `nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/check.py` & `nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/check.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/__init__.py` & `nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/adc.py` & `nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/adc.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/analyzer.py` & `nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/analyzer.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/capture.py` & `nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/capture.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/channelmux.py` & `nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/channelmux.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/dac.py` & `nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/dac.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/factory.py` & `nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/factory.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/sampler.py` & `nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/ctrlunits/sampler.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/data_buffer.py` & `nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/data_buffer.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/data_buffer_interface.py` & `nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/data_buffer_interface.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/iir_filter.py` & `nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/iir_filter.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/logical_unit_interface.py` & `nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/logical_unit_interface.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/logical_unit_interface_parser.py` & `nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/logical_unit_interface_parser.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/manager_mock.py` & `nanosurf-1.6.2/nanosurf/lib/spm/lowlevel/manager_mock.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/scanhead/__init__.py` & `nanosurf-1.6.2/nanosurf/lib/spm/scanhead/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/scanhead/drive_afm.py` & `nanosurf-1.6.2/nanosurf/lib/spm/scanhead/drive_afm.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/scanhead/motor_control.py` & `nanosurf-1.6.2/nanosurf/lib/spm/scanhead/motor_control.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/scanhead/studio_motor_control.py` & `nanosurf-1.6.2/nanosurf/lib/spm/scanhead/studio_motor_control.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/spm_app.py` & `nanosurf-1.6.2/nanosurf/lib/spm/spm_app.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/studio/__init__.py` & `nanosurf-1.6.2/nanosurf/lib/spm/studio/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/studio/wrapper/__init__.py` & `nanosurf-1.6.2/nanosurf/lib/spm/studio/wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/studio/wrapper/cmd_tree_main.py` & `nanosurf-1.6.2/nanosurf/lib/spm/studio/wrapper/cmd_tree_main.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/studio/wrapper/cmd_tree_spm.py` & `nanosurf-1.6.2/nanosurf/lib/spm/studio/wrapper/cmd_tree_spm.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/spm/workflow/frequency_sweep.py` & `nanosurf-1.6.2/nanosurf/lib/spm/workflow/frequency_sweep.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/util/dataexport.py` & `nanosurf-1.6.2/nanosurf/lib/util/dataexport.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf/lib/util/fileutil.py` & `nanosurf-1.6.2/nanosurf/lib/util/fileutil.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/nanosurf.egg-info/PKG-INFO` & `nanosurf-1.6.2/nanosurf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanosurf
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python API for Nanosurf controllers
 Author: Nanosurf AG
 Author-email: scripting@nanosurf.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -145,14 +145,18 @@
 
 Full list of objects and methods can be found in the Scripting Manual
 in Nanosurf controller software under Help tab:
 Help -> Manuals -> Script Programmers Manual, or [here](https://www.nanosurf.com/downloads/programmers-manual.pdf).
 
 ## Library Version History
 
+* v1.6.2
+  * New: qt_app_framwork supports multi screen modules
+  * Bugfix: settings should not be of dataclass type
+
 * v1.6.1
   * Bugfix: pip packaging did not copy framework files
 
 * v1.6.0
   * New: spm_template: A new template to demonstrate simple connection to CX/Studio and measure some data
   * New: app_DriveAFM_Tip_Current_Addon this app controls the amplifier of the Tip-Current Addon
   * New: demo_move_sample_stage. This demo shows basic stage movements
```

### Comparing `nanosurf-1.6.1/nanosurf.egg-info/SOURCES.txt` & `nanosurf-1.6.2/nanosurf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.1/setup.py` & `nanosurf-1.6.2/setup.py`

 * *Files identical despite different names*

