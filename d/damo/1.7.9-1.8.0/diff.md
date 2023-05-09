# Comparing `tmp/damo-1.7.9.tar.gz` & `tmp/damo-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.7.9.tar", last modified: Mon May  1 19:59:59 2023, max compression
+gzip compressed data, was "damo-1.8.0.tar", last modified: Tue May  9 17:20:48 2023, max compression
```

## Comparing `damo-1.7.9.tar` & `damo-1.8.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-01 19:59:59.216548 damo-1.7.9/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7226 2023-05-01 19:59:59.216548 damo-1.7.9/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6705 2023-05-01 19:59:55.000000 damo-1.7.9/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-05-01 19:59:55.000000 damo-1.7.9/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-05-01 19:59:59.216548 damo-1.7.9/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      959 2023-05-01 19:59:55.000000 damo-1.7.9/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-01 19:59:59.200549 damo-1.7.9/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-01 19:59:59.212548 damo-1.7.9/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      643 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9696 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3018 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5368 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      923 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damo_python2_support.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      762 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34053 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9985 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8485 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damon_args_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17961 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17960 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19344 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3644 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1849 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1170 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      768 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13296 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4691 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3613 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2772 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4481 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5144 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1196 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2970 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1611 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      565 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2406 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_stat.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1545 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_stat_kdamonds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3079 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_stat_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2809 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_stat_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      677 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      727 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      650 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3966 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        6 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5576 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-01 19:59:59.216548 damo-1.7.9/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7226 2023-05-01 19:59:59.000000 damo-1.7.9/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1135 2023-05-01 19:59:59.000000 damo-1.7.9/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-05-01 19:59:59.000000 damo-1.7.9/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-05-01 19:59:59.000000 damo-1.7.9/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-05-01 19:59:59.000000 damo-1.7.9/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-09 17:20:48.231830 damo-1.8.0/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7226 2023-05-09 17:20:48.231830 damo-1.8.0/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6705 2023-05-09 17:20:43.000000 damo-1.8.0/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-05-09 17:20:43.000000 damo-1.8.0/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-05-09 17:20:48.231830 damo-1.8.0/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      959 2023-05-09 17:20:43.000000 damo-1.8.0/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-09 17:20:48.219831 damo-1.8.0/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-09 17:20:48.231830 damo-1.8.0/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-05-09 17:20:44.000000 damo-1.8.0/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      643 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9696 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3018 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5368 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      923 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damo_python2_support.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      762 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34053 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9985 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8485 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damon_args_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17961 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17960 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19344 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3644 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1849 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1170 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      768 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13296 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4691 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3613 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2772 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4481 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5144 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1196 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2970 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1611 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      565 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2406 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_stat.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1545 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_stat_kdamonds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3079 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_stat_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2809 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_stat_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      677 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      727 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      650 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3966 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        6 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5576 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-09 17:20:48.231830 damo-1.8.0/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7226 2023-05-09 17:20:48.000000 damo-1.8.0/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1135 2023-05-09 17:20:48.000000 damo-1.8.0/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-05-09 17:20:48.000000 damo-1.8.0/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-05-09 17:20:48.000000 damo-1.8.0/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-05-09 17:20:48.000000 damo-1.8.0/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.7.9/PKG-INFO` & `damo-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.7.9
+Version: 1.8.0
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.9/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.9/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.0/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.0/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.9/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.0/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
```

### Comparing `damo-1.7.9/README.md` & `damo-1.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.9/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.9/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.0/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.0/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -44,15 +44,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.9/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.0/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
```

### Comparing `damo-1.7.9/setup.py` & `damo-1.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="damo",
-    version="1.7.9",
+    version="1.8.0",
     author="SeongJae Park",
     author_email="sj@kernel.org",
     description="DAMON user-space tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/awslabs/damo",
     project_urls={
```

### Comparing `damo-1.7.9/src/damo/_damo_dist.py` & `damo-1.8.0/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/_damo_fmt_str.py` & `damo-1.8.0/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/_damo_fs.py` & `damo-1.8.0/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/_damo_paddr_layout.py` & `damo-1.8.0/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/_damo_python2_support.py` & `damo-1.8.0/src/damo/_damo_python2_support.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/_damo_subcmds.py` & `damo-1.8.0/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/_damon.py` & `damo-1.8.0/src/damo/_damon.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/_damon_args.py` & `damo-1.8.0/src/damo/_damon_args.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/_damon_args_schemes.py` & `damo-1.8.0/src/damo/_damon_args_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/_damon_dbgfs.py` & `damo-1.8.0/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/_damon_result.py` & `damo-1.8.0/src/damo/_damon_result.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/_damon_sysfs.py` & `damo-1.8.0/src/damo/_damon_sysfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo.py` & `damo-1.8.0/src/damo/damo.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_adjust.py` & `damo-1.8.0/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_features.py` & `damo-1.8.0/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_fmt_json.py` & `damo-1.8.0/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_heats.py` & `damo-1.8.0/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_lru_sort.py` & `damo-1.8.0/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_monitor.py` & `damo-1.8.0/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_nr_regions.py` & `damo-1.8.0/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_reclaim.py` & `damo-1.8.0/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_record.py` & `damo-1.8.0/src/damo/damo_record.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_report.py` & `damo-1.8.0/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_report_raw.py` & `damo-1.8.0/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_schemes.py` & `damo-1.8.0/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_start.py` & `damo-1.8.0/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_stat.py` & `damo-1.8.0/src/damo/damo_stat.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_stat_kdamonds.py` & `damo-1.8.0/src/damo/damo_stat_kdamonds.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_stat_regions.py` & `damo-1.8.0/src/damo/damo_stat_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_stat_schemes.py` & `damo-1.8.0/src/damo/damo_stat_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_stop.py` & `damo-1.8.0/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_translate_damos.py` & `damo-1.8.0/src/damo/damo_translate_damos.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_tune.py` & `damo-1.8.0/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_validate.py` & `damo-1.8.0/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo/damo_wss.py` & `damo-1.8.0/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.9/src/damo.egg-info/PKG-INFO` & `damo-1.8.0/src/damo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.7.9
+Version: 1.8.0
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.9/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.9/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.0/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.0/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.9/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.0/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
```

### Comparing `damo-1.7.9/src/damo.egg-info/SOURCES.txt` & `damo-1.8.0/src/damo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

