# Comparing `tmp/MCSimPython-0.1.3.tar.gz` & `tmp/MCSimPython-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MCSimPython-0.1.3.tar", last modified: Fri May  5 08:38:33 2023, max compression
+gzip compressed data, was "MCSimPython-0.1.4.tar", last modified: Tue May  9 14:32:18 2023, max compression
```

## Comparing `MCSimPython-0.1.3.tar` & `MCSimPython-0.1.4.tar`

### file list

```diff
@@ -1,67 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.128327 MCSimPython-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-05 08:37:48.000000 MCSimPython-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-05 08:37:48.000000 MCSimPython-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-05 08:38:33.128327 MCSimPython-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-05 08:37:48.000000 MCSimPython-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:38:33.128327 MCSimPython-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.092327 MCSimPython-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.092327 MCSimPython-0.1.3/src/MCSimPython/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 08:38:24.000000 MCSimPython-0.1.3/src/MCSimPython/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.096327 MCSimPython-0.1.3/src/MCSimPython/control/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/control/adaptiveFS.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/control/backstepping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/control/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.096327 MCSimPython-0.1.3/src/MCSimPython/guidance/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/guidance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/guidance/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/guidance/path_param.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.096327 MCSimPython-0.1.3/src/MCSimPython/observer/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/observer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/observer/ekf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/observer/ltv_kf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/observer/nonlinobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.096327 MCSimPython-0.1.3/src/MCSimPython/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/simulator/csad.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/simulator/gunnerus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/simulator/thruster_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/simulator/vessel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.096327 MCSimPython-0.1.3/src/MCSimPython/thrust_allocation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/thrust_allocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/thrust_allocation/allocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/thrust_allocation/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/thrust_allocation/thruster.py
--rw-r--r--   0 runner    (1001) docker     (123)    27663 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.096327 MCSimPython-0.1.3/src/MCSimPython/vessel_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.100327 MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/freqs.npy
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/headings.npy
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/thruster_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json
--rw-r--r--   0 runner    (1001) docker     (123)  1961336 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/vessel_json.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.120327 MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2939897 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl
--rw-r--r--   0 runner    (1001) docker     (123)  5568933 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/rvg_config.json
--rw-r--r--   0 runner    (1001) docker     (123)  4723068 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/vessel.json
--rw-r--r--   0 runner    (1001) docker     (123)  4733857 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/vessel_2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.128327 MCSimPython-0.1.3/src/MCSimPython/waves/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/waves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19467 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/waves/wave_loads.py
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/waves/wave_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/src/MCSimPython/waves/wave_spreading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.092327 MCSimPython-0.1.3/src/MCSimPython.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-05 08:38:33.000000 MCSimPython-0.1.3/src/MCSimPython.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-05 08:38:33.000000 MCSimPython-0.1.3/src/MCSimPython.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:38:33.000000 MCSimPython-0.1.3/src/MCSimPython.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 08:38:33.000000 MCSimPython-0.1.3/src/MCSimPython.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 08:38:33.000000 MCSimPython-0.1.3/src/MCSimPython.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:38:33.128327 MCSimPython-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-05 08:37:51.000000 MCSimPython-0.1.3/tests/test_wave_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:18.458230 MCSimPython-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-09 14:29:20.000000 MCSimPython-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-09 14:29:20.000000 MCSimPython-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-09 14:32:18.458230 MCSimPython-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-09 14:29:20.000000 MCSimPython-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 14:32:18.458230 MCSimPython-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:18.422230 MCSimPython-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:18.422230 MCSimPython-0.1.4/src/MCSimPython/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 14:32:08.000000 MCSimPython-0.1.4/src/MCSimPython/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:18.422230 MCSimPython-0.1.4/src/MCSimPython/control/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/control/adaptiveFS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/control/backstepping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/control/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:18.422230 MCSimPython-0.1.4/src/MCSimPython/guidance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/guidance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/guidance/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/guidance/path_param.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:18.422230 MCSimPython-0.1.4/src/MCSimPython/observer/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/observer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/observer/ekf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/observer/ltv_kf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/observer/nonlinobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:18.426230 MCSimPython-0.1.4/src/MCSimPython/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/simulator/csad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/simulator/gunnerus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/simulator/thruster_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/simulator/vessel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:18.426230 MCSimPython-0.1.4/src/MCSimPython/thrust_allocation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/thrust_allocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/thrust_allocation/allocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/thrust_allocation/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/thrust_allocation/thruster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45304 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:18.426230 MCSimPython-0.1.4/src/MCSimPython/vessel_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:18.426230 MCSimPython-0.1.4/src/MCSimPython/vessel_data/CSAD/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/CSAD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/CSAD/freqs.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/CSAD/headings.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/CSAD/thruster_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1961336 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/CSAD/vessel_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:18.454230 MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2939897 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  5603889 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/rvg2_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/rvg3ABC_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/rvg3ABC_config_.json
+-rw-r--r--   0 runner    (1001) docker     (123)  5611180 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/rvg3_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)  5568933 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/rvg_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4723068 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/vessel.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4733857 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/vessel_2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:18.458230 MCSimPython-0.1.4/src/MCSimPython/waves/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/waves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/waves/wave_loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/waves/wave_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/src/MCSimPython/waves/wave_spreading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:18.422230 MCSimPython-0.1.4/src/MCSimPython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-09 14:32:18.000000 MCSimPython-0.1.4/src/MCSimPython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-09 14:32:18.000000 MCSimPython-0.1.4/src/MCSimPython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:32:18.000000 MCSimPython-0.1.4/src/MCSimPython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-09 14:32:18.000000 MCSimPython-0.1.4/src/MCSimPython.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 14:32:18.000000 MCSimPython-0.1.4/src/MCSimPython.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:32:18.458230 MCSimPython-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-09 14:29:23.000000 MCSimPython-0.1.4/tests/test_wave_spectra.py
```

### Comparing `MCSimPython-0.1.3/LICENSE` & `MCSimPython-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/PKG-INFO` & `MCSimPython-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCSimPython
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python vessel simulation environment
 Author-email: Jan-Erik Hygen <janereh@stud.ntnu.no>
 Keywords: mcsim,MCSimPython,DP,dynamic positioning,Marine Cybernetics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `MCSimPython-0.1.3/README.md` & `MCSimPython-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/pyproject.toml` & `MCSimPython-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/control/adaptiveFS.py` & `MCSimPython-0.1.4/src/MCSimPython/control/adaptiveFS.py`

 * *Files 12% similar despite different names*

```diff
@@ -138,10 +138,23 @@
         Parameters
         -----------
             - w_min: Lower bound frequency
             - w_max: Upper bound frequency
             - N: Number of components
         '''
         self._N = N
-        dw = (w_max-w_min)/ self._N
-        self._freqs = np.arange(w_min, w_max, dw)
+        try:
+            dw = (w_max-w_min)/ self._N
+            self._freqs = np.arange(w_min, w_max, dw)
+        except ZeroDivisionError:
+            self._freqs = np.array([])
+            
+
+    def set_tuning_params(self, K1: list, K2: list, gamma: list):
+        self._K1 = np.diag(K1)
+        self._K2 = np.diag(K2)
+        #self._gamma = np.eye((2*self._N +1)*3) * gamma
+        if len(gamma) != (2*self._N +1)*3:
+            raise ValueError
+        self._gamma = np.diag(gamma)
+
```

### Comparing `MCSimPython-0.1.3/src/MCSimPython/control/backstepping.py` & `MCSimPython-0.1.4/src/MCSimPython/control/backstepping.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/control/basic.py` & `MCSimPython-0.1.4/src/MCSimPython/control/basic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # basic.py
 
 # ----------------------------------------------------------------------------
 # This code is part of the MCSimPython toolbox and repository.
 # Created By: Jan-Erik Hygen
 # Created Date: 2023-01-30
 # Revised: 2023-02 - Added Direct Bias Compensation Controller - Harald Mo
+#          2023-05 - Added PI controller - Harald Mo
+#
 # Tested:
 # 
 # Copyright (C) 2023: NTNU, Trondheim
 # Licensed under GPL-3.0-or-later
 # ---------------------------------------------------------------------------
 
 import numpy as np
@@ -90,14 +92,49 @@
         z2 = nu - nu_d
 
         self.zi[:2] += self.dt*(eta[:2] - eta_d[:2])
         self.zi[2] += self.dt*pipi(eta[2] - eta_d[2])
         return -self.Kp@z1 - self.Kd@z2 - Rz(psi).T@self.Ki@self.zi
 
 
+class PI:
+    """Proportional control with integral action."""
+
+    def __init__(self, kp: list, ki: list, dt: float = 0.01):
+        self.Kp = np.diag(kp)
+        self.Ki = np.diag(ki)
+        self.zi = np.zeros(3)
+        self.dt = dt
+
+    def get_tau(self, eta, eta_d):
+        """Calculate control loads.
+        
+        Parameters
+        ----------
+        eta : array_like
+            Vessel pose in surge, sway and yaw.
+        eta_d : array_like
+            Desired vessel pose in surge, sway and yaw (NED-frame).
+        
+        Returns
+        -------
+        tau : array_like
+            Controller load in surge, sway, and yaw (body-frame).
+        """
+        psi = eta[-1]
+
+        eta_tilde = eta - eta_d
+        eta_tilde[-1] = pipi(eta_tilde[-1])
+
+        z1 = Rz(psi).T@eta_tilde
+
+        self.zi += self.dt*(eta_tilde)
+
+        return -self.Kp@z1 - Rz(psi).T@self.Ki@self.zi
+    
 
 class DirectBiasCompensationController():
     '''
     Bias estimate provided from the observer as direct compensation in a nominal PD control law.
     '''
     def __init__(self, kp: list, kd: list):
```

### Comparing `MCSimPython-0.1.3/src/MCSimPython/guidance/__init__.py` & `MCSimPython-0.1.4/src/MCSimPython/guidance/__init__.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/guidance/filter.py` & `MCSimPython-0.1.4/src/MCSimPython/guidance/filter.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/guidance/path_param.py` & `MCSimPython-0.1.4/src/MCSimPython/guidance/path_param.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/observer/__init__.py` & `MCSimPython-0.1.4/src/MCSimPython/observer/__init__.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/observer/ekf.py` & `MCSimPython-0.1.4/src/MCSimPython/observer/ekf.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/observer/ltv_kf.py` & `MCSimPython-0.1.4/src/MCSimPython/observer/ltv_kf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # ltv_kf.py
 # ----------------------------------------------------------------------------
 # This code is part of the MCSimPython toolbox and repository.
-# Created By: Harald Mo
+# Created By:   Harald Mo
 # Created Date: 2023-05-03
-# 
+# Revised:      2023-05-09 Harald Mo        Added dead reckoning
+#
+#
 # Copyright (C) 2023: NTNU, Trondheim
 # Licensed under GPL-3.0-or-later
 # ---------------------------------------------------------------------------
 
 import numpy as np
 from MCSimPython.utils import Rz, pipi, six2threeDOF, three2sixDOF
 
@@ -114,15 +116,15 @@
         self._Ed = np.zeros((15,6))
         self._Ed[3:6,0:3], self._Ed[9:12,3:6] = np.diag([1,1,1])*self._dt, np.eye(3)*self._dt
 
         self._H = np.zeros((3,15))
         self._H[0:3,3:6], self._H[0:3,6:9] = np.eye(3), np.eye(3)
 
 
-    def update(self, tau, y, psi_m, asynchronous = False):
+    def update(self, tau, y, psi_m, asynchronous = False, dead_reckoning = False):
         '''
         Update:
         Update function to be called at every timestep during a simulation. Calls the predictor and corrector.
 
         Parameters
         ----------
             - tau: Control Parameters (3DOF)
@@ -132,33 +134,33 @@
         '''
 
         if asynchronous:
             self.update_async(tau, y, psi_m)
             return None
         
         # Correct
-        self.corrector(y)
+        self.corrector(y, dead_reckoning)
         # Predict        
         self.predictor(tau, psi_m)
     
 
     def update_async(self, tau, y, psi_m):
-        return NotImplementedError
+        raise NotImplementedError
     
         
     
     def predictor(self, tau, psi_m):
         Ad =  self.Ad(psi_m)   # Get the time-varying state matrix
 
         self.xbar = Ad@self.xhat + self._Bd@tau
         self.Pbar = Ad@self.Phat@Ad.T + self._Ed@self.Qd@self._Ed.T
 
     
-    def corrector(self, y):
-        if np.any(np.isnan(y)) == True:    # If no new measurements: Set corrector equal to predictor (Dead reckoning)
+    def corrector(self, y, dead_reckoning):
+        if dead_reckoning:    # If dead reckoning: Set corrector equal to predictor (Dead reckoning)
             self.Phat = self.Pbar
             self.xhat = self.xbar
         else:
             K = self.KF_gain
             prediction_error = y - (self._H@self.xbar)
             prediction_error[2] = pipi(prediction_error[2])   # Smallest signed angle modification
 
@@ -191,15 +193,15 @@
         Calculate the time-varying matrix Ad in x_dot = Ad*x + Bd*u + Ed*w
 
         A(t)= [Aw       0_(6x3)     0_(6x3)         0_(6x3)    \n
               0_(3x6)   0_(3x3)     0_(3x3)         R(t)        \n
               0_(3x6)   0_(3x3)     0_(3x3)         0_(3x3)     \n
               0_(3x6)   0_(3x3)     M_inv*R(t).T    -M_inv*D ]
         and 
-        Ad = e^(dt*A)   OR   Ad = I + dt * A
+        Ad = I + dt * A
         '''
         A = np.block([
             [self._Aw,          np.zeros((6,3)),    np.zeros((6,3)),      np.zeros((6,3))],
             [np.zeros((3,6)),   np.zeros((3,3)),    np.zeros((3,3)),      Rz(psi_m)],
             [np.zeros((3,6)),   np.zeros((3,3)),    np.zeros((3,3)),      np.zeros((3,3)),],
             [np.zeros((3,6)),   np.zeros((3,3)),    self._Minv@Rz(psi_m).T, -self._Minv@self._D]
         ])
```

### Comparing `MCSimPython-0.1.3/src/MCSimPython/observer/nonlinobs.py` & `MCSimPython-0.1.4/src/MCSimPython/observer/nonlinobs.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/simulator/__init__.py` & `MCSimPython-0.1.4/src/MCSimPython/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/simulator/csad.py` & `MCSimPython-0.1.4/src/MCSimPython/simulator/csad.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/simulator/gunnerus.py` & `MCSimPython-0.1.4/src/MCSimPython/simulator/gunnerus.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/simulator/thruster_dynamics.py` & `MCSimPython-0.1.4/src/MCSimPython/simulator/thruster_dynamics.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/simulator/vessel.py` & `MCSimPython-0.1.4/src/MCSimPython/simulator/vessel.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/thrust_allocation/allocation.py` & `MCSimPython-0.1.4/src/MCSimPython/thrust_allocation/allocation.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/thrust_allocation/constraints.py` & `MCSimPython-0.1.4/src/MCSimPython/thrust_allocation/constraints.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/thrust_allocation/thruster.py` & `MCSimPython-0.1.4/src/MCSimPython/thrust_allocation/thruster.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/utils.py` & `MCSimPython-0.1.4/src/MCSimPython/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Utility functions
 
 # ----------------------------------------------------------------------------
 # This code is part of the MCSimPython toolbox and repository.
 # Created By: Jan-Erik Hygen
 # Created Date: 2022-10-12
 # Revised: 2023-02-09 Harald Mo    Add from/to 6 and 3DOF functions
+#          2023-05-07 Jan-Erik Hygen add fluid memory estimation
 # 
 # Tested:  See tests/test_utils.py
 # 
 # Copyright (C) 202x: NTNU, Trondheim
 # Licensed under GPL-3.0-or-later
 # ---------------------------------------------------------------------------
 
@@ -16,14 +17,18 @@
 from time import time
 from scipy.signal import welch
 import matplotlib.pyplot as plt
 import re
 import os
 import json
 
+from scipy.signal import TransferFunction
+from scipy.optimize import least_squares
+
+
 dof3_matrix_mask = np.ix_([0, 1, 5], [0, 1 ,5])
 dof3_array = np.ix_([0, 1, 5])
 
 def complex_to_polar(complex_values):
     """Complex value to polar coordinates.
     
     Parameters
@@ -545,14 +550,24 @@
         run_info.append(f.readline())
 
     rhow, g = data2num(run_info[0])
     lpp, breadth, draught = data2num(run_info[1])
     LCG, VCG = data2num(run_info[2])
     version, *_ = data2int(run_info[3])
     print(f"Version = {version}")
+    
+    # Gravity vector in body-fixed frame
+    r_g = np.array([-LCG, 0, 0])
+    
+    # Transformation matrices
+    T = np.diag([-1, 1, -1, -1, 1, -1])
+    H = np.block([
+        [np.eye(3), Smat(r_g).T],
+        [np.zeros((3, 3)), np.eye(3)]
+    ])
 
     novel, nohead, nofreq, nodof = data2int(f.readline())
 
     A = np.zeros((nodof, nodof, nofreq, novel))
     A_added = np.zeros_like(A)
     B = np.zeros_like(A)
     B_added = np.zeros_like(B)
@@ -562,14 +577,16 @@
     Bv44_nonlin = np.zeros_like(Bv44_linear)
     Bv44_linearized = np.zeros_like(Bv44_linear)
 
     Mrb = np.zeros((nodof, nodof))
     for i in range(nodof):
         Mrb[i] = [m for m in data2num(f.readline())]
 
+    nabla = float(Mrb[0, 0]/rhow)
+
     for v in range(novel):
         vel, *_ = data2float(f.readline())
         for h in range(nohead):
             head, *_ = data2float(f.readline())
             for j in range(nofreq):
                 freq, *_ = data2float(f.readline())
                 for k in range(nodof):
@@ -597,17 +614,30 @@
                         temp = f.readline()
                         C_added[k, :, j, v] = np.array([cc for cc in data2num(temp)])
                 bv_l, bv_nl, bv_ll, *_ = data2num(f.readline())
                 Bv44_linear[j, h, v] = bv_l
                 Bv44_nonlin[j, h, v] = bv_nl
                 Bv44_linearized[j, h, v] = bv_ll
     
-
     f.close()
-    return Mrb, A, B, C, Bv44_linear, Bv44_nonlin, Bv44_linearized
+    
+    # Transforming coefficients from CG to CO and from from Veres to MCSimPython axis system.
+    Mrb_co = H.T@T@Mrb@T@H
+    
+    A_co = np.zeros_like(A)
+    B_co = np.zeros_like(B)
+    C_co = np.zeros_like(C)
+    
+    for v in range(novel):
+        for f in range(nofreq):
+            A_co[:, :, f, v] = H.T@T@A[:, :, f, v]@T@H
+            B_co[:, :, f, v] = H.T@T@B[:, :, f, v]@T@H
+            C_co[:, :, f, v] = H.T@T@C[:, :, f, v]@T@H
+    
+    return Mrb_co, A_co, B_co, C_co, Bv44_linear, Bv44_nonlin, Bv44_linearized, nabla, rhow, lpp
 
 
 def read_wave_drift(filepath):
     f = open(filepath, 'r')
 
     header = []
     run_info = []
@@ -821,19 +851,27 @@
     print("Read motion RAOs (.re1)...")
     freqs, headings, vels, motion_rao_c, motion_rao_amp, motion_rao_phase = read_tf(re1)
     print("Read force RAOs (.re8)...")
     _, _, _, force_rao_c, force_rao_amp, force_rao_phase = read_tf(re8)
     print("Read wave drift data (.re2)...")
     drift_frc = read_wave_drift(re2)
     print("Read hydrodynamic parameters (.re7)...")
-    Mrb, A, B, C, Bv44_lin, Bv44_nonlin, Bv44_linearized = read_hydrod(re7)
+    Mrb, A, B, C, Bv44_lin, Bv44_nonlin, Bv44_linearized, nabla, rhow, lpp = read_hydrod(re7)
     print("COMPLETE".center(100, '.'))
     # Functions for reading the other files
-        ## ADD FUNCTIONS HERE
+    
+    # Add hydrodynamic data for surge. Based on Søding (1982)
+    A11_0 = 2.7*(rhow/lpp**2)*nabla**(5/3)
+    A22_0 = A[1, 1, 0, 0]
+    alpha = A11_0/A22_0
+    A[0, 0] = alpha*A[1, 1]
+    B[0, 0] = alpha*B[1, 1]
+    
     # Add the inputs to dictionary.
+    vessel_config['main'] = {'lpp': lpp, 'nabla': nabla, 'rhow': rhow}
     vessel_config['freqs'] = freqs.tolist()
     vessel_config['headings'] = headings.tolist()
     vessel_config['velocity'] = vels.tolist()
     vessel_config['motionRAO']['complex'] = motion_rao_c.tolist()
     vessel_config['motionRAO']['amp'] = motion_rao_amp.tolist()
     vessel_config['motionRAO']['phase'] = motion_rao_phase.tolist()
     vessel_config['motionRAO']['w'] = freqs.tolist()
@@ -846,22 +884,445 @@
     vessel_config['B'] = B.tolist()
     vessel_config['C'] = C.tolist()
     vessel_config['MRB'] = Mrb.tolist()
     vessel_config['Bv44']['Linear'] = Bv44_lin.tolist()
     vessel_config['Bv44']['Nonlin'] = Bv44_nonlin.tolist()
     vessel_config['Bv44']['Linearized'] = Bv44_linearized.tolist()
     Bv = np.zeros((6, 6))
-    # Bv[3, 3] = Bv44_linearized
-    vessel_config['Bv'] = np.zeros((6, 6)).tolist()   # Should add some viscous damping estimates here.
+    Bv[3, 3] = Bv44_lin[0, 0, 0]
+    vessel_config['Bv'] = Bv.tolist()   # Should add some viscous damping estimates here.
 
     if headings.size <= 19:
         print(f"VERES results only for heading {np.min(headings)} to {np.max(headings)}. ")
         _complete_sector_coeffs(vessel_config)
     elif np.max(headings) <= np.pi:
         print(f"VERES results only for headings {headings}.")
         raise NotImplementedError
     
     
     return vessel_config
-    # Add some saving method here.
     
-    
+    
+    
+# ---------- FLUID MEMEORY EFFECT ESTIMATION ------------
+
+# This can maybe be set in a separate file.
+
+def invfreqs(h, w, nb, na, weights=None, method=0, maxiter=40):
+    """
+    Estimate the numerator and denominator coefficients of a transfer function from
+    frequency response data using complex function curve fitting with quasi-linear least squares.
+
+    Parameters
+    ----------
+    h : array_like
+        The frequency response values.
+    w : array_like
+        The frequencies (in radians/sample) corresponding to the frequency response values.
+    nb : int
+        The order of the numerator.
+    na : int
+        The order of the denominator.
+    weights : array_like, optional
+        The weighting factors for the frequency response values. Default is None.
+
+    Returns
+    -------
+    b : ndarray
+        The estimated numerator coefficients of the transfer function.
+    a : ndarray
+        The estimated denominator coefficients of the transfer function.
+    success : bool
+        True if the fit succeeded, False otherwise.
+    """
+
+    # Check input arguments
+    h = np.asarray(h, dtype=complex)
+    w = np.asarray(w, dtype=float)
+    if len(h) != len(w):
+        raise ValueError("h and w must have the same length")
+    if nb <= 0:
+        raise ValueError("nb must be a positive integer")
+    if na <= 0:
+        raise ValueError("na must be a positive integer")
+
+    # Define the transfer function numerator and denominator functions
+    def transfer_function(w, b, a):
+        return np.polyval(b[::-1], 1j * w) / np.polyval(a[::-1], 1j * w)
+
+    # Define the objective function
+    def fun_residuals(params, w, h, weights):
+        b = params[:nb]
+        a = params[nb:]
+        ypred = transfer_function(w, b, a)
+        residuals = np.concatenate([np.real(ypred - h), np.imag(ypred - h)])
+        if weights is not None:
+            weights = np.asarray(weights)
+            weights = np.repeat(weights, 2)
+            residuals *= np.sqrt(weights)
+        return residuals
+
+    # Initialize the coefficients
+    p0 = np.random.randn(nb + na)
+    # p0 = np.ones(nb + na)
+
+    # Perform the quasi-linear least squares fitting
+
+    result = least_squares(fun_residuals, p0, args=(w, h, weights), loss='soft_l1')
+    if method==2:
+        print(f"Using iterative method.")
+        weights = np.ones_like(w)
+        for i in range(maxiter):
+            result = least_squares(fun_residuals, result.x, args=(w, h, weights), loss='soft_l1')
+            # weights = 1 / np.abs(transfer_function(w, result.x[:nb], result.x[nb:]))**2
+            weights = np.abs(np.polyval(_stabilize(result.x[nb:][::-1]), 1j * w))**2
+
+    return result.x[:nb], result.x[nb:], result.success
+
+
+def _invfreqs_alt(g, worN, nB, nA, wf=None, nk=0):
+    g = np.atleast_1d(g)
+    worN = np.atleast_1d(worN)
+    if wf is None:
+        wf = np.ones_like(worN)
+    if len(g)!=len(worN) or len(worN)!=len(wf):
+        raise ValueError("The lengths of g, worN and wf must coincide.")
+    if np.any(worN<0):
+        raise ValueError("worN has negative values.")
+    s = 1j*worN
+
+    # Constraining B(s) with nk trailing zeros
+    nm = np.maximum(nA, nB+nk)
+    mD = np.vander(1j*worN, nm+1)
+    mH = np.mat(np.diag(g))
+    mM = np.mat(np.hstack(( mH*np.mat(mD[:,-nA:]),\
+            -np.mat(mD[:,-nk-nB-1:][:,:nB+1]))))
+    mW = np.mat(np.diag(wf))
+    Y = np.linalg.solve(np.real(mM.H*mW*mM), -np.real(mM.H*mW*mH*np.mat(mD)[:,-nA-1]))
+    a = np.ones(nA+1)
+    a[1:] = Y[:nA].flatten()
+    b = np.zeros(nB+nk+1)
+    b[:nB+1] = Y[nA:].flatten()
+
+    return b,a
+
+def _stabilize(a):
+    """Stabilize the denominator polynomial by switching sign of real part for roots with real part > 1.
+    
+    Parameters
+    ----------
+    a : array_like
+        The denominator polynomial coefficients.
+    
+    Returns
+    -------
+    a : ndarray
+        The stabilized denominator polynomial coefficients.
+    """
+    # Find the roots of the denominator polynomial
+    r = np.roots(a)
+    
+    # Switch sign of real part for roots with real part > 1
+    r = np.where(np.real(r) > 0, -r, r)
+    
+    # Compute the stabilized denominator polynomial
+    return np.poly(r)
+    
+    
+
+def joint_identification(w, A, B, order, plot_estimate=False, method=0):
+    """Joint identification of infinity added mass and radiation forces.
+    
+    Parameters
+    ----------
+    w : array_like
+        The frequencies (in radians/sample) corresponding to the frequency response values.
+    A : array_like
+        The frequency response values of the added mass.
+    B : array_like
+        The frequency response values of the radiation forces.
+    order : int
+        The order of the numerator and denominator polynomials.
+    plot_estimate : bool, optional
+        If True, plot the estimated transfer function. Default is False.
+    
+    Returns
+    -------
+    Ma : ndarray
+        The estimated infinity added mass coefficients.
+    Arad : array_like
+        The system matrix of the radiation forces.
+    Brad : array_like
+        The input matrix of the radiation forces.
+    Crad : array_like
+        The output matrix of the radiation forces.
+    """
+    
+    # Compute the complex added mass coeficient.
+    Ac = B/(1j * w) + A
+    
+    # Scale the frequency response values for better prediction.
+    Ac_scaled = Ac / np.max(np.abs(Ac))
+    
+    num, den, success = invfreqs(Ac_scaled, w, order, order, method=method)
+    # num, den = _invfreqs_alt(Ac_scaled, w, order, order, wf=None)
+    # success = True
+    # if method == 2:
+    #     for i in range(40):
+    #         weights = 1/np.abs(np.polyval(den, 1j*w))**2
+    #         num, den = _invfreqs_alt(Ac_scaled, w, order, order, wf=weights)
+    # num = num[::-1]
+    # den = den[::-1]
+    if not success:
+        raise ValueError("Least squares fit failed")
+    if np.any(np.real(np.roots(den[::-1])) > 0):
+        print("WARNING: The estimated denominator has positive roots.")
+    # Rescale the coefficients.
+    num = num * np.max(np.abs(Ac))
+    
+    As = TransferFunction(num[::-1], den[::-1])
+    Ainf = As.num[0]
+    
+    # The 0th term represent prior knowledge of the transfer function, which should be zero at s=0.
+    Pik = np.concatenate((As.num - Ainf*As.den, [0]))
+    Qik = np.array(_stabilize(As.den))
+    
+    # Compute the estimated transfer function with relative degree 1.
+    H_hat = TransferFunction(Pik[2:], Qik)
+    Kw_hat = H_hat.freqresp(w)[1]
+    
+    Aest = np.imag(Kw_hat)/w + Ainf
+    Best = np.real(Kw_hat)
+    
+    if plot_estimate:
+        w_new = np.arange(w.min()*0.1, 10.01, 0.01)
+        fig, ax = plt.subplots(2, 2, constrained_layout=True)
+        plt.sca(ax[0, 0])
+        plt.title(f"Re (roots(As)) = {np.real(np.roots(As.den))}")
+        plt.plot(w, np.abs(Ac), 'o', label="Ac")
+        plt.plot(w_new, np.abs(As.freqresp(w_new)[1]), label="As")
+        plt.xlabel("Frequency [rad/s]")
+        plt.ylabel("Magnitude")
+        plt.legend()
+        
+        plt.sca(ax[1, 0])
+        plt.plot(w, np.angle(Ac), 'o', label="Ac")
+        plt.plot(w_new, np.angle(As.freqresp(w_new)[1]), label="As")
+        plt.xlabel("Frequency [rad/s]")
+        plt.ylabel("Phase [rad]")
+        plt.legend()
+        
+        Kw_hat_new = H_hat.freqresp(w_new)[1]
+        plt.sca(ax[0, 1])
+        plt.plot(w, A, 'o', label="A")
+        plt.plot(w_new, (np.imag(Kw_hat_new/w_new) + Ainf), label="Aest")
+        plt.legend()
+        plt.xlabel("Frequency [rad/s]")
+        
+        plt.sca(ax[1, 1])
+        plt.plot(w, B, 'o', label="B")
+        plt.plot(w_new, (np.real(Kw_hat_new)), label="Best")
+        plt.legend()
+        plt.xlabel("Frequency [rad/s]")
+        plt.show()
+        
+    
+    # TODO: Check for positive roots of the denominator. If roots are positive, the roots must be flipped sign to
+    #      obtain a stable system.
+    
+    return Ainf, Aest, Best, H_hat
+
+
+def system_identification(w, A, B, max_order=10, method=0, plot_estimate=False):
+    order = 2
+    treshold = 0.99
+    dofs = np.array([
+        [0, 0],
+        [1, 1],
+        [1, 3],
+        [1, 5],
+        [2, 2],
+        [2, 4],
+        [3, 3],
+        [3, 5],
+        [4, 4],
+        [5, 5]
+    ])
+    
+    MA = np.zeros((6, 6))
+    # Ar = [[[]]*6]*6
+    # Br = [[[]]*6]*6
+    # Cr = [[[]]*6]*6
+    Ar = [list(range(1 + 6 * i, 1 + 6 * (i + 1))) for i in range(6)]
+    Br = [list(range(1 + 6 * i, 1 + 6 * (i + 1))) for i in range(6)]
+    Cr = [list(range(1 + 6 * i, 1 + 6 * (i + 1))) for i in range(6)]
+    
+    
+    for dof_ik in dofs:
+        a = A[dof_ik[0], dof_ik[1], :]
+        b = B[dof_ik[0], dof_ik[1], :]
+        sucess = False
+        print(f"Running estimation for dof {dof_ik+1}")
+        while not sucess:
+            try:
+                if np.sum(a) == 0.:
+                    print("a is zero")
+                    break
+                a_inf_ik, a_est_ik, b_est_ik, kw_est_ik = joint_identification(w, a, b, order, method=method, plot_estimate=False)
+                # Compute some values to check if the fit is good.
+                sseb = np.sum((b - b_est_ik)**2)
+                sstb = np.sum((b - np.mean(b))**2)
+                rsqrb = 1 - sseb/sstb
+                
+                ssea = np.sum((a - a_est_ik)**2)
+                ssta = np.sum((a - np.mean(a))**2)
+                rsqra = 1 - ssea/ssta
+                if (rsqrb >= treshold) and (rsqra >= treshold):
+                    sucess = True
+                    print(f"Joint identification successful for DOF {dof_ik+1}. Order = {order}.")
+                    MA[dof_ik[0], dof_ik[1]] = a_inf_ik
+                    Krad = kw_est_ik.to_ss()
+                    Ar[dof_ik[0]][dof_ik[1]] = Krad.A.tolist()
+                    Br[dof_ik[0]][dof_ik[1]] = Krad.B.tolist()
+                    Cr[dof_ik[0]][dof_ik[1]] = Krad.C.tolist()
+                    
+                    if dof_ik[0] != dof_ik[1]:
+                        MA[dof_ik[1], dof_ik[0]] = a_inf_ik
+                        Ar[dof_ik[1]][dof_ik[0]] = Krad.A.tolist()
+                        Br[dof_ik[1]][dof_ik[0]] = Krad.B.tolist()
+                        Cr[dof_ik[1]][dof_ik[0]] = Krad.C.tolist()
+                        
+                    if plot_estimate:
+                        wmin = np.min(w)*.1
+                        wmax = 10
+                        w_new = np.arange(wmin, wmax+0.01, 0.01)
+                        Kw_hat_n = kw_est_ik.freqresp(w_new)[1]
+                        Aest_n = np.imag(Kw_hat_n)/w_new + a_inf_ik
+                        Best_n = np.real(Kw_hat_n)
+                        plt.figure()
+                        plt.title("Complex curve fit")
+                        plt.plot(w_new, np.abs(Kw_hat_n), '-', label='|Kw_hat|')
+                        plt.plot(w, np.abs(b + 1j*w*(a-a_inf_ik)), 'o', label='|Kw|')
+                        plt.legend()
+                        plt.show()
+                        
+                        fig, ax = plt.subplots(1, 2, figsize=(12, 6), constrained_layout=True)
+                        fig.suptitle(f"Joint identification of DOF {dof_ik+1} with order {order}")
+                        plt.sca(ax[0])
+                        plt.title("Estimated added mass.   rsqra = {:.3f}".format(rsqra))
+                        plt.plot(w, a, 'o', label='A')
+                        plt.plot(w_new, Aest_n, '-', label='Aest')
+                        plt.legend()
+                        
+                        plt.sca(ax[1])
+                        plt.title("Estimated damping.   rsqrb = {:.3f}".format(rsqrb))
+                        plt.plot(w, b, 'o', label='B')
+                        plt.plot(w_new, Best_n, '-', label='Best')
+                        plt.legend()
+                        
+                        plt.show()
+                if order > max_order:
+                    print("Could not find a good fit for order less than max_order = {}.".format(max_order))
+                    cont = input("Would you like to manually find best fit? [y/n] ")
+                    if cont.lower() == "y":
+                        order = int(input("Enter new order (recommended: 2-5): "))
+                    else:
+                        break
+                    print("Evaluate the transfer function and select order manually.")
+                    a_inf_ik, a_est_ik, b_est_ik, kw_est_ik = joint_identification(w, a, b, order, method=method, plot_estimate=plot_estimate)
+                    # Compute some values to check if the fit is good.
+                    sseb = np.sum((b - b_est_ik)**2)
+                    sstb = np.sum((b - np.mean(b))**2)
+                    rsqrb = 1 - sseb/sstb
+                    
+                    ssea = np.sum((a - a_est_ik)**2)
+                    ssta = np.sum((a - np.mean(a))**2)
+                    rsqra = 1 - ssea/ssta
+                    wmin = np.min(w)*.1
+                    wmax = 10
+                    w_new = np.arange(wmin, wmax+0.01, 0.01)
+                    Kw_hat_n = kw_est_ik.freqresp(w_new)[1]
+                    Aest_n = np.imag(Kw_hat_n)/w_new + a_inf_ik
+                    Best_n = np.real(Kw_hat_n)
+                    plt.figure()
+                    plt.title("Complex curve fit")
+                    plt.plot(w_new, np.abs(Kw_hat_n), '-', label='|Kw_hat|')
+                    plt.plot(w, np.abs(b + 1j*w*(a-a_inf_ik)), 'o', label='|Kw|')
+                    plt.legend()
+                    plt.show()
+                    
+                    fig, ax = plt.subplots(1, 2, figsize=(12, 6), constrained_layout=True)
+                    fig.suptitle(f"Joint identification of DOF {dof_ik+1} with order {order}")
+                    plt.sca(ax[0])
+                    plt.title("Estimated added mass.   rsqra = {:.3f}".format(rsqra))
+                    plt.plot(w, a, 'o', label='A')
+                    plt.plot(w_new, Aest_n, '-', label='Aest')
+                    plt.legend()
+                    
+                    plt.sca(ax[1])
+                    plt.title("Estimated damping.   rsqrb = {:.3f}".format(rsqrb))
+                    plt.plot(w, b, 'o', label='B')
+                    plt.plot(w_new, Best_n, '-', label='Best')
+                    plt.legend()
+                    
+                    plt.show()
+                    yn = input("If the fit is good, enter 'y' to continue. Otherwise, enter 'n' to run a different order. ")
+                    if yn.lower() == 'y':
+                        sucess = True
+                        print(f"Joint identification successful for DOF {dof_ik+1}. Order = {order}.")
+                        MA[dof_ik[0], dof_ik[1]] = a_inf_ik
+                        Krad = kw_est_ik.to_ss()
+                        Ar[dof_ik[0]][dof_ik[1]] = Krad.A.tolist()
+                        Br[dof_ik[0]][dof_ik[1]] = Krad.B.tolist()
+                        Cr[dof_ik[0]][dof_ik[1]] = Krad.C.tolist()
+                        
+
+                        if dof_ik[0] != dof_ik[1]:
+                            MA[dof_ik[1], dof_ik[0]] = a_inf_ik
+                            Ar[dof_ik[1]][dof_ik[0]] = Krad.A.tolist()
+                            Br[dof_ik[1]][dof_ik[0]] = Krad.B.tolist()
+                            Cr[dof_ik[1]][dof_ik[0]] = Krad.C.tolist()
+                    else:
+                        order = max_order + 1
+                        
+                else:
+                    order += 1
+                    
+            except ValueError:
+                print(f"Joint identification failed for {dof_ik}. Using order {order+1} instead.")
+                order += 1
+                if order > max_order:
+                    cont = input("Order exceeded maximum order. Continue? [y/n] ")
+                    if cont.lower() == "y":
+                        order = int(input("Enter new order (recommended: 2-5): "))
+                    else:
+                        break
+                continue
+        order = 2
+        sucess = False
+        
+    return MA, Ar, Br, Cr
+
+
+def quat2eul(w, x, y, z):
+    """
+    Returns the ZYX roll-pitch-yaw angles from a quaternion.
+    """
+    q = np.array((w, x, y, z))
+    #if np.abs(np.linalg.norm(q) - 1) > 1e-6:
+    #   raise RuntimeError('Norm of the quaternion must be equal to 1')
+
+    eta = q[0]
+    eps = q[1:]
+
+    S = Smat(eps)
+
+    R = np.eye(3) + 2 * eta * S + 2 * np.linalg.matrix_power(S, 2)
+
+    if np.abs(R[2, 0]) > 1.0:
+        raise RuntimeError('Solution is singular for pitch of +- 90 degrees')
+
+    roll = np.arctan2(R[2, 1], R[2, 2])
+    pitch = -np.arcsin(R[2, 0])
+    yaw = np.arctan2(R[1, 0], R[0, 0])
+
+    return np.array([roll, pitch, yaw])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json` & `MCSimPython-0.1.4/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/vessel_data/CSAD/vessel_json.json` & `MCSimPython-0.1.4/src/MCSimPython/vessel_data/CSAD/vessel_json.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json` & `MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl` & `MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl` & `MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/rvg_config.json` & `MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/rvg_config.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/vessel.json` & `MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/vessel.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/vessel_data/gunnerus/vessel_2.json` & `MCSimPython-0.1.4/src/MCSimPython/vessel_data/gunnerus/vessel_2.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/waves/wave_loads.py` & `MCSimPython-0.1.4/src/MCSimPython/waves/wave_loads.py`

 * *Files 2% similar despite different names*

```diff
@@ -437,16 +437,14 @@
         self._Br_lst = self.vessel_data['Br']   # List of input matrices
         self._Cr_lst = self.vessel_data['Cr']   # List of output matrices
 
         self._xr, self._Ar, self._Br, self._Cr, self.indices = self._set_ss_model()
         self.n_systems = len(self._xr)
 
         self.mu = np.zeros(6)
-
-
         
 
     @property
     def mu(self):
         return self._mu
     
     @mu.setter
@@ -479,20 +477,26 @@
         return vessel_data
 
     def _set_ss_model(self):
         dimensions = [np.asarray(ar_i).shape for ar_i in self._Ar_lst]
         xr = [np.zeros(dim[0]) for dim in dimensions if len(dim) > 1]
         indices = [i for i, dim in enumerate(dimensions) if len(dim) > 1]
         Ar = [np.asarray(self._Ar_lst[ind]) for ind in indices]
-        Br = [np.asarray(self._Br_lst[ind]) for ind in indices]
+        Br = [np.asarray(self._Br_lst[ind]).reshape(-1,) for ind in indices]
         Cr = [np.asarray(self._Cr_lst[ind]) for ind in indices]
         return xr, Ar, Br, Cr, indices
     
     
     def integrate(self, nu):
         yr = np.zeros(6)
         for i, indices in enumerate(self.indices):
             dof = indices//6
             xr_dot = self._Ar[i]@self._xr[i] + self._Br[i]*nu[indices%6]
             self._xr[i] = self._xr[i] + self.dt * xr_dot
             yr[dof] += self._Cr[i]@self._xr[i]
         self.mu = yr
+        
+    def reset(self):
+        for i in range(len(self.indices)):
+            self._xr[i] = np.zeros_like(self._xr[i])
+        self.mu = np.zeros(6)
+
```

### Comparing `MCSimPython-0.1.3/src/MCSimPython/waves/wave_spectra.py` & `MCSimPython-0.1.4/src/MCSimPython/waves/wave_spectra.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython/waves/wave_spreading.py` & `MCSimPython-0.1.4/src/MCSimPython/waves/wave_spreading.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/src/MCSimPython.egg-info/PKG-INFO` & `MCSimPython-0.1.4/src/MCSimPython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCSimPython
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python vessel simulation environment
 Author-email: Jan-Erik Hygen <janereh@stud.ntnu.no>
 Keywords: mcsim,MCSimPython,DP,dynamic positioning,Marine Cybernetics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `MCSimPython-0.1.3/src/MCSimPython.egg-info/SOURCES.txt` & `MCSimPython-0.1.4/src/MCSimPython.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,18 @@
 src/MCSimPython/vessel_data/CSAD/thruster_data.py
 src/MCSimPython/vessel_data/CSAD/vesselABC_json.json
 src/MCSimPython/vessel_data/CSAD/vessel_json.json
 src/MCSimPython/vessel_data/gunnerus/__init__.py
 src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json
 src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl
 src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl
+src/MCSimPython/vessel_data/gunnerus/rvg2_config.json
+src/MCSimPython/vessel_data/gunnerus/rvg3ABC_config.json
+src/MCSimPython/vessel_data/gunnerus/rvg3ABC_config_.json
+src/MCSimPython/vessel_data/gunnerus/rvg3_config.json
 src/MCSimPython/vessel_data/gunnerus/rvg_config.json
 src/MCSimPython/vessel_data/gunnerus/vessel.json
 src/MCSimPython/vessel_data/gunnerus/vessel_2.json
 src/MCSimPython/waves/__init__.py
 src/MCSimPython/waves/wave_loads.py
 src/MCSimPython/waves/wave_spectra.py
 src/MCSimPython/waves/wave_spreading.py
```

### Comparing `MCSimPython-0.1.3/tests/test_utils.py` & `MCSimPython-0.1.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.3/tests/test_wave_spectra.py` & `MCSimPython-0.1.4/tests/test_wave_spectra.py`

 * *Files identical despite different names*

