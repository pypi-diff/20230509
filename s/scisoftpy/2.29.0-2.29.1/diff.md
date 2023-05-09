# Comparing `tmp/scisoftpy-2.29.0.tar.gz` & `tmp/scisoftpy-2.29.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scisoftpy-2.29.0.tar", last modified: Mon May  1 11:02:09 2023, max compression
+gzip compressed data, was "scisoftpy-2.29.1.tar", last modified: Tue May  9 11:09:24 2023, max compression
```

## Comparing `scisoftpy-2.29.0.tar` & `scisoftpy-2.29.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-01 11:02:09.471651 scisoftpy-2.29.0/
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      692 2023-05-01 11:02:09.472651 scisoftpy-2.29.0/PKG-INFO
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      101 2023-03-14 09:41:03.000000 scisoftpy-2.29.0/pyproject.toml
-drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-01 11:02:09.467651 scisoftpy-2.29.0/scisoftpy/
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     5809 2023-03-14 09:41:03.000000 scisoftpy-2.29.0/scisoftpy/__init__.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      727 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/crystallography.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      988 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/data.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    15992 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/dictutils.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      719 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/diffraction.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    21434 2023-05-01 11:00:38.000000 scisoftpy-2.29.0/scisoftpy/external.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      756 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/fft.py
-drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-01 11:02:09.467651 scisoftpy-2.29.0/scisoftpy/fit/
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      788 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/fit/__init__.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1074 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/flatten.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      718 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/image.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    11231 2023-03-09 14:46:32.000000 scisoftpy-2.29.0/scisoftpy/io.py
-drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-01 11:02:09.470651 scisoftpy-2.29.0/scisoftpy/jython/
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)        0 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/jython/__init__.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    20722 2023-03-09 14:46:32.000000 scisoftpy-2.29.0/scisoftpy/jython/fitcore.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4653 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/function.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2107 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jybeans.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4137 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jycomparisons.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    60797 2023-03-14 09:41:03.000000 scisoftpy-2.29.0/scisoftpy/jython/jycore.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1849 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jycrystallography.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      516 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jydata.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2815 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jydiffraction.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2294 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jyfft.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      905 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jyflatten.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     7320 2022-05-27 10:34:28.000000 scisoftpy-2.29.0/scisoftpy/jython/jyhdf5io.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4287 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/jython/jyimage.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    13632 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jyio.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4636 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jylinalg.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    19173 2022-11-29 10:59:56.000000 scisoftpy-2.29.0/scisoftpy/jython/jymaths.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1672 2022-05-27 10:34:28.000000 scisoftpy-2.29.0/scisoftpy/jython/jynxio.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     6095 2022-08-12 09:11:57.000000 scisoftpy-2.29.0/scisoftpy/jython/jyplot.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1427 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jyplottingsystem.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2898 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/jython/jyrandom.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     8515 2023-03-16 13:37:01.000000 scisoftpy-2.29.0/scisoftpy/jython/jyroi.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4739 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/jython/jyrpc.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     3196 2022-11-29 10:59:56.000000 scisoftpy-2.29.0/scisoftpy/jython/jyscisoft.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2166 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/jython/jysignal.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      993 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/jython/jywrapper.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      722 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/linalg.py
-drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-01 11:02:09.470651 scisoftpy-2.29.0/scisoftpy/nexus/
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      770 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/nexus/__init__.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     5809 2022-05-27 10:34:28.000000 scisoftpy-2.29.0/scisoftpy/nexus/hdf5.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    17001 2022-05-27 10:34:28.000000 scisoftpy-2.29.0/scisoftpy/nexus/nxclasses.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2128 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/nexus/utils.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    33907 2023-03-16 13:37:01.000000 scisoftpy-2.29.0/scisoftpy/plot.py
-drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-01 11:02:09.471651 scisoftpy-2.29.0/scisoftpy/python/
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)        0 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/python/__init__.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     7924 2022-08-12 09:11:57.000000 scisoftpy-2.29.0/scisoftpy/python/pybeans.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1127 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/python/pycomparisons.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    10966 2023-03-14 09:41:03.000000 scisoftpy-2.29.0/scisoftpy/python/pycore.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      309 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/python/pydata.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    23547 2022-08-12 09:11:57.000000 scisoftpy-2.29.0/scisoftpy/python/pyflatten.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     8720 2023-03-14 09:41:03.000000 scisoftpy-2.29.0/scisoftpy/python/pyh5py.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      790 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/python/pyhdf5io.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    22658 2023-03-09 14:46:32.000000 scisoftpy-2.29.0/scisoftpy/python/pyio.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     3733 2022-11-29 10:59:56.000000 scisoftpy-2.29.0/scisoftpy/python/pymaths.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      912 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/python/pynxio.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     5296 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/python/pyplot.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      836 2022-04-12 13:05:39.000000 scisoftpy-2.29.0/scisoftpy/python/pyplottingsystem.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     9310 2022-08-12 09:11:57.000000 scisoftpy-2.29.0/scisoftpy/python/pyroi.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     7597 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/python/pyrpc.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     3600 2023-03-14 09:41:03.000000 scisoftpy-2.29.0/scisoftpy/python/pyscisoft.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1112 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/python/pysignal.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2500 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/python/pywrapper.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      722 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/random.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1927 2022-08-12 09:11:57.000000 scisoftpy-2.29.0/scisoftpy/roi.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2346 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/rpc.py
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      780 2022-04-12 13:05:38.000000 scisoftpy-2.29.0/scisoftpy/signal.py
-drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-01 11:02:09.467651 scisoftpy-2.29.0/scisoftpy.egg-info/
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      692 2023-05-01 11:02:09.000000 scisoftpy-2.29.0/scisoftpy.egg-info/PKG-INFO
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1927 2023-05-01 11:02:09.000000 scisoftpy-2.29.0/scisoftpy.egg-info/SOURCES.txt
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)        1 2023-05-01 11:02:09.000000 scisoftpy-2.29.0/scisoftpy.egg-info/dependency_links.txt
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)       77 2023-05-01 11:02:09.000000 scisoftpy-2.29.0/scisoftpy.egg-info/requires.txt
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)       10 2023-05-01 11:02:09.000000 scisoftpy-2.29.0/scisoftpy.egg-info/top_level.txt
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)        1 2022-09-07 15:14:39.000000 scisoftpy-2.29.0/scisoftpy.egg-info/zip-safe
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      469 2023-05-01 11:02:09.472651 scisoftpy-2.29.0/setup.cfg
--rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1095 2023-03-14 09:41:03.000000 scisoftpy-2.29.0/setup.py
+drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-09 11:09:24.348068 scisoftpy-2.29.1/
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      692 2023-05-09 11:09:24.348068 scisoftpy-2.29.1/PKG-INFO
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      101 2023-03-14 09:41:03.000000 scisoftpy-2.29.1/pyproject.toml
+drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-09 11:09:24.344068 scisoftpy-2.29.1/scisoftpy/
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     5809 2023-05-04 16:04:03.000000 scisoftpy-2.29.1/scisoftpy/__init__.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      727 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/crystallography.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      988 2022-04-12 13:05:39.000000 scisoftpy-2.29.1/scisoftpy/data.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    15992 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/dictutils.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      719 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/diffraction.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    24091 2023-05-04 22:43:57.000000 scisoftpy-2.29.1/scisoftpy/external.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      756 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/fft.py
+drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-09 11:09:24.344068 scisoftpy-2.29.1/scisoftpy/fit/
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      788 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/fit/__init__.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1074 2022-04-12 13:05:39.000000 scisoftpy-2.29.1/scisoftpy/flatten.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      718 2022-04-12 13:05:39.000000 scisoftpy-2.29.1/scisoftpy/image.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    11231 2023-03-09 14:46:32.000000 scisoftpy-2.29.1/scisoftpy/io.py
+drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-09 11:09:24.346068 scisoftpy-2.29.1/scisoftpy/jython/
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)        0 2022-04-12 13:05:39.000000 scisoftpy-2.29.1/scisoftpy/jython/__init__.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    20722 2023-03-09 14:46:32.000000 scisoftpy-2.29.1/scisoftpy/jython/fitcore.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4653 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/jython/function.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2107 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/jython/jybeans.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4137 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/jython/jycomparisons.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    60797 2023-03-14 09:41:03.000000 scisoftpy-2.29.1/scisoftpy/jython/jycore.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1849 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/jython/jycrystallography.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      516 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/jython/jydata.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2815 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/jython/jydiffraction.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2294 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/jython/jyfft.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      905 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/jython/jyflatten.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     7320 2022-05-27 10:34:28.000000 scisoftpy-2.29.1/scisoftpy/jython/jyhdf5io.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4287 2022-04-12 13:05:39.000000 scisoftpy-2.29.1/scisoftpy/jython/jyimage.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    13632 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/jython/jyio.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4636 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/jython/jylinalg.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    19173 2022-11-29 10:59:56.000000 scisoftpy-2.29.1/scisoftpy/jython/jymaths.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1672 2022-05-27 10:34:28.000000 scisoftpy-2.29.1/scisoftpy/jython/jynxio.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     6095 2022-08-12 09:11:57.000000 scisoftpy-2.29.1/scisoftpy/jython/jyplot.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1427 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/jython/jyplottingsystem.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2898 2022-04-12 13:05:39.000000 scisoftpy-2.29.1/scisoftpy/jython/jyrandom.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     8515 2023-03-16 13:37:01.000000 scisoftpy-2.29.1/scisoftpy/jython/jyroi.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     4739 2022-04-12 13:05:39.000000 scisoftpy-2.29.1/scisoftpy/jython/jyrpc.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     3196 2022-11-29 10:59:56.000000 scisoftpy-2.29.1/scisoftpy/jython/jyscisoft.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2166 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/jython/jysignal.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      993 2022-04-12 13:05:39.000000 scisoftpy-2.29.1/scisoftpy/jython/jywrapper.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      722 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/linalg.py
+drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-09 11:09:24.346068 scisoftpy-2.29.1/scisoftpy/nexus/
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      770 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/nexus/__init__.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     5809 2022-05-27 10:34:28.000000 scisoftpy-2.29.1/scisoftpy/nexus/hdf5.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    17001 2022-05-27 10:34:28.000000 scisoftpy-2.29.1/scisoftpy/nexus/nxclasses.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2128 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/nexus/utils.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    33907 2023-03-16 13:37:01.000000 scisoftpy-2.29.1/scisoftpy/plot.py
+drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-09 11:09:24.348068 scisoftpy-2.29.1/scisoftpy/python/
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)        0 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/python/__init__.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     7924 2022-08-12 09:11:57.000000 scisoftpy-2.29.1/scisoftpy/python/pybeans.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1127 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/python/pycomparisons.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    11071 2023-05-02 18:39:06.000000 scisoftpy-2.29.1/scisoftpy/python/pycore.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      309 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/python/pydata.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    23547 2022-08-12 09:11:57.000000 scisoftpy-2.29.1/scisoftpy/python/pyflatten.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     9067 2023-05-04 17:43:38.000000 scisoftpy-2.29.1/scisoftpy/python/pyh5py.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      790 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/python/pyhdf5io.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)    22783 2023-05-04 17:41:57.000000 scisoftpy-2.29.1/scisoftpy/python/pyio.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     3733 2022-11-29 10:59:56.000000 scisoftpy-2.29.1/scisoftpy/python/pymaths.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      912 2022-04-12 13:05:39.000000 scisoftpy-2.29.1/scisoftpy/python/pynxio.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     5296 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/python/pyplot.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      836 2022-04-12 13:05:39.000000 scisoftpy-2.29.1/scisoftpy/python/pyplottingsystem.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     9310 2022-08-12 09:11:57.000000 scisoftpy-2.29.1/scisoftpy/python/pyroi.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     7597 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/python/pyrpc.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     3600 2023-03-14 09:41:03.000000 scisoftpy-2.29.1/scisoftpy/python/pyscisoft.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1112 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/python/pysignal.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2500 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/python/pywrapper.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      722 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/random.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1927 2022-08-12 09:11:57.000000 scisoftpy-2.29.1/scisoftpy/roi.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     2346 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/rpc.py
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      780 2022-04-12 13:05:38.000000 scisoftpy-2.29.1/scisoftpy/signal.py
+drwxrwxr-x   0 src77879 (1006840) src77879 (1006840)        0 2023-05-09 11:09:24.344068 scisoftpy-2.29.1/scisoftpy.egg-info/
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      692 2023-05-09 11:09:24.000000 scisoftpy-2.29.1/scisoftpy.egg-info/PKG-INFO
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1927 2023-05-09 11:09:24.000000 scisoftpy-2.29.1/scisoftpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)        1 2023-05-09 11:09:24.000000 scisoftpy-2.29.1/scisoftpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      116 2023-05-09 11:09:24.000000 scisoftpy-2.29.1/scisoftpy.egg-info/requires.txt
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)       10 2023-05-09 11:09:24.000000 scisoftpy-2.29.1/scisoftpy.egg-info/top_level.txt
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)        1 2022-09-07 15:14:39.000000 scisoftpy-2.29.1/scisoftpy.egg-info/zip-safe
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)      469 2023-05-09 11:09:24.348068 scisoftpy-2.29.1/setup.cfg
+-rw-rw-r--   0 src77879 (1006840) src77879 (1006840)     1152 2023-05-09 10:08:21.000000 scisoftpy-2.29.1/setup.py
```

### Comparing `scisoftpy-2.29.0/PKG-INFO` & `scisoftpy-2.29.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scisoftpy
-Version: 2.29.0
+Version: 2.29.1
 Summary: DAWN Python Extensions
 Home-page: https://gerrit.diamond.ac.uk/plugins/gitiles/scisoft/scisoft-core
 Author: Peter Chang
 Author-email: dataanalysis@diamond.ac.uk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `scisoftpy-2.29.0/scisoftpy/__init__.py` & `scisoftpy-2.29.1/scisoftpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     from .jython.jyscisoft import *
 else:
     from .python.pycore import *
     from .python.pymaths import *
     from .python.pycomparisons import *
     from .python.pyscisoft import *
 
-__version__ = "2.29.0"
+__version__ = "2.29.1"
 
 '''
 Imports should work with python+numpy only agreed with MB 11 Nov 2011
 '''
 try:
     from . import nexus
 except Exception as e:
```

### Comparing `scisoftpy-2.29.0/scisoftpy/crystallography.py` & `scisoftpy-2.29.1/scisoftpy/crystallography.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/data.py` & `scisoftpy-2.29.1/scisoftpy/data.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/dictutils.py` & `scisoftpy-2.29.1/scisoftpy/dictutils.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/diffraction.py` & `scisoftpy-2.29.1/scisoftpy/diffraction.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/external.py` & `scisoftpy-2.29.1/scisoftpy/external.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,29 +47,61 @@
 . unpickle output
 . exception raising
 '''
 
 from os import path as _path
 
 import sys
-py3 = sys.hexversion >= 0x03000000
+
+_pyhexver = sys.hexversion
+py3 = _pyhexver >= 0x03000000
 if py3:
     from pickle import dump as _psave, load as _pload
     import subprocess as sub
 else:
     from cPickle import dump as _psave, load as _pload
     if os.name == 'posix':
         try:
             import subprocess32 as sub
         except ImportError:
             import subprocess as sub
     else:
         import subprocess as sub
 
+if _pyhexver < 0x03060000:
+    import linecache
+    class FrameSummary(object):
+        def __init__(self, filename, lineno, name, lookup_line=True, locals=None, line=None, end_lineno=None, colno=None, end_colno=None):
+            self.filename = filename
+            self.lineno = lineno
+            self.name = name
+            self._line = line
+            if lookup_line:
+                self.line
+            self.locals = {k: _safe_string(v, 'local', func=repr)
+                for k, v in locals.items()} if locals else None
+            self.end_lineno = end_lineno
+            self.colno = colno
+            self.end_colno = end_colno
+
+        def __iter__(self):
+            return iter([self.filename, self.lineno, self.name, self.line])
+
+        @property
+        def line(self):
+            if self._line is None:
+                if self.lineno is None:
+                    return None
+                self._line = linecache.getline(self.filename, self.lineno)
+            return self._line.strip()
+    import traceback
+    setattr(traceback, FrameSummary.__name__, FrameSummary)
+
 _PICKLE_PROTOCOL=2
+
 def save_args(arg, dir=None): #@ReservedAssignment
     '''Save arguments as files in a temporary directory
     Use pickle for most objects but use NumPy's npy format for arrays
     arg -- sequence of arguments
     dir -- if None then create a secure temporary, else create if does not exist
     Return name of directory used
     '''
@@ -221,27 +253,28 @@
         if ldpath is not None:
             pyldpath = ldpath
         else:
             pyldpath = None
 
     # add current package
     h, _t = _path.split(__file__)
-    if '__pyclasspath__' in h:
-        _h, t = _path.split(h)
-        cp = [ p for p in _env['CLASSPATH'].split(os.pathsep) if not p.endswith('jar') ]
-        for p in cp:
-            f = _path.join(p, t)
-            if _path.exists(f):
-                pkg = p
-                break
+    if 'site-packages' not in h: # only if not installed
+        if '__pyclasspath__' in h:
+            _h, t = _path.split(h)
+            cp = [ p for p in _env['CLASSPATH'].split(os.pathsep) if not p.endswith('jar') ]
+            for p in cp:
+                f = _path.join(p, t)
+                if _path.exists(f):
+                    pkg = p
+                    break
+            else:
+                raise RuntimeError('Cannot find ScisoftPy in PYTHONPATH')
         else:
-            raise RuntimeError('Cannot find ScisoftPy in PYTHONPATH')
-    else:
-        pkg, _t = _path.split(h)
-    pypath.insert(0, pkg)
+            pkg, _t = _path.split(h)
+        pypath.insert(0, pkg)
 
     return pyexe, pypath, pyldpath
 
 
 _dls_modules = dict() # cache for modules
 
 _PYTHONPATH = 'PYTHONPATH'
@@ -256,49 +289,61 @@
         raise ValueError('Cannot use dls_module argument on Mac OS X')
     elif not sys.platform.startswith('linux') and not sys.platform.startswith('java'):
         print('Warning dls_module argument may not work')
 
     env = dict(_env)
     env.pop(_PYTHONPATH, None)
     import subprocess as sub
-    p = sub.Popen(['bash', '-l'], env=env, stdin=sub.PIPE, stdout=sub.PIPE, stderr=sub.PIPE, universal_newlines=True)
-    p.stdin.write('source {}\n'.format(module_init))
-    p.stdin.write('module load {}\n'.format(module))
-    p.stdin.write('pyexe=$(which python)\n')
-    p.stdin.write('echo "EXEC:$pyexe"\n')
-    p.stdin.write('echo "PATH:$PYTHONPATH"\n')
-    p.stdin.write('echo "LDPATH:$LD_LIBRARY_PATH"\n')
-    p.stdin.close()
-    exe, path, ldpath = parse_for_env(p.stdout)
-    if exe is None:
-        raise RuntimeError('Problem with running external process: ' + p.stderr.read())
+    try:
+        p = sub.Popen(['bash', '-l'], env=env, close_fds=True, stdin=sub.PIPE, stdout=sub.PIPE, stderr=sub.PIPE, universal_newlines=True)
+        p.stdin.write('source {}\n'.format(module_init))
+        p.stdin.write('module load {}\n'.format(module))
+        p.stdin.write('pyexe=$(which python)\n')
+        p.stdin.write('echo "EXEC:$pyexe"\n')
+        p.stdin.write('echo "PATH:$PYTHONPATH"\n')
+        p.stdin.write('echo "LDPATH:$LD_LIBRARY_PATH"\n')
+        p.stdin.close()
+        exe, path, ldpath = parse_for_env(p.stdout)
+        if exe is None:
+            raise RuntimeError('Problem with running external process: ' + p.stderr.read())
+    finally:
+        p.stdout.close()
+        p.stderr.close()
+        p.terminate()
+        p.wait()
     _dls_modules[module] = exe, path, ldpath
     return exe, path, ldpath
 
 def get_python(py3=True):
     env = dict(_env)
     env.pop(_PYTHONPATH, None)
     pyexe = 'python2' if not py3 else 'python3'
-    p = sub.Popen(pyexe, env=env, stdin=sub.PIPE, stdout=sub.PIPE, stderr=sub.PIPE, universal_newlines=True)
-    p.stdin.write('import sys\n')
-    p.stdin.write('print("EXEC|" + sys.executable)\n')
-    p.stdin.write('print("PATH|" + "|".join(sys.path))\n')
-    p.stdin.write('import os\n')
-    p.stdin.write('if sys.platform == "win32":\n')
-    p.stdin.write('    key = "PATH"\n')
-    p.stdin.write('elif sys.platform == "darwin":\n')
-    p.stdin.write('    key = "DYLD_LIBRARY_PATH"\n')
-    p.stdin.write('else:\n')
-    p.stdin.write('    key = "LD_LIBRARY_PATH"\n')
-    p.stdin.write('lp = os.environ[key].split(os.pathsep)\n')
-    p.stdin.write('print("LDPATH|" + "|".join(lp))\n')
-    p.stdin.close()
-    exe, path, ldpath = parse_for_env(p.stdout, sep='|')
-    if exe is None:
-        raise RuntimeError('Problem with running external process: ' + p.stderr.read())
+    try:
+        p = sub.Popen(pyexe, env=env, close_fds=True, stdin=sub.PIPE, stdout=sub.PIPE, stderr=sub.PIPE, universal_newlines=True)
+        p.stdin.write('import sys\n')
+        p.stdin.write('print("EXEC|" + sys.executable)\n')
+        p.stdin.write('print("PATH|" + "|".join(sys.path))\n')
+        p.stdin.write('import os\n')
+        p.stdin.write('if sys.platform == "win32":\n')
+        p.stdin.write('    key = "PATH"\n')
+        p.stdin.write('elif sys.platform == "darwin":\n')
+        p.stdin.write('    key = "DYLD_LIBRARY_PATH"\n')
+        p.stdin.write('else:\n')
+        p.stdin.write('    key = "LD_LIBRARY_PATH"\n')
+        p.stdin.write('lp = os.environ[key].split(os.pathsep)\n')
+        p.stdin.write('print("LDPATH|" + "|".join(lp))\n')
+        p.stdin.close()
+        exe, path, ldpath = parse_for_env(p.stdout, sep='|')
+        if exe is None:
+            raise RuntimeError('Problem with running external process: ' + p.stderr.read())
+    finally:
+        p.stdout.close()
+        p.stderr.close()
+        p.terminate()
+        p.wait()
     return exe, path, ldpath
 
 def parse_for_env(stream, sep=':'):
     exe = None
     path = None
     ldpath = None
     while True:
@@ -376,41 +421,44 @@
                         line = self.stream.readline()
                         if line:
                             self.out.put(line)
                         else:
                             self.out.put('\n')
                             self.alive = False
                             break
+                    self.stream.close()
             else:
                 def add():
                     with open('/tmp/%s.log' % self.name, 'w') as log:
                         while self.alive:
                             line = self.stream.readline()
                             if line:
                                 print(line, file=log)
                                 self.out.put(line)
                             else:
                                 self.out.put('\n')
                                 print('Finished %s' % self.name, file=log)
                                 self.alive = False
                                 break
+                        self.stream.close()
             self.thd = Thread(target=add)
             self.thd.daemon = True
             self.thd.start()
 
         def readline(self, timeout=None):
             try:
                 if self.alive:
                     return self.out.get(block=True, timeout=timeout)
                 return self.out.get_nowait()
             except Empty:
                 return None
 
         def kill(self):
             self.alive = False
+            self.thd.join(2)
 
         def clear(self):
             while self.out.qsize() > 0:
                 self.out.get_nowait()
 
     class PythonSubProcess(object):
         READY = 'READY\n'
@@ -418,15 +466,15 @@
         def __init__(self, exe='python', env=None):
             if env is None:
                 env = dict(os.environ)
                 env.pop(_PYTHONPATH, None)
 #             print('PyExe: %s' % exe, file=sys.stderr)
 #             if _PYTHONPATH in env:
 #                 print('PyEnv: %s' % env[_PYTHONPATH], file=sys.stderr)
-            self.proc = sub.Popen([exe, '-c', cmds], bufsize=1, env=env, stdin=sub.PIPE, stdout=sub.PIPE, stderr=sub.PIPE, universal_newlines=True)
+            self.proc = sub.Popen([exe, '-c', cmds], bufsize=1, env=env, close_fds=True, stdin=sub.PIPE, stdout=sub.PIPE, stderr=sub.PIPE, universal_newlines=True)
 #             self.out = StreamHandler(self.proc.stdout, 'out')
 #             self.err = StreamHandler(self.proc.stderr, 'err')
             self.out = StreamHandler(self.proc.stdout)
             self.err = StreamHandler(self.proc.stderr)
             self.stdin = self.proc.stdin
             from time import sleep
             sleep(0.5)
@@ -467,14 +515,19 @@
             self.out.clear()
             self.err.clear()
             self.stdin.write(text)
             self.stdin.flush()
 
         def stop(self):
             self.stdin.close()
+            self.out.kill()
+            self.err.kill()
+            self.proc.terminate()
+            self.proc.wait()
+            self.proc = None
 
 class ExternalFunction(object):
     '''Emulates a function object with an attached python process
     '''
     def __init__(self, exe, env, module, function, keep):
         self.exe = exe
         self.env = env
@@ -542,15 +595,24 @@
                     if l.startswith('FWOUT'):
                         r = l.split('|')
                         if len(r) > 1:
                             d = r[1]
                             try:
                                 ret, err = load_args(d)
                                 if err:
-                                    sys.stderr.writelines(err[2])
+                                    frames = err[2]
+                                    if frames and not isinstance(frames[0], str):
+                                        if _pyhexver >= 0x030b0000:
+                                            for f in frames:
+                                                if not hasattr(f, 'colno'):
+                                                    setattr(f, 'colno', 0)
+                                                    setattr(f, 'end_colno', -1)
+                                                    setattr(f, 'end_lineno', -1)
+                                        frames = traceback.format_list(frames)
+                                    sys.stderr.writelines(frames)
                                     raise err[1]
                                 return ret
                             finally:
                                 shutil.rmtree(d)
                     else:
                         print(l)
             if err:
@@ -610,28 +672,33 @@
 
     ldpath = None
     if dls_module:
         if isinstance(dls_module, str):
             exe, path, ldpath = get_dls_module(dls_module)
         else:
             exe, path, ldpath = get_dls_module()
+    elif isinstance(path, str):
+        path = [path]
     exe, path, ldpath = pyenv(exe, path, ldpath)
 
     if p is None:
         p = find_module_path(path, module)
     if p is None:
         p = find_module_path(sys.path, module)
     if p and p not in path:
         path.insert(0, p)
     if extra_path:
         if p is None:
             p = find_module_path(extra_path, module)
-        path = extra_path + path
+        extras = [ e for e in extra_path if e not in path ]
+        if extras:
+            path = extras + path
     if p is None:
         raise ValueError('Cannot find module in path: try specifying it in extra_path')
+
     env = dict(_env)
     env[_PYTHONPATH] = os.pathsep.join(path)
     if ldpath:
         if sys.platform == 'win32':
             key = 'PATH'
         elif sys.platform == 'darwin':
             key = 'DYLD_LIBRARY_PATH'
```

### Comparing `scisoftpy-2.29.0/scisoftpy/fft.py` & `scisoftpy-2.29.1/scisoftpy/fft.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/fit/__init__.py` & `scisoftpy-2.29.1/scisoftpy/fit/__init__.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/flatten.py` & `scisoftpy-2.29.1/scisoftpy/flatten.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/image.py` & `scisoftpy-2.29.1/scisoftpy/image.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/io.py` & `scisoftpy-2.29.1/scisoftpy/io.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/fitcore.py` & `scisoftpy-2.29.1/scisoftpy/jython/fitcore.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/function.py` & `scisoftpy-2.29.1/scisoftpy/jython/function.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jybeans.py` & `scisoftpy-2.29.1/scisoftpy/jython/jybeans.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jycomparisons.py` & `scisoftpy-2.29.1/scisoftpy/jython/jycomparisons.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jycore.py` & `scisoftpy-2.29.1/scisoftpy/jython/jycore.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jycrystallography.py` & `scisoftpy-2.29.1/scisoftpy/jython/jycrystallography.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jydata.py` & `scisoftpy-2.29.1/scisoftpy/jython/jydata.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jydiffraction.py` & `scisoftpy-2.29.1/scisoftpy/jython/jydiffraction.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jyfft.py` & `scisoftpy-2.29.1/scisoftpy/jython/jyfft.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jyflatten.py` & `scisoftpy-2.29.1/scisoftpy/jython/jyflatten.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jyhdf5io.py` & `scisoftpy-2.29.1/scisoftpy/jython/jyhdf5io.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jyimage.py` & `scisoftpy-2.29.1/scisoftpy/jython/jyimage.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jyio.py` & `scisoftpy-2.29.1/scisoftpy/jython/jyio.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jylinalg.py` & `scisoftpy-2.29.1/scisoftpy/jython/jylinalg.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jymaths.py` & `scisoftpy-2.29.1/scisoftpy/jython/jymaths.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jynxio.py` & `scisoftpy-2.29.1/scisoftpy/jython/jynxio.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jyplot.py` & `scisoftpy-2.29.1/scisoftpy/jython/jyplot.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jyplottingsystem.py` & `scisoftpy-2.29.1/scisoftpy/jython/jyplottingsystem.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jyrandom.py` & `scisoftpy-2.29.1/scisoftpy/jython/jyrandom.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jyroi.py` & `scisoftpy-2.29.1/scisoftpy/jython/jyroi.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jyrpc.py` & `scisoftpy-2.29.1/scisoftpy/jython/jyrpc.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jyscisoft.py` & `scisoftpy-2.29.1/scisoftpy/jython/jyscisoft.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jysignal.py` & `scisoftpy-2.29.1/scisoftpy/jython/jysignal.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/jython/jywrapper.py` & `scisoftpy-2.29.1/scisoftpy/jython/jywrapper.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/linalg.py` & `scisoftpy-2.29.1/scisoftpy/linalg.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/nexus/__init__.py` & `scisoftpy-2.29.1/scisoftpy/nexus/__init__.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/nexus/hdf5.py` & `scisoftpy-2.29.1/scisoftpy/nexus/hdf5.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/nexus/nxclasses.py` & `scisoftpy-2.29.1/scisoftpy/nexus/nxclasses.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/nexus/utils.py` & `scisoftpy-2.29.1/scisoftpy/nexus/utils.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/plot.py` & `scisoftpy-2.29.1/scisoftpy/plot.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/python/pybeans.py` & `scisoftpy-2.29.1/scisoftpy/python/pybeans.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/python/pycomparisons.py` & `scisoftpy-2.29.1/scisoftpy/python/pycomparisons.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/python/pycore.py` & `scisoftpy-2.29.1/scisoftpy/python/pycore.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,23 @@
 ###
 
 '''
 '''
 
 import numpy as _np #@UnresolvedImport
 
-from distutils.version import LooseVersion
-
-_np_version_cur = LooseVersion(_np.version.version)
-_is_np_version_ge_1_8 = _np_version_cur >= LooseVersion('1.8')
-_is_np_version_ge_1_18 = _np_version_cur >= LooseVersion('1.18')
+import sys
+if sys.hexversion < 0x030a0000:
+    from distutils.version import LooseVersion as _Version
+else:
+    from packaging.version import parse as _Version
+
+_np_version_cur = _Version(_np.version.version)
+_is_np_version_ge_1_8 = _np_version_cur >= _Version('1.8')
+_is_np_version_ge_1_18 = _np_version_cur >= _Version('1.18')
 
 newaxis = _np.newaxis
 
 ndarray = _np.ndarray
 generic = ndgeneric = _np.generic
 bool = _np.bool_ #@ReservedAssignment
 int8 = _np.int8
```

### Comparing `scisoftpy-2.29.0/scisoftpy/python/pyflatten.py` & `scisoftpy-2.29.1/scisoftpy/python/pyflatten.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/python/pyh5py.py` & `scisoftpy-2.29.1/scisoftpy/python/pyh5py.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,84 +58,85 @@
             raise io_exception(e)
         finally:
             pass
 
         if fh is None:
             raise io_exception("No tree found")
 
-        ds = fh[self.name]
-
-        slices,sliced = _key2slice(key, self.shape)
-        dshape = [ l if s is None else len(list(range(*s.indices(l)))) for s, l in zip(slices, self.shape)] # destination shape
-        nshape = [ l for f,l in zip(sliced, dshape) if f ]
-#        print 'new shape:', nshape
-
-        if self.chunking is None:
-            if len(self.shape) == 0 and key is Ellipsis:
-                return ds[...]
-
-            nslices = [ s if s else slice(None) for s in slices ]
-            v = ds[tuple(nslices)]
-            if isinstance(v, ndarray):
-                return v.reshape(nshape)
-            return v
-
-        split = [ c <= 1 or l > 1 for c, l in zip(self.chunking, dshape) ]
         try:
-            split.index(False)
-        except:
-            nslices = [ s if s else slice(None) for s in slices ]
-            v = ds[tuple(nslices)]
-            return v.reshape(nshape)
-
-        # load slice-by-slice
-        v = zeros(dshape, dtype=self.dtype)
-
-        ssize = 1 # slice size
-        for i in range(self.rank):
-            if split[i]:
-                dshape[i] = 1
-            else:
-                ssize *= dshape[i]
-            
-
-        if ssize == 1:
-            for i in reversed(list(range(self.rank))):
-                l = v.shape[i]
-                if l > 1:
-                    dshape[i] = l
-                    split[i] = False
-                    ssize = l
-                    break
-
-        # iterate over split dimensions
-        dst_ranges = [ list(range(l)) for f, l in zip(split, v.shape) if f ]
-        dst_iter = product(*dst_ranges)
-
-        src_ranges = [ list(range(*s.indices(l))) if s else list(range(l)) for f, l, s in zip(split, self.shape, slices) if f ]
-        src_iter = product(*src_ranges)
-
-        for d,s in zip(dst_iter, src_iter):
-            dst_pos = []
-            src_pos = []
-            p = 0
+            ds = fh[self.name]
+    
+            slices,sliced = _key2slice(key, self.shape)
+            dshape = [ l if s is None else len(list(range(*s.indices(l)))) for s, l in zip(slices, self.shape)] # destination shape
+            nshape = [ l for f,l in zip(sliced, dshape) if f ]
+    #        print 'new shape:', nshape
+    
+            if self.chunking is None:
+                if len(self.shape) == 0 and key is Ellipsis:
+                    return ds[...]
+    
+                nslices = [ s if s else slice(None) for s in slices ]
+                v = ds[tuple(nslices)]
+                if isinstance(v, ndarray):
+                    return v.reshape(nshape)
+                return v
+    
+            split = [ c <= 1 or l > 1 for c, l in zip(self.chunking, dshape) ]
+            try:
+                split.index(False)
+            except:
+                nslices = [ s if s else slice(None) for s in slices ]
+                v = ds[tuple(nslices)]
+                return v.reshape(nshape)
+    
+            # load slice-by-slice
+            v = zeros(dshape, dtype=self.dtype)
+    
+            ssize = 1 # slice size
             for i in range(self.rank):
                 if split[i]:
-                    dst_pos.append(d[p])
-                    src_pos.append(s[p])
-                    p += 1
+                    dshape[i] = 1
                 else:
-                    dst_pos.append(slice(None))
-                    sl = slices[i]
-                    src_pos.append(sl if sl else slice(None))
-
-#            print dst_pos, src_pos
-            v[tuple(dst_pos)] = ds[tuple(src_pos)]
-
-        fh.close()
+                    ssize *= dshape[i]
+                
+    
+            if ssize == 1:
+                for i in reversed(list(range(self.rank))):
+                    l = v.shape[i]
+                    if l > 1:
+                        dshape[i] = l
+                        split[i] = False
+                        ssize = l
+                        break
+    
+            # iterate over split dimensions
+            dst_ranges = [ list(range(l)) for f, l in zip(split, v.shape) if f ]
+            dst_iter = product(*dst_ranges)
+    
+            src_ranges = [ list(range(*s.indices(l))) if s else list(range(l)) for f, l, s in zip(split, self.shape, slices) if f ]
+            src_iter = product(*src_ranges)
+    
+            for d,s in zip(dst_iter, src_iter):
+                dst_pos = []
+                src_pos = []
+                p = 0
+                for i in range(self.rank):
+                    if split[i]:
+                        dst_pos.append(d[p])
+                        src_pos.append(s[p])
+                        p += 1
+                    else:
+                        dst_pos.append(slice(None))
+                        sl = slices[i]
+                        src_pos.append(sl if sl else slice(None))
+    
+    #            print dst_pos, src_pos
+                v[tuple(dst_pos)] = ds[tuple(src_pos)]
+        finally:
+            fh.close()
         return v.reshape(nshape)
 
 
 class SDS(_dataset):
     def __init__(self, dataset, attrs={}, parent=None, warn=True):
         '''Make a SDS
         
@@ -169,17 +170,19 @@
 
         if fh is None:
             raise io_exception("No tree found")
 
         self.warn = warn
         # convert tree to own tree
         pool = dict()
-        t = self._copynode(pool, fh)
-        pool.clear()
-        fh.close()
+        try:
+            t = self._copynode(pool, fh)
+            pool.clear()
+        finally:
+            fh.close()
         return t
 
     def _mkgroup(self, node, attrs, parent):
         if parent is None:
             return _tree(node.filename, attrs)
         return _group(attrs, parent, self.warn)
```

### Comparing `scisoftpy-2.29.0/scisoftpy/python/pyhdf5io.py` & `scisoftpy-2.29.1/scisoftpy/python/pyhdf5io.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/python/pyio.py` & `scisoftpy-2.29.1/scisoftpy/python/pyio.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,32 +457,36 @@
         if self.load_metadata:
             metadata = dict()
         else:
             metadata = None
 
         t = _tf.TiffFile(self.name)
 
-        if stack:
-            data.append(("stack", t.asarray()))
-        else:
-            for i, p in enumerate(t.pages):
-                d = p.asarray()
-                data.append(("image-%02d" % (i+1,), d))
-                if self.load_metadata:
-                    for k,v in p.tags.items():
-                        metadata[k] = v.value
+        try:
+            if stack:
+                data.append(("stack", t.asarray()))
+            else:
+                for i, p in enumerate(t.pages):
+                    d = p.asarray()
+                    data.append(("image-%02d" % (i+1,), d))
+                    if self.load_metadata:
+                        for k,v in p.tags.items():
+                            metadata[k] = v.value
+    
+            pho = t.pages[0].photometric
+            if pho == pho.RGB:
+                # convert to an rgb dataset
+                for i, d in enumerate(data):
+                    di = _core.asarray(d[1], dtype=_core.int16).view(_RGB)
+                    if not self.ascolour:
+                        di = di.get_grey()
+                    data[i] = (d[0], di)
+        finally:
+            t.close()
 
-        pho = t.pages[0].photometric
-        if pho == pho.RGB:
-            # convert to an rgb dataset
-            for i, d in enumerate(data):
-                di = _core.asarray(d[1], dtype=_core.int16).view(_RGB)
-                if not self.ascolour:
-                    di = di.get_grey()
-                data[i] = (d[0], di)
         return DataHolder(data, metadata, warn)
 
 if _tf is None:
     TIFFLoader = ImageLoader
 else:
     TIFFLoader = TIFFfileLoader
```

### Comparing `scisoftpy-2.29.0/scisoftpy/python/pymaths.py` & `scisoftpy-2.29.1/scisoftpy/python/pymaths.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/python/pynxio.py` & `scisoftpy-2.29.1/scisoftpy/python/pynxio.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/python/pyplot.py` & `scisoftpy-2.29.1/scisoftpy/python/pyplot.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/python/pyplottingsystem.py` & `scisoftpy-2.29.1/scisoftpy/python/pyplottingsystem.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/python/pyroi.py` & `scisoftpy-2.29.1/scisoftpy/python/pyroi.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/python/pyrpc.py` & `scisoftpy-2.29.1/scisoftpy/python/pyrpc.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/python/pyscisoft.py` & `scisoftpy-2.29.1/scisoftpy/python/pyscisoft.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/python/pysignal.py` & `scisoftpy-2.29.1/scisoftpy/python/pysignal.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/python/pywrapper.py` & `scisoftpy-2.29.1/scisoftpy/python/pywrapper.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/random.py` & `scisoftpy-2.29.1/scisoftpy/random.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/roi.py` & `scisoftpy-2.29.1/scisoftpy/roi.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/rpc.py` & `scisoftpy-2.29.1/scisoftpy/rpc.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy/signal.py` & `scisoftpy-2.29.1/scisoftpy/signal.py`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/scisoftpy.egg-info/PKG-INFO` & `scisoftpy-2.29.1/scisoftpy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scisoftpy
-Version: 2.29.0
+Version: 2.29.1
 Summary: DAWN Python Extensions
 Home-page: https://gerrit.diamond.ac.uk/plugins/gitiles/scisoft/scisoft-core
 Author: Peter Chang
 Author-email: dataanalysis@diamond.ac.uk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `scisoftpy-2.29.0/scisoftpy.egg-info/SOURCES.txt` & `scisoftpy-2.29.1/scisoftpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scisoftpy-2.29.0/setup.py` & `scisoftpy-2.29.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="scisoftpy",
-    version="2.29.0",
+    version="2.29.1",
     description="DAWN Python Extensions",
     author="Peter Chang",
     author_email="dataanalysis@diamond.ac.uk",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
@@ -16,17 +16,18 @@
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     packages=find_packages(exclude=["uk*"]),
     install_requires=[
         "h5py", # depends on numpy
-        "pillow",
+        "Pillow",
         "six",
+        "packaging; python_version >= '3.10'",
         "subprocess32; python_version < '3' and os_name == 'posix'"
     ],
     extra_requires={
-        "all": [ "tifffile", "pycbf; python_version >= '3'" ],
+        "all": [ "tifffile[all]", "pycbf[all]; python_version >= '3'" ],
     },
     zip_safe=True,
     url="https://gerrit.diamond.ac.uk/plugins/gitiles/scisoft/scisoft-core",
 )
```

