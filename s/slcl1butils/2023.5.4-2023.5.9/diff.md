# Comparing `tmp/slcl1butils-2023.5.4.tar.gz` & `tmp/slcl1butils-2023.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slcl1butils-2023.5.4.tar", last modified: Thu May  4 13:31:30 2023, max compression
+gzip compressed data, was "slcl1butils-2023.5.9.tar", last modified: Tue May  9 10:09:37 2023, max compression
```

## Comparing `slcl1butils-2023.5.4.tar` & `slcl1butils-2023.5.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.511541 slcl1butils-2023.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.507541 slcl1butils-2023.5.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.507541 slcl1butils-2023.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-04 13:31:30.511541 slcl1butils-2023.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.503541 slcl1butils-2023.5.4/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.507541 slcl1butils-2023.5.4/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.507541 slcl1butils-2023.5.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.503541 slcl1butils-2023.5.4/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.507541 slcl1butils-2023.5.4/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/_static/css/slcl1butils.css
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/basic_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.507541 slcl1butils-2023.5.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/examples/display_a_IW_L1B_xspectra.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/examples/intro.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/oceanspectrumSAR.png
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/get_polygons_from_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:31:30.511541 slcl1butils-2023.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.507541 slcl1butils-2023.5.4/slcl1butils/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.511541 slcl1butils-2023.5.4/slcl1butils/coloc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/coloc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/coloc/coloc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.511541 slcl1butils-2023.5.4/slcl1butils/compute/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/compute/compute_from_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/compute/cwave.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/compute/macs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/compute/stack_iw_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/compute/stack_wv_l1c_monthly.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/conversion_polar_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/cwave_parameters_computation_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/get_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/get_polygons_from_l1b.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.511541 slcl1butils-2023.5.4/slcl1butils/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
--rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/plotting/display_one_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/plotting/display_xspectra_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/raster_readers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.511541 slcl1butils-2023.5.4/slcl1butils/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs
--rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/spectrum_clockwise_to_trigo.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/spectrum_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/symmetrize_l1b_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.511541 slcl1butils-2023.5.4/slcl1butils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-04 13:31:30.000000 slcl1butils-2023.5.4/slcl1butils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-04 13:31:30.000000 slcl1butils-2023.5.4/slcl1butils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:31:30.000000 slcl1butils-2023.5.4/slcl1butils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-04 13:31:30.000000 slcl1butils-2023.5.4/slcl1butils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 13:31:30.000000 slcl1butils-2023.5.4/slcl1butils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 13:31:30.000000 slcl1butils-2023.5.4/slcl1butils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.044831 slcl1butils-2023.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.032831 slcl1butils-2023.5.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.032831 slcl1butils-2023.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-09 10:09:37.044831 slcl1butils-2023.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.028831 slcl1butils-2023.5.9/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.032831 slcl1butils-2023.5.9/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.036831 slcl1butils-2023.5.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.028831 slcl1butils-2023.5.9/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.036831 slcl1butils-2023.5.9/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/_static/css/slcl1butils.css
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.036831 slcl1butils-2023.5.9/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/examples/display_a_IW_L1B_xspectra.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/examples/intro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/oceanspectrumSAR.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/get_polygons_from_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 10:09:37.044831 slcl1butils-2023.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.036831 slcl1butils-2023.5.9/slcl1butils/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.040831 slcl1butils-2023.5.9/slcl1butils/coloc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/coloc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/coloc/coloc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.040831 slcl1butils-2023.5.9/slcl1butils/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/compute/compute_from_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/compute/cwave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/compute/macs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/compute/stack_iw_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/compute/stack_wv_l1c_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/conversion_polar_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/cwave_parameters_computation_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/get_polygons_from_l1b.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.040831 slcl1butils-2023.5.9/slcl1butils/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/plotting/display_one_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/plotting/display_xspectra_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/raster_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.044831 slcl1butils-2023.5.9/slcl1butils/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/spectrum_clockwise_to_trigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/spectrum_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/symmetrize_l1b_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.040831 slcl1butils-2023.5.9/slcl1butils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-09 10:09:37.000000 slcl1butils-2023.5.9/slcl1butils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-09 10:09:37.000000 slcl1butils-2023.5.9/slcl1butils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:09:37.000000 slcl1butils-2023.5.9/slcl1butils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-09 10:09:37.000000 slcl1butils-2023.5.9/slcl1butils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-09 10:09:37.000000 slcl1butils-2023.5.9/slcl1butils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 10:09:37.000000 slcl1butils-2023.5.9/slcl1butils.egg-info/top_level.txt
```

### Comparing `slcl1butils-2023.5.4/.github/workflows/publish.yml` & `slcl1butils-2023.5.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/.gitignore` & `slcl1butils-2023.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/.pre-commit-config.yaml` & `slcl1butils-2023.5.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/LICENSE` & `slcl1butils-2023.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/PKG-INFO` & `slcl1butils-2023.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slcl1butils
-Version: 2023.5.4
+Version: 2023.5.9
 Summary: Python library to exploit SAR IFREMER L1B products
 Author: Alexis Mouche
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `slcl1butils-2023.5.4/docs/Makefile` & `slcl1butils-2023.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/docs/conf.py` & `slcl1butils-2023.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/docs/examples/display_a_IW_L1B_xspectra.ipynb` & `slcl1butils-2023.5.9/docs/examples/display_a_IW_L1B_xspectra.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb` & `slcl1butils-2023.5.9/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb` & `slcl1butils-2023.5.9/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb` & `slcl1butils-2023.5.9/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/docs/index.rst` & `slcl1butils-2023.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/docs/installing.rst` & `slcl1butils-2023.5.9/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/docs/oceanspectrumSAR.png` & `slcl1butils-2023.5.9/docs/oceanspectrumSAR.png`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/get_polygons_from_l1b.py` & `slcl1butils-2023.5.9/get_polygons_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/pyproject.toml` & `slcl1butils-2023.5.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 dependencies = [
     "xarray",
     "numpy",
     "netCDF4",
     "shapely",
     "xarray-datatree",
     "importlib_resources",
-    'tqdm'
+    'tqdm',
+    "zarr"
 ]
 dynamic = ["version"]
 
 [build-system]
 requires = ["setuptools>=64.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
```

### Comparing `slcl1butils-2023.5.4/slcl1butils/coloc/coloc.py` & `slcl1butils-2023.5.9/slcl1butils/coloc/coloc.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/compute/cwave.py` & `slcl1butils-2023.5.9/slcl1butils/compute/cwave.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/compute/macs.py` & `slcl1butils-2023.5.9/slcl1butils/compute/macs.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/compute/stack_iw_l1b.py` & `slcl1butils-2023.5.9/slcl1butils/compute/stack_iw_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/compute/stack_wv_l1c_monthly.py` & `slcl1butils-2023.5.9/slcl1butils/compute/stack_wv_l1c_monthly.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/conversion_polar_cartesian.py` & `slcl1butils-2023.5.9/slcl1butils/conversion_polar_cartesian.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/cwave_parameters_computation_example.ipynb` & `slcl1butils-2023.5.9/slcl1butils/cwave_parameters_computation_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/get_config.py` & `slcl1butils-2023.5.9/slcl1butils/get_config.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/get_polygons_from_l1b.py` & `slcl1butils-2023.5.9/slcl1butils/get_polygons_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py` & `slcl1butils-2023.5.9/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/plotting/display_one_spectra.py` & `slcl1butils-2023.5.9/slcl1butils/plotting/display_one_spectra.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/plotting/display_xspectra_grid.py` & `slcl1butils-2023.5.9/slcl1butils/plotting/display_xspectra_grid.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb` & `slcl1butils-2023.5.9/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb` & `slcl1butils-2023.5.9/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py` & `slcl1butils-2023.5.9/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/raster_readers.py` & `slcl1butils-2023.5.9/slcl1butils/raster_readers.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs` & `slcl1butils-2023.5.9/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py` & `slcl1butils-2023.5.9/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import sys, os
 from slcl1butils.get_polygons_from_l1b import get_swath_tiles_polygons_from_l1bgroup
 from slcl1butils.coloc.coloc import raster_cropping_in_polygon_bounding_box, coloc_tiles_from_l1bgroup_with_raster
 from slcl1butils.compute.compute_from_l1b import compute_xs_from_l1b
 from slcl1butils.compute.cwave import compute_cwave_parameters
 from slcl1butils.compute.macs import compute_macs
 from slcl1butils.get_config import get_conf
+from collections import defaultdict
 from tqdm import tqdm
 import warnings
 warnings.simplefilter(action='ignore')
 conf = get_conf()
 
 def do_L1C_SAFE_from_L1B_SAFE(full_safe_file,version, outputdir, cwave=True, macs=True, colocat=True,
                               time_separation='2tau', overwrite=False,dev=False):
@@ -69,26 +70,34 @@
     if len(files) == 0:
         return None
 
     # Loop on L1B netCDF files (per slice)
     if dev:
         logging.info('dev mode -> only one L1B file to treat')
         files = files[0:1]
+    cpt = defaultdict(int)
     pbar = tqdm(range(len(files)))
     for ii in pbar:
+        cpt['L1B_traeted'] += 1
         pbar.set_description('')
         l1b_fullpath = files[ii]
         l1c_full_path = get_l1c_filepath(l1b_fullpath,version=version, outputdir=outputdir)
         if os.path.exists(l1c_full_path) and overwrite is False:
             logging.info('%s already exists', l1c_full_path)
         else:
             ds_intra, ds_inter = enrich_onesubswath_l1b(l1b_fullpath, ancillary_list=None, cwave=cwave, macs=macs,
                                                         colocat=colocat,
                                                         time_separation=time_separation)
-            save_l1c_to_netcdf(l1c_full_path, ds_intra, ds_inter,version=version)
+            if 'xspectra' in ds_inter:
+                save_l1c_to_netcdf(l1c_full_path, ds_intra, ds_inter,version=version)
+                cpt['saved_in_nc'] += 1
+            else:
+                logging.info('there is no xspectra in this subswath -> the L1C will not be saved')
+                cpt['L1B_without_spectra'] += 1
+    logging.info('cpt: %s',cpt)
     return 0
 
 
 def enrich_onesubswath_l1b(l1b_fullpath, ancillary_list=None, cwave=True, macs=True, colocat=True,
                            time_separation='2tau'):
 
     logging.info('File in: %s', l1b_fullpath)
@@ -106,15 +115,15 @@
     burst_type = 'inter'
     time_separation = 'None'
     xs_inter, ds_inter = compute_xs_from_l1b(l1b_fullpath, burst_type=burst_type, time_separation=time_separation)
 
     # ====================
     # CWAVE
     # ====================
-    if cwave:
+    if cwave and xs_intra is not None and xs_inter is not None:
         #
         # CWAVE Processing Parameters
         kmax = 2 * np.pi / 25
         kmin = 2 * np.pi / 600
         Nk = 4
         Nphi = 5
         # Intraburst at 2tau CWAVE parameters
@@ -126,15 +135,15 @@
         # updating the L1B dataset
         ds_intra = xr.merge([ds_intra, ds_cwave_parameters_intra])
         ds_inter = xr.merge([ds_inter, ds_cwave_parameters_inter])
 
     # ====================
     # MACS
     # ====================
-    if macs:
+    if macs and xs_intra is not None and xs_inter is not None:
         # MACS parameters
         lambda_range_max = [50, 75, 100, 125, 150, 175, 200, 225, 250, 275]
         # Intraburst at 2tau MACS
         ds_macs_intra = compute_macs(xs_intra, lambda_range_max=lambda_range_max)
         # Interburst MACS
         ds_macs_inter = compute_macs(xs_inter, lambda_range_max=lambda_range_max)
         # updating the L1B dataset
```

### Comparing `slcl1butils-2023.5.4/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py` & `slcl1butils-2023.5.9/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs` & `slcl1butils-2023.5.9/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py` & `slcl1butils-2023.5.9/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/spectrum_clockwise_to_trigo.py` & `slcl1butils-2023.5.9/slcl1butils/spectrum_clockwise_to_trigo.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/spectrum_rotation.py` & `slcl1butils-2023.5.9/slcl1butils/spectrum_rotation.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/symmetrize_l1b_spectra.py` & `slcl1butils-2023.5.9/slcl1butils/symmetrize_l1b_spectra.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils/utils.py` & `slcl1butils-2023.5.9/slcl1butils/utils.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.4/slcl1butils.egg-info/PKG-INFO` & `slcl1butils-2023.5.9/slcl1butils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slcl1butils
-Version: 2023.5.4
+Version: 2023.5.9
 Summary: Python library to exploit SAR IFREMER L1B products
 Author: Alexis Mouche
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `slcl1butils-2023.5.4/slcl1butils.egg-info/SOURCES.txt` & `slcl1butils-2023.5.9/slcl1butils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

