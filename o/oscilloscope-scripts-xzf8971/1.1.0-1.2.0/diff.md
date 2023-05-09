# Comparing `tmp/oscilloscope_scripts_xzf8971-1.1.0.tar.gz` & `tmp/oscilloscope_scripts_xzf8971-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pi/Documents/zifengCode/oscilloscope_scripts/dist/tmpcv6ri_m8/oscilloscope_scripts_xzf8971-1.1.0.tar", last modified: Tue Nov 15 11:43:31 2022, max compression
+gzip compressed data, was "C:\Users\zifeng\Documents\zifengCode\oscilloscope_scripts\dist\.tmp-wn5yao9o\oscilloscope_scripts_xzf8971-1.2.0.tar", last modified: Tue May  9 09:29:54 2023, max compression
```

## Comparing `oscilloscope_scripts_xzf8971-1.1.0.tar` & `oscilloscope_scripts_xzf8971-1.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-11-15 11:43:31.000000 oscilloscope_scripts_xzf8971-1.1.0/
--rw-r--r--   0 pi        (1000) pi        (1000)     1174 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/.gitignore
--rw-r--r--   0 pi        (1000) pi        (1000)     1067 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     3477 2022-11-15 11:43:31.000000 oscilloscope_scripts_xzf8971-1.1.0/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     2879 2022-11-15 11:10:55.000000 oscilloscope_scripts_xzf8971-1.1.0/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-11-15 11:43:31.000000 oscilloscope_scripts_xzf8971-1.1.0/Tektronix_TBS2000B_analysis/
--rw-r--r--   0 pi        (1000) pi        (1000)     8374 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/Tektronix_TBS2000B_analysis/QuickAnalysis.py
--rw-r--r--   0 pi        (1000) pi        (1000)       28 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/Tektronix_TBS2000B_analysis/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1388 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/Tektronix_TBS2000B_analysis/__main__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-11-15 11:43:31.000000 oscilloscope_scripts_xzf8971-1.1.0/Tektronix_TBS2000B_control/
--rw-r--r--   0 pi        (1000) pi        (1000)       34 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/Tektronix_TBS2000B_control/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     8168 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/Tektronix_TBS2000B_control/oscilloscope_control.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-11-15 11:43:31.000000 oscilloscope_scripts_xzf8971-1.1.0/Tektronix_TBS2000B_scripts/
--rw-r--r--   0 pi        (1000) pi        (1000)       29 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/Tektronix_TBS2000B_scripts/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3290 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/Tektronix_TBS2000B_scripts/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4618 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/Tektronix_TBS2000B_scripts/helper_function.py
--rw-r--r--   0 pi        (1000) pi        (1000)       82 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-11-15 11:43:31.000000 oscilloscope_scripts_xzf8971-1.1.0/oscilloscope_scripts_xzf8971.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     3477 2022-11-15 11:43:31.000000 oscilloscope_scripts_xzf8971-1.1.0/oscilloscope_scripts_xzf8971.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     1282 2022-11-15 11:43:31.000000 oscilloscope_scripts_xzf8971-1.1.0/oscilloscope_scripts_xzf8971.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2022-11-15 11:43:31.000000 oscilloscope_scripts_xzf8971-1.1.0/oscilloscope_scripts_xzf8971.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2022-11-15 11:40:08.000000 oscilloscope_scripts_xzf8971-1.1.0/oscilloscope_scripts_xzf8971.egg-info/not-zip-safe
--rw-r--r--   0 pi        (1000) pi        (1000)       50 2022-11-15 11:43:31.000000 oscilloscope_scripts_xzf8971-1.1.0/oscilloscope_scripts_xzf8971.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       82 2022-11-15 11:43:31.000000 oscilloscope_scripts_xzf8971-1.1.0/oscilloscope_scripts_xzf8971.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      793 2022-11-15 11:38:57.000000 oscilloscope_scripts_xzf8971-1.1.0/pyproject.toml
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-11-15 11:43:31.000000 oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/
--rw-r--r--   0 pi        (1000) pi        (1000)     6869 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/MakeWorkspaceForGain.C
--rw-r--r--   0 pi        (1000) pi        (1000)     3745 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/OutputCharge.C
--rw-r--r--   0 pi        (1000) pi        (1000)     3108 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/OutputCharge.h
--rw-r--r--   0 pi        (1000) pi        (1000)     3897 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/Plot_waveform_from_root.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5001 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/Transform_csv_to_tree.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7083 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/UseWorkspaceForFit.C
--rw-r--r--   0 pi        (1000) pi        (1000)     1433 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/analysis_waveform_data.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-11-15 11:43:31.000000 oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/naive_bayesian_classifier/
--rw-r--r--   0 pi        (1000) pi        (1000)     1561 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/naive_bayesian_classifier/Event.py
--rw-r--r--   0 pi        (1000) pi        (1000)     8269 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/naive_bayesian_classifier/naive_bayesian_classifier.py
--rw-r--r--   0 pi        (1000) pi        (1000)     8291 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/naive_bayesian_classifier/naive_bayesian_classifier_CH2.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6398 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/single_channel_selector.C
--rw-r--r--   0 pi        (1000) pi        (1000)     3343 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/single_channel_selector.h
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2022-11-15 11:43:31.000000 oscilloscope_scripts_xzf8971-1.1.0/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      128 2022-11-03 07:56:02.000000 oscilloscope_scripts_xzf8971-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:29:54.196194 oscilloscope_scripts_xzf8971-1.2.0/
+-rw-rw-rw-   0        0        0     1277 2022-11-01 14:30:47.000000 oscilloscope_scripts_xzf8971-1.2.0/.gitignore
+-rw-rw-rw-   0        0        0     1088 2022-10-30 06:36:02.000000 oscilloscope_scripts_xzf8971-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3603 2023-05-09 09:29:54.194157 oscilloscope_scripts_xzf8971-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2991 2023-05-09 09:16:56.000000 oscilloscope_scripts_xzf8971-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 09:29:54.121197 oscilloscope_scripts_xzf8971-1.2.0/Tektronix_TBS2000B_analysis/
+-rw-rw-rw-   0        0        0     8599 2022-11-01 13:54:57.000000 oscilloscope_scripts_xzf8971-1.2.0/Tektronix_TBS2000B_analysis/QuickAnalysis.py
+-rw-rw-rw-   0        0        0       29 2022-11-01 13:55:00.000000 oscilloscope_scripts_xzf8971-1.2.0/Tektronix_TBS2000B_analysis/__init__.py
+-rw-rw-rw-   0        0        0     1416 2022-11-01 13:54:40.000000 oscilloscope_scripts_xzf8971-1.2.0/Tektronix_TBS2000B_analysis/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:29:54.126207 oscilloscope_scripts_xzf8971-1.2.0/Tektronix_TBS2000B_control/
+-rw-rw-rw-   0        0        0       34 2022-11-01 12:27:09.000000 oscilloscope_scripts_xzf8971-1.2.0/Tektronix_TBS2000B_control/__init__.py
+-rw-rw-rw-   0        0        0     8368 2022-11-01 08:20:54.000000 oscilloscope_scripts_xzf8971-1.2.0/Tektronix_TBS2000B_control/oscilloscope_control.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:29:54.134725 oscilloscope_scripts_xzf8971-1.2.0/Tektronix_TBS2000B_scripts/
+-rw-rw-rw-   0        0        0       29 2022-11-01 13:44:09.000000 oscilloscope_scripts_xzf8971-1.2.0/Tektronix_TBS2000B_scripts/__init__.py
+-rw-rw-rw-   0        0        0     3500 2023-05-09 09:16:32.000000 oscilloscope_scripts_xzf8971-1.2.0/Tektronix_TBS2000B_scripts/__main__.py
+-rw-rw-rw-   0        0        0     4728 2022-11-01 13:37:20.000000 oscilloscope_scripts_xzf8971-1.2.0/Tektronix_TBS2000B_scripts/helper_function.py
+-rw-rw-rw-   0        0        0       83 2022-11-01 12:49:49.000000 oscilloscope_scripts_xzf8971-1.2.0/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:29:54.154426 oscilloscope_scripts_xzf8971-1.2.0/oscilloscope_scripts_xzf8971.egg-info/
+-rw-rw-rw-   0        0        0     3603 2023-05-09 09:29:53.000000 oscilloscope_scripts_xzf8971-1.2.0/oscilloscope_scripts_xzf8971.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1282 2023-05-09 09:29:54.000000 oscilloscope_scripts_xzf8971-1.2.0/oscilloscope_scripts_xzf8971.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 09:29:53.000000 oscilloscope_scripts_xzf8971-1.2.0/oscilloscope_scripts_xzf8971.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-09 09:29:52.000000 oscilloscope_scripts_xzf8971-1.2.0/oscilloscope_scripts_xzf8971.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       50 2023-05-09 09:29:53.000000 oscilloscope_scripts_xzf8971-1.2.0/oscilloscope_scripts_xzf8971.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       82 2023-05-09 09:29:53.000000 oscilloscope_scripts_xzf8971-1.2.0/oscilloscope_scripts_xzf8971.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      815 2023-05-09 09:19:35.000000 oscilloscope_scripts_xzf8971-1.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-09 09:29:54.181642 oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/
+-rw-rw-rw-   0        0        0     6999 2022-11-01 08:20:54.000000 oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/MakeWorkspaceForGain.C
+-rw-rw-rw-   0        0        0     3846 2022-11-01 08:20:54.000000 oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/OutputCharge.C
+-rw-rw-rw-   0        0        0     3192 2022-11-01 08:20:54.000000 oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/OutputCharge.h
+-rw-rw-rw-   0        0        0     3989 2022-11-01 08:20:54.000000 oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/Plot_waveform_from_root.py
+-rw-rw-rw-   0        0        0     5108 2022-11-01 08:20:54.000000 oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/Transform_csv_to_tree.py
+-rw-rw-rw-   0        0        0     7271 2022-11-01 08:20:54.000000 oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/UseWorkspaceForFit.C
+-rw-rw-rw-   0        0        0     1481 2022-11-01 08:20:54.000000 oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/analysis_waveform_data.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:29:54.190148 oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/naive_bayesian_classifier/
+-rw-rw-rw-   0        0        0     1599 2022-11-01 08:20:54.000000 oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/naive_bayesian_classifier/Event.py
+-rw-rw-rw-   0        0        0     8453 2022-11-01 08:20:54.000000 oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/naive_bayesian_classifier/naive_bayesian_classifier.py
+-rw-rw-rw-   0        0        0     8475 2022-11-01 08:20:54.000000 oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/naive_bayesian_classifier/naive_bayesian_classifier_CH2.py
+-rw-rw-rw-   0        0        0     6617 2022-11-01 08:20:54.000000 oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/single_channel_selector.C
+-rw-rw-rw-   0        0        0     3444 2022-11-01 08:20:54.000000 oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/single_channel_selector.h
+-rw-rw-rw-   0        0        0       42 2023-05-09 09:29:54.196194 oscilloscope_scripts_xzf8971-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      137 2022-11-01 12:09:12.000000 oscilloscope_scripts_xzf8971-1.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/PKG-INFO` & `oscilloscope_scripts_xzf8971-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-Metadata-Version: 2.1
-Name: oscilloscope_scripts_xzf8971
-Version: 1.1.0
-Summary: A package to control and read data from oscilloscope. Support TekTronix TBS2000B now.
-Author-email: Zifeng <zifeng.xu@foxmail.com>
-Project-URL: Homepage, https://github.com/xzf89718/oscilloscope_scripts
-Project-URL: Bug Tracker, https://github.com/xzf89718/oscilloscope_scripts/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Oscilloscope scripts
-
-This project contains interface to help you collect waveform data from osilloscope. TekTronix TBS2000B is supported now. If you prefer old version follow the course slides. Please check here: https://github.com/xzf89718/oscilloscope_scripts/tree/v7.2 and https://github.com/xzf89718/oscilloscope_scripts/releases/tag/v7.2
-
-## Getting started  
-### Setup python and NI-VISA  
-#### For Windows   
-Python 3.8:   
-https://www.python.org/downloads/release/python-383/   
-NI-VISA:   
-https://www.ni.com/zh-cn/support/downloads/drivers/download.ni-visa.html  
-#### For Linux/Mac OS 
-Please install libserial or other lib as backen  
-### Install   
-#### Install package with pip     
-```bash
-pip install oscilloscope-scripts-xzf8971  
-```
-#### Install package from github with pip
-```bash
-pip install git+https://github.com/xzf89718/oscilloscope_scripts
-```
-Get source code from github:  
-```bash
-git clone git@github.com:xzf89718/oscilloscope_scripts.git
-```   
-
-### The commands here aim to setup package for python  
-```bash
-pip install -U virtualenv  
-virtualenv -p 3.8 ~/pyvisa_3d8  
-~/pyvisa_3d8/Scripts/activate  
-```
-
-## How to use this package
-### Every Login
-```bash
-cd ~/pyvisa_3d8/Scripts     
-.\activate  
-```
-### Use Tektronix_TBS2000B_scripts for TBS2000B DAQ
-#### Batch mode  
-```bash
-python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode batch
-# On macOS or linux
-# python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode batch --backen pyvisa-py
-```
-#### Interactive mode (for debug)
-```bash
-python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode inter
-# On macOS or linux
-# python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode inter --backen pyvisa-py
-Enter your scope_name, also provide "default" and "auto" for quick setup  
-auto  
-```
-If the setup is correct, you will got a plot contain waveforms from CH1 and CH2  
-
-
-## Get some help
-```bash
-python  xxx.py --help  
-```
-Read the comments on the begin of each scripts  
-
-## Other materials
-In order to use the root scripts, you need ROOT and pyroot setup. Get Ubuntu20.04 VM with ROOT here: https://box.nju.edu.cn/d/045506afb0f347b78806/   
-How to build your own ROOT release on Ubuntu20.04: https://blog.csdn.net/weixin_44121665/article/details/102637844?spm=1001.2014.3001.5502  
-Data collected by me, without proper Impedance matching: https://box.nju.edu.cn/d/8c35131d91e846c4ada6/     
-## Contact me
-Author: Zifeng XU  
-Email:  
-zifeng.xu@foxmail.com  
-mg20220214@smail.nju.edu.cn  
-zifeng.xu@cern.ch  
+Metadata-Version: 2.1
+Name: oscilloscope_scripts_xzf8971
+Version: 1.2.0
+Summary: A package to control and read data from oscilloscope. Support TekTronix TBS2000B now.
+Author-email: Zifeng <zifeng.xu@foxmail.com>
+Project-URL: Homepage, https://github.com/xzf89718/oscilloscope_scripts
+Project-URL: Bug Tracker, https://github.com/xzf89718/oscilloscope_scripts/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Oscilloscope scripts
+
+This project contains interface to help you collect waveform data from osilloscope. TekTronix TBS2000B is supported now. If you prefer old version follow the course slides. Please check here: https://github.com/xzf89718/oscilloscope_scripts/tree/v7.2 and https://github.com/xzf89718/oscilloscope_scripts/releases/tag/v7.2
+
+## Getting started  
+### Setup python and NI-VISA  
+#### For Windows   
+Python 3.8:   
+https://www.python.org/downloads/release/python-383/   
+NI-VISA:   
+https://www.ni.com/zh-cn/support/downloads/drivers/download.ni-visa.html  
+#### For Linux/Mac OS 
+Please install libserial libusb pyserial pyusb and install pure python base pyvisa-py
+### Install   
+#### Install package with pip     
+```bash
+pip install oscilloscope-scripts-xzf8971  
+```
+#### Install package from github with pip
+```bash
+pip install git+https://github.com/xzf89718/oscilloscope_scripts
+```
+Get source code from github:  
+```bash
+git clone git@github.com:xzf89718/oscilloscope_scripts.git
+```   
+
+### The commands here aim to setup package for python  
+```bash
+pip install -U virtualenv  
+virtualenv -p 3.8 ~/pyvisa_3d8  
+~/pyvisa_3d8/Scripts/activate  
+```
+
+## How to use this package
+### Every Login
+```bash
+cd ~/pyvisa_3d8/Scripts     
+.\activate  
+```
+### Use Tektronix_TBS2000B_scripts for TBS2000B DAQ
+#### Batch mode  
+```bash
+python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode batch
+# On macOS or linux
+# python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode batch --backend pyvisa-py
+```
+#### Interactive mode (for debug)
+```bash
+python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode inter
+# On macOS or linux
+# python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode inter --backend pyvisa-py
+Enter your scope_name, also provide "default" and "auto" for quick setup  
+auto  
+```
+If the setup is correct, you will got a plot contain waveforms from CH1 and CH2  
+
+
+## Get some help
+```bash
+python  xxx.py --help  
+```
+Read the comments on the begin of each scripts  
+
+## Other materials
+In order to use the root scripts, you need ROOT and pyroot setup. Get Ubuntu20.04 VM with ROOT here: https://box.nju.edu.cn/d/045506afb0f347b78806/   
+How to build your own ROOT release on Ubuntu20.04: https://blog.csdn.net/weixin_44121665/article/details/102637844?spm=1001.2014.3001.5502  
+Data collected by me, without proper Impedance matching: https://box.nju.edu.cn/d/8c35131d91e846c4ada6/     
+## Contact me
+Author: Zifeng XU  
+Email:  
+zifeng.xu@foxmail.com  
+mg20220214@smail.nju.edu.cn  
+zifeng.xu@cern.ch
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/README.md` & `oscilloscope_scripts_xzf8971-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-# Oscilloscope scripts
-
-This project contains interface to help you collect waveform data from osilloscope. TekTronix TBS2000B is supported now. If you prefer old version follow the course slides. Please check here: https://github.com/xzf89718/oscilloscope_scripts/tree/v7.2 and https://github.com/xzf89718/oscilloscope_scripts/releases/tag/v7.2
-
-## Getting started  
-### Setup python and NI-VISA  
-#### For Windows   
-Python 3.8:   
-https://www.python.org/downloads/release/python-383/   
-NI-VISA:   
-https://www.ni.com/zh-cn/support/downloads/drivers/download.ni-visa.html  
-#### For Linux/Mac OS 
-Please install libserial or other lib as backen  
-### Install   
-#### Install package with pip     
-```bash
-pip install oscilloscope-scripts-xzf8971  
-```
-#### Install package from github with pip
-```bash
-pip install git+https://github.com/xzf89718/oscilloscope_scripts
-```
-Get source code from github:  
-```bash
-git clone git@github.com:xzf89718/oscilloscope_scripts.git
-```   
-
-### The commands here aim to setup package for python  
-```bash
-pip install -U virtualenv  
-virtualenv -p 3.8 ~/pyvisa_3d8  
-~/pyvisa_3d8/Scripts/activate  
-```
-
-## How to use this package
-### Every Login
-```bash
-cd ~/pyvisa_3d8/Scripts     
-.\activate  
-```
-### Use Tektronix_TBS2000B_scripts for TBS2000B DAQ
-#### Batch mode  
-```bash
-python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode batch
-# On macOS or linux
-# python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode batch --backen pyvisa-py
-```
-#### Interactive mode (for debug)
-```bash
-python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode inter
-# On macOS or linux
-# python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode inter --backen pyvisa-py
-Enter your scope_name, also provide "default" and "auto" for quick setup  
-auto  
-```
-If the setup is correct, you will got a plot contain waveforms from CH1 and CH2  
-
-
-## Get some help
-```bash
-python  xxx.py --help  
-```
-Read the comments on the begin of each scripts  
-
-## Other materials
-In order to use the root scripts, you need ROOT and pyroot setup. Get Ubuntu20.04 VM with ROOT here: https://box.nju.edu.cn/d/045506afb0f347b78806/   
-How to build your own ROOT release on Ubuntu20.04: https://blog.csdn.net/weixin_44121665/article/details/102637844?spm=1001.2014.3001.5502  
-Data collected by me, without proper Impedance matching: https://box.nju.edu.cn/d/8c35131d91e846c4ada6/     
-## Contact me
-Author: Zifeng XU  
-Email:  
-zifeng.xu@foxmail.com  
-mg20220214@smail.nju.edu.cn  
-zifeng.xu@cern.ch  
+# Oscilloscope scripts
+
+This project contains interface to help you collect waveform data from osilloscope. TekTronix TBS2000B is supported now. If you prefer old version follow the course slides. Please check here: https://github.com/xzf89718/oscilloscope_scripts/tree/v7.2 and https://github.com/xzf89718/oscilloscope_scripts/releases/tag/v7.2
+
+## Getting started  
+### Setup python and NI-VISA  
+#### For Windows   
+Python 3.8:   
+https://www.python.org/downloads/release/python-383/   
+NI-VISA:   
+https://www.ni.com/zh-cn/support/downloads/drivers/download.ni-visa.html  
+#### For Linux/Mac OS 
+Please install libserial libusb pyserial pyusb and install pure python base pyvisa-py
+### Install   
+#### Install package with pip     
+```bash
+pip install oscilloscope-scripts-xzf8971  
+```
+#### Install package from github with pip
+```bash
+pip install git+https://github.com/xzf89718/oscilloscope_scripts
+```
+Get source code from github:  
+```bash
+git clone git@github.com:xzf89718/oscilloscope_scripts.git
+```   
+
+### The commands here aim to setup package for python  
+```bash
+pip install -U virtualenv  
+virtualenv -p 3.8 ~/pyvisa_3d8  
+~/pyvisa_3d8/Scripts/activate  
+```
+
+## How to use this package
+### Every Login
+```bash
+cd ~/pyvisa_3d8/Scripts     
+.\activate  
+```
+### Use Tektronix_TBS2000B_scripts for TBS2000B DAQ
+#### Batch mode  
+```bash
+python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode batch
+# On macOS or linux
+# python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode batch --backend pyvisa-py
+```
+#### Interactive mode (for debug)
+```bash
+python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode inter
+# On macOS or linux
+# python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode inter --backend pyvisa-py
+Enter your scope_name, also provide "default" and "auto" for quick setup  
+auto  
+```
+If the setup is correct, you will got a plot contain waveforms from CH1 and CH2  
+
+
+## Get some help
+```bash
+python  xxx.py --help  
+```
+Read the comments on the begin of each scripts  
+
+## Other materials
+In order to use the root scripts, you need ROOT and pyroot setup. Get Ubuntu20.04 VM with ROOT here: https://box.nju.edu.cn/d/045506afb0f347b78806/   
+How to build your own ROOT release on Ubuntu20.04: https://blog.csdn.net/weixin_44121665/article/details/102637844?spm=1001.2014.3001.5502  
+Data collected by me, without proper Impedance matching: https://box.nju.edu.cn/d/8c35131d91e846c4ada6/     
+## Contact me
+Author: Zifeng XU  
+Email:  
+zifeng.xu@foxmail.com  
+mg20220214@smail.nju.edu.cn  
+zifeng.xu@cern.ch
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/Tektronix_TBS2000B_analysis/__main__.py` & `oscilloscope_scripts_xzf8971-1.2.0/Tektronix_TBS2000B_analysis/__main__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import argparse
-from Tektronix_TBS2000B_analysis import QuickAnalysis_Zifeng
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(
-        description="Standalone python data analysis skeleton wrapper")
-    parser.add_argument("input_filename", type=str,
-                        help="Input filename for csv files. filename prefix exactly")
-    parser.add_argument("--n_save_waveforms", type=int, default=10,
-                        help="N_Waveforms save in the output scripts")
-    parser.add_argument("--save_channels", type=str, default="CH1,CH2",
-                        help="Which channel should we save in the scripts? Example: CH1,CH2. Becarful, if you add wrong Channel here, often cause this program break down")
-    parser.add_argument("--input_dir", type=str, default="./",
-                        help="Where you save your data. Need full path.")
-    args = parser.parse_args()
-    print("This scripts is made by Zifeng Xu. Email: zifeng.xu@foxmail.com")
-    print("All parameters get from parser are:")
-    print(args)
-    INPUT_FILENAME = args.input_filename
-    N_SAVE_WAVEFORMS = args.n_save_waveforms
-    SAVE_CHANNELS = args.save_channels
-    INPUT_DIR = args.input_dir
-
-    # Start Analysis
-    quickanalysis = QuickAnalysis_Zifeng(
-        INPUT_FILENAME, N_SAVE_WAVEFORMS, SAVE_CHANNELS, INPUT_DIR)
-    quickanalysis.RunAnalysis()
-
-    print("Goodbye!")
+import argparse
+from Tektronix_TBS2000B_analysis import QuickAnalysis_Zifeng
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(
+        description="Standalone python data analysis skeleton wrapper")
+    parser.add_argument("input_filename", type=str,
+                        help="Input filename for csv files. filename prefix exactly")
+    parser.add_argument("--n_save_waveforms", type=int, default=10,
+                        help="N_Waveforms save in the output scripts")
+    parser.add_argument("--save_channels", type=str, default="CH1,CH2",
+                        help="Which channel should we save in the scripts? Example: CH1,CH2. Becarful, if you add wrong Channel here, often cause this program break down")
+    parser.add_argument("--input_dir", type=str, default="./",
+                        help="Where you save your data. Need full path.")
+    args = parser.parse_args()
+    print("This scripts is made by Zifeng Xu. Email: zifeng.xu@foxmail.com")
+    print("All parameters get from parser are:")
+    print(args)
+    INPUT_FILENAME = args.input_filename
+    N_SAVE_WAVEFORMS = args.n_save_waveforms
+    SAVE_CHANNELS = args.save_channels
+    INPUT_DIR = args.input_dir
+
+    # Start Analysis
+    quickanalysis = QuickAnalysis_Zifeng(
+        INPUT_FILENAME, N_SAVE_WAVEFORMS, SAVE_CHANNELS, INPUT_DIR)
+    quickanalysis.RunAnalysis()
+
+    print("Goodbye!")
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/Tektronix_TBS2000B_control/oscilloscope_control.py` & `oscilloscope_scripts_xzf8971-1.2.0/Tektronix_TBS2000B_control/oscilloscope_control.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-#!/usr/bin/env python
-# Author: Zifeng Xu, Changge Zi.
-# Email: zifeng.xu@cern.ch
-# Note:1, How to detect muon decay events in our lab?
-#      2, Only sample the channel you already setup
-import pyvisa
-import time
-import sys
-
-import numpy as np
-import matplotlib.pyplot as plt
-
-
-class Oscilloscope():
-
-    """
-    This class include method of initialize and setup the oscilloscope via usb.
-    And some methods to measure the waveform and get the data.
-
-    """
-
-    def __init__(self, resource_name='USB0::0x0699::0x03C7::C011248::INSTR'):
-        print("Osilloscope::INFO instrumente name: {0}".format(resource_name))
-        # enable libvisa support. Only available on Mac and Windows
-        self.resource_manager = pyvisa.ResourceManager()
-        # enable full python pyvisa
-        # self.resource_manager=pyvisa.ResourceManager("@py")
-        self.inst = self.resource_manager.open_resource(
-            resource_name=resource_name)
-        self.inst.timeout = 10000  # ms
-        self.inst.encoding = 'latin_1'
-        self.inst.read_termination = '\n'
-        self.inst.write_termination = None
-        self._channel = 'DEFAULT'
-        self.inst.write('*cls')  # clear ESR
-        self.inst.write('header OFF')  # disable attribute echo in replies
-        print(self.inst.query('*idn?'))
-        # autoset
-        # self.Autoset()
-
-    def Sampling(self, sammple_channels="CH1", M=2000):  # M is the number of sampling points
-        list_channels = sammple_channels.split(',')
-        # Prepare sampling
-        # default setup
-        # self.inst.write('*rst')
-        r = self.inst.query('*opc?')  # sync
-
-        # acquisition
-        self.inst.write('acquire:state OFF')  # stop
-        self.inst.write('acquire:stopafter SEQUENCE;state ON')  # single
-        r = self.inst.query('*opc?')
-
-        # curve configuration
-        self.inst.write('data:encdg SRIBINARY')  # signed integer
-        acq_record = int(M)  # self.inst.query('horizontal:recordlength?')
-        # 2021/06/14 Zifeng edit, This is a very importrant bug! You must specified the start point of the query!
-        # For TBS2000B, 1 to 2500 means a full waveform!
-        # If you dont specified, a random start will applied, what is not you want exactly.
-        self.inst.write('data:start 1')
-        self.inst.write('data:stop {0}'.format(acq_record))
-        self.inst.write('wfmoutpre:byt_nr 1')  # 1 byte per sample
-
-        dic_waveforms = {}
-        dic_scaledtime = {}
-        for channel in list_channels:
-            self.SetChannel(channel)
-            self.inst.write('data:source {0}'.format(self._channel))
-            # data query
-            # send message in binary form
-            bin_wave = self.inst.query_binary_values(
-                'curve?', datatype='b', container=np.array)
-            # retrieve scaling factors
-            wfm_record = int(self.inst.query('wfmoutpre:nr_pt?'))
-            pre_trig_record = int(self.inst.query('wfmoutpre:pt_off?'))
-            t_scale = float(self.inst.query('wfmoutpre:xincr?'))
-            # sub-sample trigger correction
-            t_sub = float(self.inst.query('wfmoutpre:xzero?'))
-            v_scale = float(self.inst.query(
-                'wfmoutpre:ymult?'))  # volts / level
-            # reference voltage
-            v_off = float(self.inst.query('wfmoutpre:yzero?'))
-            # reference position (level)
-            v_pos = float(self.inst.query('wfmoutpre:yoff?'))
-
-            # error checking
-            r = int(self.inst.query('*esr?'))
-            r = self.inst.query('allev?').strip()
-
-            # create scaled vectors
-            # horizontal (time)
-            total_time = t_scale * wfm_record
-            t_start = (-pre_trig_record * t_scale) + t_sub
-            t_stop = t_start + total_time
-            scaled_time = np.linspace(
-                t_start, t_stop, num=wfm_record, endpoint=False)
-
-            # vertical (voltage)
-            # data type conversion
-            unscaled_wave = np.array(bin_wave, dtype='double')
-            scaled_wave = (unscaled_wave - v_pos) * v_scale + v_off
-            dic_scaledtime[channel] = scaled_time
-            dic_waveforms[channel] = scaled_wave
-        # return scaled_time, scaled_wave
-        return dic_scaledtime, dic_waveforms
-
-    def MeasureFreq(self, measure_channels="CH1"):  # MEASUre Frequency
-        dic_freq = {}
-        for _channel in measure_channels.split(','):
-            self.SetChannel(_channel)
-            self.inst.write(
-                ':MEASUrement:IMMed:SOUrce1 {0}'.format(self._channel))
-            self.inst.write(':MEASUrement:IMMed:TYPe FREQuency')
-            dic_freq[_channel] = self.inst.query(':MEASUrement:IMMed:VALue?')
-        return dic_freq
-
-    def MeasureAmpl(self, measure_channels="CH1"):  # MEASUre Amplitude
-        dic_ampl = {}
-        for _channel in measure_channels.split(','):
-            self.SetChannel(_channel)
-            self.inst.write(
-                ':MEASUrement:IMMed:SOUrce1 {0}'.format(self._channel))
-            self.inst.write(':MEASUrement:IMMed:TYPe AMPlitude')
-            dic_ampl[_channel] = self.inst.query(':MEASUrement:IMMed:VALue?')
-        return dic_ampl
-
-    def MeasureHigh(self, measure_channels="CH1"):  # MEASUre Low
-        dic_high = {}
-        for _channel in measure_channels.split(','):
-            self.SetChannel(_channel)
-            self.inst.write(
-                ':MEASUrement:IMMed:SOUrce1 {0}'.format(self._channel))
-            self.inst.write(':MEASUrement:IMMed:TYPe HIGH')
-            dic_high[_channel] = self.inst.query(':MEASUrement:IMMed:VALue?')
-        return dic_high
-
-    def MeasureLow(self, measure_channels="CH1"):  # MEASUre Low
-        dic_low = {}
-        for _channel in measure_channels:
-            self.SetChannel(_channel)
-            self.inst.write(
-                ':MEASUrement:IMMed:SOUrce1 {0}}'.format(self._channel))
-            self.inst.write(':MEASUrement:IMMed:TYPe LOW')
-            dic_low[_channel] = self.inst.query(':MEASUrement:IMMed:VALue?')
-        return dic_low
-
-    def SetChannel(self, channel):
-        """
-        Set channel for Measure and Sampling
-        example, "CH1" "CH2"
-        """
-
-        # Check if channel is legal
-        if(channel == 'DEFAULT'):
-            print(
-                "Oscilloscop::WARNING the channel is set to DEFAULT now, no measure of data-save is proceeded")
-        if(channel == 'CH1'):
-            self._channel = channel
-            print("Set CH1")
-        elif(channel == 'CH2'):
-            self._channel = channel
-            print("Set CH2")
-        elif(channel == 'CH3'):
-            self._channel = channel
-            print("Set CH3")
-        elif(channel == 'CH4'):
-            self._channel = channel
-            print("Set CH4")
-        else:
-            # self._channel = "DEFAULT"
-            # print("The select channel should be one of CH1, CH2, CH3, CH4\nSet DEFUALT")
-            ex = Exception("Oscilloscope::ERROR Sampling channl not exist. Example:CH1,CH2,CH3,CH4")
-            raise ex
-
-    def Autoset(self):
-        self.inst.write('autoset EXECUTE')
-
-    # disconnect
-    def Close(self):
-        self.inst.close()
-        self.resource_manager.close()
-
-
-def WriteToCsv(output_filename, array_time, array_voltage, sep=','):
-    # Check the len of time and voltage
-    length_of_time = len(array_time)
-    length_of_voltage = len(array_voltage)
-    if(not(length_of_time == length_of_voltage)):
-        ex = Exception("The size of time and voltage is not equal")
-        raise ex
-    # Write header
-    try:
-        with open(output_filename, 'w') as file_object:
-            file_object.write("scaled_time{0}scaled_voltage\n".format(sep))
-            i = 0
-            while (i < length_of_voltage):
-                file_object.write("{0}{1}{2}{3}".format(
-                    str(array_time[i]), sep, str(array_voltage[i]),  "\n"))
-                i = i + 1
-    except FileNotFoundError:
-        print("Oscilloscope WriteToCsv ERROR: {0} not exist. Create this dir first. like $mkdir {0} or just create this in Windows GUI. This scripts has been terminated.".format(output_filename.split("/")[0]))
+#!/usr/bin/env python
+# Author: Zifeng Xu, Changge Zi.
+# Email: zifeng.xu@cern.ch
+# Note:1, How to detect muon decay events in our lab?
+#      2, Only sample the channel you already setup
+import pyvisa
+import time
+import sys
+
+import numpy as np
+import matplotlib.pyplot as plt
+
+
+class Oscilloscope():
+
+    """
+    This class include method of initialize and setup the oscilloscope via usb.
+    And some methods to measure the waveform and get the data.
+
+    """
+
+    def __init__(self, resource_name='USB0::0x0699::0x03C7::C011248::INSTR'):
+        print("Osilloscope::INFO instrumente name: {0}".format(resource_name))
+        # enable libvisa support. Only available on Mac and Windows
+        self.resource_manager = pyvisa.ResourceManager()
+        # enable full python pyvisa
+        # self.resource_manager=pyvisa.ResourceManager("@py")
+        self.inst = self.resource_manager.open_resource(
+            resource_name=resource_name)
+        self.inst.timeout = 10000  # ms
+        self.inst.encoding = 'latin_1'
+        self.inst.read_termination = '\n'
+        self.inst.write_termination = None
+        self._channel = 'DEFAULT'
+        self.inst.write('*cls')  # clear ESR
+        self.inst.write('header OFF')  # disable attribute echo in replies
+        print(self.inst.query('*idn?'))
+        # autoset
+        # self.Autoset()
+
+    def Sampling(self, sammple_channels="CH1", M=2000):  # M is the number of sampling points
+        list_channels = sammple_channels.split(',')
+        # Prepare sampling
+        # default setup
+        # self.inst.write('*rst')
+        r = self.inst.query('*opc?')  # sync
+
+        # acquisition
+        self.inst.write('acquire:state OFF')  # stop
+        self.inst.write('acquire:stopafter SEQUENCE;state ON')  # single
+        r = self.inst.query('*opc?')
+
+        # curve configuration
+        self.inst.write('data:encdg SRIBINARY')  # signed integer
+        acq_record = int(M)  # self.inst.query('horizontal:recordlength?')
+        # 2021/06/14 Zifeng edit, This is a very importrant bug! You must specified the start point of the query!
+        # For TBS2000B, 1 to 2500 means a full waveform!
+        # If you dont specified, a random start will applied, what is not you want exactly.
+        self.inst.write('data:start 1')
+        self.inst.write('data:stop {0}'.format(acq_record))
+        self.inst.write('wfmoutpre:byt_nr 1')  # 1 byte per sample
+
+        dic_waveforms = {}
+        dic_scaledtime = {}
+        for channel in list_channels:
+            self.SetChannel(channel)
+            self.inst.write('data:source {0}'.format(self._channel))
+            # data query
+            # send message in binary form
+            bin_wave = self.inst.query_binary_values(
+                'curve?', datatype='b', container=np.array)
+            # retrieve scaling factors
+            wfm_record = int(self.inst.query('wfmoutpre:nr_pt?'))
+            pre_trig_record = int(self.inst.query('wfmoutpre:pt_off?'))
+            t_scale = float(self.inst.query('wfmoutpre:xincr?'))
+            # sub-sample trigger correction
+            t_sub = float(self.inst.query('wfmoutpre:xzero?'))
+            v_scale = float(self.inst.query(
+                'wfmoutpre:ymult?'))  # volts / level
+            # reference voltage
+            v_off = float(self.inst.query('wfmoutpre:yzero?'))
+            # reference position (level)
+            v_pos = float(self.inst.query('wfmoutpre:yoff?'))
+
+            # error checking
+            r = int(self.inst.query('*esr?'))
+            r = self.inst.query('allev?').strip()
+
+            # create scaled vectors
+            # horizontal (time)
+            total_time = t_scale * wfm_record
+            t_start = (-pre_trig_record * t_scale) + t_sub
+            t_stop = t_start + total_time
+            scaled_time = np.linspace(
+                t_start, t_stop, num=wfm_record, endpoint=False)
+
+            # vertical (voltage)
+            # data type conversion
+            unscaled_wave = np.array(bin_wave, dtype='double')
+            scaled_wave = (unscaled_wave - v_pos) * v_scale + v_off
+            dic_scaledtime[channel] = scaled_time
+            dic_waveforms[channel] = scaled_wave
+        # return scaled_time, scaled_wave
+        return dic_scaledtime, dic_waveforms
+
+    def MeasureFreq(self, measure_channels="CH1"):  # MEASUre Frequency
+        dic_freq = {}
+        for _channel in measure_channels.split(','):
+            self.SetChannel(_channel)
+            self.inst.write(
+                ':MEASUrement:IMMed:SOUrce1 {0}'.format(self._channel))
+            self.inst.write(':MEASUrement:IMMed:TYPe FREQuency')
+            dic_freq[_channel] = self.inst.query(':MEASUrement:IMMed:VALue?')
+        return dic_freq
+
+    def MeasureAmpl(self, measure_channels="CH1"):  # MEASUre Amplitude
+        dic_ampl = {}
+        for _channel in measure_channels.split(','):
+            self.SetChannel(_channel)
+            self.inst.write(
+                ':MEASUrement:IMMed:SOUrce1 {0}'.format(self._channel))
+            self.inst.write(':MEASUrement:IMMed:TYPe AMPlitude')
+            dic_ampl[_channel] = self.inst.query(':MEASUrement:IMMed:VALue?')
+        return dic_ampl
+
+    def MeasureHigh(self, measure_channels="CH1"):  # MEASUre Low
+        dic_high = {}
+        for _channel in measure_channels.split(','):
+            self.SetChannel(_channel)
+            self.inst.write(
+                ':MEASUrement:IMMed:SOUrce1 {0}'.format(self._channel))
+            self.inst.write(':MEASUrement:IMMed:TYPe HIGH')
+            dic_high[_channel] = self.inst.query(':MEASUrement:IMMed:VALue?')
+        return dic_high
+
+    def MeasureLow(self, measure_channels="CH1"):  # MEASUre Low
+        dic_low = {}
+        for _channel in measure_channels:
+            self.SetChannel(_channel)
+            self.inst.write(
+                ':MEASUrement:IMMed:SOUrce1 {0}}'.format(self._channel))
+            self.inst.write(':MEASUrement:IMMed:TYPe LOW')
+            dic_low[_channel] = self.inst.query(':MEASUrement:IMMed:VALue?')
+        return dic_low
+
+    def SetChannel(self, channel):
+        """
+        Set channel for Measure and Sampling
+        example, "CH1" "CH2"
+        """
+
+        # Check if channel is legal
+        if(channel == 'DEFAULT'):
+            print(
+                "Oscilloscop::WARNING the channel is set to DEFAULT now, no measure of data-save is proceeded")
+        if(channel == 'CH1'):
+            self._channel = channel
+            print("Set CH1")
+        elif(channel == 'CH2'):
+            self._channel = channel
+            print("Set CH2")
+        elif(channel == 'CH3'):
+            self._channel = channel
+            print("Set CH3")
+        elif(channel == 'CH4'):
+            self._channel = channel
+            print("Set CH4")
+        else:
+            # self._channel = "DEFAULT"
+            # print("The select channel should be one of CH1, CH2, CH3, CH4\nSet DEFUALT")
+            ex = Exception("Oscilloscope::ERROR Sampling channl not exist. Example:CH1,CH2,CH3,CH4")
+            raise ex
+
+    def Autoset(self):
+        self.inst.write('autoset EXECUTE')
+
+    # disconnect
+    def Close(self):
+        self.inst.close()
+        self.resource_manager.close()
+
+
+def WriteToCsv(output_filename, array_time, array_voltage, sep=','):
+    # Check the len of time and voltage
+    length_of_time = len(array_time)
+    length_of_voltage = len(array_voltage)
+    if(not(length_of_time == length_of_voltage)):
+        ex = Exception("The size of time and voltage is not equal")
+        raise ex
+    # Write header
+    try:
+        with open(output_filename, 'w') as file_object:
+            file_object.write("scaled_time{0}scaled_voltage\n".format(sep))
+            i = 0
+            while (i < length_of_voltage):
+                file_object.write("{0}{1}{2}{3}".format(
+                    str(array_time[i]), sep, str(array_voltage[i]),  "\n"))
+                i = i + 1
+    except FileNotFoundError:
+        print("Oscilloscope WriteToCsv ERROR: {0} not exist. Create this dir first. like $mkdir {0} or just create this in Windows GUI. This scripts has been terminated.".format(output_filename.split("/")[0]))
         sys.exit()
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/Tektronix_TBS2000B_scripts/__main__.py` & `oscilloscope_scripts_xzf8971-1.2.0/Tektronix_TBS2000B_scripts/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-#!/usr/bin/env python
-
-# Author: Zifeng XU
-# Email: zifeng.xu@cern.ch
-# Usage: provide interafate to save waveform data from Tek TBS2000B oscilloscope
-# Make sure you have output_dir, make sure the save_channels is enable in oscilloscope
-# Example: python RunMeasurement.py this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir
-# Use auto scope_name, the first name
-# Example: python RunMeasurement.py this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto
-# Example: python RunMeasurement.py this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name USB0::0x0699::0x03C7::C011248::INSTR
-# Output filename for example will be this_is_an_example-CH1.csv in output_dir
-import argparse
-import time
-
-import pyvisa
-
-from Tektronix_TBS2000B_scripts.helper_function import batchDataTaking, interactiveDataTaking
-
-# Batch mode
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(
-        description="Save multiple waveform into csv files. You can even make measure. Author: Zifeng XU, email: zifeng.xu@cern.ch")
-    parser.add_argument("output_filename", type=str,
-                        help="Output file name for waveforms")
-    parser.add_argument("--n_save_waveforms", type=int, default=10,
-                        help="N_Waveforms save in the output scripts")
-    parser.add_argument("--save_channels", type=str, default="CH1",
-                        help="Which channel should we save in the scripts? Example: CH1,CH2. Becarful, if you add wrong Channel here, often cause this program break down")
-    parser.add_argument("--output_dir", type=str, default="./",
-                        help="Which directory to save waveform data, please make sure you have this directory in you USB. For examle: /usb0/waveform_data")
-    parser.add_argument("--scope_name", type=str, default="default",
-                        help="scope_name, every oscilloscope has its own name, which is needed when instantiate the Scope, default, auto, and specify the name you like is supported")
-    parser.add_argument("--mode", type=str, choices=["batch", "inter"], required=True, help="Supported options: inter batch")
-    parser.add_argument("--backen", type=str, default="NIVISA", choices=["NIVISA", "pyvisa-py"], help="Supported options: NIVISA, pyvisa-py")
-    args = parser.parse_args()
-    print("All parameters get from commandline are:")
-    print(args)
-
-    output_filename = args.output_filename
-    n_save_waveforms = args.n_save_waveforms
-    save_channels = args.save_channels
-    output_dir = args.output_dir
-    scope_name = args.scope_name
-    mode = args.mode
-    backen = args.backen
-
-    print("Here are instruments' name you have:")
-    if (backen == "NIVISA"):
-        resource_manager = pyvisa.ResourceManager()
-    elif (backen == "pyvisa-py"):
-        resource_manager = pyvisa.ResourceManager("@py")
-    inst_name = resource_manager.list_resources()
-    print("{0}".format(inst_name))
-    time.sleep(3)
-    if (mode == "batch"):
-        batchDataTaking(output_filename, n_save_waveforms,
-                        save_channels, output_dir, scope_name, inst_name)
-    elif (mode == "inter"):
-        interactiveDataTaking(inst_name, save_channels)
+#!/usr/bin/env python
+
+# Author: Zifeng XU
+# Email: zifeng.xu@cern.ch
+# Usage: provide interafate to save waveform data from Tek TBS2000B oscilloscope
+# Make sure you have output_dir, make sure the save_channels is enable in oscilloscope
+# Example: python RunMeasurement.py this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir
+# Use auto scope_name, the first name
+# Example: python RunMeasurement.py this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto
+# Example: python RunMeasurement.py this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name USB0::0x0699::0x03C7::C011248::INSTR
+# Output filename for example will be this_is_an_example-CH1.csv in output_dir
+import argparse
+import time
+
+import pyvisa
+
+from Tektronix_TBS2000B_scripts.helper_function import batchDataTaking, interactiveDataTaking
+
+# Batch mode
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(
+        description="Save multiple waveform into csv files. You can even make measure. Author: Zifeng XU, email: zifeng.xu@cern.ch")
+    parser.add_argument("output_filename", type=str,
+                        help="Output file name for waveforms")
+    parser.add_argument("--n_save_waveforms", type=int, default=10,
+                        help="N_Waveforms save in the output scripts")
+    parser.add_argument("--save_channels", type=str, default="CH1",
+                        help="Which channel should we save in the scripts? Example: CH1,CH2. Becarful, if you add wrong Channel here, often cause this program break down")
+    parser.add_argument("--output_dir", type=str, default="./",
+                        help="Which directory to save waveform data, please make sure you have this directory in you USB. For examle: /usb0/waveform_data")
+    parser.add_argument("--scope_name", type=str, default="default",
+                        help="scope_name, every oscilloscope has its own name, which is needed when instantiate the Scope, default, auto, and specify the name you like is supported")
+    parser.add_argument("--mode", type=str, choices=["batch", "inter"], required=True, help="Supported options: inter batch")
+    parser.add_argument("--backend", type=str, default="NIVISA", choices=["NIVISA", "pyvisa-py"], help="Supported options: NIVISA, pyvisa-py. For Microsoft's Windows, use the NIVISA. For MacOS or Linux, please use pyvisa-py(acompanied with libusb libserial and there Python interfaces).")
+    args = parser.parse_args()
+    print("All parameters get from commandline are:")
+    print(args)
+
+    output_filename = args.output_filename
+    n_save_waveforms = args.n_save_waveforms
+    save_channels = args.save_channels
+    output_dir = args.output_dir
+    scope_name = args.scope_name
+    mode = args.mode
+    backend = args.backend
+
+    print("Here are instruments' name you have:")
+    if (backend == "NIVISA"):
+        resource_manager = pyvisa.ResourceManager()
+    elif (backend == "pyvisa-py"):
+        resource_manager = pyvisa.ResourceManager("@py")
+    inst_name = resource_manager.list_resources()
+    print("{0}".format(inst_name))
+    time.sleep(3)
+    if (mode == "batch"):
+        batchDataTaking(output_filename, n_save_waveforms,
+                        save_channels, output_dir, scope_name, inst_name)
+    elif (mode == "inter"):
+        interactiveDataTaking(inst_name, save_channels)
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/Tektronix_TBS2000B_scripts/helper_function.py` & `oscilloscope_scripts_xzf8971-1.2.0/Tektronix_TBS2000B_scripts/helper_function.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-from Tektronix_TBS2000B_control.oscilloscope_control import Oscilloscope, WriteToCsv
-import time
-import os
-import numpy as np
-import matplotlib.pyplot as plt
-import pyvisa
-
-
-def Software_trigger(dic_scaled_time, dic_scaled_voltage):
-    """
-    User software trigger
-    """
-
-    # Pass tirgger
-    return True
-
-
-def sampleOnce(inst, save_channels='CH1,CH2'):
-    try:
-        wavetime, waveform = inst.Sampling(save_channels)
-        wavetime, waveform = inst.Sampling(save_channels)
-    except pyvisa.VisaIOError as error:
-        print(
-            "The oscilloscope is not triggered more than 10s. VI_ERROR_TMO\n\033[33mA kindly remind: Check TRIGGER on oscilloscope, make sure you got a signal on the screen when press Single\033[0m")
-        print("The information below is prepared for experts:\n\033[31mVisaIOError\033[0m, meassage:{0}".format(
-            error.args))
-        return False
-    for channel in save_channels.split(","):
-        plt.plot(wavetime[channel], waveform[channel])
-        print(len(waveform[channel]))
-    plt.xlabel('time')
-    plt.ylabel('voltage')
-    plt.savefig('sample_once_{channels}'.format(
-        channels=save_channels.replace(',', '_')))
-    plt.show()
-
-
-def interactiveDataTaking(inst_name, save_channels="CH1,CH2"):
-    print("Interactive mode")
-    print("Use command RunMeasurement.SampleOnce(RunMeasurement.Scope,\"CH1,CH2,CH3\")")
-    try:
-        # Interactive mode
-        scope_name = input(
-            "Enter your scope_name, also provide \"default\" and \"auto\" for quick setup\n")
-        if (scope_name == "default"):
-            Scope = Oscilloscope()
-        elif (scope_name == "auto"):
-            Scope = Oscilloscope(inst_name[0])
-        else:
-            Scope = Oscilloscope(scope_name)
-        sampleOnce(inst=Scope, save_channels=save_channels)
-    except pyvisa.VisaIOError:
-        print("Fail to create a Osilloscope object.\n1, Check connection between oscilloscope and computer\n2, Check the name of Scope and the inst_name")
-
-
-def batchDataTaking(output_filename,
-                    n_save_waveforms,
-                    save_channels,
-                    output_dir,
-                    scope_name, inst_name):
-    print("****************************************************************************************")
-    print("****************************************************************************************")
-    print("****************************************************************************************")
-    print("*                Please check the channel option here very carefully                   *")
-    print("****************************************************************************************")
-    print("****************************************************************************************")
-    print("****************************************************************************************")
-    begin_time = time.time()
-    # Initialize Oscilloscope
-    if(scope_name == "default"):
-        Scope = Oscilloscope()
-    elif(scope_name == "auto"):
-        Scope = Oscilloscope(inst_name[0])
-    else:
-        Scope = Oscilloscope(scope_name)
-    # Loop from 0 to n_save_waveforms, save all wave form
-    t_list = []
-    for i_waveform in range(0, n_save_waveforms):
-        t1 = time.time()
-        # Autoset, you wont want this in our measurement!
-        # Scope.Autoset()
-        wavetime, waveform = Scope.Sampling(save_channels)
-        while (not Software_trigger(wavetime, waveform)):
-            wavetime, waveform = Scope.Sampling(save_channels)
-        for _channel in save_channels.split(","):
-            WriteToCsv("{3}/{0}-{1}-{2}.csv".format(output_filename, _channel,
-                       str(i_waveform), output_dir), wavetime[_channel], waveform[_channel])
-        t2 = time.time()
-
-        t_list.append(t2-t1)
-        t_mean = np.mean(t_list)
-
-        percentage_of_job = float(i_waveform) / float(n_save_waveforms)
-        # clear screen
-        os.system("cls")
-        print(
-            "**************{0:.1f}% job is processed.***************".format(percentage_of_job*100))
-        time_left = t_mean*(n_save_waveforms-i_waveform)  # (s)
-        print(time.strftime("%Mmin %Ss", time.gmtime(time_left)), "left")
-
-    Scope.Close()
-    os.system("cls")
-    end_time = time.time()
-    event_rate = float(n_save_waveforms) / (end_time - begin_time)
-
-    print("****************************")
-    print("****************************")
-    print("**  Event rate: {0:.2f}Hz **".format(event_rate))
-    print("****************************")
-    print("****************************")
+from Tektronix_TBS2000B_control.oscilloscope_control import Oscilloscope, WriteToCsv
+import time
+import os
+import numpy as np
+import matplotlib.pyplot as plt
+import pyvisa
+
+
+def Software_trigger(dic_scaled_time, dic_scaled_voltage):
+    """
+    User software trigger
+    """
+
+    # Pass tirgger
+    return True
+
+
+def sampleOnce(inst, save_channels='CH1,CH2'):
+    try:
+        wavetime, waveform = inst.Sampling(save_channels)
+        wavetime, waveform = inst.Sampling(save_channels)
+    except pyvisa.VisaIOError as error:
+        print(
+            "The oscilloscope is not triggered more than 10s. VI_ERROR_TMO\n\033[33mA kindly remind: Check TRIGGER on oscilloscope, make sure you got a signal on the screen when press Single\033[0m")
+        print("The information below is prepared for experts:\n\033[31mVisaIOError\033[0m, meassage:{0}".format(
+            error.args))
+        return False
+    for channel in save_channels.split(","):
+        plt.plot(wavetime[channel], waveform[channel])
+        print(len(waveform[channel]))
+    plt.xlabel('time')
+    plt.ylabel('voltage')
+    plt.savefig('sample_once_{channels}'.format(
+        channels=save_channels.replace(',', '_')))
+    plt.show()
+
+
+def interactiveDataTaking(inst_name, save_channels="CH1,CH2"):
+    print("Interactive mode")
+    print("Use command RunMeasurement.SampleOnce(RunMeasurement.Scope,\"CH1,CH2,CH3\")")
+    try:
+        # Interactive mode
+        scope_name = input(
+            "Enter your scope_name, also provide \"default\" and \"auto\" for quick setup\n")
+        if (scope_name == "default"):
+            Scope = Oscilloscope()
+        elif (scope_name == "auto"):
+            Scope = Oscilloscope(inst_name[0])
+        else:
+            Scope = Oscilloscope(scope_name)
+        sampleOnce(inst=Scope, save_channels=save_channels)
+    except pyvisa.VisaIOError:
+        print("Fail to create a Osilloscope object.\n1, Check connection between oscilloscope and computer\n2, Check the name of Scope and the inst_name")
+
+
+def batchDataTaking(output_filename,
+                    n_save_waveforms,
+                    save_channels,
+                    output_dir,
+                    scope_name, inst_name):
+    print("****************************************************************************************")
+    print("****************************************************************************************")
+    print("****************************************************************************************")
+    print("*                Please check the channel option here very carefully                   *")
+    print("****************************************************************************************")
+    print("****************************************************************************************")
+    print("****************************************************************************************")
+    begin_time = time.time()
+    # Initialize Oscilloscope
+    if(scope_name == "default"):
+        Scope = Oscilloscope()
+    elif(scope_name == "auto"):
+        Scope = Oscilloscope(inst_name[0])
+    else:
+        Scope = Oscilloscope(scope_name)
+    # Loop from 0 to n_save_waveforms, save all wave form
+    t_list = []
+    for i_waveform in range(0, n_save_waveforms):
+        t1 = time.time()
+        # Autoset, you wont want this in our measurement!
+        # Scope.Autoset()
+        wavetime, waveform = Scope.Sampling(save_channels)
+        while (not Software_trigger(wavetime, waveform)):
+            wavetime, waveform = Scope.Sampling(save_channels)
+        for _channel in save_channels.split(","):
+            WriteToCsv("{3}/{0}-{1}-{2}.csv".format(output_filename, _channel,
+                       str(i_waveform), output_dir), wavetime[_channel], waveform[_channel])
+        t2 = time.time()
+
+        t_list.append(t2-t1)
+        t_mean = np.mean(t_list)
+
+        percentage_of_job = float(i_waveform) / float(n_save_waveforms)
+        # clear screen
+        os.system("cls")
+        print(
+            "**************{0:.1f}% job is processed.***************".format(percentage_of_job*100))
+        time_left = t_mean*(n_save_waveforms-i_waveform)  # (s)
+        print(time.strftime("%Mmin %Ss", time.gmtime(time_left)), "left")
+
+    Scope.Close()
+    os.system("cls")
+    end_time = time.time()
+    event_rate = float(n_save_waveforms) / (end_time - begin_time)
+
+    print("****************************")
+    print("****************************")
+    print("**  Event rate: {0:.2f}Hz **".format(event_rate))
+    print("****************************")
+    print("****************************")
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/oscilloscope_scripts_xzf8971.egg-info/PKG-INFO` & `oscilloscope_scripts_xzf8971-1.2.0/oscilloscope_scripts_xzf8971.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-Metadata-Version: 2.1
-Name: oscilloscope-scripts-xzf8971
-Version: 1.1.0
-Summary: A package to control and read data from oscilloscope. Support TekTronix TBS2000B now.
-Author-email: Zifeng <zifeng.xu@foxmail.com>
-Project-URL: Homepage, https://github.com/xzf89718/oscilloscope_scripts
-Project-URL: Bug Tracker, https://github.com/xzf89718/oscilloscope_scripts/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Oscilloscope scripts
-
-This project contains interface to help you collect waveform data from osilloscope. TekTronix TBS2000B is supported now. If you prefer old version follow the course slides. Please check here: https://github.com/xzf89718/oscilloscope_scripts/tree/v7.2 and https://github.com/xzf89718/oscilloscope_scripts/releases/tag/v7.2
-
-## Getting started  
-### Setup python and NI-VISA  
-#### For Windows   
-Python 3.8:   
-https://www.python.org/downloads/release/python-383/   
-NI-VISA:   
-https://www.ni.com/zh-cn/support/downloads/drivers/download.ni-visa.html  
-#### For Linux/Mac OS 
-Please install libserial or other lib as backen  
-### Install   
-#### Install package with pip     
-```bash
-pip install oscilloscope-scripts-xzf8971  
-```
-#### Install package from github with pip
-```bash
-pip install git+https://github.com/xzf89718/oscilloscope_scripts
-```
-Get source code from github:  
-```bash
-git clone git@github.com:xzf89718/oscilloscope_scripts.git
-```   
-
-### The commands here aim to setup package for python  
-```bash
-pip install -U virtualenv  
-virtualenv -p 3.8 ~/pyvisa_3d8  
-~/pyvisa_3d8/Scripts/activate  
-```
-
-## How to use this package
-### Every Login
-```bash
-cd ~/pyvisa_3d8/Scripts     
-.\activate  
-```
-### Use Tektronix_TBS2000B_scripts for TBS2000B DAQ
-#### Batch mode  
-```bash
-python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode batch
-# On macOS or linux
-# python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode batch --backen pyvisa-py
-```
-#### Interactive mode (for debug)
-```bash
-python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode inter
-# On macOS or linux
-# python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode inter --backen pyvisa-py
-Enter your scope_name, also provide "default" and "auto" for quick setup  
-auto  
-```
-If the setup is correct, you will got a plot contain waveforms from CH1 and CH2  
-
-
-## Get some help
-```bash
-python  xxx.py --help  
-```
-Read the comments on the begin of each scripts  
-
-## Other materials
-In order to use the root scripts, you need ROOT and pyroot setup. Get Ubuntu20.04 VM with ROOT here: https://box.nju.edu.cn/d/045506afb0f347b78806/   
-How to build your own ROOT release on Ubuntu20.04: https://blog.csdn.net/weixin_44121665/article/details/102637844?spm=1001.2014.3001.5502  
-Data collected by me, without proper Impedance matching: https://box.nju.edu.cn/d/8c35131d91e846c4ada6/     
-## Contact me
-Author: Zifeng XU  
-Email:  
-zifeng.xu@foxmail.com  
-mg20220214@smail.nju.edu.cn  
-zifeng.xu@cern.ch  
+Metadata-Version: 2.1
+Name: oscilloscope-scripts-xzf8971
+Version: 1.2.0
+Summary: A package to control and read data from oscilloscope. Support TekTronix TBS2000B now.
+Author-email: Zifeng <zifeng.xu@foxmail.com>
+Project-URL: Homepage, https://github.com/xzf89718/oscilloscope_scripts
+Project-URL: Bug Tracker, https://github.com/xzf89718/oscilloscope_scripts/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Oscilloscope scripts
+
+This project contains interface to help you collect waveform data from osilloscope. TekTronix TBS2000B is supported now. If you prefer old version follow the course slides. Please check here: https://github.com/xzf89718/oscilloscope_scripts/tree/v7.2 and https://github.com/xzf89718/oscilloscope_scripts/releases/tag/v7.2
+
+## Getting started  
+### Setup python and NI-VISA  
+#### For Windows   
+Python 3.8:   
+https://www.python.org/downloads/release/python-383/   
+NI-VISA:   
+https://www.ni.com/zh-cn/support/downloads/drivers/download.ni-visa.html  
+#### For Linux/Mac OS 
+Please install libserial libusb pyserial pyusb and install pure python base pyvisa-py
+### Install   
+#### Install package with pip     
+```bash
+pip install oscilloscope-scripts-xzf8971  
+```
+#### Install package from github with pip
+```bash
+pip install git+https://github.com/xzf89718/oscilloscope_scripts
+```
+Get source code from github:  
+```bash
+git clone git@github.com:xzf89718/oscilloscope_scripts.git
+```   
+
+### The commands here aim to setup package for python  
+```bash
+pip install -U virtualenv  
+virtualenv -p 3.8 ~/pyvisa_3d8  
+~/pyvisa_3d8/Scripts/activate  
+```
+
+## How to use this package
+### Every Login
+```bash
+cd ~/pyvisa_3d8/Scripts     
+.\activate  
+```
+### Use Tektronix_TBS2000B_scripts for TBS2000B DAQ
+#### Batch mode  
+```bash
+python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode batch
+# On macOS or linux
+# python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode batch --backend pyvisa-py
+```
+#### Interactive mode (for debug)
+```bash
+python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode inter
+# On macOS or linux
+# python -m Tektronix_TBS2000B_scripts this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --output_dir output_dir --scope_name auto --mode inter --backend pyvisa-py
+Enter your scope_name, also provide "default" and "auto" for quick setup  
+auto  
+```
+If the setup is correct, you will got a plot contain waveforms from CH1 and CH2  
+
+
+## Get some help
+```bash
+python  xxx.py --help  
+```
+Read the comments on the begin of each scripts  
+
+## Other materials
+In order to use the root scripts, you need ROOT and pyroot setup. Get Ubuntu20.04 VM with ROOT here: https://box.nju.edu.cn/d/045506afb0f347b78806/   
+How to build your own ROOT release on Ubuntu20.04: https://blog.csdn.net/weixin_44121665/article/details/102637844?spm=1001.2014.3001.5502  
+Data collected by me, without proper Impedance matching: https://box.nju.edu.cn/d/8c35131d91e846c4ada6/     
+## Contact me
+Author: Zifeng XU  
+Email:  
+zifeng.xu@foxmail.com  
+mg20220214@smail.nju.edu.cn  
+zifeng.xu@cern.ch
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/oscilloscope_scripts_xzf8971.egg-info/SOURCES.txt` & `oscilloscope_scripts_xzf8971-1.2.0/oscilloscope_scripts_xzf8971.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/pyproject.toml` & `oscilloscope_scripts_xzf8971-1.2.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-[build-system]
-requires = ["setuptools>=61.0", "setuptools-scm", "cython ~= 0.29.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "oscilloscope_scripts_xzf8971"
-version = "1.1.0"
-authors = [
-  { name="Zifeng", email="zifeng.xu@foxmail.com" },
-]
-description = "A package to control and read data from oscilloscope. Support TekTronix TBS2000B now."
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = ["numpy", "matplotlib", "pyserial", "pyvisa", "pyvisa-py", "pandas"]
-
-[project.urls]
-"Homepage" = "https://github.com/xzf89718/oscilloscope_scripts"
+[build-system]
+requires = ["setuptools>=61.0", "setuptools-scm", "cython ~= 0.29.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "oscilloscope_scripts_xzf8971"
+version = "1.2.0"
+authors = [
+  { name="Zifeng", email="zifeng.xu@foxmail.com" },
+]
+description = "A package to control and read data from oscilloscope. Support TekTronix TBS2000B now."
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = ["numpy", "matplotlib", "pyserial", "pyvisa", "pyvisa-py", "pandas"]
+
+[project.urls]
+"Homepage" = "https://github.com/xzf89718/oscilloscope_scripts"
 "Bug Tracker" = "https://github.com/xzf89718/oscilloscope_scripts/issues"
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/MakeWorkspaceForGain.C` & `oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/MakeWorkspaceForGain.C`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-#include "RooRealVar.h"
-#include "RooDataSet.h"
-#include "RooGaussian.h"
-#include "RooPoisson.h"
-#include "RooConstVar.h"
-#include "RooChebychev.h"
-#include "RooFormulaVar.h"
-
-#include "RooAddPdf.h"
-#include "RooProdPdf.h"
-#include "RooWorkspace.h"
-#include "RooPlot.h"
-#include "TCanvas.h"
-#include "TAxis.h"
-#include "TFile.h"
-#include "TH1.h"
-#include <vector>
-using namespace RooFit;
-
-int MakeWorkspaceForGain()
-{
-    RooWorkspace worksapceTwoPeak("worksapceTwoPeak");
-    RooWorkspace workspaceThreePeak("workspaceThreePeak");
-    RooWorkspace workspaceFourPeak("workspaceFourPeak");
-    RooWorkspace workspaceFivePeak("workspaceFivePeak");
-    RooWorkspace workspaceSixPeak("workspaceSixPeak");
-
-
-    // build three gaussian to fit the data
-    RooRealVar voltage0("voltage0", "Any unit", -5500., -4000.);
-    RooRealVar voltage1("voltage1", "Any unit", -5500., -4000.);
-    RooRealVar voltage2("voltage2", "Any unit", -5500., -4000.);
-    RooRealVar voltage3("voltage3", "Any unit", -5500., -4000.);
-    RooRealVar voltage4("voltage4", "Any unit", -5500., -4000.);
-
-
-    // Use gaussian as approximation of poisson
-    RooRealVar mean1("mean1", "Any unit", -4900., -5500., -4800.);
-    RooRealVar mean2("mean2", "Any unit", -4900., -5500., -4800.);
-    RooRealVar mean3("mean3", "Any unit", -4900., -5500., -4800.);
-    RooRealVar mean4("mean4", "Any unit", -4900., -5500., -4800.);
-    RooRealVar mean5("mean5", "Any unit", -4900., -5500., -4800.);
-    RooRealVar mean6("mean6", "Any unit", -4900., -5500., -4800.);
-
-
-    // Use gaussian as approximation of poisson
-    RooRealVar var1("var1", "var1", 10., 1.0, 1000.);
-    RooRealVar var2("var2", "var2", 10., 1.0, 1000.);
-    RooRealVar var3("var3", "var3", 10., 1.0, 1000.);
-    RooRealVar var4("var4", "var4", 10., 1.0, 1000.);
-    RooRealVar var5("var5", "var5", 10., 1.0, 1000.);
-    RooRealVar var6("var6", "var6", 10., 1.0, 1000.);
-
-    // Build gaussian
-    RooGaussian gaus1TwoPeak("gaus1TwoPeak", "gaus1TwoPeak", voltage0, mean1, var1);
-    RooGaussian gaus2TwoPeak("gaus2TwoPeak", "gaus2TwoPeak", voltage0, mean2, var2);
-
-    RooGaussian gaus1ThreePeak("gaus1ThreePeak", "gaus1ThreePeak", voltage1, mean1, var1);
-    RooGaussian gaus2ThreePeak("gaus2ThreePeak", "gaus2ThreePeak", voltage1, mean2, var2);
-    RooGaussian gaus3ThreePeak("gaus3ThreePeak", "gaus3ThreePeak", voltage1, mean3, var3);
-
-    RooGaussian gaus1FourPeak("gaus1FourPeak", "gaus1FourPeak", voltage2, mean1, var1);
-    RooGaussian gaus2FourPeak("gaus2FourPeak", "gaus2FourPeak", voltage2, mean2, var2);
-    RooGaussian gaus3FourPeak("gaus3FourPeak", "gaus3FourPeak", voltage2, mean3, var3);
-    RooGaussian gaus4FourPeak("gaus4FourPeak", "gaus4FourPeak", voltage2, mean4, var4);
-
-    RooGaussian gaus1FivePeak("gaus1FivePeak", "gaus1FivePeak", voltage3, mean1, var1);
-    RooGaussian gaus2FivePeak("gaus2FivePeak", "gaus2FivePeak", voltage3, mean2, var2);
-    RooGaussian gaus3FivePeak("gaus3FivePeak", "gaus3FivePeak", voltage3, mean3, var3);
-    RooGaussian gaus4FivePeak("gaus4FivePeak", "gaus4FivePeak", voltage3, mean4, var4);
-    RooGaussian gaus5FivePeak("gaus5FivePeak", "gaus5FivePeak", voltage3, mean5, var5);
-
-    RooGaussian gaus1SixPeak("gaus1SixPeak", "gaus1SixPeak", voltage4, mean1, var1);
-    RooGaussian gaus2SixPeak("gaus2SixPeak", "gaus2SixPeak", voltage4, mean2, var2);
-    RooGaussian gaus3SixPeak("gaus3SixPeak", "gaus3SixPeak", voltage4, mean3, var3);
-    RooGaussian gaus4SixPeak("gaus4SixPeak", "gaus4SixPeak", voltage4, mean4, var4);
-    RooGaussian gaus5SixPeak("gaus5SixPeak", "gaus5SixPeak", voltage4, mean5, var5);
-    RooGaussian gaus6SixPeak("gaus6SixPeak", "gaus6SixPeak", voltage4, mean6, var6);
-
-        // Fraction of different gaussian
-    RooRealVar n1("n1", "#Number of peak 1", 0.1, 0., 1.);
-    RooRealVar n2("n2", "#Number of peak 2", 0.1, 0., 1.);
-    RooRealVar n3("n3", "#Number of peak 3", 0.1, 0., 1.);
-    RooRealVar n4("n4", "#Number of peak 4", 0.1, 0., 1.);
-    RooRealVar n5("n5", "#Number of peak 5", 0.1, 0., 1.);
-    RooRealVar n6("n6", "#Number of peak 6", 0.1, 0., 1.);
-    // Build combined distribution PDF
-    RooAddPdf twoPeakGaus("twoPeakGaus", "gaus1+gaus2", RooArgList(gaus1TwoPeak, gaus2TwoPeak), RooArgList(n1));
-    RooAddPdf threePeakGaus("threePeakGaus", "gaus1+gaus2+gaus3", RooArgList(gaus1ThreePeak, gaus2ThreePeak, gaus3ThreePeak), RooArgList(n1, n2));
-    RooAddPdf fourPeakGaus("fourPeakGaus", "gaus1+gaus2+gaus3+gaus4", RooArgList(gaus1FourPeak, gaus2FourPeak, gaus3FourPeak, gaus4FourPeak), RooArgList(n1, n2, n3));
-    RooAddPdf fivePeakGaus("fivePeakGaus", "gaus1+gaus2+gaus3+gaus4+gaus5", RooArgList(gaus1FivePeak, gaus2FivePeak, gaus3FivePeak, gaus4FivePeak, gaus5FivePeak), RooArgList(n1, n2, n3, n4));
-    RooAddPdf sixPeakGaus("sixPeakGaus", "gaus1+gaus2+gaus3+gaus4+gaus5+gaus6", RooArgList(gaus1SixPeak, gaus2SixPeak, gaus3SixPeak, gaus4SixPeak, gaus5SixPeak, gaus6SixPeak), RooArgList(n1, n2, n3, n4, n5));
-
-
-    worksapceTwoPeak.import(twoPeakGaus);
-    workspaceThreePeak.import(threePeakGaus);
-    workspaceFourPeak.import(fourPeakGaus);
-    workspaceFivePeak.import(fivePeakGaus);
-    workspaceSixPeak.import(sixPeakGaus);
-
-    // Generate toy model
-    // for (auto i = 0; i < 100; i++)
-    // {
-    //     RooDataSet *dataThreePeak = threePeakGaus.generate(voltage1, 10000, Name((std::string("toydataThreePeak") + std::to_string(i)).c_str()));
-    //     RooDataSet *dataFourPeak = fourPeakGaus.generate(voltage2, 10000, Name((std::string("toydataFourPeak") + std::to_string(i)).c_str()));
-    //     RooDataSet *dataFivePeak = fivePeakGaus.generate(voltage3, 10000, Name((std::string("toydataFivePeak") + std::to_string(i)).c_str()));
-    //     RooDataSet *dataSixPeak = sixPeakGaus.generate(voltage4, 10000, Name((std::string("toydataSixPeak") + std::to_string(i)).c_str()));
-
-    //     workspaceThreePeak.import(*dataThreePeak);
-    //     workspaceFourPeak.import(*dataFourPeak);
-    //     workspaceFivePeak.import(*dataFivePeak);
-    //     workspaceSixPeak.import(*dataSixPeak);
-
-    // }
-    // auto *toydataThreePeak = workspaceThreePeak.data("toydataThreePeak100");
-    // threePeakGaus.fitTo(*toydataThreePeak);
-    // auto *toydataFourPeak = workspaceFourPeak.data("toydataFourPeak100");
-    // fourPeakGaus.fitTo(*toydataFourPeak);
-    // auto *toydataFivePeak = workspaceFivePeak.data("toydataFivePeak100");
-    // fivePeakGaus.fitTo(*toydataFivePeak);
-    // auto *toydataSixPeak = workspaceSixPeak.data("toydataSixPeak100");
-    // sixPeakGaus.fitTo(*toydataSixPeak);
-
-    workspaceThreePeak.writeToFile("gainFitWorkspace.root", true);
-    worksapceTwoPeak.writeToFile("gainFitWorkspace.root", false);
-    workspaceFourPeak.writeToFile("gainFitWorkspace.root", false);
-    workspaceFivePeak.writeToFile("gainFitWorkspace.root", false);
-    workspaceSixPeak.writeToFile("gainFitWorkspace.root", false);
-    return 0;
-}
+#include "RooRealVar.h"
+#include "RooDataSet.h"
+#include "RooGaussian.h"
+#include "RooPoisson.h"
+#include "RooConstVar.h"
+#include "RooChebychev.h"
+#include "RooFormulaVar.h"
+
+#include "RooAddPdf.h"
+#include "RooProdPdf.h"
+#include "RooWorkspace.h"
+#include "RooPlot.h"
+#include "TCanvas.h"
+#include "TAxis.h"
+#include "TFile.h"
+#include "TH1.h"
+#include <vector>
+using namespace RooFit;
+
+int MakeWorkspaceForGain()
+{
+    RooWorkspace worksapceTwoPeak("worksapceTwoPeak");
+    RooWorkspace workspaceThreePeak("workspaceThreePeak");
+    RooWorkspace workspaceFourPeak("workspaceFourPeak");
+    RooWorkspace workspaceFivePeak("workspaceFivePeak");
+    RooWorkspace workspaceSixPeak("workspaceSixPeak");
+
+
+    // build three gaussian to fit the data
+    RooRealVar voltage0("voltage0", "Any unit", -5500., -4000.);
+    RooRealVar voltage1("voltage1", "Any unit", -5500., -4000.);
+    RooRealVar voltage2("voltage2", "Any unit", -5500., -4000.);
+    RooRealVar voltage3("voltage3", "Any unit", -5500., -4000.);
+    RooRealVar voltage4("voltage4", "Any unit", -5500., -4000.);
+
+
+    // Use gaussian as approximation of poisson
+    RooRealVar mean1("mean1", "Any unit", -4900., -5500., -4800.);
+    RooRealVar mean2("mean2", "Any unit", -4900., -5500., -4800.);
+    RooRealVar mean3("mean3", "Any unit", -4900., -5500., -4800.);
+    RooRealVar mean4("mean4", "Any unit", -4900., -5500., -4800.);
+    RooRealVar mean5("mean5", "Any unit", -4900., -5500., -4800.);
+    RooRealVar mean6("mean6", "Any unit", -4900., -5500., -4800.);
+
+
+    // Use gaussian as approximation of poisson
+    RooRealVar var1("var1", "var1", 10., 1.0, 1000.);
+    RooRealVar var2("var2", "var2", 10., 1.0, 1000.);
+    RooRealVar var3("var3", "var3", 10., 1.0, 1000.);
+    RooRealVar var4("var4", "var4", 10., 1.0, 1000.);
+    RooRealVar var5("var5", "var5", 10., 1.0, 1000.);
+    RooRealVar var6("var6", "var6", 10., 1.0, 1000.);
+
+    // Build gaussian
+    RooGaussian gaus1TwoPeak("gaus1TwoPeak", "gaus1TwoPeak", voltage0, mean1, var1);
+    RooGaussian gaus2TwoPeak("gaus2TwoPeak", "gaus2TwoPeak", voltage0, mean2, var2);
+
+    RooGaussian gaus1ThreePeak("gaus1ThreePeak", "gaus1ThreePeak", voltage1, mean1, var1);
+    RooGaussian gaus2ThreePeak("gaus2ThreePeak", "gaus2ThreePeak", voltage1, mean2, var2);
+    RooGaussian gaus3ThreePeak("gaus3ThreePeak", "gaus3ThreePeak", voltage1, mean3, var3);
+
+    RooGaussian gaus1FourPeak("gaus1FourPeak", "gaus1FourPeak", voltage2, mean1, var1);
+    RooGaussian gaus2FourPeak("gaus2FourPeak", "gaus2FourPeak", voltage2, mean2, var2);
+    RooGaussian gaus3FourPeak("gaus3FourPeak", "gaus3FourPeak", voltage2, mean3, var3);
+    RooGaussian gaus4FourPeak("gaus4FourPeak", "gaus4FourPeak", voltage2, mean4, var4);
+
+    RooGaussian gaus1FivePeak("gaus1FivePeak", "gaus1FivePeak", voltage3, mean1, var1);
+    RooGaussian gaus2FivePeak("gaus2FivePeak", "gaus2FivePeak", voltage3, mean2, var2);
+    RooGaussian gaus3FivePeak("gaus3FivePeak", "gaus3FivePeak", voltage3, mean3, var3);
+    RooGaussian gaus4FivePeak("gaus4FivePeak", "gaus4FivePeak", voltage3, mean4, var4);
+    RooGaussian gaus5FivePeak("gaus5FivePeak", "gaus5FivePeak", voltage3, mean5, var5);
+
+    RooGaussian gaus1SixPeak("gaus1SixPeak", "gaus1SixPeak", voltage4, mean1, var1);
+    RooGaussian gaus2SixPeak("gaus2SixPeak", "gaus2SixPeak", voltage4, mean2, var2);
+    RooGaussian gaus3SixPeak("gaus3SixPeak", "gaus3SixPeak", voltage4, mean3, var3);
+    RooGaussian gaus4SixPeak("gaus4SixPeak", "gaus4SixPeak", voltage4, mean4, var4);
+    RooGaussian gaus5SixPeak("gaus5SixPeak", "gaus5SixPeak", voltage4, mean5, var5);
+    RooGaussian gaus6SixPeak("gaus6SixPeak", "gaus6SixPeak", voltage4, mean6, var6);
+
+        // Fraction of different gaussian
+    RooRealVar n1("n1", "#Number of peak 1", 0.1, 0., 1.);
+    RooRealVar n2("n2", "#Number of peak 2", 0.1, 0., 1.);
+    RooRealVar n3("n3", "#Number of peak 3", 0.1, 0., 1.);
+    RooRealVar n4("n4", "#Number of peak 4", 0.1, 0., 1.);
+    RooRealVar n5("n5", "#Number of peak 5", 0.1, 0., 1.);
+    RooRealVar n6("n6", "#Number of peak 6", 0.1, 0., 1.);
+    // Build combined distribution PDF
+    RooAddPdf twoPeakGaus("twoPeakGaus", "gaus1+gaus2", RooArgList(gaus1TwoPeak, gaus2TwoPeak), RooArgList(n1));
+    RooAddPdf threePeakGaus("threePeakGaus", "gaus1+gaus2+gaus3", RooArgList(gaus1ThreePeak, gaus2ThreePeak, gaus3ThreePeak), RooArgList(n1, n2));
+    RooAddPdf fourPeakGaus("fourPeakGaus", "gaus1+gaus2+gaus3+gaus4", RooArgList(gaus1FourPeak, gaus2FourPeak, gaus3FourPeak, gaus4FourPeak), RooArgList(n1, n2, n3));
+    RooAddPdf fivePeakGaus("fivePeakGaus", "gaus1+gaus2+gaus3+gaus4+gaus5", RooArgList(gaus1FivePeak, gaus2FivePeak, gaus3FivePeak, gaus4FivePeak, gaus5FivePeak), RooArgList(n1, n2, n3, n4));
+    RooAddPdf sixPeakGaus("sixPeakGaus", "gaus1+gaus2+gaus3+gaus4+gaus5+gaus6", RooArgList(gaus1SixPeak, gaus2SixPeak, gaus3SixPeak, gaus4SixPeak, gaus5SixPeak, gaus6SixPeak), RooArgList(n1, n2, n3, n4, n5));
+
+
+    worksapceTwoPeak.import(twoPeakGaus);
+    workspaceThreePeak.import(threePeakGaus);
+    workspaceFourPeak.import(fourPeakGaus);
+    workspaceFivePeak.import(fivePeakGaus);
+    workspaceSixPeak.import(sixPeakGaus);
+
+    // Generate toy model
+    // for (auto i = 0; i < 100; i++)
+    // {
+    //     RooDataSet *dataThreePeak = threePeakGaus.generate(voltage1, 10000, Name((std::string("toydataThreePeak") + std::to_string(i)).c_str()));
+    //     RooDataSet *dataFourPeak = fourPeakGaus.generate(voltage2, 10000, Name((std::string("toydataFourPeak") + std::to_string(i)).c_str()));
+    //     RooDataSet *dataFivePeak = fivePeakGaus.generate(voltage3, 10000, Name((std::string("toydataFivePeak") + std::to_string(i)).c_str()));
+    //     RooDataSet *dataSixPeak = sixPeakGaus.generate(voltage4, 10000, Name((std::string("toydataSixPeak") + std::to_string(i)).c_str()));
+
+    //     workspaceThreePeak.import(*dataThreePeak);
+    //     workspaceFourPeak.import(*dataFourPeak);
+    //     workspaceFivePeak.import(*dataFivePeak);
+    //     workspaceSixPeak.import(*dataSixPeak);
+
+    // }
+    // auto *toydataThreePeak = workspaceThreePeak.data("toydataThreePeak100");
+    // threePeakGaus.fitTo(*toydataThreePeak);
+    // auto *toydataFourPeak = workspaceFourPeak.data("toydataFourPeak100");
+    // fourPeakGaus.fitTo(*toydataFourPeak);
+    // auto *toydataFivePeak = workspaceFivePeak.data("toydataFivePeak100");
+    // fivePeakGaus.fitTo(*toydataFivePeak);
+    // auto *toydataSixPeak = workspaceSixPeak.data("toydataSixPeak100");
+    // sixPeakGaus.fitTo(*toydataSixPeak);
+
+    workspaceThreePeak.writeToFile("gainFitWorkspace.root", true);
+    worksapceTwoPeak.writeToFile("gainFitWorkspace.root", false);
+    workspaceFourPeak.writeToFile("gainFitWorkspace.root", false);
+    workspaceFivePeak.writeToFile("gainFitWorkspace.root", false);
+    workspaceSixPeak.writeToFile("gainFitWorkspace.root", false);
+    return 0;
+}
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/OutputCharge.C` & `oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/OutputCharge.C`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-#define OutputCharge_cxx
-// The class definition in OutputCharge.h has been generated automatically
-// by the ROOT utility TTree::MakeSelector(). This class is derived
-// from the ROOT class TSelector. For more information on the TSelector
-// framework see $ROOTSYS/README/README.SELECTOR or the ROOT User Manual.
-
-// The following methods are defined in this file:
-//    Begin():        called every time a loop on the tree starts,
-//                    a convenient place to create your histograms.
-//    SlaveBegin():   called after Begin(), when on PROOF called only on the
-//                    slave servers.
-//    Process():      called for each event, in this function you decide what
-//                    to read and fill your histograms.
-//    SlaveTerminate: called at the end of the loop on the tree, when on PROOF
-//                    called only on the slave servers.
-//    Terminate():    called at the end of the loop on the tree,
-//                    a convenient place to draw/fit your histograms.
-//
-// To use this file, try the following session on your Tree T:
-//
-// root> T->Process("OutputCharge.C")
-// root> T->Process("OutputCharge.C","some options")
-// root> T->Process("OutputCharge.C+")
-//
-
-#include "OutputCharge.h"
-#include <TH2.h>
-#include <TStyle.h>
-#include <TTree.h>
-
-void OutputCharge::Begin(TTree * /*tree*/)
-{
-   // The Begin() function is called at the start of the query.
-   // When running with PROOF Begin() is only called on the client.
-   // The tree argument is deprecated (on PROOF 0 is passed).
-
-   TString option = GetOption();
-   m_output_file = TFile::Open("output_charge.root", "RECREATE");
-   ahisto = new TH1F("ahisto", "ahisto", 500, -5200, -4700);
-   ahisto_shift = new TH1F("ahisto_shift", "ahisto_shift", 500, -500., 100.);
-   
-}
-
-void OutputCharge::SlaveBegin(TTree * /*tree*/)
-{
-   // The SlaveBegin() function is called after the Begin() function.
-   // When running with PROOF SlaveBegin() is called on each slave server.
-   // The tree argument is deprecated (on PROOF 0 is passed).
-
-   TString option = GetOption();
-}
-
-Bool_t OutputCharge::Process(Long64_t entry)
-{
-   // The Process() function is called for each entry in the tree (or possibly
-   // keyed object in the case of PROOF) to be processed. The entry argument
-   // specifies which entry in the currently loaded tree is to be processed.
-   // When processing keyed objects with PROOF, the object is already loaded
-   // and is available via the fObject pointer.
-   //
-   // This function should contain the \"body\" of the analysis. It can contain
-   // simple or elaborate selection criteria, run algorithms on the data
-   // of the event and typically fill histograms.
-   //
-   // The processing can be stopped by calling Abort().
-   //
-   // Use fStatus to set the return value of TTree::Process().
-   //
-   // The return value is currently not used.
-
-   fReader.SetLocalEntry(entry);
-   // only read data both channel has waveform
-   // if (!*trig_level)
-   /// read all data
-   // if(true)
-   // only do this if you want to measure the mean charge of no signal
-   if(*trig_level)
-   {
-      ahisto->Fill(*charge);
-      ahisto_shift->Fill(*charge_shift);
-   }
-   return kTRUE;
-}
-
-void OutputCharge::SlaveTerminate()
-{
-   // The SlaveTerminate() function is called after all entries or objects
-   // have been processed. When running with PROOF SlaveTerminate() is called
-   // on each slave server.
-}
-
-void OutputCharge::Terminate()
-{
-   // The Terminate() function is the last function to be called during
-   // a query. It always runs on the client, it can be used to present
-   // the results graphically or save the results to file.
-
-   ahisto->Write();
-   ahisto_shift->Write();
-   m_output_file->Close();
-}
+#define OutputCharge_cxx
+// The class definition in OutputCharge.h has been generated automatically
+// by the ROOT utility TTree::MakeSelector(). This class is derived
+// from the ROOT class TSelector. For more information on the TSelector
+// framework see $ROOTSYS/README/README.SELECTOR or the ROOT User Manual.
+
+// The following methods are defined in this file:
+//    Begin():        called every time a loop on the tree starts,
+//                    a convenient place to create your histograms.
+//    SlaveBegin():   called after Begin(), when on PROOF called only on the
+//                    slave servers.
+//    Process():      called for each event, in this function you decide what
+//                    to read and fill your histograms.
+//    SlaveTerminate: called at the end of the loop on the tree, when on PROOF
+//                    called only on the slave servers.
+//    Terminate():    called at the end of the loop on the tree,
+//                    a convenient place to draw/fit your histograms.
+//
+// To use this file, try the following session on your Tree T:
+//
+// root> T->Process("OutputCharge.C")
+// root> T->Process("OutputCharge.C","some options")
+// root> T->Process("OutputCharge.C+")
+//
+
+#include "OutputCharge.h"
+#include <TH2.h>
+#include <TStyle.h>
+#include <TTree.h>
+
+void OutputCharge::Begin(TTree * /*tree*/)
+{
+   // The Begin() function is called at the start of the query.
+   // When running with PROOF Begin() is only called on the client.
+   // The tree argument is deprecated (on PROOF 0 is passed).
+
+   TString option = GetOption();
+   m_output_file = TFile::Open("output_charge.root", "RECREATE");
+   ahisto = new TH1F("ahisto", "ahisto", 500, -5200, -4700);
+   ahisto_shift = new TH1F("ahisto_shift", "ahisto_shift", 500, -500., 100.);
+   
+}
+
+void OutputCharge::SlaveBegin(TTree * /*tree*/)
+{
+   // The SlaveBegin() function is called after the Begin() function.
+   // When running with PROOF SlaveBegin() is called on each slave server.
+   // The tree argument is deprecated (on PROOF 0 is passed).
+
+   TString option = GetOption();
+}
+
+Bool_t OutputCharge::Process(Long64_t entry)
+{
+   // The Process() function is called for each entry in the tree (or possibly
+   // keyed object in the case of PROOF) to be processed. The entry argument
+   // specifies which entry in the currently loaded tree is to be processed.
+   // When processing keyed objects with PROOF, the object is already loaded
+   // and is available via the fObject pointer.
+   //
+   // This function should contain the \"body\" of the analysis. It can contain
+   // simple or elaborate selection criteria, run algorithms on the data
+   // of the event and typically fill histograms.
+   //
+   // The processing can be stopped by calling Abort().
+   //
+   // Use fStatus to set the return value of TTree::Process().
+   //
+   // The return value is currently not used.
+
+   fReader.SetLocalEntry(entry);
+   // only read data both channel has waveform
+   // if (!*trig_level)
+   /// read all data
+   // if(true)
+   // only do this if you want to measure the mean charge of no signal
+   if(*trig_level)
+   {
+      ahisto->Fill(*charge);
+      ahisto_shift->Fill(*charge_shift);
+   }
+   return kTRUE;
+}
+
+void OutputCharge::SlaveTerminate()
+{
+   // The SlaveTerminate() function is called after all entries or objects
+   // have been processed. When running with PROOF SlaveTerminate() is called
+   // on each slave server.
+}
+
+void OutputCharge::Terminate()
+{
+   // The Terminate() function is the last function to be called during
+   // a query. It always runs on the client, it can be used to present
+   // the results graphically or save the results to file.
+
+   ahisto->Write();
+   ahisto_shift->Write();
+   m_output_file->Close();
+}
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/OutputCharge.h` & `oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/OutputCharge.h`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-//////////////////////////////////////////////////////////
-// This class has been automatically generated on
-// Sun Sep 12 21:29:49 2021 by ROOT version 6.24/00
-// from TTree event/event
-// found on file: channel2_trig_n3p00_cut_charge_n4400_level_n2p68_CH3.root
-//////////////////////////////////////////////////////////
-
-#ifndef OutputCharge_h
-#define OutputCharge_h
-
-#include <TROOT.h>
-#include <TChain.h>
-#include <TFile.h>
-#include <TSelector.h>
-#include <TTreeReader.h>
-#include <TTreeReaderValue.h>
-#include <TTreeReaderArray.h>
-
-// Headers needed by this particular selector
-
-class OutputCharge : public TSelector
-{
-public:
-   TTreeReader fReader; //!the tree reader
-   TTree *fChain = 0;   //!pointer to the analyzed TTree or TChain
-   TFile *m_output_file;
-   TH1F *ahisto;
-   TH1F *ahisto_shift;
-   // Readers to access the data (delete the ones you do not need).
-   TTreeReaderValue<Double_t> max_voltage = {fReader, "max_voltage"};
-   TTreeReaderValue<Int_t> width = {fReader, "width"};
-   TTreeReaderValue<Double_t> charge = {fReader, "charge"};
-   TTreeReaderValue<Double_t> charge_shift = {fReader, "charge_shift"};
-   TTreeReaderValue<Int_t> trig_charge = {fReader, "trig_charge"};
-   TTreeReaderValue<Int_t> pass_width = {fReader, "pass_width"};
-   TTreeReaderValue<Int_t> trig_level = {fReader, "trig_level"};
-   TTreeReaderValue<Double_t> baseline_estimate = {fReader, "baseline_estimate"};
-
-   OutputCharge(TTree * /*tree*/ = 0) {}
-   virtual ~OutputCharge() {}
-   virtual Int_t Version() const { return 2; }
-   virtual void Begin(TTree *tree);
-   virtual void SlaveBegin(TTree *tree);
-   virtual void Init(TTree *tree);
-   virtual Bool_t Notify();
-   virtual Bool_t Process(Long64_t entry);
-   virtual Int_t GetEntry(Long64_t entry, Int_t getall = 0) { return fChain ? fChain->GetTree()->GetEntry(entry, getall) : 0; }
-   virtual void SetOption(const char *option) { fOption = option; }
-   virtual void SetObject(TObject *obj) { fObject = obj; }
-   virtual void SetInputList(TList *input) { fInput = input; }
-   virtual TList *GetOutputList() const { return fOutput; }
-   virtual void SlaveTerminate();
-   virtual void Terminate();
-
-   ClassDef(OutputCharge, 0);
-};
-
-#endif
-
-#ifdef OutputCharge_cxx
-void OutputCharge::Init(TTree *tree)
-{
-   // The Init() function is called when the selector needs to initialize
-   // a new tree or chain. Typically here the reader is initialized.
-   // It is normally not necessary to make changes to the generated
-   // code, but the routine can be extended by the user if needed.
-   // Init() will be called many times when running on PROOF
-   // (once per file to be processed).
-
-   fReader.SetTree(tree);
-}
-
-Bool_t OutputCharge::Notify()
-{
-   // The Notify() function is called when a new file is opened. This
-   // can be either for a new TTree in a TChain or when when a new TTree
-   // is started when using PROOF. It is normally not necessary to make changes
-   // to the generated code, but the routine can be extended by the
-   // user if needed. The return value is currently not used.
-
-   return kTRUE;
-}
-
-#endif // #ifdef OutputCharge_cxx
+//////////////////////////////////////////////////////////
+// This class has been automatically generated on
+// Sun Sep 12 21:29:49 2021 by ROOT version 6.24/00
+// from TTree event/event
+// found on file: channel2_trig_n3p00_cut_charge_n4400_level_n2p68_CH3.root
+//////////////////////////////////////////////////////////
+
+#ifndef OutputCharge_h
+#define OutputCharge_h
+
+#include <TROOT.h>
+#include <TChain.h>
+#include <TFile.h>
+#include <TSelector.h>
+#include <TTreeReader.h>
+#include <TTreeReaderValue.h>
+#include <TTreeReaderArray.h>
+
+// Headers needed by this particular selector
+
+class OutputCharge : public TSelector
+{
+public:
+   TTreeReader fReader; //!the tree reader
+   TTree *fChain = 0;   //!pointer to the analyzed TTree or TChain
+   TFile *m_output_file;
+   TH1F *ahisto;
+   TH1F *ahisto_shift;
+   // Readers to access the data (delete the ones you do not need).
+   TTreeReaderValue<Double_t> max_voltage = {fReader, "max_voltage"};
+   TTreeReaderValue<Int_t> width = {fReader, "width"};
+   TTreeReaderValue<Double_t> charge = {fReader, "charge"};
+   TTreeReaderValue<Double_t> charge_shift = {fReader, "charge_shift"};
+   TTreeReaderValue<Int_t> trig_charge = {fReader, "trig_charge"};
+   TTreeReaderValue<Int_t> pass_width = {fReader, "pass_width"};
+   TTreeReaderValue<Int_t> trig_level = {fReader, "trig_level"};
+   TTreeReaderValue<Double_t> baseline_estimate = {fReader, "baseline_estimate"};
+
+   OutputCharge(TTree * /*tree*/ = 0) {}
+   virtual ~OutputCharge() {}
+   virtual Int_t Version() const { return 2; }
+   virtual void Begin(TTree *tree);
+   virtual void SlaveBegin(TTree *tree);
+   virtual void Init(TTree *tree);
+   virtual Bool_t Notify();
+   virtual Bool_t Process(Long64_t entry);
+   virtual Int_t GetEntry(Long64_t entry, Int_t getall = 0) { return fChain ? fChain->GetTree()->GetEntry(entry, getall) : 0; }
+   virtual void SetOption(const char *option) { fOption = option; }
+   virtual void SetObject(TObject *obj) { fObject = obj; }
+   virtual void SetInputList(TList *input) { fInput = input; }
+   virtual TList *GetOutputList() const { return fOutput; }
+   virtual void SlaveTerminate();
+   virtual void Terminate();
+
+   ClassDef(OutputCharge, 0);
+};
+
+#endif
+
+#ifdef OutputCharge_cxx
+void OutputCharge::Init(TTree *tree)
+{
+   // The Init() function is called when the selector needs to initialize
+   // a new tree or chain. Typically here the reader is initialized.
+   // It is normally not necessary to make changes to the generated
+   // code, but the routine can be extended by the user if needed.
+   // Init() will be called many times when running on PROOF
+   // (once per file to be processed).
+
+   fReader.SetTree(tree);
+}
+
+Bool_t OutputCharge::Notify()
+{
+   // The Notify() function is called when a new file is opened. This
+   // can be either for a new TTree in a TChain or when when a new TTree
+   // is started when using PROOF. It is normally not necessary to make changes
+   // to the generated code, but the routine can be extended by the
+   // user if needed. The return value is currently not used.
+
+   return kTRUE;
+}
+
+#endif // #ifdef OutputCharge_cxx
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/Plot_waveform_from_root.py` & `oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/Plot_waveform_from_root.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-#!/usr/bin/env python
-# Author: Zifeng Xu
-# Email: zifeng.xu@cern.ch
-# Usage: Use this script to draw charge and max voltage in waveform
-# Example: python Plot_waveform_from_root.py this_is_an_example.root --n_plot_waveforms 10 --plot_channels CH1,CH2,CH3 --save_names this_is_an_example
-import argparse
-import matplotlib.pyplot as plt
-import ROOT
-import numpy as np
-import matplotlib
-matplotlib.use("TkAgg")
-
-
-class Waveform_one_channel():
-    def __init__(self) -> None:
-        self.size = np.zeros(1, dtype=int)
-        self.time = np.zeros(5000, dtype=float)
-        self.voltage = np.zeros(5000, dtype=float)
-
-
-class Tree_waveform():
-
-    def __init__(self, input_filename, list_channels) -> None:
-        self.entry = 0
-        self.list_channels = list_channels
-        self.__input_filename = input_filename
-        self.__input_TFile = ROOT.TFile.Open(input_filename)
-        self.dic_tree = {}
-        self.dic_waveform_one_channel = {}
-        for _channel in self.list_channels.split(','):
-            self.dic_tree[_channel] = self.__input_TFile.Get(
-                "tree_waveform_{0}".format(_channel))
-            self.dic_waveform_one_channel[_channel] = Waveform_one_channel()
-            self.dic_tree[_channel].SetBranchAddress(
-                "size", self.dic_waveform_one_channel[_channel].size)
-            self.dic_tree[_channel].SetBranchAddress(
-                "time", self.dic_waveform_one_channel[_channel].time)
-            self.dic_tree[_channel].SetBranchAddress(
-                "voltage", self.dic_waveform_one_channel[_channel].voltage)
-
-    def my_GetEntry(self, i_entry):
-        for _channel in self.list_channels.split(','):
-            self.dic_tree[_channel].GetEntry(i_entry)
-
-        self.entry = i_entry
-
-    def Plot_this_entry(self, save_name):
-        for _channel in self.list_channels.split(','):
-            plt.plot(
-                self.dic_waveform_one_channel[_channel].time[:
-                                                             self.dic_waveform_one_channel[_channel].size[0]],
-                self.dic_waveform_one_channel[_channel].voltage[:
-                                                                self.dic_waveform_one_channel[_channel].size[0]],
-                label=_channel)
-        plt.legend()
-        plt.savefig(save_name)
-        plt.close()
-        # plt.show()
-
-
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser(
-        description="Use this script to plot some waveform figure. Author: Zifeng XU, email: zifeng.xu@cern.ch")
-
-    parser.add_argument("input_rootfile", type=str,
-                        help="Input root file. Please include full path to the file")
-    parser.add_argument("index_you_want_to_plot", type=int,
-                        help="Which one you want to plot")
-    parser.add_argument("--n_plot_waveforms", type=int, default=10,
-                        help="N_Waveforms save in the output scripts")
-    parser.add_argument("--plot_channels", type=str, default="CH1,CH2,CH3",
-                        help="Which channel should we save in the scripts? Example: CH1,CH2,CH3")
-    parser.add_argument("--save_name", type=str, default='waveform_plot',
-                        help="header of saved figures")
-
-    args = parser.parse_args()
-    print("All parameters get from commandline are:")
-    print(args)
-
-    input_rootfile = args.input_rootfile
-    index_you_want_to_plot = args.index_you_want_to_plot
-    n_plot_waveforms = args.n_plot_waveforms
-    plot_channels = args.plot_channels
-    save_name = args.save_name
-
-    # Init
-    my_tree_waveforms = Tree_waveform(
-        input_filename=input_rootfile, list_channels=plot_channels)
-    for i in range(index_you_want_to_plot, index_you_want_to_plot+n_plot_waveforms):
-        my_tree_waveforms.my_GetEntry(i)
-        my_tree_waveforms.Plot_this_entry(
-            save_name='{0}-{1}.png'.format(save_name, str(i)))
+#!/usr/bin/env python
+# Author: Zifeng Xu
+# Email: zifeng.xu@cern.ch
+# Usage: Use this script to draw charge and max voltage in waveform
+# Example: python Plot_waveform_from_root.py this_is_an_example.root --n_plot_waveforms 10 --plot_channels CH1,CH2,CH3 --save_names this_is_an_example
+import argparse
+import matplotlib.pyplot as plt
+import ROOT
+import numpy as np
+import matplotlib
+matplotlib.use("TkAgg")
+
+
+class Waveform_one_channel():
+    def __init__(self) -> None:
+        self.size = np.zeros(1, dtype=int)
+        self.time = np.zeros(5000, dtype=float)
+        self.voltage = np.zeros(5000, dtype=float)
+
+
+class Tree_waveform():
+
+    def __init__(self, input_filename, list_channels) -> None:
+        self.entry = 0
+        self.list_channels = list_channels
+        self.__input_filename = input_filename
+        self.__input_TFile = ROOT.TFile.Open(input_filename)
+        self.dic_tree = {}
+        self.dic_waveform_one_channel = {}
+        for _channel in self.list_channels.split(','):
+            self.dic_tree[_channel] = self.__input_TFile.Get(
+                "tree_waveform_{0}".format(_channel))
+            self.dic_waveform_one_channel[_channel] = Waveform_one_channel()
+            self.dic_tree[_channel].SetBranchAddress(
+                "size", self.dic_waveform_one_channel[_channel].size)
+            self.dic_tree[_channel].SetBranchAddress(
+                "time", self.dic_waveform_one_channel[_channel].time)
+            self.dic_tree[_channel].SetBranchAddress(
+                "voltage", self.dic_waveform_one_channel[_channel].voltage)
+
+    def my_GetEntry(self, i_entry):
+        for _channel in self.list_channels.split(','):
+            self.dic_tree[_channel].GetEntry(i_entry)
+
+        self.entry = i_entry
+
+    def Plot_this_entry(self, save_name):
+        for _channel in self.list_channels.split(','):
+            plt.plot(
+                self.dic_waveform_one_channel[_channel].time[:
+                                                             self.dic_waveform_one_channel[_channel].size[0]],
+                self.dic_waveform_one_channel[_channel].voltage[:
+                                                                self.dic_waveform_one_channel[_channel].size[0]],
+                label=_channel)
+        plt.legend()
+        plt.savefig(save_name)
+        plt.close()
+        # plt.show()
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser(
+        description="Use this script to plot some waveform figure. Author: Zifeng XU, email: zifeng.xu@cern.ch")
+
+    parser.add_argument("input_rootfile", type=str,
+                        help="Input root file. Please include full path to the file")
+    parser.add_argument("index_you_want_to_plot", type=int,
+                        help="Which one you want to plot")
+    parser.add_argument("--n_plot_waveforms", type=int, default=10,
+                        help="N_Waveforms save in the output scripts")
+    parser.add_argument("--plot_channels", type=str, default="CH1,CH2,CH3",
+                        help="Which channel should we save in the scripts? Example: CH1,CH2,CH3")
+    parser.add_argument("--save_name", type=str, default='waveform_plot',
+                        help="header of saved figures")
+
+    args = parser.parse_args()
+    print("All parameters get from commandline are:")
+    print(args)
+
+    input_rootfile = args.input_rootfile
+    index_you_want_to_plot = args.index_you_want_to_plot
+    n_plot_waveforms = args.n_plot_waveforms
+    plot_channels = args.plot_channels
+    save_name = args.save_name
+
+    # Init
+    my_tree_waveforms = Tree_waveform(
+        input_filename=input_rootfile, list_channels=plot_channels)
+    for i in range(index_you_want_to_plot, index_you_want_to_plot+n_plot_waveforms):
+        my_tree_waveforms.my_GetEntry(i)
+        my_tree_waveforms.Plot_this_entry(
+            save_name='{0}-{1}.png'.format(save_name, str(i)))
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/Transform_csv_to_tree.py` & `oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/Transform_csv_to_tree.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-#! /usr/bin/env python
-# Author: Zifeng Xu
-# email: zifeng.xu@cern.ch
-# Usage: Use this scripts to transform different channels with many output to one TTree
-# Example: python Transform_csv_to_tree.py this_is_an_example.root input_dir input_file_name this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --n_max_points 2000
-# Use pandas to readcsv file, and them use pyroot to write a tree
-
-import argparse
-
-import ROOT as R
-import pandas as pd
-# import matplotlib.pyplot as plt
-import numpy as np
-
-parser = argparse.ArgumentParser(
-    description="Use this script to transform csv files to TTree. Author: Zifeng XU, email: zifeng.xu@cern.ch")
-
-parser.add_argument("output_filename", type=str,
-                    help="Output file name")
-parser.add_argument("input_dir", type=str,
-                    help="Dir to input files, for example: ~/inputfiles/")
-parser.add_argument("input_file_name", type=str,
-                    help="The begin part of the input file name, For example: suppose you have a set of input files named test-CH1-1.csv, the input_file_name is test")
-parser.add_argument("--n_save_waveforms", type=int, default=10,
-                    help="N_Waveforms save in the output scripts")
-parser.add_argument("--save_channels", type=str, default="CH1,CH2",
-                    help="Which channel should we save in the scripts? Example: CH1,CH2")
-parser.add_argument("--n_max_points", type=int, default=2000,
-                    help="Max save points for one saved waveform")
-
-args = parser.parse_args()
-print("All parameters get from commandline are:")
-print(args)
-
-output_filename = args.output_filename
-input_dir = args.input_dir
-input_file_name = args.input_file_name
-n_save_waveforms = args.n_save_waveforms
-save_channels = args.save_channels
-n_max_points = args.n_max_points
-
-# Open a TFile to save TTrees
-file_output = R.TFile.Open("{0}".format(output_filename), "RECREATE")
-# Open a TFile to save TTree
-dic_trees = {}
-dic_arrays = {}
-for channel in save_channels.split(","):
-    dic_trees[channel] = R.TTree(
-        "tree_waveform_{0}".format(channel), "A tree save channel {0} wave form data and size of each measurment".format(channel))
-    dic_arrays["{0}_size".format(channel)] = np.zeros(1, dtype=int)
-    dic_arrays["{0}_time".format(channel)] = np.zeros(
-        n_max_points, dtype=float)
-    dic_arrays["{0}_voltage".format(channel)] = np.zeros(
-        n_max_points, dtype=float)
-    dic_trees[channel].Branch("size".format(
-        channel), dic_arrays["{0}_size".format(channel)], "size/I".format(channel))
-    dic_trees[channel].Branch("time".format(channel), dic_arrays["{0}_time".format(
-        channel)], "time[{1}]/D".format(channel, str(n_max_points)))
-    dic_trees[channel].Branch("voltage".format(
-        channel), dic_arrays["{0}_voltage".format(channel)], "voltage[{1}]/D".format(channel, str(n_max_points)))
-for channel in save_channels.split(","):
-    dic_trees[channel].Print()
-    dic_trees[channel].Show()
-# Loop over all inputfiles
-for n_waveform in range(0, n_save_waveforms):
-    # Loop all channels
-    for channel in save_channels.split(","):
-        # Use pandas to open the file
-        df_inputfile = pd.read_csv("{0}{1}-{2}-{3}.csv".format(
-            input_dir, input_file_name, channel, str(n_waveform)), sep=",")
-        # print("DEBUG {0}".format(str(df_inputfile)))
-        # print(df_inputfile)
-        # TODO: check if NaN exist in the file, if exist ,warning and change the Nan to 0.0
-        i = 0
-        # Save max to n_max_points points, or just the len(df_inputfile[used_colums[0]])points
-        if(len(df_inputfile['scaled_time']) <= n_max_points):
-            length_to_save = len(df_inputfile['scaled_time'])
-        else:
-            print("WARNING The lenght of colums in data is larger than the n_max_points, you may miss some data points now!")
-            length_to_save = n_max_points
-        # print("DEBUG length to save is {0}".format(str(length_to_save)))
-        dic_arrays["{0}_size".format(channel)][0] = length_to_save
-        # Copy the data one by one to the
-        while i < length_to_save:
-            dic_arrays["{0}_time".format(
-                channel)][i] = df_inputfile['scaled_time'][i]
-            dic_arrays["{0}_voltage".format(
-                channel)][i] = df_inputfile['scaled_voltage'][i]
-            i = i+1
-        # print("DEBUG ",end="")
-        # print(dic_arrays["{0}_time".format(
-        #         channel)])
-        # print("DEBUG ",end="")
-        # print(dic_arrays["{0}_voltage".format(
-        #         channel)])
-        dic_trees[channel].Fill()
-        print("INFO Fill tree for " + "{0}{1}-{2}-{3}.csv".format(
-            input_dir, input_file_name, channel, str(n_waveform)))
-
-file_output.cd()
-# Write all the trees into TFile
-for channel in save_channels.split(","):
-    dic_trees[channel].Write()
-    print("INFO Write tree for {0}, totally n_files is {1}".format(
-        channel, n_save_waveforms))
-file_output.Close()
-print("INFO Finish all jobs")
+#! /usr/bin/env python
+# Author: Zifeng Xu
+# email: zifeng.xu@cern.ch
+# Usage: Use this scripts to transform different channels with many output to one TTree
+# Example: python Transform_csv_to_tree.py this_is_an_example.root input_dir input_file_name this_is_an_example --n_save_waveforms 5 --save_channels CH1,CH2 --n_max_points 2000
+# Use pandas to readcsv file, and them use pyroot to write a tree
+
+import argparse
+
+import ROOT as R
+import pandas as pd
+# import matplotlib.pyplot as plt
+import numpy as np
+
+parser = argparse.ArgumentParser(
+    description="Use this script to transform csv files to TTree. Author: Zifeng XU, email: zifeng.xu@cern.ch")
+
+parser.add_argument("output_filename", type=str,
+                    help="Output file name")
+parser.add_argument("input_dir", type=str,
+                    help="Dir to input files, for example: ~/inputfiles/")
+parser.add_argument("input_file_name", type=str,
+                    help="The begin part of the input file name, For example: suppose you have a set of input files named test-CH1-1.csv, the input_file_name is test")
+parser.add_argument("--n_save_waveforms", type=int, default=10,
+                    help="N_Waveforms save in the output scripts")
+parser.add_argument("--save_channels", type=str, default="CH1,CH2",
+                    help="Which channel should we save in the scripts? Example: CH1,CH2")
+parser.add_argument("--n_max_points", type=int, default=2000,
+                    help="Max save points for one saved waveform")
+
+args = parser.parse_args()
+print("All parameters get from commandline are:")
+print(args)
+
+output_filename = args.output_filename
+input_dir = args.input_dir
+input_file_name = args.input_file_name
+n_save_waveforms = args.n_save_waveforms
+save_channels = args.save_channels
+n_max_points = args.n_max_points
+
+# Open a TFile to save TTrees
+file_output = R.TFile.Open("{0}".format(output_filename), "RECREATE")
+# Open a TFile to save TTree
+dic_trees = {}
+dic_arrays = {}
+for channel in save_channels.split(","):
+    dic_trees[channel] = R.TTree(
+        "tree_waveform_{0}".format(channel), "A tree save channel {0} wave form data and size of each measurment".format(channel))
+    dic_arrays["{0}_size".format(channel)] = np.zeros(1, dtype=int)
+    dic_arrays["{0}_time".format(channel)] = np.zeros(
+        n_max_points, dtype=float)
+    dic_arrays["{0}_voltage".format(channel)] = np.zeros(
+        n_max_points, dtype=float)
+    dic_trees[channel].Branch("size".format(
+        channel), dic_arrays["{0}_size".format(channel)], "size/I".format(channel))
+    dic_trees[channel].Branch("time".format(channel), dic_arrays["{0}_time".format(
+        channel)], "time[{1}]/D".format(channel, str(n_max_points)))
+    dic_trees[channel].Branch("voltage".format(
+        channel), dic_arrays["{0}_voltage".format(channel)], "voltage[{1}]/D".format(channel, str(n_max_points)))
+for channel in save_channels.split(","):
+    dic_trees[channel].Print()
+    dic_trees[channel].Show()
+# Loop over all inputfiles
+for n_waveform in range(0, n_save_waveforms):
+    # Loop all channels
+    for channel in save_channels.split(","):
+        # Use pandas to open the file
+        df_inputfile = pd.read_csv("{0}{1}-{2}-{3}.csv".format(
+            input_dir, input_file_name, channel, str(n_waveform)), sep=",")
+        # print("DEBUG {0}".format(str(df_inputfile)))
+        # print(df_inputfile)
+        # TODO: check if NaN exist in the file, if exist ,warning and change the Nan to 0.0
+        i = 0
+        # Save max to n_max_points points, or just the len(df_inputfile[used_colums[0]])points
+        if(len(df_inputfile['scaled_time']) <= n_max_points):
+            length_to_save = len(df_inputfile['scaled_time'])
+        else:
+            print("WARNING The lenght of colums in data is larger than the n_max_points, you may miss some data points now!")
+            length_to_save = n_max_points
+        # print("DEBUG length to save is {0}".format(str(length_to_save)))
+        dic_arrays["{0}_size".format(channel)][0] = length_to_save
+        # Copy the data one by one to the
+        while i < length_to_save:
+            dic_arrays["{0}_time".format(
+                channel)][i] = df_inputfile['scaled_time'][i]
+            dic_arrays["{0}_voltage".format(
+                channel)][i] = df_inputfile['scaled_voltage'][i]
+            i = i+1
+        # print("DEBUG ",end="")
+        # print(dic_arrays["{0}_time".format(
+        #         channel)])
+        # print("DEBUG ",end="")
+        # print(dic_arrays["{0}_voltage".format(
+        #         channel)])
+        dic_trees[channel].Fill()
+        print("INFO Fill tree for " + "{0}{1}-{2}-{3}.csv".format(
+            input_dir, input_file_name, channel, str(n_waveform)))
+
+file_output.cd()
+# Write all the trees into TFile
+for channel in save_channels.split(","):
+    dic_trees[channel].Write()
+    print("INFO Write tree for {0}, totally n_files is {1}".format(
+        channel, n_save_waveforms))
+file_output.Close()
+print("INFO Finish all jobs")
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/UseWorkspaceForFit.C` & `oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/UseWorkspaceForFit.C`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,188 +1,188 @@
-#include "RooRealVar.h"
-#include "RooDataSet.h"
-#include "RooGaussian.h"
-#include "RooPoisson.h"
-#include "RooConstVar.h"
-#include "RooChebychev.h"
-#include "RooFormulaVar.h"
-
-#include "RooAddPdf.h"
-#include "RooProdPdf.h"
-#include "RooWorkspace.h"
-#include "RooPlot.h"
-#include "TCanvas.h"
-#include "TAxis.h"
-#include "TFile.h"
-#include "TH1.h"
-#include <vector>
-using namespace RooFit;
-
-// Two peak and three peak no shift model is valid for this experiment, please use it to obtain Gain.
-// Shift model is not available now!
-int UseWorkspaceForFit(TString input_file = "gainFitWorkspace.root")
-{
-
-    auto f1 = TFile::Open(input_file, "read");
-    auto f2 = TFile::Open("output_charge.root", "READ");
-    // charge, include baseline
-    auto h1 = (TH1F *)f2->Get("ahisto");
-    // charge, deduct baseline
-    auto h1_shift = (TH1F*)f2->Get("ahisto_shift");
-
-    // Get all workspace
-    auto wTwo = (RooWorkspace *)f1->Get("worksapceTwoPeak");
-    auto wThree = (RooWorkspace *)f1->Get("workspaceThreePeak");
-    auto wFour = (RooWorkspace *)f1->Get("workspaceFourPeak");
-    auto wFive = (RooWorkspace *)f1->Get("workspaceFivePeak");
-    auto wSix = (RooWorkspace *)f1->Get("workspaceSixPeak");
-
-    // // three peak
-    // auto threePeakGaus = wThree->pdf("threePeakGaus");
-    // auto voltage1 = wThree->var("voltage1");
-    // // auto mean1 = wThree->var("mean1");
-    // // auto mean2 = wThree->var("mean2");
-    // // auto mean3 = wThree->var("mean3");
-    // auto data1 = wThree->data("toydataThreePeak1");
-
-    // auto c1 = new TCanvas();
-    // auto frame_voltage1 = voltage1->frame();
-    // data1->plotOn(frame_voltage1);
-    // threePeakGaus->fitTo(*data1);
-    // threePeakGaus->plotOn(frame_voltage1);
-    // frame_voltage1->Draw();
-    // gPad->Update();
-
-    // // four peak
-    // auto fourPeakGaus = wFour->pdf("fourPeakGaus");
-    // auto voltage2 = wFour->var("voltage2");
-    // // auto mean1 = wThree->var("mean1");
-    // // auto mean2 = wThree->var("mean2");
-    // // auto mean3 = wThree->var("mean3");
-    // // auto mean4 = wThree->var("mean4");
-    // auto data2 = wFour->data("toydataFourPeak1");
-    // gPad->Update();
-
-    // auto c2 = new TCanvas();
-    // auto frame_voltage2 = voltage2->frame();
-    // data2->plotOn(frame_voltage2);
-    // fourPeakGaus->fitTo(*data2);
-    // fourPeakGaus->plotOn(frame_voltage2);
-    // frame_voltage2->Draw();
-    // gPad->Update();
-
-    // // five peak
-    // auto fivePeakGaus = wFive->pdf("fivePeakGaus");
-    // auto voltage3 = wFive->var("voltage3");
-    // // auto mean1 = wThree->var("mean1");
-    // // auto mean2 = wThree->var("mean2");
-    // // auto mean3 = wThree->var("mean3");
-    // // auto mean4 = wThree->var("mean4");
-    // // auto mean5 = wThree->var("mean5");
-    // auto data3 = wFive->data("toydataFivePeak1");
-
-    // auto c3 = new TCanvas();
-    // auto frame_voltage3 = voltage3->frame();
-    // data3->plotOn(frame_voltage3);
-    // fivePeakGaus->fitTo(*data3);
-    // fivePeakGaus->plotOn(frame_voltage3);
-    // frame_voltage3->Draw();
-    // gPad->Update();
-
-    // // six peak
-    // auto sixPeakGaus = wSix->pdf("sixPeakGaus");
-    // auto voltage4 = wSix->var("voltage4");
-    // // auto mean1 = wSix->var("mean1");
-    // // auto mean2 = wSix->var("mean2");
-    // // auto mean3 = wSix->var("mean3");
-    // // auto mean4 = wSix->var("mean4");
-    // // auto mean5 = wSix->var("mean5");
-    // // auto mean6 = wSix->var("mean6");
-    // auto data4 = wSix->data("toydataSixPeak1");
-
-    // auto c4 = new TCanvas();
-    // auto frame_voltage4 = voltage4->frame();
-    // data4->plotOn(frame_voltage4);
-    // sixPeakGaus->fitTo(*data4);
-    // sixPeakGaus->plotOn(frame_voltage4);
-    // frame_voltage4->Draw();
-    // gPad->Update();
-
-    // two peak
-    auto twoPeakGaus = wTwo->pdf("twoPeakGaus");
-    auto voltage0= wTwo->var("voltage0");
-    voltage0->setRange(-5200., -4700.);
-    auto mean0_1 = wTwo->var("mean1");
-    // mean0_1->setRange(-4860., -4850.);
-    mean0_1->setVal(-5120.);
-    auto mean0_2 = wTwo->var("mean2");
-    // mean0_2->setRange(-5160., -5120.);
-    mean0_2->setVal(-5140.);
-    RooDataHist data0("data0", "data0", *voltage0, h1);
-    auto c12 = new TCanvas();
-    auto frame_voltage0= voltage0->frame();
-    data0.plotOn(frame_voltage0);
-    twoPeakGaus->chi2FitTo(data0,PrintEvalErrors(10));
-    twoPeakGaus->plotOn(frame_voltage0);
-    frame_voltage0->Draw();
-    gPad->Update();
-
-
-    // // three peak
-    // auto threePeakGaus = wThree->pdf("threePeakGaus");
-    // auto voltage1= wThree->var("voltage1");
-    // voltage1->setRange(-5200., -4700.);
-    // auto mean1_1 = wThree->var("mean1");
-    // // mean1_1->setRange(-5120., -5100.);
-    // mean1_1->setVal(-5120.);
-    // auto mean1_2 = wThree->var("mean2");
-    // // mean1_2->setRange(-5160., -5120.);
-    // mean1_2->setVal(-5130.); 
-    // auto mean1_3 = wThree->var("mean3");
-    // // mean1_3->setRange(-5200., -5100.);
-    // // mean1_3->setVal(-5140.);
-    // // auto gaus1 = wThree->pdf("gaus1ThreePeak");
-    // // auto n1 = wThree->var("n1");
-    // // auto gaus2 = wThree->pdf("gaus2ThreePeak");
-    // // auto n2 = wThree->var("n2");
-    // // auto gaus3 = wThree->pdf("gaus3ThreePeak");
-    // // auto n3 = wThree->var("n3");
-    // RooDataHist data1("data1", "data1", *voltage1, h1);
-    // auto c13 = new TCanvas();
-    // auto frame_voltage1= voltage1->frame();
-    // data1.plotOn(frame_voltage1);
-    // threePeakGaus->fitTo(data1,PrintEvalErrors(10));
-    // threePeakGaus->plotOn(frame_voltage1);
-    // threePeakGaus->plotOn(frame_voltage1, Components("gaus1ThreePeak"), LineColor(kRed), LineStyle(kDashed));
-    // threePeakGaus->plotOn(frame_voltage1, Components("gaus2ThreePeak"), LineColor(kBlue), LineStyle(kDashed));
-    // threePeakGaus->plotOn(frame_voltage1, Components("gaus3ThreePeak"), LineColor(kGreen), LineStyle(kDashed));
-    // frame_voltage1->Draw();
-    // gPad->Update();
-
-    // three peak deduct baseline
-    auto threePeakGaus = wThree->pdf("threePeakGaus");
-    auto voltage1= wThree->var("voltage1");
-    voltage1->setRange(-500., 100.);
-    auto mean1_1 = wThree->var("mean1");
-    mean1_1->setRange(-100., 0.);
-    mean1_1->setVal(-10.);
-    auto mean1_2 = wThree->var("mean2");
-    mean1_2->setRange(-100., 0.);
-    mean1_2->setVal(-10.); 
-    auto mean1_3 = wThree->var("mean3");
-    mean1_3->setRange(-100., -0.);
-    mean1_3->setVal(-10.);
-    auto n3 = wThree->var("n3");
-    RooDataHist data1("data1", "data1", *voltage1, h1_shift);
-    auto c13 = new TCanvas();
-    auto frame_voltage1= voltage1->frame();
-    data1.plotOn(frame_voltage1);
-    threePeakGaus->fitTo(data1,PrintEvalErrors(10));
-    threePeakGaus->plotOn(frame_voltage1);
-    threePeakGaus->plotOn(frame_voltage1, Components("gaus1ThreePeak"), LineColor(kRed), LineStyle(kDashed));
-    threePeakGaus->plotOn(frame_voltage1, Components("gaus2ThreePeak"), LineColor(kBlue), LineStyle(kDashed));
-    threePeakGaus->plotOn(frame_voltage1, Components("gaus3ThreePeak"), LineColor(kGreen), LineStyle(kDashed));
-    frame_voltage1->Draw();
-    gPad->Update();
-
-    return 0;
-}
+#include "RooRealVar.h"
+#include "RooDataSet.h"
+#include "RooGaussian.h"
+#include "RooPoisson.h"
+#include "RooConstVar.h"
+#include "RooChebychev.h"
+#include "RooFormulaVar.h"
+
+#include "RooAddPdf.h"
+#include "RooProdPdf.h"
+#include "RooWorkspace.h"
+#include "RooPlot.h"
+#include "TCanvas.h"
+#include "TAxis.h"
+#include "TFile.h"
+#include "TH1.h"
+#include <vector>
+using namespace RooFit;
+
+// Two peak and three peak no shift model is valid for this experiment, please use it to obtain Gain.
+// Shift model is not available now!
+int UseWorkspaceForFit(TString input_file = "gainFitWorkspace.root")
+{
+
+    auto f1 = TFile::Open(input_file, "read");
+    auto f2 = TFile::Open("output_charge.root", "READ");
+    // charge, include baseline
+    auto h1 = (TH1F *)f2->Get("ahisto");
+    // charge, deduct baseline
+    auto h1_shift = (TH1F*)f2->Get("ahisto_shift");
+
+    // Get all workspace
+    auto wTwo = (RooWorkspace *)f1->Get("worksapceTwoPeak");
+    auto wThree = (RooWorkspace *)f1->Get("workspaceThreePeak");
+    auto wFour = (RooWorkspace *)f1->Get("workspaceFourPeak");
+    auto wFive = (RooWorkspace *)f1->Get("workspaceFivePeak");
+    auto wSix = (RooWorkspace *)f1->Get("workspaceSixPeak");
+
+    // // three peak
+    // auto threePeakGaus = wThree->pdf("threePeakGaus");
+    // auto voltage1 = wThree->var("voltage1");
+    // // auto mean1 = wThree->var("mean1");
+    // // auto mean2 = wThree->var("mean2");
+    // // auto mean3 = wThree->var("mean3");
+    // auto data1 = wThree->data("toydataThreePeak1");
+
+    // auto c1 = new TCanvas();
+    // auto frame_voltage1 = voltage1->frame();
+    // data1->plotOn(frame_voltage1);
+    // threePeakGaus->fitTo(*data1);
+    // threePeakGaus->plotOn(frame_voltage1);
+    // frame_voltage1->Draw();
+    // gPad->Update();
+
+    // // four peak
+    // auto fourPeakGaus = wFour->pdf("fourPeakGaus");
+    // auto voltage2 = wFour->var("voltage2");
+    // // auto mean1 = wThree->var("mean1");
+    // // auto mean2 = wThree->var("mean2");
+    // // auto mean3 = wThree->var("mean3");
+    // // auto mean4 = wThree->var("mean4");
+    // auto data2 = wFour->data("toydataFourPeak1");
+    // gPad->Update();
+
+    // auto c2 = new TCanvas();
+    // auto frame_voltage2 = voltage2->frame();
+    // data2->plotOn(frame_voltage2);
+    // fourPeakGaus->fitTo(*data2);
+    // fourPeakGaus->plotOn(frame_voltage2);
+    // frame_voltage2->Draw();
+    // gPad->Update();
+
+    // // five peak
+    // auto fivePeakGaus = wFive->pdf("fivePeakGaus");
+    // auto voltage3 = wFive->var("voltage3");
+    // // auto mean1 = wThree->var("mean1");
+    // // auto mean2 = wThree->var("mean2");
+    // // auto mean3 = wThree->var("mean3");
+    // // auto mean4 = wThree->var("mean4");
+    // // auto mean5 = wThree->var("mean5");
+    // auto data3 = wFive->data("toydataFivePeak1");
+
+    // auto c3 = new TCanvas();
+    // auto frame_voltage3 = voltage3->frame();
+    // data3->plotOn(frame_voltage3);
+    // fivePeakGaus->fitTo(*data3);
+    // fivePeakGaus->plotOn(frame_voltage3);
+    // frame_voltage3->Draw();
+    // gPad->Update();
+
+    // // six peak
+    // auto sixPeakGaus = wSix->pdf("sixPeakGaus");
+    // auto voltage4 = wSix->var("voltage4");
+    // // auto mean1 = wSix->var("mean1");
+    // // auto mean2 = wSix->var("mean2");
+    // // auto mean3 = wSix->var("mean3");
+    // // auto mean4 = wSix->var("mean4");
+    // // auto mean5 = wSix->var("mean5");
+    // // auto mean6 = wSix->var("mean6");
+    // auto data4 = wSix->data("toydataSixPeak1");
+
+    // auto c4 = new TCanvas();
+    // auto frame_voltage4 = voltage4->frame();
+    // data4->plotOn(frame_voltage4);
+    // sixPeakGaus->fitTo(*data4);
+    // sixPeakGaus->plotOn(frame_voltage4);
+    // frame_voltage4->Draw();
+    // gPad->Update();
+
+    // two peak
+    auto twoPeakGaus = wTwo->pdf("twoPeakGaus");
+    auto voltage0= wTwo->var("voltage0");
+    voltage0->setRange(-5200., -4700.);
+    auto mean0_1 = wTwo->var("mean1");
+    // mean0_1->setRange(-4860., -4850.);
+    mean0_1->setVal(-5120.);
+    auto mean0_2 = wTwo->var("mean2");
+    // mean0_2->setRange(-5160., -5120.);
+    mean0_2->setVal(-5140.);
+    RooDataHist data0("data0", "data0", *voltage0, h1);
+    auto c12 = new TCanvas();
+    auto frame_voltage0= voltage0->frame();
+    data0.plotOn(frame_voltage0);
+    twoPeakGaus->chi2FitTo(data0,PrintEvalErrors(10));
+    twoPeakGaus->plotOn(frame_voltage0);
+    frame_voltage0->Draw();
+    gPad->Update();
+
+
+    // // three peak
+    // auto threePeakGaus = wThree->pdf("threePeakGaus");
+    // auto voltage1= wThree->var("voltage1");
+    // voltage1->setRange(-5200., -4700.);
+    // auto mean1_1 = wThree->var("mean1");
+    // // mean1_1->setRange(-5120., -5100.);
+    // mean1_1->setVal(-5120.);
+    // auto mean1_2 = wThree->var("mean2");
+    // // mean1_2->setRange(-5160., -5120.);
+    // mean1_2->setVal(-5130.); 
+    // auto mean1_3 = wThree->var("mean3");
+    // // mean1_3->setRange(-5200., -5100.);
+    // // mean1_3->setVal(-5140.);
+    // // auto gaus1 = wThree->pdf("gaus1ThreePeak");
+    // // auto n1 = wThree->var("n1");
+    // // auto gaus2 = wThree->pdf("gaus2ThreePeak");
+    // // auto n2 = wThree->var("n2");
+    // // auto gaus3 = wThree->pdf("gaus3ThreePeak");
+    // // auto n3 = wThree->var("n3");
+    // RooDataHist data1("data1", "data1", *voltage1, h1);
+    // auto c13 = new TCanvas();
+    // auto frame_voltage1= voltage1->frame();
+    // data1.plotOn(frame_voltage1);
+    // threePeakGaus->fitTo(data1,PrintEvalErrors(10));
+    // threePeakGaus->plotOn(frame_voltage1);
+    // threePeakGaus->plotOn(frame_voltage1, Components("gaus1ThreePeak"), LineColor(kRed), LineStyle(kDashed));
+    // threePeakGaus->plotOn(frame_voltage1, Components("gaus2ThreePeak"), LineColor(kBlue), LineStyle(kDashed));
+    // threePeakGaus->plotOn(frame_voltage1, Components("gaus3ThreePeak"), LineColor(kGreen), LineStyle(kDashed));
+    // frame_voltage1->Draw();
+    // gPad->Update();
+
+    // three peak deduct baseline
+    auto threePeakGaus = wThree->pdf("threePeakGaus");
+    auto voltage1= wThree->var("voltage1");
+    voltage1->setRange(-500., 100.);
+    auto mean1_1 = wThree->var("mean1");
+    mean1_1->setRange(-100., 0.);
+    mean1_1->setVal(-10.);
+    auto mean1_2 = wThree->var("mean2");
+    mean1_2->setRange(-100., 0.);
+    mean1_2->setVal(-10.); 
+    auto mean1_3 = wThree->var("mean3");
+    mean1_3->setRange(-100., -0.);
+    mean1_3->setVal(-10.);
+    auto n3 = wThree->var("n3");
+    RooDataHist data1("data1", "data1", *voltage1, h1_shift);
+    auto c13 = new TCanvas();
+    auto frame_voltage1= voltage1->frame();
+    data1.plotOn(frame_voltage1);
+    threePeakGaus->fitTo(data1,PrintEvalErrors(10));
+    threePeakGaus->plotOn(frame_voltage1);
+    threePeakGaus->plotOn(frame_voltage1, Components("gaus1ThreePeak"), LineColor(kRed), LineStyle(kDashed));
+    threePeakGaus->plotOn(frame_voltage1, Components("gaus2ThreePeak"), LineColor(kBlue), LineStyle(kDashed));
+    threePeakGaus->plotOn(frame_voltage1, Components("gaus3ThreePeak"), LineColor(kGreen), LineStyle(kDashed));
+    frame_voltage1->Draw();
+    gPad->Update();
+
+    return 0;
+}
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/analysis_waveform_data.py` & `oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/analysis_waveform_data.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-#!/usr/bin/env python
-# Author: Zifeng Xu
-# Email: zifeng.xu@cern.ch
-# Usage: Use this interface to get charge and max voltage in waveform
-
-
-import argparse
-import sys
-
-import numpy as np
-# import matplotlib
-# matplotlib.use('TkAgg')
-# import matplotlib.pyplot as plt
-import ROOT
-
-def RunSelector(input_TFile, channels='CH1,CH2,CH3', output_filename='output_filename'):
-
-    list_channel = channels.split(',')
-
-    for _channel in list_channel:
-        try:
-            tree=input_TFile.Get("tree_waveform_{0}".format(_channel))
-        except:
-            print("tree_waveform_{0} is not exist".format(_channel))
-        tree.Process("single_channel_selector.C+", "{1}_{0}.root".format(_channel, output_filename))
-
-    return 0
-
-def RunAnalysis(channels='CH1,CH2,CH3', input_filename='output_filename', min_trig_level_cut=0.0):
-
-    dic_TFile = {}
-    dic_tree = {}
-    list_channels = channels.split(',')
-    for _channel in list_channels:
-
-        try:
-            ROOT.TFile.Open("{0}_{1}.root".format(input_filename, _channel))
-        except:
-            print("{0}_{1}.root".format(input_filename, _channel))
-
-    # Check the length of these trees
-
-    return 0
-
- 
-input_TFile=ROOT.TFile.Open("./waveform_data_root/channel2_trig_n3p00.root", "READ")
-RunSelector(input_TFile, "CH1,CH2,CH3", output_filename='channel2_trig_n3p00_cut_charge_n4400_level_n2p68')
-# RunAnalysis(channels='CH1,CH2', input_filename='output_filename')
+#!/usr/bin/env python
+# Author: Zifeng Xu
+# Email: zifeng.xu@cern.ch
+# Usage: Use this interface to get charge and max voltage in waveform
+
+
+import argparse
+import sys
+
+import numpy as np
+# import matplotlib
+# matplotlib.use('TkAgg')
+# import matplotlib.pyplot as plt
+import ROOT
+
+def RunSelector(input_TFile, channels='CH1,CH2,CH3', output_filename='output_filename'):
+
+    list_channel = channels.split(',')
+
+    for _channel in list_channel:
+        try:
+            tree=input_TFile.Get("tree_waveform_{0}".format(_channel))
+        except:
+            print("tree_waveform_{0} is not exist".format(_channel))
+        tree.Process("single_channel_selector.C+", "{1}_{0}.root".format(_channel, output_filename))
+
+    return 0
+
+def RunAnalysis(channels='CH1,CH2,CH3', input_filename='output_filename', min_trig_level_cut=0.0):
+
+    dic_TFile = {}
+    dic_tree = {}
+    list_channels = channels.split(',')
+    for _channel in list_channels:
+
+        try:
+            ROOT.TFile.Open("{0}_{1}.root".format(input_filename, _channel))
+        except:
+            print("{0}_{1}.root".format(input_filename, _channel))
+
+    # Check the length of these trees
+
+    return 0
+
+ 
+input_TFile=ROOT.TFile.Open("./waveform_data_root/channel2_trig_n3p00.root", "READ")
+RunSelector(input_TFile, "CH1,CH2,CH3", output_filename='channel2_trig_n3p00_cut_charge_n4400_level_n2p68')
+# RunAnalysis(channels='CH1,CH2', input_filename='output_filename')
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/naive_bayesian_classifier/Event.py` & `oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/naive_bayesian_classifier/Event.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-#!/usr/bin/env python
-# Author: Zifeng Xu
-# This is a container class for a .root file derive from single_channel_selector.C
-
-import ROOT
-import numpy as np
-# import matplotlib.pyplot as plt
-
-
-class Event():
-
-    def __init__(self, input_TFile) -> None:
-
-        self.__input_TFile = ROOT.TFile.Open(input_TFile, "READ")
-        self.m_tree_event = self.__input_TFile.Get("event")
-        self.entries = self.m_tree_event.GetEntries()
-
-        self.max_voltage = np.zeros(1, dtype=float)
-        self.width = np.zeros(1, dtype=int)
-        self.charge = np.zeros(1, dtype=float)
-        self.trig_charge = np.zeros(1, dtype=int)
-        self.pass_width = np.zeros(1, dtype=int)
-        self.trig_level = np.zeros(1, dtype=int)
-        self.__m_dic_branches= {}
-        # Add branch address here
-        self.SetBranchAddress()
-
-    def SetBranchAddress(self):
-        """
-        Add Branch Address for all branch
-        """
-        self.__m_dic_branches['max_voltage']=self.m_tree_event.SetBranchAddress("max_voltage", self.max_voltage)
-        self.__m_dic_branches['width']=self.m_tree_event.SetBranchAddress('width',self.width)
-        self.__m_dic_branches['charge']=self.m_tree_event.SetBranchAddress('charge',self.charge)
-        self.__m_dic_branches['trig_charge']=self.m_tree_event.SetBranchAddress('trig_charge',self.trig_charge)
-        self.__m_dic_branches['pass_width']=self.m_tree_event.SetBranchAddress('pass_width',self.pass_width)
-        self.__m_dic_branches['trig_level']=self.m_tree_event.SetBranchAddress('trig_level',self.trig_level)
-
+#!/usr/bin/env python
+# Author: Zifeng Xu
+# This is a container class for a .root file derive from single_channel_selector.C
+
+import ROOT
+import numpy as np
+# import matplotlib.pyplot as plt
+
+
+class Event():
+
+    def __init__(self, input_TFile) -> None:
+
+        self.__input_TFile = ROOT.TFile.Open(input_TFile, "READ")
+        self.m_tree_event = self.__input_TFile.Get("event")
+        self.entries = self.m_tree_event.GetEntries()
+
+        self.max_voltage = np.zeros(1, dtype=float)
+        self.width = np.zeros(1, dtype=int)
+        self.charge = np.zeros(1, dtype=float)
+        self.trig_charge = np.zeros(1, dtype=int)
+        self.pass_width = np.zeros(1, dtype=int)
+        self.trig_level = np.zeros(1, dtype=int)
+        self.__m_dic_branches= {}
+        # Add branch address here
+        self.SetBranchAddress()
+
+    def SetBranchAddress(self):
+        """
+        Add Branch Address for all branch
+        """
+        self.__m_dic_branches['max_voltage']=self.m_tree_event.SetBranchAddress("max_voltage", self.max_voltage)
+        self.__m_dic_branches['width']=self.m_tree_event.SetBranchAddress('width',self.width)
+        self.__m_dic_branches['charge']=self.m_tree_event.SetBranchAddress('charge',self.charge)
+        self.__m_dic_branches['trig_charge']=self.m_tree_event.SetBranchAddress('trig_charge',self.trig_charge)
+        self.__m_dic_branches['pass_width']=self.m_tree_event.SetBranchAddress('pass_width',self.pass_width)
+        self.__m_dic_branches['trig_level']=self.m_tree_event.SetBranchAddress('trig_level',self.trig_level)
+
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/naive_bayesian_classifier/naive_bayesian_classifier.py` & `oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/naive_bayesian_classifier/naive_bayesian_classifier_CH2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-#!/usr/bin/env python
-# Author: Zifeng Xu
-# This scripts aim to train the classifier use 7000 data, and use the classifier to predict.
-# Also, the confusion matrix.
-
-from Event import Event as Ev
-import numpy as np
-import ROOT
-ROOT.gROOT.SetBatch(True)
-ROOT.gROOT.SetStyle("ATLAS")
-# import matplotlib.pyplot as plt
-
-LAMBDA = 1.0
-train_set = 7000
-test_set = 3000
-# Init all event we need
-event_CH1 = Ev('../channel2_trig_n3p00_cut_charge_n4400_level_n2p68_CH1.root')
-event_CH2 = Ev('../channel2_trig_n3p00_cut_charge_n4400_level_n2p68_CH2.root')
-event_CH3 = Ev('../channel2_trig_n3p00_cut_charge_n4400_level_n2p68_CH3.root')
-
-# Use 0-6999 to learn, use 7000-9999 to test
-
-
-charge_bin_x = np.array([-4950., -4860., -4845., -4800])
-width_binx = np.array([274., 294., 300., 303.])
-# max_voltage_binx = np.array([-5.5, -2.4, -2.3])
-
-dic_hist = {}
-# Train
-h_charge_sig = ROOT.TH1F("charge_sig", "charge_sig",
-                         len(charge_bin_x) - 1, charge_bin_x)
-h_charge_bkg = ROOT.TH1F("charge_bkg", "charge_bkg",
-                         len(charge_bin_x) - 1, charge_bin_x)
-h_width_sig = ROOT.TH1I("width_sig", "width_sig",
-                        len(width_binx)-1, width_binx)
-h_width_bkg = ROOT.TH1I("width_bkg", "width_bkg",
-                        len(width_binx)-1, width_binx)
-# h_max_voltage_sig = ROOT.TH1F("max_voltage_sig", "max_voltage_sig", len(
-#     max_voltage_binx)-1, max_voltage_binx)
-# h_max_voltage_bkg = ROOT.TH1F("max_voltage_bkg", "max_voltage_bkg", len(
-#     max_voltage_binx)-1, max_voltage_binx)
-dic_hist['bkg'] = {'charge': h_charge_bkg,
-                   'width': h_width_bkg}
-dic_hist['sig'] = {'charge': h_charge_sig,
-                   'width': h_width_sig}
-# Use Maximum Likelihood estimate parameters
-# Just fill the histogram first
-for i in range(6999, 10000):
-    # GetEntry
-    event_CH1.m_tree_event.GetEntry(i)
-    event_CH2.m_tree_event.GetEntry(i)
-    event_CH3.m_tree_event.GetEntry(i)
-
-    # If sig
-    if(event_CH3.trig_level[0] == 0):
-        h_charge_sig.Fill(event_CH3.charge[0])
-        h_width_sig.Fill(event_CH3.width[0])
-        # h_max_voltage_sig.Fill(event_CH3.max_voltage[0])
-    # If bkg
-    elif (event_CH3.trig_level[0] == 1):
-        h_charge_bkg.Fill(event_CH3.charge[0])
-        h_width_bkg.Fill(event_CH3.width[0])
-        # h_max_voltage_bkg.Fill(event_CH3.max_voltage[0])
-# Plot here
-# dic_canvas = {'bkg': ['charge', 'width'],
-#               'sig': ['charge', 'width']}
-# for key in dic_canvas.keys():
-#     for variable in dic_canvas[key]:
-#         _canvas=ROOT.TCanvas("test_{0}_{1}".format(key,variable),"{0}_{1}".format(key,variable),800,600)
-#         dic_hist[key][variable].Draw("hist e")
-#         ROOT.gPad.Update()
-#         _canvas.SaveAs("test_{0}_{1}.png".format(key,variable))
-
-# estimate prior probability
-dic_prior = {}
-prior_bkg = (dic_hist['bkg']['charge'].GetEntries() +
-             LAMBDA) / (float(train_set) + 2*LAMBDA)
-prior_sig = (dic_hist['sig']['charge'].GetEntries() +
-             LAMBDA) / (float(train_set) + 2*LAMBDA)
-dic_prior['bkg'] = prior_bkg
-dic_prior['sig'] = prior_sig
-
-# estimate conditional probability
-dic_condi_pro = {'bkg': {}, 'sig': {}}
-for cat in ['bkg', 'sig']:
-    for variable in ['charge', 'width']:
-        _list_condi_pro = []
-        for i in range(0, dic_hist[cat][variable].GetNbinsX()+2):
-            _list_condi_pro.append((dic_hist[cat][variable].GetBinContent(
-                i) + LAMBDA) / (dic_hist[cat][variable].GetEntries() + dic_hist[cat][variable].GetNbinsX() * LAMBDA))
-        dic_condi_pro[cat][variable] = _list_condi_pro
-
-print("/**************prior posibillity****************/")
-print(dic_prior)
-print("/**************condition posibillity****************/")
-print(dic_condi_pro)
-
-h_sig_and_bkg_train_set = ROOT.TH1I(
-    "h_sig_and_bkg_train_set", "h_sig_and_bkg_train_set", 2, 0, 2)
-h_sig_and_bkg_train_set_predict = ROOT.TH1I(
-    "h_sig_and_bkg_train_set_predict", "h_sig_and_bkg_train_set_predict", 2, 0, 2)
-dic_posterior_train_set = {'bkg': [], 'sig': []}
-# Now calculate the predict result of train dateset
-# for i in range(0, train_set + test_set):
-for i in range(0, train_set):
-    # GetEntry
-    event_CH1.m_tree_event.GetEntry(i)
-    event_CH2.m_tree_event.GetEntry(i)
-    event_CH3.m_tree_event.GetEntry(i)
-    h_sig_and_bkg_train_set.Fill(event_CH3.trig_level[0])
-    dic_posterior = {'bkg': None, 'sig': None}
-    for key in dic_hist:
-        i_bin_charge = dic_hist[key]['charge'].FindBin(event_CH3.charge[0])
-        i_bin_width = dic_hist[key]['width'].FindBin(event_CH3.width[0])
-        # i_bin_max_voltage = dic_hist[key]['max_voltage'].FindBin(
-        #     event_CH3.max_voltage[0])
-        condi_pro_charge = dic_condi_pro[key]['charge'][i_bin_charge]
-        condi_pro_width = dic_condi_pro[key]['width'][i_bin_width]
-        # condi_pro_max_voltage = dic_condi_pro[key]['max_voltage'][i_bin_max_voltage]
-        # calculate posterior
-        dic_posterior[key] = dic_prior[key] * condi_pro_charge * \
-            condi_pro_width * 1#condi_pro_max_voltage
-    dic_posterior_train_set['sig'].append(dic_posterior['sig'])
-    dic_posterior_train_set['bkg'].append(dic_posterior['bkg'])
-    if(dic_posterior['sig'] >= dic_posterior['bkg'] and event_CH3.trig_level[0] == 0):
-        h_sig_and_bkg_train_set_predict.Fill(0)
-    elif (dic_posterior['sig'] < dic_posterior['bkg'] and event_CH3.trig_level[0] == 1):
-        h_sig_and_bkg_train_set_predict.Fill(1)
-
-
-print("/**************posterior posibbility for train set****************/")
-for i in range(0, len(dic_posterior_train_set['bkg'])):
-    print("bkg: {0:f}, sig: {1:f}".format(
-        dic_posterior_train_set['bkg'][i], dic_posterior_train_set['sig'][i]))
-print("truth sig: {0}".format(h_sig_and_bkg_train_set.GetBinContent(1)))
-print("truth bkg:{0}".format(h_sig_and_bkg_train_set.GetBinContent(2)))
-print("pred sig: {0}".format(h_sig_and_bkg_train_set_predict.GetBinContent(1)))
-print("pred bkg:{0}".format(h_sig_and_bkg_train_set_predict.GetBinContent(2)))
-
-
-h_sig_and_bkg_test_set = ROOT.TH1I(
-    "h_sig_and_bkg_test_set", "h_sig_and_bkg_test_set", 2, 0, 2)
-h_sig_and_bkg_test_set_predict = ROOT.TH1I(
-    "h_sig_and_bkg_test_set_predict", "h_sig_and_bkg_test_set_predict", 2, 0, 2)
-dic_posterior_test_set = {'bkg': [], 'sig': []}
-# Now calculate the predict result of train dateset
-# for i in range(0, train_set + test_set):
-for i in range(train_set, train_set + test_set):
-    # GetEntry
-    event_CH1.m_tree_event.GetEntry(i)
-    event_CH2.m_tree_event.GetEntry(i)
-    event_CH3.m_tree_event.GetEntry(i)
-    h_sig_and_bkg_test_set.Fill(event_CH3.trig_level[0])
-    dic_posterior = {'bkg': None, 'sig': None}
-    for key in dic_hist:
-        i_bin_charge = dic_hist[key]['charge'].FindBin(event_CH3.charge[0])
-        i_bin_width = dic_hist[key]['width'].FindBin(event_CH3.width[0])
-        # i_bin_max_voltage = dic_hist[key]['max_voltage'].FindBin(
-        #     event_CH3.max_voltage[0])
-        condi_pro_charge = dic_condi_pro[key]['charge'][i_bin_charge]
-        condi_pro_width = dic_condi_pro[key]['width'][i_bin_width]
-        # condi_pro_max_voltage = dic_condi_pro[key]['max_voltage'][i_bin_max_voltage]
-        # calculate posterior
-        dic_posterior[key] = dic_prior[key] * condi_pro_charge * \
-            condi_pro_width * 1#condi_pro_max_voltage
-    dic_posterior_test_set['sig'].append(dic_posterior['sig'])
-    dic_posterior_test_set['bkg'].append(dic_posterior['bkg'])
-    if(dic_posterior['sig'] >= dic_posterior['bkg'] and event_CH3.trig_level[0] == 0):
-        h_sig_and_bkg_test_set_predict.Fill(0)
-    elif (dic_posterior['sig'] < dic_posterior['bkg'] and event_CH3.trig_level[0] == 1):
-        h_sig_and_bkg_test_set_predict.Fill(1)
-
-
-print("/**************posterior posibbility for test set****************/")
-for i in range(0, len(dic_posterior_test_set['bkg'])):
-    print("bkg: {0:f}, sig: {1:f}".format(
-        dic_posterior_test_set['bkg'][i], dic_posterior_test_set['sig'][i]))
-print("truth sig: {0}".format(h_sig_and_bkg_test_set.GetBinContent(1)))
-print("truth bkg:{0}".format(h_sig_and_bkg_test_set.GetBinContent(2)))
-print("pred sig: {0}".format(h_sig_and_bkg_test_set_predict.GetBinContent(1)))
-print("pred bkg:{0}".format(h_sig_and_bkg_test_set_predict.GetBinContent(2)))
-
-
-# Calculate
+#!/usr/bin/env python
+# Author: Zifeng Xu
+# This scripts aim to train the classifier use 7000 data, and use the classifier to predict.
+# Also, the confusion matrix.
+
+from Event import Event as Ev
+import numpy as np
+import ROOT
+ROOT.gROOT.SetBatch(True)
+ROOT.gROOT.SetStyle("ATLAS")
+# import matplotlib.pyplot as plt
+
+LAMBDA = 1.0
+train_set = 7000
+test_set = 3000
+# Init all event we need
+event_CH1 = Ev('../channel2_trig_n3p00_cut_charge_n4400_level_n2p68_CH1.root')
+event_CH2 = Ev('../channel2_trig_n3p00_cut_charge_n4400_level_n2p68_CH2.root')
+event_CH3 = Ev('../channel2_trig_n3p00_cut_charge_n4400_level_n2p68_CH3.root')
+
+# Use 0-6999 to learn, use 7000-9999 to test
+
+
+charge_bin_x = np.array([-4950., -4860., -4845., -4800])
+width_binx = np.array([274., 294., 300., 303.])
+# max_voltage_binx = np.array([-5.5, -2.4, -2.3])
+
+dic_hist = {}
+# Train
+h_charge_sig = ROOT.TH1F("charge_sig", "charge_sig",
+                         len(charge_bin_x) - 1, charge_bin_x)
+h_charge_bkg = ROOT.TH1F("charge_bkg", "charge_bkg",
+                         len(charge_bin_x) - 1, charge_bin_x)
+h_width_sig = ROOT.TH1I("width_sig", "width_sig",
+                        len(width_binx)-1, width_binx)
+h_width_bkg = ROOT.TH1I("width_bkg", "width_bkg",
+                        len(width_binx)-1, width_binx)
+# h_max_voltage_sig = ROOT.TH1F("max_voltage_sig", "max_voltage_sig", len(
+#     max_voltage_binx)-1, max_voltage_binx)
+# h_max_voltage_bkg = ROOT.TH1F("max_voltage_bkg", "max_voltage_bkg", len(
+#     max_voltage_binx)-1, max_voltage_binx)
+dic_hist['bkg'] = {'charge': h_charge_bkg,
+                   'width': h_width_bkg}
+dic_hist['sig'] = {'charge': h_charge_sig,
+                   'width': h_width_sig}
+# Use Maximum Likelihood estimate parameters
+# Just fill the histogram first
+for i in range(0, train_set):
+    # GetEntry
+    event_CH1.m_tree_event.GetEntry(i)
+    event_CH2.m_tree_event.GetEntry(i)
+    event_CH3.m_tree_event.GetEntry(i)
+
+    # If sig
+    if(event_CH3.trig_level[0] == 0):
+        h_charge_sig.Fill(event_CH3.charge[0])
+        h_width_sig.Fill(event_CH3.width[0])
+        # h_max_voltage_sig.Fill(event_CH3.max_voltage[0])
+    # If bkg
+    elif (event_CH3.trig_level[0] == 1):
+        h_charge_bkg.Fill(event_CH3.charge[0])
+        h_width_bkg.Fill(event_CH3.width[0])
+        # h_max_voltage_bkg.Fill(event_CH3.max_voltage[0])
+
+# dic_canvas = {'bkg': ['charge', 'width', 'max_voltage'],
+#               'sig': ['charge', 'width', 'max_voltage']}
+# for key in dic_canvas.keys():
+#     for variable in dic_canvas[key]:
+#         _canvas=ROOT.TCanvas("train_{0}_{1}".format(key,variable),"{0}_{1}".format(key,variable),800,600)
+#         dic_hist[key][variable].Draw("hist e")
+#         ROOT.gPad.Update()
+#         _canvas.SaveAs("train_{0}_{1}.png".format(key,variable))
+
+# estimate prior probability
+dic_prior = {}
+prior_bkg = (dic_hist['bkg']['charge'].GetEntries() +
+             LAMBDA) / (float(train_set) + 2*LAMBDA)
+prior_sig = (dic_hist['sig']['charge'].GetEntries() +
+             LAMBDA) / (float(train_set) + 2*LAMBDA)
+dic_prior['bkg'] = prior_bkg
+dic_prior['sig'] = prior_sig
+
+# estimate conditional probability
+dic_condi_pro = {'bkg': {}, 'sig': {}}
+for cat in ['bkg', 'sig']:
+    for variable in ['charge', 'width']:
+        _list_condi_pro = []
+        for i in range(0, dic_hist[cat][variable].GetNbinsX()+2):
+            _list_condi_pro.append((dic_hist[cat][variable].GetBinContent(
+                i) + LAMBDA) / (dic_hist[cat][variable].GetEntries() + dic_hist[cat][variable].GetNbinsX() * LAMBDA))
+        dic_condi_pro[cat][variable] = _list_condi_pro
+
+print("/**************prior posibillity****************/")
+print(dic_prior)
+print("/**************condition posibillity****************/")
+print(dic_condi_pro)
+
+h_sig_and_bkg_train_set = ROOT.TH1I(
+    "h_sig_and_bkg_train_set", "h_sig_and_bkg_train_set", 2, 0, 2)
+h_sig_and_bkg_train_set_predict = ROOT.TH1I(
+    "h_sig_and_bkg_train_set_predict", "h_sig_and_bkg_train_set_predict", 2, 0, 2)
+dic_posterior_train_set = {'bkg': [], 'sig': []}
+# Now calculate the predict result of train dateset
+# for i in range(0, train_set + test_set):
+for i in range(0, train_set):
+    # GetEntry
+    event_CH1.m_tree_event.GetEntry(i)
+    event_CH2.m_tree_event.GetEntry(i)
+    event_CH3.m_tree_event.GetEntry(i)
+    h_sig_and_bkg_train_set.Fill(event_CH3.trig_level[0])
+    dic_posterior = {'bkg': None, 'sig': None}
+    for key in dic_hist:
+        i_bin_charge = dic_hist[key]['charge'].FindBin(event_CH3.charge[0])
+        i_bin_width = dic_hist[key]['width'].FindBin(event_CH3.width[0])
+        # i_bin_max_voltage = dic_hist[key]['max_voltage'].FindBin(
+        #     event_CH3.max_voltage[0])
+        condi_pro_charge = dic_condi_pro[key]['charge'][i_bin_charge]
+        condi_pro_width = dic_condi_pro[key]['width'][i_bin_width]
+        # condi_pro_max_voltage = dic_condi_pro[key]['max_voltage'][i_bin_max_voltage]
+        # calculate posterior
+        dic_posterior[key] = dic_prior[key] * condi_pro_charge * \
+            condi_pro_width * 1#condi_pro_max_voltage
+    dic_posterior_train_set['sig'].append(dic_posterior['sig'])
+    dic_posterior_train_set['bkg'].append(dic_posterior['bkg'])
+    if(dic_posterior['sig'] >= dic_posterior['bkg'] and event_CH3.trig_level[0] == 0):
+        h_sig_and_bkg_train_set_predict.Fill(0)
+    elif (dic_posterior['sig'] < dic_posterior['bkg'] and event_CH3.trig_level[0] == 1):
+        h_sig_and_bkg_train_set_predict.Fill(1)
+
+
+print("/**************posterior posibbility for train set****************/")
+for i in range(0, len(dic_posterior_train_set['bkg'])):
+    print("bkg: {0:f}, sig: {1:f}".format(
+        dic_posterior_train_set['bkg'][i], dic_posterior_train_set['sig'][i]))
+print("truth sig: {0}".format(h_sig_and_bkg_train_set.GetBinContent(1)))
+print("truth bkg:{0}".format(h_sig_and_bkg_train_set.GetBinContent(2)))
+print("pred sig: {0}".format(h_sig_and_bkg_train_set_predict.GetBinContent(1)))
+print("pred bkg:{0}".format(h_sig_and_bkg_train_set_predict.GetBinContent(2)))
+
+
+h_sig_and_bkg_test_set = ROOT.TH1I(
+    "h_sig_and_bkg_test_set", "h_sig_and_bkg_test_set", 2, 0, 2)
+h_sig_and_bkg_test_set_predict = ROOT.TH1I(
+    "h_sig_and_bkg_test_set_predict", "h_sig_and_bkg_test_set_predict", 2, 0, 2)
+dic_posterior_test_set = {'bkg': [], 'sig': []}
+# Now calculate the predict result of train dateset
+# for i in range(0, train_set + test_set):
+for i in range(train_set, train_set + test_set):
+    # GetEntry
+    event_CH1.m_tree_event.GetEntry(i)
+    event_CH2.m_tree_event.GetEntry(i)
+    event_CH3.m_tree_event.GetEntry(i)
+    h_sig_and_bkg_test_set.Fill(event_CH3.trig_level[0])
+    dic_posterior = {'bkg': None, 'sig': None}
+    for key in dic_hist:
+        i_bin_charge = dic_hist[key]['charge'].FindBin(event_CH3.charge[0])
+        i_bin_width = dic_hist[key]['width'].FindBin(event_CH3.width[0])
+        # i_bin_max_voltage = dic_hist[key]['max_voltage'].FindBin(
+        #     event_CH3.max_voltage[0])
+        condi_pro_charge = dic_condi_pro[key]['charge'][i_bin_charge]
+        condi_pro_width = dic_condi_pro[key]['width'][i_bin_width]
+        # condi_pro_max_voltage = dic_condi_pro[key]['max_voltage'][i_bin_max_voltage]
+        # calculate posterior
+        dic_posterior[key] = dic_prior[key] * condi_pro_charge * \
+            condi_pro_width * 1#condi_pro_max_voltage
+    dic_posterior_test_set['sig'].append(dic_posterior['sig'])
+    dic_posterior_test_set['bkg'].append(dic_posterior['bkg'])
+    if(dic_posterior['sig'] >= dic_posterior['bkg'] and event_CH3.trig_level[0] == 0):
+        h_sig_and_bkg_test_set_predict.Fill(0)
+    elif (dic_posterior['sig'] < dic_posterior['bkg'] and event_CH3.trig_level[0] == 1):
+        h_sig_and_bkg_test_set_predict.Fill(1)
+
+
+print("/**************posterior posibbility for test set****************/")
+for i in range(0, len(dic_posterior_test_set['bkg'])):
+    print("bkg: {0:f}, sig: {1:f}".format(
+        dic_posterior_test_set['bkg'][i], dic_posterior_test_set['sig'][i]))
+print("truth sig: {0}".format(h_sig_and_bkg_test_set.GetBinContent(1)))
+print("truth bkg:{0}".format(h_sig_and_bkg_test_set.GetBinContent(2)))
+print("pred sig: {0}".format(h_sig_and_bkg_test_set_predict.GetBinContent(1)))
+print("pred bkg:{0}".format(h_sig_and_bkg_test_set_predict.GetBinContent(2)))
+
+
+# Calculate
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/naive_bayesian_classifier/naive_bayesian_classifier_CH2.py` & `oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/naive_bayesian_classifier/naive_bayesian_classifier.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-#!/usr/bin/env python
-# Author: Zifeng Xu
-# This scripts aim to train the classifier use 7000 data, and use the classifier to predict.
-# Also, the confusion matrix.
-
-from Event import Event as Ev
-import numpy as np
-import ROOT
-ROOT.gROOT.SetBatch(True)
-ROOT.gROOT.SetStyle("ATLAS")
-# import matplotlib.pyplot as plt
-
-LAMBDA = 1.0
-train_set = 7000
-test_set = 3000
-# Init all event we need
-event_CH1 = Ev('../channel2_trig_n3p00_cut_charge_n4400_level_n2p68_CH1.root')
-event_CH2 = Ev('../channel2_trig_n3p00_cut_charge_n4400_level_n2p68_CH2.root')
-event_CH3 = Ev('../channel2_trig_n3p00_cut_charge_n4400_level_n2p68_CH3.root')
-
-# Use 0-6999 to learn, use 7000-9999 to test
-
-
-charge_bin_x = np.array([-4950., -4860., -4845., -4800])
-width_binx = np.array([274., 294., 300., 303.])
-# max_voltage_binx = np.array([-5.5, -2.4, -2.3])
-
-dic_hist = {}
-# Train
-h_charge_sig = ROOT.TH1F("charge_sig", "charge_sig",
-                         len(charge_bin_x) - 1, charge_bin_x)
-h_charge_bkg = ROOT.TH1F("charge_bkg", "charge_bkg",
-                         len(charge_bin_x) - 1, charge_bin_x)
-h_width_sig = ROOT.TH1I("width_sig", "width_sig",
-                        len(width_binx)-1, width_binx)
-h_width_bkg = ROOT.TH1I("width_bkg", "width_bkg",
-                        len(width_binx)-1, width_binx)
-# h_max_voltage_sig = ROOT.TH1F("max_voltage_sig", "max_voltage_sig", len(
-#     max_voltage_binx)-1, max_voltage_binx)
-# h_max_voltage_bkg = ROOT.TH1F("max_voltage_bkg", "max_voltage_bkg", len(
-#     max_voltage_binx)-1, max_voltage_binx)
-dic_hist['bkg'] = {'charge': h_charge_bkg,
-                   'width': h_width_bkg}
-dic_hist['sig'] = {'charge': h_charge_sig,
-                   'width': h_width_sig}
-# Use Maximum Likelihood estimate parameters
-# Just fill the histogram first
-for i in range(0, train_set):
-    # GetEntry
-    event_CH1.m_tree_event.GetEntry(i)
-    event_CH2.m_tree_event.GetEntry(i)
-    event_CH3.m_tree_event.GetEntry(i)
-
-    # If sig
-    if(event_CH3.trig_level[0] == 0):
-        h_charge_sig.Fill(event_CH3.charge[0])
-        h_width_sig.Fill(event_CH3.width[0])
-        # h_max_voltage_sig.Fill(event_CH3.max_voltage[0])
-    # If bkg
-    elif (event_CH3.trig_level[0] == 1):
-        h_charge_bkg.Fill(event_CH3.charge[0])
-        h_width_bkg.Fill(event_CH3.width[0])
-        # h_max_voltage_bkg.Fill(event_CH3.max_voltage[0])
-
-# dic_canvas = {'bkg': ['charge', 'width', 'max_voltage'],
-#               'sig': ['charge', 'width', 'max_voltage']}
-# for key in dic_canvas.keys():
-#     for variable in dic_canvas[key]:
-#         _canvas=ROOT.TCanvas("train_{0}_{1}".format(key,variable),"{0}_{1}".format(key,variable),800,600)
-#         dic_hist[key][variable].Draw("hist e")
-#         ROOT.gPad.Update()
-#         _canvas.SaveAs("train_{0}_{1}.png".format(key,variable))
-
-# estimate prior probability
-dic_prior = {}
-prior_bkg = (dic_hist['bkg']['charge'].GetEntries() +
-             LAMBDA) / (float(train_set) + 2*LAMBDA)
-prior_sig = (dic_hist['sig']['charge'].GetEntries() +
-             LAMBDA) / (float(train_set) + 2*LAMBDA)
-dic_prior['bkg'] = prior_bkg
-dic_prior['sig'] = prior_sig
-
-# estimate conditional probability
-dic_condi_pro = {'bkg': {}, 'sig': {}}
-for cat in ['bkg', 'sig']:
-    for variable in ['charge', 'width']:
-        _list_condi_pro = []
-        for i in range(0, dic_hist[cat][variable].GetNbinsX()+2):
-            _list_condi_pro.append((dic_hist[cat][variable].GetBinContent(
-                i) + LAMBDA) / (dic_hist[cat][variable].GetEntries() + dic_hist[cat][variable].GetNbinsX() * LAMBDA))
-        dic_condi_pro[cat][variable] = _list_condi_pro
-
-print("/**************prior posibillity****************/")
-print(dic_prior)
-print("/**************condition posibillity****************/")
-print(dic_condi_pro)
-
-h_sig_and_bkg_train_set = ROOT.TH1I(
-    "h_sig_and_bkg_train_set", "h_sig_and_bkg_train_set", 2, 0, 2)
-h_sig_and_bkg_train_set_predict = ROOT.TH1I(
-    "h_sig_and_bkg_train_set_predict", "h_sig_and_bkg_train_set_predict", 2, 0, 2)
-dic_posterior_train_set = {'bkg': [], 'sig': []}
-# Now calculate the predict result of train dateset
-# for i in range(0, train_set + test_set):
-for i in range(0, train_set):
-    # GetEntry
-    event_CH1.m_tree_event.GetEntry(i)
-    event_CH2.m_tree_event.GetEntry(i)
-    event_CH3.m_tree_event.GetEntry(i)
-    h_sig_and_bkg_train_set.Fill(event_CH3.trig_level[0])
-    dic_posterior = {'bkg': None, 'sig': None}
-    for key in dic_hist:
-        i_bin_charge = dic_hist[key]['charge'].FindBin(event_CH3.charge[0])
-        i_bin_width = dic_hist[key]['width'].FindBin(event_CH3.width[0])
-        # i_bin_max_voltage = dic_hist[key]['max_voltage'].FindBin(
-        #     event_CH3.max_voltage[0])
-        condi_pro_charge = dic_condi_pro[key]['charge'][i_bin_charge]
-        condi_pro_width = dic_condi_pro[key]['width'][i_bin_width]
-        # condi_pro_max_voltage = dic_condi_pro[key]['max_voltage'][i_bin_max_voltage]
-        # calculate posterior
-        dic_posterior[key] = dic_prior[key] * condi_pro_charge * \
-            condi_pro_width * 1#condi_pro_max_voltage
-    dic_posterior_train_set['sig'].append(dic_posterior['sig'])
-    dic_posterior_train_set['bkg'].append(dic_posterior['bkg'])
-    if(dic_posterior['sig'] >= dic_posterior['bkg'] and event_CH3.trig_level[0] == 0):
-        h_sig_and_bkg_train_set_predict.Fill(0)
-    elif (dic_posterior['sig'] < dic_posterior['bkg'] and event_CH3.trig_level[0] == 1):
-        h_sig_and_bkg_train_set_predict.Fill(1)
-
-
-print("/**************posterior posibbility for train set****************/")
-for i in range(0, len(dic_posterior_train_set['bkg'])):
-    print("bkg: {0:f}, sig: {1:f}".format(
-        dic_posterior_train_set['bkg'][i], dic_posterior_train_set['sig'][i]))
-print("truth sig: {0}".format(h_sig_and_bkg_train_set.GetBinContent(1)))
-print("truth bkg:{0}".format(h_sig_and_bkg_train_set.GetBinContent(2)))
-print("pred sig: {0}".format(h_sig_and_bkg_train_set_predict.GetBinContent(1)))
-print("pred bkg:{0}".format(h_sig_and_bkg_train_set_predict.GetBinContent(2)))
-
-
-h_sig_and_bkg_test_set = ROOT.TH1I(
-    "h_sig_and_bkg_test_set", "h_sig_and_bkg_test_set", 2, 0, 2)
-h_sig_and_bkg_test_set_predict = ROOT.TH1I(
-    "h_sig_and_bkg_test_set_predict", "h_sig_and_bkg_test_set_predict", 2, 0, 2)
-dic_posterior_test_set = {'bkg': [], 'sig': []}
-# Now calculate the predict result of train dateset
-# for i in range(0, train_set + test_set):
-for i in range(train_set, train_set + test_set):
-    # GetEntry
-    event_CH1.m_tree_event.GetEntry(i)
-    event_CH2.m_tree_event.GetEntry(i)
-    event_CH3.m_tree_event.GetEntry(i)
-    h_sig_and_bkg_test_set.Fill(event_CH3.trig_level[0])
-    dic_posterior = {'bkg': None, 'sig': None}
-    for key in dic_hist:
-        i_bin_charge = dic_hist[key]['charge'].FindBin(event_CH3.charge[0])
-        i_bin_width = dic_hist[key]['width'].FindBin(event_CH3.width[0])
-        # i_bin_max_voltage = dic_hist[key]['max_voltage'].FindBin(
-        #     event_CH3.max_voltage[0])
-        condi_pro_charge = dic_condi_pro[key]['charge'][i_bin_charge]
-        condi_pro_width = dic_condi_pro[key]['width'][i_bin_width]
-        # condi_pro_max_voltage = dic_condi_pro[key]['max_voltage'][i_bin_max_voltage]
-        # calculate posterior
-        dic_posterior[key] = dic_prior[key] * condi_pro_charge * \
-            condi_pro_width * 1#condi_pro_max_voltage
-    dic_posterior_test_set['sig'].append(dic_posterior['sig'])
-    dic_posterior_test_set['bkg'].append(dic_posterior['bkg'])
-    if(dic_posterior['sig'] >= dic_posterior['bkg'] and event_CH3.trig_level[0] == 0):
-        h_sig_and_bkg_test_set_predict.Fill(0)
-    elif (dic_posterior['sig'] < dic_posterior['bkg'] and event_CH3.trig_level[0] == 1):
-        h_sig_and_bkg_test_set_predict.Fill(1)
-
-
-print("/**************posterior posibbility for test set****************/")
-for i in range(0, len(dic_posterior_test_set['bkg'])):
-    print("bkg: {0:f}, sig: {1:f}".format(
-        dic_posterior_test_set['bkg'][i], dic_posterior_test_set['sig'][i]))
-print("truth sig: {0}".format(h_sig_and_bkg_test_set.GetBinContent(1)))
-print("truth bkg:{0}".format(h_sig_and_bkg_test_set.GetBinContent(2)))
-print("pred sig: {0}".format(h_sig_and_bkg_test_set_predict.GetBinContent(1)))
-print("pred bkg:{0}".format(h_sig_and_bkg_test_set_predict.GetBinContent(2)))
-
-
-# Calculate
+#!/usr/bin/env python
+# Author: Zifeng Xu
+# This scripts aim to train the classifier use 7000 data, and use the classifier to predict.
+# Also, the confusion matrix.
+
+from Event import Event as Ev
+import numpy as np
+import ROOT
+ROOT.gROOT.SetBatch(True)
+ROOT.gROOT.SetStyle("ATLAS")
+# import matplotlib.pyplot as plt
+
+LAMBDA = 1.0
+train_set = 7000
+test_set = 3000
+# Init all event we need
+event_CH1 = Ev('../channel2_trig_n3p00_cut_charge_n4400_level_n2p68_CH1.root')
+event_CH2 = Ev('../channel2_trig_n3p00_cut_charge_n4400_level_n2p68_CH2.root')
+event_CH3 = Ev('../channel2_trig_n3p00_cut_charge_n4400_level_n2p68_CH3.root')
+
+# Use 0-6999 to learn, use 7000-9999 to test
+
+
+charge_bin_x = np.array([-4950., -4860., -4845., -4800])
+width_binx = np.array([274., 294., 300., 303.])
+# max_voltage_binx = np.array([-5.5, -2.4, -2.3])
+
+dic_hist = {}
+# Train
+h_charge_sig = ROOT.TH1F("charge_sig", "charge_sig",
+                         len(charge_bin_x) - 1, charge_bin_x)
+h_charge_bkg = ROOT.TH1F("charge_bkg", "charge_bkg",
+                         len(charge_bin_x) - 1, charge_bin_x)
+h_width_sig = ROOT.TH1I("width_sig", "width_sig",
+                        len(width_binx)-1, width_binx)
+h_width_bkg = ROOT.TH1I("width_bkg", "width_bkg",
+                        len(width_binx)-1, width_binx)
+# h_max_voltage_sig = ROOT.TH1F("max_voltage_sig", "max_voltage_sig", len(
+#     max_voltage_binx)-1, max_voltage_binx)
+# h_max_voltage_bkg = ROOT.TH1F("max_voltage_bkg", "max_voltage_bkg", len(
+#     max_voltage_binx)-1, max_voltage_binx)
+dic_hist['bkg'] = {'charge': h_charge_bkg,
+                   'width': h_width_bkg}
+dic_hist['sig'] = {'charge': h_charge_sig,
+                   'width': h_width_sig}
+# Use Maximum Likelihood estimate parameters
+# Just fill the histogram first
+for i in range(6999, 10000):
+    # GetEntry
+    event_CH1.m_tree_event.GetEntry(i)
+    event_CH2.m_tree_event.GetEntry(i)
+    event_CH3.m_tree_event.GetEntry(i)
+
+    # If sig
+    if(event_CH3.trig_level[0] == 0):
+        h_charge_sig.Fill(event_CH3.charge[0])
+        h_width_sig.Fill(event_CH3.width[0])
+        # h_max_voltage_sig.Fill(event_CH3.max_voltage[0])
+    # If bkg
+    elif (event_CH3.trig_level[0] == 1):
+        h_charge_bkg.Fill(event_CH3.charge[0])
+        h_width_bkg.Fill(event_CH3.width[0])
+        # h_max_voltage_bkg.Fill(event_CH3.max_voltage[0])
+# Plot here
+# dic_canvas = {'bkg': ['charge', 'width'],
+#               'sig': ['charge', 'width']}
+# for key in dic_canvas.keys():
+#     for variable in dic_canvas[key]:
+#         _canvas=ROOT.TCanvas("test_{0}_{1}".format(key,variable),"{0}_{1}".format(key,variable),800,600)
+#         dic_hist[key][variable].Draw("hist e")
+#         ROOT.gPad.Update()
+#         _canvas.SaveAs("test_{0}_{1}.png".format(key,variable))
+
+# estimate prior probability
+dic_prior = {}
+prior_bkg = (dic_hist['bkg']['charge'].GetEntries() +
+             LAMBDA) / (float(train_set) + 2*LAMBDA)
+prior_sig = (dic_hist['sig']['charge'].GetEntries() +
+             LAMBDA) / (float(train_set) + 2*LAMBDA)
+dic_prior['bkg'] = prior_bkg
+dic_prior['sig'] = prior_sig
+
+# estimate conditional probability
+dic_condi_pro = {'bkg': {}, 'sig': {}}
+for cat in ['bkg', 'sig']:
+    for variable in ['charge', 'width']:
+        _list_condi_pro = []
+        for i in range(0, dic_hist[cat][variable].GetNbinsX()+2):
+            _list_condi_pro.append((dic_hist[cat][variable].GetBinContent(
+                i) + LAMBDA) / (dic_hist[cat][variable].GetEntries() + dic_hist[cat][variable].GetNbinsX() * LAMBDA))
+        dic_condi_pro[cat][variable] = _list_condi_pro
+
+print("/**************prior posibillity****************/")
+print(dic_prior)
+print("/**************condition posibillity****************/")
+print(dic_condi_pro)
+
+h_sig_and_bkg_train_set = ROOT.TH1I(
+    "h_sig_and_bkg_train_set", "h_sig_and_bkg_train_set", 2, 0, 2)
+h_sig_and_bkg_train_set_predict = ROOT.TH1I(
+    "h_sig_and_bkg_train_set_predict", "h_sig_and_bkg_train_set_predict", 2, 0, 2)
+dic_posterior_train_set = {'bkg': [], 'sig': []}
+# Now calculate the predict result of train dateset
+# for i in range(0, train_set + test_set):
+for i in range(0, train_set):
+    # GetEntry
+    event_CH1.m_tree_event.GetEntry(i)
+    event_CH2.m_tree_event.GetEntry(i)
+    event_CH3.m_tree_event.GetEntry(i)
+    h_sig_and_bkg_train_set.Fill(event_CH3.trig_level[0])
+    dic_posterior = {'bkg': None, 'sig': None}
+    for key in dic_hist:
+        i_bin_charge = dic_hist[key]['charge'].FindBin(event_CH3.charge[0])
+        i_bin_width = dic_hist[key]['width'].FindBin(event_CH3.width[0])
+        # i_bin_max_voltage = dic_hist[key]['max_voltage'].FindBin(
+        #     event_CH3.max_voltage[0])
+        condi_pro_charge = dic_condi_pro[key]['charge'][i_bin_charge]
+        condi_pro_width = dic_condi_pro[key]['width'][i_bin_width]
+        # condi_pro_max_voltage = dic_condi_pro[key]['max_voltage'][i_bin_max_voltage]
+        # calculate posterior
+        dic_posterior[key] = dic_prior[key] * condi_pro_charge * \
+            condi_pro_width * 1#condi_pro_max_voltage
+    dic_posterior_train_set['sig'].append(dic_posterior['sig'])
+    dic_posterior_train_set['bkg'].append(dic_posterior['bkg'])
+    if(dic_posterior['sig'] >= dic_posterior['bkg'] and event_CH3.trig_level[0] == 0):
+        h_sig_and_bkg_train_set_predict.Fill(0)
+    elif (dic_posterior['sig'] < dic_posterior['bkg'] and event_CH3.trig_level[0] == 1):
+        h_sig_and_bkg_train_set_predict.Fill(1)
+
+
+print("/**************posterior posibbility for train set****************/")
+for i in range(0, len(dic_posterior_train_set['bkg'])):
+    print("bkg: {0:f}, sig: {1:f}".format(
+        dic_posterior_train_set['bkg'][i], dic_posterior_train_set['sig'][i]))
+print("truth sig: {0}".format(h_sig_and_bkg_train_set.GetBinContent(1)))
+print("truth bkg:{0}".format(h_sig_and_bkg_train_set.GetBinContent(2)))
+print("pred sig: {0}".format(h_sig_and_bkg_train_set_predict.GetBinContent(1)))
+print("pred bkg:{0}".format(h_sig_and_bkg_train_set_predict.GetBinContent(2)))
+
+
+h_sig_and_bkg_test_set = ROOT.TH1I(
+    "h_sig_and_bkg_test_set", "h_sig_and_bkg_test_set", 2, 0, 2)
+h_sig_and_bkg_test_set_predict = ROOT.TH1I(
+    "h_sig_and_bkg_test_set_predict", "h_sig_and_bkg_test_set_predict", 2, 0, 2)
+dic_posterior_test_set = {'bkg': [], 'sig': []}
+# Now calculate the predict result of train dateset
+# for i in range(0, train_set + test_set):
+for i in range(train_set, train_set + test_set):
+    # GetEntry
+    event_CH1.m_tree_event.GetEntry(i)
+    event_CH2.m_tree_event.GetEntry(i)
+    event_CH3.m_tree_event.GetEntry(i)
+    h_sig_and_bkg_test_set.Fill(event_CH3.trig_level[0])
+    dic_posterior = {'bkg': None, 'sig': None}
+    for key in dic_hist:
+        i_bin_charge = dic_hist[key]['charge'].FindBin(event_CH3.charge[0])
+        i_bin_width = dic_hist[key]['width'].FindBin(event_CH3.width[0])
+        # i_bin_max_voltage = dic_hist[key]['max_voltage'].FindBin(
+        #     event_CH3.max_voltage[0])
+        condi_pro_charge = dic_condi_pro[key]['charge'][i_bin_charge]
+        condi_pro_width = dic_condi_pro[key]['width'][i_bin_width]
+        # condi_pro_max_voltage = dic_condi_pro[key]['max_voltage'][i_bin_max_voltage]
+        # calculate posterior
+        dic_posterior[key] = dic_prior[key] * condi_pro_charge * \
+            condi_pro_width * 1#condi_pro_max_voltage
+    dic_posterior_test_set['sig'].append(dic_posterior['sig'])
+    dic_posterior_test_set['bkg'].append(dic_posterior['bkg'])
+    if(dic_posterior['sig'] >= dic_posterior['bkg'] and event_CH3.trig_level[0] == 0):
+        h_sig_and_bkg_test_set_predict.Fill(0)
+    elif (dic_posterior['sig'] < dic_posterior['bkg'] and event_CH3.trig_level[0] == 1):
+        h_sig_and_bkg_test_set_predict.Fill(1)
+
+
+print("/**************posterior posibbility for test set****************/")
+for i in range(0, len(dic_posterior_test_set['bkg'])):
+    print("bkg: {0:f}, sig: {1:f}".format(
+        dic_posterior_test_set['bkg'][i], dic_posterior_test_set['sig'][i]))
+print("truth sig: {0}".format(h_sig_and_bkg_test_set.GetBinContent(1)))
+print("truth bkg:{0}".format(h_sig_and_bkg_test_set.GetBinContent(2)))
+print("pred sig: {0}".format(h_sig_and_bkg_test_set_predict.GetBinContent(1)))
+print("pred bkg:{0}".format(h_sig_and_bkg_test_set_predict.GetBinContent(2)))
+
+
+# Calculate
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/single_channel_selector.C` & `oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/single_channel_selector.C`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-#define single_channel_selector_cxx
-// The class definition in single_channel_selector.h has been generated automatically
-// by the ROOT utility TTree::MakeSelector(). This class is derived
-// from the ROOT class TSelector. For more information on the TSelector
-// framework see $ROOTSYS/README/README.SELECTOR or the ROOT User Manual.
-
-// The following methods are defined in this file:
-//    Begin():        called every time a loop on the tree starts,
-//                    a convenient place to create your histograms.
-//    SlaveBegin():   called after Begin(), when on PROOF called only on the
-//                    slave servers.
-//    Process():      called for each event, in this function you decide what
-//                    to read and fill your histograms.
-//    SlaveTerminate: called at the end of the loop on the tree, when on PROOF
-//                    called only on the slave servers.
-//    Terminate():    called at the end of the loop on the tree,
-//                    a convenient place to draw/fit your histograms.
-//
-// To use this file, try the following session on your Tree T:
-//
-// root> T->Process("single_channel_selector.C")
-// root> T->Process("single_channel_selector.C","some options")
-// root> T->Process("single_channel_selector.C+")
-//
-
-#include "single_channel_selector.h"
-#include <TH2.h>
-#include <TStyle.h>
-#include "TH1F.h"
-#include "TTree.h"
-#include "TFile.h"
-#include "TMath.h"
-#include <iostream>
-//using std::vector;
-//using std::string;
-void single_channel_selector::Begin(TTree * /*tree*/)
-{
-   // The Begin() function is called at the start of the query.
-   // When running with PROOF Begin() is only called on the client.
-   // The tree argument is deprecated (on PROOF 0 is passed).
-
-   TString option = GetOption();
-   TString output_filename = option;
-
-   // // Initialize output file
-   m_output_file = TFile::Open(output_filename, "RECREATE");
-   // Initialize TTree
-   m_tree_event = new TTree("event", "event");
-   m_tree_event->Branch("max_voltage", &m_max_voltage, "max_voltage/D");
-   m_tree_event->Branch("width", &m_width, "width/I");
-   m_tree_event->Branch("charge", &m_charge, "charge/D");
-   m_tree_event->Branch("charge_shift", &m_charge_shift, "charge_shift/D");
-   m_tree_event->Branch("trig_charge", &m_trig_charge, "trig_charge/I");
-   m_tree_event->Branch("pass_width", &m_pass_width, "pass_width/I");
-   m_tree_event->Branch("trig_level", &m_trig_level, "trig_level/I");
-   m_tree_event->Branch("baseline_estimate", &m_baseline_voltage, "baseline_estimate/D");
-}
-
-void single_channel_selector::SlaveBegin(TTree * /*tree*/)
-{
-   // The SlaveBegin() function is called after the Begin() function.
-   // When running with PROOF SlaveBegin() is called on each slave server.
-   // The tree argument is deprecated (on PROOF 0 is passed).
-
-   TString option = GetOption();
-}
-
-Bool_t single_channel_selector::Process(Long64_t entry)
-{
-   // The Process() function is called for each entry in the tree (or possibly
-   // keyed object in the case of PROOF) to be processed. The entry argument
-   // specifies which entry in the currently loaded tree is to be processed.
-   // When processing keyed objects with PROOF, the object is already loaded
-   // and is available via the fObject pointer.
-   //
-   // This function should contain the \"body\" of the analysis. It can contain
-   // simple or elaborate selection criteria, run algorithms on the data
-   // of the event and typically fill histograms.
-   //
-   // The processing can be stopped by calling Abort().
-   //
-   // Use fStatus to set the return value of TTree::Process().
-   //
-   // The return value is currently not used.
-
-   fReader.SetLocalEntry(entry);
-   // Check if size == 0;
-   if ((*size) <= 0)
-   {
-      std::clog << "single_channel_selector::ERROR size of channel == 0; exit!" << std::endl;
-      return kFALSE;
-   }
-
-   m_baseline_voltage = GetBaseLineEstimate();
-   m_max_voltage = GetMinimumValue();
-   m_width = GetWidth();
-   m_charge = GetCharge();
-   m_charge_shift = m_charge - m_baseline_voltage * 2000;
-
-   m_trig_charge = Pass_trigger_charge();
-   m_pass_width = Pass_width();
-   m_trig_level = Pass_trigger_level();
-
-   m_tree_event->Fill();
-
-   return kTRUE;
-}
-
-void single_channel_selector::SlaveTerminate()
-{
-   // The SlaveTerminate() function is called after all entries or objects
-   // have been processed. When running with PROOF SlaveTerminate() is called
-   // on each slave server.
-}
-
-void single_channel_selector::Terminate()
-{
-   // The Terminate() function is the last function to be called during
-   // a query. It always runs on the client, it can be used to present
-   // the results graphically or save the results to file.
-
-   m_tree_event->Write();
-   m_output_file->Close();
-}
-
-Int_t single_channel_selector::Pass_width()
-{
-   if (m_width <= 100)
-   {
-      return 1;
-   }
-   else
-   {
-      return 0;
-   }
-}
-Int_t single_channel_selector::Pass_trigger_charge()
-{
-
-   if (m_charge <= -m_baseline_voltage * 2000)
-   {
-      return 1;
-   }
-   else
-   {
-      return 0;
-   }
-}
-
-Int_t single_channel_selector::Pass_trigger_level()
-{
-   Double_t pass_level = -0.2;
-   if (m_max_voltage - m_baseline_voltage <= pass_level)
-   {
-      return 1;
-   }
-   else
-   {
-      return 0;
-   }
-}
-
-Double_t single_channel_selector::GetMinimumValue()
-{
-
-   Double_t minimum_value;
-   minimum_value = voltage[0];
-   //for (auto i = 999; i < (*size); i++)
-   for (auto i = 899; i < 1200; i++)
-   {
-      if (voltage[i] < minimum_value)
-      {
-         minimum_value = voltage[i];
-      }
-   }
-
-   return minimum_value;
-}
-
-Int_t single_channel_selector::GetWidth()
-{
-   Int_t width = 0;
-   Double_t max_amplitude = m_baseline_voltage - m_max_voltage;
-   for (auto i = 899; i < 1200; i++)
-   {
-      if ((m_baseline_voltage - voltage[i]) >= (max_amplitude / (1.4142136)))
-      {
-         width = width + 1;
-      }
-   }
-
-   return width;
-}
-
-Double_t single_channel_selector::GetCharge()
-{
-   Double_t charge = 0;
-   for (auto i = 0; i < (*size); i++)
-   {
-      charge = charge + voltage[i];
-   }
-
-   return charge;
-}
-
-Double_t single_channel_selector::GetBaseLineEstimate()
-{
-   int n_points = 500;
-   int i_begin = 0;
-   Double_t baseline = 0;
-   for (auto i = i_begin; i < i_begin + n_points; i++)
-   {
-      baseline = baseline + voltage[i];
-   }
-
-   baseline = baseline / n_points;
-   m_baseline_voltage = baseline;
-   return baseline;
-}
+#define single_channel_selector_cxx
+// The class definition in single_channel_selector.h has been generated automatically
+// by the ROOT utility TTree::MakeSelector(). This class is derived
+// from the ROOT class TSelector. For more information on the TSelector
+// framework see $ROOTSYS/README/README.SELECTOR or the ROOT User Manual.
+
+// The following methods are defined in this file:
+//    Begin():        called every time a loop on the tree starts,
+//                    a convenient place to create your histograms.
+//    SlaveBegin():   called after Begin(), when on PROOF called only on the
+//                    slave servers.
+//    Process():      called for each event, in this function you decide what
+//                    to read and fill your histograms.
+//    SlaveTerminate: called at the end of the loop on the tree, when on PROOF
+//                    called only on the slave servers.
+//    Terminate():    called at the end of the loop on the tree,
+//                    a convenient place to draw/fit your histograms.
+//
+// To use this file, try the following session on your Tree T:
+//
+// root> T->Process("single_channel_selector.C")
+// root> T->Process("single_channel_selector.C","some options")
+// root> T->Process("single_channel_selector.C+")
+//
+
+#include "single_channel_selector.h"
+#include <TH2.h>
+#include <TStyle.h>
+#include "TH1F.h"
+#include "TTree.h"
+#include "TFile.h"
+#include "TMath.h"
+#include <iostream>
+//using std::vector;
+//using std::string;
+void single_channel_selector::Begin(TTree * /*tree*/)
+{
+   // The Begin() function is called at the start of the query.
+   // When running with PROOF Begin() is only called on the client.
+   // The tree argument is deprecated (on PROOF 0 is passed).
+
+   TString option = GetOption();
+   TString output_filename = option;
+
+   // // Initialize output file
+   m_output_file = TFile::Open(output_filename, "RECREATE");
+   // Initialize TTree
+   m_tree_event = new TTree("event", "event");
+   m_tree_event->Branch("max_voltage", &m_max_voltage, "max_voltage/D");
+   m_tree_event->Branch("width", &m_width, "width/I");
+   m_tree_event->Branch("charge", &m_charge, "charge/D");
+   m_tree_event->Branch("charge_shift", &m_charge_shift, "charge_shift/D");
+   m_tree_event->Branch("trig_charge", &m_trig_charge, "trig_charge/I");
+   m_tree_event->Branch("pass_width", &m_pass_width, "pass_width/I");
+   m_tree_event->Branch("trig_level", &m_trig_level, "trig_level/I");
+   m_tree_event->Branch("baseline_estimate", &m_baseline_voltage, "baseline_estimate/D");
+}
+
+void single_channel_selector::SlaveBegin(TTree * /*tree*/)
+{
+   // The SlaveBegin() function is called after the Begin() function.
+   // When running with PROOF SlaveBegin() is called on each slave server.
+   // The tree argument is deprecated (on PROOF 0 is passed).
+
+   TString option = GetOption();
+}
+
+Bool_t single_channel_selector::Process(Long64_t entry)
+{
+   // The Process() function is called for each entry in the tree (or possibly
+   // keyed object in the case of PROOF) to be processed. The entry argument
+   // specifies which entry in the currently loaded tree is to be processed.
+   // When processing keyed objects with PROOF, the object is already loaded
+   // and is available via the fObject pointer.
+   //
+   // This function should contain the \"body\" of the analysis. It can contain
+   // simple or elaborate selection criteria, run algorithms on the data
+   // of the event and typically fill histograms.
+   //
+   // The processing can be stopped by calling Abort().
+   //
+   // Use fStatus to set the return value of TTree::Process().
+   //
+   // The return value is currently not used.
+
+   fReader.SetLocalEntry(entry);
+   // Check if size == 0;
+   if ((*size) <= 0)
+   {
+      std::clog << "single_channel_selector::ERROR size of channel == 0; exit!" << std::endl;
+      return kFALSE;
+   }
+
+   m_baseline_voltage = GetBaseLineEstimate();
+   m_max_voltage = GetMinimumValue();
+   m_width = GetWidth();
+   m_charge = GetCharge();
+   m_charge_shift = m_charge - m_baseline_voltage * 2000;
+
+   m_trig_charge = Pass_trigger_charge();
+   m_pass_width = Pass_width();
+   m_trig_level = Pass_trigger_level();
+
+   m_tree_event->Fill();
+
+   return kTRUE;
+}
+
+void single_channel_selector::SlaveTerminate()
+{
+   // The SlaveTerminate() function is called after all entries or objects
+   // have been processed. When running with PROOF SlaveTerminate() is called
+   // on each slave server.
+}
+
+void single_channel_selector::Terminate()
+{
+   // The Terminate() function is the last function to be called during
+   // a query. It always runs on the client, it can be used to present
+   // the results graphically or save the results to file.
+
+   m_tree_event->Write();
+   m_output_file->Close();
+}
+
+Int_t single_channel_selector::Pass_width()
+{
+   if (m_width <= 100)
+   {
+      return 1;
+   }
+   else
+   {
+      return 0;
+   }
+}
+Int_t single_channel_selector::Pass_trigger_charge()
+{
+
+   if (m_charge <= -m_baseline_voltage * 2000)
+   {
+      return 1;
+   }
+   else
+   {
+      return 0;
+   }
+}
+
+Int_t single_channel_selector::Pass_trigger_level()
+{
+   Double_t pass_level = -0.2;
+   if (m_max_voltage - m_baseline_voltage <= pass_level)
+   {
+      return 1;
+   }
+   else
+   {
+      return 0;
+   }
+}
+
+Double_t single_channel_selector::GetMinimumValue()
+{
+
+   Double_t minimum_value;
+   minimum_value = voltage[0];
+   //for (auto i = 999; i < (*size); i++)
+   for (auto i = 899; i < 1200; i++)
+   {
+      if (voltage[i] < minimum_value)
+      {
+         minimum_value = voltage[i];
+      }
+   }
+
+   return minimum_value;
+}
+
+Int_t single_channel_selector::GetWidth()
+{
+   Int_t width = 0;
+   Double_t max_amplitude = m_baseline_voltage - m_max_voltage;
+   for (auto i = 899; i < 1200; i++)
+   {
+      if ((m_baseline_voltage - voltage[i]) >= (max_amplitude / (1.4142136)))
+      {
+         width = width + 1;
+      }
+   }
+
+   return width;
+}
+
+Double_t single_channel_selector::GetCharge()
+{
+   Double_t charge = 0;
+   for (auto i = 0; i < (*size); i++)
+   {
+      charge = charge + voltage[i];
+   }
+
+   return charge;
+}
+
+Double_t single_channel_selector::GetBaseLineEstimate()
+{
+   int n_points = 500;
+   int i_begin = 0;
+   Double_t baseline = 0;
+   for (auto i = i_begin; i < i_begin + n_points; i++)
+   {
+      baseline = baseline + voltage[i];
+   }
+
+   baseline = baseline / n_points;
+   m_baseline_voltage = baseline;
+   return baseline;
+}
```

### Comparing `oscilloscope_scripts_xzf8971-1.1.0/scripts_need_ROOT/single_channel_selector.h` & `oscilloscope_scripts_xzf8971-1.2.0/scripts_need_ROOT/single_channel_selector.h`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-//////////////////////////////////////////////////////////
-// This class has been automatically generated on
-// Sat May 29 19:44:01 2021 by ROOT version 6.22/06
-// from TTree tree_waveform_CH1/A tree save channel CH1 wave form data and size of each measurment
-// found on file: CH1_and_CH2_test.root
-//////////////////////////////////////////////////////////
-
-#ifndef single_channel_selector_h
-#define single_channel_selector_h
-
-#include <TROOT.h>
-#include <TChain.h>
-#include <TFile.h>
-#include <TSelector.h>
-#include <TTreeReader.h>
-#include <TTreeReaderValue.h>
-#include <TTreeReaderArray.h>
-#include "TTree.h"
-
-// Headers needed by this particular selector
-//using std::string;
-//using std::vector;
-class single_channel_selector : public TSelector
-{
-public:
-   TTreeReader fReader; //!the tree reader
-   TTree *fChain = 0;   //!pointer to the analyzed TTree or TChain
-
-   // Readers to access the data (delete the ones you do not need).
-   TTreeReaderValue<Int_t> size = {fReader, "size"};
-   TTreeReaderArray<Double_t> time = {fReader, "time"};
-   TTreeReaderArray<Double_t> voltage = {fReader, "voltage"};
-
-   single_channel_selector(TTree * /*tree*/ = 0) {}
-   virtual ~single_channel_selector() {}
-   virtual Int_t Version() const { return 2; }
-   virtual void Begin(TTree *tree);
-   virtual void SlaveBegin(TTree *tree);
-   virtual void Init(TTree *tree);
-   virtual Bool_t Notify();
-   virtual Bool_t Process(Long64_t entry);
-   virtual Int_t GetEntry(Long64_t entry, Int_t getall = 0) { return fChain ? fChain->GetTree()->GetEntry(entry, getall) : 0; }
-   virtual void SetOption(const char *option) { fOption = option; }
-   virtual void SetObject(TObject *obj) { fObject = obj; }
-   virtual void SetInputList(TList *input) { fInput = input; }
-   virtual TList *GetOutputList() const { return fOutput; }
-   virtual void SlaveTerminate();
-   virtual void Terminate();
-
-   ClassDef(single_channel_selector, 0);
-
-private:
-   TFile *m_output_file;
-   TTree *m_tree_event;
-
-   Double_t m_baseline_voltage;
-   Double_t m_max_voltage;
-   Int_t m_width;
-   Double_t m_charge;
-   Double_t m_charge_shift;
-   Int_t m_trig_charge;
-   Int_t m_pass_width;
-   Int_t m_trig_level;
-
-   Double_t GetMinimumValue();
-   Double_t GetCharge();
-   Double_t GetBaseLineEstimate();
-   Int_t GetWidth();
-
-   Int_t Pass_trigger_charge();
-   Int_t Pass_width();
-   Int_t Pass_trigger_level();
-};
-
-#endif
-
-#ifdef single_channel_selector_cxx
-void single_channel_selector::Init(TTree *tree)
-{
-   // The Init() function is called when the selector needs to initialize
-   // a new tree or chain. Typically here the reader is initialized.
-   // It is normally not necessary to make changes to the generated
-   // code, but the routine can be extended by the user if needed.
-   // Init() will be called many times when running on PROOF
-   // (once per file to be processed).
-
-   fReader.SetTree(tree);
-}
-
-Bool_t single_channel_selector::Notify()
-{
-   // The Notify() function is called when a new file is opened. This
-   // can be either for a new TTree in a TChain or when when a new TTree
-   // is started when using PROOF. It is normally not necessary to make changes
-   // to the generated code, but the routine can be extended by the
-   // user if needed. The return value is currently not used.
-
-   return kTRUE;
-}
-
-#endif // #ifdef single_channel_selector_cxx
+//////////////////////////////////////////////////////////
+// This class has been automatically generated on
+// Sat May 29 19:44:01 2021 by ROOT version 6.22/06
+// from TTree tree_waveform_CH1/A tree save channel CH1 wave form data and size of each measurment
+// found on file: CH1_and_CH2_test.root
+//////////////////////////////////////////////////////////
+
+#ifndef single_channel_selector_h
+#define single_channel_selector_h
+
+#include <TROOT.h>
+#include <TChain.h>
+#include <TFile.h>
+#include <TSelector.h>
+#include <TTreeReader.h>
+#include <TTreeReaderValue.h>
+#include <TTreeReaderArray.h>
+#include "TTree.h"
+
+// Headers needed by this particular selector
+//using std::string;
+//using std::vector;
+class single_channel_selector : public TSelector
+{
+public:
+   TTreeReader fReader; //!the tree reader
+   TTree *fChain = 0;   //!pointer to the analyzed TTree or TChain
+
+   // Readers to access the data (delete the ones you do not need).
+   TTreeReaderValue<Int_t> size = {fReader, "size"};
+   TTreeReaderArray<Double_t> time = {fReader, "time"};
+   TTreeReaderArray<Double_t> voltage = {fReader, "voltage"};
+
+   single_channel_selector(TTree * /*tree*/ = 0) {}
+   virtual ~single_channel_selector() {}
+   virtual Int_t Version() const { return 2; }
+   virtual void Begin(TTree *tree);
+   virtual void SlaveBegin(TTree *tree);
+   virtual void Init(TTree *tree);
+   virtual Bool_t Notify();
+   virtual Bool_t Process(Long64_t entry);
+   virtual Int_t GetEntry(Long64_t entry, Int_t getall = 0) { return fChain ? fChain->GetTree()->GetEntry(entry, getall) : 0; }
+   virtual void SetOption(const char *option) { fOption = option; }
+   virtual void SetObject(TObject *obj) { fObject = obj; }
+   virtual void SetInputList(TList *input) { fInput = input; }
+   virtual TList *GetOutputList() const { return fOutput; }
+   virtual void SlaveTerminate();
+   virtual void Terminate();
+
+   ClassDef(single_channel_selector, 0);
+
+private:
+   TFile *m_output_file;
+   TTree *m_tree_event;
+
+   Double_t m_baseline_voltage;
+   Double_t m_max_voltage;
+   Int_t m_width;
+   Double_t m_charge;
+   Double_t m_charge_shift;
+   Int_t m_trig_charge;
+   Int_t m_pass_width;
+   Int_t m_trig_level;
+
+   Double_t GetMinimumValue();
+   Double_t GetCharge();
+   Double_t GetBaseLineEstimate();
+   Int_t GetWidth();
+
+   Int_t Pass_trigger_charge();
+   Int_t Pass_width();
+   Int_t Pass_trigger_level();
+};
+
+#endif
+
+#ifdef single_channel_selector_cxx
+void single_channel_selector::Init(TTree *tree)
+{
+   // The Init() function is called when the selector needs to initialize
+   // a new tree or chain. Typically here the reader is initialized.
+   // It is normally not necessary to make changes to the generated
+   // code, but the routine can be extended by the user if needed.
+   // Init() will be called many times when running on PROOF
+   // (once per file to be processed).
+
+   fReader.SetTree(tree);
+}
+
+Bool_t single_channel_selector::Notify()
+{
+   // The Notify() function is called when a new file is opened. This
+   // can be either for a new TTree in a TChain or when when a new TTree
+   // is started when using PROOF. It is normally not necessary to make changes
+   // to the generated code, but the routine can be extended by the
+   // user if needed. The return value is currently not used.
+
+   return kTRUE;
+}
+
+#endif // #ifdef single_channel_selector_cxx
```

