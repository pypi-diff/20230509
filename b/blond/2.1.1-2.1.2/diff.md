# Comparing `tmp/blond-2.1.1.tar.gz` & `tmp/blond-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blond-2.1.1.tar", last modified: Thu May  4 09:50:52 2023, max compression
+gzip compressed data, was "blond-2.1.2.tar", last modified: Tue May  9 15:49:52 2023, max compression
```

## Comparing `blond-2.1.1.tar` & `blond-2.1.2.tar`

### file list

```diff
@@ -1,312 +1,313 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.628000 blond-2.1.1/
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-04 09:50:22.000000 blond-2.1.1/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     6226 2023-05-04 09:50:22.000000 blond-2.1.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2869 2023-05-04 09:50:22.000000 blond-2.1.1/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1665 2023-05-04 09:50:22.000000 blond-2.1.1/CHANGELOG
--rw-r--r--   0 root         (0) root         (0)    35797 2023-05-04 09:50:22.000000 blond-2.1.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      339 2023-05-04 09:50:22.000000 blond-2.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13244 2023-05-04 09:50:52.628000 blond-2.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12468 2023-05-04 09:50:22.000000 blond-2.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)      794 2023-05-04 09:50:22.000000 blond-2.1.1/WARNINGS.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.592000 blond-2.1.1/__BENCHMARKS/
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-04 09:50:22.000000 blond-2.1.1/__BENCHMARKS/.gitignore
--rw-r--r--   0 root         (0) root         (0)    16964 2023-05-04 09:50:22.000000 blond-2.1.1/__BENCHMARKS/BM1_OTFB_Vind_beam_1.py
--rw-r--r--   0 root         (0) root         (0)     4291 2023-05-04 09:50:22.000000 blond-2.1.1/__BENCHMARKS/BM2_OTFB_no_beam.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-05-04 09:50:22.000000 blond-2.1.1/__BENCHMARKS/BM3_OTFB_moving_average.py
--rw-r--r--   0 root         (0) root         (0)     7415 2023-05-04 09:50:22.000000 blond-2.1.1/__BENCHMARKS/BM4_OTFB_with_beam.py
--rw-r--r--   0 root         (0) root         (0)     8956 2023-05-04 09:50:22.000000 blond-2.1.1/__BENCHMARKS/BM5_OTFB_feedforward.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.584000 blond-2.1.1/__EXAMPLES/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.592000 blond-2.1.1/__EXAMPLES/gpu_main_files/
--rw-r--r--   0 root         (0) root         (0)     5807 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_01_Acceleration.py
--rw-r--r--   0 root         (0) root         (0)     8578 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_02_Main_long_ps_booster.py
--rw-r--r--   0 root         (0) root         (0)     6581 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_03_RFnoise.py
--rw-r--r--   0 root         (0) root         (0)     7056 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_04_Stationary_multistation.py
--rw-r--r--   0 root         (0) root         (0)    14174 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_05_Wake_impedance.py
--rw-r--r--   0 root         (0) root         (0)     7328 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_07_Ions.py
--rw-r--r--   0 root         (0) root         (0)     5041 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_08_Phase_Loop.py
--rw-r--r--   0 root         (0) root         (0)     5582 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_09_Radial_Loop.py
--rw-r--r--   0 root         (0) root         (0)     5941 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_10_Fixed_frequency.py
--rw-r--r--   0 root         (0) root         (0)     5953 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_16_impedance_test.py
--rw-r--r--   0 root         (0) root         (0)     9212 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_17_multi_turn_wake.py
--rw-r--r--   0 root         (0) root         (0)     8115 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/gpu_main_files/EX_18_robinson_instability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.592000 blond-2.1.1/__EXAMPLES/input_files/
--rw-r--r--   0 root         (0) root         (0)    11866 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/input_files/EX_02_Ekicker_1.4GeV.txt
--rw-r--r--   0 root         (0) root         (0)    16868 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/input_files/EX_02_Finemet.txt
--rw-r--r--   0 root         (0) root         (0)     1043 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/input_files/EX_05_new_HQ_table.dat
--rw-r--r--   0 root         (0) root         (0)    11976 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/input_files/EX_06_Source_TOF_P.csv
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c02.txt
--rw-r--r--   0 root         (0) root         (0)      316 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c04.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c16.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.596000 blond-2.1.1/__EXAMPLES/main_files/
--rw-r--r--   0 root         (0) root         (0)     4668 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_01_Acceleration.py
--rw-r--r--   0 root         (0) root         (0)     7353 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_02_Main_long_ps_booster.py
--rw-r--r--   0 root         (0) root         (0)     5605 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_03_RFnoise.py
--rw-r--r--   0 root         (0) root         (0)     5413 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_04_Stationary_multistation.py
--rw-r--r--   0 root         (0) root         (0)    11556 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_05_Wake_impedance.py
--rw-r--r--   0 root         (0) root         (0)     3396 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_06_Preprocess.py
--rw-r--r--   0 root         (0) root         (0)     6400 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_07_Ions.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_08_Phase_Loop.py
--rw-r--r--   0 root         (0) root         (0)     4864 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_09_Radial_Loop.py
--rw-r--r--   0 root         (0) root         (0)     4938 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_10_Fixed_frequency.py
--rw-r--r--   0 root         (0) root         (0)     4651 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_11_comparison_music_fourier_analytical.py
--rw-r--r--   0 root         (0) root         (0)    11630 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_12_synchrotron_frequency_distribution.py
--rw-r--r--   0 root         (0) root         (0)    10276 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_13_synchrotron_radiation.py
--rw-r--r--   0 root         (0) root         (0)     4639 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_14_sparse_slicing.py
--rw-r--r--   0 root         (0) root         (0)     4665 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_15_sparse_multi_bunch.py
--rw-r--r--   0 root         (0) root         (0)     5447 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_16_impedance_test.py
--rw-r--r--   0 root         (0) root         (0)     7736 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_17_multi_turn_wake.py
--rw-r--r--   0 root         (0) root         (0)     7438 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_18_robinson_instability.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_19_bunch_generation.py
--rw-r--r--   0 root         (0) root         (0)     6646 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_20_bunch_generation_multibunch.py
--rw-r--r--   0 root         (0) root         (0)     3132 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_21_bunch_distribution.py
--rwxr-xr-x   0 root         (0) root         (0)     4029 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/main_files/EX_22_Coherent_Radiation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.596000 blond-2.1.1/__EXAMPLES/mpi_main_files/
--rw-r--r--   0 root         (0) root         (0)     5008 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_01_Acceleration.py
--rw-r--r--   0 root         (0) root         (0)     7618 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_02_Main_long_ps_booster.py
--rw-r--r--   0 root         (0) root         (0)     5932 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_03_RFnoise.py
--rw-r--r--   0 root         (0) root         (0)     5703 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_04_Stationary_multistation.py
--rw-r--r--   0 root         (0) root         (0)    12098 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_05_Wake_impedance.py
--rw-r--r--   0 root         (0) root         (0)     6688 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_07_Ions.py
--rw-r--r--   0 root         (0) root         (0)     4632 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_08_Phase_Loop.py
--rw-r--r--   0 root         (0) root         (0)     5181 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_09_Radial_Loop.py
--rw-r--r--   0 root         (0) root         (0)     5255 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_10_Fixed_frequency.py
--rw-r--r--   0 root         (0) root         (0)     5659 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_16_impedance_test.py
--rw-r--r--   0 root         (0) root         (0)     7914 2023-05-04 09:50:22.000000 blond-2.1.1/__EXAMPLES/mpi_main_files/EX_18_robinson_instability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.596000 blond-2.1.1/__doc/
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/Makefile
--rw-r--r--   0 root         (0) root         (0)     5664 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/conf.py
--rw-r--r--   0 root         (0) root         (0)     1162 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/index.rst
--rw-r--r--   0 root         (0) root         (0)      809 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.600000 blond-2.1.1/__doc/modules/
--rwxr-xr-x   0 root         (0) root         (0)   135010 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/ACS_cavity_loop.png
--rwxr-xr-x   0 root         (0) root         (0)   185223 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/ACS_cavity_loop.svg
--rwxr-xr-x   0 root         (0) root         (0)     1144 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/RF_noise.gle
--rwxr-xr-x   0 root         (0) root         (0)    81234 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/RF_noise.png
--rwxr-xr-x   0 root         (0) root         (0)   176302 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/SPS_OTFB.png
--rwxr-xr-x   0 root         (0) root         (0)   655573 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/SPS_OTFB.svg
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/beam.rst
--rw-r--r--   0 root         (0) root         (0)      177 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/compile.rst
--rw-r--r--   0 root         (0) root         (0)    51317 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/csr_impedance_real.png
--rw-r--r--   0 root         (0) root         (0)    19684 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/equations_of_motion.rst
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/impedances.rst
--rw-r--r--   0 root         (0) root         (0)      754 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/input_parameters.rst
--rwxr-xr-x   0 root         (0) root         (0)     7100 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/lhc_cavity_loop.rst
--rw-r--r--   0 root         (0) root         (0)    20259 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/llrf.rst
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/monitors.rst
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/plots.rst
--rwxr-xr-x   0 root         (0) root         (0)     1050 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/ring_and_RFstation.gle
--rwxr-xr-x   0 root         (0) root         (0)    84423 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/ring_and_RFstation.png
--rwxr-xr-x   0 root         (0) root         (0)       39 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/sample.dat
--rwxr-xr-x   0 root         (0) root         (0)       77 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/sample2.dat
--rwxr-xr-x   0 root         (0) root         (0)    14087 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/sps_cavity_loop.rst
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/synchrotron_radiation.rst
--rw-r--r--   0 root         (0) root         (0)     1166 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/toolbox.rst
--rw-r--r--   0 root         (0) root         (0)      344 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/trackers.rst
--rw-r--r--   0 root         (0) root         (0)      484 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/modules/utils.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.584000 blond-2.1.1/__doc/themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.604000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/
--rw-r--r--   0 root         (0) root         (0)      324 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/breadcrumbs.html
--rw-r--r--   0 root         (0) root         (0)     1978 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/footer.html
--rw-r--r--   0 root         (0) root         (0)     7063 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/layout.html
--rw-r--r--   0 root         (0) root         (0)     7526 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/layout_old.html
--rw-r--r--   0 root         (0) root         (0)     1530 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/search.html
--rw-r--r--   0 root         (0) root         (0)      365 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/searchbox.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.588000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.604000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/
--rw-r--r--   0 root         (0) root         (0)     3381 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css
--rw-r--r--   0 root         (0) root         (0)     3153 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css.map
--rw-r--r--   0 root         (0) root         (0)   114281 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/theme.css
--rw-r--r--   0 root         (0) root         (0)    67610 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/theme.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.608000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/
--rw-r--r--   0 root         (0) root         (0)   124988 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/FontAwesome.otf
--rw-r--r--   0 root         (0) root         (0)   109948 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Bold.ttf
--rw-r--r--   0 root         (0) root         (0)    96964 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Regular.ttf
--rw-r--r--   0 root         (0) root         (0)   656544 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Bold.ttf
--rw-r--r--   0 root         (0) root         (0)   656568 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Regular.ttf
--rw-r--r--   0 root         (0) root         (0)   170616 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Bold.ttf
--rw-r--r--   0 root         (0) root         (0)   169064 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Regular.ttf
--rw-r--r--   0 root         (0) root         (0)    76518 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)   391622 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)   152796 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    90412 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 root         (0) root         (0)    71896 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.608000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/js/
--rw-r--r--   0 root         (0) root         (0)     2457 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js~
--rw-r--r--   0 root         (0) root         (0)    15414 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/js/modernizr.min.js
--rw-r--r--   0 root         (0) root         (0)     6477 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/js/theme.js
--rw-r--r--   0 root         (0) root         (0)      260 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/theme.conf
--rw-r--r--   0 root         (0) root         (0)     1299 2023-05-04 09:50:22.000000 blond-2.1.1/__doc/themes/sphinx_rtd_theme/versions.html
--rw-r--r--   0 root         (0) root         (0)     1380 2023-05-04 09:50:22.000000 blond-2.1.1/appveyor.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.608000 blond-2.1.1/blond/
--rw-r--r--   0 root         (0) root         (0)     1199 2023-05-04 09:50:22.000000 blond-2.1.1/blond/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-04 09:50:48.000000 blond-2.1.1/blond/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.612000 blond-2.1.1/blond/beam/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/beam/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20461 2023-05-04 09:50:22.000000 blond-2.1.1/blond/beam/beam.py
--rw-r--r--   0 root         (0) root         (0)     3685 2023-05-04 09:50:22.000000 blond-2.1.1/blond/beam/coasting_beam.py
--rw-r--r--   0 root         (0) root         (0)    41527 2023-05-04 09:50:22.000000 blond-2.1.1/blond/beam/distributions.py
--rw-r--r--   0 root         (0) root         (0)    39107 2023-05-04 09:50:22.000000 blond-2.1.1/blond/beam/distributions_multibunch.py
--rw-r--r--   0 root         (0) root         (0)    24385 2023-05-04 09:50:22.000000 blond-2.1.1/blond/beam/profile.py
--rw-r--r--   0 root         (0) root         (0)     5740 2023-05-04 09:50:22.000000 blond-2.1.1/blond/beam/sparse_histogram.cpp
--rw-r--r--   0 root         (0) root         (0)     4804 2023-05-04 09:50:22.000000 blond-2.1.1/blond/beam/sparse_slices.py
--rw-r--r--   0 root         (0) root         (0)    11654 2023-05-04 09:50:22.000000 blond-2.1.1/blond/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.612000 blond-2.1.1/blond/cpp_routines/
--rw-r--r--   0 root         (0) root         (0)     3088 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/beam_phase.cpp
--rw-r--r--   0 root         (0) root         (0)    29022 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/blondmath.cpp
--rw-r--r--   0 root         (0) root         (0)    13334 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/blondmath.h
--rw-r--r--   0 root         (0) root         (0)     1316 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/cos.h
--rw-r--r--   0 root         (0) root         (0)     5747 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/drift.cpp
--rw-r--r--   0 root         (0) root         (0)     4376 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/exp.h
--rw-r--r--   0 root         (0) root         (0)     4661 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/fast_resonator.cpp
--rw-r--r--   0 root         (0) root         (0)    29481 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/fft.cpp
--rw-r--r--   0 root         (0) root         (0)     4419 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/fft.h
--rw-r--r--   0 root         (0) root         (0)    10013 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/histogram.cpp
--rw-r--r--   0 root         (0) root         (0)     3493 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/kick.cpp
--rwxr-xr-x   0 root         (0) root         (0)   126096 2023-05-04 09:50:52.000000 blond-2.1.1/blond/cpp_routines/libblond.so
--rw-r--r--   0 root         (0) root         (0)     6406 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/linear_interp_kick.cpp
--rw-r--r--   0 root         (0) root         (0)    15181 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/music_track.cpp
--rw-r--r--   0 root         (0) root         (0)      169 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/openmp.cpp
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/openmp.h
--rw-r--r--   0 root         (0) root         (0)     1960 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/sin.h
--rw-r--r--   0 root         (0) root         (0)     5871 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/sincos.h
--rw-r--r--   0 root         (0) root         (0)     7480 2023-05-04 09:50:22.000000 blond-2.1.1/blond/cpp_routines/vdtcore_common.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.612000 blond-2.1.1/blond/gpu/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/gpu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.612000 blond-2.1.1/blond/gpu/cuda_kernels/
--rw-r--r--   0 root         (0) root         (0)    14390 2023-05-04 09:50:22.000000 blond-2.1.1/blond/gpu/cuda_kernels/kernels_double.cu
--rw-r--r--   0 root         (0) root         (0)    14135 2023-05-04 09:50:22.000000 blond-2.1.1/blond/gpu/cuda_kernels/kernels_single.cu
--rw-r--r--   0 root         (0) root         (0)    10769 2023-05-04 09:50:22.000000 blond-2.1.1/blond/gpu/cupy_butils_wrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.616000 blond-2.1.1/blond/impedances/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/impedances/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39560 2023-05-04 09:50:22.000000 blond-2.1.1/blond/impedances/impedance.py
--rw-r--r--   0 root         (0) root         (0)    45892 2023-05-04 09:50:22.000000 blond-2.1.1/blond/impedances/impedance_sources.py
--rw-r--r--   0 root         (0) root         (0)     3541 2023-05-04 09:50:22.000000 blond-2.1.1/blond/impedances/induced_voltage_analytical.py
--rw-r--r--   0 root         (0) root         (0)    12228 2023-05-04 09:50:22.000000 blond-2.1.1/blond/impedances/music.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.616000 blond-2.1.1/blond/input_parameters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/input_parameters/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24903 2023-05-04 09:50:22.000000 blond-2.1.1/blond/input_parameters/rf_parameters.py
--rw-r--r--   0 root         (0) root         (0)    20249 2023-05-04 09:50:22.000000 blond-2.1.1/blond/input_parameters/rf_parameters_options.py
--rw-r--r--   0 root         (0) root         (0)    17272 2023-05-04 09:50:22.000000 blond-2.1.1/blond/input_parameters/ring.py
--rw-r--r--   0 root         (0) root         (0)    22443 2023-05-04 09:50:22.000000 blond-2.1.1/blond/input_parameters/ring_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.616000 blond-2.1.1/blond/llrf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22090 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/beam_feedback.py
--rw-r--r--   0 root         (0) root         (0)    36313 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/cavity_feedback.py
--rw-r--r--   0 root         (0) root         (0)    14383 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/impulse_response.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/notch_filter.py
--rw-r--r--   0 root         (0) root         (0)     7257 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/offset_frequency.py
--rw-r--r--   0 root         (0) root         (0)     4394 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/rf_modulation.py
--rw-r--r--   0 root         (0) root         (0)    15759 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/rf_noise.py
--rw-r--r--   0 root         (0) root         (0)    18814 2023-05-04 09:50:22.000000 blond-2.1.1/blond/llrf/signal_processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.616000 blond-2.1.1/blond/monitors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/monitors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20936 2023-05-04 09:50:22.000000 blond-2.1.1/blond/monitors/monitors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.616000 blond-2.1.1/blond/plots/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/plots/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11025 2023-05-04 09:50:22.000000 blond-2.1.1/blond/plots/plot.py
--rw-r--r--   0 root         (0) root         (0)    10004 2023-05-04 09:50:22.000000 blond-2.1.1/blond/plots/plot_beams.py
--rw-r--r--   0 root         (0) root         (0)     4777 2023-05-04 09:50:22.000000 blond-2.1.1/blond/plots/plot_impedance.py
--rw-r--r--   0 root         (0) root         (0)    14165 2023-05-04 09:50:22.000000 blond-2.1.1/blond/plots/plot_llrf.py
--rw-r--r--   0 root         (0) root         (0)     1210 2023-05-04 09:50:22.000000 blond-2.1.1/blond/plots/plot_parameters.py
--rw-r--r--   0 root         (0) root         (0)     2725 2023-05-04 09:50:22.000000 blond-2.1.1/blond/plots/plot_slices.py
--rw-r--r--   0 root         (0) root         (0)     6671 2023-05-04 09:50:22.000000 blond-2.1.1/blond/sanity_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.616000 blond-2.1.1/blond/synchrotron_radiation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/synchrotron_radiation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5364 2023-05-04 09:50:22.000000 blond-2.1.1/blond/synchrotron_radiation/synchrotron_radiation.cpp
--rw-r--r--   0 root         (0) root         (0)     8111 2023-05-04 09:50:22.000000 blond-2.1.1/blond/synchrotron_radiation/synchrotron_radiation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.620000 blond-2.1.1/blond/toolbox/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5221 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/action.py
--rw-r--r--   0 root         (0) root         (0)     7570 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/diffusion.py
--rw-r--r--   0 root         (0) root         (0)     7484 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/filters_and_fitting.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/logger.py
--rw-r--r--   0 root         (0) root         (0)     3377 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/next_regular.py
--rw-r--r--   0 root         (0) root         (0)    21008 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/parameter_scaling.py
--rw-r--r--   0 root         (0) root         (0)     2358 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/tomoscope.cpp
--rw-r--r--   0 root         (0) root         (0)     4877 2023-05-04 09:50:22.000000 blond-2.1.1/blond/toolbox/tomoscope.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.620000 blond-2.1.1/blond/trackers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/trackers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26351 2023-05-04 09:50:22.000000 blond-2.1.1/blond/trackers/tracker.py
--rw-r--r--   0 root         (0) root         (0)    31233 2023-05-04 09:50:22.000000 blond-2.1.1/blond/trackers/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.620000 blond-2.1.1/blond/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8233 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/bmath.py
--rw-r--r--   0 root         (0) root         (0)    48243 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/butils_wrap.py
--rw-r--r--   0 root         (0) root         (0)     3467 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/data_check.py
--rw-r--r--   0 root         (0) root         (0)     1965 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     4145 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/input_parser.py
--rw-r--r--   0 root         (0) root         (0)    14206 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/mpi_config.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/profile_mock.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-05-04 09:50:22.000000 blond-2.1.1/blond/utils/track_iteration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.608000 blond-2.1.1/blond.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13244 2023-05-04 09:50:52.000000 blond-2.1.1/blond.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9882 2023-05-04 09:50:52.000000 blond-2.1.1/blond.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 09:50:52.000000 blond-2.1.1/blond.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 09:50:48.000000 blond-2.1.1/blond.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      226 2023-05-04 09:50:52.000000 blond-2.1.1/blond.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-04 09:50:52.000000 blond-2.1.1/blond.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-05-04 09:50:22.000000 blond-2.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-04 09:50:22.000000 blond-2.1.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 09:50:52.628000 blond-2.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4446 2023-05-04 09:50:22.000000 blond-2.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.588000 blond-2.1.1/unittests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.620000 blond-2.1.1/unittests/beam_profile/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/beam_profile/__init__.py
--rw-r--r--   0 root         (0) root         (0)   800196 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/beam_profile/dt_coordinates.npz
--rw-r--r--   0 root         (0) root         (0)    12422 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/beam_profile/test_beam_profile_object.py
--rw-r--r--   0 root         (0) root         (0)     7221 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/beam_profile/test_sparse_profile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.620000 blond-2.1.1/unittests/beams/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/beams/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14105 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/beams/test_beam_object.py
--rw-r--r--   0 root         (0) root         (0)     5659 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/beams/test_coasting_beam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.620000 blond-2.1.1/unittests/general/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/general/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16184 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/general/test_separatrix_bigaussian.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.624000 blond-2.1.1/unittests/gpu/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/gpu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5011 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/gpu/test_ffts.py
--rw-r--r--   0 root         (0) root         (0)    16996 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/gpu/test_impedance.py
--rw-r--r--   0 root         (0) root         (0)    22133 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/gpu/test_physics_kernels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.624000 blond-2.1.1/unittests/impedances/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/impedances/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4475 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/impedances/test_impedance.py
--rwxr-xr-x   0 root         (0) root         (0)     4940 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/impedances/test_impedance_sources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.624000 blond-2.1.1/unittests/input_parameters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/input_parameters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/input_parameters/test_preprocess.py
--rw-r--r--   0 root         (0) root         (0)    10862 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/input_parameters/test_rf_params_object.py
--rw-r--r--   0 root         (0) root         (0)     7576 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/input_parameters/test_ring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.624000 blond-2.1.1/unittests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4307 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/integration/test_examples.py
--rw-r--r--   0 root         (0) root         (0)     3047 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/integration/test_gpu_examples.py
--rw-r--r--   0 root         (0) root         (0)     3043 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/integration/test_mpi_examples.py
--rw-r--r--   0 root         (0) root         (0)     4116 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/integration/test_validate_gpu.py
--rw-r--r--   0 root         (0) root         (0)     4005 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/integration/test_validate_mpi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.624000 blond-2.1.1/unittests/llrf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    74048 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/ref_DV_MOD_FR.npy
--rw-r--r--   0 root         (0) root         (0)    74048 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/ref_DV_MOD_FRF.npy
--rw-r--r--   0 root         (0) root         (0)    74048 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/ref_V_IND_COARSE_GEN.npy
--rw-r--r--   0 root         (0) root         (0)     8741 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/test_beam_feedback.py
--rw-r--r--   0 root         (0) root         (0)    31675 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/test_cavity_feedback.py
--rw-r--r--   0 root         (0) root         (0)    40554 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/test_impulse_response.py
--rw-r--r--   0 root         (0) root         (0)     3649 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/test_offset_frequency.py
--rw-r--r--   0 root         (0) root         (0)     8157 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/test_rf_modulation.py
--rw-r--r--   0 root         (0) root         (0)    31838 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/llrf/test_signal_processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.624000 blond-2.1.1/unittests/synchrotron_radiation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/synchrotron_radiation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32615 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/synchrotron_radiation/test_synch_rad.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.628000 blond-2.1.1/unittests/trackers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/trackers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17866 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/trackers/comparison_drift.py
--rw-r--r--   0 root         (0) root         (0)    19415 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/trackers/test_drift.py
--rw-r--r--   0 root         (0) root         (0)    10188 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/trackers/test_tracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:50:52.628000 blond-2.1.1/unittests/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21108 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/utils/test_blondmath.py
--rw-r--r--   0 root         (0) root         (0)     3790 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/utils/test_data_check.py
--rw-r--r--   0 root         (0) root         (0)     9952 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/utils/test_ffts.py
--rw-r--r--   0 root         (0) root         (0)     5103 2023-05-04 09:50:22.000000 blond-2.1.1/unittests/utils/test_iteration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.656000 blond-2.1.2/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-09 15:49:23.000000 blond-2.1.2/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     6235 2023-05-09 15:49:23.000000 blond-2.1.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-05-09 15:49:23.000000 blond-2.1.2/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-05-09 15:49:23.000000 blond-2.1.2/CHANGELOG
+-rw-r--r--   0 root         (0) root         (0)    35797 2023-05-09 15:49:23.000000 blond-2.1.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      339 2023-05-09 15:49:23.000000 blond-2.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    13940 2023-05-09 15:49:52.656000 blond-2.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13164 2023-05-09 15:49:23.000000 blond-2.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      794 2023-05-09 15:49:23.000000 blond-2.1.2/WARNINGS.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.616000 blond-2.1.2/__BENCHMARKS/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-09 15:49:23.000000 blond-2.1.2/__BENCHMARKS/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    16964 2023-05-09 15:49:23.000000 blond-2.1.2/__BENCHMARKS/BM1_OTFB_Vind_beam_1.py
+-rw-r--r--   0 root         (0) root         (0)     4291 2023-05-09 15:49:23.000000 blond-2.1.2/__BENCHMARKS/BM2_OTFB_no_beam.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-05-09 15:49:23.000000 blond-2.1.2/__BENCHMARKS/BM3_OTFB_moving_average.py
+-rw-r--r--   0 root         (0) root         (0)     7415 2023-05-09 15:49:23.000000 blond-2.1.2/__BENCHMARKS/BM4_OTFB_with_beam.py
+-rw-r--r--   0 root         (0) root         (0)     8956 2023-05-09 15:49:23.000000 blond-2.1.2/__BENCHMARKS/BM5_OTFB_feedforward.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.612000 blond-2.1.2/__EXAMPLES/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.620000 blond-2.1.2/__EXAMPLES/gpu_main_files/
+-rw-r--r--   0 root         (0) root         (0)     5807 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_01_Acceleration.py
+-rw-r--r--   0 root         (0) root         (0)     8578 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_02_Main_long_ps_booster.py
+-rw-r--r--   0 root         (0) root         (0)     6581 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_03_RFnoise.py
+-rw-r--r--   0 root         (0) root         (0)     7056 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_04_Stationary_multistation.py
+-rw-r--r--   0 root         (0) root         (0)    14174 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_05_Wake_impedance.py
+-rw-r--r--   0 root         (0) root         (0)     7328 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_07_Ions.py
+-rw-r--r--   0 root         (0) root         (0)     5041 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_08_Phase_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     5582 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_09_Radial_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     5941 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_10_Fixed_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     5953 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_16_impedance_test.py
+-rw-r--r--   0 root         (0) root         (0)     9212 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_17_multi_turn_wake.py
+-rw-r--r--   0 root         (0) root         (0)     8115 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_18_robinson_instability.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.620000 blond-2.1.2/__EXAMPLES/input_files/
+-rw-r--r--   0 root         (0) root         (0)    11866 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/input_files/EX_02_Ekicker_1.4GeV.txt
+-rw-r--r--   0 root         (0) root         (0)    16868 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/input_files/EX_02_Finemet.txt
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/input_files/EX_05_new_HQ_table.dat
+-rw-r--r--   0 root         (0) root         (0)    11976 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/input_files/EX_06_Source_TOF_P.csv
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c02.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c04.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c16.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.624000 blond-2.1.2/__EXAMPLES/main_files/
+-rw-r--r--   0 root         (0) root         (0)     4668 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_01_Acceleration.py
+-rw-r--r--   0 root         (0) root         (0)     7353 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_02_Main_long_ps_booster.py
+-rw-r--r--   0 root         (0) root         (0)     5605 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_03_RFnoise.py
+-rw-r--r--   0 root         (0) root         (0)     5413 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_04_Stationary_multistation.py
+-rw-r--r--   0 root         (0) root         (0)    11556 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_05_Wake_impedance.py
+-rw-r--r--   0 root         (0) root         (0)     3396 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_06_Preprocess.py
+-rw-r--r--   0 root         (0) root         (0)     6400 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_07_Ions.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_08_Phase_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_09_Radial_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     4938 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_10_Fixed_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     4651 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_11_comparison_music_fourier_analytical.py
+-rw-r--r--   0 root         (0) root         (0)    11630 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_12_synchrotron_frequency_distribution.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_13_synchrotron_radiation.py
+-rw-r--r--   0 root         (0) root         (0)     4639 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_14_sparse_slicing.py
+-rw-r--r--   0 root         (0) root         (0)     4665 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_15_sparse_multi_bunch.py
+-rw-r--r--   0 root         (0) root         (0)     5447 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_16_impedance_test.py
+-rw-r--r--   0 root         (0) root         (0)     7736 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_17_multi_turn_wake.py
+-rw-r--r--   0 root         (0) root         (0)     7438 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_18_robinson_instability.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_19_bunch_generation.py
+-rw-r--r--   0 root         (0) root         (0)     6646 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_20_bunch_generation_multibunch.py
+-rw-r--r--   0 root         (0) root         (0)     3132 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_21_bunch_distribution.py
+-rwxr-xr-x   0 root         (0) root         (0)     4029 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_22_Coherent_Radiation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.624000 blond-2.1.2/__EXAMPLES/mpi_main_files/
+-rw-r--r--   0 root         (0) root         (0)     5008 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_01_Acceleration.py
+-rw-r--r--   0 root         (0) root         (0)     7618 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_02_Main_long_ps_booster.py
+-rw-r--r--   0 root         (0) root         (0)     5932 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_03_RFnoise.py
+-rw-r--r--   0 root         (0) root         (0)     5703 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_04_Stationary_multistation.py
+-rw-r--r--   0 root         (0) root         (0)    12098 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_05_Wake_impedance.py
+-rw-r--r--   0 root         (0) root         (0)     6688 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_07_Ions.py
+-rw-r--r--   0 root         (0) root         (0)     4632 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_08_Phase_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     5181 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_09_Radial_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     5255 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_10_Fixed_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     5659 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_16_impedance_test.py
+-rw-r--r--   0 root         (0) root         (0)     7914 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_18_robinson_instability.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.624000 blond-2.1.2/__doc/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/Makefile
+-rw-r--r--   0 root         (0) root         (0)     5797 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/conf.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)      809 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.628000 blond-2.1.2/__doc/modules/
+-rwxr-xr-x   0 root         (0) root         (0)   135010 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/ACS_cavity_loop.png
+-rwxr-xr-x   0 root         (0) root         (0)   185223 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/ACS_cavity_loop.svg
+-rwxr-xr-x   0 root         (0) root         (0)     1144 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/RF_noise.gle
+-rwxr-xr-x   0 root         (0) root         (0)    81234 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/RF_noise.png
+-rwxr-xr-x   0 root         (0) root         (0)   176302 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/SPS_OTFB.png
+-rwxr-xr-x   0 root         (0) root         (0)   655573 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/SPS_OTFB.svg
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/beam.rst
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/compile.rst
+-rw-r--r--   0 root         (0) root         (0)    51317 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/csr_impedance_real.png
+-rw-r--r--   0 root         (0) root         (0)    19684 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/equations_of_motion.rst
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/impedances.rst
+-rw-r--r--   0 root         (0) root         (0)      754 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/input_parameters.rst
+-rwxr-xr-x   0 root         (0) root         (0)     7100 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/lhc_cavity_loop.rst
+-rw-r--r--   0 root         (0) root         (0)    20259 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/llrf.rst
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/monitors.rst
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/plots.rst
+-rwxr-xr-x   0 root         (0) root         (0)     1050 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/ring_and_RFstation.gle
+-rwxr-xr-x   0 root         (0) root         (0)    84423 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/ring_and_RFstation.png
+-rwxr-xr-x   0 root         (0) root         (0)       39 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/sample.dat
+-rwxr-xr-x   0 root         (0) root         (0)       77 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/sample2.dat
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/sanity_check.rst
+-rwxr-xr-x   0 root         (0) root         (0)    14087 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/sps_cavity_loop.rst
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/synchrotron_radiation.rst
+-rw-r--r--   0 root         (0) root         (0)     1166 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/toolbox.rst
+-rw-r--r--   0 root         (0) root         (0)      344 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/trackers.rst
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/utils.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.612000 blond-2.1.2/__doc/themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.632000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/breadcrumbs.html
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/footer.html
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/layout.html
+-rw-r--r--   0 root         (0) root         (0)     7526 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/layout_old.html
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/search.html
+-rw-r--r--   0 root         (0) root         (0)      365 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/searchbox.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.612000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.632000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css
+-rw-r--r--   0 root         (0) root         (0)     3153 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css.map
+-rw-r--r--   0 root         (0) root         (0)   114281 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/theme.css
+-rw-r--r--   0 root         (0) root         (0)    67610 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/theme.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.636000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/
+-rw-r--r--   0 root         (0) root         (0)   124988 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/FontAwesome.otf
+-rw-r--r--   0 root         (0) root         (0)   109948 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Bold.ttf
+-rw-r--r--   0 root         (0) root         (0)    96964 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Regular.ttf
+-rw-r--r--   0 root         (0) root         (0)   656544 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Bold.ttf
+-rw-r--r--   0 root         (0) root         (0)   656568 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Regular.ttf
+-rw-r--r--   0 root         (0) root         (0)   170616 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Bold.ttf
+-rw-r--r--   0 root         (0) root         (0)   169064 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Regular.ttf
+-rw-r--r--   0 root         (0) root         (0)    76518 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 root         (0) root         (0)   391622 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 root         (0) root         (0)   152796 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    90412 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 root         (0) root         (0)    71896 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.636000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/js/
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js~
+-rw-r--r--   0 root         (0) root         (0)    15414 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/js/modernizr.min.js
+-rw-r--r--   0 root         (0) root         (0)     6477 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/js/theme.js
+-rw-r--r--   0 root         (0) root         (0)      260 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/theme.conf
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/versions.html
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-05-09 15:49:23.000000 blond-2.1.2/appveyor.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.636000 blond-2.1.2/blond/
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-05-09 15:49:23.000000 blond-2.1.2/blond/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-09 15:49:48.000000 blond-2.1.2/blond/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.640000 blond-2.1.2/blond/beam/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/beam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20374 2023-05-09 15:49:23.000000 blond-2.1.2/blond/beam/beam.py
+-rw-r--r--   0 root         (0) root         (0)     3685 2023-05-09 15:49:23.000000 blond-2.1.2/blond/beam/coasting_beam.py
+-rw-r--r--   0 root         (0) root         (0)    41527 2023-05-09 15:49:23.000000 blond-2.1.2/blond/beam/distributions.py
+-rw-r--r--   0 root         (0) root         (0)    39107 2023-05-09 15:49:23.000000 blond-2.1.2/blond/beam/distributions_multibunch.py
+-rw-r--r--   0 root         (0) root         (0)    24385 2023-05-09 15:49:23.000000 blond-2.1.2/blond/beam/profile.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-05-09 15:49:23.000000 blond-2.1.2/blond/beam/sparse_histogram.cpp
+-rw-r--r--   0 root         (0) root         (0)     4804 2023-05-09 15:49:23.000000 blond-2.1.2/blond/beam/sparse_slices.py
+-rw-r--r--   0 root         (0) root         (0)    11654 2023-05-09 15:49:23.000000 blond-2.1.2/blond/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.640000 blond-2.1.2/blond/cpp_routines/
+-rw-r--r--   0 root         (0) root         (0)     3088 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/beam_phase.cpp
+-rw-r--r--   0 root         (0) root         (0)    29022 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/blondmath.cpp
+-rw-r--r--   0 root         (0) root         (0)    13334 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/blondmath.h
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/cos.h
+-rw-r--r--   0 root         (0) root         (0)     5747 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/drift.cpp
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/exp.h
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/fast_resonator.cpp
+-rw-r--r--   0 root         (0) root         (0)    29481 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/fft.cpp
+-rw-r--r--   0 root         (0) root         (0)     4419 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/fft.h
+-rw-r--r--   0 root         (0) root         (0)    10031 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/histogram.cpp
+-rw-r--r--   0 root         (0) root         (0)     3493 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/kick.cpp
+-rwxr-xr-x   0 root         (0) root         (0)   126096 2023-05-09 15:49:52.000000 blond-2.1.2/blond/cpp_routines/libblond.so
+-rw-r--r--   0 root         (0) root         (0)     6406 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/linear_interp_kick.cpp
+-rw-r--r--   0 root         (0) root         (0)    15181 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/music_track.cpp
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/openmp.cpp
+-rw-r--r--   0 root         (0) root         (0)      245 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/openmp.h
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/sin.h
+-rw-r--r--   0 root         (0) root         (0)     5871 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/sincos.h
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/vdtcore_common.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.640000 blond-2.1.2/blond/gpu/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/gpu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.640000 blond-2.1.2/blond/gpu/cuda_kernels/
+-rw-r--r--   0 root         (0) root         (0)    14390 2023-05-09 15:49:23.000000 blond-2.1.2/blond/gpu/cuda_kernels/kernels_double.cu
+-rw-r--r--   0 root         (0) root         (0)    14135 2023-05-09 15:49:23.000000 blond-2.1.2/blond/gpu/cuda_kernels/kernels_single.cu
+-rw-r--r--   0 root         (0) root         (0)    10769 2023-05-09 15:49:23.000000 blond-2.1.2/blond/gpu/cupy_butils_wrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.644000 blond-2.1.2/blond/impedances/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/impedances/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39560 2023-05-09 15:49:23.000000 blond-2.1.2/blond/impedances/impedance.py
+-rw-r--r--   0 root         (0) root         (0)    45896 2023-05-09 15:49:23.000000 blond-2.1.2/blond/impedances/impedance_sources.py
+-rw-r--r--   0 root         (0) root         (0)     3529 2023-05-09 15:49:23.000000 blond-2.1.2/blond/impedances/induced_voltage_analytical.py
+-rw-r--r--   0 root         (0) root         (0)    12228 2023-05-09 15:49:23.000000 blond-2.1.2/blond/impedances/music.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.644000 blond-2.1.2/blond/input_parameters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/input_parameters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24903 2023-05-09 15:49:23.000000 blond-2.1.2/blond/input_parameters/rf_parameters.py
+-rw-r--r--   0 root         (0) root         (0)    20249 2023-05-09 15:49:23.000000 blond-2.1.2/blond/input_parameters/rf_parameters_options.py
+-rw-r--r--   0 root         (0) root         (0)    17272 2023-05-09 15:49:23.000000 blond-2.1.2/blond/input_parameters/ring.py
+-rw-r--r--   0 root         (0) root         (0)    22443 2023-05-09 15:49:23.000000 blond-2.1.2/blond/input_parameters/ring_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.644000 blond-2.1.2/blond/llrf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22090 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/beam_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    36313 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/cavity_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    14383 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/impulse_response.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/notch_filter.py
+-rw-r--r--   0 root         (0) root         (0)     7257 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/offset_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     4394 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/rf_modulation.py
+-rw-r--r--   0 root         (0) root         (0)    15759 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/rf_noise.py
+-rw-r--r--   0 root         (0) root         (0)    18814 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/signal_processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.644000 blond-2.1.2/blond/monitors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/monitors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20936 2023-05-09 15:49:23.000000 blond-2.1.2/blond/monitors/monitors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.644000 blond-2.1.2/blond/plots/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/plots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11025 2023-05-09 15:49:23.000000 blond-2.1.2/blond/plots/plot.py
+-rw-r--r--   0 root         (0) root         (0)    10004 2023-05-09 15:49:23.000000 blond-2.1.2/blond/plots/plot_beams.py
+-rw-r--r--   0 root         (0) root         (0)     4777 2023-05-09 15:49:23.000000 blond-2.1.2/blond/plots/plot_impedance.py
+-rw-r--r--   0 root         (0) root         (0)    14165 2023-05-09 15:49:23.000000 blond-2.1.2/blond/plots/plot_llrf.py
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-05-09 15:49:23.000000 blond-2.1.2/blond/plots/plot_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2023-05-09 15:49:23.000000 blond-2.1.2/blond/plots/plot_slices.py
+-rw-r--r--   0 root         (0) root         (0)     6671 2023-05-09 15:49:23.000000 blond-2.1.2/blond/sanity_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.644000 blond-2.1.2/blond/synchrotron_radiation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/synchrotron_radiation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5364 2023-05-09 15:49:23.000000 blond-2.1.2/blond/synchrotron_radiation/synchrotron_radiation.cpp
+-rw-r--r--   0 root         (0) root         (0)     8111 2023-05-09 15:49:23.000000 blond-2.1.2/blond/synchrotron_radiation/synchrotron_radiation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.648000 blond-2.1.2/blond/toolbox/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5221 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/action.py
+-rw-r--r--   0 root         (0) root         (0)     7570 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/diffusion.py
+-rw-r--r--   0 root         (0) root         (0)     7479 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/filters_and_fitting.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/logger.py
+-rw-r--r--   0 root         (0) root         (0)     3377 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/next_regular.py
+-rw-r--r--   0 root         (0) root         (0)    21008 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/parameter_scaling.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/tomoscope.cpp
+-rw-r--r--   0 root         (0) root         (0)     4877 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/tomoscope.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.648000 blond-2.1.2/blond/trackers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/trackers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26351 2023-05-09 15:49:23.000000 blond-2.1.2/blond/trackers/tracker.py
+-rw-r--r--   0 root         (0) root         (0)    31248 2023-05-09 15:49:23.000000 blond-2.1.2/blond/trackers/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.648000 blond-2.1.2/blond/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8233 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/bmath.py
+-rw-r--r--   0 root         (0) root         (0)    48243 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/butils_wrap.py
+-rw-r--r--   0 root         (0) root         (0)     3467 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     4145 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/input_parser.py
+-rw-r--r--   0 root         (0) root         (0)    14206 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/mpi_config.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/profile_mock.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/track_iteration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.636000 blond-2.1.2/blond.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13940 2023-05-09 15:49:52.000000 blond-2.1.2/blond.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9913 2023-05-09 15:49:52.000000 blond-2.1.2/blond.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 15:49:52.000000 blond-2.1.2/blond.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 15:49:48.000000 blond-2.1.2/blond.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      400 2023-05-09 15:49:52.000000 blond-2.1.2/blond.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-09 15:49:52.000000 blond-2.1.2/blond.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      207 2023-05-09 15:49:23.000000 blond-2.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-09 15:49:23.000000 blond-2.1.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 15:49:52.656000 blond-2.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4808 2023-05-09 15:49:23.000000 blond-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.616000 blond-2.1.2/unittests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.648000 blond-2.1.2/unittests/beam_profile/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/beam_profile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   800196 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/beam_profile/dt_coordinates.npz
+-rw-r--r--   0 root         (0) root         (0)    12422 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/beam_profile/test_beam_profile_object.py
+-rw-r--r--   0 root         (0) root         (0)     7221 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/beam_profile/test_sparse_profile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.652000 blond-2.1.2/unittests/beams/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/beams/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14105 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/beams/test_beam_object.py
+-rw-r--r--   0 root         (0) root         (0)     5659 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/beams/test_coasting_beam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.652000 blond-2.1.2/unittests/general/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/general/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16184 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/general/test_separatrix_bigaussian.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.652000 blond-2.1.2/unittests/gpu/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/gpu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/gpu/test_ffts.py
+-rw-r--r--   0 root         (0) root         (0)    16996 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/gpu/test_impedance.py
+-rw-r--r--   0 root         (0) root         (0)    22133 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/gpu/test_physics_kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.652000 blond-2.1.2/unittests/impedances/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/impedances/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4475 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/impedances/test_impedance.py
+-rwxr-xr-x   0 root         (0) root         (0)     4940 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/impedances/test_impedance_sources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.652000 blond-2.1.2/unittests/input_parameters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/input_parameters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/input_parameters/test_preprocess.py
+-rw-r--r--   0 root         (0) root         (0)    10862 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/input_parameters/test_rf_params_object.py
+-rw-r--r--   0 root         (0) root         (0)     7576 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/input_parameters/test_ring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.652000 blond-2.1.2/unittests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4307 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/integration/test_examples.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/integration/test_gpu_examples.py
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/integration/test_mpi_examples.py
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/integration/test_validate_gpu.py
+-rw-r--r--   0 root         (0) root         (0)     4005 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/integration/test_validate_mpi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.656000 blond-2.1.2/unittests/llrf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    74048 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/ref_DV_MOD_FR.npy
+-rw-r--r--   0 root         (0) root         (0)    74048 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/ref_DV_MOD_FRF.npy
+-rw-r--r--   0 root         (0) root         (0)    74048 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/ref_V_IND_COARSE_GEN.npy
+-rw-r--r--   0 root         (0) root         (0)     8741 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/test_beam_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    31675 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/test_cavity_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    40554 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/test_impulse_response.py
+-rw-r--r--   0 root         (0) root         (0)     3649 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/test_offset_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     8157 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/test_rf_modulation.py
+-rw-r--r--   0 root         (0) root         (0)    31838 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/test_signal_processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.656000 blond-2.1.2/unittests/synchrotron_radiation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/synchrotron_radiation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32615 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/synchrotron_radiation/test_synch_rad.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.656000 blond-2.1.2/unittests/trackers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/trackers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17866 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/trackers/comparison_drift.py
+-rw-r--r--   0 root         (0) root         (0)    19415 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/trackers/test_drift.py
+-rw-r--r--   0 root         (0) root         (0)    10188 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/trackers/test_tracker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.656000 blond-2.1.2/unittests/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21108 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/utils/test_blondmath.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/utils/test_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     9952 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/utils/test_ffts.py
+-rw-r--r--   0 root         (0) root         (0)     5103 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/utils/test_iteration.py
```

### Comparing `blond-2.1.1/.gitignore` & `blond-2.1.2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 *.cubin
 .pytest_cache
 .ipynb_checkpoints
 *__pycache__
 *.DS_Store
 *egg-info
 venvs
+.vscode
 
 # End of placeholder for user defined entries
 
 # Custom entries added by Java DevTools (accsoft-devtools-support@cern.ch)
 
 *.pyc
 *core.[0-9]*
```

### Comparing `blond-2.1.1/.gitlab-ci.yml` & `blond-2.1.2/.gitlab-ci.yml`

 * *Files 23% similar despite different names*

```diff
@@ -99,7 +99,24 @@
    - python3 -m twine upload --verbose
         --repository-url="${PYPI_UPLOAD_URL}"
         --username="${PYPI_USERNAME}"
         --password="${PYPI_PASSWORD}"
         dist/*.tar.gz
 
 
+pages:
+  variables:
+    PY_VERSION: "3.9"
+  image: python:${PY_VERSION}
+  script:
+   - cd ${project_root}
+   - mkdir public
+  #  - python3 -m pip install --upgrade pyqt5 sphinx sphinx-rtd-theme sphinxcontrib-napoleon sphinx-autopackagesummary
+  #  - python3 -m pip install -r requirements
+   - python3 -m pip install -v ${project_root}[doc]
+   - make -C __doc html
+   - cp -r __doc/_build/html/* public/
+  artifacts:
+    paths:
+     - ${project_root}public
+  only:
+   - master
```

### Comparing `blond-2.1.1/CHANGELOG` & `blond-2.1.2/CHANGELOG`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/LICENSE.txt` & `blond-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/PKG-INFO` & `blond-2.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blond
-Version: 2.1.1
+Version: 2.1.2
 Summary: CERN code for simulating longitudinal beam dynamics in synchrotrons.
 Home-page: https://gitlab.cern.ch/blond/BLonD
 Author: Helga Timko et al.
 Author-email: helga.timko@cern.ch
 Maintainer: Konstantinos Iliakis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -17,17 +17,17 @@
 Provides-Extra: core
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.txt
 
-# Code Name
+[![Pipeline Status](https://gitlab.cern.ch/blond/BLonD/badges/master/pipeline.svg)](https://gitlab.cern.ch/blond/BLonD/-/commits/master) [![Coverage Report](https://gitlab.cern.ch/blond/BLonD/badges/master/coverage.svg)](https://gitlab.cern.ch/blond/BLonD/-/commits/master) [![Latest Release](https://gitlab.cern.ch/blond/BLonD/-/badges/release.svg)](https://gitlab.cern.ch/blond/BLonD/-/releases) [![PyPi](https://img.shields.io/pypi/v/blond.svg)](https://pypi.org/project/blond/) [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org) [![Documentation Pages](https://img.shields.io/badge/docs-sphinx-blue)](https://blond-code.docs.cern.ch/)
 
-BLonD (Beam Longitudinal Dynamics)
+# Beam Longitudinal Dynamics Code (BLonD)
 
 # Copyright Notice
 
 *Copyright 2019 CERN. This software is distributed under the terms of the
 GNU General Public Licence version 3 (GPL Version 3), copied verbatim in
 the file LICENCE.txt. In applying this licence, CERN does not waive the
 privileges and immunities granted to it by virtue of its status as an
@@ -36,17 +36,17 @@
 # Description
 
 CERN code for the simulation of longitudinal beam dynamics in
 synchrotrons.
 
 # Useful Links
 
-Repository: <https://github.com/blond-admin/BLonD>
+Repository: <https://gitlab.cern.ch/blond/BLonD>
 
-Documentation: <http://blond-admin.github.io/BLonD/>
+Documentation: <https://blond-code.docs.cern.ch/>
 
 Project website: <http://blond.web.cern.ch>
 
 # Install
 
 ## Requirements
```

### Comparing `blond-2.1.1/README.md` & `blond-2.1.2/blond.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,33 @@
-# Code Name
+Metadata-Version: 2.1
+Name: blond
+Version: 2.1.2
+Summary: CERN code for simulating longitudinal beam dynamics in synchrotrons.
+Home-page: https://gitlab.cern.ch/blond/BLonD
+Author: Helga Timko et al.
+Author-email: helga.timko@cern.ch
+Maintainer: Konstantinos Iliakis
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: core
+Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: doc
+Provides-Extra: all
+License-File: LICENSE.txt
 
-BLonD (Beam Longitudinal Dynamics)
+[![Pipeline Status](https://gitlab.cern.ch/blond/BLonD/badges/master/pipeline.svg)](https://gitlab.cern.ch/blond/BLonD/-/commits/master) [![Coverage Report](https://gitlab.cern.ch/blond/BLonD/badges/master/coverage.svg)](https://gitlab.cern.ch/blond/BLonD/-/commits/master) [![Latest Release](https://gitlab.cern.ch/blond/BLonD/-/badges/release.svg)](https://gitlab.cern.ch/blond/BLonD/-/releases) [![PyPi](https://img.shields.io/pypi/v/blond.svg)](https://pypi.org/project/blond/) [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org) [![Documentation Pages](https://img.shields.io/badge/docs-sphinx-blue)](https://blond-code.docs.cern.ch/)
+
+# Beam Longitudinal Dynamics Code (BLonD)
 
 # Copyright Notice
 
 *Copyright 2019 CERN. This software is distributed under the terms of the
 GNU General Public Licence version 3 (GPL Version 3), copied verbatim in
 the file LICENCE.txt. In applying this licence, CERN does not waive the
 privileges and immunities granted to it by virtue of its status as an
@@ -13,17 +36,17 @@
 # Description
 
 CERN code for the simulation of longitudinal beam dynamics in
 synchrotrons.
 
 # Useful Links
 
-Repository: <https://github.com/blond-admin/BLonD>
+Repository: <https://gitlab.cern.ch/blond/BLonD>
 
-Documentation: <http://blond-admin.github.io/BLonD/>
+Documentation: <https://blond-code.docs.cern.ch/>
 
 Project website: <http://blond.web.cern.ch>
 
 # Install
 
 ## Requirements
```

### Comparing `blond-2.1.1/WARNINGS.txt` & `blond-2.1.2/WARNINGS.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__BENCHMARKS/BM1_OTFB_Vind_beam_1.py` & `blond-2.1.2/__BENCHMARKS/BM1_OTFB_Vind_beam_1.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__BENCHMARKS/BM2_OTFB_no_beam.py` & `blond-2.1.2/__BENCHMARKS/BM2_OTFB_no_beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__BENCHMARKS/BM3_OTFB_moving_average.py` & `blond-2.1.2/__BENCHMARKS/BM3_OTFB_moving_average.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__BENCHMARKS/BM4_OTFB_with_beam.py` & `blond-2.1.2/__BENCHMARKS/BM4_OTFB_with_beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__BENCHMARKS/BM5_OTFB_feedforward.py` & `blond-2.1.2/__BENCHMARKS/BM5_OTFB_feedforward.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_01_Acceleration.py` & `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_01_Acceleration.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_02_Main_long_ps_booster.py` & `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_02_Main_long_ps_booster.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_03_RFnoise.py` & `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_03_RFnoise.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_04_Stationary_multistation.py` & `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_04_Stationary_multistation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_05_Wake_impedance.py` & `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_05_Wake_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_07_Ions.py` & `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_07_Ions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_08_Phase_Loop.py` & `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_08_Phase_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_09_Radial_Loop.py` & `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_09_Radial_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_10_Fixed_frequency.py` & `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_10_Fixed_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_16_impedance_test.py` & `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_16_impedance_test.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_17_multi_turn_wake.py` & `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_17_multi_turn_wake.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/gpu_main_files/EX_18_robinson_instability.py` & `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_18_robinson_instability.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/input_files/EX_02_Ekicker_1.4GeV.txt` & `blond-2.1.2/__EXAMPLES/input_files/EX_02_Ekicker_1.4GeV.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/input_files/EX_02_Finemet.txt` & `blond-2.1.2/__EXAMPLES/input_files/EX_02_Finemet.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/input_files/EX_05_new_HQ_table.dat` & `blond-2.1.2/__EXAMPLES/input_files/EX_05_new_HQ_table.dat`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/input_files/EX_06_Source_TOF_P.csv` & `blond-2.1.2/__EXAMPLES/input_files/EX_06_Source_TOF_P.csv`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_01_Acceleration.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_01_Acceleration.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_02_Main_long_ps_booster.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_02_Main_long_ps_booster.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_03_RFnoise.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_03_RFnoise.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_04_Stationary_multistation.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_04_Stationary_multistation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_05_Wake_impedance.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_05_Wake_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_06_Preprocess.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_06_Preprocess.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_07_Ions.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_07_Ions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_08_Phase_Loop.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_08_Phase_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_09_Radial_Loop.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_09_Radial_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_10_Fixed_frequency.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_10_Fixed_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_11_comparison_music_fourier_analytical.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_11_comparison_music_fourier_analytical.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_12_synchrotron_frequency_distribution.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_12_synchrotron_frequency_distribution.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_13_synchrotron_radiation.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_13_synchrotron_radiation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_14_sparse_slicing.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_14_sparse_slicing.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_15_sparse_multi_bunch.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_15_sparse_multi_bunch.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_16_impedance_test.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_16_impedance_test.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_17_multi_turn_wake.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_17_multi_turn_wake.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_18_robinson_instability.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_18_robinson_instability.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_19_bunch_generation.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_19_bunch_generation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_20_bunch_generation_multibunch.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_20_bunch_generation_multibunch.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_21_bunch_distribution.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_21_bunch_distribution.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/main_files/EX_22_Coherent_Radiation.py` & `blond-2.1.2/__EXAMPLES/main_files/EX_22_Coherent_Radiation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_01_Acceleration.py` & `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_01_Acceleration.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_02_Main_long_ps_booster.py` & `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_02_Main_long_ps_booster.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_03_RFnoise.py` & `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_03_RFnoise.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_04_Stationary_multistation.py` & `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_04_Stationary_multistation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_05_Wake_impedance.py` & `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_05_Wake_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_07_Ions.py` & `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_07_Ions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_08_Phase_Loop.py` & `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_08_Phase_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_09_Radial_Loop.py` & `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_09_Radial_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_10_Fixed_frequency.py` & `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_10_Fixed_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_16_impedance_test.py` & `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_16_impedance_test.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__EXAMPLES/mpi_main_files/EX_18_robinson_instability.py` & `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_18_robinson_instability.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/Makefile` & `blond-2.1.2/__doc/Makefile`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/conf.py` & `blond-2.1.2/__doc/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,30 +61,31 @@
 master_doc = 'index'
 
 # General information about the project.
 project = u'BLonD'
 copyright = u'2017'
 author = u'BLonD-admin'
 
+autodoc_mock_imports = ["mpi4py", "cupy"]
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = u'1.1'
+version = u'2.1'
 # The full version, including alpha/beta/rc tags.
-release = u'1.1'
+release = u'2.1'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 #exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store', '_themes']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
@@ -110,14 +111,19 @@
 #html_theme = 'sphinxdoc'
 #html_theme = 'classic'
 #html_theme = 'alabaster'
 
 html_theme = 'sphinx_rtd_theme'
 html_theme_path = ["themes",]
 
+# html_theme_options = {
+#     'collapsiblesidebar': True,
+#     'externalrefs':True,
+# }
+
 html_theme_options = {
     'collapse_navigation':False,
     'sticky_navigation':False,
     'navigation_depth':3
 }
 
 # Theme options are theme-specific and customize the look and feel of a theme
```

### Comparing `blond-2.1.1/__doc/index.rst` & `blond-2.1.2/__doc/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 ===================================
 
 Contents
 ========
 The Beam Longitudinal Dynamics code BLonD is a CERN software package for the
 simulatation of longitudinal beam dynamics in synchrotrons.
 
-Visit the BLonD website_ for more details and the github_ distribution to 
+Visit the BLonD website_ for more details and the gitlab_ distribution to 
 download the code.
 
 .. _website: http://blond.web.cern.ch/
-.. _github: https://github.com/blond-admin/BLonD/releases
+.. _gitlab: https://gitlab.cern.ch/blond/BLonD
 
 Modules
 =======
 
 .. toctree::
     :maxdepth: 2
 
@@ -31,16 +31,17 @@
     modules/input_parameters.rst
     modules/llrf.rst
     modules/monitors.rst
     modules/plots.rst
     modules/synchrotron_radiation.rst
     modules/toolbox.rst
     modules/trackers.rst
-    modules/compile.rst
     modules/utils.rst
+    modules/compile.rst
+    modules/sanity_check.rst
 
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
```

### Comparing `blond-2.1.1/__doc/make.bat` & `blond-2.1.2/__doc/make.bat`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/ACS_cavity_loop.png` & `blond-2.1.2/__doc/modules/ACS_cavity_loop.png`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/ACS_cavity_loop.svg` & `blond-2.1.2/__doc/modules/ACS_cavity_loop.svg`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/RF_noise.gle` & `blond-2.1.2/__doc/modules/RF_noise.gle`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/RF_noise.png` & `blond-2.1.2/__doc/modules/RF_noise.png`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/SPS_OTFB.png` & `blond-2.1.2/__doc/modules/SPS_OTFB.png`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/SPS_OTFB.svg` & `blond-2.1.2/__doc/modules/SPS_OTFB.svg`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/beam.rst` & `blond-2.1.2/__doc/modules/beam.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/csr_impedance_real.png` & `blond-2.1.2/__doc/modules/csr_impedance_real.png`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/equations_of_motion.rst` & `blond-2.1.2/__doc/modules/equations_of_motion.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/impedances.rst` & `blond-2.1.2/__doc/modules/impedances.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/input_parameters.rst` & `blond-2.1.2/__doc/modules/input_parameters.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 ---------------------------
 
 .. automodule:: blond.input_parameters.rf_parameters
     :members:
     :undoc-members:
     :show-inheritance:
 
+:mod:`rf_parameters_options` Module
+-----------------------------------
+
+.. automodule:: blond.input_parameters.rf_parameters_options
+    :members:
+    :undoc-members:
+    :show-inheritance:
+
 :mod:`ring` Module
 ------------------
 
 .. automodule:: blond.input_parameters.ring
     :members:
     :undoc-members:
     :show-inheritance:
@@ -21,16 +29,8 @@
 --------------------------
 
 .. automodule:: blond.input_parameters.ring_options
     :members:
     :undoc-members:
     :show-inheritance:
 
-:mod:`rf_parameters_options` Module
------------------------------------
-
-.. automodule:: blond.input_parameters.rf_parameters_options
-    :members:
-    :undoc-members:
-    :show-inheritance:
-
```

### Comparing `blond-2.1.1/__doc/modules/lhc_cavity_loop.rst` & `blond-2.1.2/__doc/modules/lhc_cavity_loop.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/llrf.rst` & `blond-2.1.2/__doc/modules/llrf.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/plots.rst` & `blond-2.1.2/__doc/modules/plots.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/ring_and_RFstation.gle` & `blond-2.1.2/__doc/modules/ring_and_RFstation.gle`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/ring_and_RFstation.png` & `blond-2.1.2/__doc/modules/ring_and_RFstation.png`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/sps_cavity_loop.rst` & `blond-2.1.2/__doc/modules/sps_cavity_loop.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/modules/toolbox.rst` & `blond-2.1.2/__doc/modules/toolbox.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/breadcrumbs.html` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/footer.html` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/footer.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/layout.html` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/layout.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/layout_old.html` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/layout_old.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/search.html` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/search.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css.map` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css.map`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/theme.css` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/css/theme.css.map` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/theme.css.map`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/FontAwesome.otf` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Bold.ttf` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Bold.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Regular.ttf` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Regular.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Bold.ttf` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Regular.ttf` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Bold.ttf` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Bold.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Regular.ttf` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Regular.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff2` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/js/modernizr.min.js` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/js/modernizr.min.js`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/static/js/theme.js` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/__doc/themes/sphinx_rtd_theme/versions.html` & `blond-2.1.2/__doc/themes/sphinx_rtd_theme/versions.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/appveyor.yml` & `blond-2.1.2/appveyor.yml`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/__init__.py` & `blond-2.1.2/blond/__init__.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/beam/beam.py` & `blond-2.1.2/blond/beam/beam.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,16 +156,14 @@
         standard deviation of beam energy offset [eV].
     intensity : float
         total intensity of the beam in number of charges [].
     n_macroparticles : int
         total number of macroparticles in the beam [].
     ratio : float
         ratio intensity per macroparticle [].
-    n_macroparticles_lost : int
-        number of macro-particles marked as 'lost' [].
     id : numpy_array, int
         unique macro-particle ID number; zero if particle is 'lost'.
 
     See Also
     ---------
     distributions.matched_from_line_density:
         match a beam with a given bunch profile.
```

### Comparing `blond-2.1.1/blond/beam/coasting_beam.py` & `blond-2.1.2/blond/beam/coasting_beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/beam/distributions.py` & `blond-2.1.2/blond/beam/distributions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/beam/distributions_multibunch.py` & `blond-2.1.2/blond/beam/distributions_multibunch.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/beam/profile.py` & `blond-2.1.2/blond/beam/profile.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/beam/sparse_histogram.cpp` & `blond-2.1.2/blond/beam/sparse_histogram.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/beam/sparse_slices.py` & `blond-2.1.2/blond/beam/sparse_slices.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/compile.py` & `blond-2.1.2/blond/compile.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/cpp_routines/beam_phase.cpp` & `blond-2.1.2/blond/cpp_routines/beam_phase.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/cpp_routines/blondmath.cpp` & `blond-2.1.2/blond/cpp_routines/blondmath.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/cpp_routines/blondmath.h` & `blond-2.1.2/blond/cpp_routines/blondmath.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/cpp_routines/cos.h` & `blond-2.1.2/blond/cpp_routines/cos.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/cpp_routines/drift.cpp` & `blond-2.1.2/blond/cpp_routines/drift.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/cpp_routines/exp.h` & `blond-2.1.2/blond/cpp_routines/exp.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/cpp_routines/fast_resonator.cpp` & `blond-2.1.2/blond/cpp_routines/fast_resonator.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/cpp_routines/fft.cpp` & `blond-2.1.2/blond/cpp_routines/fft.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/cpp_routines/fft.h` & `blond-2.1.2/blond/cpp_routines/fft.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/cpp_routines/histogram.cpp` & `blond-2.1.2/blond/cpp_routines/histogram.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         histo[i] = (*histo + n_slices * i);
 
     #pragma omp parallel
     {
         const int id = omp_get_thread_num();
         const int threads = omp_get_num_threads();
         memset(histo[id], 0., n_slices * sizeof(double));
-        float fbin[STEP];
+        float fbin[STEP] = { -1 };
         #pragma omp for
         for (int i = 0; i < n_macroparticles; i += STEP) {
 
             const int loop_count = n_macroparticles - i > STEP ?
                                    STEP : n_macroparticles - i;
 
             // First calculate the index to update
@@ -150,15 +150,15 @@
     }
 
     #pragma omp parallel
     {
         const int id = omp_get_thread_num();
         const int threads = omp_get_num_threads();
         memset(histo[id], 0., n_slices * sizeof(float));
-        float fbin[STEP];
+        float fbin[STEP] = { -1 };
         #pragma omp for
         for (int i = 0; i < n_macroparticles; i += STEP) {
 
             const int loop_count = n_macroparticles - i > STEP ?
                                    STEP : n_macroparticles - i;
 
             // First calculate the index to update
```

### Comparing `blond-2.1.1/blond/cpp_routines/kick.cpp` & `blond-2.1.2/blond/cpp_routines/kick.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/cpp_routines/libblond.so` & `blond-2.1.2/blond/cpp_routines/libblond.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 2% similar despite different names*

#### readelf --wide --program-header {}

```diff
@@ -2,16 +2,16 @@
 Elf file type is DYN (Shared object file)
 Entry point 0x32d0
 There are 10 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
   LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x002770 0x002770 R   0x1000
-  LOAD           0x003000 0x0000000000003000 0x0000000000003000 0x0142bd 0x0142bd R E 0x1000
-  LOAD           0x018000 0x0000000000018000 0x0000000000018000 0x00223c 0x00223c R   0x1000
+  LOAD           0x003000 0x0000000000003000 0x0000000000003000 0x01427d 0x01427d R E 0x1000
+  LOAD           0x018000 0x0000000000018000 0x0000000000018000 0x002234 0x002234 R   0x1000
   LOAD           0x01ada0 0x000000000001bda0 0x000000000001bda0 0x0003d8 0x0003f0 RW  0x1000
   DYNAMIC        0x01adc0 0x000000000001bdc0 0x000000000001bdc0 0x000200 0x000200 RW  0x8
   NOTE           0x000270 0x0000000000000270 0x0000000000000270 0x000024 0x000024 R   0x4
   TLS            0x01ada0 0x000000000001bda0 0x000000000001bda0 0x000000 0x000068 R   0x10
   GNU_EH_FRAME   0x018480 0x0000000000018480 0x0000000000018480 0x0004ac 0x0004ac R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
   GNU_RELRO      0x01ada0 0x000000000001bda0 0x000000000001bda0 0x000260 0x000260 R   0x1
```

#### readelf --wide --sections {}

```diff
@@ -10,20 +10,20 @@
   [ 5] .gnu.version      VERSYM          0000000000002064 002064 000126 02   A  3   0  2
   [ 6] .gnu.version_r    VERNEED         0000000000002190 002190 0000d0 00   A  4   5  8
   [ 7] .rela.dyn         RELA            0000000000002260 002260 000138 18   A  3   0  8
   [ 8] .rela.plt         RELA            0000000000002398 002398 0003d8 18  AI  3  23  8
   [ 9] .init             PROGBITS        0000000000003000 003000 000017 00  AX  0   0  4
   [10] .plt              PROGBITS        0000000000003020 003020 0002a0 10  AX  0   0 16
   [11] .plt.got          PROGBITS        00000000000032c0 0032c0 000008 08  AX  0   0  8
-  [12] .text             PROGBITS        00000000000032d0 0032d0 013fe1 00  AX  0   0 16
-  [13] .fini             PROGBITS        00000000000172b4 0172b4 000009 00  AX  0   0  4
+  [12] .text             PROGBITS        00000000000032d0 0032d0 013fa1 00  AX  0   0 16
+  [13] .fini             PROGBITS        0000000000017274 017274 000009 00  AX  0   0  4
   [14] .rodata           PROGBITS        0000000000018000 018000 000480 00   A  0   0 16
   [15] .eh_frame_hdr     PROGBITS        0000000000018480 018480 0004ac 00   A  0   0  4
-  [16] .eh_frame         PROGBITS        0000000000018930 018930 0018c8 00   A  0   0  8
-  [17] .gcc_except_table PROGBITS        000000000001a1f8 01a1f8 000044 00   A  0   0  1
+  [16] .eh_frame         PROGBITS        0000000000018930 018930 0018c0 00   A  0   0  8
+  [17] .gcc_except_table PROGBITS        000000000001a1f0 01a1f0 000044 00   A  0   0  1
   [18] .tbss             NOBITS          000000000001bda0 01ada0 000068 00 WAT  0   0 16
   [19] .init_array       INIT_ARRAY      000000000001bda0 01ada0 000018 08  WA  0   0  8
   [20] .fini_array       FINI_ARRAY      000000000001bdb8 01adb8 000008 08  WA  0   0  8
   [21] .dynamic          DYNAMIC         000000000001bdc0 01adc0 000200 10  WA  4   0  8
   [22] .got              PROGBITS        000000000001bfc0 01afc0 000040 08  WA  0   0  8
   [23] .got.plt          PROGBITS        000000000001c000 01b000 000160 08  WA  0   0  8
   [24] .data             PROGBITS        000000000001c160 01b160 000018 00  WA  0   0  8
```

#### readelf --wide --symbols {}

```diff
@@ -22,135 +22,135 @@
     18: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __gxx_personality_v0@CXXABI_1.3 (7)
     19: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __tls_get_addr@GLIBC_2.3 (8)
     20: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
     21: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _Unwind_Resume@GCC_3.0 (9)
     22: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
     23: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
     24: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt8ios_base4InitD1Ev@GLIBCXX_3.4 (2)
-    25: 000000000000c760  1914 FUNC    GLOBAL DEFAULT   12 music_track
-    26: 00000000000124c0    38 FUNC    GLOBAL DEFAULT   12 scalar_mul_int64
-    27: 0000000000012ba0   926 FUNC    GLOBAL DEFAULT   12 sort_double
-    28: 000000000000d950  2002 FUNC    GLOBAL DEFAULT   12 music_trackf
-    29: 0000000000010fb0    81 FUNC    GLOBAL DEFAULT   12 fast_expv
-    30: 00000000000105d0   185 FUNC    GLOBAL DEFAULT   12 mean
-    31: 0000000000010f50    81 FUNC    GLOBAL DEFAULT   12 fast_cosv
-    32: 0000000000013f80   427 FUNC    WEAK   DEFAULT   12 _ZSt16__introsort_loopIPflN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIfEEEEvT_S7_T0_T1_
-    33: 000000000000f990   255 FUNC    GLOBAL DEFAULT   12 wheref
-    34: 000000000000fe70   191 FUNC    GLOBAL DEFAULT   12 add_uint16_vector_inplace
+    25: 000000000000c720  1914 FUNC    GLOBAL DEFAULT   12 music_track
+    26: 0000000000012480    38 FUNC    GLOBAL DEFAULT   12 scalar_mul_int64
+    27: 0000000000012b60   926 FUNC    GLOBAL DEFAULT   12 sort_double
+    28: 000000000000d910  2002 FUNC    GLOBAL DEFAULT   12 music_trackf
+    29: 0000000000010f70    81 FUNC    GLOBAL DEFAULT   12 fast_expv
+    30: 0000000000010590   185 FUNC    GLOBAL DEFAULT   12 mean
+    31: 0000000000010f10    81 FUNC    GLOBAL DEFAULT   12 fast_cosv
+    32: 0000000000013f40   427 FUNC    WEAK   DEFAULT   12 _ZSt16__introsort_loopIPflN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIfEEEEvT_S7_T0_T1_
+    33: 000000000000f950   255 FUNC    GLOBAL DEFAULT   12 wheref
+    34: 000000000000fe30   191 FUNC    GLOBAL DEFAULT   12 add_uint16_vector_inplace
     35: 0000000000008510  3439 FUNC    GLOBAL DEFAULT   12 driftf
-    36: 0000000000011820    75 FUNC    GLOBAL DEFAULT   12 min_idx
-    37: 0000000000011f30    75 FUNC    GLOBAL DEFAULT   12 min_idxf
-    38: 000000000000fc90    85 FUNC    GLOBAL DEFAULT   12 add_longint_vector
-    39: 0000000000016c20   256 FUNC    WEAK   DEFAULT   12 _ZNSt23mersenne_twister_engineImLm64ELm312ELm156ELm31ELm13043109905998158313ELm29ELm6148914691236517205ELm17ELm8202884508482404352ELm37ELm18444473444759240704ELm43ELm6364136223846793005EE11_M_gen_randEv
-    40: 000000000000e400   336 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorI8particleIfESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
-    41: 0000000000015a10   377 FUNC    GLOBAL DEFAULT   12 beam_phasef
-    42: 000000000000f190   541 FUNC    GLOBAL DEFAULT   12 where_more_thanf
-    43: 0000000000010110   522 FUNC    GLOBAL DEFAULT   12 convolution
+    36: 00000000000117e0    75 FUNC    GLOBAL DEFAULT   12 min_idx
+    37: 0000000000011ef0    75 FUNC    GLOBAL DEFAULT   12 min_idxf
+    38: 000000000000fc50    85 FUNC    GLOBAL DEFAULT   12 add_longint_vector
+    39: 0000000000016be0   256 FUNC    WEAK   DEFAULT   12 _ZNSt23mersenne_twister_engineImLm64ELm312ELm156ELm31ELm13043109905998158313ELm29ELm6148914691236517205ELm17ELm8202884508482404352ELm37ELm18444473444759240704ELm43ELm6364136223846793005EE11_M_gen_randEv
+    40: 000000000000e3c0   336 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorI8particleIfESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
+    41: 00000000000159d0   377 FUNC    GLOBAL DEFAULT   12 beam_phasef
+    42: 000000000000f150   541 FUNC    GLOBAL DEFAULT   12 where_more_thanf
+    43: 00000000000100d0   522 FUNC    GLOBAL DEFAULT   12 convolution
     44: 000000000001c170     8 OBJECT  GLOBAL DEFAULT   24 seed
-    45: 000000000000cee0  2671 FUNC    GLOBAL DEFAULT   12 music_track_multiturnf
+    45: 000000000000cea0  2671 FUNC    GLOBAL DEFAULT   12 music_track_multiturnf
     46: 0000000000009280   695 FUNC    GLOBAL DEFAULT   12 linear_interp_kick
-    47: 00000000000119d0   261 FUNC    GLOBAL DEFAULT   12 arange_double
-    48: 0000000000011f80    75 FUNC    GLOBAL DEFAULT   12 max_idxf
-    49: 0000000000011e80   169 FUNC    GLOBAL DEFAULT   12 trapz_const_deltaf
+    47: 0000000000011990   261 FUNC    GLOBAL DEFAULT   12 arange_double
+    48: 0000000000011f40    75 FUNC    GLOBAL DEFAULT   12 max_idxf
+    49: 0000000000011e40   169 FUNC    GLOBAL DEFAULT   12 trapz_const_deltaf
     50: 0000000000006fc0  3969 FUNC    GLOBAL DEFAULT   12 rf_volt_compf
-    51: 00000000000110d0    81 FUNC    GLOBAL DEFAULT   12 fast_expvf
-    52: 000000000000fdf0   125 FUNC    GLOBAL DEFAULT   12 add_int_vector_inplace
-    53: 0000000000011b90   178 FUNC    GLOBAL DEFAULT   12 cumtrapz_w_initialf
-    54: 0000000000015be0   591 FUNC    GLOBAL DEFAULT   12 generate_distribution
-    55: 00000000000122d0   145 FUNC    GLOBAL DEFAULT   12 sum
-    56: 00000000000142f0   451 FUNC    WEAK   DEFAULT   12 _ZSt16__introsort_loopIPllN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIlEEEEvT_S7_T0_T1_
-    57: 0000000000010070   149 FUNC    GLOBAL DEFAULT   12 add_float_vector_inplace
-    58: 0000000000015bb0     3 FUNC    GLOBAL DEFAULT   12 _Z18omp_get_thread_numv
-    59: 000000000000fc00   141 FUNC    GLOBAL DEFAULT   12 add_uint32_vector
-    60: 000000000000fd50   149 FUNC    GLOBAL DEFAULT   12 add_float_vector
-    61: 000000000000fa90   141 FUNC    GLOBAL DEFAULT   12 add_int_vector
-    62: 000000000000e2b0   328 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorI8particleIdESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
+    51: 0000000000011090    81 FUNC    GLOBAL DEFAULT   12 fast_expvf
+    52: 000000000000fdb0   125 FUNC    GLOBAL DEFAULT   12 add_int_vector_inplace
+    53: 0000000000011b50   178 FUNC    GLOBAL DEFAULT   12 cumtrapz_w_initialf
+    54: 0000000000015ba0   591 FUNC    GLOBAL DEFAULT   12 generate_distribution
+    55: 0000000000012290   145 FUNC    GLOBAL DEFAULT   12 sum
+    56: 00000000000142b0   451 FUNC    WEAK   DEFAULT   12 _ZSt16__introsort_loopIPllN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIlEEEEvT_S7_T0_T1_
+    57: 0000000000010030   149 FUNC    GLOBAL DEFAULT   12 add_float_vector_inplace
+    58: 0000000000015b70     3 FUNC    GLOBAL DEFAULT   12 _Z18omp_get_thread_numv
+    59: 000000000000fbc0   141 FUNC    GLOBAL DEFAULT   12 add_uint32_vector
+    60: 000000000000fd10   149 FUNC    GLOBAL DEFAULT   12 add_float_vector
+    61: 000000000000fa50   141 FUNC    GLOBAL DEFAULT   12 add_int_vector
+    62: 000000000000e270   328 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorI8particleIdESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
     63: 0000000000005f80  4150 FUNC    GLOBAL DEFAULT   12 kickf
-    64: 0000000000010a50   290 FUNC    GLOBAL DEFAULT   12 fast_cos
-    65: 000000000000e1f0   188 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorI8particleIfESaIS1_EE7reserveEm
-    66: 0000000000011530   170 FUNC    GLOBAL DEFAULT   12 cumtrapz_wo_initial
-    67: 0000000000011010    81 FUNC    GLOBAL DEFAULT   12 fast_sinvf
-    68: 0000000000011c50   554 FUNC    GLOBAL DEFAULT   12 trapz_var_deltaf
-    69: 00000000000121e0   229 FUNC    GLOBAL DEFAULT   12 arange_int
-    70: 000000000000f3b0   529 FUNC    GLOBAL DEFAULT   12 where_less_thanf
-    71: 00000000000129a0   408 FUNC    GLOBAL DEFAULT   12 vector_mul_complex64
-    72: 0000000000011230   242 FUNC    GLOBAL DEFAULT   12 interpf
-    73: 000000000000e130   188 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorI8particleIdESaIS1_EE7reserveEm
-    74: 00000000000127b0   181 FUNC    GLOBAL DEFAULT   12 vector_mul_int32
-    75: 0000000000016ff0   705 FUNC    GLOBAL DEFAULT   12 sparse_histogramf
-    76: 0000000000011750   194 FUNC    GLOBAL DEFAULT   12 trapz_const_delta
+    64: 0000000000010a10   290 FUNC    GLOBAL DEFAULT   12 fast_cos
+    65: 000000000000e1b0   188 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorI8particleIfESaIS1_EE7reserveEm
+    66: 00000000000114f0   170 FUNC    GLOBAL DEFAULT   12 cumtrapz_wo_initial
+    67: 0000000000010fd0    81 FUNC    GLOBAL DEFAULT   12 fast_sinvf
+    68: 0000000000011c10   554 FUNC    GLOBAL DEFAULT   12 trapz_var_deltaf
+    69: 00000000000121a0   229 FUNC    GLOBAL DEFAULT   12 arange_int
+    70: 000000000000f370   529 FUNC    GLOBAL DEFAULT   12 where_less_thanf
+    71: 0000000000012960   408 FUNC    GLOBAL DEFAULT   12 vector_mul_complex64
+    72: 00000000000111f0   242 FUNC    GLOBAL DEFAULT   12 interpf
+    73: 000000000000e0f0   188 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorI8particleIdESaIS1_EE7reserveEm
+    74: 0000000000012770   181 FUNC    GLOBAL DEFAULT   12 vector_mul_int32
+    75: 0000000000016fb0   705 FUNC    GLOBAL DEFAULT   12 sparse_histogramf
+    76: 0000000000011710   194 FUNC    GLOBAL DEFAULT   12 trapz_const_delta
     77: 0000000000009650  1176 FUNC    GLOBAL DEFAULT   12 linear_interp_kickf
-    78: 00000000000115e0   178 FUNC    GLOBAL DEFAULT   12 cumtrapz_w_initial
-    79: 00000000000161f0    14 FUNC    GLOBAL DEFAULT   12 set_random_seed
-    80: 0000000000012870    39 FUNC    GLOBAL DEFAULT   12 vector_mul_int64
-    81: 0000000000015e30   448 FUNC    GLOBAL DEFAULT   12 synchrotron_radiation
-    82: 00000000000144c0  1932 FUNC    GLOBAL DEFAULT   12 fast_resonator_real_imag
-    83: 00000000000118c0   261 FUNC    GLOBAL DEFAULT   12 linspace
-    84: 00000000000135d0   834 FUNC    GLOBAL DEFAULT   12 sort_longint
-    85: 00000000000124f0   141 FUNC    GLOBAL DEFAULT   12 scalar_mul_float32
-    86: 0000000000010010    93 FUNC    GLOBAL DEFAULT   12 add_double_vector_inplace
-    87: 0000000000012f40   893 FUNC    GLOBAL DEFAULT   12 sort_float
-    88: 0000000000010c70   216 FUNC    GLOBAL DEFAULT   12 fast_sinf
-    89: 0000000000015bc0    30 FUNC    GLOBAL DEFAULT   12 _Z5randdv
-    90: 0000000000009c80  2809 FUNC    GLOBAL DEFAULT   12 histogram
-    91: 0000000000012370   137 FUNC    GLOBAL DEFAULT   12 sumf
-    92: 000000000000f940    71 FUNC    GLOBAL DEFAULT   12 where
-    93: 000000000000ffb0    85 FUNC    GLOBAL DEFAULT   12 add_longint_vector_inplace
-    94: 0000000000016200  1254 FUNC    GLOBAL DEFAULT   12 synchrotron_radiation_full
-    95: 0000000000012580    85 FUNC    GLOBAL DEFAULT   12 scalar_mul_float64
-    96: 000000000000b420   637 FUNC    GLOBAL DEFAULT   12 smooth_histogramf
+    78: 00000000000115a0   178 FUNC    GLOBAL DEFAULT   12 cumtrapz_w_initial
+    79: 00000000000161b0    14 FUNC    GLOBAL DEFAULT   12 set_random_seed
+    80: 0000000000012830    39 FUNC    GLOBAL DEFAULT   12 vector_mul_int64
+    81: 0000000000015df0   448 FUNC    GLOBAL DEFAULT   12 synchrotron_radiation
+    82: 0000000000014480  1932 FUNC    GLOBAL DEFAULT   12 fast_resonator_real_imag
+    83: 0000000000011880   261 FUNC    GLOBAL DEFAULT   12 linspace
+    84: 0000000000013590   834 FUNC    GLOBAL DEFAULT   12 sort_longint
+    85: 00000000000124b0   141 FUNC    GLOBAL DEFAULT   12 scalar_mul_float32
+    86: 000000000000ffd0    93 FUNC    GLOBAL DEFAULT   12 add_double_vector_inplace
+    87: 0000000000012f00   893 FUNC    GLOBAL DEFAULT   12 sort_float
+    88: 0000000000010c30   216 FUNC    GLOBAL DEFAULT   12 fast_sinf
+    89: 0000000000015b80    30 FUNC    GLOBAL DEFAULT   12 _Z5randdv
+    90: 0000000000009c80  2774 FUNC    GLOBAL DEFAULT   12 histogram
+    91: 0000000000012330   137 FUNC    GLOBAL DEFAULT   12 sumf
+    92: 000000000000f900    71 FUNC    GLOBAL DEFAULT   12 where
+    93: 000000000000ff70    85 FUNC    GLOBAL DEFAULT   12 add_longint_vector_inplace
+    94: 00000000000161c0  1254 FUNC    GLOBAL DEFAULT   12 synchrotron_radiation_full
+    95: 0000000000012540    85 FUNC    GLOBAL DEFAULT   12 scalar_mul_float64
+    96: 000000000000b3e0   637 FUNC    GLOBAL DEFAULT   12 smooth_histogramf
     97: 0000000000007f50  1467 FUNC    GLOBAL DEFAULT   12 drift
-    98: 0000000000011130   242 FUNC    GLOBAL DEFAULT   12 interp
-    99: 000000000000a780   589 FUNC    GLOBAL DEFAULT   12 smooth_histogram
-   100: 0000000000011070    81 FUNC    GLOBAL DEFAULT   12 fast_cosvf
-   101: 0000000000013dc0   443 FUNC    WEAK   DEFAULT   12 _ZSt16__introsort_loopIPdlN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIdEEEEvT_S7_T0_T1_
+    98: 00000000000110f0   242 FUNC    GLOBAL DEFAULT   12 interp
+    99: 000000000000a760   589 FUNC    GLOBAL DEFAULT   12 smooth_histogram
+   100: 0000000000011030    81 FUNC    GLOBAL DEFAULT   12 fast_cosvf
+   101: 0000000000013d80   443 FUNC    WEAK   DEFAULT   12 _ZSt16__introsort_loopIPdlN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIdEEEEvT_S7_T0_T1_
    102: 0000000000003460  5579 FUNC    GLOBAL DEFAULT   12 kick
-   103: 000000000000fb20   219 FUNC    GLOBAL DEFAULT   12 add_uint16_vector
-   104: 000000000000f120    35 FUNC    GLOBAL DEFAULT   12 where_less_than
-   105: 0000000000010820   238 FUNC    GLOBAL DEFAULT   12 stdevf
-   106: 000000000000bd70  2530 FUNC    GLOBAL DEFAULT   12 music_track_multiturn
-   107: 0000000000015b90     6 FUNC    GLOBAL DEFAULT   12 _Z19omp_get_max_threadsv
-   108: 000000000000fcf0    93 FUNC    GLOBAL DEFAULT   12 add_double_vector
-   109: 00000000000128a0   149 FUNC    GLOBAL DEFAULT   12 vector_mul_float32
-   110: 0000000000016d20   709 FUNC    GLOBAL DEFAULT   12 sparse_histogram
-   111: 000000000000a9d0  2635 FUNC    GLOBAL DEFAULT   12 histogramf
-   112: 000000000000f0f0    35 FUNC    GLOBAL DEFAULT   12 where_more_than
-   113: 0000000000011870    75 FUNC    GLOBAL DEFAULT   12 max_idx
-   114: 0000000000010ef0    81 FUNC    GLOBAL DEFAULT   12 fast_sinv
-   115: 0000000000012940    93 FUNC    GLOBAL DEFAULT   12 vector_mul_float64
-   116: 0000000000012b40    82 FUNC    GLOBAL DEFAULT   12 vector_mul_complex128
-   117: 00000000000116a0   176 FUNC    GLOBAL DEFAULT   12 trapz_var_delta
-   118: 0000000000011fd0   229 FUNC    GLOBAL DEFAULT   12 linspacef
-   119: 000000000000f5d0   873 FUNC    GLOBAL DEFAULT   12 where_more_less_thanf
-   120: 0000000000011430   247 FUNC    GLOBAL DEFAULT   12 interp_const_spacef
-   121: 0000000000015ba0     6 FUNC    GLOBAL DEFAULT   12 _Z19omp_get_num_threadsv
-   122: 0000000000014130   434 FUNC    WEAK   DEFAULT   12 _ZSt16__introsort_loopIPilN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIiEEEEvT_S7_T0_T1_
-   123: 0000000000010b80   239 FUNC    GLOBAL DEFAULT   12 fast_exp
-   124: 0000000000010e10   224 FUNC    GLOBAL DEFAULT   12 fast_expf
-   125: 0000000000010d50   190 FUNC    GLOBAL DEFAULT   12 fast_cosf
+   103: 000000000000fae0   219 FUNC    GLOBAL DEFAULT   12 add_uint16_vector
+   104: 000000000000f0e0    35 FUNC    GLOBAL DEFAULT   12 where_less_than
+   105: 00000000000107e0   238 FUNC    GLOBAL DEFAULT   12 stdevf
+   106: 000000000000bd30  2530 FUNC    GLOBAL DEFAULT   12 music_track_multiturn
+   107: 0000000000015b50     6 FUNC    GLOBAL DEFAULT   12 _Z19omp_get_max_threadsv
+   108: 000000000000fcb0    93 FUNC    GLOBAL DEFAULT   12 add_double_vector
+   109: 0000000000012860   149 FUNC    GLOBAL DEFAULT   12 vector_mul_float32
+   110: 0000000000016ce0   709 FUNC    GLOBAL DEFAULT   12 sparse_histogram
+   111: 000000000000a9b0  2603 FUNC    GLOBAL DEFAULT   12 histogramf
+   112: 000000000000f0b0    35 FUNC    GLOBAL DEFAULT   12 where_more_than
+   113: 0000000000011830    75 FUNC    GLOBAL DEFAULT   12 max_idx
+   114: 0000000000010eb0    81 FUNC    GLOBAL DEFAULT   12 fast_sinv
+   115: 0000000000012900    93 FUNC    GLOBAL DEFAULT   12 vector_mul_float64
+   116: 0000000000012b00    82 FUNC    GLOBAL DEFAULT   12 vector_mul_complex128
+   117: 0000000000011660   176 FUNC    GLOBAL DEFAULT   12 trapz_var_delta
+   118: 0000000000011f90   229 FUNC    GLOBAL DEFAULT   12 linspacef
+   119: 000000000000f590   873 FUNC    GLOBAL DEFAULT   12 where_more_less_thanf
+   120: 00000000000113f0   247 FUNC    GLOBAL DEFAULT   12 interp_const_spacef
+   121: 0000000000015b60     6 FUNC    GLOBAL DEFAULT   12 _Z19omp_get_num_threadsv
+   122: 00000000000140f0   434 FUNC    WEAK   DEFAULT   12 _ZSt16__introsort_loopIPilN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIiEEEEvT_S7_T0_T1_
+   123: 0000000000010b40   239 FUNC    GLOBAL DEFAULT   12 fast_exp
+   124: 0000000000010dd0   224 FUNC    GLOBAL DEFAULT   12 fast_expf
+   125: 0000000000010d10   190 FUNC    GLOBAL DEFAULT   12 fast_cosf
    126: 0000000000009af0   395 FUNC    GLOBAL DEFAULT   12 linear_interp_time_translationf
-   127: 000000000000ff30   125 FUNC    GLOBAL DEFAULT   12 add_uint32_vector_inplace
-   128: 0000000000015750   382 FUNC    GLOBAL DEFAULT   12 beam_phase
-   129: 0000000000011ae0   170 FUNC    GLOBAL DEFAULT   12 cumtrapz_wo_initialf
-   130: 00000000000125e0   368 FUNC    GLOBAL DEFAULT   12 scalar_mul_complex64
-   131: 0000000000010910   305 FUNC    GLOBAL DEFAULT   12 fast_sin
-   132: 0000000000014c50  2804 FUNC    GLOBAL DEFAULT   12 fast_resonator_real_imagf
-   133: 00000000000132c0   774 FUNC    GLOBAL DEFAULT   12 sort_int
-   134: 00000000000120c0   277 FUNC    GLOBAL DEFAULT   12 arange_float
-   135: 0000000000015ff0   506 FUNC    GLOBAL DEFAULT   12 synchrotron_radiationf
+   127: 000000000000fef0   125 FUNC    GLOBAL DEFAULT   12 add_uint32_vector_inplace
+   128: 0000000000015710   382 FUNC    GLOBAL DEFAULT   12 beam_phase
+   129: 0000000000011aa0   170 FUNC    GLOBAL DEFAULT   12 cumtrapz_wo_initialf
+   130: 00000000000125a0   368 FUNC    GLOBAL DEFAULT   12 scalar_mul_complex64
+   131: 00000000000108d0   305 FUNC    GLOBAL DEFAULT   12 fast_sin
+   132: 0000000000014c10  2804 FUNC    GLOBAL DEFAULT   12 fast_resonator_real_imagf
+   133: 0000000000013280   774 FUNC    GLOBAL DEFAULT   12 sort_int
+   134: 0000000000012080   277 FUNC    GLOBAL DEFAULT   12 arange_float
+   135: 0000000000015fb0   506 FUNC    GLOBAL DEFAULT   12 synchrotron_radiationf
    136: 0000000000004a30  5446 FUNC    GLOBAL DEFAULT   12 rf_volt_comp
-   137: 000000000000f150    51 FUNC    GLOBAL DEFAULT   12 where_more_less_than
-   138: 00000000000158d0   308 FUNC    GLOBAL DEFAULT   12 beam_phase_fast
-   139: 00000000000166f0  1320 FUNC    GLOBAL DEFAULT   12 synchrotron_radiation_fullf
-   140: 0000000000012750    92 FUNC    GLOBAL DEFAULT   12 scalar_mul_complex128
-   141: 0000000000011330   247 FUNC    GLOBAL DEFAULT   12 interp_const_space
-   142: 0000000000010690   214 FUNC    GLOBAL DEFAULT   12 stdev
-   143: 0000000000012400   181 FUNC    GLOBAL DEFAULT   12 scalar_mul_int32
-   144: 0000000000010770   169 FUNC    GLOBAL DEFAULT   12 meanf
-   145: 0000000000010320   685 FUNC    GLOBAL DEFAULT   12 convolutionf
+   137: 000000000000f110    51 FUNC    GLOBAL DEFAULT   12 where_more_less_than
+   138: 0000000000015890   308 FUNC    GLOBAL DEFAULT   12 beam_phase_fast
+   139: 00000000000166b0  1320 FUNC    GLOBAL DEFAULT   12 synchrotron_radiation_fullf
+   140: 0000000000012710    92 FUNC    GLOBAL DEFAULT   12 scalar_mul_complex128
+   141: 00000000000112f0   247 FUNC    GLOBAL DEFAULT   12 interp_const_space
+   142: 0000000000010650   214 FUNC    GLOBAL DEFAULT   12 stdev
+   143: 00000000000123c0   181 FUNC    GLOBAL DEFAULT   12 scalar_mul_int32
+   144: 0000000000010730   169 FUNC    GLOBAL DEFAULT   12 meanf
+   145: 00000000000102e0   685 FUNC    GLOBAL DEFAULT   12 convolutionf
    146: 0000000000009540   261 FUNC    GLOBAL DEFAULT   12 linear_interp_time_translation
 
 Symbol table '.symtab' contains 246 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000270     0 SECTION LOCAL  DEFAULT    1 .note.gnu.build-id
      2: 0000000000000298     0 SECTION LOCAL  DEFAULT    2 .gnu.hash
@@ -160,19 +160,19 @@
      6: 0000000000002190     0 SECTION LOCAL  DEFAULT    6 .gnu.version_r
      7: 0000000000002260     0 SECTION LOCAL  DEFAULT    7 .rela.dyn
      8: 0000000000002398     0 SECTION LOCAL  DEFAULT    8 .rela.plt
      9: 0000000000003000     0 SECTION LOCAL  DEFAULT    9 .init
     10: 0000000000003020     0 SECTION LOCAL  DEFAULT   10 .plt
     11: 00000000000032c0     0 SECTION LOCAL  DEFAULT   11 .plt.got
     12: 00000000000032d0     0 SECTION LOCAL  DEFAULT   12 .text
-    13: 00000000000172b4     0 SECTION LOCAL  DEFAULT   13 .fini
+    13: 0000000000017274     0 SECTION LOCAL  DEFAULT   13 .fini
     14: 0000000000018000     0 SECTION LOCAL  DEFAULT   14 .rodata
     15: 0000000000018480     0 SECTION LOCAL  DEFAULT   15 .eh_frame_hdr
     16: 0000000000018930     0 SECTION LOCAL  DEFAULT   16 .eh_frame
-    17: 000000000001a1f8     0 SECTION LOCAL  DEFAULT   17 .gcc_except_table
+    17: 000000000001a1f0     0 SECTION LOCAL  DEFAULT   17 .gcc_except_table
     18: 000000000001bda0     0 SECTION LOCAL  DEFAULT   18 .tbss
     19: 000000000001bda0     0 SECTION LOCAL  DEFAULT   19 .init_array
     20: 000000000001bdb8     0 SECTION LOCAL  DEFAULT   20 .fini_array
     21: 000000000001bdc0     0 SECTION LOCAL  DEFAULT   21 .dynamic
     22: 000000000001bfc0     0 SECTION LOCAL  DEFAULT   22 .got
     23: 000000000001c000     0 SECTION LOCAL  DEFAULT   23 .got.plt
     24: 000000000001c160     0 SECTION LOCAL  DEFAULT   24 .data
@@ -182,18 +182,18 @@
     28: 0000000000000000     0 SECTION LOCAL  DEFAULT   28 .debug_info
     29: 0000000000000000     0 SECTION LOCAL  DEFAULT   29 .debug_abbrev
     30: 0000000000000000     0 SECTION LOCAL  DEFAULT   30 .debug_line
     31: 0000000000000000     0 SECTION LOCAL  DEFAULT   31 .debug_str
     32: 0000000000000000     0 SECTION LOCAL  DEFAULT   32 .debug_loc
     33: 0000000000000000     0 SECTION LOCAL  DEFAULT   33 .debug_ranges
     34: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS music_track.cpp
-    35: 000000000000b6a0   321 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIN9__gnu_cxx17__normal_iteratorIP8particleIfESt6vectorIS3_SaIS3_EEEElS3_NS0_5__ops15_Iter_less_iterEEvT_T0_SC_T1_T2_.isra.0
-    36: 000000000000b7f0   348 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIN9__gnu_cxx17__normal_iteratorIP8particleIdESt6vectorIS3_SaIS3_EEEElS3_NS0_5__ops15_Iter_less_iterEEvT_T0_SC_T1_T2_.isra.0
-    37: 000000000000b950   512 FUNC    LOCAL  DEFAULT   12 _ZSt16__introsort_loopIN9__gnu_cxx17__normal_iteratorIP8particleIfESt6vectorIS3_SaIS3_EEEElNS0_5__ops15_Iter_less_iterEEvT_SB_T0_T1_.isra.0
-    38: 000000000000bb50   543 FUNC    LOCAL  DEFAULT   12 _ZSt16__introsort_loopIN9__gnu_cxx17__normal_iteratorIP8particleIdESt6vectorIS3_SaIS3_EEEElNS0_5__ops15_Iter_less_iterEEvT_SB_T0_T1_.isra.0
+    35: 000000000000b660   321 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIN9__gnu_cxx17__normal_iteratorIP8particleIfESt6vectorIS3_SaIS3_EEEElS3_NS0_5__ops15_Iter_less_iterEEvT_T0_SC_T1_T2_.isra.0
+    36: 000000000000b7b0   348 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIN9__gnu_cxx17__normal_iteratorIP8particleIdESt6vectorIS3_SaIS3_EEEElS3_NS0_5__ops15_Iter_less_iterEEvT_T0_SC_T1_T2_.isra.0
+    37: 000000000000b910   512 FUNC    LOCAL  DEFAULT   12 _ZSt16__introsort_loopIN9__gnu_cxx17__normal_iteratorIP8particleIfESt6vectorIS3_SaIS3_EEEElNS0_5__ops15_Iter_less_iterEEvT_SB_T0_T1_.isra.0
+    38: 000000000000bb10   543 FUNC    LOCAL  DEFAULT   12 _ZSt16__introsort_loopIN9__gnu_cxx17__normal_iteratorIP8particleIdESt6vectorIS3_SaIS3_EEEElNS0_5__ops15_Iter_less_iterEEvT_SB_T0_T1_.isra.0
     39: 00000000000032d0    26 FUNC    LOCAL  DEFAULT   12 music_track_multiturn.cold
     40: 00000000000032ea    26 FUNC    LOCAL  DEFAULT   12 music_track.cold
     41: 0000000000003304    23 FUNC    LOCAL  DEFAULT   12 music_track_multiturnf.cold
     42: 000000000000331b    23 FUNC    LOCAL  DEFAULT   12 music_trackf.cold
     43: 0000000000003350    46 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_music_track.cpp
     44: 000000000001c188     1 OBJECT  LOCAL  DEFAULT   25 _ZStL8__ioinit
     45: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS beam_phase.cpp
@@ -212,188 +212,188 @@
     58: 000000000001bda0     0 OBJECT  LOCAL  DEFAULT   19 __frame_dummy_init_array_entry
     59: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS kick.cpp
     60: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS drift.cpp
     61: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS linear_interp_kick.cpp
     62: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS histogram.cpp
     63: 000000000001c180     8 OBJECT  LOCAL  DEFAULT   25 _ZZ10histogramfE5histo
     64: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS blondmath.cpp
-    65: 000000000000e550   289 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIPlllN9__gnu_cxx5__ops15_Iter_less_iterEEvT_T0_S5_T1_T2_.isra.0
-    66: 0000000000013920   289 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIPlllN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIlEEEEvT_T0_S8_T1_T2_.isra.0
-    67: 000000000000e680   265 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIPiliN9__gnu_cxx5__ops15_Iter_less_iterEEvT_T0_S5_T1_T2_.isra.0
-    68: 0000000000013a50   265 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIPiliN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIiEEEEvT_T0_S8_T1_T2_.isra.0
-    69: 000000000000e790   296 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIPflfN9__gnu_cxx5__ops15_Iter_less_iterEEvT_T0_S5_T1_T2_.isra.0
-    70: 0000000000013b60   296 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIPflfN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIfEEEEvT_T0_S8_T1_T2_.isra.0
-    71: 000000000000e8c0   296 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIPdldN9__gnu_cxx5__ops15_Iter_less_iterEEvT_T0_S5_T1_T2_.isra.0
-    72: 0000000000013c90   296 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIPdldN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIdEEEEvT_T0_S8_T1_T2_.isra.0
-    73: 000000000000e9f0   451 FUNC    LOCAL  DEFAULT   12 _ZSt16__introsort_loopIPllN9__gnu_cxx5__ops15_Iter_less_iterEEvT_S4_T0_T1_.isra.0
-    74: 000000000000ebc0   434 FUNC    LOCAL  DEFAULT   12 _ZSt16__introsort_loopIPilN9__gnu_cxx5__ops15_Iter_less_iterEEvT_S4_T0_T1_.isra.0
-    75: 000000000000ed80   427 FUNC    LOCAL  DEFAULT   12 _ZSt16__introsort_loopIPflN9__gnu_cxx5__ops15_Iter_less_iterEEvT_S4_T0_T1_.isra.0
-    76: 000000000000ef30   443 FUNC    LOCAL  DEFAULT   12 _ZSt16__introsort_loopIPdlN9__gnu_cxx5__ops15_Iter_less_iterEEvT_S4_T0_T1_.isra.0
+    65: 000000000000e510   289 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIPlllN9__gnu_cxx5__ops15_Iter_less_iterEEvT_T0_S5_T1_T2_.isra.0
+    66: 00000000000138e0   289 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIPlllN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIlEEEEvT_T0_S8_T1_T2_.isra.0
+    67: 000000000000e640   265 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIPiliN9__gnu_cxx5__ops15_Iter_less_iterEEvT_T0_S5_T1_T2_.isra.0
+    68: 0000000000013a10   265 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIPiliN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIiEEEEvT_T0_S8_T1_T2_.isra.0
+    69: 000000000000e750   296 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIPflfN9__gnu_cxx5__ops15_Iter_less_iterEEvT_T0_S5_T1_T2_.isra.0
+    70: 0000000000013b20   296 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIPflfN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIfEEEEvT_T0_S8_T1_T2_.isra.0
+    71: 000000000000e880   296 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIPdldN9__gnu_cxx5__ops15_Iter_less_iterEEvT_T0_S5_T1_T2_.isra.0
+    72: 0000000000013c50   296 FUNC    LOCAL  DEFAULT   12 _ZSt13__adjust_heapIPdldN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIdEEEEvT_T0_S8_T1_T2_.isra.0
+    73: 000000000000e9b0   451 FUNC    LOCAL  DEFAULT   12 _ZSt16__introsort_loopIPllN9__gnu_cxx5__ops15_Iter_less_iterEEvT_S4_T0_T1_.isra.0
+    74: 000000000000eb80   434 FUNC    LOCAL  DEFAULT   12 _ZSt16__introsort_loopIPilN9__gnu_cxx5__ops15_Iter_less_iterEEvT_S4_T0_T1_.isra.0
+    75: 000000000000ed40   427 FUNC    LOCAL  DEFAULT   12 _ZSt16__introsort_loopIPflN9__gnu_cxx5__ops15_Iter_less_iterEEvT_S4_T0_T1_.isra.0
+    76: 000000000000eef0   443 FUNC    LOCAL  DEFAULT   12 _ZSt16__introsort_loopIPdlN9__gnu_cxx5__ops15_Iter_less_iterEEvT_S4_T0_T1_.isra.0
     77: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS fast_resonator.cpp
     78: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS fft.cpp
     79: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS openmp.cpp
     80: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tomoscope.cpp
     81: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS synchrotron_radiation.cpp
     82: 0000000000000060     8 TLS     LOCAL  DEFAULT   18 _ZZ26synchrotron_radiation_fullE3gen
     83: 0000000000000038     8 TLS     LOCAL  DEFAULT   18 _ZGVZ26synchrotron_radiation_fullE4dist
     84: 0000000000000040    32 TLS     LOCAL  DEFAULT   18 _ZZ26synchrotron_radiation_fullE4dist
     85: 0000000000000030     8 TLS     LOCAL  DEFAULT   18 _ZZ27synchrotron_radiation_fullfE3gen
     86: 0000000000000000     8 TLS     LOCAL  DEFAULT   18 _ZGVZ27synchrotron_radiation_fullfE4dist
     87: 0000000000000010    32 TLS     LOCAL  DEFAULT   18 _ZZ27synchrotron_radiation_fullfE4dist
     88: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS sparse_histogram.cpp
     89: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    90: 000000000001a1f4     0 OBJECT  LOCAL  DEFAULT   16 __FRAME_END__
+    90: 000000000001a1ec     0 OBJECT  LOCAL  DEFAULT   16 __FRAME_END__
     91: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
     92: 0000000000018480     0 NOTYPE  LOCAL  DEFAULT   15 __GNU_EH_FRAME_HDR
     93: 000000000001c160     0 OBJECT  LOCAL  DEFAULT   24 __dso_handle
     94: 000000000001c168     8 OBJECT  LOCAL  DEFAULT   24 DW.ref.__gxx_personality_v0
-    95: 00000000000172b4     0 FUNC    LOCAL  DEFAULT   13 _fini
+    95: 0000000000017274     0 FUNC    LOCAL  DEFAULT   13 _fini
     96: 0000000000003000     0 FUNC    LOCAL  DEFAULT    9 _init
     97: 000000000001bdc0     0 OBJECT  LOCAL  DEFAULT   21 _DYNAMIC
     98: 000000000001c178     0 OBJECT  LOCAL  DEFAULT   24 __TMC_END__
     99: 000000000001c000     0 OBJECT  LOCAL  DEFAULT   23 _GLOBAL_OFFSET_TABLE_
-   100: 0000000000011230   242 FUNC    GLOBAL DEFAULT   12 interpf
+   100: 00000000000111f0   242 FUNC    GLOBAL DEFAULT   12 interpf
    101: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _Znam@GLIBCXX_3.4
-   102: 0000000000010070   149 FUNC    GLOBAL DEFAULT   12 add_float_vector_inplace
-   103: 000000000000fcf0    93 FUNC    GLOBAL DEFAULT   12 add_double_vector
-   104: 0000000000015bb0     3 FUNC    GLOBAL DEFAULT   12 _Z18omp_get_thread_numv
-   105: 00000000000118c0   261 FUNC    GLOBAL DEFAULT   12 linspace
-   106: 000000000000c760  1914 FUNC    GLOBAL DEFAULT   12 music_track
-   107: 000000000000b420   637 FUNC    GLOBAL DEFAULT   12 smooth_histogramf
-   108: 000000000000fd50   149 FUNC    GLOBAL DEFAULT   12 add_float_vector
+   102: 0000000000010030   149 FUNC    GLOBAL DEFAULT   12 add_float_vector_inplace
+   103: 000000000000fcb0    93 FUNC    GLOBAL DEFAULT   12 add_double_vector
+   104: 0000000000015b70     3 FUNC    GLOBAL DEFAULT   12 _Z18omp_get_thread_numv
+   105: 0000000000011880   261 FUNC    GLOBAL DEFAULT   12 linspace
+   106: 000000000000c720  1914 FUNC    GLOBAL DEFAULT   12 music_track
+   107: 000000000000b3e0   637 FUNC    GLOBAL DEFAULT   12 smooth_histogramf
+   108: 000000000000fd10   149 FUNC    GLOBAL DEFAULT   12 add_float_vector
    109: 0000000000009650  1176 FUNC    GLOBAL DEFAULT   12 linear_interp_kickf
-   110: 0000000000010a50   290 FUNC    GLOBAL DEFAULT   12 fast_cos
-   111: 00000000000121e0   229 FUNC    GLOBAL DEFAULT   12 arange_int
+   110: 0000000000010a10   290 FUNC    GLOBAL DEFAULT   12 fast_cos
+   111: 00000000000121a0   229 FUNC    GLOBAL DEFAULT   12 arange_int
    112: 000000000001c170     8 OBJECT  GLOBAL DEFAULT   24 seed
    113: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND rand@GLIBC_2.2.5
-   114: 0000000000015bc0    30 FUNC    GLOBAL DEFAULT   12 _Z5randdv
-   115: 000000000000f940    71 FUNC    GLOBAL DEFAULT   12 where
+   114: 0000000000015b80    30 FUNC    GLOBAL DEFAULT   12 _Z5randdv
+   115: 000000000000f900    71 FUNC    GLOBAL DEFAULT   12 where
    116: 0000000000007f50  1467 FUNC    GLOBAL DEFAULT   12 drift
-   117: 0000000000012870    39 FUNC    GLOBAL DEFAULT   12 vector_mul_int64
-   118: 0000000000013f80   427 FUNC    WEAK   DEFAULT   12 _ZSt16__introsort_loopIPflN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIfEEEEvT_S7_T0_T1_
-   119: 00000000000135d0   834 FUNC    GLOBAL DEFAULT   12 sort_longint
-   120: 0000000000015ba0     6 FUNC    GLOBAL DEFAULT   12 _Z19omp_get_num_threadsv
-   121: 0000000000011010    81 FUNC    GLOBAL DEFAULT   12 fast_sinvf
-   122: 000000000000fc90    85 FUNC    GLOBAL DEFAULT   12 add_longint_vector
-   123: 000000000000e130   188 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorI8particleIdESaIS1_EE7reserveEm
+   117: 0000000000012830    39 FUNC    GLOBAL DEFAULT   12 vector_mul_int64
+   118: 0000000000013f40   427 FUNC    WEAK   DEFAULT   12 _ZSt16__introsort_loopIPflN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIfEEEEvT_S7_T0_T1_
+   119: 0000000000013590   834 FUNC    GLOBAL DEFAULT   12 sort_longint
+   120: 0000000000015b60     6 FUNC    GLOBAL DEFAULT   12 _Z19omp_get_num_threadsv
+   121: 0000000000010fd0    81 FUNC    GLOBAL DEFAULT   12 fast_sinvf
+   122: 000000000000fc50    85 FUNC    GLOBAL DEFAULT   12 add_longint_vector
+   123: 000000000000e0f0   188 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorI8particleIdESaIS1_EE7reserveEm
    124: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5
-   125: 00000000000128a0   149 FUNC    GLOBAL DEFAULT   12 vector_mul_float32
-   126: 0000000000015a10   377 FUNC    GLOBAL DEFAULT   12 beam_phasef
-   127: 000000000000f990   255 FUNC    GLOBAL DEFAULT   12 wheref
-   128: 000000000000f190   541 FUNC    GLOBAL DEFAULT   12 where_more_thanf
-   129: 000000000000e1f0   188 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorI8particleIfESaIS1_EE7reserveEm
-   130: 0000000000010d50   190 FUNC    GLOBAL DEFAULT   12 fast_cosf
+   125: 0000000000012860   149 FUNC    GLOBAL DEFAULT   12 vector_mul_float32
+   126: 00000000000159d0   377 FUNC    GLOBAL DEFAULT   12 beam_phasef
+   127: 000000000000f950   255 FUNC    GLOBAL DEFAULT   12 wheref
+   128: 000000000000f150   541 FUNC    GLOBAL DEFAULT   12 where_more_thanf
+   129: 000000000000e1b0   188 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorI8particleIfESaIS1_EE7reserveEm
+   130: 0000000000010d10   190 FUNC    GLOBAL DEFAULT   12 fast_cosf
    131: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt20__throw_length_errorPKc@GLIBCXX_3.4
-   132: 00000000000105d0   185 FUNC    GLOBAL DEFAULT   12 mean
+   132: 0000000000010590   185 FUNC    GLOBAL DEFAULT   12 mean
    133: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memset@GLIBC_2.2.5
-   134: 0000000000010f50    81 FUNC    GLOBAL DEFAULT   12 fast_cosv
-   135: 0000000000011f80    75 FUNC    GLOBAL DEFAULT   12 max_idxf
-   136: 00000000000129a0   408 FUNC    GLOBAL DEFAULT   12 vector_mul_complex64
-   137: 000000000000fdf0   125 FUNC    GLOBAL DEFAULT   12 add_int_vector_inplace
-   138: 00000000000120c0   277 FUNC    GLOBAL DEFAULT   12 arange_float
-   139: 0000000000011c50   554 FUNC    GLOBAL DEFAULT   12 trapz_var_deltaf
-   140: 0000000000011ae0   170 FUNC    GLOBAL DEFAULT   12 cumtrapz_wo_initialf
-   141: 0000000000012750    92 FUNC    GLOBAL DEFAULT   12 scalar_mul_complex128
-   142: 000000000000bd70  2530 FUNC    GLOBAL DEFAULT   12 music_track_multiturn
-   143: 00000000000125e0   368 FUNC    GLOBAL DEFAULT   12 scalar_mul_complex64
-   144: 0000000000011b90   178 FUNC    GLOBAL DEFAULT   12 cumtrapz_w_initialf
-   145: 00000000000115e0   178 FUNC    GLOBAL DEFAULT   12 cumtrapz_w_initial
+   134: 0000000000010f10    81 FUNC    GLOBAL DEFAULT   12 fast_cosv
+   135: 0000000000011f40    75 FUNC    GLOBAL DEFAULT   12 max_idxf
+   136: 0000000000012960   408 FUNC    GLOBAL DEFAULT   12 vector_mul_complex64
+   137: 000000000000fdb0   125 FUNC    GLOBAL DEFAULT   12 add_int_vector_inplace
+   138: 0000000000012080   277 FUNC    GLOBAL DEFAULT   12 arange_float
+   139: 0000000000011c10   554 FUNC    GLOBAL DEFAULT   12 trapz_var_deltaf
+   140: 0000000000011aa0   170 FUNC    GLOBAL DEFAULT   12 cumtrapz_wo_initialf
+   141: 0000000000012710    92 FUNC    GLOBAL DEFAULT   12 scalar_mul_complex128
+   142: 000000000000bd30  2530 FUNC    GLOBAL DEFAULT   12 music_track_multiturn
+   143: 00000000000125a0   368 FUNC    GLOBAL DEFAULT   12 scalar_mul_complex64
+   144: 0000000000011b50   178 FUNC    GLOBAL DEFAULT   12 cumtrapz_w_initialf
+   145: 00000000000115a0   178 FUNC    GLOBAL DEFAULT   12 cumtrapz_w_initial
    146: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND log@GLIBC_2.29
    147: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memcpy@GLIBC_2.14
-   148: 0000000000012940    93 FUNC    GLOBAL DEFAULT   12 vector_mul_float64
-   149: 0000000000011330   247 FUNC    GLOBAL DEFAULT   12 interp_const_space
-   150: 00000000000122d0   145 FUNC    GLOBAL DEFAULT   12 sum
+   148: 0000000000012900    93 FUNC    GLOBAL DEFAULT   12 vector_mul_float64
+   149: 00000000000112f0   247 FUNC    GLOBAL DEFAULT   12 interp_const_space
+   150: 0000000000012290   145 FUNC    GLOBAL DEFAULT   12 sum
    151: 0000000000009af0   395 FUNC    GLOBAL DEFAULT   12 linear_interp_time_translationf
-   152: 0000000000009c80  2809 FUNC    GLOBAL DEFAULT   12 histogram
-   153: 000000000000ffb0    85 FUNC    GLOBAL DEFAULT   12 add_longint_vector_inplace
+   152: 0000000000009c80  2774 FUNC    GLOBAL DEFAULT   12 histogram
+   153: 000000000000ff70    85 FUNC    GLOBAL DEFAULT   12 add_longint_vector_inplace
    154: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@GLIBC_2.2.5
-   155: 00000000000119d0   261 FUNC    GLOBAL DEFAULT   12 arange_double
-   156: 0000000000014c50  2804 FUNC    GLOBAL DEFAULT   12 fast_resonator_real_imagf
-   157: 0000000000011130   242 FUNC    GLOBAL DEFAULT   12 interp
-   158: 0000000000011820    75 FUNC    GLOBAL DEFAULT   12 min_idx
-   159: 0000000000015ff0   506 FUNC    GLOBAL DEFAULT   12 synchrotron_radiationf
-   160: 0000000000012b40    82 FUNC    GLOBAL DEFAULT   12 vector_mul_complex128
+   155: 0000000000011990   261 FUNC    GLOBAL DEFAULT   12 arange_double
+   156: 0000000000014c10  2804 FUNC    GLOBAL DEFAULT   12 fast_resonator_real_imagf
+   157: 00000000000110f0   242 FUNC    GLOBAL DEFAULT   12 interp
+   158: 00000000000117e0    75 FUNC    GLOBAL DEFAULT   12 min_idx
+   159: 0000000000015fb0   506 FUNC    GLOBAL DEFAULT   12 synchrotron_radiationf
+   160: 0000000000012b00    82 FUNC    GLOBAL DEFAULT   12 vector_mul_complex128
    161: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZdlPv@GLIBCXX_3.4
    162: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND srand@GLIBC_2.2.5
-   163: 0000000000014130   434 FUNC    WEAK   DEFAULT   12 _ZSt16__introsort_loopIPilN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIiEEEEvT_S7_T0_T1_
-   164: 0000000000012370   137 FUNC    GLOBAL DEFAULT   12 sumf
+   163: 00000000000140f0   434 FUNC    WEAK   DEFAULT   12 _ZSt16__introsort_loopIPilN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIiEEEEvT_S7_T0_T1_
+   164: 0000000000012330   137 FUNC    GLOBAL DEFAULT   12 sumf
    165: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _Znwm@GLIBCXX_3.4
-   166: 000000000000f0f0    35 FUNC    GLOBAL DEFAULT   12 where_more_than
-   167: 000000000000fb20   219 FUNC    GLOBAL DEFAULT   12 add_uint16_vector
-   168: 00000000000132c0   774 FUNC    GLOBAL DEFAULT   12 sort_int
-   169: 00000000000124c0    38 FUNC    GLOBAL DEFAULT   12 scalar_mul_int64
-   170: 00000000000158d0   308 FUNC    GLOBAL DEFAULT   12 beam_phase_fast
-   171: 000000000000f5d0   873 FUNC    GLOBAL DEFAULT   12 where_more_less_thanf
-   172: 0000000000011430   247 FUNC    GLOBAL DEFAULT   12 interp_const_spacef
-   173: 0000000000010010    93 FUNC    GLOBAL DEFAULT   12 add_double_vector_inplace
+   166: 000000000000f0b0    35 FUNC    GLOBAL DEFAULT   12 where_more_than
+   167: 000000000000fae0   219 FUNC    GLOBAL DEFAULT   12 add_uint16_vector
+   168: 0000000000013280   774 FUNC    GLOBAL DEFAULT   12 sort_int
+   169: 0000000000012480    38 FUNC    GLOBAL DEFAULT   12 scalar_mul_int64
+   170: 0000000000015890   308 FUNC    GLOBAL DEFAULT   12 beam_phase_fast
+   171: 000000000000f590   873 FUNC    GLOBAL DEFAULT   12 where_more_less_thanf
+   172: 00000000000113f0   247 FUNC    GLOBAL DEFAULT   12 interp_const_spacef
+   173: 000000000000ffd0    93 FUNC    GLOBAL DEFAULT   12 add_double_vector_inplace
    174: 0000000000006fc0  3969 FUNC    GLOBAL DEFAULT   12 rf_volt_compf
-   175: 000000000000f3b0   529 FUNC    GLOBAL DEFAULT   12 where_less_thanf
-   176: 000000000000f120    35 FUNC    GLOBAL DEFAULT   12 where_less_than
-   177: 0000000000011870    75 FUNC    GLOBAL DEFAULT   12 max_idx
-   178: 000000000000ff30   125 FUNC    GLOBAL DEFAULT   12 add_uint32_vector_inplace
-   179: 000000000000cee0  2671 FUNC    GLOBAL DEFAULT   12 music_track_multiturnf
-   180: 00000000000116a0   176 FUNC    GLOBAL DEFAULT   12 trapz_var_delta
-   181: 0000000000012400   181 FUNC    GLOBAL DEFAULT   12 scalar_mul_int32
-   182: 0000000000010b80   239 FUNC    GLOBAL DEFAULT   12 fast_exp
+   175: 000000000000f370   529 FUNC    GLOBAL DEFAULT   12 where_less_thanf
+   176: 000000000000f0e0    35 FUNC    GLOBAL DEFAULT   12 where_less_than
+   177: 0000000000011830    75 FUNC    GLOBAL DEFAULT   12 max_idx
+   178: 000000000000fef0   125 FUNC    GLOBAL DEFAULT   12 add_uint32_vector_inplace
+   179: 000000000000cea0  2671 FUNC    GLOBAL DEFAULT   12 music_track_multiturnf
+   180: 0000000000011660   176 FUNC    GLOBAL DEFAULT   12 trapz_var_delta
+   181: 00000000000123c0   181 FUNC    GLOBAL DEFAULT   12 scalar_mul_int32
+   182: 0000000000010b40   239 FUNC    GLOBAL DEFAULT   12 fast_exp
    183: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@GLIBC_2.2.5
-   184: 00000000000161f0    14 FUNC    GLOBAL DEFAULT   12 set_random_seed
-   185: 0000000000012580    85 FUNC    GLOBAL DEFAULT   12 scalar_mul_float64
-   186: 0000000000012f40   893 FUNC    GLOBAL DEFAULT   12 sort_float
-   187: 0000000000010690   214 FUNC    GLOBAL DEFAULT   12 stdev
+   184: 00000000000161b0    14 FUNC    GLOBAL DEFAULT   12 set_random_seed
+   185: 0000000000012540    85 FUNC    GLOBAL DEFAULT   12 scalar_mul_float64
+   186: 0000000000012f00   893 FUNC    GLOBAL DEFAULT   12 sort_float
+   187: 0000000000010650   214 FUNC    GLOBAL DEFAULT   12 stdev
    188: 0000000000009280   695 FUNC    GLOBAL DEFAULT   12 linear_interp_kick
-   189: 0000000000016200  1254 FUNC    GLOBAL DEFAULT   12 synchrotron_radiation_full
-   190: 00000000000127b0   181 FUNC    GLOBAL DEFAULT   12 vector_mul_int32
+   189: 00000000000161c0  1254 FUNC    GLOBAL DEFAULT   12 synchrotron_radiation_full
+   190: 0000000000012770   181 FUNC    GLOBAL DEFAULT   12 vector_mul_int32
    191: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZdaPv@GLIBCXX_3.4
-   192: 00000000000124f0   141 FUNC    GLOBAL DEFAULT   12 scalar_mul_float32
+   192: 00000000000124b0   141 FUNC    GLOBAL DEFAULT   12 scalar_mul_float32
    193: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@GLIBC_2.2.5
-   194: 000000000000a780   589 FUNC    GLOBAL DEFAULT   12 smooth_histogram
-   195: 0000000000016ff0   705 FUNC    GLOBAL DEFAULT   12 sparse_histogramf
+   194: 000000000000a760   589 FUNC    GLOBAL DEFAULT   12 smooth_histogram
+   195: 0000000000016fb0   705 FUNC    GLOBAL DEFAULT   12 sparse_histogramf
    196: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_throw_bad_array_new_length@CXXABI_1.3.8
-   197: 00000000000110d0    81 FUNC    GLOBAL DEFAULT   12 fast_expvf
-   198: 0000000000016d20   709 FUNC    GLOBAL DEFAULT   12 sparse_histogram
-   199: 0000000000015b90     6 FUNC    GLOBAL DEFAULT   12 _Z19omp_get_max_threadsv
+   197: 0000000000011090    81 FUNC    GLOBAL DEFAULT   12 fast_expvf
+   198: 0000000000016ce0   709 FUNC    GLOBAL DEFAULT   12 sparse_histogram
+   199: 0000000000015b50     6 FUNC    GLOBAL DEFAULT   12 _Z19omp_get_max_threadsv
    200: 0000000000004a30  5446 FUNC    GLOBAL DEFAULT   12 rf_volt_comp
    201: 0000000000009540   261 FUNC    GLOBAL DEFAULT   12 linear_interp_time_translation
-   202: 000000000000e2b0   328 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorI8particleIdESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
+   202: 000000000000e270   328 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorI8particleIdESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
    203: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt8ios_base4InitC1Ev@GLIBCXX_3.4
-   204: 0000000000010820   238 FUNC    GLOBAL DEFAULT   12 stdevf
-   205: 000000000000fe70   191 FUNC    GLOBAL DEFAULT   12 add_uint16_vector_inplace
-   206: 0000000000012ba0   926 FUNC    GLOBAL DEFAULT   12 sort_double
-   207: 00000000000144c0  1932 FUNC    GLOBAL DEFAULT   12 fast_resonator_real_imag
-   208: 0000000000011530   170 FUNC    GLOBAL DEFAULT   12 cumtrapz_wo_initial
-   209: 0000000000011070    81 FUNC    GLOBAL DEFAULT   12 fast_cosvf
-   210: 0000000000015750   382 FUNC    GLOBAL DEFAULT   12 beam_phase
+   204: 00000000000107e0   238 FUNC    GLOBAL DEFAULT   12 stdevf
+   205: 000000000000fe30   191 FUNC    GLOBAL DEFAULT   12 add_uint16_vector_inplace
+   206: 0000000000012b60   926 FUNC    GLOBAL DEFAULT   12 sort_double
+   207: 0000000000014480  1932 FUNC    GLOBAL DEFAULT   12 fast_resonator_real_imag
+   208: 00000000000114f0   170 FUNC    GLOBAL DEFAULT   12 cumtrapz_wo_initial
+   209: 0000000000011030    81 FUNC    GLOBAL DEFAULT   12 fast_cosvf
+   210: 0000000000015710   382 FUNC    GLOBAL DEFAULT   12 beam_phase
    211: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memmove@GLIBC_2.2.5
    212: 0000000000008510  3439 FUNC    GLOBAL DEFAULT   12 driftf
-   213: 0000000000010770   169 FUNC    GLOBAL DEFAULT   12 meanf
-   214: 0000000000010fb0    81 FUNC    GLOBAL DEFAULT   12 fast_expv
+   213: 0000000000010730   169 FUNC    GLOBAL DEFAULT   12 meanf
+   214: 0000000000010f70    81 FUNC    GLOBAL DEFAULT   12 fast_expv
    215: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __gxx_personality_v0@CXXABI_1.3
-   216: 000000000000e400   336 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorI8particleIfESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
-   217: 0000000000010910   305 FUNC    GLOBAL DEFAULT   12 fast_sin
-   218: 0000000000010e10   224 FUNC    GLOBAL DEFAULT   12 fast_expf
-   219: 000000000000fc00   141 FUNC    GLOBAL DEFAULT   12 add_uint32_vector
+   216: 000000000000e3c0   336 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorI8particleIfESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
+   217: 00000000000108d0   305 FUNC    GLOBAL DEFAULT   12 fast_sin
+   218: 0000000000010dd0   224 FUNC    GLOBAL DEFAULT   12 fast_expf
+   219: 000000000000fbc0   141 FUNC    GLOBAL DEFAULT   12 add_uint32_vector
    220: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __tls_get_addr@GLIBC_2.3
-   221: 0000000000013dc0   443 FUNC    WEAK   DEFAULT   12 _ZSt16__introsort_loopIPdlN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIdEEEEvT_S7_T0_T1_
+   221: 0000000000013d80   443 FUNC    WEAK   DEFAULT   12 _ZSt16__introsort_loopIPdlN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIdEEEEvT_S7_T0_T1_
    222: 0000000000003460  5579 FUNC    GLOBAL DEFAULT   12 kick
-   223: 000000000000a9d0  2635 FUNC    GLOBAL DEFAULT   12 histogramf
-   224: 000000000000fa90   141 FUNC    GLOBAL DEFAULT   12 add_int_vector
-   225: 0000000000010320   685 FUNC    GLOBAL DEFAULT   12 convolutionf
-   226: 000000000000f150    51 FUNC    GLOBAL DEFAULT   12 where_more_less_than
+   223: 000000000000a9b0  2603 FUNC    GLOBAL DEFAULT   12 histogramf
+   224: 000000000000fa50   141 FUNC    GLOBAL DEFAULT   12 add_int_vector
+   225: 00000000000102e0   685 FUNC    GLOBAL DEFAULT   12 convolutionf
+   226: 000000000000f110    51 FUNC    GLOBAL DEFAULT   12 where_more_less_than
    227: 0000000000005f80  4150 FUNC    GLOBAL DEFAULT   12 kickf
    228: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
    229: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _Unwind_Resume@GCC_3.0
-   230: 000000000000d950  2002 FUNC    GLOBAL DEFAULT   12 music_trackf
-   231: 0000000000016c20   256 FUNC    WEAK   DEFAULT   12 _ZNSt23mersenne_twister_engineImLm64ELm312ELm156ELm31ELm13043109905998158313ELm29ELm6148914691236517205ELm17ELm8202884508482404352ELm37ELm18444473444759240704ELm43ELm6364136223846793005EE11_M_gen_randEv
-   232: 0000000000011750   194 FUNC    GLOBAL DEFAULT   12 trapz_const_delta
-   233: 0000000000015e30   448 FUNC    GLOBAL DEFAULT   12 synchrotron_radiation
-   234: 0000000000015be0   591 FUNC    GLOBAL DEFAULT   12 generate_distribution
-   235: 0000000000010c70   216 FUNC    GLOBAL DEFAULT   12 fast_sinf
-   236: 0000000000011f30    75 FUNC    GLOBAL DEFAULT   12 min_idxf
-   237: 0000000000011fd0   229 FUNC    GLOBAL DEFAULT   12 linspacef
-   238: 00000000000142f0   451 FUNC    WEAK   DEFAULT   12 _ZSt16__introsort_loopIPllN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIlEEEEvT_S7_T0_T1_
-   239: 0000000000011e80   169 FUNC    GLOBAL DEFAULT   12 trapz_const_deltaf
+   230: 000000000000d910  2002 FUNC    GLOBAL DEFAULT   12 music_trackf
+   231: 0000000000016be0   256 FUNC    WEAK   DEFAULT   12 _ZNSt23mersenne_twister_engineImLm64ELm312ELm156ELm31ELm13043109905998158313ELm29ELm6148914691236517205ELm17ELm8202884508482404352ELm37ELm18444473444759240704ELm43ELm6364136223846793005EE11_M_gen_randEv
+   232: 0000000000011710   194 FUNC    GLOBAL DEFAULT   12 trapz_const_delta
+   233: 0000000000015df0   448 FUNC    GLOBAL DEFAULT   12 synchrotron_radiation
+   234: 0000000000015ba0   591 FUNC    GLOBAL DEFAULT   12 generate_distribution
+   235: 0000000000010c30   216 FUNC    GLOBAL DEFAULT   12 fast_sinf
+   236: 0000000000011ef0    75 FUNC    GLOBAL DEFAULT   12 min_idxf
+   237: 0000000000011f90   229 FUNC    GLOBAL DEFAULT   12 linspacef
+   238: 00000000000142b0   451 FUNC    WEAK   DEFAULT   12 _ZSt16__introsort_loopIPllN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIlEEEEvT_S7_T0_T1_
+   239: 0000000000011e40   169 FUNC    GLOBAL DEFAULT   12 trapz_const_deltaf
    240: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
    241: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-   242: 0000000000010ef0    81 FUNC    GLOBAL DEFAULT   12 fast_sinv
-   243: 0000000000010110   522 FUNC    GLOBAL DEFAULT   12 convolution
-   244: 00000000000166f0  1320 FUNC    GLOBAL DEFAULT   12 synchrotron_radiation_fullf
+   242: 0000000000010eb0    81 FUNC    GLOBAL DEFAULT   12 fast_sinv
+   243: 00000000000100d0   522 FUNC    GLOBAL DEFAULT   12 convolution
+   244: 00000000000166b0  1320 FUNC    GLOBAL DEFAULT   12 synchrotron_radiation_fullf
    245: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt8ios_base4InitD1Ev@GLIBCXX_3.4
```

#### readelf --wide --relocs {}

```diff
@@ -14,47 +14,47 @@
 000000000001bff0  0000001700000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
 000000000001bff8  0000001800000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSt8ios_base4InitD1Ev@GLIBCXX_3.4 + 0
 000000000001c168  0000001200000001 R_X86_64_64            0000000000000000 __gxx_personality_v0@CXXABI_1.3 + 0
 
 Relocation section '.rela.plt' at offset 0x2398 contains 41 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 000000000001c018  0000000100000007 R_X86_64_JUMP_SLOT     0000000000000000 _Znam@GLIBCXX_3.4 + 0
-000000000001c020  0000003a00000007 R_X86_64_JUMP_SLOT     0000000000015bb0 _Z18omp_get_thread_numv + 0
-000000000001c028  0000004000000007 R_X86_64_JUMP_SLOT     0000000000010a50 fast_cos + 0
+000000000001c020  0000003a00000007 R_X86_64_JUMP_SLOT     0000000000015b70 _Z18omp_get_thread_numv + 0
+000000000001c028  0000004000000007 R_X86_64_JUMP_SLOT     0000000000010a10 fast_cos + 0
 000000000001c030  0000000200000007 R_X86_64_JUMP_SLOT     0000000000000000 rand@GLIBC_2.2.5 + 0
-000000000001c038  0000005900000007 R_X86_64_JUMP_SLOT     0000000000015bc0 _Z5randdv + 0
-000000000001c040  0000002000000007 R_X86_64_JUMP_SLOT     0000000000013f80 _ZSt16__introsort_loopIPflN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIfEEEEvT_S7_T0_T1_ + 0
-000000000001c048  0000007900000007 R_X86_64_JUMP_SLOT     0000000000015ba0 _Z19omp_get_num_threadsv + 0
-000000000001c050  0000004900000007 R_X86_64_JUMP_SLOT     000000000000e130 _ZNSt6vectorI8particleIdESaIS1_EE7reserveEm + 0
-000000000001c058  0000004100000007 R_X86_64_JUMP_SLOT     000000000000e1f0 _ZNSt6vectorI8particleIfESaIS1_EE7reserveEm + 0
-000000000001c060  0000007d00000007 R_X86_64_JUMP_SLOT     0000000000010d50 fast_cosf + 0
+000000000001c038  0000005900000007 R_X86_64_JUMP_SLOT     0000000000015b80 _Z5randdv + 0
+000000000001c040  0000002000000007 R_X86_64_JUMP_SLOT     0000000000013f40 _ZSt16__introsort_loopIPflN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIfEEEEvT_S7_T0_T1_ + 0
+000000000001c048  0000007900000007 R_X86_64_JUMP_SLOT     0000000000015b60 _Z19omp_get_num_threadsv + 0
+000000000001c050  0000004900000007 R_X86_64_JUMP_SLOT     000000000000e0f0 _ZNSt6vectorI8particleIdESaIS1_EE7reserveEm + 0
+000000000001c058  0000004100000007 R_X86_64_JUMP_SLOT     000000000000e1b0 _ZNSt6vectorI8particleIfESaIS1_EE7reserveEm + 0
+000000000001c060  0000007d00000007 R_X86_64_JUMP_SLOT     0000000000010d10 fast_cosf + 0
 000000000001c068  0000000400000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZSt20__throw_length_errorPKc@GLIBCXX_3.4 + 0
-000000000001c070  0000001e00000007 R_X86_64_JUMP_SLOT     00000000000105d0 mean + 0
+000000000001c070  0000001e00000007 R_X86_64_JUMP_SLOT     0000000000010590 mean + 0
 000000000001c078  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 memset@GLIBC_2.2.5 + 0
 000000000001c080  0000000600000007 R_X86_64_JUMP_SLOT     0000000000000000 log@GLIBC_2.29 + 0
 000000000001c088  0000000700000007 R_X86_64_JUMP_SLOT     0000000000000000 memcpy@GLIBC_2.14 + 0
 000000000001c090  0000000800000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_atexit@GLIBC_2.2.5 + 0
 000000000001c098  0000000900000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZdlPv@GLIBCXX_3.4 + 0
 000000000001c0a0  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000000000 srand@GLIBC_2.2.5 + 0
-000000000001c0a8  0000007a00000007 R_X86_64_JUMP_SLOT     0000000000014130 _ZSt16__introsort_loopIPilN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIiEEEEvT_S7_T0_T1_ + 0
+000000000001c0a8  0000007a00000007 R_X86_64_JUMP_SLOT     00000000000140f0 _ZSt16__introsort_loopIPilN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIiEEEEvT_S7_T0_T1_ + 0
 000000000001c0b0  0000000b00000007 R_X86_64_JUMP_SLOT     0000000000000000 _Znwm@GLIBCXX_3.4 + 0
-000000000001c0b8  0000007b00000007 R_X86_64_JUMP_SLOT     0000000000010b80 fast_exp + 0
+000000000001c0b8  0000007b00000007 R_X86_64_JUMP_SLOT     0000000000010b40 fast_exp + 0
 000000000001c0c0  0000000c00000007 R_X86_64_JUMP_SLOT     0000000000000000 free@GLIBC_2.2.5 + 0
 000000000001c0c8  0000000d00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZdaPv@GLIBCXX_3.4 + 0
 000000000001c0d0  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000000000 malloc@GLIBC_2.2.5 + 0
 000000000001c0d8  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_throw_bad_array_new_length@CXXABI_1.3.8 + 0
-000000000001c0e0  0000006b00000007 R_X86_64_JUMP_SLOT     0000000000015b90 _Z19omp_get_max_threadsv + 0
-000000000001c0e8  0000003e00000007 R_X86_64_JUMP_SLOT     000000000000e2b0 _ZNSt6vectorI8particleIdESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_ + 0
+000000000001c0e0  0000006b00000007 R_X86_64_JUMP_SLOT     0000000000015b50 _Z19omp_get_max_threadsv + 0
+000000000001c0e8  0000003e00000007 R_X86_64_JUMP_SLOT     000000000000e270 _ZNSt6vectorI8particleIdESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_ + 0
 000000000001c0f0  0000001000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt8ios_base4InitC1Ev@GLIBCXX_3.4 + 0
 000000000001c0f8  0000001100000007 R_X86_64_JUMP_SLOT     0000000000000000 memmove@GLIBC_2.2.5 + 0
-000000000001c100  0000009000000007 R_X86_64_JUMP_SLOT     0000000000010770 meanf + 0
-000000000001c108  0000002800000007 R_X86_64_JUMP_SLOT     000000000000e400 _ZNSt6vectorI8particleIfESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_ + 0
-000000000001c110  0000008300000007 R_X86_64_JUMP_SLOT     0000000000010910 fast_sin + 0
-000000000001c118  0000007c00000007 R_X86_64_JUMP_SLOT     0000000000010e10 fast_expf + 0
+000000000001c100  0000009000000007 R_X86_64_JUMP_SLOT     0000000000010730 meanf + 0
+000000000001c108  0000002800000007 R_X86_64_JUMP_SLOT     000000000000e3c0 _ZNSt6vectorI8particleIfESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_ + 0
+000000000001c110  0000008300000007 R_X86_64_JUMP_SLOT     00000000000108d0 fast_sin + 0
+000000000001c118  0000007c00000007 R_X86_64_JUMP_SLOT     0000000000010dd0 fast_expf + 0
 000000000001c120  0000001300000007 R_X86_64_JUMP_SLOT     0000000000000000 __tls_get_addr@GLIBC_2.3 + 0
-000000000001c128  0000006500000007 R_X86_64_JUMP_SLOT     0000000000013dc0 _ZSt16__introsort_loopIPdlN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIdEEEEvT_S7_T0_T1_ + 0
+000000000001c128  0000006500000007 R_X86_64_JUMP_SLOT     0000000000013d80 _ZSt16__introsort_loopIPdlN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIdEEEEvT_S7_T0_T1_ + 0
 000000000001c130  0000001500000007 R_X86_64_JUMP_SLOT     0000000000000000 _Unwind_Resume@GCC_3.0 + 0
-000000000001c138  0000002700000007 R_X86_64_JUMP_SLOT     0000000000016c20 _ZNSt23mersenne_twister_engineImLm64ELm312ELm156ELm31ELm13043109905998158313ELm29ELm6148914691236517205ELm17ELm8202884508482404352ELm37ELm18444473444759240704ELm43ELm6364136223846793005EE11_M_gen_randEv + 0
-000000000001c140  0000004c00000007 R_X86_64_JUMP_SLOT     0000000000011750 trapz_const_delta + 0
-000000000001c148  0000005800000007 R_X86_64_JUMP_SLOT     0000000000010c70 fast_sinf + 0
-000000000001c150  0000003800000007 R_X86_64_JUMP_SLOT     00000000000142f0 _ZSt16__introsort_loopIPllN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIlEEEEvT_S7_T0_T1_ + 0
-000000000001c158  0000003100000007 R_X86_64_JUMP_SLOT     0000000000011e80 trapz_const_deltaf + 0
+000000000001c138  0000002700000007 R_X86_64_JUMP_SLOT     0000000000016be0 _ZNSt23mersenne_twister_engineImLm64ELm312ELm156ELm31ELm13043109905998158313ELm29ELm6148914691236517205ELm17ELm8202884508482404352ELm37ELm18444473444759240704ELm43ELm6364136223846793005EE11_M_gen_randEv + 0
+000000000001c140  0000004c00000007 R_X86_64_JUMP_SLOT     0000000000011710 trapz_const_delta + 0
+000000000001c148  0000005800000007 R_X86_64_JUMP_SLOT     0000000000010c30 fast_sinf + 0
+000000000001c150  0000003800000007 R_X86_64_JUMP_SLOT     00000000000142b0 _ZSt16__introsort_loopIPllN9__gnu_cxx5__ops15_Iter_comp_iterISt7greaterIlEEEEvT_S7_T0_T1_ + 0
+000000000001c158  0000003100000007 R_X86_64_JUMP_SLOT     0000000000011e40 trapz_const_deltaf + 0
```

#### readelf --wide --dynamic {}

```diff
@@ -3,15 +3,15 @@
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libstdc++.so.6]
  0x0000000000000001 (NEEDED)             Shared library: [libm.so.6]
  0x0000000000000001 (NEEDED)             Shared library: [libgcc_s.so.1]
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
  0x0000000000000001 (NEEDED)             Shared library: [ld-linux-x86-64.so.2]
  0x000000000000000c (INIT)               0x3000
- 0x000000000000000d (FINI)               0x172b4
+ 0x000000000000000d (FINI)               0x17274
  0x0000000000000019 (INIT_ARRAY)         0x1bda0
  0x000000000000001b (INIT_ARRAYSZ)       24 (bytes)
  0x000000000000001a (FINI_ARRAY)         0x1bdb8
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x298
  0x0000000000000005 (STRTAB)             0x1460
  0x0000000000000006 (SYMTAB)             0x698
```

#### readelf --wide --notes {}

```diff
@@ -1,4 +1,4 @@
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 97387f7ebd9f1ab0cf267f3252710bddc3696fd2
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 30f032825074e2c1c08a3bd6e122235b1b61bbc4
```

#### readelf --wide --debug-dump=frames {}

```diff
@@ -361,15 +361,15 @@
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000002e8 0000000000000048 000002ec FDE cie=00000000 pc=0000000000009c80..000000000000a779
+000002e8 0000000000000048 000002ec FDE cie=00000000 pc=0000000000009c80..000000000000a756
   DW_CFA_advance_loc: 10 to 0000000000009c8a
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
   DW_CFA_advance_loc: 9 to 0000000000009c93
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_advance_loc: 5 to 0000000000009c98
@@ -380,2021 +380,2014 @@
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_advance_loc: 1 to 0000000000009c9b
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_advance_loc: 5 to 0000000000009ca0
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 9 to 0000000000009ca9
-  DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc2: 2750 to 000000000000a767
+  DW_CFA_advance_loc: 6 to 0000000000009ca6
+  DW_CFA_def_cfa_offset: 128
+  DW_CFA_advance_loc2: 2718 to 000000000000a744
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 000000000000a76b
+  DW_CFA_advance_loc: 4 to 000000000000a748
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 000000000000a76c
+  DW_CFA_advance_loc: 1 to 000000000000a749
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000a76e
+  DW_CFA_advance_loc: 2 to 000000000000a74b
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000a770
+  DW_CFA_advance_loc: 2 to 000000000000a74d
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000a772
+  DW_CFA_advance_loc: 2 to 000000000000a74f
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000a774
+  DW_CFA_advance_loc: 2 to 000000000000a751
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000334 0000000000000048 00000338 FDE cie=00000000 pc=000000000000a780..000000000000a9cd
-  DW_CFA_advance_loc: 2 to 000000000000a782
+00000334 0000000000000048 00000338 FDE cie=00000000 pc=000000000000a760..000000000000a9ad
+  DW_CFA_advance_loc: 2 to 000000000000a762
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 13 to 000000000000a78f
+  DW_CFA_advance_loc: 13 to 000000000000a76f
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 9 to 000000000000a798
+  DW_CFA_advance_loc: 9 to 000000000000a778
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 000000000000a79a
+  DW_CFA_advance_loc: 2 to 000000000000a77a
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000000a79b
+  DW_CFA_advance_loc: 1 to 000000000000a77b
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 000000000000a79c
+  DW_CFA_advance_loc: 1 to 000000000000a77c
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 11 to 000000000000a7a7
+  DW_CFA_advance_loc: 11 to 000000000000a787
   DW_CFA_def_cfa_offset: 128
-  DW_CFA_advance_loc2: 532 to 000000000000a9bb
+  DW_CFA_advance_loc2: 532 to 000000000000a99b
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 000000000000a9bf
+  DW_CFA_advance_loc: 4 to 000000000000a99f
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 000000000000a9c0
+  DW_CFA_advance_loc: 1 to 000000000000a9a0
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000a9c2
+  DW_CFA_advance_loc: 2 to 000000000000a9a2
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000a9c4
+  DW_CFA_advance_loc: 2 to 000000000000a9a4
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000a9c6
+  DW_CFA_advance_loc: 2 to 000000000000a9a6
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000a9c8
+  DW_CFA_advance_loc: 2 to 000000000000a9a8
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000380 000000000000004c 00000384 FDE cie=00000000 pc=000000000000a9d0..000000000000b41b
-  DW_CFA_advance_loc: 2 to 000000000000a9d2
+00000380 0000000000000048 00000384 FDE cie=00000000 pc=000000000000a9b0..000000000000b3db
+  DW_CFA_advance_loc: 2 to 000000000000a9b2
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 13 to 000000000000a9df
+  DW_CFA_advance_loc: 13 to 000000000000a9bf
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 5 to 000000000000a9e4
+  DW_CFA_advance_loc: 5 to 000000000000a9c4
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 000000000000a9e6
+  DW_CFA_advance_loc: 2 to 000000000000a9c6
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000000a9e7
+  DW_CFA_advance_loc: 1 to 000000000000a9c7
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 000000000000a9e8
+  DW_CFA_advance_loc: 1 to 000000000000a9c8
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 14 to 000000000000a9f6
-  DW_CFA_def_cfa_offset: 160
-  DW_CFA_advance_loc2: 2446 to 000000000000b384
+  DW_CFA_advance_loc: 14 to 000000000000a9d6
+  DW_CFA_def_cfa_offset: 96
+  DW_CFA_advance_loc2: 2414 to 000000000000b344
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 000000000000b385
+  DW_CFA_advance_loc: 1 to 000000000000b345
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 000000000000b386
+  DW_CFA_advance_loc: 1 to 000000000000b346
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000b388
+  DW_CFA_advance_loc: 2 to 000000000000b348
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000b38a
+  DW_CFA_advance_loc: 2 to 000000000000b34a
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000b38c
+  DW_CFA_advance_loc: 2 to 000000000000b34c
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000b38e
+  DW_CFA_advance_loc: 2 to 000000000000b34e
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000000000000b38f
+  DW_CFA_advance_loc: 1 to 000000000000b34f
   DW_CFA_restore_state
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
 
-000003d0 000000000000004c 000003d4 FDE cie=00000000 pc=000000000000b420..000000000000b69d
-  DW_CFA_advance_loc: 2 to 000000000000b422
+000003cc 0000000000000048 000003d0 FDE cie=00000000 pc=000000000000b3e0..000000000000b65d
+  DW_CFA_advance_loc: 2 to 000000000000b3e2
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 13 to 000000000000b42f
+  DW_CFA_advance_loc: 13 to 000000000000b3ef
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 12 to 000000000000b43b
+  DW_CFA_advance_loc: 12 to 000000000000b3fb
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 000000000000b43d
+  DW_CFA_advance_loc: 2 to 000000000000b3fd
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000000b43e
+  DW_CFA_advance_loc: 1 to 000000000000b3fe
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 000000000000b43f
+  DW_CFA_advance_loc: 1 to 000000000000b3ff
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 10 to 000000000000b449
+  DW_CFA_advance_loc: 10 to 000000000000b409
   DW_CFA_def_cfa_offset: 112
-  DW_CFA_advance_loc2: 578 to 000000000000b68b
+  DW_CFA_advance_loc2: 578 to 000000000000b64b
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 000000000000b68f
+  DW_CFA_advance_loc: 4 to 000000000000b64f
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 000000000000b690
+  DW_CFA_advance_loc: 1 to 000000000000b650
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000b692
+  DW_CFA_advance_loc: 2 to 000000000000b652
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000b694
+  DW_CFA_advance_loc: 2 to 000000000000b654
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000b696
+  DW_CFA_advance_loc: 2 to 000000000000b656
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000b698
+  DW_CFA_advance_loc: 2 to 000000000000b658
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
 
-00000420 0000000000000028 00000424 FDE cie=00000000 pc=000000000000b6a0..000000000000b7e1
-  DW_CFA_advance_loc: 5 to 000000000000b6a5
+00000418 0000000000000028 0000041c FDE cie=00000000 pc=000000000000b660..000000000000b7a1
+  DW_CFA_advance_loc: 5 to 000000000000b665
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 10 to 000000000000b6af
+  DW_CFA_advance_loc: 10 to 000000000000b66f
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r3 (rbx) at cfa-24
-  DW_CFA_advance_loc1: 213 to 000000000000b784
+  DW_CFA_advance_loc1: 213 to 000000000000b744
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 000000000000b785
+  DW_CFA_advance_loc: 1 to 000000000000b745
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 11 to 000000000000b790
+  DW_CFA_advance_loc: 11 to 000000000000b750
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 79 to 000000000000b7df
+  DW_CFA_advance_loc1: 79 to 000000000000b79f
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 000000000000b7e0
+  DW_CFA_advance_loc: 1 to 000000000000b7a0
   DW_CFA_def_cfa_offset: 8
 
-0000044c 0000000000000020 00000450 FDE cie=00000000 pc=000000000000b7f0..000000000000b94c
-  DW_CFA_advance_loc: 5 to 000000000000b7f5
+00000444 0000000000000020 00000448 FDE cie=00000000 pc=000000000000b7b0..000000000000b90c
+  DW_CFA_advance_loc: 5 to 000000000000b7b5
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r3 (rbx) at cfa-16
-  DW_CFA_advance_loc1: 243 to 000000000000b8e8
+  DW_CFA_advance_loc1: 243 to 000000000000b8a8
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 000000000000b8f0
+  DW_CFA_advance_loc: 8 to 000000000000b8b0
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 91 to 000000000000b94b
+  DW_CFA_advance_loc1: 91 to 000000000000b90b
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000470 0000000000000040 00000474 FDE cie=00000000 pc=000000000000b950..000000000000bb50
-  DW_CFA_advance_loc: 20 to 000000000000b964
+00000468 0000000000000040 0000046c FDE cie=00000000 pc=000000000000b910..000000000000bb10
+  DW_CFA_advance_loc: 20 to 000000000000b924
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 5 to 000000000000b969
+  DW_CFA_advance_loc: 5 to 000000000000b929
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 2 to 000000000000b96b
+  DW_CFA_advance_loc: 2 to 000000000000b92b
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 4 to 000000000000b96f
+  DW_CFA_advance_loc: 4 to 000000000000b92f
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 4 to 000000000000b973
+  DW_CFA_advance_loc: 4 to 000000000000b933
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc2: 468 to 000000000000bb47
+  DW_CFA_advance_loc2: 468 to 000000000000bb07
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 000000000000bb48
+  DW_CFA_advance_loc: 1 to 000000000000bb08
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000bb4a
+  DW_CFA_advance_loc: 2 to 000000000000bb0a
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000bb4c
+  DW_CFA_advance_loc: 2 to 000000000000bb0c
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000bb4e
+  DW_CFA_advance_loc: 2 to 000000000000bb0e
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000000000000bb4f
+  DW_CFA_advance_loc: 1 to 000000000000bb0f
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_restore: r13 (r13)
   DW_CFA_restore: r14 (r14)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000004b4 0000000000000040 000004b8 FDE cie=00000000 pc=000000000000bb50..000000000000bd6f
-  DW_CFA_advance_loc: 20 to 000000000000bb64
+000004ac 0000000000000040 000004b0 FDE cie=00000000 pc=000000000000bb10..000000000000bd2f
+  DW_CFA_advance_loc: 20 to 000000000000bb24
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 5 to 000000000000bb69
+  DW_CFA_advance_loc: 5 to 000000000000bb29
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 5 to 000000000000bb6e
+  DW_CFA_advance_loc: 5 to 000000000000bb2e
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 1 to 000000000000bb6f
+  DW_CFA_advance_loc: 1 to 000000000000bb2f
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 4 to 000000000000bb73
+  DW_CFA_advance_loc: 4 to 000000000000bb33
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc2: 499 to 000000000000bd66
+  DW_CFA_advance_loc2: 499 to 000000000000bd26
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 000000000000bd67
+  DW_CFA_advance_loc: 1 to 000000000000bd27
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000bd69
+  DW_CFA_advance_loc: 2 to 000000000000bd29
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000bd6b
+  DW_CFA_advance_loc: 2 to 000000000000bd2b
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000bd6d
+  DW_CFA_advance_loc: 2 to 000000000000bd2d
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000000000000bd6e
+  DW_CFA_advance_loc: 1 to 000000000000bd2e
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_restore: r13 (r13)
   DW_CFA_restore: r14 (r14)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000004f8 000000000000004c 000004fc FDE cie=00000000 pc=000000000000e130..000000000000e1ec
-  DW_CFA_advance_loc: 12 to 000000000000e13c
+000004f0 000000000000004c 000004f4 FDE cie=00000000 pc=000000000000e0f0..000000000000e1ac
+  DW_CFA_advance_loc: 12 to 000000000000e0fc
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 2 to 000000000000e13e
+  DW_CFA_advance_loc: 2 to 000000000000e0fe
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 2 to 000000000000e140
+  DW_CFA_advance_loc: 2 to 000000000000e100
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 1 to 000000000000e141
+  DW_CFA_advance_loc: 1 to 000000000000e101
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000000e142
+  DW_CFA_advance_loc: 1 to 000000000000e102
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc: 32 to 000000000000e162
+  DW_CFA_advance_loc: 32 to 000000000000e122
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 000000000000e163
+  DW_CFA_advance_loc: 1 to 000000000000e123
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000e165
+  DW_CFA_advance_loc: 2 to 000000000000e125
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000e167
+  DW_CFA_advance_loc: 2 to 000000000000e127
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000e169
+  DW_CFA_advance_loc: 2 to 000000000000e129
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 7 to 000000000000e170
+  DW_CFA_advance_loc: 7 to 000000000000e130
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 68 to 000000000000e1b4
+  DW_CFA_advance_loc1: 68 to 000000000000e174
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 000000000000e1b5
+  DW_CFA_advance_loc: 1 to 000000000000e175
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000e1b7
+  DW_CFA_advance_loc: 2 to 000000000000e177
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000e1b9
+  DW_CFA_advance_loc: 2 to 000000000000e179
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000e1bb
+  DW_CFA_advance_loc: 2 to 000000000000e17b
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 5 to 000000000000e1c0
+  DW_CFA_advance_loc: 5 to 000000000000e180
   DW_CFA_restore_state
   DW_CFA_nop
 
-00000548 000000000000004c 0000054c FDE cie=00000000 pc=000000000000e1f0..000000000000e2ac
-  DW_CFA_advance_loc: 12 to 000000000000e1fc
+00000540 000000000000004c 00000544 FDE cie=00000000 pc=000000000000e1b0..000000000000e26c
+  DW_CFA_advance_loc: 12 to 000000000000e1bc
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 2 to 000000000000e1fe
+  DW_CFA_advance_loc: 2 to 000000000000e1be
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 2 to 000000000000e200
+  DW_CFA_advance_loc: 2 to 000000000000e1c0
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 1 to 000000000000e201
+  DW_CFA_advance_loc: 1 to 000000000000e1c1
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000000e202
+  DW_CFA_advance_loc: 1 to 000000000000e1c2
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc: 32 to 000000000000e222
+  DW_CFA_advance_loc: 32 to 000000000000e1e2
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 000000000000e223
+  DW_CFA_advance_loc: 1 to 000000000000e1e3
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000e225
+  DW_CFA_advance_loc: 2 to 000000000000e1e5
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000e227
+  DW_CFA_advance_loc: 2 to 000000000000e1e7
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000e229
+  DW_CFA_advance_loc: 2 to 000000000000e1e9
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 7 to 000000000000e230
+  DW_CFA_advance_loc: 7 to 000000000000e1f0
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 69 to 000000000000e275
+  DW_CFA_advance_loc1: 69 to 000000000000e235
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 000000000000e276
+  DW_CFA_advance_loc: 1 to 000000000000e236
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000e278
+  DW_CFA_advance_loc: 2 to 000000000000e238
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000e27a
+  DW_CFA_advance_loc: 2 to 000000000000e23a
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000e27c
+  DW_CFA_advance_loc: 2 to 000000000000e23c
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 4 to 000000000000e280
+  DW_CFA_advance_loc: 4 to 000000000000e240
   DW_CFA_restore_state
   DW_CFA_nop
 
-00000598 0000000000000048 0000059c FDE cie=00000000 pc=000000000000e2b0..000000000000e3f8
-  DW_CFA_advance_loc: 2 to 000000000000e2b2
+00000590 0000000000000048 00000594 FDE cie=00000000 pc=000000000000e270..000000000000e3b8
+  DW_CFA_advance_loc: 2 to 000000000000e272
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 000000000000e2b4
+  DW_CFA_advance_loc: 2 to 000000000000e274
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 000000000000e2b6
+  DW_CFA_advance_loc: 2 to 000000000000e276
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 000000000000e2b8
+  DW_CFA_advance_loc: 2 to 000000000000e278
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000000e2b9
+  DW_CFA_advance_loc: 1 to 000000000000e279
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 000000000000e2ba
+  DW_CFA_advance_loc: 1 to 000000000000e27a
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 14 to 000000000000e2c8
+  DW_CFA_advance_loc: 14 to 000000000000e288
   DW_CFA_def_cfa_offset: 80
-  DW_CFA_advance_loc1: 147 to 000000000000e35b
+  DW_CFA_advance_loc1: 147 to 000000000000e31b
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 000000000000e35c
+  DW_CFA_advance_loc: 1 to 000000000000e31c
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 000000000000e35d
+  DW_CFA_advance_loc: 1 to 000000000000e31d
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000e35f
+  DW_CFA_advance_loc: 2 to 000000000000e31f
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000e361
+  DW_CFA_advance_loc: 2 to 000000000000e321
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000e363
+  DW_CFA_advance_loc: 2 to 000000000000e323
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000e365
+  DW_CFA_advance_loc: 2 to 000000000000e325
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 11 to 000000000000e370
+  DW_CFA_advance_loc: 11 to 000000000000e330
   DW_CFA_restore_state
   DW_CFA_nop
 
-000005e4 000000000000001c 00000000 CIE
+000005dc 000000000000001c 00000000 CIE
   Version:               1
   Augmentation:          "zPLR"
   Code alignment factor: 1
   Data alignment factor: -8
   Return address column: 16
-  Augmentation data:     9b 41 32 00 00 1b 1b
+  Augmentation data:     9b 49 32 00 00 1b 1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000604 0000000000000050 00000024 FDE cie=000005e4 pc=000000000000bd70..000000000000c752
+000005fc 0000000000000050 00000024 FDE cie=000005dc pc=000000000000bd30..000000000000c712
   Augmentation data:     b3 12 00 00
-  DW_CFA_advance_loc: 2 to 000000000000bd72
+  DW_CFA_advance_loc: 2 to 000000000000bd32
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 000000000000bd74
+  DW_CFA_advance_loc: 2 to 000000000000bd34
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 000000000000bd76
+  DW_CFA_advance_loc: 2 to 000000000000bd36
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 5 to 000000000000bd7b
+  DW_CFA_advance_loc: 5 to 000000000000bd3b
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 4 to 000000000000bd7f
+  DW_CFA_advance_loc: 4 to 000000000000bd3f
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 7 to 000000000000bd86
+  DW_CFA_advance_loc: 7 to 000000000000bd46
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 000000000000bd8d
+  DW_CFA_advance_loc: 7 to 000000000000bd4d
   DW_CFA_def_cfa_offset: 224
-  DW_CFA_advance_loc2: 2184 to 000000000000c615
+  DW_CFA_advance_loc2: 2184 to 000000000000c5d5
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 000000000000c616
+  DW_CFA_advance_loc: 1 to 000000000000c5d6
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 000000000000c617
+  DW_CFA_advance_loc: 1 to 000000000000c5d7
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000c619
+  DW_CFA_advance_loc: 2 to 000000000000c5d9
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000c61b
+  DW_CFA_advance_loc: 2 to 000000000000c5db
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000c61d
+  DW_CFA_advance_loc: 2 to 000000000000c5dd
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000c61f
+  DW_CFA_advance_loc: 2 to 000000000000c5df
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000000000000c620
+  DW_CFA_advance_loc: 1 to 000000000000c5e0
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000658 000000000000002c 00000000 CIE
+00000650 000000000000002c 00000000 CIE
   Version:               1
   Augmentation:          "zPLR"
   Code alignment factor: 1
   Data alignment factor: -8
   Return address column: 16
-  Augmentation data:     9b cd 31 00 00 1b 1b
+  Augmentation data:     9b d5 31 00 00 1b 1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_def_cfa_offset: 224
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000688 0000000000000014 00000034 FDE cie=00000658 pc=00000000000032d0..00000000000032ea
+00000680 0000000000000014 00000034 FDE cie=00000650 pc=00000000000032d0..00000000000032ea
   Augmentation data:     38 12 00 00
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000006a0 0000000000000050 000000c0 FDE cie=000005e4 pc=000000000000c760..000000000000ceda
+00000698 0000000000000050 000000c0 FDE cie=000005dc pc=000000000000c720..000000000000ce9a
   Augmentation data:     28 12 00 00
-  DW_CFA_advance_loc: 2 to 000000000000c762
+  DW_CFA_advance_loc: 2 to 000000000000c722
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 5 to 000000000000c767
+  DW_CFA_advance_loc: 5 to 000000000000c727
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 5 to 000000000000c76c
+  DW_CFA_advance_loc: 5 to 000000000000c72c
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 5 to 000000000000c771
+  DW_CFA_advance_loc: 5 to 000000000000c731
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 4 to 000000000000c775
+  DW_CFA_advance_loc: 4 to 000000000000c735
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 000000000000c776
+  DW_CFA_advance_loc: 1 to 000000000000c736
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 13 to 000000000000c783
+  DW_CFA_advance_loc: 13 to 000000000000c743
   DW_CFA_def_cfa_offset: 224
-  DW_CFA_advance_loc2: 1506 to 000000000000cd65
+  DW_CFA_advance_loc2: 1506 to 000000000000cd25
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 000000000000cd66
+  DW_CFA_advance_loc: 1 to 000000000000cd26
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 000000000000cd67
+  DW_CFA_advance_loc: 1 to 000000000000cd27
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000cd69
+  DW_CFA_advance_loc: 2 to 000000000000cd29
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000cd6b
+  DW_CFA_advance_loc: 2 to 000000000000cd2b
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000cd6d
+  DW_CFA_advance_loc: 2 to 000000000000cd2d
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000cd6f
+  DW_CFA_advance_loc: 2 to 000000000000cd2f
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000000000000cd70
+  DW_CFA_advance_loc: 1 to 000000000000cd30
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000006f4 0000000000000014 000000a0 FDE cie=00000658 pc=00000000000032ea..0000000000003304
+000006ec 0000000000000014 000000a0 FDE cie=00000650 pc=00000000000032ea..0000000000003304
   Augmentation data:     dd 11 00 00
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000070c 0000000000000048 00000710 FDE cie=00000000 pc=000000000000e400..000000000000e550
-  DW_CFA_advance_loc: 2 to 000000000000e402
+00000704 0000000000000048 00000708 FDE cie=00000000 pc=000000000000e3c0..000000000000e510
+  DW_CFA_advance_loc: 2 to 000000000000e3c2
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 000000000000e404
+  DW_CFA_advance_loc: 2 to 000000000000e3c4
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 000000000000e406
+  DW_CFA_advance_loc: 2 to 000000000000e3c6
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 000000000000e408
+  DW_CFA_advance_loc: 2 to 000000000000e3c8
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000000e409
+  DW_CFA_advance_loc: 1 to 000000000000e3c9
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 000000000000e40a
+  DW_CFA_advance_loc: 1 to 000000000000e3ca
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 14 to 000000000000e418
+  DW_CFA_advance_loc: 14 to 000000000000e3d8
   DW_CFA_def_cfa_offset: 80
-  DW_CFA_advance_loc1: 146 to 000000000000e4aa
+  DW_CFA_advance_loc1: 146 to 000000000000e46a
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 000000000000e4ab
+  DW_CFA_advance_loc: 1 to 000000000000e46b
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 000000000000e4ac
+  DW_CFA_advance_loc: 1 to 000000000000e46c
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000e4ae
+  DW_CFA_advance_loc: 2 to 000000000000e46e
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000e4b0
+  DW_CFA_advance_loc: 2 to 000000000000e470
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000e4b2
+  DW_CFA_advance_loc: 2 to 000000000000e472
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000e4b4
+  DW_CFA_advance_loc: 2 to 000000000000e474
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 4 to 000000000000e4b8
+  DW_CFA_advance_loc: 4 to 000000000000e478
   DW_CFA_restore_state
   DW_CFA_nop
 
-00000758 0000000000000050 00000178 FDE cie=000005e4 pc=000000000000cee0..000000000000d94f
+00000750 0000000000000050 00000178 FDE cie=000005dc pc=000000000000cea0..000000000000d90f
   Augmentation data:     81 11 00 00
-  DW_CFA_advance_loc: 2 to 000000000000cee2
+  DW_CFA_advance_loc: 2 to 000000000000cea2
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 000000000000cee4
+  DW_CFA_advance_loc: 2 to 000000000000cea4
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 000000000000cee6
+  DW_CFA_advance_loc: 2 to 000000000000cea6
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 5 to 000000000000ceeb
+  DW_CFA_advance_loc: 5 to 000000000000ceab
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 4 to 000000000000ceef
+  DW_CFA_advance_loc: 4 to 000000000000ceaf
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 7 to 000000000000cef6
+  DW_CFA_advance_loc: 7 to 000000000000ceb6
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 000000000000cefd
+  DW_CFA_advance_loc: 7 to 000000000000cebd
   DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc2: 2294 to 000000000000d7f3
+  DW_CFA_advance_loc2: 2294 to 000000000000d7b3
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 000000000000d7f4
+  DW_CFA_advance_loc: 1 to 000000000000d7b4
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 000000000000d7f5
+  DW_CFA_advance_loc: 1 to 000000000000d7b5
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000d7f7
+  DW_CFA_advance_loc: 2 to 000000000000d7b7
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000d7f9
+  DW_CFA_advance_loc: 2 to 000000000000d7b9
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000d7fb
+  DW_CFA_advance_loc: 2 to 000000000000d7bb
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000d7fd
+  DW_CFA_advance_loc: 2 to 000000000000d7bd
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 3 to 000000000000d800
+  DW_CFA_advance_loc: 3 to 000000000000d7c0
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000007ac 000000000000002c 00000000 CIE
+000007a4 000000000000002c 00000000 CIE
   Version:               1
   Augmentation:          "zPLR"
   Code alignment factor: 1
   Data alignment factor: -8
   Return address column: 16
-  Augmentation data:     9b 79 30 00 00 1b 1b
+  Augmentation data:     9b 81 30 00 00 1b 1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_def_cfa_offset: 192
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000007dc 0000000000000014 00000034 FDE cie=000007ac pc=0000000000003304..000000000000331b
+000007d4 0000000000000014 00000034 FDE cie=000007a4 pc=0000000000003304..000000000000331b
   Augmentation data:     06 11 00 00
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000007f4 0000000000000050 00000214 FDE cie=000005e4 pc=000000000000d950..000000000000e122
+000007ec 0000000000000050 00000214 FDE cie=000005dc pc=000000000000d910..000000000000e0e2
   Augmentation data:     f6 10 00 00
-  DW_CFA_advance_loc: 2 to 000000000000d952
+  DW_CFA_advance_loc: 2 to 000000000000d912
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 000000000000d954
+  DW_CFA_advance_loc: 2 to 000000000000d914
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 000000000000d956
+  DW_CFA_advance_loc: 2 to 000000000000d916
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 5 to 000000000000d95b
+  DW_CFA_advance_loc: 5 to 000000000000d91b
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 4 to 000000000000d95f
+  DW_CFA_advance_loc: 4 to 000000000000d91f
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 7 to 000000000000d966
+  DW_CFA_advance_loc: 7 to 000000000000d926
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 000000000000d96d
+  DW_CFA_advance_loc: 7 to 000000000000d92d
   DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc2: 1590 to 000000000000dfa3
+  DW_CFA_advance_loc2: 1590 to 000000000000df63
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 000000000000dfa4
+  DW_CFA_advance_loc: 1 to 000000000000df64
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 000000000000dfa5
+  DW_CFA_advance_loc: 1 to 000000000000df65
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000dfa7
+  DW_CFA_advance_loc: 2 to 000000000000df67
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000dfa9
+  DW_CFA_advance_loc: 2 to 000000000000df69
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000dfab
+  DW_CFA_advance_loc: 2 to 000000000000df6b
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000dfad
+  DW_CFA_advance_loc: 2 to 000000000000df6d
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 3 to 000000000000dfb0
+  DW_CFA_advance_loc: 3 to 000000000000df70
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000848 0000000000000014 000000a0 FDE cie=000007ac pc=000000000000331b..0000000000003332
+00000840 0000000000000014 000000a0 FDE cie=000007a4 pc=000000000000331b..0000000000003332
   Augmentation data:     ab 10 00 00
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000860 0000000000000014 00000864 FDE cie=00000000 pc=0000000000003350..000000000000337e
+00000858 0000000000000014 0000085c FDE cie=00000000 pc=0000000000003350..000000000000337e
   DW_CFA_advance_loc: 4 to 0000000000003354
   DW_CFA_def_cfa_offset: 16
   DW_CFA_advance_loc: 23 to 000000000000336b
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
 
-00000878 0000000000000028 0000087c FDE cie=00000000 pc=000000000000e550..000000000000e671
-  DW_CFA_advance_loc: 5 to 000000000000e555
+00000870 0000000000000028 00000874 FDE cie=00000000 pc=000000000000e510..000000000000e631
+  DW_CFA_advance_loc: 5 to 000000000000e515
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 10 to 000000000000e55f
+  DW_CFA_advance_loc: 10 to 000000000000e51f
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r3 (rbx) at cfa-24
-  DW_CFA_advance_loc1: 183 to 000000000000e616
+  DW_CFA_advance_loc1: 183 to 000000000000e5d6
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 000000000000e617
+  DW_CFA_advance_loc: 1 to 000000000000e5d7
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 9 to 000000000000e620
+  DW_CFA_advance_loc: 9 to 000000000000e5e0
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 79 to 000000000000e66f
+  DW_CFA_advance_loc1: 79 to 000000000000e62f
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 000000000000e670
+  DW_CFA_advance_loc: 1 to 000000000000e630
   DW_CFA_def_cfa_offset: 8
 
-000008a4 0000000000000028 000008a8 FDE cie=00000000 pc=0000000000013920..0000000000013a41
-  DW_CFA_advance_loc: 5 to 0000000000013925
+0000089c 0000000000000028 000008a0 FDE cie=00000000 pc=00000000000138e0..0000000000013a01
+  DW_CFA_advance_loc: 5 to 00000000000138e5
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 10 to 000000000001392f
+  DW_CFA_advance_loc: 10 to 00000000000138ef
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r3 (rbx) at cfa-24
-  DW_CFA_advance_loc1: 183 to 00000000000139e6
+  DW_CFA_advance_loc1: 183 to 00000000000139a6
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00000000000139e7
+  DW_CFA_advance_loc: 1 to 00000000000139a7
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 9 to 00000000000139f0
+  DW_CFA_advance_loc: 9 to 00000000000139b0
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 79 to 0000000000013a3f
+  DW_CFA_advance_loc1: 79 to 00000000000139ff
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 0000000000013a40
+  DW_CFA_advance_loc: 1 to 0000000000013a00
   DW_CFA_def_cfa_offset: 8
 
-000008d0 0000000000000028 000008d4 FDE cie=00000000 pc=000000000000e680..000000000000e789
-  DW_CFA_advance_loc: 5 to 000000000000e685
+000008c8 0000000000000028 000008cc FDE cie=00000000 pc=000000000000e640..000000000000e749
+  DW_CFA_advance_loc: 5 to 000000000000e645
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 10 to 000000000000e68f
+  DW_CFA_advance_loc: 10 to 000000000000e64f
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r3 (rbx) at cfa-24
-  DW_CFA_advance_loc1: 174 to 000000000000e73d
+  DW_CFA_advance_loc1: 174 to 000000000000e6fd
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 000000000000e73e
+  DW_CFA_advance_loc: 1 to 000000000000e6fe
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 2 to 000000000000e740
+  DW_CFA_advance_loc: 2 to 000000000000e700
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 71 to 000000000000e787
+  DW_CFA_advance_loc1: 71 to 000000000000e747
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 000000000000e788
+  DW_CFA_advance_loc: 1 to 000000000000e748
   DW_CFA_def_cfa_offset: 8
 
-000008fc 0000000000000028 00000900 FDE cie=00000000 pc=0000000000013a50..0000000000013b59
-  DW_CFA_advance_loc: 5 to 0000000000013a55
+000008f4 0000000000000028 000008f8 FDE cie=00000000 pc=0000000000013a10..0000000000013b19
+  DW_CFA_advance_loc: 5 to 0000000000013a15
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 10 to 0000000000013a5f
+  DW_CFA_advance_loc: 10 to 0000000000013a1f
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r3 (rbx) at cfa-24
-  DW_CFA_advance_loc1: 174 to 0000000000013b0d
+  DW_CFA_advance_loc1: 174 to 0000000000013acd
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 0000000000013b0e
+  DW_CFA_advance_loc: 1 to 0000000000013ace
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 2 to 0000000000013b10
+  DW_CFA_advance_loc: 2 to 0000000000013ad0
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 71 to 0000000000013b57
+  DW_CFA_advance_loc1: 71 to 0000000000013b17
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 0000000000013b58
+  DW_CFA_advance_loc: 1 to 0000000000013b18
   DW_CFA_def_cfa_offset: 8
 
-00000928 0000000000000010 0000092c FDE cie=00000000 pc=000000000000e790..000000000000e8b8
+00000920 0000000000000010 00000924 FDE cie=00000000 pc=000000000000e750..000000000000e878
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000093c 0000000000000010 00000940 FDE cie=00000000 pc=0000000000013b60..0000000000013c88
+00000934 0000000000000010 00000938 FDE cie=00000000 pc=0000000000013b20..0000000000013c48
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000950 0000000000000010 00000954 FDE cie=00000000 pc=000000000000e8c0..000000000000e9e8
+00000948 0000000000000010 0000094c FDE cie=00000000 pc=000000000000e880..000000000000e9a8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000964 0000000000000010 00000968 FDE cie=00000000 pc=0000000000013c90..0000000000013db8
+0000095c 0000000000000010 00000960 FDE cie=00000000 pc=0000000000013c50..0000000000013d78
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000978 0000000000000044 0000097c FDE cie=00000000 pc=000000000000e9f0..000000000000ebb3
-  DW_CFA_advance_loc: 20 to 000000000000ea04
+00000970 0000000000000044 00000974 FDE cie=00000000 pc=000000000000e9b0..000000000000eb73
+  DW_CFA_advance_loc: 20 to 000000000000e9c4
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 8 to 000000000000ea0c
+  DW_CFA_advance_loc: 8 to 000000000000e9cc
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 5 to 000000000000ea11
+  DW_CFA_advance_loc: 5 to 000000000000e9d1
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 1 to 000000000000ea12
+  DW_CFA_advance_loc: 1 to 000000000000e9d2
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 5 to 000000000000ea17
+  DW_CFA_advance_loc: 5 to 000000000000e9d7
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc2: 375 to 000000000000eb8e
+  DW_CFA_advance_loc2: 375 to 000000000000eb4e
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 000000000000eb8f
+  DW_CFA_advance_loc: 1 to 000000000000eb4f
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000eb91
+  DW_CFA_advance_loc: 2 to 000000000000eb51
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000eb93
+  DW_CFA_advance_loc: 2 to 000000000000eb53
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000eb95
+  DW_CFA_advance_loc: 2 to 000000000000eb55
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000000000000eb96
+  DW_CFA_advance_loc: 1 to 000000000000eb56
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 28 to 000000000000ebb2
+  DW_CFA_advance_loc: 28 to 000000000000eb72
   DW_CFA_def_cfa_offset: 8
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_restore: r13 (r13)
   DW_CFA_restore: r14 (r14)
   DW_CFA_nop
   DW_CFA_nop
 
-000009c0 0000000000000044 000009c4 FDE cie=00000000 pc=000000000000ebc0..000000000000ed72
-  DW_CFA_advance_loc: 18 to 000000000000ebd2
+000009b8 0000000000000044 000009bc FDE cie=00000000 pc=000000000000eb80..000000000000ed32
+  DW_CFA_advance_loc: 18 to 000000000000eb92
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 8 to 000000000000ebda
+  DW_CFA_advance_loc: 8 to 000000000000eb9a
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 5 to 000000000000ebdf
+  DW_CFA_advance_loc: 5 to 000000000000eb9f
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 1 to 000000000000ebe0
+  DW_CFA_advance_loc: 1 to 000000000000eba0
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 5 to 000000000000ebe5
+  DW_CFA_advance_loc: 5 to 000000000000eba5
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc2: 361 to 000000000000ed4e
+  DW_CFA_advance_loc2: 361 to 000000000000ed0e
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 000000000000ed4f
+  DW_CFA_advance_loc: 1 to 000000000000ed0f
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000ed51
+  DW_CFA_advance_loc: 2 to 000000000000ed11
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000ed53
+  DW_CFA_advance_loc: 2 to 000000000000ed13
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000ed55
+  DW_CFA_advance_loc: 2 to 000000000000ed15
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000000000000ed56
+  DW_CFA_advance_loc: 1 to 000000000000ed16
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 27 to 000000000000ed71
+  DW_CFA_advance_loc: 27 to 000000000000ed31
   DW_CFA_def_cfa_offset: 8
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_restore: r13 (r13)
   DW_CFA_restore: r14 (r14)
   DW_CFA_nop
   DW_CFA_nop
 
-00000a08 0000000000000040 00000a0c FDE cie=00000000 pc=000000000000ed80..000000000000ef2b
-  DW_CFA_advance_loc: 18 to 000000000000ed92
+00000a00 0000000000000040 00000a04 FDE cie=00000000 pc=000000000000ed40..000000000000eeeb
+  DW_CFA_advance_loc: 18 to 000000000000ed52
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 5 to 000000000000ed97
+  DW_CFA_advance_loc: 5 to 000000000000ed57
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 6 to 000000000000ed9d
+  DW_CFA_advance_loc: 6 to 000000000000ed5d
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 4 to 000000000000eda1
+  DW_CFA_advance_loc: 4 to 000000000000ed61
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000000eda2
+  DW_CFA_advance_loc: 1 to 000000000000ed62
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc2: 384 to 000000000000ef22
+  DW_CFA_advance_loc2: 384 to 000000000000eee2
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 000000000000ef23
+  DW_CFA_advance_loc: 1 to 000000000000eee3
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000ef25
+  DW_CFA_advance_loc: 2 to 000000000000eee5
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000ef27
+  DW_CFA_advance_loc: 2 to 000000000000eee7
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000ef29
+  DW_CFA_advance_loc: 2 to 000000000000eee9
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000000000000ef2a
+  DW_CFA_advance_loc: 1 to 000000000000eeea
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_restore: r13 (r13)
   DW_CFA_restore: r14 (r14)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000a4c 0000000000000040 00000a50 FDE cie=00000000 pc=000000000000ef30..000000000000f0eb
-  DW_CFA_advance_loc: 20 to 000000000000ef44
+00000a44 0000000000000040 00000a48 FDE cie=00000000 pc=000000000000eef0..000000000000f0ab
+  DW_CFA_advance_loc: 20 to 000000000000ef04
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 5 to 000000000000ef49
+  DW_CFA_advance_loc: 5 to 000000000000ef09
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 6 to 000000000000ef4f
+  DW_CFA_advance_loc: 6 to 000000000000ef0f
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 4 to 000000000000ef53
+  DW_CFA_advance_loc: 4 to 000000000000ef13
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000000ef54
+  DW_CFA_advance_loc: 1 to 000000000000ef14
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc2: 398 to 000000000000f0e2
+  DW_CFA_advance_loc2: 398 to 000000000000f0a2
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 000000000000f0e3
+  DW_CFA_advance_loc: 1 to 000000000000f0a3
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000f0e5
+  DW_CFA_advance_loc: 2 to 000000000000f0a5
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000f0e7
+  DW_CFA_advance_loc: 2 to 000000000000f0a7
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000f0e9
+  DW_CFA_advance_loc: 2 to 000000000000f0a9
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000000000000f0ea
+  DW_CFA_advance_loc: 1 to 000000000000f0aa
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_restore: r13 (r13)
   DW_CFA_restore: r14 (r14)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000a90 0000000000000010 00000a94 FDE cie=00000000 pc=000000000000f0f0..000000000000f113
+00000a88 0000000000000010 00000a8c FDE cie=00000000 pc=000000000000f0b0..000000000000f0d3
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000aa4 0000000000000010 00000aa8 FDE cie=00000000 pc=000000000000f120..000000000000f143
+00000a9c 0000000000000010 00000aa0 FDE cie=00000000 pc=000000000000f0e0..000000000000f103
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000ab8 0000000000000010 00000abc FDE cie=00000000 pc=000000000000f150..000000000000f183
+00000ab0 0000000000000010 00000ab4 FDE cie=00000000 pc=000000000000f110..000000000000f143
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000acc 0000000000000010 00000ad0 FDE cie=00000000 pc=000000000000f190..000000000000f3ad
+00000ac4 0000000000000010 00000ac8 FDE cie=00000000 pc=000000000000f150..000000000000f36d
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000ae0 0000000000000010 00000ae4 FDE cie=00000000 pc=000000000000f3b0..000000000000f5c1
+00000ad8 0000000000000010 00000adc FDE cie=00000000 pc=000000000000f370..000000000000f581
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000af4 0000000000000010 00000af8 FDE cie=00000000 pc=000000000000f5d0..000000000000f939
+00000aec 0000000000000010 00000af0 FDE cie=00000000 pc=000000000000f590..000000000000f8f9
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000b08 0000000000000010 00000b0c FDE cie=00000000 pc=000000000000f940..000000000000f987
+00000b00 0000000000000010 00000b04 FDE cie=00000000 pc=000000000000f900..000000000000f947
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000b1c 0000000000000010 00000b20 FDE cie=00000000 pc=000000000000f990..000000000000fa8f
+00000b14 0000000000000010 00000b18 FDE cie=00000000 pc=000000000000f950..000000000000fa4f
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000b30 0000000000000010 00000b34 FDE cie=00000000 pc=000000000000fa90..000000000000fb1d
+00000b28 0000000000000010 00000b2c FDE cie=00000000 pc=000000000000fa50..000000000000fadd
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000b44 0000000000000010 00000b48 FDE cie=00000000 pc=000000000000fb20..000000000000fbfb
+00000b3c 0000000000000010 00000b40 FDE cie=00000000 pc=000000000000fae0..000000000000fbbb
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000b58 0000000000000010 00000b5c FDE cie=00000000 pc=000000000000fc00..000000000000fc8d
+00000b50 0000000000000010 00000b54 FDE cie=00000000 pc=000000000000fbc0..000000000000fc4d
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000b6c 0000000000000010 00000b70 FDE cie=00000000 pc=000000000000fc90..000000000000fce5
+00000b64 0000000000000010 00000b68 FDE cie=00000000 pc=000000000000fc50..000000000000fca5
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000b80 0000000000000010 00000b84 FDE cie=00000000 pc=000000000000fcf0..000000000000fd4d
+00000b78 0000000000000010 00000b7c FDE cie=00000000 pc=000000000000fcb0..000000000000fd0d
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000b94 0000000000000010 00000b98 FDE cie=00000000 pc=000000000000fd50..000000000000fde5
+00000b8c 0000000000000010 00000b90 FDE cie=00000000 pc=000000000000fd10..000000000000fda5
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000ba8 0000000000000010 00000bac FDE cie=00000000 pc=000000000000fdf0..000000000000fe6d
+00000ba0 0000000000000010 00000ba4 FDE cie=00000000 pc=000000000000fdb0..000000000000fe2d
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000bbc 0000000000000010 00000bc0 FDE cie=00000000 pc=000000000000fe70..000000000000ff2f
+00000bb4 0000000000000010 00000bb8 FDE cie=00000000 pc=000000000000fe30..000000000000feef
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000bd0 0000000000000010 00000bd4 FDE cie=00000000 pc=000000000000ff30..000000000000ffad
+00000bc8 0000000000000010 00000bcc FDE cie=00000000 pc=000000000000fef0..000000000000ff6d
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000be4 0000000000000010 00000be8 FDE cie=00000000 pc=000000000000ffb0..0000000000010005
+00000bdc 0000000000000010 00000be0 FDE cie=00000000 pc=000000000000ff70..000000000000ffc5
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000bf8 0000000000000010 00000bfc FDE cie=00000000 pc=0000000000010010..000000000001006d
+00000bf0 0000000000000010 00000bf4 FDE cie=00000000 pc=000000000000ffd0..000000000001002d
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000c0c 0000000000000010 00000c10 FDE cie=00000000 pc=0000000000010070..0000000000010105
+00000c04 0000000000000010 00000c08 FDE cie=00000000 pc=0000000000010030..00000000000100c5
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000c20 0000000000000044 00000c24 FDE cie=00000000 pc=0000000000010110..000000000001031a
-  DW_CFA_advance_loc: 2 to 0000000000010112
+00000c18 0000000000000044 00000c1c FDE cie=00000000 pc=00000000000100d0..00000000000102da
+  DW_CFA_advance_loc: 2 to 00000000000100d2
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 5 to 0000000000010117
+  DW_CFA_advance_loc: 5 to 00000000000100d7
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000010119
+  DW_CFA_advance_loc: 2 to 00000000000100d9
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 000000000001011b
+  DW_CFA_advance_loc: 2 to 00000000000100db
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 4 to 000000000001011f
+  DW_CFA_advance_loc: 4 to 00000000000100df
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 0000000000010120
+  DW_CFA_advance_loc: 1 to 00000000000100e0
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc2: 464 to 00000000000102f0
+  DW_CFA_advance_loc2: 464 to 00000000000102b0
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000102f1
+  DW_CFA_advance_loc: 1 to 00000000000102b1
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000102f3
+  DW_CFA_advance_loc: 2 to 00000000000102b3
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000102f5
+  DW_CFA_advance_loc: 2 to 00000000000102b5
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000102f7
+  DW_CFA_advance_loc: 2 to 00000000000102b7
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000102f9
+  DW_CFA_advance_loc: 2 to 00000000000102b9
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 7 to 0000000000010300
+  DW_CFA_advance_loc: 7 to 00000000000102c0
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
 
-00000c68 0000000000000044 00000c6c FDE cie=00000000 pc=0000000000010320..00000000000105cd
-  DW_CFA_advance_loc: 2 to 0000000000010322
+00000c60 0000000000000044 00000c64 FDE cie=00000000 pc=00000000000102e0..000000000001058d
+  DW_CFA_advance_loc: 2 to 00000000000102e2
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000010324
+  DW_CFA_advance_loc: 2 to 00000000000102e4
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000010326
+  DW_CFA_advance_loc: 2 to 00000000000102e6
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 7 to 000000000001032d
+  DW_CFA_advance_loc: 7 to 00000000000102ed
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000001032e
+  DW_CFA_advance_loc: 1 to 00000000000102ee
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 000000000001032f
+  DW_CFA_advance_loc: 1 to 00000000000102ef
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc2: 621 to 000000000001059c
+  DW_CFA_advance_loc2: 621 to 000000000001055c
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 000000000001059d
+  DW_CFA_advance_loc: 1 to 000000000001055d
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000001059f
+  DW_CFA_advance_loc: 2 to 000000000001055f
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000105a1
+  DW_CFA_advance_loc: 2 to 0000000000010561
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000105a3
+  DW_CFA_advance_loc: 2 to 0000000000010563
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000105a5
+  DW_CFA_advance_loc: 2 to 0000000000010565
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 11 to 00000000000105b0
+  DW_CFA_advance_loc: 11 to 0000000000010570
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
 
-00000cb0 0000000000000010 00000cb4 FDE cie=00000000 pc=00000000000105d0..0000000000010689
+00000ca8 0000000000000010 00000cac FDE cie=00000000 pc=0000000000010590..0000000000010649
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000cc4 0000000000000028 00000cc8 FDE cie=00000000 pc=0000000000010690..0000000000010766
-  DW_CFA_advance_loc: 1 to 0000000000010691
+00000cbc 0000000000000028 00000cc0 FDE cie=00000000 pc=0000000000010650..0000000000010726
+  DW_CFA_advance_loc: 1 to 0000000000010651
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 4 to 0000000000010695
+  DW_CFA_advance_loc: 4 to 0000000000010655
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r3 (rbx) at cfa-24
-  DW_CFA_advance_loc: 6 to 000000000001069b
+  DW_CFA_advance_loc: 6 to 000000000001065b
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc1: 164 to 000000000001073f
+  DW_CFA_advance_loc1: 164 to 00000000000106ff
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 5 to 0000000000010744
+  DW_CFA_advance_loc: 5 to 0000000000010704
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 0000000000010745
+  DW_CFA_advance_loc: 1 to 0000000000010705
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 19 to 0000000000010758
+  DW_CFA_advance_loc: 19 to 0000000000010718
   DW_CFA_restore_state
   DW_CFA_nop
 
-00000cf0 0000000000000010 00000cf4 FDE cie=00000000 pc=0000000000010770..0000000000010819
+00000ce8 0000000000000010 00000cec FDE cie=00000000 pc=0000000000010730..00000000000107d9
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000d04 0000000000000028 00000d08 FDE cie=00000000 pc=0000000000010820..000000000001090e
-  DW_CFA_advance_loc: 1 to 0000000000010821
+00000cfc 0000000000000028 00000d00 FDE cie=00000000 pc=00000000000107e0..00000000000108ce
+  DW_CFA_advance_loc: 1 to 00000000000107e1
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 4 to 0000000000010825
+  DW_CFA_advance_loc: 4 to 00000000000107e5
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r3 (rbx) at cfa-24
-  DW_CFA_advance_loc: 6 to 000000000001082b
+  DW_CFA_advance_loc: 6 to 00000000000107eb
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc1: 195 to 00000000000108ee
+  DW_CFA_advance_loc1: 195 to 00000000000108ae
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 5 to 00000000000108f3
+  DW_CFA_advance_loc: 5 to 00000000000108b3
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00000000000108f4
+  DW_CFA_advance_loc: 1 to 00000000000108b4
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 12 to 0000000000010900
+  DW_CFA_advance_loc: 12 to 00000000000108c0
   DW_CFA_restore_state
   DW_CFA_nop
 
-00000d30 0000000000000010 00000d34 FDE cie=00000000 pc=0000000000010910..0000000000010a41
+00000d28 0000000000000010 00000d2c FDE cie=00000000 pc=00000000000108d0..0000000000010a01
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000d44 0000000000000010 00000d48 FDE cie=00000000 pc=0000000000010a50..0000000000010b72
+00000d3c 0000000000000010 00000d40 FDE cie=00000000 pc=0000000000010a10..0000000000010b32
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000d58 0000000000000010 00000d5c FDE cie=00000000 pc=0000000000010b80..0000000000010c6f
+00000d50 0000000000000010 00000d54 FDE cie=00000000 pc=0000000000010b40..0000000000010c2f
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000d6c 0000000000000010 00000d70 FDE cie=00000000 pc=0000000000010c70..0000000000010d48
+00000d64 0000000000000010 00000d68 FDE cie=00000000 pc=0000000000010c30..0000000000010d08
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000d80 0000000000000010 00000d84 FDE cie=00000000 pc=0000000000010d50..0000000000010e0e
+00000d78 0000000000000010 00000d7c FDE cie=00000000 pc=0000000000010d10..0000000000010dce
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000d94 0000000000000010 00000d98 FDE cie=00000000 pc=0000000000010e10..0000000000010ef0
+00000d8c 0000000000000010 00000d90 FDE cie=00000000 pc=0000000000010dd0..0000000000010eb0
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000da8 0000000000000038 00000dac FDE cie=00000000 pc=0000000000010ef0..0000000000010f41
-  DW_CFA_advance_loc: 6 to 0000000000010ef6
+00000da0 0000000000000038 00000da4 FDE cie=00000000 pc=0000000000010eb0..0000000000010f01
+  DW_CFA_advance_loc: 6 to 0000000000010eb6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r13 (r13) at cfa-16
-  DW_CFA_advance_loc: 5 to 0000000000010efb
+  DW_CFA_advance_loc: 5 to 0000000000010ebb
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r12 (r12) at cfa-24
-  DW_CFA_advance_loc: 4 to 0000000000010eff
+  DW_CFA_advance_loc: 4 to 0000000000010ebf
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r6 (rbp) at cfa-32
-  DW_CFA_advance_loc: 4 to 0000000000010f03
+  DW_CFA_advance_loc: 4 to 0000000000010ec3
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r3 (rbx) at cfa-40
-  DW_CFA_advance_loc: 6 to 0000000000010f09
+  DW_CFA_advance_loc: 6 to 0000000000010ec9
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 38 to 0000000000010f2f
+  DW_CFA_advance_loc: 38 to 0000000000010eef
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 0000000000010f30
+  DW_CFA_advance_loc: 1 to 0000000000010ef0
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 0000000000010f31
+  DW_CFA_advance_loc: 1 to 0000000000010ef1
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000010f33
+  DW_CFA_advance_loc: 2 to 0000000000010ef3
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000010f35
+  DW_CFA_advance_loc: 2 to 0000000000010ef5
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 11 to 0000000000010f40
+  DW_CFA_advance_loc: 11 to 0000000000010f00
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_restore: r13 (r13)
 
-00000de4 0000000000000038 00000de8 FDE cie=00000000 pc=0000000000010f50..0000000000010fa1
-  DW_CFA_advance_loc: 6 to 0000000000010f56
+00000ddc 0000000000000038 00000de0 FDE cie=00000000 pc=0000000000010f10..0000000000010f61
+  DW_CFA_advance_loc: 6 to 0000000000010f16
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r13 (r13) at cfa-16
-  DW_CFA_advance_loc: 5 to 0000000000010f5b
+  DW_CFA_advance_loc: 5 to 0000000000010f1b
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r12 (r12) at cfa-24
-  DW_CFA_advance_loc: 4 to 0000000000010f5f
+  DW_CFA_advance_loc: 4 to 0000000000010f1f
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r6 (rbp) at cfa-32
-  DW_CFA_advance_loc: 4 to 0000000000010f63
+  DW_CFA_advance_loc: 4 to 0000000000010f23
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r3 (rbx) at cfa-40
-  DW_CFA_advance_loc: 6 to 0000000000010f69
+  DW_CFA_advance_loc: 6 to 0000000000010f29
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 38 to 0000000000010f8f
+  DW_CFA_advance_loc: 38 to 0000000000010f4f
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 0000000000010f90
+  DW_CFA_advance_loc: 1 to 0000000000010f50
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 0000000000010f91
+  DW_CFA_advance_loc: 1 to 0000000000010f51
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000010f93
+  DW_CFA_advance_loc: 2 to 0000000000010f53
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000010f95
+  DW_CFA_advance_loc: 2 to 0000000000010f55
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 11 to 0000000000010fa0
+  DW_CFA_advance_loc: 11 to 0000000000010f60
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_restore: r13 (r13)
 
-00000e20 0000000000000038 00000e24 FDE cie=00000000 pc=0000000000010fb0..0000000000011001
-  DW_CFA_advance_loc: 6 to 0000000000010fb6
+00000e18 0000000000000038 00000e1c FDE cie=00000000 pc=0000000000010f70..0000000000010fc1
+  DW_CFA_advance_loc: 6 to 0000000000010f76
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r13 (r13) at cfa-16
-  DW_CFA_advance_loc: 5 to 0000000000010fbb
+  DW_CFA_advance_loc: 5 to 0000000000010f7b
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r12 (r12) at cfa-24
-  DW_CFA_advance_loc: 4 to 0000000000010fbf
+  DW_CFA_advance_loc: 4 to 0000000000010f7f
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r6 (rbp) at cfa-32
-  DW_CFA_advance_loc: 4 to 0000000000010fc3
+  DW_CFA_advance_loc: 4 to 0000000000010f83
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r3 (rbx) at cfa-40
-  DW_CFA_advance_loc: 6 to 0000000000010fc9
+  DW_CFA_advance_loc: 6 to 0000000000010f89
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 38 to 0000000000010fef
+  DW_CFA_advance_loc: 38 to 0000000000010faf
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 0000000000010ff0
+  DW_CFA_advance_loc: 1 to 0000000000010fb0
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 0000000000010ff1
+  DW_CFA_advance_loc: 1 to 0000000000010fb1
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000010ff3
+  DW_CFA_advance_loc: 2 to 0000000000010fb3
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000010ff5
+  DW_CFA_advance_loc: 2 to 0000000000010fb5
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 11 to 0000000000011000
+  DW_CFA_advance_loc: 11 to 0000000000010fc0
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_restore: r13 (r13)
 
-00000e5c 0000000000000038 00000e60 FDE cie=00000000 pc=0000000000011010..0000000000011061
-  DW_CFA_advance_loc: 6 to 0000000000011016
+00000e54 0000000000000038 00000e58 FDE cie=00000000 pc=0000000000010fd0..0000000000011021
+  DW_CFA_advance_loc: 6 to 0000000000010fd6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r13 (r13) at cfa-16
-  DW_CFA_advance_loc: 5 to 000000000001101b
+  DW_CFA_advance_loc: 5 to 0000000000010fdb
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r12 (r12) at cfa-24
-  DW_CFA_advance_loc: 4 to 000000000001101f
+  DW_CFA_advance_loc: 4 to 0000000000010fdf
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r6 (rbp) at cfa-32
-  DW_CFA_advance_loc: 4 to 0000000000011023
+  DW_CFA_advance_loc: 4 to 0000000000010fe3
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r3 (rbx) at cfa-40
-  DW_CFA_advance_loc: 6 to 0000000000011029
+  DW_CFA_advance_loc: 6 to 0000000000010fe9
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 46 to 0000000000011057
+  DW_CFA_advance_loc: 46 to 0000000000011017
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 0000000000011058
+  DW_CFA_advance_loc: 1 to 0000000000011018
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 0000000000011059
+  DW_CFA_advance_loc: 1 to 0000000000011019
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000001105b
+  DW_CFA_advance_loc: 2 to 000000000001101b
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000001105d
+  DW_CFA_advance_loc: 2 to 000000000001101d
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 3 to 0000000000011060
+  DW_CFA_advance_loc: 3 to 0000000000011020
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_restore: r13 (r13)
 
-00000e98 0000000000000038 00000e9c FDE cie=00000000 pc=0000000000011070..00000000000110c1
-  DW_CFA_advance_loc: 6 to 0000000000011076
+00000e90 0000000000000038 00000e94 FDE cie=00000000 pc=0000000000011030..0000000000011081
+  DW_CFA_advance_loc: 6 to 0000000000011036
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r13 (r13) at cfa-16
-  DW_CFA_advance_loc: 5 to 000000000001107b
+  DW_CFA_advance_loc: 5 to 000000000001103b
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r12 (r12) at cfa-24
-  DW_CFA_advance_loc: 4 to 000000000001107f
+  DW_CFA_advance_loc: 4 to 000000000001103f
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r6 (rbp) at cfa-32
-  DW_CFA_advance_loc: 4 to 0000000000011083
+  DW_CFA_advance_loc: 4 to 0000000000011043
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r3 (rbx) at cfa-40
-  DW_CFA_advance_loc: 6 to 0000000000011089
+  DW_CFA_advance_loc: 6 to 0000000000011049
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 46 to 00000000000110b7
+  DW_CFA_advance_loc: 46 to 0000000000011077
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 00000000000110b8
+  DW_CFA_advance_loc: 1 to 0000000000011078
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 00000000000110b9
+  DW_CFA_advance_loc: 1 to 0000000000011079
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000110bb
+  DW_CFA_advance_loc: 2 to 000000000001107b
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000110bd
+  DW_CFA_advance_loc: 2 to 000000000001107d
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 3 to 00000000000110c0
+  DW_CFA_advance_loc: 3 to 0000000000011080
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_restore: r13 (r13)
 
-00000ed4 0000000000000038 00000ed8 FDE cie=00000000 pc=00000000000110d0..0000000000011121
-  DW_CFA_advance_loc: 6 to 00000000000110d6
+00000ecc 0000000000000038 00000ed0 FDE cie=00000000 pc=0000000000011090..00000000000110e1
+  DW_CFA_advance_loc: 6 to 0000000000011096
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r13 (r13) at cfa-16
-  DW_CFA_advance_loc: 5 to 00000000000110db
+  DW_CFA_advance_loc: 5 to 000000000001109b
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r12 (r12) at cfa-24
-  DW_CFA_advance_loc: 4 to 00000000000110df
+  DW_CFA_advance_loc: 4 to 000000000001109f
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r6 (rbp) at cfa-32
-  DW_CFA_advance_loc: 4 to 00000000000110e3
+  DW_CFA_advance_loc: 4 to 00000000000110a3
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r3 (rbx) at cfa-40
-  DW_CFA_advance_loc: 6 to 00000000000110e9
+  DW_CFA_advance_loc: 6 to 00000000000110a9
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 46 to 0000000000011117
+  DW_CFA_advance_loc: 46 to 00000000000110d7
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 0000000000011118
+  DW_CFA_advance_loc: 1 to 00000000000110d8
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 0000000000011119
+  DW_CFA_advance_loc: 1 to 00000000000110d9
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000001111b
+  DW_CFA_advance_loc: 2 to 00000000000110db
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000001111d
+  DW_CFA_advance_loc: 2 to 00000000000110dd
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 3 to 0000000000011120
+  DW_CFA_advance_loc: 3 to 00000000000110e0
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_restore: r13 (r13)
 
-00000f10 0000000000000028 00000f14 FDE cie=00000000 pc=0000000000011130..0000000000011222
-  DW_CFA_advance_loc: 12 to 000000000001113c
+00000f08 0000000000000028 00000f0c FDE cie=00000000 pc=00000000000110f0..00000000000111e2
+  DW_CFA_advance_loc: 12 to 00000000000110fc
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 7 to 0000000000011143
+  DW_CFA_advance_loc: 7 to 0000000000011103
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r3 (rbx) at cfa-24
-  DW_CFA_advance_loc1: 133 to 00000000000111c8
+  DW_CFA_advance_loc1: 133 to 0000000000011188
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00000000000111c9
+  DW_CFA_advance_loc: 1 to 0000000000011189
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 7 to 00000000000111d0
+  DW_CFA_advance_loc: 7 to 0000000000011190
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 81 to 0000000000011221
+  DW_CFA_advance_loc1: 81 to 00000000000111e1
   DW_CFA_def_cfa_offset: 8
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_nop
 
-00000f3c 0000000000000028 00000f40 FDE cie=00000000 pc=0000000000011230..0000000000011322
-  DW_CFA_advance_loc: 12 to 000000000001123c
+00000f34 0000000000000028 00000f38 FDE cie=00000000 pc=00000000000111f0..00000000000112e2
+  DW_CFA_advance_loc: 12 to 00000000000111fc
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 7 to 0000000000011243
+  DW_CFA_advance_loc: 7 to 0000000000011203
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r3 (rbx) at cfa-24
-  DW_CFA_advance_loc1: 131 to 00000000000112c6
+  DW_CFA_advance_loc1: 131 to 0000000000011286
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00000000000112c7
+  DW_CFA_advance_loc: 1 to 0000000000011287
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 9 to 00000000000112d0
+  DW_CFA_advance_loc: 9 to 0000000000011290
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 81 to 0000000000011321
+  DW_CFA_advance_loc1: 81 to 00000000000112e1
   DW_CFA_def_cfa_offset: 8
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_nop
 
-00000f68 000000000000001c 00000f6c FDE cie=00000000 pc=0000000000011330..0000000000011427
-  DW_CFA_advance_loc: 1 to 0000000000011331
+00000f60 000000000000001c 00000f64 FDE cie=00000000 pc=00000000000112f0..00000000000113e7
+  DW_CFA_advance_loc: 1 to 00000000000112f1
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc1: 215 to 0000000000011408
+  DW_CFA_advance_loc1: 215 to 00000000000113c8
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 0000000000011410
+  DW_CFA_advance_loc: 8 to 00000000000113d0
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000f88 000000000000001c 00000f8c FDE cie=00000000 pc=0000000000011430..0000000000011527
-  DW_CFA_advance_loc: 1 to 0000000000011431
+00000f80 000000000000001c 00000f84 FDE cie=00000000 pc=00000000000113f0..00000000000114e7
+  DW_CFA_advance_loc: 1 to 00000000000113f1
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc1: 215 to 0000000000011508
+  DW_CFA_advance_loc1: 215 to 00000000000114c8
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 0000000000011510
+  DW_CFA_advance_loc: 8 to 00000000000114d0
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000fa8 0000000000000010 00000fac FDE cie=00000000 pc=0000000000011530..00000000000115da
+00000fa0 0000000000000010 00000fa4 FDE cie=00000000 pc=00000000000114f0..000000000001159a
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000fbc 0000000000000010 00000fc0 FDE cie=00000000 pc=00000000000115e0..0000000000011692
+00000fb4 0000000000000010 00000fb8 FDE cie=00000000 pc=00000000000115a0..0000000000011652
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000fd0 0000000000000010 00000fd4 FDE cie=00000000 pc=00000000000116a0..0000000000011750
+00000fc8 0000000000000010 00000fcc FDE cie=00000000 pc=0000000000011660..0000000000011710
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000fe4 0000000000000010 00000fe8 FDE cie=00000000 pc=0000000000011750..0000000000011812
+00000fdc 0000000000000010 00000fe0 FDE cie=00000000 pc=0000000000011710..00000000000117d2
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000ff8 0000000000000010 00000ffc FDE cie=00000000 pc=0000000000011820..000000000001186b
+00000ff0 0000000000000010 00000ff4 FDE cie=00000000 pc=00000000000117e0..000000000001182b
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000100c 0000000000000010 00001010 FDE cie=00000000 pc=0000000000011870..00000000000118bb
+00001004 0000000000000010 00001008 FDE cie=00000000 pc=0000000000011830..000000000001187b
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001020 0000000000000010 00001024 FDE cie=00000000 pc=00000000000118c0..00000000000119c5
+00001018 0000000000000010 0000101c FDE cie=00000000 pc=0000000000011880..0000000000011985
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001034 0000000000000010 00001038 FDE cie=00000000 pc=00000000000119d0..0000000000011ad5
+0000102c 0000000000000010 00001030 FDE cie=00000000 pc=0000000000011990..0000000000011a95
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001048 0000000000000010 0000104c FDE cie=00000000 pc=0000000000011ae0..0000000000011b8a
+00001040 0000000000000010 00001044 FDE cie=00000000 pc=0000000000011aa0..0000000000011b4a
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000105c 0000000000000010 00001060 FDE cie=00000000 pc=0000000000011b90..0000000000011c42
+00001054 0000000000000010 00001058 FDE cie=00000000 pc=0000000000011b50..0000000000011c02
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001070 0000000000000010 00001074 FDE cie=00000000 pc=0000000000011c50..0000000000011e7a
+00001068 0000000000000010 0000106c FDE cie=00000000 pc=0000000000011c10..0000000000011e3a
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001084 0000000000000010 00001088 FDE cie=00000000 pc=0000000000011e80..0000000000011f29
+0000107c 0000000000000010 00001080 FDE cie=00000000 pc=0000000000011e40..0000000000011ee9
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001098 0000000000000010 0000109c FDE cie=00000000 pc=0000000000011f30..0000000000011f7b
+00001090 0000000000000010 00001094 FDE cie=00000000 pc=0000000000011ef0..0000000000011f3b
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000010ac 0000000000000010 000010b0 FDE cie=00000000 pc=0000000000011f80..0000000000011fcb
+000010a4 0000000000000010 000010a8 FDE cie=00000000 pc=0000000000011f40..0000000000011f8b
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000010c0 0000000000000010 000010c4 FDE cie=00000000 pc=0000000000011fd0..00000000000120b5
+000010b8 0000000000000010 000010bc FDE cie=00000000 pc=0000000000011f90..0000000000012075
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000010d4 0000000000000010 000010d8 FDE cie=00000000 pc=00000000000120c0..00000000000121d5
+000010cc 0000000000000010 000010d0 FDE cie=00000000 pc=0000000000012080..0000000000012195
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000010e8 0000000000000010 000010ec FDE cie=00000000 pc=00000000000121e0..00000000000122c5
+000010e0 0000000000000010 000010e4 FDE cie=00000000 pc=00000000000121a0..0000000000012285
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000010fc 0000000000000010 00001100 FDE cie=00000000 pc=00000000000122d0..0000000000012361
+000010f4 0000000000000010 000010f8 FDE cie=00000000 pc=0000000000012290..0000000000012321
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001110 0000000000000010 00001114 FDE cie=00000000 pc=0000000000012370..00000000000123f9
+00001108 0000000000000010 0000110c FDE cie=00000000 pc=0000000000012330..00000000000123b9
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001124 0000000000000010 00001128 FDE cie=00000000 pc=0000000000012400..00000000000124b5
+0000111c 0000000000000010 00001120 FDE cie=00000000 pc=00000000000123c0..0000000000012475
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001138 0000000000000010 0000113c FDE cie=00000000 pc=00000000000124c0..00000000000124e6
+00001130 0000000000000010 00001134 FDE cie=00000000 pc=0000000000012480..00000000000124a6
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000114c 0000000000000010 00001150 FDE cie=00000000 pc=00000000000124f0..000000000001257d
+00001144 0000000000000010 00001148 FDE cie=00000000 pc=00000000000124b0..000000000001253d
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001160 0000000000000010 00001164 FDE cie=00000000 pc=0000000000012580..00000000000125d5
+00001158 0000000000000010 0000115c FDE cie=00000000 pc=0000000000012540..0000000000012595
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001174 0000000000000010 00001178 FDE cie=00000000 pc=00000000000125e0..0000000000012750
+0000116c 0000000000000010 00001170 FDE cie=00000000 pc=00000000000125a0..0000000000012710
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001188 0000000000000010 0000118c FDE cie=00000000 pc=0000000000012750..00000000000127ac
+00001180 0000000000000010 00001184 FDE cie=00000000 pc=0000000000012710..000000000001276c
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000119c 0000000000000010 000011a0 FDE cie=00000000 pc=00000000000127b0..0000000000012865
+00001194 0000000000000010 00001198 FDE cie=00000000 pc=0000000000012770..0000000000012825
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000011b0 0000000000000010 000011b4 FDE cie=00000000 pc=0000000000012870..0000000000012897
+000011a8 0000000000000010 000011ac FDE cie=00000000 pc=0000000000012830..0000000000012857
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000011c4 0000000000000010 000011c8 FDE cie=00000000 pc=00000000000128a0..0000000000012935
+000011bc 0000000000000010 000011c0 FDE cie=00000000 pc=0000000000012860..00000000000128f5
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000011d8 0000000000000010 000011dc FDE cie=00000000 pc=0000000000012940..000000000001299d
+000011d0 0000000000000010 000011d4 FDE cie=00000000 pc=0000000000012900..000000000001295d
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000011ec 0000000000000010 000011f0 FDE cie=00000000 pc=00000000000129a0..0000000000012b38
+000011e4 0000000000000010 000011e8 FDE cie=00000000 pc=0000000000012960..0000000000012af8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001200 0000000000000010 00001204 FDE cie=00000000 pc=0000000000012b40..0000000000012b92
+000011f8 0000000000000010 000011fc FDE cie=00000000 pc=0000000000012b00..0000000000012b52
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001214 0000000000000040 00001218 FDE cie=00000000 pc=0000000000013dc0..0000000000013f7b
-  DW_CFA_advance_loc: 20 to 0000000000013dd4
+0000120c 0000000000000040 00001210 FDE cie=00000000 pc=0000000000013d80..0000000000013f3b
+  DW_CFA_advance_loc: 20 to 0000000000013d94
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 5 to 0000000000013dd9
+  DW_CFA_advance_loc: 5 to 0000000000013d99
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 6 to 0000000000013ddf
+  DW_CFA_advance_loc: 6 to 0000000000013d9f
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 4 to 0000000000013de3
+  DW_CFA_advance_loc: 4 to 0000000000013da3
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000013de4
+  DW_CFA_advance_loc: 1 to 0000000000013da4
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc2: 398 to 0000000000013f72
+  DW_CFA_advance_loc2: 398 to 0000000000013f32
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 0000000000013f73
+  DW_CFA_advance_loc: 1 to 0000000000013f33
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000013f75
+  DW_CFA_advance_loc: 2 to 0000000000013f35
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000013f77
+  DW_CFA_advance_loc: 2 to 0000000000013f37
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000013f79
+  DW_CFA_advance_loc: 2 to 0000000000013f39
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000013f7a
+  DW_CFA_advance_loc: 1 to 0000000000013f3a
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_restore: r13 (r13)
   DW_CFA_restore: r14 (r14)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001258 0000000000000040 0000125c FDE cie=00000000 pc=0000000000012ba0..0000000000012f3e
-  DW_CFA_advance_loc: 2 to 0000000000012ba2
+00001250 0000000000000040 00001254 FDE cie=00000000 pc=0000000000012b60..0000000000012efe
+  DW_CFA_advance_loc: 2 to 0000000000012b62
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 5 to 0000000000012ba7
+  DW_CFA_advance_loc: 5 to 0000000000012b67
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000012ba9
+  DW_CFA_advance_loc: 2 to 0000000000012b69
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 9 to 0000000000012bb2
+  DW_CFA_advance_loc: 9 to 0000000000012b72
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 5 to 0000000000012bb7
+  DW_CFA_advance_loc: 5 to 0000000000012b77
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc: 7 to 0000000000012bbe
+  DW_CFA_advance_loc: 7 to 0000000000012b7e
   DW_CFA_def_cfa_offset: 64
-  DW_CFA_advance_loc1: 218 to 0000000000012c98
+  DW_CFA_advance_loc1: 218 to 0000000000012c58
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000012c99
+  DW_CFA_advance_loc: 1 to 0000000000012c59
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 0000000000012c9a
+  DW_CFA_advance_loc: 1 to 0000000000012c5a
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000012c9c
+  DW_CFA_advance_loc: 2 to 0000000000012c5c
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000012c9e
+  DW_CFA_advance_loc: 2 to 0000000000012c5e
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000012ca0
+  DW_CFA_advance_loc: 2 to 0000000000012c60
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 0000000000012ca8
+  DW_CFA_advance_loc: 8 to 0000000000012c68
   DW_CFA_restore_state
   DW_CFA_nop
 
-0000129c 0000000000000040 000012a0 FDE cie=00000000 pc=0000000000013f80..000000000001412b
-  DW_CFA_advance_loc: 18 to 0000000000013f92
+00001294 0000000000000040 00001298 FDE cie=00000000 pc=0000000000013f40..00000000000140eb
+  DW_CFA_advance_loc: 18 to 0000000000013f52
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 5 to 0000000000013f97
+  DW_CFA_advance_loc: 5 to 0000000000013f57
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 6 to 0000000000013f9d
+  DW_CFA_advance_loc: 6 to 0000000000013f5d
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 4 to 0000000000013fa1
+  DW_CFA_advance_loc: 4 to 0000000000013f61
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000013fa2
+  DW_CFA_advance_loc: 1 to 0000000000013f62
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc2: 384 to 0000000000014122
+  DW_CFA_advance_loc2: 384 to 00000000000140e2
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 0000000000014123
+  DW_CFA_advance_loc: 1 to 00000000000140e3
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000014125
+  DW_CFA_advance_loc: 2 to 00000000000140e5
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000014127
+  DW_CFA_advance_loc: 2 to 00000000000140e7
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000014129
+  DW_CFA_advance_loc: 2 to 00000000000140e9
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000000000001412a
+  DW_CFA_advance_loc: 1 to 00000000000140ea
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_restore: r13 (r13)
   DW_CFA_restore: r14 (r14)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000012e0 0000000000000040 000012e4 FDE cie=00000000 pc=0000000000012f40..00000000000132bd
-  DW_CFA_advance_loc: 2 to 0000000000012f42
+000012d8 0000000000000040 000012dc FDE cie=00000000 pc=0000000000012f00..000000000001327d
+  DW_CFA_advance_loc: 2 to 0000000000012f02
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 5 to 0000000000012f47
+  DW_CFA_advance_loc: 5 to 0000000000012f07
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000012f49
+  DW_CFA_advance_loc: 2 to 0000000000012f09
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 9 to 0000000000012f52
+  DW_CFA_advance_loc: 9 to 0000000000012f12
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 5 to 0000000000012f57
+  DW_CFA_advance_loc: 5 to 0000000000012f17
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc: 7 to 0000000000012f5e
+  DW_CFA_advance_loc: 7 to 0000000000012f1e
   DW_CFA_def_cfa_offset: 64
-  DW_CFA_advance_loc1: 201 to 0000000000013027
+  DW_CFA_advance_loc1: 201 to 0000000000012fe7
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000013028
+  DW_CFA_advance_loc: 1 to 0000000000012fe8
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 0000000000013029
+  DW_CFA_advance_loc: 1 to 0000000000012fe9
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000001302b
+  DW_CFA_advance_loc: 2 to 0000000000012feb
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000001302d
+  DW_CFA_advance_loc: 2 to 0000000000012fed
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000001302f
+  DW_CFA_advance_loc: 2 to 0000000000012fef
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000013030
+  DW_CFA_advance_loc: 1 to 0000000000012ff0
   DW_CFA_restore_state
   DW_CFA_nop
 
-00001324 0000000000000044 00001328 FDE cie=00000000 pc=0000000000014130..00000000000142e2
-  DW_CFA_advance_loc: 18 to 0000000000014142
+0000131c 0000000000000044 00001320 FDE cie=00000000 pc=00000000000140f0..00000000000142a2
+  DW_CFA_advance_loc: 18 to 0000000000014102
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 8 to 000000000001414a
+  DW_CFA_advance_loc: 8 to 000000000001410a
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 5 to 000000000001414f
+  DW_CFA_advance_loc: 5 to 000000000001410f
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 1 to 0000000000014150
+  DW_CFA_advance_loc: 1 to 0000000000014110
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 5 to 0000000000014155
+  DW_CFA_advance_loc: 5 to 0000000000014115
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc2: 361 to 00000000000142be
+  DW_CFA_advance_loc2: 361 to 000000000001427e
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 00000000000142bf
+  DW_CFA_advance_loc: 1 to 000000000001427f
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000142c1
+  DW_CFA_advance_loc: 2 to 0000000000014281
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000142c3
+  DW_CFA_advance_loc: 2 to 0000000000014283
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000142c5
+  DW_CFA_advance_loc: 2 to 0000000000014285
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 00000000000142c6
+  DW_CFA_advance_loc: 1 to 0000000000014286
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 27 to 00000000000142e1
+  DW_CFA_advance_loc: 27 to 00000000000142a1
   DW_CFA_def_cfa_offset: 8
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_restore: r13 (r13)
   DW_CFA_restore: r14 (r14)
   DW_CFA_nop
   DW_CFA_nop
 
-0000136c 0000000000000048 00001370 FDE cie=00000000 pc=00000000000132c0..00000000000135c6
-  DW_CFA_advance_loc: 2 to 00000000000132c2
+00001364 0000000000000048 00001368 FDE cie=00000000 pc=0000000000013280..0000000000013586
+  DW_CFA_advance_loc: 2 to 0000000000013282
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 5 to 00000000000132c7
+  DW_CFA_advance_loc: 5 to 0000000000013287
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 00000000000132c9
+  DW_CFA_advance_loc: 2 to 0000000000013289
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 10 to 00000000000132d3
+  DW_CFA_advance_loc: 10 to 0000000000013293
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 5 to 00000000000132d8
+  DW_CFA_advance_loc: 5 to 0000000000013298
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 00000000000132d9
+  DW_CFA_advance_loc: 1 to 0000000000013299
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 00000000000132e0
+  DW_CFA_advance_loc: 7 to 00000000000132a0
   DW_CFA_def_cfa_offset: 64
-  DW_CFA_advance_loc1: 178 to 0000000000013392
+  DW_CFA_advance_loc1: 178 to 0000000000013352
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000013393
+  DW_CFA_advance_loc: 1 to 0000000000013353
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000013394
+  DW_CFA_advance_loc: 1 to 0000000000013354
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000013396
+  DW_CFA_advance_loc: 2 to 0000000000013356
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000013398
+  DW_CFA_advance_loc: 2 to 0000000000013358
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000001339a
+  DW_CFA_advance_loc: 2 to 000000000001335a
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000001339c
+  DW_CFA_advance_loc: 2 to 000000000001335c
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 4 to 00000000000133a0
+  DW_CFA_advance_loc: 4 to 0000000000013360
   DW_CFA_restore_state
   DW_CFA_nop
 
-000013b8 0000000000000044 000013bc FDE cie=00000000 pc=00000000000142f0..00000000000144b3
-  DW_CFA_advance_loc: 20 to 0000000000014304
+000013b0 0000000000000044 000013b4 FDE cie=00000000 pc=00000000000142b0..0000000000014473
+  DW_CFA_advance_loc: 20 to 00000000000142c4
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 8 to 000000000001430c
+  DW_CFA_advance_loc: 8 to 00000000000142cc
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 5 to 0000000000014311
+  DW_CFA_advance_loc: 5 to 00000000000142d1
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 1 to 0000000000014312
+  DW_CFA_advance_loc: 1 to 00000000000142d2
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 5 to 0000000000014317
+  DW_CFA_advance_loc: 5 to 00000000000142d7
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc2: 375 to 000000000001448e
+  DW_CFA_advance_loc2: 375 to 000000000001444e
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 000000000001448f
+  DW_CFA_advance_loc: 1 to 000000000001444f
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000014491
+  DW_CFA_advance_loc: 2 to 0000000000014451
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000014493
+  DW_CFA_advance_loc: 2 to 0000000000014453
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000014495
+  DW_CFA_advance_loc: 2 to 0000000000014455
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000014496
+  DW_CFA_advance_loc: 1 to 0000000000014456
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 28 to 00000000000144b2
+  DW_CFA_advance_loc: 28 to 0000000000014472
   DW_CFA_def_cfa_offset: 8
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
   DW_CFA_restore: r12 (r12)
   DW_CFA_restore: r13 (r13)
   DW_CFA_restore: r14 (r14)
   DW_CFA_nop
   DW_CFA_nop
 
-00001400 000000000000004c 00001404 FDE cie=00000000 pc=00000000000135d0..0000000000013912
-  DW_CFA_advance_loc: 2 to 00000000000135d2
+000013f8 000000000000004c 000013fc FDE cie=00000000 pc=0000000000013590..00000000000138d2
+  DW_CFA_advance_loc: 2 to 0000000000013592
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 5 to 00000000000135d7
+  DW_CFA_advance_loc: 5 to 0000000000013597
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 00000000000135d9
+  DW_CFA_advance_loc: 2 to 0000000000013599
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 10 to 00000000000135e3
+  DW_CFA_advance_loc: 10 to 00000000000135a3
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 5 to 00000000000135e8
+  DW_CFA_advance_loc: 5 to 00000000000135a8
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 00000000000135e9
+  DW_CFA_advance_loc: 1 to 00000000000135a9
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 00000000000135f0
+  DW_CFA_advance_loc: 7 to 00000000000135b0
   DW_CFA_def_cfa_offset: 64
-  DW_CFA_advance_loc1: 188 to 00000000000136ac
+  DW_CFA_advance_loc1: 188 to 000000000001366c
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 00000000000136ad
+  DW_CFA_advance_loc: 1 to 000000000001366d
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000136ae
+  DW_CFA_advance_loc: 1 to 000000000001366e
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000136b0
+  DW_CFA_advance_loc: 2 to 0000000000013670
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000136b2
+  DW_CFA_advance_loc: 2 to 0000000000013672
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000136b4
+  DW_CFA_advance_loc: 2 to 0000000000013674
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000136b6
+  DW_CFA_advance_loc: 2 to 0000000000013676
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 10 to 00000000000136c0
+  DW_CFA_advance_loc: 10 to 0000000000013680
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001450 0000000000000048 00001454 FDE cie=00000000 pc=00000000000144c0..0000000000014c4c
-  DW_CFA_advance_loc: 2 to 00000000000144c2
+00001448 0000000000000048 0000144c FDE cie=00000000 pc=0000000000014480..0000000000014c0c
+  DW_CFA_advance_loc: 2 to 0000000000014482
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 00000000000144c4
+  DW_CFA_advance_loc: 2 to 0000000000014484
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 00000000000144c6
+  DW_CFA_advance_loc: 2 to 0000000000014486
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 00000000000144c8
+  DW_CFA_advance_loc: 2 to 0000000000014488
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 00000000000144c9
+  DW_CFA_advance_loc: 1 to 0000000000014489
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 00000000000144ca
+  DW_CFA_advance_loc: 1 to 000000000001448a
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 4 to 00000000000144ce
+  DW_CFA_advance_loc: 4 to 000000000001448e
   DW_CFA_def_cfa_offset: 104
-  DW_CFA_advance_loc2: 1828 to 0000000000014bf2
+  DW_CFA_advance_loc2: 1828 to 0000000000014bb2
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000014bf3
+  DW_CFA_advance_loc: 1 to 0000000000014bb3
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000014bf4
+  DW_CFA_advance_loc: 1 to 0000000000014bb4
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000014bf6
+  DW_CFA_advance_loc: 2 to 0000000000014bb6
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000014bf8
+  DW_CFA_advance_loc: 2 to 0000000000014bb8
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000014bfa
+  DW_CFA_advance_loc: 2 to 0000000000014bba
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000014bfc
+  DW_CFA_advance_loc: 2 to 0000000000014bbc
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000014bfd
+  DW_CFA_advance_loc: 1 to 0000000000014bbd
   DW_CFA_restore_state
 
-0000149c 0000000000000050 000014a0 FDE cie=00000000 pc=0000000000014c50..0000000000015744
-  DW_CFA_advance_loc: 2 to 0000000000014c52
+00001494 0000000000000050 00001498 FDE cie=00000000 pc=0000000000014c10..0000000000015704
+  DW_CFA_advance_loc: 2 to 0000000000014c12
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000014c54
+  DW_CFA_advance_loc: 2 to 0000000000014c14
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000014c56
+  DW_CFA_advance_loc: 2 to 0000000000014c16
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 0000000000014c58
+  DW_CFA_advance_loc: 2 to 0000000000014c18
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000014c59
+  DW_CFA_advance_loc: 1 to 0000000000014c19
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 0000000000014c5a
+  DW_CFA_advance_loc: 1 to 0000000000014c1a
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 0000000000014c61
+  DW_CFA_advance_loc: 7 to 0000000000014c21
   DW_CFA_def_cfa_offset: 296
-  DW_CFA_advance_loc2: 2675 to 00000000000156d4
+  DW_CFA_advance_loc2: 2675 to 0000000000015694
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 00000000000156d5
+  DW_CFA_advance_loc: 1 to 0000000000015695
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000156d6
+  DW_CFA_advance_loc: 1 to 0000000000015696
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000156d8
+  DW_CFA_advance_loc: 2 to 0000000000015698
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000156da
+  DW_CFA_advance_loc: 2 to 000000000001569a
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000156dc
+  DW_CFA_advance_loc: 2 to 000000000001569c
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000156de
+  DW_CFA_advance_loc: 2 to 000000000001569e
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 00000000000156df
+  DW_CFA_advance_loc: 1 to 000000000001569f
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000014f0 0000000000000048 000014f4 FDE cie=00000000 pc=0000000000015750..00000000000158ce
-  DW_CFA_advance_loc: 12 to 000000000001575c
+000014e8 0000000000000048 000014ec FDE cie=00000000 pc=0000000000015710..000000000001588e
+  DW_CFA_advance_loc: 12 to 000000000001571c
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 000000000001575e
+  DW_CFA_advance_loc: 2 to 000000000001571e
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000015760
+  DW_CFA_advance_loc: 2 to 0000000000015720
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 0000000000015762
+  DW_CFA_advance_loc: 2 to 0000000000015722
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000015763
+  DW_CFA_advance_loc: 1 to 0000000000015723
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 0000000000015764
+  DW_CFA_advance_loc: 1 to 0000000000015724
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 000000000001576b
+  DW_CFA_advance_loc: 7 to 000000000001572b
   DW_CFA_def_cfa_offset: 112
-  DW_CFA_advance_loc2: 340 to 00000000000158bf
+  DW_CFA_advance_loc2: 340 to 000000000001587f
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 00000000000158c0
+  DW_CFA_advance_loc: 1 to 0000000000015880
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 5 to 00000000000158c5
+  DW_CFA_advance_loc: 5 to 0000000000015885
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000158c7
+  DW_CFA_advance_loc: 2 to 0000000000015887
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000158c9
+  DW_CFA_advance_loc: 2 to 0000000000015889
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000158cb
+  DW_CFA_advance_loc: 2 to 000000000001588b
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000158cd
+  DW_CFA_advance_loc: 2 to 000000000001588d
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000153c 0000000000000020 00000000 CIE
+00001534 0000000000000020 00000000 CIE
   Version:               1
   Augmentation:          "zR"
   Code alignment factor: 1
   Data alignment factor: -8
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
@@ -2403,103 +2396,103 @@
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
 
-00001560 0000000000000010 00000028 FDE cie=0000153c pc=0000000000003332..0000000000003337
+00001558 0000000000000010 00000028 FDE cie=00001534 pc=0000000000003332..0000000000003337
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001574 0000000000000048 00001578 FDE cie=00000000 pc=00000000000158d0..0000000000015a04
-  DW_CFA_advance_loc: 12 to 00000000000158dc
+0000156c 0000000000000048 00001570 FDE cie=00000000 pc=0000000000015890..00000000000159c4
+  DW_CFA_advance_loc: 12 to 000000000001589c
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 00000000000158de
+  DW_CFA_advance_loc: 2 to 000000000001589e
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 00000000000158e0
+  DW_CFA_advance_loc: 2 to 00000000000158a0
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 5 to 00000000000158e5
+  DW_CFA_advance_loc: 5 to 00000000000158a5
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 00000000000158e6
+  DW_CFA_advance_loc: 1 to 00000000000158a6
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 00000000000158e7
+  DW_CFA_advance_loc: 1 to 00000000000158a7
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 4 to 00000000000158eb
+  DW_CFA_advance_loc: 4 to 00000000000158ab
   DW_CFA_def_cfa_offset: 112
-  DW_CFA_advance_loc2: 266 to 00000000000159f5
+  DW_CFA_advance_loc2: 266 to 00000000000159b5
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 00000000000159f6
+  DW_CFA_advance_loc: 1 to 00000000000159b6
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 5 to 00000000000159fb
+  DW_CFA_advance_loc: 5 to 00000000000159bb
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000159fd
+  DW_CFA_advance_loc: 2 to 00000000000159bd
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000159ff
+  DW_CFA_advance_loc: 2 to 00000000000159bf
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000015a01
+  DW_CFA_advance_loc: 2 to 00000000000159c1
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000015a03
+  DW_CFA_advance_loc: 2 to 00000000000159c3
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000015c0 0000000000000010 00000088 FDE cie=0000153c pc=0000000000003337..000000000000333c
+000015b8 0000000000000010 00000088 FDE cie=00001534 pc=0000000000003337..000000000000333c
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000015d4 0000000000000048 000015d8 FDE cie=00000000 pc=0000000000015a10..0000000000015b89
-  DW_CFA_advance_loc: 12 to 0000000000015a1c
+000015cc 0000000000000048 000015d0 FDE cie=00000000 pc=00000000000159d0..0000000000015b49
+  DW_CFA_advance_loc: 12 to 00000000000159dc
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000015a1e
+  DW_CFA_advance_loc: 2 to 00000000000159de
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000015a20
+  DW_CFA_advance_loc: 2 to 00000000000159e0
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 0000000000015a22
+  DW_CFA_advance_loc: 2 to 00000000000159e2
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000015a23
+  DW_CFA_advance_loc: 1 to 00000000000159e3
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 0000000000015a24
+  DW_CFA_advance_loc: 1 to 00000000000159e4
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 0000000000015a2b
+  DW_CFA_advance_loc: 7 to 00000000000159eb
   DW_CFA_def_cfa_offset: 96
-  DW_CFA_advance_loc2: 336 to 0000000000015b7b
+  DW_CFA_advance_loc2: 336 to 0000000000015b3b
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000015b7c
+  DW_CFA_advance_loc: 1 to 0000000000015b3c
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 4 to 0000000000015b80
+  DW_CFA_advance_loc: 4 to 0000000000015b40
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000015b82
+  DW_CFA_advance_loc: 2 to 0000000000015b42
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000015b84
+  DW_CFA_advance_loc: 2 to 0000000000015b44
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000015b86
+  DW_CFA_advance_loc: 2 to 0000000000015b46
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000015b88
+  DW_CFA_advance_loc: 2 to 0000000000015b48
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001620 0000000000000020 00000000 CIE
+00001618 0000000000000020 00000000 CIE
   Version:               1
   Augmentation:          "zR"
   Code alignment factor: 1
   Data alignment factor: -8
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
@@ -2508,295 +2501,295 @@
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
 
-00001644 0000000000000010 00000028 FDE cie=00001620 pc=000000000000333c..0000000000003341
+0000163c 0000000000000010 00000028 FDE cie=00001618 pc=000000000000333c..0000000000003341
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001658 0000000000000010 0000165c FDE cie=00000000 pc=0000000000015b90..0000000000015b96
+00001650 0000000000000010 00001654 FDE cie=00000000 pc=0000000000015b50..0000000000015b56
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000166c 0000000000000010 00001670 FDE cie=00000000 pc=0000000000015ba0..0000000000015ba6
+00001664 0000000000000010 00001668 FDE cie=00000000 pc=0000000000015b60..0000000000015b66
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001680 0000000000000014 00001684 FDE cie=00000000 pc=0000000000015bb0..0000000000015bb3
+00001678 0000000000000014 0000167c FDE cie=00000000 pc=0000000000015b70..0000000000015b73
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001698 0000000000000014 0000169c FDE cie=00000000 pc=0000000000015bc0..0000000000015bde
-  DW_CFA_advance_loc: 4 to 0000000000015bc4
+00001690 0000000000000014 00001694 FDE cie=00000000 pc=0000000000015b80..0000000000015b9e
+  DW_CFA_advance_loc: 4 to 0000000000015b84
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 25 to 0000000000015bdd
+  DW_CFA_advance_loc: 25 to 0000000000015b9d
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
 
-000016b0 000000000000002c 000016b4 FDE cie=00000000 pc=0000000000015be0..0000000000015e2f
-  DW_CFA_advance_loc: 1 to 0000000000015be1
+000016a8 000000000000002c 000016ac FDE cie=00000000 pc=0000000000015ba0..0000000000015def
+  DW_CFA_advance_loc: 1 to 0000000000015ba1
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000015be4
+  DW_CFA_advance_loc: 3 to 0000000000015ba4
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 2 to 0000000000015be6
+  DW_CFA_advance_loc: 2 to 0000000000015ba6
   DW_CFA_offset: r15 (r15) at cfa-24
-  DW_CFA_advance_loc: 7 to 0000000000015bed
+  DW_CFA_advance_loc: 7 to 0000000000015bad
   DW_CFA_offset: r14 (r14) at cfa-32
   DW_CFA_offset: r13 (r13) at cfa-40
-  DW_CFA_advance_loc: 7 to 0000000000015bf4
+  DW_CFA_advance_loc: 7 to 0000000000015bb4
   DW_CFA_offset: r12 (r12) at cfa-48
-  DW_CFA_advance_loc: 15 to 0000000000015c03
+  DW_CFA_advance_loc: 15 to 0000000000015bc3
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc2: 481 to 0000000000015de4
+  DW_CFA_advance_loc2: 481 to 0000000000015da4
   DW_CFA_remember_state
   DW_CFA_def_cfa: r7 (rsp) ofs 8
-  DW_CFA_advance_loc: 4 to 0000000000015de8
+  DW_CFA_advance_loc: 4 to 0000000000015da8
   DW_CFA_restore_state
 
-000016e0 0000000000000030 000016e4 FDE cie=00000000 pc=0000000000015e30..0000000000015ff0
-  DW_CFA_advance_loc: 45 to 0000000000015e5d
+000016d8 0000000000000030 000016dc FDE cie=00000000 pc=0000000000015df0..0000000000015fb0
+  DW_CFA_advance_loc: 45 to 0000000000015e1d
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 8 to 0000000000015e65
+  DW_CFA_advance_loc: 8 to 0000000000015e25
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r3 (rbx) at cfa-24
-  DW_CFA_advance_loc2: 377 to 0000000000015fde
+  DW_CFA_advance_loc2: 377 to 0000000000015f9e
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 0000000000015fdf
+  DW_CFA_advance_loc: 1 to 0000000000015f9f
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000015fe0
+  DW_CFA_advance_loc: 1 to 0000000000015fa0
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 4 to 0000000000015fe4
+  DW_CFA_advance_loc: 4 to 0000000000015fa4
   DW_CFA_def_cfa_offset: 8
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
-  DW_CFA_advance_loc: 1 to 0000000000015fe5
+  DW_CFA_advance_loc: 1 to 0000000000015fa5
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r3 (rbx) at cfa-24
   DW_CFA_offset: r6 (rbp) at cfa-16
   DW_CFA_nop
   DW_CFA_nop
 
-00001714 0000000000000030 00001718 FDE cie=00000000 pc=0000000000015ff0..00000000000161ea
-  DW_CFA_advance_loc: 48 to 0000000000016020
+0000170c 0000000000000030 00001710 FDE cie=00000000 pc=0000000000015fb0..00000000000161aa
+  DW_CFA_advance_loc: 48 to 0000000000015fe0
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 11 to 000000000001602b
+  DW_CFA_advance_loc: 11 to 0000000000015feb
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r3 (rbx) at cfa-24
-  DW_CFA_advance_loc2: 420 to 00000000000161cf
+  DW_CFA_advance_loc2: 420 to 000000000001618f
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00000000000161d0
+  DW_CFA_advance_loc: 1 to 0000000000016190
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 00000000000161d1
+  DW_CFA_advance_loc: 1 to 0000000000016191
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 4 to 00000000000161d5
+  DW_CFA_advance_loc: 4 to 0000000000016195
   DW_CFA_def_cfa_offset: 8
   DW_CFA_restore: r3 (rbx)
   DW_CFA_restore: r6 (rbp)
-  DW_CFA_advance_loc: 1 to 00000000000161d6
+  DW_CFA_advance_loc: 1 to 0000000000016196
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r3 (rbx) at cfa-24
   DW_CFA_offset: r6 (rbp) at cfa-16
   DW_CFA_nop
   DW_CFA_nop
 
-00001748 0000000000000010 0000174c FDE cie=00000000 pc=00000000000161f0..00000000000161fe
+00001740 0000000000000010 00001744 FDE cie=00000000 pc=00000000000161b0..00000000000161be
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000175c 0000000000000010 00001760 FDE cie=00000000 pc=0000000000016c20..0000000000016d20
+00001754 0000000000000010 00001758 FDE cie=00000000 pc=0000000000016be0..0000000000016ce0
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001770 000000000000004c 00001774 FDE cie=00000000 pc=0000000000016200..00000000000166e6
-  DW_CFA_advance_loc: 2 to 0000000000016202
+00001768 000000000000004c 0000176c FDE cie=00000000 pc=00000000000161c0..00000000000166a6
+  DW_CFA_advance_loc: 2 to 00000000000161c2
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 6 to 0000000000016208
+  DW_CFA_advance_loc: 6 to 00000000000161c8
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 000000000001620a
+  DW_CFA_advance_loc: 2 to 00000000000161ca
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 000000000001620c
+  DW_CFA_advance_loc: 2 to 00000000000161cc
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000001620d
+  DW_CFA_advance_loc: 1 to 00000000000161cd
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 000000000001620e
+  DW_CFA_advance_loc: 1 to 00000000000161ce
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 4 to 0000000000016212
+  DW_CFA_advance_loc: 4 to 00000000000161d2
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc2: 1101 to 000000000001665f
+  DW_CFA_advance_loc2: 1101 to 000000000001661f
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000016660
+  DW_CFA_advance_loc: 1 to 0000000000016620
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000016661
+  DW_CFA_advance_loc: 1 to 0000000000016621
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000016663
+  DW_CFA_advance_loc: 2 to 0000000000016623
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000016665
+  DW_CFA_advance_loc: 2 to 0000000000016625
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000016667
+  DW_CFA_advance_loc: 2 to 0000000000016627
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000016669
+  DW_CFA_advance_loc: 2 to 0000000000016629
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000000000001666a
+  DW_CFA_advance_loc: 1 to 000000000001662a
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000017c0 000000000000004c 000017c4 FDE cie=00000000 pc=00000000000166f0..0000000000016c18
-  DW_CFA_advance_loc: 13 to 00000000000166fd
+000017b8 000000000000004c 000017bc FDE cie=00000000 pc=00000000000166b0..0000000000016bd8
+  DW_CFA_advance_loc: 13 to 00000000000166bd
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 6 to 0000000000016703
+  DW_CFA_advance_loc: 6 to 00000000000166c3
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 10 to 000000000001670d
+  DW_CFA_advance_loc: 10 to 00000000000166cd
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 6 to 0000000000016713
+  DW_CFA_advance_loc: 6 to 00000000000166d3
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 9 to 000000000001671c
+  DW_CFA_advance_loc: 9 to 00000000000166dc
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 000000000001671d
+  DW_CFA_advance_loc: 1 to 00000000000166dd
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 4 to 0000000000016721
+  DW_CFA_advance_loc: 4 to 00000000000166e1
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc2: 1134 to 0000000000016b8f
+  DW_CFA_advance_loc2: 1134 to 0000000000016b4f
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000016b90
+  DW_CFA_advance_loc: 1 to 0000000000016b50
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000016b91
+  DW_CFA_advance_loc: 1 to 0000000000016b51
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000016b93
+  DW_CFA_advance_loc: 2 to 0000000000016b53
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000016b95
+  DW_CFA_advance_loc: 2 to 0000000000016b55
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000016b97
+  DW_CFA_advance_loc: 2 to 0000000000016b57
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000016b99
+  DW_CFA_advance_loc: 2 to 0000000000016b59
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000016b9a
+  DW_CFA_advance_loc: 1 to 0000000000016b5a
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001810 000000000000004c 00001814 FDE cie=00000000 pc=0000000000016d20..0000000000016fe5
-  DW_CFA_advance_loc: 2 to 0000000000016d22
+00001808 000000000000004c 0000180c FDE cie=00000000 pc=0000000000016ce0..0000000000016fa5
+  DW_CFA_advance_loc: 2 to 0000000000016ce2
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 5 to 0000000000016d27
+  DW_CFA_advance_loc: 5 to 0000000000016ce7
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 5 to 0000000000016d2c
+  DW_CFA_advance_loc: 5 to 0000000000016cec
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 5 to 0000000000016d31
+  DW_CFA_advance_loc: 5 to 0000000000016cf1
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000016d32
+  DW_CFA_advance_loc: 1 to 0000000000016cf2
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 0000000000016d33
+  DW_CFA_advance_loc: 1 to 0000000000016cf3
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 4 to 0000000000016d37
+  DW_CFA_advance_loc: 4 to 0000000000016cf7
   DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc2: 550 to 0000000000016f5d
+  DW_CFA_advance_loc2: 550 to 0000000000016f1d
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 0000000000016f61
+  DW_CFA_advance_loc: 4 to 0000000000016f21
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000016f62
+  DW_CFA_advance_loc: 1 to 0000000000016f22
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000016f64
+  DW_CFA_advance_loc: 2 to 0000000000016f24
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000016f66
+  DW_CFA_advance_loc: 2 to 0000000000016f26
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000016f68
+  DW_CFA_advance_loc: 2 to 0000000000016f28
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000016f6a
+  DW_CFA_advance_loc: 2 to 0000000000016f2a
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 5 to 0000000000016f6f
+  DW_CFA_advance_loc: 5 to 0000000000016f2f
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00001860 000000000000004c 00001864 FDE cie=00000000 pc=0000000000016ff0..00000000000172b1
-  DW_CFA_advance_loc: 2 to 0000000000016ff2
+00001858 000000000000004c 0000185c FDE cie=00000000 pc=0000000000016fb0..0000000000017271
+  DW_CFA_advance_loc: 2 to 0000000000016fb2
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 5 to 0000000000016ff7
+  DW_CFA_advance_loc: 5 to 0000000000016fb7
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 5 to 0000000000016ffc
+  DW_CFA_advance_loc: 5 to 0000000000016fbc
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 5 to 0000000000017001
+  DW_CFA_advance_loc: 5 to 0000000000016fc1
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000017002
+  DW_CFA_advance_loc: 1 to 0000000000016fc2
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 0000000000017003
+  DW_CFA_advance_loc: 1 to 0000000000016fc3
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 4 to 0000000000017007
+  DW_CFA_advance_loc: 4 to 0000000000016fc7
   DW_CFA_def_cfa_offset: 128
-  DW_CFA_advance_loc2: 550 to 000000000001722d
+  DW_CFA_advance_loc2: 550 to 00000000000171ed
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 0000000000017231
+  DW_CFA_advance_loc: 4 to 00000000000171f1
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000017232
+  DW_CFA_advance_loc: 1 to 00000000000171f2
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000017234
+  DW_CFA_advance_loc: 2 to 00000000000171f4
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000017236
+  DW_CFA_advance_loc: 2 to 00000000000171f6
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000017238
+  DW_CFA_advance_loc: 2 to 00000000000171f8
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000001723a
+  DW_CFA_advance_loc: 2 to 00000000000171fa
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 5 to 000000000001723f
+  DW_CFA_advance_loc: 5 to 00000000000171ff
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000018b0 0000000000000010 000018b4 FDE cie=00000000 pc=0000000000003380..0000000000003393
+000018a8 0000000000000010 000018ac FDE cie=00000000 pc=0000000000003380..0000000000003393
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000018c4 ZERO terminator
+000018bc ZERO terminator
```

#### strings --all --bytes=8 {}

```diff
@@ -134,15 +134,15 @@
 AWAVAUATUSH
 []A\A]A^A_
 []A\A]A^A_
 []A\A]A^A_
 []A\A]A^A_
 []A\A]A^A_
 AUATUSHc
-h[]A\A]A^A_
+([]A\A]A^A_
 []A\A]A^A_
 []A\A]A^
 []A\A]A^
 AWAVAUMc
 []A\A]A^A_
 []A\A]A^A_
 AWAVAUMc
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt {}

```diff
@@ -30,30 +30,30 @@
 
 0000000000003070 <randd()@plt>:
 	jmp    *0x18fc2(%rip)        
 	push   $0x4
 	jmp    3020 <.plt>
 
 0000000000003080 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)@plt>:
-	jmp    *0x18fba(%rip)        # 1c040 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)@@Base+0x80c0>
+	jmp    *0x18fba(%rip)        # 1c040 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)@@Base+0x8100>
 	push   $0x5
 	jmp    3020 <.plt>
 
 0000000000003090 <omp_get_num_threads()@plt>:
 	jmp    *0x18fb2(%rip)        
 	push   $0x6
 	jmp    3020 <.plt>
 
 00000000000030a0 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)@plt>:
-	jmp    *0x18faa(%rip)        # 1c050 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)@@Base+0xdf20>
+	jmp    *0x18faa(%rip)        # 1c050 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)@@Base+0xdf60>
 	push   $0x7
 	jmp    3020 <.plt>
 
 00000000000030b0 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)@plt>:
-	jmp    *0x18fa2(%rip)        # 1c058 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)@@Base+0xde68>
+	jmp    *0x18fa2(%rip)        # 1c058 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)@@Base+0xdea8>
 	push   $0x8
 	jmp    3020 <.plt>
 
 00000000000030c0 <fast_cosf@plt>:
 	jmp    *0x18f9a(%rip)        
 	push   $0x9
 	jmp    3020 <.plt>
@@ -95,15 +95,15 @@
 
 0000000000003140 <srand@plt>:
 	jmp    *0x18f5a(%rip)        
 	push   $0x11
 	jmp    3020 <.plt>
 
 0000000000003150 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)@plt>:
-	jmp    *0x18f52(%rip)        # 1c0a8 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)@@Base+0x7f78>
+	jmp    *0x18f52(%rip)        # 1c0a8 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)@@Base+0x7fb8>
 	push   $0x12
 	jmp    3020 <.plt>
 
 0000000000003160 <operator new(unsigned long)@plt>:
 	jmp    *0x18f4a(%rip)        
 	push   $0x13
 	jmp    3020 <.plt>
@@ -135,15 +135,15 @@
 
 00000000000031c0 <omp_get_max_threads()@plt>:
 	jmp    *0x18f1a(%rip)        
 	push   $0x19
 	jmp    3020 <.plt>
 
 00000000000031d0 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)@plt>:
-	jmp    *0x18f12(%rip)        # 1c0e8 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)@@Base+0xde38>
+	jmp    *0x18f12(%rip)        # 1c0e8 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)@@Base+0xde78>
 	push   $0x1a
 	jmp    3020 <.plt>
 
 00000000000031e0 <std::ios_base::Init::Init()@plt>:
 	jmp    *0x18f0a(%rip)        
 	push   $0x1b
 	jmp    3020 <.plt>
@@ -155,15 +155,15 @@
 
 0000000000003200 <meanf@plt>:
 	jmp    *0x18efa(%rip)        
 	push   $0x1d
 	jmp    3020 <.plt>
 
 0000000000003210 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)@plt>:
-	jmp    *0x18ef2(%rip)        # 1c108 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)@@Base+0xdd08>
+	jmp    *0x18ef2(%rip)        # 1c108 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)@@Base+0xdd48>
 	push   $0x1e
 	jmp    3020 <.plt>
 
 0000000000003220 <fast_sin@plt>:
 	jmp    *0x18eea(%rip)        
 	push   $0x1f
 	jmp    3020 <.plt>
@@ -175,40 +175,40 @@
 
 0000000000003240 <__tls_get_addr@plt>:
 	jmp    *0x18eda(%rip)        
 	push   $0x21
 	jmp    3020 <.plt>
 
 0000000000003250 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)@plt>:
-	jmp    *0x18ed2(%rip)        # 1c128 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)@@Base+0x8368>
+	jmp    *0x18ed2(%rip)        # 1c128 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)@@Base+0x83a8>
 	push   $0x22
 	jmp    3020 <.plt>
 
 0000000000003260 <_Unwind_Resume@plt>:
 	jmp    *0x18eca(%rip)        
 	push   $0x23
 	jmp    3020 <.plt>
 
 0000000000003270 <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()@plt>:
-	jmp    *0x18ec2(%rip)        # 1c138 <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()@@Base+0x5518>
+	jmp    *0x18ec2(%rip)        # 1c138 <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()@@Base+0x5558>
 	push   $0x24
 	jmp    3020 <.plt>
 
 0000000000003280 <trapz_const_delta@plt>:
 	jmp    *0x18eba(%rip)        
 	push   $0x25
 	jmp    3020 <.plt>
 
 0000000000003290 <fast_sinf@plt>:
 	jmp    *0x18eb2(%rip)        
 	push   $0x26
 	jmp    3020 <.plt>
 
 00000000000032a0 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)@plt>:
-	jmp    *0x18eaa(%rip)        # 1c150 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)@@Base+0x7e60>
+	jmp    *0x18eaa(%rip)        # 1c150 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)@@Base+0x7ea0>
 	push   $0x27
 	jmp    3020 <.plt>
 
 00000000000032b0 <trapz_const_deltaf@plt>:
 	jmp    *0x18ea2(%rip)        
 	push   $0x28
 	jmp    3020 <.plt>
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -5755,15 +5755,15 @@
 	mov    %edx,%r14d
 	push   %r13
 	push   %r12
 	push   %rbp
 	divsd  %xmm1,%xmm4
 	push   %rbx
 	xor    %ebx,%ebx
-	sub    $0x88,%rsp
+	sub    $0x48,%rsp
 	mov    %rsi,0x30(%rsp)
 	mov    %ecx,0xc(%rsp)
 	movsd  %xmm0,0x18(%rsp)
 	mov    %rdi,0x28(%rsp)
 	movsd  %xmm4,0x10(%rsp)
 	call   31c0 <omp_get_max_threads()@plt>
 	movslq %eax,%rdi
@@ -5777,15 +5777,15 @@
 	call   31a0 <malloc@plt>
 	mov    %rax,0x0(%r13)
 	mov    %rax,%r12
 	movslq %r14d,%rax
 	mov    %rax,0x38(%rsp)
 	lea    0x0(,%rax,8),%rbp
 	jmp    9d1b <histogram+0x9b>
-	nopl   (%rax)
+	nopw   0x0(%rax,%rax,1)
 	add    %rbx,%r12
 	add    %rbp,%rbx
 	mov    %r12,0x0(%r13,%r15,8)
 	mov    0x0(%r13),%r12
 	add    $0x1,%r15
 	call   31c0 <omp_get_max_threads()@plt>
 	cmp    %r15d,%eax
@@ -5803,554 +5803,552 @@
 	call   30f0 <memset@plt>
 	mov    0x10(%rsp),%ecx
 	movsd  0x18(%rsp),%xmm3
 	mov    %rax,%r9
 	mov    0xc(%rsp),%eax
 	movsd  0x20(%rsp),%xmm4
 	test   %eax,%eax
-	jle    a6ef <histogram+0xa6f>
+	jle    a6cf <histogram+0xa4f>
 	mov    0xc(%rsp),%ebx
-	movss  0x7c(%rsp),%xmm6
-	movss  0x78(%rsp),%xmm7
+	pxor   %xmm11,%xmm11
 	mov    0x28(%rsp),%rbp
+	movss  %xmm11,0xc(%rsp)
+	movd   %xmm11,%r15d
+	movaps %xmm11,%xmm10
+	movsd  0xe59f(%rip),%xmm7        
 	lea    -0x1(%rbx),%edx
 	lea    -0x10(%rbx),%eax
-	movss  %xmm6,0x10(%rsp)
-	mov    0x60(%rsp),%esi
+	movq   0xe3b9(%rip),%xmm6        
+	movsd  0xe528(%rip),%xmm13        
 	and    $0xfffffff0,%edx
-	movss  %xmm7,0xc(%rsp)
-	mov    0x64(%rsp),%edi
-	movss  0x44(%rsp),%xmm1
-	movss  0x48(%rsp),%xmm2
-	movss  0x4c(%rsp),%xmm5
+	movd   %xmm11,%r8d
+	movd   %xmm11,%r11d
+	movss  %xmm11,0x10(%rsp)
+	movd   %xmm11,%r10d
+	movd   %xmm11,%edi
+	movaps %xmm11,%xmm9
 	sub    %edx,%eax
-	movss  0x50(%rsp),%xmm8
-	movss  0x54(%rsp),%xmm9
-	movss  0x58(%rsp),%xmm10
-	movss  0x5c(%rsp),%xmm11
-	mov    0x68(%rsp),%r10d
-	mov    0x6c(%rsp),%r11d
-	mov    0x70(%rsp),%r8d
-	mov    0x74(%rsp),%r15d
-	movsd  0xe547(%rip),%xmm7        
-	movq   0xe367(%rip),%xmm6        
-	movsd  0xe4d6(%rip),%xmm13        
-	nopw   0x0(%rax,%rax,1)
+	movd   %xmm11,%esi
+	movaps %xmm11,%xmm8
+	movaps %xmm11,%xmm5
+	movaps %xmm11,%xmm2
+	movaps %xmm11,%xmm1
+	nopl   0x0(%rax)
 	movsd  0x0(%rbp),%xmm0
 	movapd %xmm6,%xmm12
 	subsd  %xmm3,%xmm0
 	mulsd  %xmm4,%xmm0
 	andpd  %xmm0,%xmm12
 	comisd %xmm12,%xmm7
-	jbe    9e4f <histogram+0x1cf>
+	jbe    9e37 <histogram+0x1b7>
 	cvttsd2si %xmm0,%rdx
 	pxor   %xmm12,%xmm12
 	cvtsi2sd %rdx,%xmm12
 	movapd %xmm12,%xmm14
 	cmpnlesd %xmm0,%xmm14
 	movapd %xmm12,%xmm0
 	andpd  %xmm13,%xmm14
 	subsd  %xmm14,%xmm0
 	cvtsd2ss %xmm0,%xmm0
 	cmp    $0x1,%ebx
-	je     a3f8 <histogram+0x778>
+	je     a3e0 <histogram+0x760>
 	movsd  0x8(%rbp),%xmm1
 	movapd %xmm6,%xmm12
 	subsd  %xmm3,%xmm1
 	mulsd  %xmm4,%xmm1
 	andpd  %xmm1,%xmm12
 	comisd %xmm12,%xmm7
-	jbe    9eab <histogram+0x22b>
+	jbe    9e93 <histogram+0x213>
 	cvttsd2si %xmm1,%rdx
 	pxor   %xmm12,%xmm12
 	cvtsi2sd %rdx,%xmm12
 	movapd %xmm12,%xmm14
 	cmpnlesd %xmm1,%xmm14
-	movsd  0xe43c(%rip),%xmm1        
+	movsd  0xe454(%rip),%xmm1        
 	andpd  %xmm1,%xmm14
 	movapd %xmm12,%xmm1
 	subsd  %xmm14,%xmm1
 	cvtsd2ss %xmm1,%xmm1
 	cmp    $0x2,%ebx
-	je     a3f8 <histogram+0x778>
+	je     a3e0 <histogram+0x760>
 	movsd  0x10(%rbp),%xmm2
 	movapd %xmm6,%xmm12
 	subsd  %xmm3,%xmm2
 	mulsd  %xmm4,%xmm2
 	andpd  %xmm2,%xmm12
 	comisd %xmm12,%xmm7
-	jbe    9f07 <histogram+0x287>
+	jbe    9eef <histogram+0x26f>
 	cvttsd2si %xmm2,%rdx
 	pxor   %xmm12,%xmm12
 	cvtsi2sd %rdx,%xmm12
 	movapd %xmm12,%xmm14
 	cmpnlesd %xmm2,%xmm14
-	movsd  0xe3e0(%rip),%xmm2        
+	movsd  0xe3f8(%rip),%xmm2        
 	andpd  %xmm2,%xmm14
 	movapd %xmm12,%xmm2
 	subsd  %xmm14,%xmm2
 	cvtsd2ss %xmm2,%xmm2
 	cmp    $0x3,%ebx
-	je     a3f8 <histogram+0x778>
+	je     a3e0 <histogram+0x760>
 	movsd  0x18(%rbp),%xmm5
 	movapd %xmm6,%xmm12
 	subsd  %xmm3,%xmm5
 	mulsd  %xmm4,%xmm5
 	andpd  %xmm5,%xmm12
 	comisd %xmm12,%xmm7
-	jbe    9f63 <histogram+0x2e3>
+	jbe    9f4b <histogram+0x2cb>
 	cvttsd2si %xmm5,%rdx
 	pxor   %xmm12,%xmm12
 	cvtsi2sd %rdx,%xmm12
 	movapd %xmm12,%xmm14
 	cmpnlesd %xmm5,%xmm14
-	movsd  0xe384(%rip),%xmm5        
+	movsd  0xe39c(%rip),%xmm5        
 	andpd  %xmm5,%xmm14
 	movapd %xmm12,%xmm5
 	subsd  %xmm14,%xmm5
 	cvtsd2ss %xmm5,%xmm5
 	cmp    $0x4,%ebx
-	je     a3f8 <histogram+0x778>
+	je     a3e0 <histogram+0x760>
 	movsd  0x20(%rbp),%xmm8
 	movapd %xmm6,%xmm12
 	subsd  %xmm3,%xmm8
 	mulsd  %xmm4,%xmm8
 	andpd  %xmm8,%xmm12
 	comisd %xmm12,%xmm7
-	jbe    9fc3 <histogram+0x343>
+	jbe    9fab <histogram+0x32b>
 	cvttsd2si %xmm8,%rdx
 	pxor   %xmm12,%xmm12
 	cvtsi2sd %rdx,%xmm12
 	movapd %xmm12,%xmm14
 	cmpnlesd %xmm8,%xmm14
-	movsd  0xe324(%rip),%xmm8        
+	movsd  0xe33c(%rip),%xmm8        
 	andpd  %xmm8,%xmm14
 	movapd %xmm12,%xmm8
 	subsd  %xmm14,%xmm8
 	cvtsd2ss %xmm8,%xmm8
 	cmp    $0x5,%ebx
-	je     a3f8 <histogram+0x778>
+	je     a3e0 <histogram+0x760>
 	movsd  0x28(%rbp),%xmm9
 	movapd %xmm6,%xmm12
 	subsd  %xmm3,%xmm9
 	mulsd  %xmm4,%xmm9
 	andpd  %xmm9,%xmm12
 	comisd %xmm12,%xmm7
-	jbe    a024 <histogram+0x3a4>
+	jbe    a00c <histogram+0x38c>
 	cvttsd2si %xmm9,%rdx
 	pxor   %xmm12,%xmm12
 	cvtsi2sd %rdx,%xmm12
 	movapd %xmm12,%xmm14
 	cmpnlesd %xmm9,%xmm14
-	movsd  0xe2c3(%rip),%xmm9        
+	movsd  0xe2db(%rip),%xmm9        
 	andpd  %xmm9,%xmm14
 	movapd %xmm12,%xmm9
 	subsd  %xmm14,%xmm9
 	cvtsd2ss %xmm9,%xmm9
 	cmp    $0x6,%ebx
-	je     a3f8 <histogram+0x778>
+	je     a3e0 <histogram+0x760>
 	movsd  0x30(%rbp),%xmm10
 	movapd %xmm6,%xmm12
 	subsd  %xmm3,%xmm10
 	mulsd  %xmm4,%xmm10
 	andpd  %xmm10,%xmm12
 	comisd %xmm12,%xmm7
-	jbe    a085 <histogram+0x405>
+	jbe    a06d <histogram+0x3ed>
 	cvttsd2si %xmm10,%rdx
 	pxor   %xmm12,%xmm12
 	cvtsi2sd %rdx,%xmm12
 	movapd %xmm12,%xmm14
 	cmpnlesd %xmm10,%xmm14
-	movsd  0xe262(%rip),%xmm10        
+	movsd  0xe27a(%rip),%xmm10        
 	andpd  %xmm10,%xmm14
 	movapd %xmm12,%xmm10
 	subsd  %xmm14,%xmm10
 	cvtsd2ss %xmm10,%xmm10
 	cmp    $0x7,%ebx
-	je     a3f8 <histogram+0x778>
-	movsd  0x38(%rbp),%xmm11
-	movapd %xmm6,%xmm12
-	subsd  %xmm3,%xmm11
-	mulsd  %xmm4,%xmm11
-	andpd  %xmm11,%xmm12
-	comisd %xmm12,%xmm7
-	jbe    a0dd <histogram+0x45d>
-	cvttsd2si %xmm11,%rdx
-	pxor   %xmm12,%xmm12
-	cvtsi2sd %rdx,%xmm12
-	movapd %xmm12,%xmm14
-	cmpnlesd %xmm11,%xmm14
-	movapd %xmm12,%xmm11
-	andpd  %xmm13,%xmm14
-	subsd  %xmm14,%xmm11
-	cvtsd2ss %xmm11,%xmm11
-	cmp    $0x8,%ebx
-	je     a3f8 <histogram+0x778>
-	movsd  0x40(%rbp),%xmm12
+	je     a3e0 <histogram+0x760>
+	movsd  0x38(%rbp),%xmm12
 	movapd %xmm6,%xmm14
 	subsd  %xmm3,%xmm12
 	mulsd  %xmm4,%xmm12
 	andpd  %xmm12,%xmm14
 	comisd %xmm14,%xmm7
-	jbe    a135 <histogram+0x4b5>
+	jbe    a0c5 <histogram+0x445>
 	cvttsd2si %xmm12,%rdx
 	pxor   %xmm14,%xmm14
 	cvtsi2sd %rdx,%xmm14
 	movapd %xmm14,%xmm15
 	cmpnlesd %xmm12,%xmm15
 	andpd  %xmm13,%xmm15
 	subsd  %xmm15,%xmm14
 	movapd %xmm14,%xmm12
 	pxor   %xmm15,%xmm15
 	cvtsd2ss %xmm12,%xmm15
 	movd   %xmm15,%esi
-	cmp    $0x9,%ebx
-	je     a3f8 <histogram+0x778>
-	movsd  0x48(%rbp),%xmm12
+	cmp    $0x8,%ebx
+	je     a3e0 <histogram+0x760>
+	movsd  0x40(%rbp),%xmm12
 	movapd %xmm6,%xmm14
 	subsd  %xmm3,%xmm12
 	mulsd  %xmm4,%xmm12
 	andpd  %xmm12,%xmm14
 	comisd %xmm14,%xmm7
-	jbe    a197 <histogram+0x517>
+	jbe    a127 <histogram+0x4a7>
 	cvttsd2si %xmm12,%rdx
 	pxor   %xmm14,%xmm14
 	cvtsi2sd %rdx,%xmm14
 	movapd %xmm14,%xmm15
 	cmpnlesd %xmm12,%xmm15
 	andpd  %xmm13,%xmm15
 	subsd  %xmm15,%xmm14
 	movapd %xmm14,%xmm12
 	pxor   %xmm15,%xmm15
 	cvtsd2ss %xmm12,%xmm15
 	movd   %xmm15,%edi
-	cmp    $0xa,%ebx
-	je     a3f8 <histogram+0x778>
-	movsd  0x50(%rbp),%xmm12
+	cmp    $0x9,%ebx
+	je     a3e0 <histogram+0x760>
+	movsd  0x48(%rbp),%xmm12
 	movapd %xmm6,%xmm14
 	subsd  %xmm3,%xmm12
 	mulsd  %xmm4,%xmm12
 	andpd  %xmm12,%xmm14
 	comisd %xmm14,%xmm7
-	jbe    a1f9 <histogram+0x579>
+	jbe    a189 <histogram+0x509>
 	cvttsd2si %xmm12,%rdx
 	pxor   %xmm14,%xmm14
 	cvtsi2sd %rdx,%xmm14
 	movapd %xmm14,%xmm15
 	cmpnlesd %xmm12,%xmm15
 	andpd  %xmm13,%xmm15
 	subsd  %xmm15,%xmm14
 	movapd %xmm14,%xmm12
 	pxor   %xmm15,%xmm15
 	cvtsd2ss %xmm12,%xmm15
 	movd   %xmm15,%r10d
-	cmp    $0xb,%ebx
-	je     a3f8 <histogram+0x778>
-	movsd  0x58(%rbp),%xmm12
+	cmp    $0xa,%ebx
+	je     a3e0 <histogram+0x760>
+	movsd  0x50(%rbp),%xmm12
 	movapd %xmm6,%xmm14
 	subsd  %xmm3,%xmm12
 	mulsd  %xmm4,%xmm12
 	andpd  %xmm12,%xmm14
 	comisd %xmm14,%xmm7
-	jbe    a25b <histogram+0x5db>
+	jbe    a1eb <histogram+0x56b>
 	cvttsd2si %xmm12,%rdx
 	pxor   %xmm14,%xmm14
 	cvtsi2sd %rdx,%xmm14
 	movapd %xmm14,%xmm15
 	cmpnlesd %xmm12,%xmm15
 	andpd  %xmm13,%xmm15
 	subsd  %xmm15,%xmm14
 	movapd %xmm14,%xmm12
 	pxor   %xmm15,%xmm15
 	cvtsd2ss %xmm12,%xmm15
 	movd   %xmm15,%r11d
-	cmp    $0xc,%ebx
-	je     a3f8 <histogram+0x778>
-	movsd  0x60(%rbp),%xmm12
+	cmp    $0xb,%ebx
+	je     a3e0 <histogram+0x760>
+	movsd  0x58(%rbp),%xmm12
 	movapd %xmm6,%xmm14
 	subsd  %xmm3,%xmm12
 	mulsd  %xmm4,%xmm12
 	andpd  %xmm12,%xmm14
 	comisd %xmm14,%xmm7
-	jbe    a2bd <histogram+0x63d>
+	jbe    a24d <histogram+0x5cd>
 	cvttsd2si %xmm12,%rdx
 	pxor   %xmm14,%xmm14
 	cvtsi2sd %rdx,%xmm14
 	movapd %xmm14,%xmm15
 	cmpnlesd %xmm12,%xmm15
 	andpd  %xmm13,%xmm15
 	subsd  %xmm15,%xmm14
 	movapd %xmm14,%xmm12
 	pxor   %xmm15,%xmm15
 	cvtsd2ss %xmm12,%xmm15
 	movd   %xmm15,%r8d
-	cmp    $0xd,%ebx
-	je     a3f8 <histogram+0x778>
-	movsd  0x68(%rbp),%xmm12
+	cmp    $0xc,%ebx
+	je     a3e0 <histogram+0x760>
+	movsd  0x60(%rbp),%xmm12
 	movapd %xmm6,%xmm14
 	subsd  %xmm3,%xmm12
 	mulsd  %xmm4,%xmm12
 	andpd  %xmm12,%xmm14
 	comisd %xmm14,%xmm7
-	jbe    a31f <histogram+0x69f>
+	jbe    a2af <histogram+0x62f>
 	cvttsd2si %xmm12,%rdx
 	pxor   %xmm14,%xmm14
 	cvtsi2sd %rdx,%xmm14
 	movapd %xmm14,%xmm15
 	cmpnlesd %xmm12,%xmm15
 	andpd  %xmm13,%xmm15
 	subsd  %xmm15,%xmm14
 	movapd %xmm14,%xmm12
 	pxor   %xmm15,%xmm15
 	cvtsd2ss %xmm12,%xmm15
 	movd   %xmm15,%r15d
-	cmp    $0xe,%ebx
-	je     a3f8 <histogram+0x778>
-	movsd  0x70(%rbp),%xmm12
+	cmp    $0xd,%ebx
+	je     a3e0 <histogram+0x760>
+	movsd  0x68(%rbp),%xmm12
 	movapd %xmm6,%xmm14
 	subsd  %xmm3,%xmm12
 	mulsd  %xmm4,%xmm12
 	andpd  %xmm12,%xmm14
 	comisd %xmm14,%xmm7
-	jbe    a381 <histogram+0x701>
+	jbe    a311 <histogram+0x691>
 	cvttsd2si %xmm12,%rdx
 	pxor   %xmm14,%xmm14
 	cvtsi2sd %rdx,%xmm14
 	movapd %xmm14,%xmm15
 	cmpnlesd %xmm12,%xmm15
 	andpd  %xmm13,%xmm15
 	subsd  %xmm15,%xmm14
 	movapd %xmm14,%xmm12
 	pxor   %xmm15,%xmm15
 	cvtsd2ss %xmm12,%xmm15
 	movss  %xmm15,0xc(%rsp)
+	cmp    $0xe,%ebx
+	je     a3e0 <histogram+0x760>
+	movsd  0x70(%rbp),%xmm11
+	movapd %xmm6,%xmm12
+	subsd  %xmm3,%xmm11
+	mulsd  %xmm4,%xmm11
+	andpd  %xmm11,%xmm12
+	comisd %xmm12,%xmm7
+	jbe    a375 <histogram+0x6f5>
+	cvttsd2si %xmm11,%rdx
+	pxor   %xmm12,%xmm12
+	cvtsi2sd %rdx,%xmm12
+	movapd %xmm12,%xmm14
+	cmpnlesd %xmm11,%xmm14
+	movapd %xmm12,%xmm11
+	andpd  %xmm13,%xmm14
+	subsd  %xmm14,%xmm11
+	cvtsd2ss %xmm11,%xmm11
 	cmp    $0xf,%ebx
-	je     a3f8 <histogram+0x778>
+	je     a3e0 <histogram+0x760>
 	movsd  0x78(%rbp),%xmm12
 	movapd %xmm6,%xmm14
 	subsd  %xmm3,%xmm12
 	mulsd  %xmm4,%xmm12
 	andpd  %xmm12,%xmm14
 	comisd %xmm14,%xmm7
-	jbe    a3e1 <histogram+0x761>
+	jbe    a3c9 <histogram+0x749>
 	cvttsd2si %xmm12,%rdx
 	pxor   %xmm14,%xmm14
 	cvtsi2sd %rdx,%xmm14
 	movapd %xmm14,%xmm15
 	cmpnlesd %xmm12,%xmm15
 	andpd  %xmm13,%xmm15
 	subsd  %xmm15,%xmm14
 	movapd %xmm14,%xmm12
 	pxor   %xmm15,%xmm15
 	cvtsd2ss %xmm12,%xmm15
 	movss  %xmm15,0x10(%rsp)
 	nopw   0x0(%rax,%rax,1)
 	cvttss2si %xmm0,%edx
 	cmp    %edx,%r14d
-	jle    a41c <histogram+0x79c>
+	jle    a404 <histogram+0x784>
 	test   %edx,%edx
-	js     a41c <histogram+0x79c>
+	js     a404 <histogram+0x784>
 	movslq %edx,%rdx
-	movsd  0xdec8(%rip),%xmm0        
+	movsd  0xdee0(%rip),%xmm0        
 	lea    (%r9,%rdx,8),%rdx
 	addsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rdx)
 	cmp    $0x1,%ebx
-	je     a6e0 <histogram+0xa60>
+	je     a6c0 <histogram+0xa40>
 	cvttss2si %xmm1,%edx
 	cmp    %edx,%r14d
-	jle    a449 <histogram+0x7c9>
+	jle    a431 <histogram+0x7b1>
 	test   %edx,%edx
-	js     a449 <histogram+0x7c9>
+	js     a431 <histogram+0x7b1>
 	movslq %edx,%rdx
-	movsd  0xde9b(%rip),%xmm0        
+	movsd  0xdeb3(%rip),%xmm0        
 	lea    (%r9,%rdx,8),%rdx
 	addsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rdx)
 	cmp    $0x2,%ebx
-	je     a6e0 <histogram+0xa60>
+	je     a6c0 <histogram+0xa40>
 	cvttss2si %xmm2,%edx
 	cmp    %edx,%r14d
-	jle    a476 <histogram+0x7f6>
+	jle    a45e <histogram+0x7de>
 	test   %edx,%edx
-	js     a476 <histogram+0x7f6>
+	js     a45e <histogram+0x7de>
 	movslq %edx,%rdx
-	movsd  0xde6e(%rip),%xmm0        
+	movsd  0xde86(%rip),%xmm0        
 	lea    (%r9,%rdx,8),%rdx
 	addsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rdx)
 	cmp    $0x3,%ebx
-	je     a6e0 <histogram+0xa60>
+	je     a6c0 <histogram+0xa40>
 	cvttss2si %xmm5,%edx
 	cmp    %edx,%r14d
-	jle    a4a3 <histogram+0x823>
+	jle    a48b <histogram+0x80b>
 	test   %edx,%edx
-	js     a4a3 <histogram+0x823>
+	js     a48b <histogram+0x80b>
 	movslq %edx,%rdx
-	movsd  0xde41(%rip),%xmm0        
+	movsd  0xde59(%rip),%xmm0        
 	lea    (%r9,%rdx,8),%rdx
 	addsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rdx)
 	cmp    $0x4,%ebx
-	je     a6e0 <histogram+0xa60>
+	je     a6c0 <histogram+0xa40>
 	cvttss2si %xmm8,%edx
 	test   %edx,%edx
-	js     a4d1 <histogram+0x851>
+	js     a4b9 <histogram+0x839>
 	cmp    %edx,%r14d
-	jle    a4d1 <histogram+0x851>
+	jle    a4b9 <histogram+0x839>
 	movslq %edx,%rdx
-	movsd  0xde13(%rip),%xmm0        
+	movsd  0xde2b(%rip),%xmm0        
 	lea    (%r9,%rdx,8),%rdx
 	addsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rdx)
 	cmp    $0x5,%ebx
-	je     a6e0 <histogram+0xa60>
+	je     a6c0 <histogram+0xa40>
 	cvttss2si %xmm9,%edx
 	cmp    %edx,%r14d
-	jle    a4ff <histogram+0x87f>
+	jle    a4e7 <histogram+0x867>
 	test   %edx,%edx
-	js     a4ff <histogram+0x87f>
+	js     a4e7 <histogram+0x867>
 	movslq %edx,%rdx
-	movsd  0xdde5(%rip),%xmm0        
+	movsd  0xddfd(%rip),%xmm0        
 	lea    (%r9,%rdx,8),%rdx
 	addsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rdx)
 	cmp    $0x6,%ebx
-	je     a6e0 <histogram+0xa60>
+	je     a6c0 <histogram+0xa40>
 	cvttss2si %xmm10,%edx
 	test   %edx,%edx
-	js     a52d <histogram+0x8ad>
+	js     a515 <histogram+0x895>
 	cmp    %edx,%r14d
-	jle    a52d <histogram+0x8ad>
+	jle    a515 <histogram+0x895>
 	movslq %edx,%rdx
-	movsd  0xddb7(%rip),%xmm0        
+	movsd  0xddcf(%rip),%xmm0        
 	lea    (%r9,%rdx,8),%rdx
 	addsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rdx)
 	cmp    $0x7,%ebx
-	je     a6e0 <histogram+0xa60>
-	cvttss2si %xmm11,%edx
+	je     a6c0 <histogram+0xa40>
+	movd   %esi,%xmm0
+	cvttss2si %xmm0,%edx
 	test   %edx,%edx
-	js     a55b <histogram+0x8db>
+	js     a546 <histogram+0x8c6>
 	cmp    %edx,%r14d
-	jle    a55b <histogram+0x8db>
+	jle    a546 <histogram+0x8c6>
 	movslq %edx,%rdx
-	movsd  0xdd89(%rip),%xmm0        
+	movsd  0xdd9e(%rip),%xmm0        
 	lea    (%r9,%rdx,8),%rdx
 	addsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rdx)
 	cmp    $0x8,%ebx
-	je     a6e0 <histogram+0xa60>
-	movd   %esi,%xmm0
+	je     a6c0 <histogram+0xa40>
+	movd   %edi,%xmm0
 	cvttss2si %xmm0,%edx
 	test   %edx,%edx
-	js     a58c <histogram+0x90c>
+	js     a577 <histogram+0x8f7>
 	cmp    %edx,%r14d
-	jle    a58c <histogram+0x90c>
+	jle    a577 <histogram+0x8f7>
 	movslq %edx,%rdx
-	movsd  0xdd58(%rip),%xmm0        
+	movsd  0xdd6d(%rip),%xmm0        
 	lea    (%r9,%rdx,8),%rdx
 	addsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rdx)
 	cmp    $0x9,%ebx
-	je     a6e0 <histogram+0xa60>
-	movd   %edi,%xmm0
+	je     a6c0 <histogram+0xa40>
+	movd   %r10d,%xmm0
 	cvttss2si %xmm0,%edx
 	test   %edx,%edx
-	js     a5bd <histogram+0x93d>
+	js     a5a9 <histogram+0x929>
 	cmp    %edx,%r14d
-	jle    a5bd <histogram+0x93d>
+	jle    a5a9 <histogram+0x929>
 	movslq %edx,%rdx
-	movsd  0xdd27(%rip),%xmm0        
+	movsd  0xdd3b(%rip),%xmm0        
 	lea    (%r9,%rdx,8),%rdx
 	addsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rdx)
 	cmp    $0xa,%ebx
-	je     a6e0 <histogram+0xa60>
-	movd   %r10d,%xmm0
+	je     a6c0 <histogram+0xa40>
+	movd   %r11d,%xmm0
 	cvttss2si %xmm0,%edx
 	test   %edx,%edx
-	js     a5ef <histogram+0x96f>
+	js     a5db <histogram+0x95b>
 	cmp    %edx,%r14d
-	jle    a5ef <histogram+0x96f>
+	jle    a5db <histogram+0x95b>
 	movslq %edx,%rdx
-	movsd  0xdcf5(%rip),%xmm0        
+	movsd  0xdd09(%rip),%xmm0        
 	lea    (%r9,%rdx,8),%rdx
 	addsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rdx)
 	cmp    $0xb,%ebx
-	je     a6e0 <histogram+0xa60>
-	movd   %r11d,%xmm0
+	je     a6c0 <histogram+0xa40>
+	movd   %r8d,%xmm0
 	cvttss2si %xmm0,%edx
 	test   %edx,%edx
-	js     a621 <histogram+0x9a1>
+	js     a60d <histogram+0x98d>
 	cmp    %edx,%r14d
-	jle    a621 <histogram+0x9a1>
+	jle    a60d <histogram+0x98d>
 	movslq %edx,%rdx
-	movsd  0xdcc3(%rip),%xmm0        
+	movsd  0xdcd7(%rip),%xmm0        
 	lea    (%r9,%rdx,8),%rdx
 	addsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rdx)
 	cmp    $0xc,%ebx
-	je     a6e0 <histogram+0xa60>
-	movd   %r8d,%xmm0
+	je     a6c0 <histogram+0xa40>
+	movd   %r15d,%xmm0
 	cvttss2si %xmm0,%edx
 	test   %edx,%edx
-	js     a653 <histogram+0x9d3>
+	js     a63f <histogram+0x9bf>
 	cmp    %edx,%r14d
-	jle    a653 <histogram+0x9d3>
+	jle    a63f <histogram+0x9bf>
 	movslq %edx,%rdx
-	movsd  0xdc91(%rip),%xmm0        
+	movsd  0xdca5(%rip),%xmm0        
 	lea    (%r9,%rdx,8),%rdx
 	addsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rdx)
 	cmp    $0xd,%ebx
-	je     a6e0 <histogram+0xa60>
-	movd   %r15d,%xmm0
-	cvttss2si %xmm0,%edx
+	je     a6c0 <histogram+0xa40>
+	cvttss2si 0xc(%rsp),%edx
 	test   %edx,%edx
-	js     a685 <histogram+0xa05>
+	js     a66a <histogram+0x9ea>
 	cmp    %edx,%r14d
-	jle    a685 <histogram+0xa05>
+	jle    a66a <histogram+0x9ea>
 	movslq %edx,%rdx
-	movsd  0xdc5f(%rip),%xmm0        
+	movsd  0xdc7a(%rip),%xmm0        
 	lea    (%r9,%rdx,8),%rdx
 	addsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rdx)
 	cmp    $0xe,%ebx
-	je     a6e0 <histogram+0xa60>
-	cvttss2si 0xc(%rsp),%edx
+	je     a6c0 <histogram+0xa40>
+	cvttss2si %xmm11,%edx
 	test   %edx,%edx
-	js     a6b0 <histogram+0xa30>
+	js     a694 <histogram+0xa14>
 	cmp    %edx,%r14d
-	jle    a6b0 <histogram+0xa30>
+	jle    a694 <histogram+0xa14>
 	movslq %edx,%rdx
-	movsd  0xdc34(%rip),%xmm0        
+	movsd  0xdc50(%rip),%xmm0        
 	lea    (%r9,%rdx,8),%rdx
 	addsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rdx)
 	cmp    $0xf,%ebx
-	je     a6e0 <histogram+0xa60>
+	je     a6c0 <histogram+0xa40>
 	cvttss2si 0x10(%rsp),%edx
 	test   %edx,%edx
-	js     a6e0 <histogram+0xa60>
+	js     a6c0 <histogram+0xa40>
 	cmp    %edx,%r14d
-	jle    a6e0 <histogram+0xa60>
+	jle    a6c0 <histogram+0xa40>
 	movslq %edx,%rdx
-	movsd  0xdc09(%rip),%xmm0        
+	movsd  0xdc25(%rip),%xmm0        
 	lea    (%r9,%rdx,8),%rdx
 	addsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rdx)
-	nopl   0x0(%rax,%rax,1)
+	nop
 	sub    $0x10,%ebx
 	sub    $0xffffffffffffff80,%rbp
 	cmp    %ebx,%eax
-	jne    9e08 <histogram+0x188>
+	jne    9df0 <histogram+0x170>
 	test   %r14d,%r14d
-	jle    a758 <histogram+0xad8>
+	jle    a738 <histogram+0xab8>
 	mov    0x38(%rsp),%rbx
 	mov    0x30(%rsp),%r15
 	xor    %esi,%esi
 	mov    %ecx,0xc(%rsp)
 	shl    $0x3,%rbx
 	mov    %r15,%rdi
 	mov    %rbx,%rdx
@@ -6358,41 +6356,41 @@
 	mov    0xc(%rsp),%ecx
 	xor    %esi,%esi
 	mov    %r15,%r8
 	lea    -0x1(%rcx),%eax
 	lea    0x8(%r13,%rax,8),%rdi
 	nopl   0x0(%rax)
 	test   %ecx,%ecx
-	jle    a74f <histogram+0xacf>
+	jle    a72f <histogram+0xaaf>
 	mov    %r13,%rax
 	pxor   %xmm0,%xmm0
 	nopl   0x0(%rax,%rax,1)
 	mov    (%rax),%rdx
 	add    $0x8,%rax
 	addsd  (%rdx,%rsi,1),%xmm0
 	cmp    %rdi,%rax
-	jne    a738 <histogram+0xab8>
+	jne    a718 <histogram+0xa98>
 	movsd  %xmm0,(%r8,%rsi,1)
 	add    $0x8,%rsi
 	cmp    %rsi,%rbx
-	jne    a728 <histogram+0xaa8>
+	jne    a708 <histogram+0xa88>
 	mov    %r12,%rdi
 	call   3180 <free@plt>
-	add    $0x88,%rsp
+	add    $0x48,%rsp
 	mov    %r13,%rdi
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	jmp    3180 <free@plt>
-	nopl   0x0(%rax)
+	cs nopw 0x0(%rax,%rax,1)
 
-000000000000a780 <smooth_histogram>:
+000000000000a760 <smooth_histogram>:
 smooth_histogram():
 	push   %r15
 	pxor   %xmm2,%xmm2
 	movapd %xmm0,%xmm4
 	xor    %r15d,%r15d
 	push   %r14
 	cvtsi2sd %edx,%xmm2
@@ -6409,15 +6407,15 @@
 	subsd  %xmm4,%xmm0
 	mov    %edx,0x2c(%rsp)
 	mov    %ecx,0x28(%rsp)
 	mov    %rdi,0x30(%rsp)
 	divsd  %xmm0,%xmm6
 	divsd  %xmm2,%xmm0
 	movsd  %xmm6,0x18(%rsp)
-	mulsd  0xdaf8(%rip),%xmm0        
+	mulsd  0xdb18(%rip),%xmm0        
 	addsd  %xmm0,%xmm4
 	subsd  %xmm0,%xmm1
 	movsd  %xmm4,0x8(%rsp)
 	movsd  %xmm1,0x10(%rsp)
 	call   31c0 <omp_get_max_threads()@plt>
 	movslq %eax,%rdi
 	shl    $0x3,%rdi
@@ -6430,714 +6428,710 @@
 	call   31a0 <malloc@plt>
 	mov    %rax,(%r12)
 	mov    %rax,%rbp
 	movslq %r14d,%rax
 	xor    %r14d,%r14d
 	mov    %rax,0x38(%rsp)
 	lea    0x0(,%rax,8),%r13
-	jmp    a84a <smooth_histogram+0xca>
+	jmp    a82a <smooth_histogram+0xca>
 	nopl   0x0(%rax)
 	add    %r14,%rbp
 	add    %r13,%r14
 	mov    %rbp,(%r12,%r15,8)
 	mov    (%r12),%rbp
 	add    $0x1,%r15
 	call   31c0 <omp_get_max_threads()@plt>
 	cmp    %r15d,%eax
-	jg     a838 <smooth_histogram+0xb8>
+	jg     a818 <smooth_histogram+0xb8>
 	call   3040 <omp_get_thread_num()@plt>
 	mov    %eax,%r14d
 	call   3090 <omp_get_num_threads()@plt>
 	mov    %r13,%rdx
 	xor    %esi,%esi
 	mov    %eax,%r15d
 	movslq %r14d,%rax
 	mov    (%r12,%rax,8),%rcx
 	mov    %rcx,%rdi
 	call   30f0 <memset@plt>
 	mov    0x28(%rsp),%edx
 	mov    %rax,%rcx
 	test   %edx,%edx
-	jle    a950 <smooth_histogram+0x1d0>
+	jle    a930 <smooth_histogram+0x1d0>
 	mov    0x28(%rsp),%eax
 	mov    0x30(%rsp),%rdi
-	movsd  0xda40(%rip),%xmm4        
+	movsd  0xda60(%rip),%xmm4        
 	sub    $0x1,%eax
 	lea    0x8(%rdi,%rax,8),%rax
-	jmp    a8ef <smooth_histogram+0x16f>
+	jmp    a8cf <smooth_histogram+0x16f>
 	nopw   0x0(%rax,%rax,1)
 	addsd  %xmm4,%xmm3
 	cvttsd2si %xmm3,%esi
-	movsd  0xda18(%rip),%xmm3        
+	movsd  0xda38(%rip),%xmm3        
 	movslq %edx,%rdx
-	addsd  0xda0d(%rip),%xmm1        
+	addsd  0xda2d(%rip),%xmm1        
 	lea    (%rcx,%rdx,8),%rdx
 	addsd  (%rdx),%xmm2
 	subsd  %xmm0,%xmm3
 	addsd  %xmm3,%xmm2
 	movsd  %xmm2,(%rdx)
 	movslq %esi,%rdx
 	lea    (%rcx,%rdx,8),%rdx
 	addsd  (%rdx),%xmm1
 	movsd  %xmm1,(%rdx)
 	add    $0x8,%rdi
 	cmp    %rdi,%rax
-	je     a950 <smooth_histogram+0x1d0>
+	je     a930 <smooth_histogram+0x1d0>
 	movsd  (%rdi),%xmm0
 	movsd  0x8(%rsp),%xmm5
 	comisd %xmm0,%xmm5
-	ja     a8e6 <smooth_histogram+0x166>
+	ja     a8c6 <smooth_histogram+0x166>
 	comisd 0x10(%rsp),%xmm0
-	ja     a8e6 <smooth_histogram+0x166>
+	ja     a8c6 <smooth_histogram+0x166>
 	subsd  0x20(%rsp),%xmm0
 	mulsd  0x18(%rsp),%xmm0
 	pxor   %xmm2,%xmm2
 	cvttsd2si %xmm0,%edx
 	movapd %xmm0,%xmm1
 	movapd %xmm0,%xmm3
 	cvtsi2sd %edx,%xmm2
 	subsd  %xmm2,%xmm1
-	comisd 0xd99d(%rip),%xmm1        
-	ja     a8a8 <smooth_histogram+0x128>
+	comisd 0xd9bd(%rip),%xmm1        
+	ja     a888 <smooth_histogram+0x128>
 	subsd  %xmm4,%xmm3
 	cvttsd2si %xmm3,%esi
-	jmp    a8b0 <smooth_histogram+0x130>
+	jmp    a890 <smooth_histogram+0x130>
 	cs nopw 0x0(%rax,%rax,1)
 	mov    0x2c(%rsp),%eax
 	test   %eax,%eax
-	jle    a9af <smooth_histogram+0x22f>
+	jle    a98f <smooth_histogram+0x22f>
 	mov    0x38(%rsp),%r13
 	xor    %esi,%esi
 	mov    %rbx,%rdi
 	shl    $0x3,%r13
 	mov    %r13,%rdx
 	call   30f0 <memset@plt>
 	lea    -0x1(%r15),%eax
 	xor    %ecx,%ecx
 	lea    0x8(%r12,%rax,8),%rsi
 	nopl   0x0(%rax)
 	test   %r15d,%r15d
-	jle    a9a6 <smooth_histogram+0x226>
+	jle    a986 <smooth_histogram+0x226>
 	mov    %r12,%rax
 	pxor   %xmm0,%xmm0
 	nopl   0x0(%rax)
 	mov    (%rax),%rdx
 	add    $0x8,%rax
 	addsd  (%rdx,%rcx,1),%xmm0
 	cmp    %rax,%rsi
-	jne    a990 <smooth_histogram+0x210>
+	jne    a970 <smooth_histogram+0x210>
 	movsd  %xmm0,(%rbx,%rcx,1)
 	add    $0x8,%rcx
 	cmp    %r13,%rcx
-	jne    a980 <smooth_histogram+0x200>
+	jne    a960 <smooth_histogram+0x200>
 	mov    %rbp,%rdi
 	call   3180 <free@plt>
 	add    $0x48,%rsp
 	mov    %r12,%rdi
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	jmp    3180 <free@plt>
 	nopl   (%rax)
 
-000000000000a9d0 <histogramf>:
+000000000000a9b0 <histogramf>:
 histogramf():
 	push   %r15
 	pxor   %xmm4,%xmm4
 	subss  %xmm0,%xmm1
 	movaps %xmm0,%xmm3
 	push   %r14
 	mov    %rsi,%r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
 	movslq %edx,%rbx
 	cvtsi2ss %ebx,%xmm4
 	mov    %rbx,%r12
-	sub    $0x68,%rsp
-	cmpq   $0x0,0x11782(%rip)        
+	sub    $0x28,%rsp
+	cmpq   $0x0,0x117a2(%rip)        
 	mov    %rdi,0x18(%rsp)
 	divss  %xmm1,%xmm4
 	mov    %ecx,0xc(%rsp)
-	je     b38f <histogramf+0x9bf>
+	je     b34f <histogramf+0x99f>
 	movss  %xmm3,0x14(%rsp)
 	movss  %xmm4,0x10(%rsp)
 	call   3040 <omp_get_thread_num()@plt>
 	movslq %eax,%r15
 	call   3090 <omp_get_num_threads()@plt>
-	mov    0x1174f(%rip),%rbp        
+	mov    0x1176f(%rip),%rbp        
 	xor    %esi,%esi
 	lea    0x0(,%rbx,4),%rdx
 	mov    %eax,%r13d
 	lea    0x0(%rbp,%r15,8),%r15
 	mov    (%r15),%rdi
 	call   30f0 <memset@plt>
 	mov    0xc(%rsp),%eax
 	movss  0x10(%rsp),%xmm4
 	movss  0x14(%rsp),%xmm3
 	test   %eax,%eax
-	jle    b32f <histogramf+0x95f>
-	movss  0x4c(%rsp),%xmm7
+	jle    b2ef <histogramf+0x93f>
 	mov    0xc(%rsp),%ecx
-	movss  0x5c(%rsp),%xmm6
+	pxor   %xmm11,%xmm11
+	movss  0xd8ec(%rip),%xmm7        
+	movss  0xd7e4(%rip),%xmm6        
 	mov    0x18(%rsp),%rdi
-	movss  %xmm7,0xc(%rsp)
-	movss  0x58(%rsp),%xmm7
+	movd   %xmm11,%r8d
+	movss  0xd889(%rip),%xmm13        
+	movss  %xmm11,0x14(%rsp)
 	lea    -0x1(%rcx),%eax
 	lea    -0x10(%rcx),%edx
-	movss  %xmm6,0x18(%rsp)
-	movss  0x54(%rsp),%xmm6
+	movaps %xmm11,%xmm10
+	movss  %xmm11,0x10(%rsp)
 	and    $0xfffffff0,%eax
-	movss  0x24(%rsp),%xmm0
-	movss  %xmm7,0x14(%rsp)
-	movss  0x28(%rsp),%xmm2
+	movss  %xmm11,0xc(%rsp)
+	movd   %xmm11,%r11d
+	movd   %xmm11,%r10d
+	movd   %xmm11,%r9d
+	movaps %xmm11,%xmm9
+	movaps %xmm11,%xmm8
 	sub    %eax,%edx
-	movss  0x2c(%rsp),%xmm5
-	movss  0x30(%rsp),%xmm8
-	movss  0x34(%rsp),%xmm9
-	movss  %xmm6,0x10(%rsp)
-	movss  0xd771(%rip),%xmm6        
-	movss  0x38(%rsp),%xmm10
-	movss  0x3c(%rsp),%xmm11
-	mov    0x40(%rsp),%r9d
-	mov    0x44(%rsp),%r10d
-	mov    0x48(%rsp),%r11d
-	mov    0x50(%rsp),%r8d
-	movss  0xd847(%rip),%xmm7        
-	movss  0xd7f6(%rip),%xmm13        
-	nopw   0x0(%rax,%rax,1)
+	movaps %xmm11,%xmm5
+	movaps %xmm11,%xmm2
+	movaps %xmm11,%xmm0
+	movss  %xmm11,0x18(%rsp)
+	nopl   (%rax)
 	movss  (%rdi),%xmm1
 	movaps %xmm6,%xmm12
 	subss  %xmm3,%xmm1
 	mulss  %xmm4,%xmm1
 	andps  %xmm1,%xmm12
 	comiss %xmm12,%xmm7
-	jbe    ab47 <histogramf+0x177>
+	jbe    aaff <histogramf+0x14f>
 	cvttss2si %xmm1,%eax
 	pxor   %xmm12,%xmm12
 	cvtsi2ss %eax,%xmm12
 	movaps %xmm12,%xmm14
 	cmpnless %xmm1,%xmm14
 	movaps %xmm12,%xmm1
 	andps  %xmm13,%xmm14
 	subss  %xmm14,%xmm1
 	cmp    $0x1,%ecx
-	je     b020 <histogramf+0x650>
+	je     afd8 <histogramf+0x628>
 	movss  0x4(%rdi),%xmm0
 	movaps %xmm6,%xmm12
 	subss  %xmm3,%xmm0
 	mulss  %xmm4,%xmm0
 	andps  %xmm0,%xmm12
 	comiss %xmm12,%xmm7
-	jbe    ab98 <histogramf+0x1c8>
+	jbe    ab50 <histogramf+0x1a0>
 	cvttss2si %xmm0,%eax
 	pxor   %xmm12,%xmm12
 	cvtsi2ss %eax,%xmm12
 	movaps %xmm12,%xmm14
 	cmpnless %xmm0,%xmm14
-	movss  0xd76d(%rip),%xmm0        
+	movss  0xd7b5(%rip),%xmm0        
 	andps  %xmm0,%xmm14
 	movaps %xmm12,%xmm0
 	subss  %xmm14,%xmm0
 	cmp    $0x2,%ecx
-	je     b020 <histogramf+0x650>
+	je     afd8 <histogramf+0x628>
 	movss  0x8(%rdi),%xmm2
 	movaps %xmm6,%xmm12
 	subss  %xmm3,%xmm2
 	mulss  %xmm4,%xmm2
 	andps  %xmm2,%xmm12
 	comiss %xmm12,%xmm7
-	jbe    abe9 <histogramf+0x219>
+	jbe    aba1 <histogramf+0x1f1>
 	cvttss2si %xmm2,%eax
 	pxor   %xmm12,%xmm12
 	cvtsi2ss %eax,%xmm12
 	movaps %xmm12,%xmm14
 	cmpnless %xmm2,%xmm14
-	movss  0xd71c(%rip),%xmm2        
+	movss  0xd764(%rip),%xmm2        
 	andps  %xmm2,%xmm14
 	movaps %xmm12,%xmm2
 	subss  %xmm14,%xmm2
 	cmp    $0x3,%ecx
-	je     b020 <histogramf+0x650>
+	je     afd8 <histogramf+0x628>
 	movss  0xc(%rdi),%xmm5
 	movaps %xmm6,%xmm12
 	subss  %xmm3,%xmm5
 	mulss  %xmm4,%xmm5
 	andps  %xmm5,%xmm12
 	comiss %xmm12,%xmm7
-	jbe    ac3a <histogramf+0x26a>
+	jbe    abf2 <histogramf+0x242>
 	cvttss2si %xmm5,%eax
 	pxor   %xmm12,%xmm12
 	cvtsi2ss %eax,%xmm12
 	movaps %xmm12,%xmm14
 	cmpnless %xmm5,%xmm14
-	movss  0xd6cb(%rip),%xmm5        
+	movss  0xd713(%rip),%xmm5        
 	andps  %xmm5,%xmm14
 	movaps %xmm12,%xmm5
 	subss  %xmm14,%xmm5
 	cmp    $0x4,%ecx
-	je     b020 <histogramf+0x650>
+	je     afd8 <histogramf+0x628>
 	movss  0x10(%rdi),%xmm8
 	movaps %xmm6,%xmm12
 	subss  %xmm3,%xmm8
 	mulss  %xmm4,%xmm8
 	andps  %xmm8,%xmm12
 	comiss %xmm12,%xmm7
-	jbe    ac90 <histogramf+0x2c0>
+	jbe    ac48 <histogramf+0x298>
 	cvttss2si %xmm8,%eax
 	pxor   %xmm12,%xmm12
 	cvtsi2ss %eax,%xmm12
 	movaps %xmm12,%xmm14
 	cmpnless %xmm8,%xmm14
-	movss  0xd675(%rip),%xmm8        
+	movss  0xd6bd(%rip),%xmm8        
 	andps  %xmm8,%xmm14
 	movaps %xmm12,%xmm8
 	subss  %xmm14,%xmm8
 	cmp    $0x5,%ecx
-	je     b020 <histogramf+0x650>
+	je     afd8 <histogramf+0x628>
 	movss  0x14(%rdi),%xmm9
 	movaps %xmm6,%xmm12
 	subss  %xmm3,%xmm9
 	mulss  %xmm4,%xmm9
 	andps  %xmm9,%xmm12
 	comiss %xmm12,%xmm7
-	jbe    ace6 <histogramf+0x316>
+	jbe    ac9e <histogramf+0x2ee>
 	cvttss2si %xmm9,%eax
 	pxor   %xmm12,%xmm12
 	cvtsi2ss %eax,%xmm12
 	movaps %xmm12,%xmm14
 	cmpnless %xmm9,%xmm14
-	movss  0xd61f(%rip),%xmm9        
+	movss  0xd667(%rip),%xmm9        
 	andps  %xmm9,%xmm14
 	movaps %xmm12,%xmm9
 	subss  %xmm14,%xmm9
 	cmp    $0x6,%ecx
-	je     b020 <histogramf+0x650>
+	je     afd8 <histogramf+0x628>
 	movss  0x18(%rdi),%xmm10
 	movaps %xmm6,%xmm12
 	subss  %xmm3,%xmm10
 	mulss  %xmm4,%xmm10
 	andps  %xmm10,%xmm12
 	comiss %xmm12,%xmm7
-	jbe    ad3c <histogramf+0x36c>
+	jbe    acf4 <histogramf+0x344>
 	cvttss2si %xmm10,%eax
 	pxor   %xmm12,%xmm12
 	cvtsi2ss %eax,%xmm12
 	movaps %xmm12,%xmm14
 	cmpnless %xmm10,%xmm14
-	movss  0xd5c9(%rip),%xmm10        
+	movss  0xd611(%rip),%xmm10        
 	andps  %xmm10,%xmm14
 	movaps %xmm12,%xmm10
 	subss  %xmm14,%xmm10
 	cmp    $0x7,%ecx
-	je     b020 <histogramf+0x650>
-	movss  0x1c(%rdi),%xmm11
-	movaps %xmm6,%xmm12
-	subss  %xmm3,%xmm11
-	mulss  %xmm4,%xmm11
-	andps  %xmm11,%xmm12
-	comiss %xmm12,%xmm7
-	jbe    ad89 <histogramf+0x3b9>
-	cvttss2si %xmm11,%eax
-	pxor   %xmm12,%xmm12
-	cvtsi2ss %eax,%xmm12
-	movaps %xmm12,%xmm14
-	cmpnless %xmm11,%xmm14
-	movaps %xmm12,%xmm11
-	andps  %xmm13,%xmm14
-	subss  %xmm14,%xmm11
-	cmp    $0x8,%ecx
-	je     b020 <histogramf+0x650>
-	movss  0x20(%rdi),%xmm12
+	je     afd8 <histogramf+0x628>
+	movss  0x1c(%rdi),%xmm12
 	movaps %xmm6,%xmm14
 	subss  %xmm3,%xmm12
 	mulss  %xmm4,%xmm12
 	andps  %xmm12,%xmm14
 	comiss %xmm14,%xmm7
-	jbe    add6 <histogramf+0x406>
+	jbe    ad41 <histogramf+0x391>
 	cvttss2si %xmm12,%eax
 	pxor   %xmm14,%xmm14
 	cvtsi2ss %eax,%xmm14
 	movaps %xmm14,%xmm15
 	cmpnless %xmm12,%xmm15
 	andps  %xmm13,%xmm15
 	subss  %xmm15,%xmm14
 	movaps %xmm14,%xmm12
 	movd   %xmm12,%r9d
-	cmp    $0x9,%ecx
-	je     b020 <histogramf+0x650>
-	movss  0x24(%rdi),%xmm12
+	cmp    $0x8,%ecx
+	je     afd8 <histogramf+0x628>
+	movss  0x20(%rdi),%xmm12
 	movaps %xmm6,%xmm14
 	subss  %xmm3,%xmm12
 	mulss  %xmm4,%xmm12
 	andps  %xmm12,%xmm14
 	comiss %xmm14,%xmm7
-	jbe    ae28 <histogramf+0x458>
+	jbe    ad93 <histogramf+0x3e3>
 	cvttss2si %xmm12,%eax
 	pxor   %xmm14,%xmm14
 	cvtsi2ss %eax,%xmm14
 	movaps %xmm14,%xmm15
 	cmpnless %xmm12,%xmm15
 	andps  %xmm13,%xmm15
 	subss  %xmm15,%xmm14
 	movaps %xmm14,%xmm12
 	movd   %xmm12,%r10d
-	cmp    $0xa,%ecx
-	je     b020 <histogramf+0x650>
-	movss  0x28(%rdi),%xmm12
+	cmp    $0x9,%ecx
+	je     afd8 <histogramf+0x628>
+	movss  0x24(%rdi),%xmm12
 	movaps %xmm6,%xmm14
 	subss  %xmm3,%xmm12
 	mulss  %xmm4,%xmm12
 	andps  %xmm12,%xmm14
 	comiss %xmm14,%xmm7
-	jbe    ae7a <histogramf+0x4aa>
+	jbe    ade5 <histogramf+0x435>
 	cvttss2si %xmm12,%eax
 	pxor   %xmm14,%xmm14
 	cvtsi2ss %eax,%xmm14
 	movaps %xmm14,%xmm15
 	cmpnless %xmm12,%xmm15
 	andps  %xmm13,%xmm15
 	subss  %xmm15,%xmm14
 	movaps %xmm14,%xmm12
 	movd   %xmm12,%r11d
-	cmp    $0xb,%ecx
-	je     b020 <histogramf+0x650>
-	movss  0x2c(%rdi),%xmm12
+	cmp    $0xa,%ecx
+	je     afd8 <histogramf+0x628>
+	movss  0x28(%rdi),%xmm12
 	movaps %xmm6,%xmm14
 	subss  %xmm3,%xmm12
 	mulss  %xmm4,%xmm12
 	andps  %xmm12,%xmm14
 	comiss %xmm14,%xmm7
-	jbe    aecc <histogramf+0x4fc>
+	jbe    ae37 <histogramf+0x487>
 	cvttss2si %xmm12,%eax
 	pxor   %xmm14,%xmm14
 	cvtsi2ss %eax,%xmm14
 	movaps %xmm14,%xmm15
 	cmpnless %xmm12,%xmm15
 	andps  %xmm13,%xmm15
 	subss  %xmm15,%xmm14
 	movaps %xmm14,%xmm12
 	movss  %xmm12,0xc(%rsp)
-	cmp    $0xc,%ecx
-	je     b020 <histogramf+0x650>
-	movss  0x30(%rdi),%xmm12
+	cmp    $0xb,%ecx
+	je     afd8 <histogramf+0x628>
+	movss  0x2c(%rdi),%xmm12
 	movaps %xmm6,%xmm14
 	subss  %xmm3,%xmm12
 	mulss  %xmm4,%xmm12
 	andps  %xmm12,%xmm14
 	comiss %xmm14,%xmm7
-	jbe    af20 <histogramf+0x550>
+	jbe    ae8b <histogramf+0x4db>
 	cvttss2si %xmm12,%eax
 	pxor   %xmm14,%xmm14
 	cvtsi2ss %eax,%xmm14
 	movaps %xmm14,%xmm15
 	cmpnless %xmm12,%xmm15
 	andps  %xmm13,%xmm15
 	subss  %xmm15,%xmm14
 	movaps %xmm14,%xmm12
 	movd   %xmm12,%r8d
-	cmp    $0xd,%ecx
-	je     b020 <histogramf+0x650>
-	movss  0x34(%rdi),%xmm12
+	cmp    $0xc,%ecx
+	je     afd8 <histogramf+0x628>
+	movss  0x30(%rdi),%xmm12
 	movaps %xmm6,%xmm14
 	subss  %xmm3,%xmm12
 	mulss  %xmm4,%xmm12
 	andps  %xmm12,%xmm14
 	comiss %xmm14,%xmm7
-	jbe    af72 <histogramf+0x5a2>
+	jbe    aedd <histogramf+0x52d>
 	cvttss2si %xmm12,%eax
 	pxor   %xmm14,%xmm14
 	cvtsi2ss %eax,%xmm14
 	movaps %xmm14,%xmm15
 	cmpnless %xmm12,%xmm15
 	andps  %xmm13,%xmm15
 	subss  %xmm15,%xmm14
 	movaps %xmm14,%xmm12
 	movss  %xmm12,0x10(%rsp)
-	cmp    $0xe,%ecx
-	je     b020 <histogramf+0x650>
-	movss  0x38(%rdi),%xmm12
+	cmp    $0xd,%ecx
+	je     afd8 <histogramf+0x628>
+	movss  0x34(%rdi),%xmm12
 	movaps %xmm6,%xmm14
 	subss  %xmm3,%xmm12
 	mulss  %xmm4,%xmm12
 	andps  %xmm12,%xmm14
 	comiss %xmm14,%xmm7
-	jbe    afc6 <histogramf+0x5f6>
+	jbe    af31 <histogramf+0x581>
 	cvttss2si %xmm12,%eax
 	pxor   %xmm14,%xmm14
 	cvtsi2ss %eax,%xmm14
 	movaps %xmm14,%xmm15
 	cmpnless %xmm12,%xmm15
 	andps  %xmm13,%xmm15
 	subss  %xmm15,%xmm14
 	movaps %xmm14,%xmm12
 	movss  %xmm12,0x14(%rsp)
+	cmp    $0xe,%ecx
+	je     afd8 <histogramf+0x628>
+	movss  0x38(%rdi),%xmm11
+	movaps %xmm6,%xmm12
+	subss  %xmm3,%xmm11
+	mulss  %xmm4,%xmm11
+	andps  %xmm11,%xmm12
+	comiss %xmm12,%xmm7
+	jbe    af85 <histogramf+0x5d5>
+	cvttss2si %xmm11,%eax
+	pxor   %xmm12,%xmm12
+	cvtsi2ss %eax,%xmm12
+	movaps %xmm12,%xmm14
+	cmpnless %xmm11,%xmm14
+	movaps %xmm12,%xmm11
+	andps  %xmm13,%xmm14
+	subss  %xmm14,%xmm11
 	cmp    $0xf,%ecx
-	je     b020 <histogramf+0x650>
+	je     afd8 <histogramf+0x628>
 	movss  0x3c(%rdi),%xmm12
 	movaps %xmm6,%xmm14
 	subss  %xmm3,%xmm12
 	mulss  %xmm4,%xmm12
 	andps  %xmm12,%xmm14
 	comiss %xmm14,%xmm7
-	jbe    b016 <histogramf+0x646>
+	jbe    afce <histogramf+0x61e>
 	cvttss2si %xmm12,%eax
 	pxor   %xmm14,%xmm14
 	cvtsi2ss %eax,%xmm14
 	movaps %xmm14,%xmm15
 	cmpnless %xmm12,%xmm15
 	andps  %xmm13,%xmm15
 	subss  %xmm15,%xmm14
 	movaps %xmm14,%xmm12
 	movss  %xmm12,0x18(%rsp)
 	nopl   (%rax)
 	cvttss2si %xmm1,%eax
 	cmp    %eax,%r12d
-	jle    b046 <histogramf+0x676>
+	jle    affe <histogramf+0x64e>
 	test   %eax,%eax
-	js     b046 <histogramf+0x676>
+	js     affe <histogramf+0x64e>
 	mov    (%r15),%rsi
 	cltq
-	movss  0xd2be(%rip),%xmm1        
+	movss  0xd306(%rip),%xmm1        
 	lea    (%rsi,%rax,4),%rax
 	addss  (%rax),%xmm1
 	movss  %xmm1,(%rax)
 	cmp    $0x1,%ecx
-	je     b320 <histogramf+0x950>
+	je     b2e0 <histogramf+0x930>
 	cvttss2si %xmm0,%eax
 	cmp    %eax,%r12d
-	jle    b075 <histogramf+0x6a5>
+	jle    b02d <histogramf+0x67d>
 	test   %eax,%eax
-	js     b075 <histogramf+0x6a5>
+	js     b02d <histogramf+0x67d>
 	mov    (%r15),%rsi
 	cltq
-	movss  0xd28f(%rip),%xmm1        
+	movss  0xd2d7(%rip),%xmm1        
 	lea    (%rsi,%rax,4),%rax
 	addss  (%rax),%xmm1
 	movss  %xmm1,(%rax)
 	cmp    $0x2,%ecx
-	je     b320 <histogramf+0x950>
+	je     b2e0 <histogramf+0x930>
 	cvttss2si %xmm2,%eax
 	cmp    %eax,%r12d
-	jle    b0a4 <histogramf+0x6d4>
+	jle    b05c <histogramf+0x6ac>
 	test   %eax,%eax
-	js     b0a4 <histogramf+0x6d4>
+	js     b05c <histogramf+0x6ac>
 	mov    (%r15),%rsi
 	cltq
-	movss  0xd260(%rip),%xmm1        
+	movss  0xd2a8(%rip),%xmm1        
 	lea    (%rsi,%rax,4),%rax
 	addss  (%rax),%xmm1
 	movss  %xmm1,(%rax)
 	cmp    $0x3,%ecx
-	je     b320 <histogramf+0x950>
+	je     b2e0 <histogramf+0x930>
 	cvttss2si %xmm5,%eax
 	cmp    %eax,%r12d
-	jle    b0d3 <histogramf+0x703>
+	jle    b08b <histogramf+0x6db>
 	test   %eax,%eax
-	js     b0d3 <histogramf+0x703>
+	js     b08b <histogramf+0x6db>
 	mov    (%r15),%rsi
 	cltq
-	movss  0xd231(%rip),%xmm1        
+	movss  0xd279(%rip),%xmm1        
 	lea    (%rsi,%rax,4),%rax
 	addss  (%rax),%xmm1
 	movss  %xmm1,(%rax)
 	cmp    $0x4,%ecx
-	je     b320 <histogramf+0x950>
+	je     b2e0 <histogramf+0x930>
 	cvttss2si %xmm8,%eax
 	cmp    %eax,%r12d
-	jle    b103 <histogramf+0x733>
+	jle    b0bb <histogramf+0x70b>
 	test   %eax,%eax
-	js     b103 <histogramf+0x733>
+	js     b0bb <histogramf+0x70b>
 	mov    (%r15),%rsi
 	cltq
-	movss  0xd201(%rip),%xmm1        
+	movss  0xd249(%rip),%xmm1        
 	lea    (%rsi,%rax,4),%rax
 	addss  (%rax),%xmm1
 	movss  %xmm1,(%rax)
 	cmp    $0x5,%ecx
-	je     b320 <histogramf+0x950>
+	je     b2e0 <histogramf+0x930>
 	cvttss2si %xmm9,%eax
 	test   %eax,%eax
-	js     b133 <histogramf+0x763>
+	js     b0eb <histogramf+0x73b>
 	cmp    %eax,%r12d
-	jle    b133 <histogramf+0x763>
+	jle    b0eb <histogramf+0x73b>
 	mov    (%r15),%rsi
 	cltq
-	movss  0xd1d1(%rip),%xmm1        
+	movss  0xd219(%rip),%xmm1        
 	lea    (%rsi,%rax,4),%rax
 	addss  (%rax),%xmm1
 	movss  %xmm1,(%rax)
 	cmp    $0x6,%ecx
-	je     b320 <histogramf+0x950>
+	je     b2e0 <histogramf+0x930>
 	cvttss2si %xmm10,%eax
 	test   %eax,%eax
-	js     b163 <histogramf+0x793>
+	js     b11b <histogramf+0x76b>
 	cmp    %eax,%r12d
-	jle    b163 <histogramf+0x793>
+	jle    b11b <histogramf+0x76b>
 	mov    (%r15),%rsi
 	cltq
-	movss  0xd1a1(%rip),%xmm1        
+	movss  0xd1e9(%rip),%xmm1        
 	lea    (%rsi,%rax,4),%rax
 	addss  (%rax),%xmm1
 	movss  %xmm1,(%rax)
 	cmp    $0x7,%ecx
-	je     b320 <histogramf+0x950>
-	cvttss2si %xmm11,%eax
+	je     b2e0 <histogramf+0x930>
+	movd   %r9d,%xmm1
+	cvttss2si %xmm1,%eax
 	test   %eax,%eax
-	js     b193 <histogramf+0x7c3>
+	js     b14f <histogramf+0x79f>
 	cmp    %eax,%r12d
-	jle    b193 <histogramf+0x7c3>
+	jle    b14f <histogramf+0x79f>
 	mov    (%r15),%rsi
 	cltq
-	movss  0xd171(%rip),%xmm1        
+	movss  0xd1b5(%rip),%xmm1        
 	lea    (%rsi,%rax,4),%rax
 	addss  (%rax),%xmm1
 	movss  %xmm1,(%rax)
 	cmp    $0x8,%ecx
-	je     b320 <histogramf+0x950>
-	movd   %r9d,%xmm1
+	je     b2e0 <histogramf+0x930>
+	movd   %r10d,%xmm1
 	cvttss2si %xmm1,%eax
 	test   %eax,%eax
-	js     b1c7 <histogramf+0x7f7>
+	js     b183 <histogramf+0x7d3>
 	cmp    %eax,%r12d
-	jle    b1c7 <histogramf+0x7f7>
+	jle    b183 <histogramf+0x7d3>
 	mov    (%r15),%rsi
 	cltq
-	movss  0xd13d(%rip),%xmm1        
+	movss  0xd181(%rip),%xmm1        
 	lea    (%rsi,%rax,4),%rax
 	addss  (%rax),%xmm1
 	movss  %xmm1,(%rax)
 	cmp    $0x9,%ecx
-	je     b320 <histogramf+0x950>
-	movd   %r10d,%xmm1
+	je     b2e0 <histogramf+0x930>
+	movd   %r11d,%xmm1
 	cvttss2si %xmm1,%eax
 	test   %eax,%eax
-	js     b1fb <histogramf+0x82b>
+	js     b1b7 <histogramf+0x807>
 	cmp    %eax,%r12d
-	jle    b1fb <histogramf+0x82b>
+	jle    b1b7 <histogramf+0x807>
 	mov    (%r15),%rsi
 	cltq
-	movss  0xd109(%rip),%xmm1        
+	movss  0xd14d(%rip),%xmm1        
 	lea    (%rsi,%rax,4),%rax
 	addss  (%rax),%xmm1
 	movss  %xmm1,(%rax)
 	cmp    $0xa,%ecx
-	je     b320 <histogramf+0x950>
-	movd   %r11d,%xmm1
-	cvttss2si %xmm1,%eax
+	je     b2e0 <histogramf+0x930>
+	cvttss2si 0xc(%rsp),%eax
 	test   %eax,%eax
-	js     b22f <histogramf+0x85f>
+	js     b1e8 <histogramf+0x838>
 	cmp    %eax,%r12d
-	jle    b22f <histogramf+0x85f>
+	jle    b1e8 <histogramf+0x838>
 	mov    (%r15),%rsi
 	cltq
-	movss  0xd0d5(%rip),%xmm1        
+	movss  0xd11c(%rip),%xmm1        
 	lea    (%rsi,%rax,4),%rax
 	addss  (%rax),%xmm1
 	movss  %xmm1,(%rax)
 	cmp    $0xb,%ecx
-	je     b320 <histogramf+0x950>
-	cvttss2si 0xc(%rsp),%eax
+	je     b2e0 <histogramf+0x930>
+	movd   %r8d,%xmm1
+	cvttss2si %xmm1,%eax
 	test   %eax,%eax
-	js     b260 <histogramf+0x890>
+	js     b21c <histogramf+0x86c>
 	cmp    %eax,%r12d
-	jle    b260 <histogramf+0x890>
+	jle    b21c <histogramf+0x86c>
 	mov    (%r15),%rsi
 	cltq
-	movss  0xd0a4(%rip),%xmm1        
+	movss  0xd0e8(%rip),%xmm1        
 	lea    (%rsi,%rax,4),%rax
 	addss  (%rax),%xmm1
 	movss  %xmm1,(%rax)
 	cmp    $0xc,%ecx
-	je     b320 <histogramf+0x950>
-	movd   %r8d,%xmm1
-	cvttss2si %xmm1,%eax
+	je     b2e0 <histogramf+0x930>
+	cvttss2si 0x10(%rsp),%eax
 	test   %eax,%eax
-	js     b294 <histogramf+0x8c4>
+	js     b24d <histogramf+0x89d>
 	cmp    %eax,%r12d
-	jle    b294 <histogramf+0x8c4>
+	jle    b24d <histogramf+0x89d>
 	mov    (%r15),%rsi
 	cltq
-	movss  0xd070(%rip),%xmm1        
+	movss  0xd0b7(%rip),%xmm1        
 	lea    (%rsi,%rax,4),%rax
 	addss  (%rax),%xmm1
 	movss  %xmm1,(%rax)
 	cmp    $0xd,%ecx
-	je     b320 <histogramf+0x950>
-	cvttss2si 0x10(%rsp),%eax
+	je     b2e0 <histogramf+0x930>
+	cvttss2si 0x14(%rsp),%eax
 	test   %eax,%eax
-	js     b2c5 <histogramf+0x8f5>
+	js     b27e <histogramf+0x8ce>
 	cmp    %eax,%r12d
-	jle    b2c5 <histogramf+0x8f5>
+	jle    b27e <histogramf+0x8ce>
 	mov    (%r15),%rsi
 	cltq
-	movss  0xd03f(%rip),%xmm1        
+	movss  0xd086(%rip),%xmm1        
 	lea    (%rsi,%rax,4),%rax
 	addss  (%rax),%xmm1
 	movss  %xmm1,(%rax)
 	cmp    $0xe,%ecx
-	je     b320 <histogramf+0x950>
-	cvttss2si 0x14(%rsp),%eax
+	je     b2e0 <histogramf+0x930>
+	cvttss2si %xmm11,%eax
 	test   %eax,%eax
-	js     b2f2 <histogramf+0x922>
+	js     b2aa <histogramf+0x8fa>
 	cmp    %eax,%r12d
-	jle    b2f2 <histogramf+0x922>
+	jle    b2aa <histogramf+0x8fa>
 	mov    (%r15),%rsi
 	cltq
-	movss  0xd012(%rip),%xmm1        
+	movss  0xd05a(%rip),%xmm1        
 	lea    (%rsi,%rax,4),%rax
 	addss  (%rax),%xmm1
 	movss  %xmm1,(%rax)
 	cmp    $0xf,%ecx
-	je     b320 <histogramf+0x950>
+	je     b2e0 <histogramf+0x930>
 	cvttss2si 0x18(%rsp),%eax
 	test   %eax,%eax
-	js     b320 <histogramf+0x950>
+	js     b2e0 <histogramf+0x930>
 	cmp    %eax,%r12d
-	jle    b320 <histogramf+0x950>
+	jle    b2e0 <histogramf+0x930>
 	mov    (%r15),%rsi
 	cltq
-	movss  0xcfe5(%rip),%xmm1        
+	movss  0xd02d(%rip),%xmm1        
 	lea    (%rsi,%rax,4),%rax
 	addss  (%rax),%xmm1
 	movss  %xmm1,(%rax)
-	nop
+	nopw   0x0(%rax,%rax,1)
 	sub    $0x10,%ecx
 	add    $0x40,%rdi
 	cmp    %ecx,%edx
-	jne    ab08 <histogramf+0x138>
+	jne    aac0 <histogramf+0x110>
 	test   %r12d,%r12d
-	jle    b380 <histogramf+0x9b0>
+	jle    b340 <histogramf+0x990>
 	shl    $0x2,%rbx
 	xor    %esi,%esi
 	mov    %r14,%rdi
 	mov    %rbx,%rdx
 	call   30f0 <memset@plt>
 	lea    -0x1(%r13),%eax
 	xor    %ecx,%ecx
 	lea    0x8(%rbp,%rax,8),%rsi
 	test   %r13d,%r13d
-	jle    b377 <histogramf+0x9a7>
+	jle    b337 <histogramf+0x987>
 	mov    %rbp,%rax
 	pxor   %xmm0,%xmm0
 	nopl   0x0(%rax)
 	mov    (%rax),%rdx
 	add    $0x8,%rax
 	addss  (%rdx,%rcx,1),%xmm0
 	cmp    %rsi,%rax
-	jne    b360 <histogramf+0x990>
+	jne    b320 <histogramf+0x970>
 	movss  %xmm0,(%r14,%rcx,1)
 	add    $0x4,%rcx
 	cmp    %rcx,%rbx
-	jne    b350 <histogramf+0x980>
-	add    $0x68,%rsp
+	jne    b310 <histogramf+0x960>
+	add    $0x28,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
@@ -7145,40 +7139,40 @@
 	xor    %ebp,%ebp
 	xor    %r15d,%r15d
 	movss  %xmm4,0x10(%rsp)
 	call   31c0 <omp_get_max_threads()@plt>
 	movslq %eax,%rdi
 	shl    $0x3,%rdi
 	call   31a0 <malloc@plt>
-	mov    %rax,0x10dc8(%rip)        
+	mov    %rax,0x10e08(%rip)        
 	call   31c0 <omp_get_max_threads()@plt>
-	mov    0x10dbc(%rip),%r13        
+	mov    0x10dfc(%rip),%r13        
 	imul   %ebx,%eax
 	movslq %eax,%rdi
 	shl    $0x2,%rdi
 	call   31a0 <malloc@plt>
 	mov    %rax,0x0(%r13)
 	lea    0x0(,%rbx,4),%r13
-	jmp    b400 <histogramf+0xa30>
+	jmp    b3c0 <histogramf+0xa10>
 	nopl   0x0(%rax)
-	mov    0x10d91(%rip),%rax        
+	mov    0x10dd1(%rip),%rax        
 	mov    (%rax),%rdx
 	add    %rbp,%rdx
 	add    %r13,%rbp
 	mov    %rdx,(%rax,%r15,8)
 	add    $0x1,%r15
 	call   31c0 <omp_get_max_threads()@plt>
 	cmp    %r15d,%eax
-	jg     b3e8 <histogramf+0xa18>
+	jg     b3a8 <histogramf+0x9f8>
 	movss  0x10(%rsp),%xmm4
 	movss  0x14(%rsp),%xmm3
-	jmp    aa11 <histogramf+0x41>
+	jmp    a9f1 <histogramf+0x41>
 	nopl   0x0(%rax,%rax,1)
 
-000000000000b420 <smooth_histogramf>:
+000000000000b3e0 <smooth_histogramf>:
 smooth_histogramf():
 	push   %r15
 	pxor   %xmm2,%xmm2
 	movaps %xmm0,%xmm6
 	pxor   %xmm5,%xmm5
 	push   %r14
 	cvtsi2ss %edx,%xmm2
@@ -7200,15 +7194,15 @@
 	mov    %rdi,0x20(%rsp)
 	divss  %xmm0,%xmm7
 	divss  %xmm2,%xmm0
 	pxor   %xmm2,%xmm2
 	cvtss2sd %xmm6,%xmm2
 	movss  %xmm7,0x10(%rsp)
 	cvtss2sd %xmm0,%xmm0
-	mulsd  0xce47(%rip),%xmm0        
+	mulsd  0xce87(%rip),%xmm0        
 	addsd  %xmm0,%xmm2
 	subsd  %xmm0,%xmm1
 	cvtsd2ss %xmm2,%xmm2
 	cvtsd2ss %xmm1,%xmm5
 	movss  %xmm2,0x8(%rsp)
 	movss  %xmm5,0xc(%rsp)
 	call   31c0 <omp_get_max_threads()@plt>
@@ -7223,130 +7217,130 @@
 	call   31a0 <malloc@plt>
 	mov    %rax,(%r12)
 	mov    %rax,%rbp
 	movslq %r14d,%rax
 	xor    %r14d,%r14d
 	mov    %rax,0x28(%rsp)
 	lea    0x0(,%rax,4),%r13
-	jmp    b502 <smooth_histogramf+0xe2>
+	jmp    b4c2 <smooth_histogramf+0xe2>
 	nopw   0x0(%rax,%rax,1)
 	add    %r14,%rbp
 	add    %r13,%r14
 	mov    %rbp,(%r12,%r15,8)
 	mov    (%r12),%rbp
 	add    $0x1,%r15
 	call   31c0 <omp_get_max_threads()@plt>
 	cmp    %r15d,%eax
-	jg     b4f0 <smooth_histogramf+0xd0>
+	jg     b4b0 <smooth_histogramf+0xd0>
 	call   3040 <omp_get_thread_num()@plt>
 	mov    %eax,%r14d
 	call   3090 <omp_get_num_threads()@plt>
 	mov    %r13,%rdx
 	xor    %esi,%esi
 	mov    %eax,%r15d
 	movslq %r14d,%rax
 	mov    (%r12,%rax,8),%rcx
 	mov    %rcx,%rdi
 	call   30f0 <memset@plt>
 	mov    0x18(%rsp),%edx
 	mov    %rax,%rcx
 	test   %edx,%edx
-	jle    b620 <smooth_histogramf+0x200>
+	jle    b5e0 <smooth_histogramf+0x200>
 	mov    0x18(%rsp),%eax
 	mov    0x20(%rsp),%rdi
-	movsd  0xcd88(%rip),%xmm2        
+	movsd  0xcdc8(%rip),%xmm2        
 	sub    $0x1,%eax
 	lea    0x4(%rdi,%rax,4),%rax
-	jmp    b5c3 <smooth_histogramf+0x1a3>
+	jmp    b583 <smooth_histogramf+0x1a3>
 	nopw   0x0(%rax,%rax,1)
 	addsd  %xmm2,%xmm0
 	cvttsd2si %xmm0,%esi
-	movsd  0xcd60(%rip),%xmm3        
+	movsd  0xcda0(%rip),%xmm3        
 	pxor   %xmm0,%xmm0
 	movslq %edx,%rdx
 	movslq %esi,%rsi
 	cvtss2sd %xmm1,%xmm0
 	lea    (%rcx,%rdx,4),%rdx
 	pxor   %xmm1,%xmm1
 	subsd  %xmm0,%xmm3
 	cvtss2sd (%rdx),%xmm1
-	addsd  0xcd3a(%rip),%xmm0        
+	addsd  0xcd7a(%rip),%xmm0        
 	addsd  %xmm3,%xmm1
 	cvtsd2ss %xmm1,%xmm1
 	movss  %xmm1,(%rdx)
 	lea    (%rcx,%rsi,4),%rdx
 	pxor   %xmm1,%xmm1
 	cvtss2sd (%rdx),%xmm1
 	addsd  %xmm1,%xmm0
 	cvtsd2ss %xmm0,%xmm0
 	movss  %xmm0,(%rdx)
 	add    $0x4,%rdi
 	cmp    %rdi,%rax
-	je     b620 <smooth_histogramf+0x200>
+	je     b5e0 <smooth_histogramf+0x200>
 	movss  (%rdi),%xmm0
 	movss  0x8(%rsp),%xmm4
 	comiss %xmm0,%xmm4
-	ja     b5ba <smooth_histogramf+0x19a>
+	ja     b57a <smooth_histogramf+0x19a>
 	comiss 0xc(%rsp),%xmm0
-	ja     b5ba <smooth_histogramf+0x19a>
+	ja     b57a <smooth_histogramf+0x19a>
 	subss  0x14(%rsp),%xmm0
 	mulss  0x10(%rsp),%xmm0
 	pxor   %xmm3,%xmm3
 	cvttss2si %xmm0,%edx
 	movaps %xmm0,%xmm1
 	cvtss2sd %xmm0,%xmm0
 	cvtsi2ss %edx,%xmm3
 	subss  %xmm3,%xmm1
-	comiss 0xccf1(%rip),%xmm1        
-	ja     b560 <smooth_histogramf+0x140>
+	comiss 0xcd31(%rip),%xmm1        
+	ja     b520 <smooth_histogramf+0x140>
 	subsd  %xmm2,%xmm0
 	cvttsd2si %xmm0,%esi
-	jmp    b568 <smooth_histogramf+0x148>
+	jmp    b528 <smooth_histogramf+0x148>
 	cs nopw 0x0(%rax,%rax,1)
 	mov    0x1c(%rsp),%eax
 	test   %eax,%eax
-	jle    b67f <smooth_histogramf+0x25f>
+	jle    b63f <smooth_histogramf+0x25f>
 	mov    0x28(%rsp),%r13
 	xor    %esi,%esi
 	mov    %rbx,%rdi
 	shl    $0x2,%r13
 	mov    %r13,%rdx
 	call   30f0 <memset@plt>
 	lea    -0x1(%r15),%eax
 	xor    %ecx,%ecx
 	lea    0x8(%r12,%rax,8),%rsi
 	nopl   0x0(%rax)
 	test   %r15d,%r15d
-	jle    b676 <smooth_histogramf+0x256>
+	jle    b636 <smooth_histogramf+0x256>
 	mov    %r12,%rax
 	pxor   %xmm0,%xmm0
 	nopl   0x0(%rax)
 	mov    (%rax),%rdx
 	add    $0x8,%rax
 	addss  (%rdx,%rcx,1),%xmm0
 	cmp    %rax,%rsi
-	jne    b660 <smooth_histogramf+0x240>
+	jne    b620 <smooth_histogramf+0x240>
 	movss  %xmm0,(%rbx,%rcx,1)
 	add    $0x4,%rcx
 	cmp    %r13,%rcx
-	jne    b650 <smooth_histogramf+0x230>
+	jne    b610 <smooth_histogramf+0x230>
 	mov    %rbp,%rdi
 	call   3180 <free@plt>
 	add    $0x38,%rsp
 	mov    %r12,%rdi
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	jmp    3180 <free@plt>
 	nopl   (%rax)
 
-000000000000b6a0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
+000000000000b660 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
 void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]:
 	lea    -0x1(%rdx),%rax
 	push   %rbp
 	mov    %rdx,%rbp
 	mov    %rsi,%r8
 	mov    %rax,%r11
 	push   %rbx
@@ -7356,219 +7350,219 @@
 	movq   %xmm0,%r9
 	add    %rax,%r11
 	movq   %xmm0,%rax
 	shr    $0x20,%rax
 	sar    %r11
 	movq   %rax,%xmm1
 	cmp    %r11,%rsi
-	jl     b6ef <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x4f>
-	jmp    b790 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xf0>
+	jl     b6af <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x4f>
+	jmp    b750 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xf0>
 	nopl   0x0(%rax)
 	mov    (%rax),%rcx
 	mov    %rcx,(%rdi,%rsi,8)
 	cmp    %rdx,%r11
-	jle    b72e <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x8e>
+	jle    b6ee <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x8e>
 	mov    %rdx,%rsi
 	lea    0x1(%rsi),%rax
 	lea    (%rax,%rax,1),%rdx
 	shl    $0x4,%rax
 	lea    -0x1(%rdx),%rcx
 	add    %rdi,%rax
 	lea    (%rdi,%rcx,8),%r10
 	movss  0x4(%r10),%xmm0
 	comiss 0x4(%rax),%xmm0
-	jbe    b6e0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x40>
+	jbe    b6a0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x40>
 	mov    (%r10),%rax
 	mov    %rax,(%rdi,%rsi,8)
 	cmp    %rcx,%r11
-	jle    b728 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x88>
+	jle    b6e8 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x88>
 	mov    %rcx,%rdx
-	jmp    b6ec <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x4c>
+	jmp    b6ac <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x4c>
 	nopl   0x0(%rax,%rax,1)
 	mov    %r10,%rax
 	mov    %rcx,%rdx
 	test   %rbp,%rbp
-	je     b7a0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x100>
+	je     b760 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x100>
 	lea    -0x1(%rdx),%rsi
 	mov    %rsi,%rcx
 	shr    $0x3f,%rcx
 	add    %rsi,%rcx
 	sar    %rcx
 	cmp    %r8,%rdx
-	jg     b772 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xd2>
-	jmp    b780 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe0>
+	jg     b732 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xd2>
+	jmp    b740 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe0>
 	nopl   0x0(%rax,%rax,1)
 	mov    (%rsi),%rdx
 	mov    %rdx,(%rax)
 	lea    -0x1(%rcx),%rdx
 	mov    %rdx,%rax
 	shr    $0x3f,%rax
 	add    %rdx,%rax
 	mov    %rcx,%rdx
 	sar    %rax
 	cmp    %rcx,%r8
-	jge    b7d8 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x138>
+	jge    b798 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x138>
 	mov    %rax,%rcx
 	lea    (%rdi,%rcx,8),%rsi
 	lea    (%rdi,%rdx,8),%rax
 	comiss 0x4(%rsi),%xmm1
-	ja     b750 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb0>
+	ja     b710 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb0>
 	mov    %r9,(%rax)
 	pop    %rbx
 	pop    %rbp
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 	lea    (%rdi,%rsi,8),%rax
 	test   %rbp,%rbp
-	jne    b780 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe0>
+	jne    b740 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe0>
 	mov    %r8,%rdx
 	nopl   0x0(%rax)
 	lea    -0x2(%rbx),%rcx
 	mov    %rcx,%rbx
 	shr    $0x3f,%rbx
 	add    %rcx,%rbx
 	sar    %rbx
 	cmp    %rdx,%rbx
-	jne    b733 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x93>
+	jne    b6f3 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x93>
 	lea    0x1(%rdx,%rdx,1),%rdx
 	lea    (%rdi,%rdx,8),%rcx
 	mov    (%rcx),%rsi
 	mov    %rsi,(%rax)
 	mov    %rcx,%rax
-	jmp    b733 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x93>
+	jmp    b6f3 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x93>
 	nopl   0x0(%rax)
 	mov    %rsi,%rax
 	mov    %r9,(%rax)
 	pop    %rbx
 	pop    %rbp
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
-000000000000b7f0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
+000000000000b7b0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
 void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]:
 	lea    -0x1(%rdx),%rax
 	push   %rbx
 	mov    %rdx,%rbx
 	mov    %rdx,%r11
 	mov    %rax,%r10
 	and    $0x1,%ebx
 	shr    $0x3f,%r10
 	add    %rax,%r10
 	sar    %r10
 	cmp    %r10,%rsi
-	jge    b8f0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x100>
+	jge    b8b0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x100>
 	mov    %rsi,%rdx
-	jmp    b830 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x40>
+	jmp    b7f0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x40>
 	nopl   0x0(%rax)
 	movdqu (%rax),%xmm4
 	movups %xmm4,(%rdi,%rdx,1)
 	cmp    %rcx,%r10
-	jle    b87e <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x8e>
+	jle    b83e <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x8e>
 	mov    %rcx,%rdx
 	lea    0x1(%rdx),%rax
 	shl    $0x4,%rdx
 	lea    (%rax,%rax,1),%rcx
 	shl    $0x5,%rax
 	lea    -0x1(%rcx),%r9
 	add    %rdi,%rax
 	mov    %r9,%r8
 	shl    $0x4,%r8
 	add    %rdi,%r8
 	movsd  0x8(%r8),%xmm2
 	comisd 0x8(%rax),%xmm2
-	jbe    b820 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x30>
+	jbe    b7e0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x30>
 	movdqu (%r8),%xmm5
 	movups %xmm5,(%rdi,%rdx,1)
 	cmp    %r9,%r10
-	jle    b878 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x88>
+	jle    b838 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x88>
 	mov    %r9,%rcx
-	jmp    b82d <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x3d>
+	jmp    b7ed <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x3d>
 	nopl   0x0(%rax)
 	mov    %r8,%rax
 	mov    %r9,%rcx
 	test   %rbx,%rbx
-	je     b908 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x118>
+	je     b8c8 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x118>
 	lea    -0x1(%rcx),%rdx
 	mov    %rdx,%r8
 	shr    $0x3f,%r8
 	add    %rdx,%r8
 	sar    %r8
 	cmp    %rsi,%rcx
-	jg     b8c7 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xd7>
-	jmp    b8e0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xf0>
+	jg     b887 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xd7>
+	jmp    b8a0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xf0>
 	nop
 	movdqu (%rdx),%xmm3
 	lea    -0x1(%r8),%rcx
 	movups %xmm3,(%rax)
 	mov    %rcx,%rax
 	shr    $0x3f,%rax
 	add    %rcx,%rax
 	mov    %r8,%rcx
 	sar    %rax
 	cmp    %r8,%rsi
-	jge    b940 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x150>
+	jge    b900 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x150>
 	mov    %rax,%r8
 	mov    %r8,%rdx
 	shl    $0x4,%rcx
 	shl    $0x4,%rdx
 	lea    (%rdi,%rcx,1),%rax
 	add    %rdi,%rdx
 	comisd 0x8(%rdx),%xmm1
-	ja     b8a0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb0>
+	ja     b860 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb0>
 	unpcklpd %xmm1,%xmm0
 	movups %xmm0,(%rax)
 	pop    %rbx
 	ret
 	nopl   0x0(%rax)
 	mov    %rsi,%rax
 	shl    $0x4,%rax
 	add    %rdi,%rax
 	test   %rbx,%rbx
-	jne    b8e0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xf0>
+	jne    b8a0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xf0>
 	mov    %rsi,%rcx
 	nopw   0x0(%rax,%rax,1)
 	lea    -0x2(%r11),%rdx
 	mov    %rdx,%r11
 	shr    $0x3f,%r11
 	add    %rdx,%r11
 	sar    %r11
 	cmp    %rcx,%r11
-	jne    b887 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x97>
+	jne    b847 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x97>
 	lea    0x1(%rcx,%rcx,1),%rcx
 	mov    %rcx,%rdx
 	shl    $0x4,%rdx
 	add    %rdi,%rdx
 	movdqu (%rdx),%xmm6
 	movups %xmm6,(%rax)
 	mov    %rdx,%rax
-	jmp    b887 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x97>
+	jmp    b847 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x97>
 	mov    %rdx,%rax
 	unpcklpd %xmm1,%xmm0
 	movups %xmm0,(%rax)
 	pop    %rbx
 	ret
 	nopl   0x0(%rax)
 
-000000000000b950 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
+000000000000b910 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
 void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]:
 	mov    %rsi,%rax
 	sub    %rdi,%rax
 	cmp    $0x80,%rax
-	jle    bb4f <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1ff>
+	jle    bb0f <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1ff>
 	push   %r14
 	mov    %rdx,%r14
 	push   %r13
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	mov    %rsi,%rbp
 	push   %rbx
 	test   %rdx,%rdx
-	je     bae2 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x192>
+	je     baa2 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x192>
 	lea    0x8(%rdi),%r13
 	mov    %rsi,%rax
 	movss  0xc(%r12),%xmm1
 	sub    $0x1,%r14
 	movss  -0x4(%rsi),%xmm3
 	sub    %r12,%rax
 	movss  (%r12),%xmm4
@@ -7577,134 +7571,134 @@
 	shr    $0x3f,%rax
 	sar    $0x3,%rdx
 	add    %rdx,%rax
 	sar    %rax
 	lea    (%r12,%rax,8),%rax
 	movss  0x4(%rax),%xmm0
 	comiss %xmm1,%xmm0
-	jbe    ba67 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x117>
+	jbe    ba27 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x117>
 	comiss %xmm0,%xmm3
-	ja     bac8 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x178>
+	ja     ba88 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x178>
 	comiss %xmm1,%xmm3
-	ja     ba75 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x125>
+	ja     ba35 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x125>
 	mov    0x8(%r12),%rax
 	movss  %xmm2,0xc(%r12)
 	movss  %xmm4,0x8(%r12)
 	mov    %rax,(%r12)
 	movss  -0x4(%rsi),%xmm2
 	movss  0x4(%r12),%xmm0
 	mov    %r13,%rbx
 	mov    %rsi,%rdx
 	nopl   0x0(%rax)
 	movss  0x4(%rbx),%xmm1
 	mov    %rbx,%rbp
 	comiss %xmm1,%xmm0
-	ja     ba61 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x111>
+	ja     ba21 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x111>
 	comiss %xmm0,%xmm2
 	lea    -0x8(%rdx),%rcx
 	lea    -0x10(%rdx),%rax
-	jbe    bac0 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x170>
+	jbe    ba80 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x170>
 	cs nopw 0x0(%rax,%rax,1)
 	mov    %rax,%rdx
 	sub    $0x8,%rax
 	comiss 0xc(%rax),%xmm0
-	jb     ba30 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe0>
+	jb     b9f0 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe0>
 	cmp    %rbx,%rdx
-	jbe    ba90 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x140>
+	jbe    ba50 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x140>
 	movss  (%rbx),%xmm0
 	mov    (%rdx),%rax
 	mov    %rax,(%rbx)
 	movss  -0x4(%rdx),%xmm2
 	movss  %xmm0,(%rdx)
 	movss  %xmm1,0x4(%rdx)
 	movss  0x4(%r12),%xmm0
 	add    $0x8,%rbx
-	jmp    ba08 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb8>
+	jmp    b9c8 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb8>
 	comiss %xmm1,%xmm3
-	ja     b9d8 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x88>
+	ja     b998 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x88>
 	comiss %xmm0,%xmm3
-	jbe    bac8 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x178>
+	jbe    ba88 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x178>
 	mov    -0x8(%rsi),%rax
 	mov    %rax,(%r12)
 	movss  %xmm4,-0x8(%rsi)
 	movss  %xmm2,-0x4(%rsi)
-	jmp    b9f4 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xa4>
+	jmp    b9b4 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xa4>
 	nopl   0x0(%rax)
 	mov    %r14,%rdx
 	mov    %rbx,%rdi
-	call   b950 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   b910 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	mov    %rbx,%rax
 	sub    %r12,%rax
 	cmp    $0x80,%rax
-	jle    bb46 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1f6>
+	jle    bb06 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1f6>
 	test   %r14,%r14
-	je     bae2 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x192>
+	je     baa2 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x192>
 	mov    %rbx,%rsi
-	jmp    b980 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x30>
+	jmp    b940 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x30>
 	nopw   0x0(%rax,%rax,1)
 	mov    %rcx,%rdx
-	jmp    ba3d <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xed>
+	jmp    b9fd <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xed>
 	mov    (%rax),%rdx
 	mov    %rdx,(%r12)
 	movss  %xmm2,0x4(%rax)
 	movss  -0x4(%rsi),%xmm2
 	movss  %xmm4,(%rax)
-	jmp    b9f4 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xa4>
+	jmp    b9b4 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xa4>
 	sar    $0x3,%rax
 	lea    -0x2(%rax),%r13
 	mov    %rax,%rbx
 	sar    %r13
-	jmp    baf6 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1a6>
+	jmp    bab6 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1a6>
 	sub    $0x1,%r13
 	movq   (%r12,%r13,8),%xmm0
 	mov    %rbx,%rdx
 	mov    %r13,%rsi
 	mov    %r12,%rdi
-	call   b6a0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   b660 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	test   %r13,%r13
-	jne    baf2 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1a2>
+	jne    bab2 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1a2>
 	sub    $0x8,%rbp
 	nopl   0x0(%rax,%rax,1)
 	mov    (%r12),%rax
 	mov    %rbp,%rbx
 	movq   0x0(%rbp),%xmm0
 	xor    %esi,%esi
 	sub    %r12,%rbx
 	mov    %r12,%rdi
 	sub    $0x8,%rbp
 	mov    %rax,0x8(%rbp)
 	mov    %rbx,%rdx
 	sar    $0x3,%rdx
-	call   b6a0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   b660 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, long, particle<float>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	cmp    $0x8,%rbx
-	jg     bb18 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1c8>
+	jg     bad8 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1c8>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	ret
 
-000000000000bb50 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
+000000000000bb10 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
 void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]:
 	mov    %rsi,%rax
 	sub    %rdi,%rax
 	cmp    $0x100,%rax
-	jle    bd6e <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x21e>
+	jle    bd2e <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x21e>
 	push   %r14
 	mov    %rdx,%r14
 	push   %r13
 	mov    %rdi,%r13
 	push   %r12
 	push   %rbp
 	mov    %rsi,%rbp
 	push   %rbx
 	test   %rdx,%rdx
-	je     bce2 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x192>
+	je     bca2 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x192>
 	lea    0x10(%rdi),%r12
 	mov    %rsi,%rax
 	movsd  0x18(%r13),%xmm3
 	sub    $0x1,%r14
 	movsd  -0x8(%rsi),%xmm4
 	sub    %r13,%rax
 	movsd  0x0(%r13),%xmm0
@@ -7714,99 +7708,99 @@
 	sar    $0x4,%rdx
 	add    %rdx,%rax
 	sar    %rax
 	shl    $0x4,%rax
 	add    %r13,%rax
 	movsd  0x8(%rax),%xmm1
 	comisd %xmm3,%xmm1
-	jbe    bc66 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x116>
+	jbe    bc26 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x116>
 	comisd %xmm1,%xmm4
-	ja     bcc8 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x178>
+	ja     bc88 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x178>
 	comisd %xmm3,%xmm4
-	ja     bc76 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x126>
+	ja     bc36 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x126>
 	movdqu 0x10(%r13),%xmm7
 	unpcklpd %xmm2,%xmm0
 	movups %xmm0,0x10(%r13)
 	movups %xmm7,0x0(%r13)
 	movsd  -0x8(%rsi),%xmm2
 	movsd  0x8(%r13),%xmm0
 	mov    %r12,%rbx
 	mov    %rsi,%rdx
 	nopl   0x0(%rax)
 	movsd  0x8(%rbx),%xmm1
 	mov    %rbx,%rbp
 	comisd %xmm1,%xmm0
-	ja     bc60 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x110>
+	ja     bc20 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x110>
 	comisd %xmm0,%xmm2
 	lea    -0x10(%rdx),%rcx
 	lea    -0x20(%rdx),%rax
-	jbe    bcc0 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x170>
+	jbe    bc80 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x170>
 	nopl   0x0(%rax,%rax,1)
 	mov    %rax,%rdx
 	sub    $0x10,%rax
 	comisd 0x18(%rax),%xmm0
-	jb     bc30 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe0>
+	jb     bbf0 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe0>
 	cmp    %rbx,%rdx
-	jbe    bc90 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x140>
+	jbe    bc50 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x140>
 	movsd  (%rbx),%xmm0
 	movdqu (%rdx),%xmm5
 	unpcklpd %xmm1,%xmm0
 	movups %xmm5,(%rbx)
 	movsd  -0x8(%rdx),%xmm2
 	movups %xmm0,(%rdx)
 	movsd  0x8(%r13),%xmm0
 	add    $0x10,%rbx
-	jmp    bc08 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb8>
+	jmp    bbc8 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb8>
 	comisd %xmm3,%xmm4
-	ja     bbdc <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x8c>
+	ja     bb9c <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x8c>
 	comisd %xmm1,%xmm4
-	jbe    bcc8 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x178>
+	jbe    bc88 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x178>
 	movdqu -0x10(%rsi),%xmm7
 	unpcklpd %xmm2,%xmm0
 	movups %xmm7,0x0(%r13)
 	movups %xmm0,-0x10(%rsi)
-	jmp    bbf5 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xa5>
+	jmp    bbb5 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xa5>
 	nopl   (%rax)
 	mov    %r14,%rdx
 	mov    %rbx,%rdi
-	call   bb50 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   bb10 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	mov    %rbx,%rax
 	sub    %r13,%rax
 	cmp    $0x100,%rax
-	jle    bd65 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x215>
+	jle    bd25 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x215>
 	test   %r14,%r14
-	je     bce2 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x192>
+	je     bca2 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x192>
 	mov    %rbx,%rsi
-	jmp    bb80 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x30>
+	jmp    bb40 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x30>
 	nopw   0x0(%rax,%rax,1)
 	mov    %rcx,%rdx
-	jmp    bc3e <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xee>
+	jmp    bbfe <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xee>
 	movdqu (%rax),%xmm7
 	unpcklpd %xmm2,%xmm0
 	movups %xmm7,0x0(%r13)
 	movups %xmm0,(%rax)
 	movsd  -0x8(%rsi),%xmm2
-	jmp    bbf5 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xa5>
+	jmp    bbb5 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xa5>
 	sar    $0x4,%rax
 	lea    -0x2(%rax),%rsi
 	mov    %rax,%rbx
 	sar    %rsi
-	jmp    bcf6 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1a6>
+	jmp    bcb6 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1a6>
 	sub    $0x1,%rsi
 	mov    %rsi,%rax
 	mov    %r13,%rdi
 	shl    $0x4,%rax
 	mov    0x0(%r13,%rax,1),%rdx
 	mov    0x8(%r13,%rax,1),%rax
 	movq   %rdx,%xmm0
 	movq   %rax,%xmm1
 	mov    %rbx,%rdx
-	call   b7f0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   b7b0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	test   %rsi,%rsi
-	jne    bcf2 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1a2>
+	jne    bcb2 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1a2>
 	sub    $0x10,%rbp
 	nopl   (%rax)
 	mov    0x0(%rbp),%rdx
 	mov    %rbp,%rbx
 	mov    0x8(%rbp),%rax
 	xor    %esi,%esi
 	movdqu 0x0(%r13),%xmm6
@@ -7814,27 +7808,27 @@
 	mov    %r13,%rdi
 	sub    $0x10,%rbp
 	movq   %rdx,%xmm0
 	mov    %rbx,%rdx
 	movq   %rax,%xmm1
 	movups %xmm6,0x10(%rbp)
 	sar    $0x4,%rdx
-	call   b7f0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   b7b0 <void std::__adjust_heap<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, long, particle<double>, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	cmp    $0x10,%rbx
-	jg     bd28 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1d8>
+	jg     bce8 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1d8>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	ret
 	nop
 
-000000000000bd70 <music_track_multiturn>:
+000000000000bd30 <music_track_multiturn>:
 music_track_multiturn():
 	push   %r15
 	push   %r14
 	push   %r13
 	movslq %r8d,%r13
 	push   %r12
 	mov    %rdi,%r12
@@ -7857,131 +7851,131 @@
 	movsd  %xmm4,0x28(%rsp)
 	movsd  %xmm5,0x30(%rsp)
 	movsd  %xmm6,0x38(%rsp)
 	movaps %xmm0,0x80(%rsp)
 	call   30a0 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)@plt>
 	mov    0x88(%rsp),%r8
 	test   %r13d,%r13d
-	jle    be68 <music_track_multiturn+0xf8>
+	jle    be28 <music_track_multiturn+0xf8>
 	xor    %ebx,%ebx
 	lea    0x70(%rsp),%r15
-	jmp    be28 <music_track_multiturn+0xb8>
+	jmp    bde8 <music_track_multiturn+0xb8>
 	nopl   0x0(%rax)
 	movdqa 0x70(%rsp),%xmm7
 	add    $0x10,%r8
 	add    $0x1,%rbx
 	movups %xmm7,-0x10(%r8)
 	mov    %r8,0x88(%rsp)
 	cmp    %r13,%rbx
-	je     be68 <music_track_multiturn+0xf8>
+	je     be28 <music_track_multiturn+0xf8>
 	movsd  0x0(%rbp,%rbx,8),%xmm0
 	movhpd (%r12,%rbx,8),%xmm0
 	movaps %xmm0,0x70(%rsp)
 	cmp    %r8,0x90(%rsp)
-	jne    be08 <music_track_multiturn+0x98>
+	jne    bdc8 <music_track_multiturn+0x98>
 	mov    %r15,%rdx
 	mov    %r8,%rsi
 	mov    %r14,%rdi
 	call   31d0 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)@plt>
 	add    $0x1,%rbx
 	mov    0x88(%rsp),%r8
 	cmp    %r13,%rbx
-	jne    be28 <music_track_multiturn+0xb8>
+	jne    bde8 <music_track_multiturn+0xb8>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x80(%rsp),%r15
 	cmp    %r8,%r15
-	je     bf73 <music_track_multiturn+0x203>
+	je     bf33 <music_track_multiturn+0x203>
 	mov    %r8,%rbx
 	mov    $0x3f,%edx
 	mov    %r8,%rsi
 	mov    %r15,%rdi
 	sub    %r15,%rbx
 	mov    %r8,0x58(%rsp)
 	lea    0x10(%r15),%r14
 	mov    %rbx,%rax
 	sar    $0x4,%rax
 	bsr    %rax,%rax
 	xor    $0x3f,%rax
 	sub    %eax,%edx
 	movslq %edx,%rdx
 	add    %rdx,%rdx
-	call   bb50 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   bb10 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	cmp    $0x100,%rbx
 	mov    0x58(%rsp),%r8
-	jg     c640 <music_track_multiturn+0x8d0>
+	jg     c600 <music_track_multiturn+0x8d0>
 	mov    $0x10,%ebx
 	cmp    %r14,%r8
-	je     bf6b <music_track_multiturn+0x1fb>
+	je     bf2b <music_track_multiturn+0x1fb>
 	mov    %rbp,0x68(%rsp)
 	mov    %r8,%rbp
-	jmp    bf1d <music_track_multiturn+0x1ad>
+	jmp    bedd <music_track_multiturn+0x1ad>
 	nopl   0x0(%rax)
 	cmp    %r14,%r15
-	je     bf0c <music_track_multiturn+0x19c>
+	je     becc <music_track_multiturn+0x19c>
 	sub    %r15,%rdx
 	lea    (%r15,%rbx,1),%rdi
 	mov    %r15,%rsi
 	movsd  %xmm1,0x60(%rsp)
 	movsd  %xmm0,0x58(%rsp)
 	call   31f0 <memmove@plt>
 	movsd  0x60(%rsp),%xmm1
 	movsd  0x58(%rsp),%xmm0
 	unpcklpd %xmm0,%xmm1
 	add    $0x10,%r14
 	movups %xmm1,(%r15)
 	cmp    %rbp,%r14
-	je     bf66 <music_track_multiturn+0x1f6>
+	je     bf26 <music_track_multiturn+0x1f6>
 	movsd  0x8(%r14),%xmm0
 	comisd 0x8(%r15),%xmm0
 	mov    %r14,%rdx
 	movsd  (%r14),%xmm1
-	jb     bee0 <music_track_multiturn+0x170>
+	jb     bea0 <music_track_multiturn+0x170>
 	comisd -0x8(%r14),%xmm0
 	lea    -0x10(%r14),%rax
-	jae    bf56 <music_track_multiturn+0x1e6>
+	jae    bf16 <music_track_multiturn+0x1e6>
 	nop
 	movdqu (%rax),%xmm4
 	mov    %rax,%rdx
 	sub    $0x10,%rax
 	movups %xmm4,0x20(%rax)
 	comisd 0x8(%rax),%xmm0
-	jb     bf40 <music_track_multiturn+0x1d0>
+	jb     bf00 <music_track_multiturn+0x1d0>
 	unpcklpd %xmm0,%xmm1
 	add    $0x10,%r14
 	movups %xmm1,(%rdx)
 	cmp    %rbp,%r14
-	jne    bf1d <music_track_multiturn+0x1ad>
+	jne    bedd <music_track_multiturn+0x1ad>
 	mov    0x68(%rsp),%rbp
 	mov    0x80(%rsp),%r8
 	mov    0x44(%rsp),%eax
 	test   %eax,%eax
-	jle    bff3 <music_track_multiturn+0x283>
+	jle    bfb3 <music_track_multiturn+0x283>
 	mov    0x44(%rsp),%eax
 	cmp    $0x1,%eax
-	je     c743 <music_track_multiturn+0x9d3>
+	je     c703 <music_track_multiturn+0x9d3>
 	mov    %eax,%edx
 	xor    %eax,%eax
 	shr    %edx
 	shl    $0x4,%rdx
 	nopw   0x0(%rax,%rax,1)
 	movupd (%r8,%rax,2),%xmm0
 	movupd 0x10(%r8,%rax,2),%xmm1
 	movapd %xmm0,%xmm2
 	unpckhpd %xmm1,%xmm0
 	unpcklpd %xmm1,%xmm2
 	movups %xmm0,(%r12,%rax,1)
 	movups %xmm2,0x0(%rbp,%rax,1)
 	add    $0x10,%rax
 	cmp    %rdx,%rax
-	jne    bf98 <music_track_multiturn+0x228>
+	jne    bf58 <music_track_multiturn+0x228>
 	mov    0x44(%rsp),%edi
 	mov    %edi,%eax
 	and    $0xfffffffe,%eax
 	and    $0x1,%edi
-	je     bff3 <music_track_multiturn+0x283>
+	je     bfb3 <music_track_multiturn+0x283>
 	cltq
 	mov    %rax,%rdx
 	shl    $0x4,%rdx
 	add    %r8,%rdx
 	movsd  (%rdx),%xmm0
 	movsd  %xmm0,0x0(%rbp,%rax,8)
 	movsd  0x8(%rdx),%xmm0
@@ -7991,133 +7985,133 @@
 	movsd  0x10(%rax),%xmm1
 	movsd  0x18(%rax),%xmm0
 	addsd  %xmm7,%xmm1
 	movapd %xmm1,%xmm3
 	subsd  %xmm0,%xmm3
 	subsd  %xmm1,%xmm0
 	mulsd  0x8(%rsp),%xmm0
-	comisd 0xc352(%rip),%xmm0        
-	ja     c620 <music_track_multiturn+0x8b0>
-	movsd  0xc34c(%rip),%xmm1        
+	comisd 0xc392(%rip),%xmm0        
+	ja     c5e0 <music_track_multiturn+0x8b0>
+	movsd  0xc38c(%rip),%xmm1        
 	pxor   %xmm4,%xmm4
 	pxor   %xmm2,%xmm2
-	movsd  0xc28b(%rip),%xmm9        
-	movsd  0xc28a(%rip),%xmm8        
+	movsd  0xc2cb(%rip),%xmm9        
+	movsd  0xc2ca(%rip),%xmm8        
 	mulsd  %xmm0,%xmm1
 	addsd  %xmm9,%xmm1
 	cvttsd2si %xmm1,%eax
 	cvtsd2ss %xmm1,%xmm4
 	movd   %xmm4,%edx
 	movapd %xmm0,%xmm1
 	shr    $0x1f,%edx
-	movsd  0xc31e(%rip),%xmm4        
+	movsd  0xc35e(%rip),%xmm4        
 	sub    %edx,%eax
 	cvtsi2sd %eax,%xmm2
-	mulsd  0xc308(%rip),%xmm2        
+	mulsd  0xc348(%rip),%xmm2        
 	cltq
 	add    $0x3ff,%rax
 	shl    $0x34,%rax
 	subsd  %xmm2,%xmm1
 	movapd %xmm1,%xmm2
 	mulsd  %xmm1,%xmm2
 	mulsd  %xmm2,%xmm4
-	addsd  0xc2f4(%rip),%xmm4        
+	addsd  0xc334(%rip),%xmm4        
 	mulsd  %xmm2,%xmm4
 	addsd  %xmm8,%xmm4
 	mulsd  %xmm4,%xmm1
-	movsd  0xc2e7(%rip),%xmm4        
+	movsd  0xc327(%rip),%xmm4        
 	mulsd  %xmm2,%xmm4
-	addsd  0xc2e3(%rip),%xmm4        
+	addsd  0xc323(%rip),%xmm4        
 	mulsd  %xmm2,%xmm4
-	addsd  0xc2df(%rip),%xmm4        
+	addsd  0xc31f(%rip),%xmm4        
 	mulsd  %xmm4,%xmm2
 	movapd %xmm1,%xmm4
-	addsd  0xc2d7(%rip),%xmm2        
+	addsd  0xc317(%rip),%xmm2        
 	subsd  %xmm1,%xmm2
 	divsd  %xmm2,%xmm4
 	movq   %rax,%xmm2
 	addsd  %xmm4,%xmm4
 	addsd  %xmm8,%xmm4
 	mulsd  %xmm4,%xmm2
-	movsd  0xc2bc(%rip),%xmm14        
+	movsd  0xc2fc(%rip),%xmm14        
 	pxor   %xmm12,%xmm12
 	comisd %xmm0,%xmm14
-	jbe    c119 <music_track_multiturn+0x3a9>
+	jbe    c0d9 <music_track_multiturn+0x3a9>
 	pxor   %xmm2,%xmm2
 	movapd %xmm2,%xmm12
 	mulsd  0x10(%rsp),%xmm3
-	movsd  0xc139(%rip),%xmm0        
-	movq   0xc030(%rip),%xmm10        
+	movsd  0xc179(%rip),%xmm0        
+	movq   0xc070(%rip),%xmm10        
 	movapd %xmm3,%xmm1
 	andpd  %xmm10,%xmm1
 	mulsd  %xmm1,%xmm0
 	movapd %xmm1,%xmm6
 	cvttsd2si %xmm0,%eax
 	pxor   %xmm0,%xmm0
 	add    $0x1,%eax
 	mov    %eax,%edx
 	and    $0x4,%eax
 	and    $0xfffffffe,%edx
 	cvtsi2sd %edx,%xmm0
-	mulsd  0xc108(%rip),%xmm0        
+	mulsd  0xc148(%rip),%xmm0        
 	sub    $0x2,%edx
 	mov    %edx,%ecx
 	and    $0x4,%ecx
 	and    $0x2,%edx
 	subsd  %xmm0,%xmm6
-	movsd  0xc0f9(%rip),%xmm0        
+	movsd  0xc139(%rip),%xmm0        
 	movapd %xmm6,%xmm5
 	movapd %xmm6,%xmm11
 	mulsd  %xmm6,%xmm5
 	mulsd  %xmm5,%xmm0
 	movapd %xmm5,%xmm4
-	subsd  0xc0e4(%rip),%xmm0        
+	subsd  0xc124(%rip),%xmm0        
 	mulsd  %xmm5,%xmm11
 	mulsd  %xmm5,%xmm4
 	mulsd  %xmm5,%xmm0
-	addsd  0xc0d7(%rip),%xmm0        
+	addsd  0xc117(%rip),%xmm0        
 	movapd %xmm11,%xmm1
-	movsd  0xc111(%rip),%xmm11        
+	movsd  0xc151(%rip),%xmm11        
 	mulsd  %xmm5,%xmm0
-	subsd  0xc0c5(%rip),%xmm0        
+	subsd  0xc105(%rip),%xmm0        
 	mulsd  %xmm5,%xmm0
-	addsd  0xc0c1(%rip),%xmm0        
+	addsd  0xc101(%rip),%xmm0        
 	mulsd  %xmm5,%xmm0
-	subsd  0xc0bd(%rip),%xmm0        
+	subsd  0xc0fd(%rip),%xmm0        
 	mulsd  %xmm0,%xmm1
-	movsd  0xc0b9(%rip),%xmm0        
+	movsd  0xc0f9(%rip),%xmm0        
 	mulsd  %xmm5,%xmm0
-	addsd  0xc0b5(%rip),%xmm0        
+	addsd  0xc0f5(%rip),%xmm0        
 	addsd  %xmm6,%xmm1
 	mulsd  %xmm5,%xmm0
-	subsd  0xc0ad(%rip),%xmm0        
+	subsd  0xc0ed(%rip),%xmm0        
 	mulsd  %xmm5,%xmm0
-	addsd  0xc0a9(%rip),%xmm0        
+	addsd  0xc0e9(%rip),%xmm0        
 	mulsd  %xmm5,%xmm0
-	subsd  0xc0a5(%rip),%xmm0        
+	subsd  0xc0e5(%rip),%xmm0        
 	mulsd  %xmm5,%xmm0
 	mulsd  %xmm9,%xmm5
 	addsd  %xmm11,%xmm0
 	mulsd  %xmm4,%xmm0
 	movapd %xmm8,%xmm4
 	subsd  %xmm5,%xmm4
 	addsd  %xmm4,%xmm0
-	jne    c24a <music_track_multiturn+0x4da>
+	jne    c20a <music_track_multiturn+0x4da>
 	movq   %xmm1,%rdx
 	movapd %xmm0,%xmm1
 	movq   %rdx,%xmm0
 	test   %ecx,%ecx
-	jne    c256 <music_track_multiturn+0x4e6>
-	xorpd  0xbf1a(%rip),%xmm0        
+	jne    c216 <music_track_multiturn+0x4e6>
+	xorpd  0xbf5a(%rip),%xmm0        
 	test   %eax,%eax
-	je     c262 <music_track_multiturn+0x4f2>
-	xorpd  0xbf0e(%rip),%xmm1        
+	je     c222 <music_track_multiturn+0x4f2>
+	xorpd  0xbf4e(%rip),%xmm1        
 	comisd %xmm3,%xmm12
-	jbe    c271 <music_track_multiturn+0x501>
-	xorpd  0xbeff(%rip),%xmm1        
+	jbe    c231 <music_track_multiturn+0x501>
+	xorpd  0xbf3f(%rip),%xmm1        
 	movsd  0x20(%rsp),%xmm3
 	mov    0x48(%rsp),%rax
 	movsd  0x28(%rsp),%xmm5
 	mov    0x50(%rsp),%rdi
 	mulsd  %xmm1,%xmm3
 	movsd  0x8(%rax),%xmm13
 	movsd  (%rax),%xmm6
@@ -8141,137 +8135,137 @@
 	movsd  %xmm0,(%rdi)
 	addsd  0x0(%rbp),%xmm0
 	addsd  %xmm6,%xmm3
 	movsd  %xmm0,0x0(%rbp)
 	movapd %xmm3,%xmm4
 	mulsd  %xmm2,%xmm4
 	cmp    $0x1,%eax
-	jle    c5e9 <music_track_multiturn+0x879>
+	jle    c5a9 <music_track_multiturn+0x879>
 	lea    -0x2(%rax),%r9d
 	movapd %xmm12,%xmm15
 	mov    $0x1,%eax
-	movsd  0xc053(%rip),%xmm13        
+	movsd  0xc093(%rip),%xmm13        
 	add    $0x2,%r9
 	nopl   0x0(%rax)
 	movapd %xmm7,%xmm0
 	movsd  (%r12,%rax,8),%xmm7
 	movapd %xmm13,%xmm3
 	movapd %xmm7,%xmm6
 	subsd  %xmm0,%xmm6
 	subsd  %xmm7,%xmm0
 	mulsd  0x8(%rsp),%xmm0
-	comisd 0xc027(%rip),%xmm0        
-	ja     c412 <music_track_multiturn+0x6a2>
-	movsd  0xc021(%rip),%xmm1        
+	comisd 0xc067(%rip),%xmm0        
+	ja     c3d2 <music_track_multiturn+0x6a2>
+	movsd  0xc061(%rip),%xmm1        
 	pxor   %xmm3,%xmm3
 	movapd %xmm0,%xmm2
 	mulsd  %xmm0,%xmm1
 	addsd  %xmm9,%xmm1
 	cvttsd2si %xmm1,%edx
 	cvtsd2ss %xmm1,%xmm3
 	movd   %xmm3,%ecx
 	pxor   %xmm1,%xmm1
 	shr    $0x1f,%ecx
-	movsd  0xc005(%rip),%xmm3        
+	movsd  0xc045(%rip),%xmm3        
 	sub    %ecx,%edx
 	cvtsi2sd %edx,%xmm1
-	mulsd  0xbfef(%rip),%xmm1        
+	mulsd  0xc02f(%rip),%xmm1        
 	movslq %edx,%rdx
 	add    $0x3ff,%rdx
 	shl    $0x34,%rdx
 	subsd  %xmm1,%xmm2
 	movapd %xmm2,%xmm1
 	mulsd  %xmm2,%xmm1
 	mulsd  %xmm1,%xmm3
-	addsd  0xbfd9(%rip),%xmm3        
+	addsd  0xc019(%rip),%xmm3        
 	mulsd  %xmm1,%xmm3
 	addsd  %xmm8,%xmm3
 	mulsd  %xmm2,%xmm3
-	movsd  0xbfcc(%rip),%xmm2        
+	movsd  0xc00c(%rip),%xmm2        
 	mulsd  %xmm1,%xmm2
-	addsd  0xbfc8(%rip),%xmm2        
+	addsd  0xc008(%rip),%xmm2        
 	mulsd  %xmm1,%xmm2
-	addsd  0xbfc4(%rip),%xmm2        
+	addsd  0xc004(%rip),%xmm2        
 	mulsd  %xmm1,%xmm2
-	addsd  0xbfc0(%rip),%xmm2        
+	addsd  0xc000(%rip),%xmm2        
 	subsd  %xmm3,%xmm2
 	divsd  %xmm2,%xmm3
 	movq   %rdx,%xmm2
 	addsd  %xmm3,%xmm3
 	addsd  %xmm8,%xmm3
 	mulsd  %xmm2,%xmm3
 	mulsd  0x10(%rsp),%xmm6
 	cmpnltsd %xmm14,%xmm0
-	movsd  0xbe3a(%rip),%xmm1        
+	movsd  0xbe7a(%rip),%xmm1        
 	andpd  %xmm0,%xmm3
 	movapd %xmm6,%xmm0
 	andpd  %xmm10,%xmm0
 	mulsd  %xmm0,%xmm1
 	cvttsd2si %xmm1,%edx
 	pxor   %xmm1,%xmm1
 	add    $0x1,%edx
 	mov    %edx,%ecx
 	and    $0x4,%edx
 	and    $0xfffffffe,%ecx
 	cvtsi2sd %ecx,%xmm1
-	mulsd  0xbe12(%rip),%xmm1        
+	mulsd  0xbe52(%rip),%xmm1        
 	sub    $0x2,%ecx
 	mov    %ecx,%esi
 	and    $0x4,%esi
 	and    $0x2,%ecx
 	subsd  %xmm1,%xmm0
-	movsd  0xbe03(%rip),%xmm1        
+	movsd  0xbe43(%rip),%xmm1        
 	movapd %xmm0,%xmm2
 	movapd %xmm0,%xmm12
 	mulsd  %xmm0,%xmm2
 	mulsd  %xmm2,%xmm1
 	movapd %xmm2,%xmm0
-	subsd  0xbdee(%rip),%xmm1        
+	subsd  0xbe2e(%rip),%xmm1        
 	mulsd  %xmm12,%xmm0
 	mulsd  %xmm2,%xmm1
-	addsd  0xbde5(%rip),%xmm1        
+	addsd  0xbe25(%rip),%xmm1        
 	mulsd  %xmm2,%xmm1
-	subsd  0xbde1(%rip),%xmm1        
+	subsd  0xbe21(%rip),%xmm1        
 	mulsd  %xmm2,%xmm1
-	addsd  0xbddd(%rip),%xmm1        
+	addsd  0xbe1d(%rip),%xmm1        
 	mulsd  %xmm2,%xmm1
-	subsd  0xbdd9(%rip),%xmm1        
+	subsd  0xbe19(%rip),%xmm1        
 	mulsd  %xmm1,%xmm0
-	movsd  0xbdd5(%rip),%xmm1        
+	movsd  0xbe15(%rip),%xmm1        
 	mulsd  %xmm2,%xmm1
-	addsd  0xbdd1(%rip),%xmm1        
+	addsd  0xbe11(%rip),%xmm1        
 	addsd  %xmm12,%xmm0
 	movapd %xmm2,%xmm12
 	mulsd  %xmm2,%xmm1
-	subsd  0xbdc3(%rip),%xmm1        
+	subsd  0xbe03(%rip),%xmm1        
 	mulsd  %xmm2,%xmm12
 	mulsd  %xmm2,%xmm1
-	addsd  0xbdba(%rip),%xmm1        
+	addsd  0xbdfa(%rip),%xmm1        
 	mulsd  %xmm2,%xmm1
-	subsd  0xbdb6(%rip),%xmm1        
+	subsd  0xbdf6(%rip),%xmm1        
 	mulsd  %xmm2,%xmm1
 	mulsd  %xmm9,%xmm2
 	addsd  %xmm11,%xmm1
 	mulsd  %xmm12,%xmm1
 	movapd %xmm8,%xmm12
 	subsd  %xmm2,%xmm12
 	addsd  %xmm12,%xmm1
-	jne    c53c <music_track_multiturn+0x7cc>
+	jne    c4fc <music_track_multiturn+0x7cc>
 	movq   %xmm0,%rcx
 	movapd %xmm1,%xmm0
 	movq   %rcx,%xmm1
 	test   %esi,%esi
-	jne    c548 <music_track_multiturn+0x7d8>
-	xorpd  0xbc28(%rip),%xmm1        
+	jne    c508 <music_track_multiturn+0x7d8>
+	xorpd  0xbc68(%rip),%xmm1        
 	test   %edx,%edx
-	je     c554 <music_track_multiturn+0x7e4>
-	xorpd  0xbc1c(%rip),%xmm0        
+	je     c514 <music_track_multiturn+0x7e4>
+	xorpd  0xbc5c(%rip),%xmm0        
 	comisd %xmm6,%xmm15
-	jbe    c563 <music_track_multiturn+0x7f3>
-	xorpd  0xbc0d(%rip),%xmm0        
+	jbe    c523 <music_track_multiturn+0x7f3>
+	xorpd  0xbc4d(%rip),%xmm0        
 	movsd  0x20(%rsp),%xmm6
 	movsd  0x28(%rsp),%xmm2
 	mulsd  %xmm0,%xmm6
 	mulsd  %xmm4,%xmm2
 	addsd  %xmm1,%xmm6
 	mulsd  %xmm0,%xmm2
 	mulsd  %xmm5,%xmm6
@@ -8292,110 +8286,110 @@
 	movapd %xmm2,%xmm5
 	addsd  %xmm8,%xmm5
 	movsd  %xmm0,0x0(%rbp,%rax,8)
 	add    $0x1,%rax
 	movapd %xmm1,%xmm4
 	mulsd  %xmm3,%xmm4
 	cmp    %r9,%rax
-	jne    c328 <music_track_multiturn+0x5b8>
+	jne    c2e8 <music_track_multiturn+0x5b8>
 	mov    0x48(%rsp),%rax
 	movsd  -0x8(%r12,%r13,8),%xmm0
 	unpcklpd %xmm4,%xmm5
 	movups %xmm5,(%rax)
 	movsd  %xmm0,0x18(%rax)
 	test   %r8,%r8
-	je     c60e <music_track_multiturn+0x89e>
+	je     c5ce <music_track_multiturn+0x89e>
 	mov    %r8,%rdi
 	call   3130 <operator delete(void*)@plt>
 	add    $0xa8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
-	movsd  0xbd48(%rip),%xmm2        
-	movsd  0xbc9f(%rip),%xmm9        
-	movsd  0xbc9e(%rip),%xmm8        
-	jmp    c0fb <music_track_multiturn+0x38b>
+	movsd  0xbd88(%rip),%xmm2        
+	movsd  0xbcdf(%rip),%xmm9        
+	movsd  0xbcde(%rip),%xmm8        
+	jmp    c0bb <music_track_multiturn+0x38b>
 	nop
 	mov    %r8,0x68(%rsp)
 	lea    0x100(%r15),%rbx
-	jmp    c692 <music_track_multiturn+0x922>
+	jmp    c652 <music_track_multiturn+0x922>
 	xchg   %ax,%ax
 	cmp    %r14,%r15
-	je     c681 <music_track_multiturn+0x911>
+	je     c641 <music_track_multiturn+0x911>
 	mov    $0x10,%eax
 	sub    %r15,%rdx
 	mov    %r15,%rsi
 	movsd  %xmm1,0x60(%rsp)
 	lea    (%r15,%rax,1),%rdi
 	movsd  %xmm0,0x58(%rsp)
 	call   31f0 <memmove@plt>
 	movsd  0x60(%rsp),%xmm1
 	movsd  0x58(%rsp),%xmm0
 	unpcklpd %xmm0,%xmm1
 	add    $0x10,%r14
 	movups %xmm1,(%r15)
 	cmp    %rbx,%r14
-	je     c6de <music_track_multiturn+0x96e>
+	je     c69e <music_track_multiturn+0x96e>
 	movsd  0x8(%r14),%xmm0
 	comisd 0x8(%r15),%xmm0
 	mov    %r14,%rdx
 	movsd  (%r14),%xmm1
-	jb     c650 <music_track_multiturn+0x8e0>
+	jb     c610 <music_track_multiturn+0x8e0>
 	comisd -0x8(%r14),%xmm0
 	lea    -0x10(%r14),%rax
-	jae    c6ce <music_track_multiturn+0x95e>
+	jae    c68e <music_track_multiturn+0x95e>
 	nopl   0x0(%rax)
 	movdqu (%rax),%xmm7
 	mov    %rax,%rdx
 	sub    $0x10,%rax
 	movups %xmm7,0x20(%rax)
 	comisd 0x8(%rax),%xmm0
-	jb     c6b8 <music_track_multiturn+0x948>
+	jb     c678 <music_track_multiturn+0x948>
 	unpcklpd %xmm0,%xmm1
 	add    $0x10,%r14
 	movups %xmm1,(%rdx)
 	cmp    %rbx,%r14
-	jne    c692 <music_track_multiturn+0x922>
+	jne    c652 <music_track_multiturn+0x922>
 	mov    0x68(%rsp),%r8
 	mov    %r14,%rdx
 	cmp    %r8,%r14
-	je     bf6b <music_track_multiturn+0x1fb>
+	je     bf2b <music_track_multiturn+0x1fb>
 	nop
 	movsd  0x8(%rdx),%xmm0
 	movsd  (%rdx),%xmm1
 	mov    %rdx,%rcx
 	lea    -0x10(%rdx),%rax
 	comisd -0x8(%rdx),%xmm0
-	jae    c726 <music_track_multiturn+0x9b6>
+	jae    c6e6 <music_track_multiturn+0x9b6>
 	nopw   0x0(%rax,%rax,1)
 	movdqu (%rax),%xmm7
 	mov    %rax,%rcx
 	sub    $0x10,%rax
 	movups %xmm7,0x20(%rax)
 	comisd 0x8(%rax),%xmm0
-	jb     c710 <music_track_multiturn+0x9a0>
+	jb     c6d0 <music_track_multiturn+0x9a0>
 	unpcklpd %xmm0,%xmm1
 	add    $0x10,%rdx
 	movups %xmm1,(%rcx)
 	cmp    %r8,%rdx
-	jne    c6f0 <music_track_multiturn+0x980>
+	jne    c6b0 <music_track_multiturn+0x980>
 	mov    0x80(%rsp),%r8
-	jmp    bf73 <music_track_multiturn+0x203>
+	jmp    bf33 <music_track_multiturn+0x203>
 	xor    %eax,%eax
-	jmp    bfd2 <music_track_multiturn+0x262>
+	jmp    bf92 <music_track_multiturn+0x262>
 	mov    %rax,%rbp
 	jmp    32d0 <music_track_multiturn.cold>
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-000000000000c760 <music_track>:
+000000000000c720 <music_track>:
 music_track():
 	push   %r15
 	movslq %r8d,%rax
 	push   %r14
 	mov    %rax,%r15
 	push   %r13
 	mov    %rdx,%r13
@@ -8420,274 +8414,274 @@
 	movsd  %xmm4,0x38(%rsp)
 	movsd  %xmm5,0x40(%rsp)
 	movsd  %xmm6,0x48(%rsp)
 	movaps %xmm0,0x80(%rsp)
 	call   30a0 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)@plt>
 	mov    0x88(%rsp),%r8
 	test   %r15d,%r15d
-	jle    c860 <music_track+0x100>
+	jle    c820 <music_track+0x100>
 	xor    %ebp,%ebp
 	lea    0x70(%rsp),%r15
-	jmp    c822 <music_track+0xc2>
+	jmp    c7e2 <music_track+0xc2>
 	nopl   0x0(%rax)
 	movdqa 0x70(%rsp),%xmm7
 	add    $0x10,%r8
 	add    $0x1,%rbp
 	movups %xmm7,-0x10(%r8)
 	mov    %r8,0x88(%rsp)
 	cmp    0x8(%rsp),%rbp
-	je     c860 <music_track+0x100>
+	je     c820 <music_track+0x100>
 	movsd  (%rbx,%rbp,8),%xmm0
 	movhpd (%r12,%rbp,8),%xmm0
 	movaps %xmm0,0x70(%rsp)
 	cmp    %r8,0x90(%rsp)
-	jne    c800 <music_track+0xa0>
+	jne    c7c0 <music_track+0xa0>
 	mov    %r15,%rdx
 	mov    %r8,%rsi
 	mov    %r14,%rdi
 	call   31d0 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)@plt>
 	mov    0x88(%rsp),%r8
 	add    $0x1,%rbp
 	cmp    0x8(%rsp),%rbp
-	jne    c822 <music_track+0xc2>
+	jne    c7e2 <music_track+0xc2>
 	nopl   (%rax)
 	mov    0x80(%rsp),%r15
 	cmp    %r8,%r15
-	je     c973 <music_track+0x213>
+	je     c933 <music_track+0x213>
 	mov    %r8,%rbp
 	mov    $0x3f,%edx
 	mov    %r8,%rsi
 	mov    %r15,%rdi
 	sub    %r15,%rbp
 	mov    %r8,0x58(%rsp)
 	lea    0x10(%r15),%r14
 	mov    %rbp,%rax
 	sar    $0x4,%rax
 	bsr    %rax,%rax
 	xor    $0x3f,%rax
 	sub    %eax,%edx
 	movslq %edx,%rdx
 	add    %rdx,%rdx
-	call   bb50 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   bb10 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, __gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	cmp    $0x100,%rbp
 	mov    0x58(%rsp),%r8
-	jg     cd70 <music_track+0x610>
+	jg     cd30 <music_track+0x610>
 	mov    $0x10,%ebp
 	cmp    %r14,%r8
-	je     c96b <music_track+0x20b>
+	je     c92b <music_track+0x20b>
 	mov    %rbx,0x68(%rsp)
 	mov    %r8,%rbx
-	jmp    c915 <music_track+0x1b5>
+	jmp    c8d5 <music_track+0x1b5>
 	nopl   0x0(%rax)
 	cmp    %r14,%r15
-	je     c904 <music_track+0x1a4>
+	je     c8c4 <music_track+0x1a4>
 	sub    %r15,%rdx
 	lea    (%r15,%rbp,1),%rdi
 	mov    %r15,%rsi
 	movsd  %xmm1,0x60(%rsp)
 	movsd  %xmm0,0x58(%rsp)
 	call   31f0 <memmove@plt>
 	movsd  0x60(%rsp),%xmm1
 	movsd  0x58(%rsp),%xmm0
 	unpcklpd %xmm0,%xmm1
 	add    $0x10,%r14
 	movups %xmm1,(%r15)
 	cmp    %rbx,%r14
-	je     c966 <music_track+0x206>
+	je     c926 <music_track+0x206>
 	movsd  0x8(%r14),%xmm0
 	comisd 0x8(%r15),%xmm0
 	mov    %r14,%rdx
 	movsd  (%r14),%xmm1
-	jb     c8d8 <music_track+0x178>
+	jb     c898 <music_track+0x178>
 	comisd -0x8(%r14),%xmm0
 	lea    -0x10(%r14),%rax
-	jae    c956 <music_track+0x1f6>
+	jae    c916 <music_track+0x1f6>
 	nopw   0x0(%rax,%rax,1)
 	movdqu (%rax),%xmm7
 	mov    %rax,%rdx
 	sub    $0x10,%rax
 	movups %xmm7,0x20(%rax)
 	comisd 0x8(%rax),%xmm0
-	jb     c940 <music_track+0x1e0>
+	jb     c900 <music_track+0x1e0>
 	unpcklpd %xmm0,%xmm1
 	add    $0x10,%r14
 	movups %xmm1,(%rdx)
 	cmp    %rbx,%r14
-	jne    c915 <music_track+0x1b5>
+	jne    c8d5 <music_track+0x1b5>
 	mov    0x68(%rsp),%rbx
 	mov    0x80(%rsp),%r8
 	mov    0x14(%rsp),%eax
 	test   %eax,%eax
-	jle    ce9b <music_track+0x73b>
+	jle    ce5b <music_track+0x73b>
 	cmp    $0x1,%eax
-	je     ceba <music_track+0x75a>
+	je     ce7a <music_track+0x75a>
 	shr    %eax
 	mov    %eax,%edx
 	xor    %eax,%eax
 	shl    $0x4,%rdx
 	nopw   0x0(%rax,%rax,1)
 	movupd (%r8,%rax,2),%xmm0
 	movupd 0x10(%r8,%rax,2),%xmm1
 	movapd %xmm0,%xmm2
 	unpckhpd %xmm1,%xmm0
 	unpcklpd %xmm1,%xmm2
 	movups %xmm0,(%r12,%rax,1)
 	movups %xmm2,(%rbx,%rax,1)
 	add    $0x10,%rax
 	cmp    %rdx,%rax
-	jne    c998 <music_track+0x238>
+	jne    c958 <music_track+0x238>
 	mov    0x14(%rsp),%edi
 	mov    %edi,%eax
 	and    $0xfffffffe,%eax
 	cmp    %edi,%eax
-	je     ce88 <music_track+0x728>
+	je     ce48 <music_track+0x728>
 	cltq
 	mov    %rax,%rdx
 	shl    $0x4,%rdx
 	add    %r8,%rdx
 	cmpl   $0x1,0x14(%rsp)
 	movsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rbx,%rax,8)
 	movsd  0x8(%rdx),%xmm0
 	movsd  %xmm0,(%r12,%rax,8)
 	movsd  (%rbx),%xmm0
 	addsd  0x0(%r13),%xmm0
 	movsd  %xmm0,(%rbx)
-	jle    cec1 <music_track+0x761>
+	jle    ce81 <music_track+0x761>
 	mov    0x14(%rsp),%eax
 	pxor   %xmm10,%xmm10
-	movsd  0xb8b9(%rip),%xmm8        
+	movsd  0xb8f9(%rip),%xmm8        
 	movsd  (%r12),%xmm7
 	movapd %xmm10,%xmm4
-	movsd  0xb89d(%rip),%xmm9        
+	movsd  0xb8dd(%rip),%xmm9        
 	lea    -0x2(%rax),%edi
 	movapd %xmm8,%xmm5
-	movq   0xb71c(%rip),%xmm14        
-	movsd  0xb843(%rip),%xmm13        
-	movsd  0xb84a(%rip),%xmm12        
+	movq   0xb75c(%rip),%xmm14        
+	movsd  0xb883(%rip),%xmm13        
+	movsd  0xb88a(%rip),%xmm12        
 	add    $0x2,%rdi
 	mov    $0x1,%eax
-	movsd  0xb908(%rip),%xmm11        
+	movsd  0xb948(%rip),%xmm11        
 	nopl   0x0(%rax,%rax,1)
 	movapd %xmm7,%xmm0
 	movsd  (%r12,%rax,8),%xmm7
 	movapd %xmm11,%xmm3
 	movapd %xmm7,%xmm6
 	subsd  %xmm0,%xmm6
 	subsd  %xmm7,%xmm0
 	mulsd  0x18(%rsp),%xmm0
-	comisd 0xb8df(%rip),%xmm0        
-	ja     cb5a <music_track+0x3fa>
-	movsd  0xb8d9(%rip),%xmm1        
+	comisd 0xb91f(%rip),%xmm0        
+	ja     cb1a <music_track+0x3fa>
+	movsd  0xb919(%rip),%xmm1        
 	pxor   %xmm3,%xmm3
 	movapd %xmm0,%xmm2
 	mulsd  %xmm0,%xmm1
 	addsd  %xmm9,%xmm1
 	cvttsd2si %xmm1,%edx
 	cvtsd2ss %xmm1,%xmm3
 	movd   %xmm3,%ecx
 	pxor   %xmm1,%xmm1
 	shr    $0x1f,%ecx
-	movsd  0xb8bd(%rip),%xmm3        
+	movsd  0xb8fd(%rip),%xmm3        
 	sub    %ecx,%edx
 	cvtsi2sd %edx,%xmm1
-	mulsd  0xb8a7(%rip),%xmm1        
+	mulsd  0xb8e7(%rip),%xmm1        
 	movslq %edx,%rdx
 	add    $0x3ff,%rdx
 	shl    $0x34,%rdx
 	subsd  %xmm1,%xmm2
 	movapd %xmm2,%xmm1
 	mulsd  %xmm2,%xmm1
 	mulsd  %xmm1,%xmm3
-	addsd  0xb891(%rip),%xmm3        
+	addsd  0xb8d1(%rip),%xmm3        
 	mulsd  %xmm1,%xmm3
 	addsd  %xmm8,%xmm3
 	mulsd  %xmm2,%xmm3
-	movsd  0xb884(%rip),%xmm2        
+	movsd  0xb8c4(%rip),%xmm2        
 	mulsd  %xmm1,%xmm2
-	addsd  0xb880(%rip),%xmm2        
+	addsd  0xb8c0(%rip),%xmm2        
 	mulsd  %xmm1,%xmm2
-	addsd  0xb87c(%rip),%xmm2        
+	addsd  0xb8bc(%rip),%xmm2        
 	mulsd  %xmm1,%xmm2
-	addsd  0xb878(%rip),%xmm2        
+	addsd  0xb8b8(%rip),%xmm2        
 	subsd  %xmm3,%xmm2
 	divsd  %xmm2,%xmm3
 	movq   %rdx,%xmm2
 	addsd  %xmm3,%xmm3
 	addsd  %xmm8,%xmm3
 	mulsd  %xmm2,%xmm3
 	mulsd  0x20(%rsp),%xmm6
-	movsd  0xb6f8(%rip),%xmm1        
-	cmpnltsd 0xb84f(%rip),%xmm0        
+	movsd  0xb738(%rip),%xmm1        
+	cmpnltsd 0xb88f(%rip),%xmm0        
 	andpd  %xmm0,%xmm3
 	movapd %xmm6,%xmm0
 	andpd  %xmm14,%xmm0
 	mulsd  %xmm0,%xmm1
 	cvttsd2si %xmm1,%edx
 	pxor   %xmm1,%xmm1
 	add    $0x1,%edx
 	mov    %edx,%ecx
 	and    $0x4,%edx
 	and    $0xfffffffe,%ecx
 	cvtsi2sd %ecx,%xmm1
-	mulsd  0xb6c7(%rip),%xmm1        
+	mulsd  0xb707(%rip),%xmm1        
 	sub    $0x2,%ecx
 	mov    %ecx,%esi
 	and    $0x4,%esi
 	and    $0x2,%ecx
 	subsd  %xmm1,%xmm0
-	movsd  0xb6b8(%rip),%xmm1        
+	movsd  0xb6f8(%rip),%xmm1        
 	movapd %xmm0,%xmm2
 	movapd %xmm0,%xmm15
 	mulsd  %xmm0,%xmm2
 	mulsd  %xmm2,%xmm1
 	movapd %xmm2,%xmm0
-	subsd  0xb6a3(%rip),%xmm1        
+	subsd  0xb6e3(%rip),%xmm1        
 	mulsd  %xmm15,%xmm0
 	mulsd  %xmm2,%xmm1
-	addsd  0xb69a(%rip),%xmm1        
+	addsd  0xb6da(%rip),%xmm1        
 	mulsd  %xmm2,%xmm1
-	subsd  0xb696(%rip),%xmm1        
+	subsd  0xb6d6(%rip),%xmm1        
 	mulsd  %xmm2,%xmm1
 	addsd  %xmm13,%xmm1
 	mulsd  %xmm2,%xmm1
-	subsd  0xb691(%rip),%xmm1        
+	subsd  0xb6d1(%rip),%xmm1        
 	mulsd  %xmm1,%xmm0
 	movapd %xmm2,%xmm1
 	mulsd  %xmm12,%xmm1
-	addsd  0xb68c(%rip),%xmm1        
+	addsd  0xb6cc(%rip),%xmm1        
 	mulsd  %xmm2,%xmm1
 	addsd  %xmm15,%xmm0
 	movapd %xmm2,%xmm15
-	subsd  0xb67e(%rip),%xmm1        
+	subsd  0xb6be(%rip),%xmm1        
 	mulsd  %xmm2,%xmm15
 	mulsd  %xmm2,%xmm1
-	addsd  0xb675(%rip),%xmm1        
+	addsd  0xb6b5(%rip),%xmm1        
 	mulsd  %xmm2,%xmm1
-	subsd  0xb671(%rip),%xmm1        
+	subsd  0xb6b1(%rip),%xmm1        
 	mulsd  %xmm2,%xmm1
-	addsd  0xb66d(%rip),%xmm1        
+	addsd  0xb6ad(%rip),%xmm1        
 	mulsd  %xmm9,%xmm2
 	mulsd  %xmm15,%xmm1
 	movapd %xmm8,%xmm15
 	subsd  %xmm2,%xmm15
 	addsd  %xmm15,%xmm1
-	jne    cc84 <music_track+0x524>
+	jne    cc44 <music_track+0x524>
 	movq   %xmm0,%rcx
 	movapd %xmm1,%xmm0
 	movq   %rcx,%xmm1
 	test   %esi,%esi
-	jne    cc90 <music_track+0x530>
-	xorpd  0xb4e0(%rip),%xmm1        
+	jne    cc50 <music_track+0x530>
+	xorpd  0xb520(%rip),%xmm1        
 	test   %edx,%edx
-	je     cc9c <music_track+0x53c>
-	xorpd  0xb4d4(%rip),%xmm0        
+	je     cc5c <music_track+0x53c>
+	xorpd  0xb514(%rip),%xmm0        
 	comisd %xmm6,%xmm10
-	jbe    ccab <music_track+0x54b>
-	xorpd  0xb4c5(%rip),%xmm0        
+	jbe    cc6b <music_track+0x54b>
+	xorpd  0xb505(%rip),%xmm0        
 	movsd  0x30(%rsp),%xmm6
 	movsd  0x38(%rsp),%xmm2
 	movsd  0x48(%rsp),%xmm15
 	mulsd  %xmm0,%xmm6
 	mulsd  %xmm4,%xmm2
 	mulsd  %xmm0,%xmm15
 	addsd  %xmm1,%xmm6
@@ -8708,122 +8702,122 @@
 	mulsd  %xmm3,%xmm4
 	addsd  %xmm8,%xmm5
 	movsd  %xmm0,0x0(%r13,%rax,8)
 	addsd  (%rbx,%rax,8),%xmm0
 	movsd  %xmm0,(%rbx,%rax,8)
 	add    $0x1,%rax
 	cmp    %rdi,%rax
-	jne    ca70 <music_track+0x310>
+	jne    ca30 <music_track+0x310>
 	mov    0x8(%rsp),%rdi
 	mov    0x50(%rsp),%rax
 	unpcklpd %xmm4,%xmm5
 	movsd  -0x8(%r12,%rdi,8),%xmm0
 	movups %xmm5,(%rax)
 	movsd  %xmm0,0x18(%rax)
 	test   %r8,%r8
-	je     cd5e <music_track+0x5fe>
+	je     cd1e <music_track+0x5fe>
 	mov    %r8,%rdi
 	call   3130 <operator delete(void*)@plt>
 	add    $0xa8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	lea    0x100(%r15),%rbp
 	mov    %rbx,0x68(%rsp)
 	mov    %rbp,%rbx
 	mov    %r8,%rbp
-	jmp    cdca <music_track+0x66a>
+	jmp    cd8a <music_track+0x66a>
 	nopl   0x0(%rax)
 	cmp    %r14,%r15
-	je     cdb9 <music_track+0x659>
+	je     cd79 <music_track+0x659>
 	mov    $0x10,%eax
 	sub    %r15,%rdx
 	mov    %r15,%rsi
 	movsd  %xmm1,0x60(%rsp)
 	lea    (%r15,%rax,1),%rdi
 	movsd  %xmm0,0x58(%rsp)
 	call   31f0 <memmove@plt>
 	movsd  0x60(%rsp),%xmm1
 	movsd  0x58(%rsp),%xmm0
 	unpcklpd %xmm0,%xmm1
 	add    $0x10,%r14
 	movups %xmm1,(%r15)
 	cmp    %rbx,%r14
-	je     ce16 <music_track+0x6b6>
+	je     cdd6 <music_track+0x6b6>
 	movsd  0x8(%r14),%xmm0
 	comisd 0x8(%r15),%xmm0
 	mov    %r14,%rdx
 	movsd  (%r14),%xmm1
-	jb     cd88 <music_track+0x628>
+	jb     cd48 <music_track+0x628>
 	comisd -0x8(%r14),%xmm0
 	lea    -0x10(%r14),%rax
-	jae    ce06 <music_track+0x6a6>
+	jae    cdc6 <music_track+0x6a6>
 	nopl   0x0(%rax)
 	movdqu (%rax),%xmm7
 	mov    %rax,%rdx
 	sub    $0x10,%rax
 	movups %xmm7,0x20(%rax)
 	comisd 0x8(%rax),%xmm0
-	jb     cdf0 <music_track+0x690>
+	jb     cdb0 <music_track+0x690>
 	unpcklpd %xmm0,%xmm1
 	add    $0x10,%r14
 	movups %xmm1,(%rdx)
 	cmp    %rbx,%r14
-	jne    cdca <music_track+0x66a>
+	jne    cd8a <music_track+0x66a>
 	mov    0x68(%rsp),%rbx
 	mov    %rbp,%r8
 	mov    %r14,%rdx
 	cmp    %rbp,%r14
-	je     c96b <music_track+0x20b>
+	je     c92b <music_track+0x20b>
 	nopw   0x0(%rax,%rax,1)
 	movsd  0x8(%rdx),%xmm0
 	movsd  (%rdx),%xmm1
 	mov    %rdx,%rcx
 	lea    -0x10(%rdx),%rax
 	comisd -0x8(%rdx),%xmm0
-	jae    ce66 <music_track+0x706>
+	jae    ce26 <music_track+0x706>
 	nopw   0x0(%rax,%rax,1)
 	movdqu (%rax),%xmm4
 	mov    %rax,%rcx
 	sub    $0x10,%rax
 	movups %xmm4,0x20(%rax)
 	comisd 0x8(%rax),%xmm0
-	jb     ce50 <music_track+0x6f0>
+	jb     ce10 <music_track+0x6f0>
 	unpcklpd %xmm0,%xmm1
 	add    $0x10,%rdx
 	movups %xmm1,(%rcx)
 	cmp    %r8,%rdx
-	jne    ce30 <music_track+0x6d0>
+	jne    cdf0 <music_track+0x6d0>
 	mov    0x80(%rsp),%r8
-	jmp    c973 <music_track+0x213>
+	jmp    c933 <music_track+0x213>
 	nopl   0x0(%rax,%rax,1)
 	movsd  (%rbx),%xmm0
 	addsd  0x0(%r13),%xmm0
 	movsd  %xmm0,(%rbx)
-	jmp    ca0d <music_track+0x2ad>
+	jmp    c9cd <music_track+0x2ad>
 	movsd  (%rbx),%xmm0
 	addsd  0x0(%r13),%xmm0
 	pxor   %xmm4,%xmm4
-	movsd  0xb427(%rip),%xmm5        
+	movsd  0xb467(%rip),%xmm5        
 	movsd  %xmm0,(%rbx)
-	jmp    cd34 <music_track+0x5d4>
+	jmp    ccf4 <music_track+0x5d4>
 	xor    %eax,%eax
-	jmp    c9d4 <music_track+0x274>
-	movsd  0xb40f(%rip),%xmm5        
+	jmp    c994 <music_track+0x274>
+	movsd  0xb44f(%rip),%xmm5        
 	pxor   %xmm4,%xmm4
-	jmp    cd34 <music_track+0x5d4>
+	jmp    ccf4 <music_track+0x5d4>
 	mov    %rax,%rbp
 	jmp    32ea <music_track.cold>
 	nopw   0x0(%rax,%rax,1)
 
-000000000000cee0 <music_track_multiturnf>:
+000000000000cea0 <music_track_multiturnf>:
 music_track_multiturnf():
 	push   %r15
 	push   %r14
 	push   %r13
 	movslq %r8d,%r13
 	push   %r12
 	mov    %rdi,%r12
@@ -8846,153 +8840,153 @@
 	movss  %xmm4,0x18(%rsp)
 	movss  %xmm5,0x1c(%rsp)
 	movss  %xmm6,0x20(%rsp)
 	movaps %xmm0,0x60(%rsp)
 	call   30b0 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)@plt>
 	mov    0x68(%rsp),%r8
 	test   %r13d,%r13d
-	jle    cfd0 <music_track_multiturnf+0xf0>
+	jle    cf90 <music_track_multiturnf+0xf0>
 	xor    %ebx,%ebx
 	lea    0x58(%rsp),%r15
-	jmp    cf8b <music_track_multiturnf+0xab>
+	jmp    cf4b <music_track_multiturnf+0xab>
 	nopl   0x0(%rax,%rax,1)
 	mov    0x58(%rsp),%rax
 	add    $0x8,%r8
 	add    $0x1,%rbx
 	mov    %rax,-0x8(%r8)
 	mov    %r8,0x68(%rsp)
 	cmp    %r13,%rbx
-	je     cfd0 <music_track_multiturnf+0xf0>
+	je     cf90 <music_track_multiturnf+0xf0>
 	movss  0x0(%rbp,%rbx,4),%xmm0
 	movss  %xmm0,0x58(%rsp)
 	movss  (%r12,%rbx,4),%xmm0
 	movss  %xmm0,0x5c(%rsp)
 	cmp    %r8,0x70(%rsp)
-	jne    cf70 <music_track_multiturnf+0x90>
+	jne    cf30 <music_track_multiturnf+0x90>
 	mov    %r15,%rdx
 	mov    %r8,%rsi
 	mov    %r14,%rdi
 	call   3210 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)@plt>
 	add    $0x1,%rbx
 	mov    0x68(%rsp),%r8
 	cmp    %r13,%rbx
-	jne    cf8b <music_track_multiturnf+0xab>
+	jne    cf4b <music_track_multiturnf+0xab>
 	cs nopw 0x0(%rax,%rax,1)
 	mov    0x60(%rsp),%r15
 	cmp    %r8,%r15
-	je     d0d8 <music_track_multiturnf+0x1f8>
+	je     d098 <music_track_multiturnf+0x1f8>
 	mov    %r8,%rbx
 	mov    $0x3f,%edx
 	mov    %r8,%rsi
 	mov    %r15,%rdi
 	sub    %r15,%rbx
 	mov    %r8,0x38(%rsp)
 	lea    0x8(%r15),%r14
 	mov    %rbx,%rax
 	sar    $0x3,%rax
 	bsr    %rax,%rax
 	xor    $0x3f,%rax
 	sub    %eax,%edx
 	movslq %edx,%rdx
 	add    %rdx,%rdx
-	call   b950 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   b910 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	cmp    $0x80,%rbx
 	mov    0x38(%rsp),%r8
-	jg     d830 <music_track_multiturnf+0x950>
+	jg     d7f0 <music_track_multiturnf+0x950>
 	mov    $0x8,%ebx
 	cmp    %r14,%r8
-	je     d0d3 <music_track_multiturnf+0x1f3>
+	je     d093 <music_track_multiturnf+0x1f3>
 	mov    %rbp,0x48(%rsp)
 	mov    %r8,%rbp
-	jmp    d083 <music_track_multiturnf+0x1a3>
+	jmp    d043 <music_track_multiturnf+0x1a3>
 	xchg   %ax,%ax
 	cmp    %r14,%r15
-	je     d06f <music_track_multiturnf+0x18f>
+	je     d02f <music_track_multiturnf+0x18f>
 	mov    %r14,%rdx
 	lea    (%r15,%rbx,1),%rdi
 	mov    %r15,%rsi
 	movss  %xmm1,0x44(%rsp)
 	sub    %r15,%rdx
 	movss  %xmm0,0x38(%rsp)
 	call   31f0 <memmove@plt>
 	movss  0x44(%rsp),%xmm1
 	movss  0x38(%rsp),%xmm0
 	add    $0x8,%r14
 	movss  %xmm1,(%r15)
 	movss  %xmm0,0x4(%r15)
 	cmp    %rbp,%r14
-	je     d0ce <music_track_multiturnf+0x1ee>
+	je     d08e <music_track_multiturnf+0x1ee>
 	movss  0x4(%r14),%xmm0
 	comiss 0x4(%r15),%xmm0
 	mov    %r14,%rcx
 	movss  (%r14),%xmm1
-	jb     d040 <music_track_multiturnf+0x160>
+	jb     d000 <music_track_multiturnf+0x160>
 	comiss -0x4(%r14),%xmm0
 	lea    -0x8(%r14),%rax
-	jae    d0bc <music_track_multiturnf+0x1dc>
+	jae    d07c <music_track_multiturnf+0x1dc>
 	nopl   0x0(%rax,%rax,1)
 	mov    (%rax),%rdx
 	mov    %rax,%rcx
 	sub    $0x8,%rax
 	mov    %rdx,0x10(%rax)
 	comiss 0x4(%rax),%xmm0
-	jb     d0a8 <music_track_multiturnf+0x1c8>
+	jb     d068 <music_track_multiturnf+0x1c8>
 	add    $0x8,%r14
 	movss  %xmm1,(%rcx)
 	movss  %xmm0,0x4(%rcx)
 	cmp    %rbp,%r14
-	jne    d083 <music_track_multiturnf+0x1a3>
+	jne    d043 <music_track_multiturnf+0x1a3>
 	mov    0x48(%rsp),%rbp
 	mov    0x60(%rsp),%r8
 	mov    0x24(%rsp),%eax
 	test   %eax,%eax
-	jle    d19c <music_track_multiturnf+0x2bc>
+	jle    d15c <music_track_multiturnf+0x2bc>
 	mov    0x24(%rsp),%esi
 	lea    -0x1(%rsi),%eax
 	cmp    $0x2,%eax
-	jbe    d940 <music_track_multiturnf+0xa60>
+	jbe    d900 <music_track_multiturnf+0xa60>
 	shr    $0x2,%esi
 	xor    %eax,%eax
 	mov    %esi,%edx
 	shl    $0x4,%rdx
 	nop
 	movups (%r8,%rax,2),%xmm0
 	movups 0x10(%r8,%rax,2),%xmm1
 	movaps %xmm0,%xmm2
 	shufps $0xdd,%xmm1,%xmm0
 	movups %xmm0,(%r12,%rax,1)
 	shufps $0x88,%xmm1,%xmm2
 	movups %xmm2,0x0(%rbp,%rax,1)
 	add    $0x10,%rax
 	cmp    %rax,%rdx
-	jne    d100 <music_track_multiturnf+0x220>
+	jne    d0c0 <music_track_multiturnf+0x220>
 	mov    0x24(%rsp),%esi
 	mov    %esi,%eax
 	and    $0xfffffffc,%eax
 	and    $0x3,%esi
-	je     d19c <music_track_multiturnf+0x2bc>
+	je     d15c <music_track_multiturnf+0x2bc>
 	movslq %eax,%rdx
 	mov    0x24(%rsp),%esi
 	lea    (%r8,%rdx,8),%rcx
 	movss  (%rcx),%xmm0
 	movss  %xmm0,0x0(%rbp,%rdx,4)
 	movss  0x4(%rcx),%xmm0
 	movss  %xmm0,(%r12,%rdx,4)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%esi
-	jle    d19c <music_track_multiturnf+0x2bc>
+	jle    d15c <music_track_multiturnf+0x2bc>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	lea    (%r8,%rdx,8),%rcx
 	movss  (%rcx),%xmm0
 	movss  %xmm0,0x0(%rbp,%rdx,4)
 	movss  0x4(%rcx),%xmm0
 	movss  %xmm0,(%r12,%rdx,4)
 	cmp    %eax,%esi
-	jle    d19c <music_track_multiturnf+0x2bc>
+	jle    d15c <music_track_multiturnf+0x2bc>
 	cltq
 	lea    (%r8,%rax,8),%rdx
 	movss  (%rdx),%xmm0
 	movss  %xmm0,0x0(%rbp,%rax,4)
 	movss  0x4(%rdx),%xmm0
 	movss  %xmm0,(%r12,%rax,4)
 	mov    0x28(%rsp),%rax
@@ -9000,132 +8994,132 @@
 	movss  0x8(%rax),%xmm0
 	movss  0xc(%rax),%xmm1
 	addss  %xmm6,%xmm0
 	movaps %xmm0,%xmm3
 	subss  %xmm1,%xmm3
 	subss  %xmm0,%xmm1
 	mulss  0xc(%rsp),%xmm1
-	comiss 0xb1fb(%rip),%xmm1        
-	ja     d810 <music_track_multiturnf+0x930>
-	movsd  0xb1a5(%rip),%xmm2        
+	comiss 0xb23b(%rip),%xmm1        
+	ja     d7d0 <music_track_multiturnf+0x930>
+	movsd  0xb1e5(%rip),%xmm2        
 	pxor   %xmm0,%xmm0
 	pxor   %xmm4,%xmm4
-	movsd  0xb0e4(%rip),%xmm8        
-	movsd  0xb0e3(%rip),%xmm9        
+	movsd  0xb124(%rip),%xmm8        
+	movsd  0xb123(%rip),%xmm9        
 	cvtss2sd %xmm1,%xmm0
 	mulsd  %xmm0,%xmm2
 	addsd  %xmm8,%xmm2
 	cvttsd2si %xmm2,%eax
 	cvtsd2ss %xmm2,%xmm4
 	movd   %xmm4,%edx
 	pxor   %xmm2,%xmm2
 	shr    $0x1f,%edx
-	movsd  0xb173(%rip),%xmm4        
+	movsd  0xb1b3(%rip),%xmm4        
 	sub    %edx,%eax
 	cvtsi2sd %eax,%xmm2
-	mulsd  0xb15d(%rip),%xmm2        
+	mulsd  0xb19d(%rip),%xmm2        
 	cltq
 	add    $0x3ff,%rax
 	shl    $0x34,%rax
 	subsd  %xmm2,%xmm0
 	movapd %xmm0,%xmm2
 	mulsd  %xmm0,%xmm2
 	mulsd  %xmm2,%xmm4
-	addsd  0xb149(%rip),%xmm4        
+	addsd  0xb189(%rip),%xmm4        
 	mulsd  %xmm2,%xmm4
 	addsd  %xmm9,%xmm4
 	mulsd  %xmm4,%xmm0
-	movsd  0xb13c(%rip),%xmm4        
+	movsd  0xb17c(%rip),%xmm4        
 	mulsd  %xmm2,%xmm4
-	addsd  0xb138(%rip),%xmm4        
+	addsd  0xb178(%rip),%xmm4        
 	mulsd  %xmm2,%xmm4
-	addsd  0xb134(%rip),%xmm4        
+	addsd  0xb174(%rip),%xmm4        
 	mulsd  %xmm4,%xmm2
 	movq   %rax,%xmm4
-	addsd  0xb12b(%rip),%xmm2        
+	addsd  0xb16b(%rip),%xmm2        
 	subsd  %xmm0,%xmm2
 	divsd  %xmm2,%xmm0
 	addsd  %xmm0,%xmm0
 	addsd  %xmm9,%xmm0
 	mulsd  %xmm4,%xmm0
-	movss  0xb121(%rip),%xmm15        
+	movss  0xb161(%rip),%xmm15        
 	comiss %xmm1,%xmm15
-	ja     d800 <music_track_multiturnf+0x920>
+	ja     d7c0 <music_track_multiturnf+0x920>
 	pxor   %xmm10,%xmm10
 	pxor   %xmm12,%xmm12
 	cvtsd2ss %xmm0,%xmm10
 	mulss  0x10(%rsp),%xmm3
-	movsd  0xaf8e(%rip),%xmm0        
+	movsd  0xafce(%rip),%xmm0        
 	pxor   %xmm2,%xmm2
-	movq   0xae81(%rip),%xmm13        
+	movq   0xaec1(%rip),%xmm13        
 	cvtss2sd %xmm3,%xmm2
 	andpd  %xmm13,%xmm2
 	mulsd  %xmm2,%xmm0
 	cvttsd2si %xmm0,%eax
 	pxor   %xmm0,%xmm0
 	add    $0x1,%eax
 	mov    %eax,%edx
 	and    $0x4,%eax
 	and    $0xfffffffe,%edx
 	cvtsi2sd %edx,%xmm0
-	mulsd  0xaf5d(%rip),%xmm0        
+	mulsd  0xaf9d(%rip),%xmm0        
 	sub    $0x2,%edx
 	mov    %edx,%ecx
 	and    $0x4,%ecx
 	and    $0x2,%edx
 	subsd  %xmm0,%xmm2
-	movsd  0xaf4e(%rip),%xmm0        
+	movsd  0xaf8e(%rip),%xmm0        
 	movapd %xmm2,%xmm4
 	movapd %xmm2,%xmm5
 	mulsd  %xmm2,%xmm4
 	mulsd  %xmm4,%xmm0
-	subsd  0xaf3e(%rip),%xmm0        
+	subsd  0xaf7e(%rip),%xmm0        
 	mulsd  %xmm4,%xmm5
 	mulsd  %xmm4,%xmm0
-	addsd  0xaf36(%rip),%xmm0        
+	addsd  0xaf76(%rip),%xmm0        
 	mulsd  %xmm4,%xmm0
-	subsd  0xaf32(%rip),%xmm0        
+	subsd  0xaf72(%rip),%xmm0        
 	mulsd  %xmm4,%xmm0
-	addsd  0xaf2e(%rip),%xmm0        
+	addsd  0xaf6e(%rip),%xmm0        
 	mulsd  %xmm4,%xmm0
-	subsd  0xaf2a(%rip),%xmm0        
+	subsd  0xaf6a(%rip),%xmm0        
 	mulsd  %xmm0,%xmm5
-	movsd  0xaf26(%rip),%xmm0        
+	movsd  0xaf66(%rip),%xmm0        
 	mulsd  %xmm4,%xmm0
-	addsd  0xaf22(%rip),%xmm0        
+	addsd  0xaf62(%rip),%xmm0        
 	addsd  %xmm5,%xmm2
 	movapd %xmm4,%xmm5
 	mulsd  %xmm4,%xmm0
-	subsd  0xaf16(%rip),%xmm0        
+	subsd  0xaf56(%rip),%xmm0        
 	mulsd  %xmm4,%xmm5
 	mulsd  %xmm4,%xmm0
-	addsd  0xaf0e(%rip),%xmm0        
+	addsd  0xaf4e(%rip),%xmm0        
 	mulsd  %xmm4,%xmm0
-	subsd  0xaf0a(%rip),%xmm0        
+	subsd  0xaf4a(%rip),%xmm0        
 	mulsd  %xmm4,%xmm0
-	addsd  0xaf06(%rip),%xmm0        
+	addsd  0xaf46(%rip),%xmm0        
 	mulsd  %xmm8,%xmm4
 	mulsd  %xmm5,%xmm0
 	movapd %xmm9,%xmm5
 	subsd  %xmm4,%xmm5
 	addsd  %xmm5,%xmm0
-	jne    d3e8 <music_track_multiturnf+0x508>
+	jne    d3a8 <music_track_multiturnf+0x508>
 	movq   %xmm2,%rdx
 	movapd %xmm0,%xmm2
 	movq   %rdx,%xmm0
 	test   %ecx,%ecx
-	jne    d3f4 <music_track_multiturnf+0x514>
-	xorpd  0xad7c(%rip),%xmm0        
+	jne    d3b4 <music_track_multiturnf+0x514>
+	xorpd  0xadbc(%rip),%xmm0        
 	test   %eax,%eax
-	je     d400 <music_track_multiturnf+0x520>
-	xorpd  0xad70(%rip),%xmm2        
+	je     d3c0 <music_track_multiturnf+0x520>
+	xorpd  0xadb0(%rip),%xmm2        
 	comiss %xmm3,%xmm12
 	cvtsd2ss %xmm0,%xmm0
-	jbe    d412 <music_track_multiturnf+0x532>
-	xorpd  0xad5e(%rip),%xmm2        
+	jbe    d3d2 <music_track_multiturnf+0x532>
+	xorpd  0xad9e(%rip),%xmm2        
 	movss  0x14(%rsp),%xmm3
 	mov    0x28(%rsp),%rax
 	pxor   %xmm1,%xmm1
 	pxor   %xmm11,%xmm11
 	cvtsd2ss %xmm2,%xmm1
 	movss  0x18(%rsp),%xmm4
 	movss  0x20(%rsp),%xmm2
@@ -9146,150 +9140,150 @@
 	mulss  %xmm7,%xmm2
 	addss  %xmm3,%xmm4
 	mulss  %xmm1,%xmm5
 	mulss  %xmm10,%xmm4
 	addss  %xmm5,%xmm2
 	cvtss2sd %xmm4,%xmm0
 	addsd  %xmm8,%xmm0
-	addss  0xae5d(%rip),%xmm4        
+	addss  0xae9d(%rip),%xmm4        
 	mulss  %xmm10,%xmm2
 	mulsd  %xmm11,%xmm0
 	cvtsd2ss %xmm0,%xmm0
 	movss  %xmm0,(%r10)
 	addss  0x0(%rbp),%xmm0
 	movss  %xmm0,0x0(%rbp)
 	cmp    $0x1,%eax
-	jle    d7c5 <music_track_multiturnf+0x8e5>
-	movsd  0xaea6(%rip),%xmm14        
+	jle    d785 <music_track_multiturnf+0x8e5>
+	movsd  0xaee6(%rip),%xmm14        
 	lea    -0x2(%rax),%r9d
 	mov    $0x1,%eax
 	add    $0x2,%r9
 	nopw   0x0(%rax,%rax,1)
 	movaps %xmm6,%xmm1
 	movss  (%r12,%rax,4),%xmm6
 	movapd %xmm14,%xmm0
 	movaps %xmm6,%xmm5
 	subss  %xmm1,%xmm5
 	subss  %xmm6,%xmm1
 	mulss  0xc(%rsp),%xmm1
-	comiss 0xaec2(%rip),%xmm1        
-	ja     d5cf <music_track_multiturnf+0x6ef>
-	movsd  0xae6c(%rip),%xmm3        
+	comiss 0xaf02(%rip),%xmm1        
+	ja     d58f <music_track_multiturnf+0x6ef>
+	movsd  0xaeac(%rip),%xmm3        
 	pxor   %xmm0,%xmm0
 	pxor   %xmm7,%xmm7
 	cvtss2sd %xmm1,%xmm0
 	mulsd  %xmm0,%xmm3
 	addsd  %xmm8,%xmm3
 	cvttsd2si %xmm3,%edx
 	cvtsd2ss %xmm3,%xmm7
 	movd   %xmm7,%ecx
 	pxor   %xmm3,%xmm3
 	shr    $0x1f,%ecx
 	movapd %xmm0,%xmm7
-	movsd  0xae48(%rip),%xmm0        
+	movsd  0xae88(%rip),%xmm0        
 	sub    %ecx,%edx
 	cvtsi2sd %edx,%xmm3
-	mulsd  0xae32(%rip),%xmm3        
+	mulsd  0xae72(%rip),%xmm3        
 	movslq %edx,%rdx
 	add    $0x3ff,%rdx
 	shl    $0x34,%rdx
 	subsd  %xmm3,%xmm7
 	movapd %xmm7,%xmm3
 	mulsd  %xmm7,%xmm3
 	mulsd  %xmm3,%xmm0
-	addsd  0xae1c(%rip),%xmm0        
+	addsd  0xae5c(%rip),%xmm0        
 	mulsd  %xmm3,%xmm0
 	addsd  %xmm9,%xmm0
 	mulsd  %xmm7,%xmm0
-	movsd  0xae0f(%rip),%xmm7        
+	movsd  0xae4f(%rip),%xmm7        
 	mulsd  %xmm3,%xmm7
-	addsd  0xae0b(%rip),%xmm7        
+	addsd  0xae4b(%rip),%xmm7        
 	mulsd  %xmm3,%xmm7
-	addsd  0xae07(%rip),%xmm7        
+	addsd  0xae47(%rip),%xmm7        
 	mulsd  %xmm3,%xmm7
-	addsd  0xae03(%rip),%xmm7        
+	addsd  0xae43(%rip),%xmm7        
 	subsd  %xmm0,%xmm7
 	divsd  %xmm7,%xmm0
 	movq   %rdx,%xmm7
 	addsd  %xmm0,%xmm0
 	addsd  %xmm9,%xmm0
 	mulsd  %xmm7,%xmm0
 	comiss %xmm1,%xmm15
 	movaps %xmm12,%xmm7
-	ja     d5e1 <music_track_multiturnf+0x701>
+	ja     d5a1 <music_track_multiturnf+0x701>
 	pxor   %xmm7,%xmm7
 	cvtsd2ss %xmm0,%xmm7
 	mulss  0x10(%rsp),%xmm5
-	movsd  0xac71(%rip),%xmm0        
+	movsd  0xacb1(%rip),%xmm0        
 	pxor   %xmm3,%xmm3
 	cvtss2sd %xmm5,%xmm3
 	andpd  %xmm13,%xmm3
 	mulsd  %xmm3,%xmm0
 	cvttsd2si %xmm0,%edx
 	pxor   %xmm0,%xmm0
 	add    $0x1,%edx
 	mov    %edx,%ecx
 	and    $0x4,%edx
 	and    $0xfffffffe,%ecx
 	cvtsi2sd %ecx,%xmm0
-	mulsd  0xac49(%rip),%xmm0        
+	mulsd  0xac89(%rip),%xmm0        
 	sub    $0x2,%ecx
 	mov    %ecx,%edi
 	and    $0x4,%edi
 	and    $0x2,%ecx
 	subsd  %xmm0,%xmm3
-	movsd  0xac3a(%rip),%xmm0        
+	movsd  0xac7a(%rip),%xmm0        
 	movapd %xmm3,%xmm1
 	mulsd  %xmm3,%xmm1
 	mulsd  %xmm1,%xmm0
 	movapd %xmm1,%xmm10
-	subsd  0xac29(%rip),%xmm0        
+	subsd  0xac69(%rip),%xmm0        
 	mulsd  %xmm3,%xmm10
 	mulsd  %xmm1,%xmm0
-	addsd  0xac20(%rip),%xmm0        
+	addsd  0xac60(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
-	subsd  0xac1c(%rip),%xmm0        
+	subsd  0xac5c(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
-	addsd  0xac18(%rip),%xmm0        
+	addsd  0xac58(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
-	subsd  0xac14(%rip),%xmm0        
+	subsd  0xac54(%rip),%xmm0        
 	mulsd  %xmm10,%xmm0
 	movapd %xmm1,%xmm10
 	mulsd  %xmm1,%xmm10
 	addsd  %xmm3,%xmm0
-	movsd  0xac01(%rip),%xmm3        
+	movsd  0xac41(%rip),%xmm3        
 	mulsd  %xmm1,%xmm3
-	addsd  0xabfd(%rip),%xmm3        
+	addsd  0xac3d(%rip),%xmm3        
 	mulsd  %xmm1,%xmm3
-	subsd  0xabf9(%rip),%xmm3        
+	subsd  0xac39(%rip),%xmm3        
 	mulsd  %xmm1,%xmm3
-	addsd  0xabf5(%rip),%xmm3        
+	addsd  0xac35(%rip),%xmm3        
 	mulsd  %xmm1,%xmm3
-	subsd  0xabf1(%rip),%xmm3        
+	subsd  0xac31(%rip),%xmm3        
 	mulsd  %xmm1,%xmm3
-	addsd  0xabed(%rip),%xmm3        
+	addsd  0xac2d(%rip),%xmm3        
 	mulsd  %xmm8,%xmm1
 	mulsd  %xmm10,%xmm3
 	movapd %xmm9,%xmm10
 	subsd  %xmm1,%xmm10
 	addsd  %xmm10,%xmm3
-	jne    d704 <music_track_multiturnf+0x824>
+	jne    d6c4 <music_track_multiturnf+0x824>
 	movq   %xmm0,%rcx
 	movapd %xmm3,%xmm0
 	movq   %rcx,%xmm3
 	test   %edi,%edi
-	jne    d710 <music_track_multiturnf+0x830>
-	xorpd  0xaa60(%rip),%xmm3        
+	jne    d6d0 <music_track_multiturnf+0x830>
+	xorpd  0xaaa0(%rip),%xmm3        
 	test   %edx,%edx
-	je     d71c <music_track_multiturnf+0x83c>
-	xorpd  0xaa54(%rip),%xmm0        
+	je     d6dc <music_track_multiturnf+0x83c>
+	xorpd  0xaa94(%rip),%xmm0        
 	comiss %xmm5,%xmm12
 	cvtsd2ss %xmm3,%xmm3
-	jbe    d72e <music_track_multiturnf+0x84e>
-	xorpd  0xaa42(%rip),%xmm0        
+	jbe    d6ee <music_track_multiturnf+0x84e>
+	xorpd  0xaa82(%rip),%xmm0        
 	movss  0x14(%rsp),%xmm1
 	cvtsd2ss %xmm0,%xmm0
 	movss  0x18(%rsp),%xmm5
 	movss  0x20(%rsp),%xmm10
 	mulss  %xmm0,%xmm1
 	mulss  %xmm2,%xmm5
 	mulss  %xmm0,%xmm10
@@ -9301,132 +9295,132 @@
 	mulss  %xmm2,%xmm3
 	addss  %xmm5,%xmm1
 	mulss  %xmm0,%xmm4
 	pxor   %xmm0,%xmm0
 	movaps %xmm3,%xmm2
 	mulss  %xmm7,%xmm1
 	addss  %xmm4,%xmm2
-	movss  0xab6c(%rip),%xmm4        
+	movss  0xabac(%rip),%xmm4        
 	cvtss2sd %xmm1,%xmm0
 	addsd  %xmm8,%xmm0
 	addss  %xmm1,%xmm4
 	mulss  %xmm7,%xmm2
 	mulsd  %xmm11,%xmm0
 	cvtsd2ss %xmm0,%xmm0
 	movss  %xmm0,(%r10,%rax,4)
 	addss  0x0(%rbp,%rax,4),%xmm0
 	movss  %xmm0,0x0(%rbp,%rax,4)
 	add    $0x1,%rax
 	cmp    %rax,%r9
-	jne    d4e0 <music_track_multiturnf+0x600>
+	jne    d4a0 <music_track_multiturnf+0x600>
 	mov    0x28(%rsp),%rax
 	movss  -0x4(%r12,%r13,4),%xmm0
 	movss  %xmm4,(%rax)
 	movss  %xmm2,0x4(%rax)
 	movss  %xmm0,0xc(%rax)
 	test   %r8,%r8
-	je     d7ec <music_track_multiturnf+0x90c>
+	je     d7ac <music_track_multiturnf+0x90c>
 	mov    %r8,%rdi
 	call   3130 <operator delete(void*)@plt>
 	add    $0x88,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	xchg   %ax,%ax
 	pxor   %xmm12,%xmm12
 	movaps %xmm12,%xmm10
-	jmp    d2c4 <music_track_multiturnf+0x3e4>
+	jmp    d284 <music_track_multiturnf+0x3e4>
 	xchg   %ax,%ax
-	movsd  0xab58(%rip),%xmm0        
-	movsd  0xaaaf(%rip),%xmm8        
-	movsd  0xaaae(%rip),%xmm9        
-	jmp    d2a2 <music_track_multiturnf+0x3c2>
+	movsd  0xab98(%rip),%xmm0        
+	movsd  0xaaef(%rip),%xmm8        
+	movsd  0xaaee(%rip),%xmm9        
+	jmp    d262 <music_track_multiturnf+0x3c2>
 	nop
 	lea    0x80(%r15),%rbx
 	mov    %rbp,0x48(%rsp)
 	mov    %rbx,%rbp
 	mov    %r15,%rbx
 	mov    %r8,%r15
-	jmp    d896 <music_track_multiturnf+0x9b6>
+	jmp    d856 <music_track_multiturnf+0x9b6>
 	nopw   0x0(%rax,%rax,1)
 	cmp    %r14,%rbx
-	je     d884 <music_track_multiturnf+0x9a4>
+	je     d844 <music_track_multiturnf+0x9a4>
 	mov    $0x8,%eax
 	mov    %r14,%rdx
 	mov    %rbx,%rsi
 	movss  %xmm1,0x44(%rsp)
 	sub    %rbx,%rdx
 	lea    (%rbx,%rax,1),%rdi
 	movss  %xmm0,0x38(%rsp)
 	call   31f0 <memmove@plt>
 	movss  0x44(%rsp),%xmm1
 	movss  0x38(%rsp),%xmm0
 	add    $0x8,%r14
 	movss  %xmm1,(%rbx)
 	movss  %xmm0,0x4(%rbx)
 	cmp    %r14,%rbp
-	je     d8de <music_track_multiturnf+0x9fe>
+	je     d89e <music_track_multiturnf+0x9fe>
 	movss  0x4(%r14),%xmm0
 	comiss 0x4(%rbx),%xmm0
 	mov    %r14,%rcx
 	movss  (%r14),%xmm1
-	jb     d850 <music_track_multiturnf+0x970>
+	jb     d810 <music_track_multiturnf+0x970>
 	comiss -0x4(%r14),%xmm0
 	lea    -0x8(%r14),%rax
-	jae    d8cc <music_track_multiturnf+0x9ec>
+	jae    d88c <music_track_multiturnf+0x9ec>
 	nopl   (%rax)
 	mov    (%rax),%rdx
 	mov    %rax,%rcx
 	sub    $0x8,%rax
 	mov    %rdx,0x10(%rax)
 	comiss 0x4(%rax),%xmm0
-	jb     d8b8 <music_track_multiturnf+0x9d8>
+	jb     d878 <music_track_multiturnf+0x9d8>
 	add    $0x8,%r14
 	movss  %xmm1,(%rcx)
 	movss  %xmm0,0x4(%rcx)
 	cmp    %r14,%rbp
-	jne    d896 <music_track_multiturnf+0x9b6>
+	jne    d856 <music_track_multiturnf+0x9b6>
 	mov    %rbp,%rbx
 	mov    %r15,%r8
 	mov    0x48(%rsp),%rbp
 	mov    %rbx,%rsi
 	cmp    %r15,%rbx
-	je     d0d3 <music_track_multiturnf+0x1f3>
+	je     d093 <music_track_multiturnf+0x1f3>
 	nopl   (%rax)
 	movss  0x4(%rsi),%xmm0
 	comiss -0x4(%rsi),%xmm0
 	mov    %rsi,%rcx
 	lea    -0x8(%rsi),%rax
 	movss  (%rsi),%xmm1
-	jae    d924 <music_track_multiturnf+0xa44>
+	jae    d8e4 <music_track_multiturnf+0xa44>
 	xchg   %ax,%ax
 	mov    (%rax),%rdx
 	mov    %rax,%rcx
 	sub    $0x8,%rax
 	mov    %rdx,0x10(%rax)
 	comiss 0x4(%rax),%xmm0
-	jb     d910 <music_track_multiturnf+0xa30>
+	jb     d8d0 <music_track_multiturnf+0xa30>
 	add    $0x8,%rsi
 	movss  %xmm1,(%rcx)
 	movss  %xmm0,0x4(%rcx)
 	cmp    %r8,%rsi
-	jne    d8f8 <music_track_multiturnf+0xa18>
+	jne    d8b8 <music_track_multiturnf+0xa18>
 	mov    0x60(%rsp),%r8
-	jmp    d0d8 <music_track_multiturnf+0x1f8>
+	jmp    d098 <music_track_multiturnf+0x1f8>
 	xor    %eax,%eax
-	jmp    d137 <music_track_multiturnf+0x257>
+	jmp    d0f7 <music_track_multiturnf+0x257>
 	mov    %rax,%rbp
 	jmp    3304 <music_track_multiturnf.cold>
 	nop
 
-000000000000d950 <music_trackf>:
+000000000000d910 <music_trackf>:
 music_trackf():
 	push   %r15
 	push   %r14
 	push   %r13
 	movslq %r8d,%r13
 	push   %r12
 	mov    %rdi,%r12
@@ -9449,301 +9443,301 @@
 	movss  %xmm4,0x18(%rsp)
 	movss  %xmm5,0x1c(%rsp)
 	movss  %xmm6,0x20(%rsp)
 	movaps %xmm0,0x60(%rsp)
 	call   30b0 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)@plt>
 	mov    0x68(%rsp),%r8
 	test   %r13d,%r13d
-	jle    da40 <music_trackf+0xf0>
+	jle    da00 <music_trackf+0xf0>
 	xor    %ebx,%ebx
 	lea    0x58(%rsp),%r15
-	jmp    d9fb <music_trackf+0xab>
+	jmp    d9bb <music_trackf+0xab>
 	nopl   0x0(%rax,%rax,1)
 	mov    0x58(%rsp),%rax
 	add    $0x8,%r8
 	add    $0x1,%rbx
 	mov    %rax,-0x8(%r8)
 	mov    %r8,0x68(%rsp)
 	cmp    %r13,%rbx
-	je     da40 <music_trackf+0xf0>
+	je     da00 <music_trackf+0xf0>
 	movss  0x0(%rbp,%rbx,4),%xmm0
 	movss  %xmm0,0x58(%rsp)
 	movss  (%r12,%rbx,4),%xmm0
 	movss  %xmm0,0x5c(%rsp)
 	cmp    %r8,0x70(%rsp)
-	jne    d9e0 <music_trackf+0x90>
+	jne    d9a0 <music_trackf+0x90>
 	mov    %r15,%rdx
 	mov    %r8,%rsi
 	mov    %r14,%rdi
 	call   3210 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)@plt>
 	add    $0x1,%rbx
 	mov    0x68(%rsp),%r8
 	cmp    %r13,%rbx
-	jne    d9fb <music_trackf+0xab>
+	jne    d9bb <music_trackf+0xab>
 	cs nopw 0x0(%rax,%rax,1)
 	mov    0x60(%rsp),%r15
 	cmp    %r8,%r15
-	je     db48 <music_trackf+0x1f8>
+	je     db08 <music_trackf+0x1f8>
 	mov    %r8,%rbx
 	mov    $0x3f,%edx
 	mov    %r8,%rsi
 	mov    %r15,%rdi
 	sub    %r15,%rbx
 	mov    %r8,0x38(%rsp)
 	lea    0x8(%r15),%r14
 	mov    %rbx,%rax
 	sar    $0x3,%rax
 	bsr    %rax,%rax
 	xor    $0x3f,%rax
 	sub    %eax,%edx
 	movslq %edx,%rdx
 	add    %rdx,%rdx
-	call   b950 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   b910 <void std::__introsort_loop<__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter>(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, __gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	cmp    $0x80,%rbx
 	mov    0x38(%rsp),%r8
-	jg     dfb0 <music_trackf+0x660>
+	jg     df70 <music_trackf+0x660>
 	mov    $0x8,%ebx
 	cmp    %r14,%r8
-	je     db43 <music_trackf+0x1f3>
+	je     db03 <music_trackf+0x1f3>
 	mov    %rbp,0x48(%rsp)
 	mov    %r8,%rbp
-	jmp    daf3 <music_trackf+0x1a3>
+	jmp    dab3 <music_trackf+0x1a3>
 	xchg   %ax,%ax
 	cmp    %r14,%r15
-	je     dadf <music_trackf+0x18f>
+	je     da9f <music_trackf+0x18f>
 	mov    %r14,%rdx
 	lea    (%r15,%rbx,1),%rdi
 	mov    %r15,%rsi
 	movss  %xmm1,0x44(%rsp)
 	sub    %r15,%rdx
 	movss  %xmm0,0x38(%rsp)
 	call   31f0 <memmove@plt>
 	movss  0x44(%rsp),%xmm1
 	movss  0x38(%rsp),%xmm0
 	add    $0x8,%r14
 	movss  %xmm1,(%r15)
 	movss  %xmm0,0x4(%r15)
 	cmp    %rbp,%r14
-	je     db3e <music_trackf+0x1ee>
+	je     dafe <music_trackf+0x1ee>
 	movss  0x4(%r14),%xmm0
 	comiss 0x4(%r15),%xmm0
 	mov    %r14,%rcx
 	movss  (%r14),%xmm1
-	jb     dab0 <music_trackf+0x160>
+	jb     da70 <music_trackf+0x160>
 	comiss -0x4(%r14),%xmm0
 	lea    -0x8(%r14),%rax
-	jae    db2c <music_trackf+0x1dc>
+	jae    daec <music_trackf+0x1dc>
 	nopl   0x0(%rax,%rax,1)
 	mov    (%rax),%rdx
 	mov    %rax,%rcx
 	sub    $0x8,%rax
 	mov    %rdx,0x10(%rax)
 	comiss 0x4(%rax),%xmm0
-	jb     db18 <music_trackf+0x1c8>
+	jb     dad8 <music_trackf+0x1c8>
 	add    $0x8,%r14
 	movss  %xmm1,(%rcx)
 	movss  %xmm0,0x4(%rcx)
 	cmp    %rbp,%r14
-	jne    daf3 <music_trackf+0x1a3>
+	jne    dab3 <music_trackf+0x1a3>
 	mov    0x48(%rsp),%rbp
 	mov    0x60(%rsp),%r8
 	mov    0x24(%rsp),%edi
 	test   %edi,%edi
-	jle    e0c0 <music_trackf+0x770>
+	jle    e080 <music_trackf+0x770>
 	lea    -0x1(%rdi),%eax
 	cmp    $0x2,%eax
-	jbe    e0e4 <music_trackf+0x794>
+	jbe    e0a4 <music_trackf+0x794>
 	shr    $0x2,%edi
 	xor    %eax,%eax
 	mov    %edi,%edx
 	shl    $0x4,%rdx
 	nopl   0x0(%rax,%rax,1)
 	movups (%r8,%rax,2),%xmm0
 	movups 0x10(%r8,%rax,2),%xmm1
 	movaps %xmm0,%xmm2
 	shufps $0xdd,%xmm1,%xmm0
 	movups %xmm0,(%r12,%rax,1)
 	shufps $0x88,%xmm1,%xmm2
 	movups %xmm2,0x0(%rbp,%rax,1)
 	add    $0x10,%rax
 	cmp    %rax,%rdx
-	jne    db70 <music_trackf+0x220>
+	jne    db30 <music_trackf+0x220>
 	mov    0x24(%rsp),%edi
 	mov    %edi,%eax
 	and    $0xfffffffc,%eax
 	and    $0x3,%edi
-	je     dc10 <music_trackf+0x2c0>
+	je     dbd0 <music_trackf+0x2c0>
 	movslq %eax,%rdx
 	mov    0x24(%rsp),%edi
 	lea    (%r8,%rdx,8),%rcx
 	movss  (%rcx),%xmm0
 	movss  %xmm0,0x0(%rbp,%rdx,4)
 	movss  0x4(%rcx),%xmm0
 	movss  %xmm0,(%r12,%rdx,4)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%edi
-	jle    e0eb <music_trackf+0x79b>
+	jle    e0ab <music_trackf+0x79b>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	lea    (%r8,%rdx,8),%rcx
 	movss  (%rcx),%xmm0
 	movss  %xmm0,0x0(%rbp,%rdx,4)
 	movss  0x4(%rcx),%xmm0
 	movss  %xmm0,(%r12,%rdx,4)
 	cmp    %eax,%edi
-	jle    dc10 <music_trackf+0x2c0>
+	jle    dbd0 <music_trackf+0x2c0>
 	cltq
 	lea    (%r8,%rax,8),%rdx
 	movss  (%rdx),%xmm0
 	movss  %xmm0,0x0(%rbp,%rax,4)
 	movss  0x4(%rdx),%xmm0
 	movss  %xmm0,(%r12,%rax,4)
 	mov    0x28(%rsp),%rax
 	movss  0x0(%rbp),%xmm0
 	addss  (%rax),%xmm0
 	movss  %xmm0,0x0(%rbp)
 	mov    0x24(%rsp),%eax
 	pxor   %xmm9,%xmm9
 	movss  (%r12),%xmm6
 	pxor   %xmm15,%xmm15
-	movss  0xa6b9(%rip),%xmm4        
+	movss  0xa6f9(%rip),%xmm4        
 	mov    0x28(%rsp),%r9
 	movaps %xmm9,%xmm2
 	cvtss2sd 0x40(%rsp),%xmm15
-	movsd  0xa678(%rip),%xmm8        
+	movsd  0xa6b8(%rip),%xmm8        
 	lea    -0x2(%rax),%edi
-	movsd  0xa674(%rip),%xmm10        
+	movsd  0xa6b4(%rip),%xmm10        
 	mov    $0x1,%eax
-	movss  0xa75a(%rip),%xmm14        
+	movss  0xa79a(%rip),%xmm14        
 	add    $0x2,%rdi
-	movq   0xa4e1(%rip),%xmm13        
-	movsd  0xa6e8(%rip),%xmm12        
+	movq   0xa521(%rip),%xmm13        
+	movsd  0xa728(%rip),%xmm12        
 	nopl   0x0(%rax,%rax,1)
 	movaps %xmm6,%xmm1
 	movss  (%r12,%rax,4),%xmm6
 	movapd %xmm12,%xmm0
 	movaps %xmm6,%xmm5
 	subss  %xmm1,%xmm5
 	subss  %xmm6,%xmm1
 	mulss  0xc(%rsp),%xmm1
-	comiss 0xa712(%rip),%xmm1        
-	ja     dd7f <music_trackf+0x42f>
-	movsd  0xa6bc(%rip),%xmm3        
+	comiss 0xa752(%rip),%xmm1        
+	ja     dd3f <music_trackf+0x42f>
+	movsd  0xa6fc(%rip),%xmm3        
 	pxor   %xmm0,%xmm0
 	pxor   %xmm7,%xmm7
 	cvtss2sd %xmm1,%xmm0
 	mulsd  %xmm0,%xmm3
 	addsd  %xmm8,%xmm3
 	cvttsd2si %xmm3,%edx
 	cvtsd2ss %xmm3,%xmm7
 	movd   %xmm7,%ecx
 	pxor   %xmm3,%xmm3
 	shr    $0x1f,%ecx
 	movapd %xmm0,%xmm7
-	movsd  0xa698(%rip),%xmm0        
+	movsd  0xa6d8(%rip),%xmm0        
 	sub    %ecx,%edx
 	cvtsi2sd %edx,%xmm3
-	mulsd  0xa682(%rip),%xmm3        
+	mulsd  0xa6c2(%rip),%xmm3        
 	movslq %edx,%rdx
 	add    $0x3ff,%rdx
 	shl    $0x34,%rdx
 	subsd  %xmm3,%xmm7
 	movapd %xmm7,%xmm3
 	mulsd  %xmm7,%xmm3
 	mulsd  %xmm3,%xmm0
-	addsd  0xa66c(%rip),%xmm0        
+	addsd  0xa6ac(%rip),%xmm0        
 	mulsd  %xmm3,%xmm0
 	addsd  %xmm10,%xmm0
 	mulsd  %xmm7,%xmm0
-	movsd  0xa65f(%rip),%xmm7        
+	movsd  0xa69f(%rip),%xmm7        
 	mulsd  %xmm3,%xmm7
-	addsd  0xa65b(%rip),%xmm7        
+	addsd  0xa69b(%rip),%xmm7        
 	mulsd  %xmm3,%xmm7
-	addsd  0xa657(%rip),%xmm7        
+	addsd  0xa697(%rip),%xmm7        
 	mulsd  %xmm3,%xmm7
-	addsd  0xa653(%rip),%xmm7        
+	addsd  0xa693(%rip),%xmm7        
 	subsd  %xmm0,%xmm7
 	divsd  %xmm7,%xmm0
 	movq   %rdx,%xmm7
 	addsd  %xmm0,%xmm0
 	addsd  %xmm10,%xmm0
 	mulsd  %xmm7,%xmm0
 	comiss %xmm1,%xmm14
 	movaps %xmm9,%xmm7
-	ja     dd91 <music_trackf+0x441>
+	ja     dd51 <music_trackf+0x441>
 	pxor   %xmm7,%xmm7
 	cvtsd2ss %xmm0,%xmm7
 	mulss  0x10(%rsp),%xmm5
-	movsd  0xa4c1(%rip),%xmm0        
+	movsd  0xa501(%rip),%xmm0        
 	pxor   %xmm3,%xmm3
 	cvtss2sd %xmm5,%xmm3
 	andpd  %xmm13,%xmm3
 	mulsd  %xmm3,%xmm0
 	cvttsd2si %xmm0,%edx
 	pxor   %xmm0,%xmm0
 	add    $0x1,%edx
 	mov    %edx,%ecx
 	and    $0x4,%edx
 	and    $0xfffffffe,%ecx
 	cvtsi2sd %ecx,%xmm0
-	mulsd  0xa499(%rip),%xmm0        
+	mulsd  0xa4d9(%rip),%xmm0        
 	sub    $0x2,%ecx
 	mov    %ecx,%esi
 	and    $0x4,%esi
 	and    $0x2,%ecx
 	subsd  %xmm0,%xmm3
-	movsd  0xa48a(%rip),%xmm0        
+	movsd  0xa4ca(%rip),%xmm0        
 	movapd %xmm3,%xmm1
 	mulsd  %xmm3,%xmm1
 	mulsd  %xmm1,%xmm0
 	movapd %xmm1,%xmm11
-	subsd  0xa479(%rip),%xmm0        
+	subsd  0xa4b9(%rip),%xmm0        
 	mulsd  %xmm3,%xmm11
 	mulsd  %xmm1,%xmm0
-	addsd  0xa470(%rip),%xmm0        
+	addsd  0xa4b0(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
-	subsd  0xa46c(%rip),%xmm0        
+	subsd  0xa4ac(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
-	addsd  0xa468(%rip),%xmm0        
+	addsd  0xa4a8(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
-	subsd  0xa464(%rip),%xmm0        
+	subsd  0xa4a4(%rip),%xmm0        
 	mulsd  %xmm11,%xmm0
 	movapd %xmm1,%xmm11
 	mulsd  %xmm1,%xmm11
 	addsd  %xmm3,%xmm0
-	movsd  0xa451(%rip),%xmm3        
+	movsd  0xa491(%rip),%xmm3        
 	mulsd  %xmm1,%xmm3
-	addsd  0xa44d(%rip),%xmm3        
+	addsd  0xa48d(%rip),%xmm3        
 	mulsd  %xmm1,%xmm3
-	subsd  0xa449(%rip),%xmm3        
+	subsd  0xa489(%rip),%xmm3        
 	mulsd  %xmm1,%xmm3
-	addsd  0xa445(%rip),%xmm3        
+	addsd  0xa485(%rip),%xmm3        
 	mulsd  %xmm1,%xmm3
-	subsd  0xa441(%rip),%xmm3        
+	subsd  0xa481(%rip),%xmm3        
 	mulsd  %xmm1,%xmm3
-	addsd  0xa43d(%rip),%xmm3        
+	addsd  0xa47d(%rip),%xmm3        
 	mulsd  %xmm8,%xmm1
 	mulsd  %xmm11,%xmm3
 	movapd %xmm10,%xmm11
 	subsd  %xmm1,%xmm11
 	addsd  %xmm11,%xmm3
-	jne    deb4 <music_trackf+0x564>
+	jne    de74 <music_trackf+0x564>
 	movq   %xmm0,%rcx
 	movapd %xmm3,%xmm0
 	movq   %rcx,%xmm3
 	test   %esi,%esi
-	jne    dec0 <music_trackf+0x570>
-	xorpd  0xa2b0(%rip),%xmm3        
+	jne    de80 <music_trackf+0x570>
+	xorpd  0xa2f0(%rip),%xmm3        
 	test   %edx,%edx
-	je     decc <music_trackf+0x57c>
-	xorpd  0xa2a4(%rip),%xmm0        
+	je     de8c <music_trackf+0x57c>
+	xorpd  0xa2e4(%rip),%xmm0        
 	comiss %xmm5,%xmm9
 	cvtsd2ss %xmm3,%xmm3
-	jbe    dede <music_trackf+0x58e>
-	xorpd  0xa292(%rip),%xmm0        
+	jbe    de9e <music_trackf+0x58e>
+	xorpd  0xa2d2(%rip),%xmm0        
 	movss  0x14(%rsp),%xmm1
 	cvtsd2ss %xmm0,%xmm0
 	movss  0x18(%rsp),%xmm5
 	movss  0x20(%rsp),%xmm11
 	mulss  %xmm0,%xmm1
 	mulss  %xmm2,%xmm5
 	mulss  %xmm0,%xmm11
@@ -9755,34 +9749,34 @@
 	mulss  %xmm2,%xmm3
 	addss  %xmm5,%xmm1
 	mulss  %xmm0,%xmm4
 	pxor   %xmm0,%xmm0
 	movaps %xmm3,%xmm2
 	mulss  %xmm7,%xmm1
 	addss  %xmm4,%xmm2
-	movss  0xa3bc(%rip),%xmm4        
+	movss  0xa3fc(%rip),%xmm4        
 	cvtss2sd %xmm1,%xmm0
 	addsd  %xmm8,%xmm0
 	addss  %xmm1,%xmm4
 	mulss  %xmm7,%xmm2
 	mulsd  %xmm15,%xmm0
 	cvtsd2ss %xmm0,%xmm0
 	movss  %xmm0,(%r9,%rax,4)
 	addss  0x0(%rbp,%rax,4),%xmm0
 	movss  %xmm0,0x0(%rbp,%rax,4)
 	add    $0x1,%rax
 	cmp    %rax,%rdi
-	jne    dc90 <music_trackf+0x340>
+	jne    dc50 <music_trackf+0x340>
 	mov    0x30(%rsp),%rax
 	movss  -0x4(%r12,%r13,4),%xmm0
 	movss  %xmm4,(%rax)
 	movss  %xmm2,0x4(%rax)
 	movss  %xmm0,0xc(%rax)
 	test   %r8,%r8
-	je     df9c <music_trackf+0x64c>
+	je     df5c <music_trackf+0x64c>
 	mov    %r8,%rdi
 	call   3130 <operator delete(void*)@plt>
 	add    $0x88,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
@@ -9791,143 +9785,143 @@
 	ret
 	xchg   %ax,%ax
 	lea    0x80(%r15),%rbx
 	mov    %rbp,0x48(%rsp)
 	mov    %rbx,%rbp
 	mov    %r15,%rbx
 	mov    %r8,%r15
-	jmp    e016 <music_trackf+0x6c6>
+	jmp    dfd6 <music_trackf+0x6c6>
 	nopw   0x0(%rax,%rax,1)
 	cmp    %r14,%rbx
-	je     e004 <music_trackf+0x6b4>
+	je     dfc4 <music_trackf+0x6b4>
 	mov    $0x8,%eax
 	mov    %r14,%rdx
 	mov    %rbx,%rsi
 	movss  %xmm1,0x44(%rsp)
 	sub    %rbx,%rdx
 	lea    (%rbx,%rax,1),%rdi
 	movss  %xmm0,0x38(%rsp)
 	call   31f0 <memmove@plt>
 	movss  0x44(%rsp),%xmm1
 	movss  0x38(%rsp),%xmm0
 	add    $0x8,%r14
 	movss  %xmm1,(%rbx)
 	movss  %xmm0,0x4(%rbx)
 	cmp    %r14,%rbp
-	je     e05e <music_trackf+0x70e>
+	je     e01e <music_trackf+0x70e>
 	movss  0x4(%r14),%xmm0
 	comiss 0x4(%rbx),%xmm0
 	mov    %r14,%rcx
 	movss  (%r14),%xmm1
-	jb     dfd0 <music_trackf+0x680>
+	jb     df90 <music_trackf+0x680>
 	comiss -0x4(%r14),%xmm0
 	lea    -0x8(%r14),%rax
-	jae    e04c <music_trackf+0x6fc>
+	jae    e00c <music_trackf+0x6fc>
 	nopl   (%rax)
 	mov    (%rax),%rdx
 	mov    %rax,%rcx
 	sub    $0x8,%rax
 	mov    %rdx,0x10(%rax)
 	comiss 0x4(%rax),%xmm0
-	jb     e038 <music_trackf+0x6e8>
+	jb     dff8 <music_trackf+0x6e8>
 	add    $0x8,%r14
 	movss  %xmm1,(%rcx)
 	movss  %xmm0,0x4(%rcx)
 	cmp    %r14,%rbp
-	jne    e016 <music_trackf+0x6c6>
+	jne    dfd6 <music_trackf+0x6c6>
 	mov    %rbp,%rbx
 	mov    %r15,%r8
 	mov    0x48(%rsp),%rbp
 	mov    %rbx,%rsi
 	cmp    %r15,%rbx
-	je     db43 <music_trackf+0x1f3>
+	je     db03 <music_trackf+0x1f3>
 	nopl   (%rax)
 	movss  0x4(%rsi),%xmm0
 	comiss -0x4(%rsi),%xmm0
 	mov    %rsi,%rcx
 	lea    -0x8(%rsi),%rax
 	movss  (%rsi),%xmm1
-	jae    e0a4 <music_trackf+0x754>
+	jae    e064 <music_trackf+0x754>
 	xchg   %ax,%ax
 	mov    (%rax),%rdx
 	mov    %rax,%rcx
 	sub    $0x8,%rax
 	mov    %rdx,0x10(%rax)
 	comiss 0x4(%rax),%xmm0
-	jb     e090 <music_trackf+0x740>
+	jb     e050 <music_trackf+0x740>
 	add    $0x8,%rsi
 	movss  %xmm1,(%rcx)
 	movss  %xmm0,0x4(%rcx)
 	cmp    %r8,%rsi
-	jne    e078 <music_trackf+0x728>
+	jne    e038 <music_trackf+0x728>
 	mov    0x60(%rsp),%r8
-	jmp    db48 <music_trackf+0x1f8>
+	jmp    db08 <music_trackf+0x1f8>
 	mov    0x28(%rsp),%rax
 	movss  0x0(%rbp),%xmm0
 	pxor   %xmm2,%xmm2
-	movss  0xa222(%rip),%xmm4        
+	movss  0xa262(%rip),%xmm4        
 	addss  (%rax),%xmm0
 	movss  %xmm0,0x0(%rbp)
-	jmp    df75 <music_trackf+0x625>
+	jmp    df35 <music_trackf+0x625>
 	xor    %eax,%eax
-	jmp    dba7 <music_trackf+0x257>
+	jmp    db67 <music_trackf+0x257>
 	mov    0x28(%rsp),%rax
 	movss  0x0(%rbp),%xmm0
 	cmpl   $0x1,0x24(%rsp)
 	addss  (%rax),%xmm0
 	movss  %xmm0,0x0(%rbp)
-	jg     dc23 <music_trackf+0x2d3>
-	movss  0xa1e7(%rip),%xmm4        
+	jg     dbe3 <music_trackf+0x2d3>
+	movss  0xa227(%rip),%xmm4        
 	pxor   %xmm2,%xmm2
-	jmp    df75 <music_trackf+0x625>
+	jmp    df35 <music_trackf+0x625>
 	mov    %rax,%rbp
 	jmp    331b <music_trackf.cold>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
-000000000000e130 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)>:
+000000000000e0f0 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)>:
 std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long):
 	movabs $0x7ffffffffffffff,%rax
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
 	cmp    %rax,%rsi
-	ja     e1e0 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)+0xb0>
+	ja     e1a0 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)+0xb0>
 	mov    (%rdi),%rbp
 	mov    0x10(%rdi),%rax
 	mov    %rdi,%rbx
 	sub    %rbp,%rax
 	sar    $0x4,%rax
 	cmp    %rax,%rsi
-	ja     e170 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)+0x40>
+	ja     e130 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)+0x40>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	nopw   0x0(%rax,%rax,1)
 	mov    0x8(%rdi),%r13
 	mov    %rsi,%r14
 	shl    $0x4,%r14
 	sub    %rbp,%r13
 	test   %rsi,%rsi
-	je     e1d8 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)+0xa8>
+	je     e198 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)+0xa8>
 	mov    %r14,%rdi
 	call   3160 <operator new(unsigned long)@plt>
 	mov    (%rbx),%rbp
 	mov    0x8(%rbx),%rdx
 	mov    %rax,%r12
 	sub    %rbp,%rdx
 	test   %rdx,%rdx
-	jg     e1c0 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)+0x90>
+	jg     e180 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)+0x90>
 	test   %rbp,%rbp
-	jne    e1cb <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)+0x9b>
+	jne    e18b <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)+0x9b>
 	mov    %r12,(%rbx)
 	add    %r12,%r13
 	add    %r14,%r12
 	mov    %r13,0x8(%rbx)
 	mov    %r12,0x10(%rbx)
 	pop    %rbx
 	pop    %rbp
@@ -9937,62 +9931,62 @@
 	ret
 	nopl   0x0(%rax)
 	mov    %rbp,%rsi
 	mov    %r12,%rdi
 	call   31f0 <memmove@plt>
 	mov    %rbp,%rdi
 	call   3130 <operator delete(void*)@plt>
-	jmp    e1a2 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)+0x72>
+	jmp    e162 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)+0x72>
 	nopl   (%rax)
 	mov    %r13,%rdx
 	xor    %r12d,%r12d
-	jmp    e198 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)+0x68>
-	lea    0xa15d(%rip),%rdi        
+	jmp    e158 <std::vector<particle<double>, std::allocator<particle<double> > >::reserve(unsigned long)+0x68>
+	lea    0xa19d(%rip),%rdi        
 	call   30d0 <std::__throw_length_error(char const*)@plt>
 	nopl   0x0(%rax)
 
-000000000000e1f0 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)>:
+000000000000e1b0 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)>:
 std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long):
 	movabs $0xfffffffffffffff,%rax
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
 	cmp    %rax,%rsi
-	ja     e2a0 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)+0xb0>
+	ja     e260 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)+0xb0>
 	mov    (%rdi),%rbp
 	mov    0x10(%rdi),%rax
 	mov    %rdi,%rbx
 	sub    %rbp,%rax
 	sar    $0x3,%rax
 	cmp    %rax,%rsi
-	ja     e230 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)+0x40>
+	ja     e1f0 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)+0x40>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	nopw   0x0(%rax,%rax,1)
 	mov    0x8(%rdi),%r13
 	lea    0x0(,%rsi,8),%r14
 	sub    %rbp,%r13
 	test   %rsi,%rsi
-	je     e298 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)+0xa8>
+	je     e258 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)+0xa8>
 	mov    %r14,%rdi
 	call   3160 <operator new(unsigned long)@plt>
 	mov    (%rbx),%rbp
 	mov    0x8(%rbx),%rdx
 	mov    %rax,%r12
 	sub    %rbp,%rdx
 	test   %rdx,%rdx
-	jg     e280 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)+0x90>
+	jg     e240 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)+0x90>
 	test   %rbp,%rbp
-	jne    e28b <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)+0x9b>
+	jne    e24b <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)+0x9b>
 	mov    %r12,(%rbx)
 	add    %r12,%r13
 	add    %r14,%r12
 	mov    %r13,0x8(%rbx)
 	mov    %r12,0x10(%rbx)
 	pop    %rbx
 	pop    %rbp
@@ -10002,24 +9996,24 @@
 	ret
 	nopl   (%rax)
 	mov    %rbp,%rsi
 	mov    %r12,%rdi
 	call   31f0 <memmove@plt>
 	mov    %rbp,%rdi
 	call   3130 <operator delete(void*)@plt>
-	jmp    e263 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)+0x73>
+	jmp    e223 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)+0x73>
 	nopl   (%rax)
 	mov    %r13,%rdx
 	xor    %r12d,%r12d
-	jmp    e259 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)+0x69>
-	lea    0xa09d(%rip),%rdi        
+	jmp    e219 <std::vector<particle<float>, std::allocator<particle<float> > >::reserve(unsigned long)+0x69>
+	lea    0xa0dd(%rip),%rdi        
 	call   30d0 <std::__throw_length_error(char const*)@plt>
 	nopl   0x0(%rax)
 
-000000000000e2b0 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)>:
+000000000000e270 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)>:
 void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&):
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
@@ -10027,44 +10021,44 @@
 	sub    $0x18,%rsp
 	mov    0x8(%rdi),%r13
 	mov    (%rdi),%r15
 	mov    %r13,%rax
 	sub    %r15,%rax
 	sar    $0x4,%rax
 	cmp    %rbx,%rax
-	je     e3ec <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0x13c>
+	je     e3ac <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0x13c>
 	test   %rax,%rax
 	mov    %rdx,%rcx
 	mov    $0x1,%edx
 	mov    %rsi,%r14
 	cmovne %rax,%rdx
 	xor    %esi,%esi
 	mov    %rdi,%r12
 	add    %rdx,%rax
 	mov    %r14,%rdx
 	setb   %sil
 	sub    %r15,%rdx
 	test   %rsi,%rsi
-	jne    e3e0 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0x130>
+	jne    e3a0 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0x130>
 	test   %rax,%rax
-	jne    e370 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0xc0>
+	jne    e330 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0xc0>
 	xor    %ebx,%ebx
 	xor    %ebp,%ebp
 	movdqu (%rcx),%xmm1
 	lea    0x10(%rbp,%rdx,1),%r9
 	sub    %r14,%r13
 	lea    (%r9,%r13,1),%rax
 	mov    %rax,(%rsp)
 	movups %xmm1,0x0(%rbp,%rdx,1)
 	test   %rdx,%rdx
-	jg     e3a0 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0xf0>
+	jg     e360 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0xf0>
 	test   %r13,%r13
-	jg     e3c8 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0x118>
+	jg     e388 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0x118>
 	test   %r15,%r15
-	jne    e3ba <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0x10a>
+	jne    e37a <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0x10a>
 	movq   %rbp,%xmm0
 	mov    %rbx,0x10(%r12)
 	movhps (%rsp),%xmm0
 	movups %xmm0,(%r12)
 	add    $0x18,%rsp
 	pop    %rbx
 	pop    %rbp
@@ -10081,39 +10075,39 @@
 	mov    %rcx,0x8(%rsp)
 	mov    %rdx,(%rsp)
 	call   3160 <operator new(unsigned long)@plt>
 	mov    (%rsp),%rdx
 	mov    0x8(%rsp),%rcx
 	mov    %rax,%rbp
 	add    %rax,%rbx
-	jmp    e318 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0x68>
+	jmp    e2d8 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0x68>
 	mov    %r15,%rsi
 	mov    %rbp,%rdi
 	mov    %r9,0x8(%rsp)
 	call   31f0 <memmove@plt>
 	test   %r13,%r13
 	mov    0x8(%rsp),%r9
-	jg     e3c8 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0x118>
+	jg     e388 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0x118>
 	mov    %r15,%rdi
 	call   3130 <operator delete(void*)@plt>
-	jmp    e344 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0x94>
+	jmp    e304 <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0x94>
 	nopl   0x0(%rax)
 	mov    %r13,%rdx
 	mov    %r14,%rsi
 	mov    %r9,%rdi
 	call   3110 <memcpy@plt>
-	jmp    e33f <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0x8f>
+	jmp    e2ff <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0x8f>
 	nopl   0x0(%rax,%rax,1)
 	movabs $0x7ffffffffffffff0,%rbx
-	jmp    e37b <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0xcb>
-	lea    0x9f61(%rip),%rdi        
+	jmp    e33b <void std::vector<particle<double>, std::allocator<particle<double> > >::_M_realloc_insert<particle<double> >(__gnu_cxx::__normal_iterator<particle<double>*, std::vector<particle<double>, std::allocator<particle<double> > > >, particle<double>&&)+0xcb>
+	lea    0x9fa1(%rip),%rdi        
 	call   30d0 <std::__throw_length_error(char const*)@plt>
 	nopl   0x0(%rax,%rax,1)
 
-000000000000e400 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)>:
+000000000000e3c0 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)>:
 void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&):
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
@@ -10121,44 +10115,44 @@
 	sub    $0x18,%rsp
 	mov    0x8(%rdi),%r13
 	mov    (%rdi),%r15
 	mov    %r13,%rax
 	sub    %r15,%rax
 	sar    $0x3,%rax
 	cmp    %rbx,%rax
-	je     e544 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0x144>
+	je     e504 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0x144>
 	test   %rax,%rax
 	mov    %rdx,%rcx
 	mov    $0x1,%edx
 	mov    %rsi,%r14
 	cmovne %rax,%rdx
 	xor    %esi,%esi
 	mov    %rdi,%r12
 	add    %rdx,%rax
 	mov    %r14,%rdx
 	setb   %sil
 	sub    %r15,%rdx
 	test   %rsi,%rsi
-	jne    e538 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0x138>
+	jne    e4f8 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0x138>
 	test   %rax,%rax
-	jne    e4b8 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0xb8>
+	jne    e478 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0xb8>
 	xor    %ebx,%ebx
 	xor    %ebp,%ebp
 	mov    (%rcx),%rax
 	lea    0x8(%rbp,%rdx,1),%r9
 	sub    %r14,%r13
 	mov    %rax,0x0(%rbp,%rdx,1)
 	lea    (%r9,%r13,1),%rax
 	mov    %rax,(%rsp)
 	test   %rdx,%rdx
-	jg     e4f0 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0xf0>
+	jg     e4b0 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0xf0>
 	test   %r13,%r13
-	jg     e520 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0x120>
+	jg     e4e0 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0x120>
 	test   %r15,%r15
-	jne    e50a <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0x10a>
+	jne    e4ca <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0x10a>
 	movq   %rbp,%xmm0
 	mov    %rbx,0x10(%r12)
 	movhps (%rsp),%xmm0
 	movups %xmm0,(%r12)
 	add    $0x18,%rsp
 	pop    %rbx
 	pop    %rbp
@@ -10175,975 +10169,975 @@
 	mov    %rcx,0x8(%rsp)
 	mov    %rdx,(%rsp)
 	call   3160 <operator new(unsigned long)@plt>
 	mov    (%rsp),%rdx
 	mov    0x8(%rsp),%rcx
 	mov    %rax,%rbp
 	add    %rax,%rbx
-	jmp    e468 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0x68>
+	jmp    e428 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0x68>
 	nopl   0x0(%rax)
 	mov    %r15,%rsi
 	mov    %rbp,%rdi
 	mov    %r9,0x8(%rsp)
 	call   31f0 <memmove@plt>
 	test   %r13,%r13
 	mov    0x8(%rsp),%r9
-	jg     e520 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0x120>
+	jg     e4e0 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0x120>
 	mov    %r15,%rdi
 	call   3130 <operator delete(void*)@plt>
-	jmp    e493 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0x93>
+	jmp    e453 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0x93>
 	nopw   0x0(%rax,%rax,1)
 	mov    %r13,%rdx
 	mov    %r14,%rsi
 	mov    %r9,%rdi
 	call   3110 <memcpy@plt>
-	jmp    e48e <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0x8e>
+	jmp    e44e <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0x8e>
 	nopl   0x0(%rax,%rax,1)
 	movabs $0x7ffffffffffffff8,%rbx
-	jmp    e4c7 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0xc7>
-	lea    0x9e09(%rip),%rdi        
+	jmp    e487 <void std::vector<particle<float>, std::allocator<particle<float> > >::_M_realloc_insert<particle<float> >(__gnu_cxx::__normal_iterator<particle<float>*, std::vector<particle<float>, std::allocator<particle<float> > > >, particle<float>&&)+0xc7>
+	lea    0x9e49(%rip),%rdi        
 	call   30d0 <std::__throw_length_error(char const*)@plt>
 
-000000000000e550 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
+000000000000e510 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
 void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]:
 	lea    -0x1(%rdx),%rax
 	push   %rbp
 	mov    %rdx,%rbp
 	mov    %rsi,%r8
 	mov    %rax,%r11
 	push   %rbx
 	mov    %rcx,%r9
 	mov    %rdx,%rbx
 	shr    $0x3f,%r11
 	and    $0x1,%ebp
 	add    %rax,%r11
 	sar    %r11
 	cmp    %r11,%rsi
-	jl     e597 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x47>
-	jmp    e620 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xd0>
+	jl     e557 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x47>
+	jmp    e5e0 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xd0>
 	nopl   0x0(%rax)
 	sub    $0x1,%rax
 	lea    (%rdi,%rax,8),%rcx
 	mov    (%rcx),%rdx
 	mov    %rdx,(%rdi,%rsi,8)
 	cmp    %r11,%rax
-	jge    e5ba <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6a>
+	jge    e57a <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6a>
 	mov    %rax,%rsi
 	lea    0x1(%rsi),%rdx
 	lea    (%rdx,%rdx,1),%rax
 	shl    $0x4,%rdx
 	lea    (%rdi,%rdx,1),%rcx
 	mov    (%rcx),%r10
 	cmp    -0x8(%rdi,%rdx,1),%r10
-	jl     e580 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x30>
+	jl     e540 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x30>
 	mov    %r10,(%rdi,%rsi,8)
 	cmp    %r11,%rax
-	jl     e594 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x44>
+	jl     e554 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x44>
 	test   %rbp,%rbp
-	je     e630 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe0>
+	je     e5f0 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe0>
 	lea    -0x1(%rax),%rdx
 	mov    %rdx,%rsi
 	shr    $0x3f,%rsi
 	add    %rdx,%rsi
 	sar    %rsi
 	cmp    %r8,%rax
-	jg     e602 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb2>
-	jmp    e612 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc2>
+	jg     e5c2 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb2>
+	jmp    e5d2 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc2>
 	nopw   0x0(%rax,%rax,1)
 	mov    %rdx,(%rcx)
 	lea    -0x1(%rsi),%rdx
 	mov    %rdx,%rax
 	shr    $0x3f,%rax
 	add    %rdx,%rax
 	sar    %rax
 	mov    %rax,%rdx
 	mov    %rsi,%rax
 	cmp    %rsi,%r8
-	jge    e668 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x118>
+	jge    e628 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x118>
 	mov    %rdx,%rsi
 	lea    (%rdi,%rsi,8),%r10
 	lea    (%rdi,%rax,8),%rcx
 	mov    (%r10),%rdx
 	cmp    %r9,%rdx
-	jl     e5e0 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x90>
+	jl     e5a0 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x90>
 	mov    %r9,(%rcx)
 	pop    %rbx
 	pop    %rbp
 	ret
 	nopl   0x0(%rax,%rax,1)
 	lea    (%rdi,%rsi,8),%rcx
 	test   %rbp,%rbp
-	jne    e612 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc2>
+	jne    e5d2 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc2>
 	mov    %r8,%rax
 	nopl   0x0(%rax)
 	lea    -0x2(%rbx),%rdx
 	mov    %rdx,%rbx
 	shr    $0x3f,%rbx
 	add    %rdx,%rbx
 	sar    %rbx
 	cmp    %rbx,%rax
-	jne    e5bf <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6f>
+	jne    e57f <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6f>
 	lea    0x2(%rax,%rax,1),%rax
 	mov    -0x8(%rdi,%rax,8),%rdx
 	sub    $0x1,%rax
 	mov    %rdx,(%rcx)
 	lea    (%rdi,%rax,8),%rcx
-	jmp    e5bf <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6f>
+	jmp    e57f <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6f>
 	nopl   0x0(%rax)
 	mov    %r10,%rcx
 	mov    %r9,(%rcx)
 	pop    %rbx
 	pop    %rbp
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
-000000000000e680 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
+000000000000e640 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
 void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]:
 	lea    -0x1(%rdx),%rax
 	push   %rbp
 	mov    %rdx,%rbp
 	mov    %rsi,%r8
 	mov    %rax,%r11
 	push   %rbx
 	mov    %ecx,%r9d
 	mov    %rdx,%rbx
 	shr    $0x3f,%r11
 	and    $0x1,%ebp
 	add    %rax,%r11
 	sar    %r11
 	cmp    %r11,%rsi
-	jl     e6c5 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x45>
-	jmp    e740 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc0>
+	jl     e685 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x45>
+	jmp    e700 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc0>
 	nopl   0x0(%rax)
 	sub    $0x1,%rax
 	lea    (%rdi,%rax,4),%rcx
 	mov    (%rcx),%edx
 	mov    %edx,(%rdi,%rsi,4)
 	cmp    %r11,%rax
-	jge    e6e8 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x68>
+	jge    e6a8 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x68>
 	mov    %rax,%rsi
 	lea    0x1(%rsi),%rdx
 	lea    (%rdx,%rdx,1),%rax
 	shl    $0x3,%rdx
 	lea    (%rdi,%rdx,1),%rcx
 	mov    (%rcx),%r10d
 	cmp    -0x4(%rdi,%rdx,1),%r10d
-	jl     e6b0 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x30>
+	jl     e670 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x30>
 	mov    %r10d,(%rdi,%rsi,4)
 	cmp    %r11,%rax
-	jl     e6c2 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x42>
+	jl     e682 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x42>
 	test   %rbp,%rbp
-	je     e750 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xd0>
+	je     e710 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xd0>
 	lea    -0x1(%rax),%rdx
 	mov    %rdx,%rsi
 	shr    $0x3f,%rsi
 	add    %rdx,%rsi
 	sar    %rsi
 	cmp    %r8,%rax
-	jg     e729 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xa9>
-	jmp    e739 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb9>
+	jg     e6e9 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xa9>
+	jmp    e6f9 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb9>
 	nopl   (%rax)
 	mov    %edx,(%rcx)
 	lea    -0x1(%rsi),%rdx
 	mov    %rdx,%rax
 	shr    $0x3f,%rax
 	add    %rdx,%rax
 	sar    %rax
 	mov    %rax,%rdx
 	mov    %rsi,%rax
 	cmp    %rsi,%r8
-	jge    e780 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x100>
+	jge    e740 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x100>
 	mov    %rdx,%rsi
 	lea    (%rdi,%rsi,4),%r10
 	lea    (%rdi,%rax,4),%rcx
 	mov    (%r10),%edx
 	cmp    %r9d,%edx
-	jl     e708 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x88>
+	jl     e6c8 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x88>
 	mov    %r9d,(%rcx)
 	pop    %rbx
 	pop    %rbp
 	ret
 	nop
 	lea    (%rdi,%rsi,4),%rcx
 	test   %rbp,%rbp
-	jne    e739 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb9>
+	jne    e6f9 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb9>
 	mov    %r8,%rax
 	nopl   0x0(%rax)
 	lea    -0x2(%rbx),%rdx
 	mov    %rdx,%rbx
 	shr    $0x3f,%rbx
 	add    %rdx,%rbx
 	sar    %rbx
 	cmp    %rbx,%rax
-	jne    e6ed <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6d>
+	jne    e6ad <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6d>
 	lea    0x2(%rax,%rax,1),%rax
 	mov    -0x4(%rdi,%rax,4),%edx
 	sub    $0x1,%rax
 	mov    %edx,(%rcx)
 	lea    (%rdi,%rax,4),%rcx
-	jmp    e6ed <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6d>
+	jmp    e6ad <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6d>
 	xchg   %ax,%ax
 	mov    %r10,%rcx
 	mov    %r9d,(%rcx)
 	pop    %rbx
 	pop    %rbp
 	ret
 	nopl   0x0(%rax)
 
-000000000000e790 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
+000000000000e750 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
 void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]:
 	lea    -0x1(%rdx),%rax
 	mov    %rdx,%r11
 	mov    %rsi,%r8
 	mov    %rdx,%r10
 	mov    %rax,%r9
 	movaps %xmm0,%xmm1
 	and    $0x1,%r11d
 	shr    $0x3f,%r9
 	add    %rax,%r9
 	sar    %r9
 	cmp    %r9,%rsi
-	jl     e7d9 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x49>
-	jmp    e860 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xd0>
+	jl     e799 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x49>
+	jmp    e820 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xd0>
 	nopl   0x0(%rax,%rax,1)
 	sub    $0x1,%rax
 	lea    (%rdi,%rax,4),%rcx
 	movss  (%rcx),%xmm0
 	movss  %xmm0,(%rdi,%rsi,4)
 	cmp    %r9,%rax
-	jge    e7fe <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6e>
+	jge    e7be <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6e>
 	mov    %rax,%rsi
 	lea    0x1(%rsi),%rdx
 	lea    (%rdx,%rdx,1),%rax
 	shl    $0x3,%rdx
 	lea    (%rdi,%rdx,1),%rcx
 	movss  (%rcx),%xmm0
 	comiss -0x4(%rdi,%rdx,1),%xmm0
-	jb     e7c0 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x30>
+	jb     e780 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x30>
 	movss  %xmm0,(%rdi,%rsi,4)
 	cmp    %r9,%rax
-	jl     e7d6 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x46>
+	jl     e796 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x46>
 	test   %r11,%r11
-	je     e870 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe0>
+	je     e830 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe0>
 	lea    -0x1(%rax),%rdx
 	mov    %rdx,%rsi
 	shr    $0x3f,%rsi
 	add    %rdx,%rsi
 	sar    %rsi
 	cmp    %r8,%rax
-	jg     e843 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb3>
-	jmp    e855 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc5>
+	jg     e803 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb3>
+	jmp    e815 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc5>
 	nopl   0x0(%rax,%rax,1)
 	lea    -0x1(%rsi),%rdx
 	movss  %xmm0,(%rcx)
 	mov    %rdx,%rax
 	shr    $0x3f,%rax
 	add    %rdx,%rax
 	sar    %rax
 	mov    %rax,%rdx
 	mov    %rsi,%rax
 	cmp    %rsi,%r8
-	jge    e8b0 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x120>
+	jge    e870 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x120>
 	mov    %rdx,%rsi
 	lea    (%rdi,%rsi,4),%r9
 	lea    (%rdi,%rax,4),%rcx
 	movss  (%r9),%xmm0
 	comiss %xmm0,%xmm1
-	ja     e820 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x90>
+	ja     e7e0 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x90>
 	movss  %xmm1,(%rcx)
 	ret
 	nopw   0x0(%rax,%rax,1)
 	lea    (%rdi,%rsi,4),%rcx
 	test   %r11,%r11
-	jne    e855 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc5>
+	jne    e815 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc5>
 	mov    %r8,%rax
 	nopl   0x0(%rax)
 	lea    -0x2(%r10),%rdx
 	mov    %rdx,%r10
 	shr    $0x3f,%r10
 	add    %rdx,%r10
 	sar    %r10
 	cmp    %r10,%rax
-	jne    e803 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x73>
+	jne    e7c3 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x73>
 	lea    0x2(%rax,%rax,1),%rax
 	movss  -0x4(%rdi,%rax,4),%xmm0
 	sub    $0x1,%rax
 	movss  %xmm0,(%rcx)
 	lea    (%rdi,%rax,4),%rcx
-	jmp    e803 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x73>
+	jmp    e7c3 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x73>
 	cs nopw 0x0(%rax,%rax,1)
 	mov    %r9,%rcx
 	movss  %xmm1,(%rcx)
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-000000000000e8c0 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
+000000000000e880 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
 void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]:
 	lea    -0x1(%rdx),%rax
 	mov    %rdx,%r11
 	mov    %rsi,%r8
 	mov    %rdx,%r10
 	mov    %rax,%r9
 	movapd %xmm0,%xmm1
 	and    $0x1,%r11d
 	shr    $0x3f,%r9
 	add    %rax,%r9
 	sar    %r9
 	cmp    %r9,%rsi
-	jl     e909 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x49>
-	jmp    e990 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xd0>
+	jl     e8c9 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x49>
+	jmp    e950 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xd0>
 	nopl   0x0(%rax)
 	sub    $0x1,%rax
 	lea    (%rdi,%rax,8),%rcx
 	movsd  (%rcx),%xmm0
 	movsd  %xmm0,(%rdi,%rsi,8)
 	cmp    %r9,%rax
-	jge    e92f <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6f>
+	jge    e8ef <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6f>
 	mov    %rax,%rsi
 	lea    0x1(%rsi),%rdx
 	lea    (%rdx,%rdx,1),%rax
 	shl    $0x4,%rdx
 	lea    (%rdi,%rdx,1),%rcx
 	movsd  (%rcx),%xmm0
 	comisd -0x8(%rdi,%rdx,1),%xmm0
-	jb     e8f0 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x30>
+	jb     e8b0 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x30>
 	movsd  %xmm0,(%rdi,%rsi,8)
 	cmp    %r9,%rax
-	jl     e906 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x46>
+	jl     e8c6 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x46>
 	test   %r11,%r11
-	je     e9a0 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe0>
+	je     e960 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe0>
 	lea    -0x1(%rax),%rdx
 	mov    %rdx,%rsi
 	shr    $0x3f,%rsi
 	add    %rdx,%rsi
 	sar    %rsi
 	cmp    %r8,%rax
-	jg     e973 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb3>
-	jmp    e986 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc6>
+	jg     e933 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb3>
+	jmp    e946 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc6>
 	nopl   0x0(%rax)
 	lea    -0x1(%rsi),%rdx
 	movsd  %xmm0,(%rcx)
 	mov    %rdx,%rax
 	shr    $0x3f,%rax
 	add    %rdx,%rax
 	sar    %rax
 	mov    %rax,%rdx
 	mov    %rsi,%rax
 	cmp    %rsi,%r8
-	jge    e9e0 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x120>
+	jge    e9a0 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x120>
 	mov    %rdx,%rsi
 	lea    (%rdi,%rsi,8),%r9
 	lea    (%rdi,%rax,8),%rcx
 	movsd  (%r9),%xmm0
 	comisd %xmm0,%xmm1
-	ja     e950 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x90>
+	ja     e910 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x90>
 	movsd  %xmm1,(%rcx)
 	ret
 	nopl   0x0(%rax,%rax,1)
 	lea    (%rdi,%rsi,8),%rcx
 	test   %r11,%r11
-	jne    e986 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc6>
+	jne    e946 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc6>
 	mov    %r8,%rax
 	nopl   0x0(%rax)
 	lea    -0x2(%r10),%rdx
 	mov    %rdx,%r10
 	shr    $0x3f,%r10
 	add    %rdx,%r10
 	sar    %r10
 	cmp    %r10,%rax
-	jne    e934 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x74>
+	jne    e8f4 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x74>
 	lea    0x2(%rax,%rax,1),%rax
 	movsd  -0x8(%rdi,%rax,8),%xmm0
 	sub    $0x1,%rax
 	movsd  %xmm0,(%rcx)
 	lea    (%rdi,%rax,8),%rcx
-	jmp    e934 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x74>
+	jmp    e8f4 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x74>
 	cs nopw 0x0(%rax,%rax,1)
 	mov    %r9,%rcx
 	movsd  %xmm1,(%rcx)
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-000000000000e9f0 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
+000000000000e9b0 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
 void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]:
 	mov    %rsi,%rax
 	sub    %rdi,%rax
 	cmp    $0x80,%rax
-	jle    ebb2 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1c2>
+	jle    eb72 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1c2>
 	push   %r14
 	mov    %rsi,%r8
 	mov    %rdx,%r14
 	push   %r13
 	mov    %rdi,%r13
 	push   %r12
 	push   %rbp
 	lea    0x8(%rdi),%rbp
 	push   %rbx
 	test   %rdx,%rdx
-	je     eb1b <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x12b>
+	je     eadb <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x12b>
 	sar    $0x4,%rax
 	mov    0x8(%r13),%rcx
 	mov    -0x8(%r8),%rsi
 	sub    $0x1,%r14
 	lea    0x0(%r13,%rax,8),%rdi
 	mov    0x0(%r13),%rdx
 	mov    (%rdi),%rax
 	cmp    %rax,%rcx
-	jge    eadd <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xed>
+	jge    ea9d <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xed>
 	cmp    %rsi,%rax
-	jl     eb07 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x117>
+	jl     eac7 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x117>
 	cmp    %rsi,%rcx
-	jge    eb96 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1a6>
+	jge    eb56 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1a6>
 	mov    %rsi,0x0(%r13)
 	mov    %rdx,-0x8(%r8)
 	mov    0x0(%r13),%rcx
 	mov    %rbp,%rbx
 	mov    %r8,%rax
 	nopl   0x0(%rax)
 	mov    (%rbx),%rsi
 	mov    %rbx,%r12
 	cmp    %rcx,%rsi
-	jl     eaa8 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb8>
+	jl     ea68 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb8>
 	sub    $0x8,%rax
 	cmp    %rdx,%rcx
-	jge    ea95 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xa5>
+	jge    ea55 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xa5>
 	nopl   0x0(%rax)
 	mov    -0x8(%rax),%rdx
 	sub    $0x8,%rax
 	cmp    %rcx,%rdx
-	jg     ea88 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x98>
+	jg     ea48 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x98>
 	cmp    %rbx,%rax
-	jbe    eab0 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc0>
+	jbe    ea70 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc0>
 	mov    %rdx,(%rbx)
 	mov    -0x8(%rax),%rdx
 	mov    %rsi,(%rax)
 	mov    0x0(%r13),%rcx
 	add    $0x8,%rbx
-	jmp    ea70 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x80>
+	jmp    ea30 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x80>
 	xchg   %ax,%ax
 	mov    %r14,%rdx
 	mov    %r8,%rsi
 	mov    %rbx,%rdi
-	call   e9f0 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   e9b0 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	mov    %rbx,%rax
 	sub    %r13,%rax
 	cmp    $0x80,%rax
-	jle    eb8d <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x19d>
+	jle    eb4d <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x19d>
 	test   %r14,%r14
-	je     eb1e <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x12e>
+	je     eade <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x12e>
 	mov    %rbx,%r8
-	jmp    ea20 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x30>
+	jmp    e9e0 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x30>
 	cmp    %rsi,%rcx
-	jge    eafe <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x10e>
+	jge    eabe <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x10e>
 	movq   %rdx,%xmm1
 	movq   %rcx,%xmm0
 	punpcklqdq %xmm1,%xmm0
 	movups %xmm0,0x0(%r13)
 	mov    -0x8(%r8),%rdx
-	jmp    ea63 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x73>
+	jmp    ea23 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x73>
 	cmp    %rsi,%rax
-	jl     ea57 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x67>
+	jl     ea17 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x67>
 	mov    %rax,0x0(%r13)
 	mov    %rdx,(%rdi)
 	mov    0x0(%r13),%rcx
 	mov    -0x8(%r8),%rdx
-	jmp    ea63 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x73>
+	jmp    ea23 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x73>
 	mov    %rsi,%r12
 	sar    $0x3,%rax
 	mov    %r13,%rdi
 	lea    -0x2(%rax),%rbp
 	mov    %rax,%rdx
 	mov    %rax,%rbx
 	sar    %rbp
 	mov    0x0(%r13,%rbp,8),%rcx
 	mov    %rbp,%rsi
-	call   e550 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   e510 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	sub    $0x1,%rbp
 	mov    %rbx,%rdx
 	mov    %r13,%rdi
 	mov    0x0(%r13,%rbp,8),%rcx
 	mov    %rbp,%rsi
-	call   e550 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   e510 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	test   %rbp,%rbp
-	jne    eb3f <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x14f>
+	jne    eaff <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x14f>
 	nopl   0x0(%rax,%rax,1)
 	sub    $0x8,%r12
 	mov    0x0(%r13),%rax
 	mov    (%r12),%rcx
 	xor    %esi,%esi
 	mov    %r12,%rbx
 	mov    %r13,%rdi
 	sub    %r13,%rbx
 	mov    %rax,(%r12)
 	mov    %rbx,%rdx
 	sar    $0x3,%rdx
-	call   e550 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   e510 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long, long, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	cmp    $0x8,%rbx
-	jg     eb60 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x170>
+	jg     eb20 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x170>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	movq   %rdx,%xmm2
 	movq   %rcx,%xmm0
 	punpcklqdq %xmm2,%xmm0
 	movups %xmm0,0x0(%r13)
 	mov    -0x8(%r8),%rdx
-	jmp    ea63 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x73>
+	jmp    ea23 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x73>
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	xchg   %ax,%ax
 
-000000000000ebc0 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
+000000000000eb80 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
 void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]:
 	mov    %rsi,%rax
 	sub    %rdi,%rax
 	cmp    $0x40,%rax
-	jle    ed71 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1b1>
+	jle    ed31 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1b1>
 	push   %r14
 	mov    %rsi,%r8
 	mov    %rdx,%r14
 	push   %r13
 	mov    %rdi,%r13
 	push   %r12
 	push   %rbp
 	lea    0x4(%rdi),%rbp
 	push   %rbx
 	test   %rdx,%rdx
-	je     ecdd <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x11d>
+	je     ec9d <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x11d>
 	sar    $0x3,%rax
 	mov    0x4(%r13),%ecx
 	mov    -0x4(%r8),%esi
 	sub    $0x1,%r14
 	lea    0x0(%r13,%rax,4),%rdi
 	mov    0x0(%r13),%edx
 	mov    (%rdi),%eax
 	cmp    %eax,%ecx
-	jge    eca3 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe3>
+	jge    ec63 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe3>
 	cmp    %esi,%eax
-	jl     ecca <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x10a>
+	jl     ec8a <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x10a>
 	cmp    %esi,%ecx
-	jge    ed56 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x196>
+	jge    ed16 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x196>
 	mov    %esi,0x0(%r13)
 	mov    %edx,-0x4(%r8)
 	mov    0x0(%r13),%ecx
 	mov    %rbp,%rbx
 	mov    %r8,%rax
 	nopl   0x0(%rax,%rax,1)
 	mov    (%rbx),%esi
 	mov    %rbx,%r12
 	cmp    %ecx,%esi
-	jl     ec6b <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xab>
+	jl     ec2b <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xab>
 	sub    $0x4,%rax
 	cmp    %edx,%ecx
-	jge    ec5b <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x9b>
+	jge    ec1b <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x9b>
 	nopl   0x0(%rax)
 	mov    -0x4(%rax),%edx
 	sub    $0x4,%rax
 	cmp    %ecx,%edx
-	jg     ec50 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x90>
+	jg     ec10 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x90>
 	cmp    %rbx,%rax
-	jbe    ec78 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb8>
+	jbe    ec38 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xb8>
 	mov    %edx,(%rbx)
 	mov    -0x4(%rax),%edx
 	mov    %esi,(%rax)
 	mov    0x0(%r13),%ecx
 	add    $0x4,%rbx
-	jmp    ec38 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x78>
+	jmp    ebf8 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x78>
 	nopl   0x0(%rax)
 	mov    %r14,%rdx
 	mov    %r8,%rsi
 	mov    %rbx,%rdi
-	call   ebc0 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   eb80 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	mov    %rbx,%rax
 	sub    %r13,%rax
 	cmp    $0x40,%rax
-	jle    ed4d <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x18d>
+	jle    ed0d <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x18d>
 	test   %r14,%r14
-	je     ece0 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x120>
+	je     eca0 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x120>
 	mov    %rbx,%r8
-	jmp    ebee <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x2e>
+	jmp    ebae <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x2e>
 	cmp    %esi,%ecx
-	jge    ecc2 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x102>
+	jge    ec82 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x102>
 	movd   %edx,%xmm1
 	movd   %ecx,%xmm0
 	punpckldq %xmm1,%xmm0
 	movq   %xmm0,0x0(%r13)
 	mov    -0x4(%r8),%edx
-	jmp    ec2d <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6d>
+	jmp    ebed <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6d>
 	cmp    %esi,%eax
-	jl     ec21 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x61>
+	jl     ebe1 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x61>
 	mov    %eax,0x0(%r13)
 	mov    %edx,(%rdi)
 	mov    0x0(%r13),%ecx
 	mov    -0x4(%r8),%edx
-	jmp    ec2d <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6d>
+	jmp    ebed <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6d>
 	mov    %rsi,%r12
 	sar    $0x2,%rax
 	mov    %r13,%rdi
 	lea    -0x2(%rax),%rbp
 	mov    %rax,%rdx
 	mov    %rax,%rbx
 	sar    %rbp
 	mov    0x0(%r13,%rbp,4),%ecx
 	mov    %rbp,%rsi
-	call   e680 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   e640 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	sub    $0x1,%rbp
 	mov    %rbx,%rdx
 	mov    %r13,%rdi
 	mov    0x0(%r13,%rbp,4),%ecx
 	mov    %rbp,%rsi
-	call   e680 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   e640 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	test   %rbp,%rbp
-	jne    ed01 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x141>
+	jne    ecc1 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x141>
 	nopl   (%rax)
 	sub    $0x4,%r12
 	mov    0x0(%r13),%eax
 	mov    (%r12),%ecx
 	xor    %esi,%esi
 	mov    %r12,%rbx
 	mov    %r13,%rdi
 	sub    %r13,%rbx
 	mov    %eax,(%r12)
 	mov    %rbx,%rdx
 	sar    $0x2,%rdx
-	call   e680 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   e640 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_less_iter>(int*, long, long, int, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	cmp    $0x4,%rbx
-	jg     ed20 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x160>
+	jg     ece0 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x160>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	movd   %edx,%xmm2
 	movd   %ecx,%xmm0
 	punpckldq %xmm2,%xmm0
 	movq   %xmm0,0x0(%r13)
 	mov    -0x4(%r8),%edx
-	jmp    ec2d <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6d>
+	jmp    ebed <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x6d>
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-000000000000ed80 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
+000000000000ed40 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
 void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]:
 	mov    %rsi,%rax
 	sub    %rdi,%rax
 	cmp    $0x40,%rax
-	jle    ef2a <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1aa>
+	jle    eeea <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1aa>
 	push   %r14
 	mov    %rdx,%r14
 	push   %r13
 	lea    0x4(%rdi),%r13
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	push   %rbx
 	test   %rdx,%rdx
-	je     eeaa <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x12a>
+	je     ee6a <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x12a>
 	sar    $0x3,%rax
 	movss  0x4(%r12),%xmm1
 	sub    $0x1,%r14
 	movss  -0x4(%rsi),%xmm3
 	lea    (%r12,%rax,4),%rax
 	movss  (%r12),%xmm0
 	movss  (%rax),%xmm2
 	comiss %xmm1,%xmm2
-	jbe    ee44 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc4>
+	jbe    ee04 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc4>
 	comiss %xmm2,%xmm3
-	ja     ee90 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x110>
+	ja     ee50 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x110>
 	comiss %xmm1,%xmm3
-	ja     ee4e <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xce>
+	ja     ee0e <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xce>
 	movss  %xmm1,(%r12)
 	movss  %xmm0,0x4(%r12)
 	movss  -0x4(%rsi),%xmm0
 	mov    %r13,%rbx
 	mov    %rsi,%rax
 	nopl   0x0(%rax,%rax,1)
 	movss  (%rbx),%xmm2
 	mov    %rbx,%rbp
 	comiss %xmm2,%xmm1
-	ja     ee3e <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xbe>
+	ja     edfe <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xbe>
 	sub    $0x4,%rax
 	comiss %xmm1,%xmm0
-	jbe    ee26 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xa6>
+	jbe    ede6 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xa6>
 	nopl   (%rax)
 	movss  -0x4(%rax),%xmm0
 	sub    $0x4,%rax
 	comiss %xmm1,%xmm0
-	ja     ee18 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x98>
+	ja     edd8 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x98>
 	cmp    %rbx,%rax
-	jbe    ee68 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe8>
+	jbe    ee28 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xe8>
 	movss  %xmm0,(%rbx)
 	movss  -0x4(%rax),%xmm0
 	movss  %xmm2,(%rax)
 	movss  (%r12),%xmm1
 	add    $0x4,%rbx
-	jmp    ee00 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x80>
+	jmp    edc0 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x80>
 	comiss %xmm1,%xmm3
-	ja     ede0 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x60>
+	ja     eda0 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x60>
 	comiss %xmm2,%xmm3
-	jbe    ee90 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x110>
+	jbe    ee50 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x110>
 	movss  %xmm3,(%r12)
 	movss  %xmm0,-0x4(%rsi)
 	movss  (%r12),%xmm1
-	jmp    edf2 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x72>
+	jmp    edb2 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x72>
 	nopl   0x0(%rax)
 	mov    %r14,%rdx
 	mov    %rbx,%rdi
-	call   ed80 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   ed40 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	mov    %rbx,%rax
 	sub    %r12,%rax
 	cmp    $0x40,%rax
-	jle    ef21 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1a1>
+	jle    eee1 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1a1>
 	test   %r14,%r14
-	je     eead <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x12d>
+	je     ee6d <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x12d>
 	mov    %rbx,%rsi
-	jmp    edab <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x2b>
+	jmp    ed6b <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x2b>
 	movss  %xmm2,(%r12)
 	movss  %xmm0,(%rax)
 	movss  (%r12),%xmm1
 	movss  -0x4(%rsi),%xmm0
-	jmp    edf2 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x72>
+	jmp    edb2 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x72>
 	mov    %rsi,%rbp
 	sar    $0x2,%rax
 	mov    %r12,%rdi
 	lea    -0x2(%rax),%r13
 	mov    %rax,%rdx
 	mov    %rax,%rbx
 	sar    %r13
 	movss  (%r12,%r13,4),%xmm0
 	mov    %r13,%rsi
-	call   e790 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   e750 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	sub    $0x1,%r13
 	mov    %rbx,%rdx
 	mov    %r12,%rdi
 	movss  (%r12,%r13,4),%xmm0
 	mov    %r13,%rsi
-	call   e790 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   e750 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	test   %r13,%r13
-	jne    eecf <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x14f>
+	jne    ee8f <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x14f>
 	nopl   0x0(%rax)
 	sub    $0x4,%rbp
 	movss  (%r12),%xmm1
 	xor    %esi,%esi
 	mov    %r12,%rdi
 	mov    %rbp,%rbx
 	movss  0x0(%rbp),%xmm0
 	sub    %r12,%rbx
 	movss  %xmm1,0x0(%rbp)
 	mov    %rbx,%rdx
 	sar    $0x2,%rdx
-	call   e790 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   e750 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_less_iter>(float*, long, long, float, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	cmp    $0x4,%rbx
-	jg     eef0 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x170>
+	jg     eeb0 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x170>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-000000000000ef30 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
+000000000000eef0 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>:
 void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]:
 	mov    %rsi,%rax
 	sub    %rdi,%rax
 	cmp    $0x80,%rax
-	jle    f0ea <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1ba>
+	jle    f0aa <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1ba>
 	push   %r14
 	mov    %rdx,%r14
 	push   %r13
 	lea    0x8(%rdi),%r13
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	push   %rbx
 	test   %rdx,%rdx
-	je     f064 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x134>
+	je     f024 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x134>
 	sar    $0x4,%rax
 	movsd  0x8(%r12),%xmm1
 	sub    $0x1,%r14
 	movsd  -0x8(%rsi),%xmm3
 	lea    (%r12,%rax,8),%rax
 	movsd  (%r12),%xmm0
 	movsd  (%rax),%xmm2
 	comisd %xmm1,%xmm2
-	jbe    effd <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xcd>
+	jbe    efbd <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xcd>
 	comisd %xmm2,%xmm3
-	ja     f04a <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x11a>
+	ja     f00a <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x11a>
 	comisd %xmm1,%xmm3
-	ja     f009 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xd9>
+	ja     efc9 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xd9>
 	movapd %xmm1,%xmm2
 	unpcklpd %xmm0,%xmm2
 	movups %xmm2,(%r12)
 	movsd  -0x8(%rsi),%xmm0
 	mov    %r13,%rbx
 	mov    %rsi,%rax
 	nopl   (%rax)
 	movsd  (%rbx),%xmm2
 	mov    %rbx,%rbp
 	comisd %xmm2,%xmm1
-	ja     eff7 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc7>
+	ja     efb7 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xc7>
 	sub    $0x8,%rax
 	comisd %xmm1,%xmm0
-	jbe    efdf <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xaf>
+	jbe    ef9f <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xaf>
 	nopw   0x0(%rax,%rax,1)
 	movsd  -0x8(%rax),%xmm0
 	sub    $0x8,%rax
 	comisd %xmm1,%xmm0
-	ja     efd0 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xa0>
+	ja     ef90 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xa0>
 	cmp    %rbx,%rax
-	jbe    f020 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xf0>
+	jbe    efe0 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0xf0>
 	movsd  %xmm0,(%rbx)
 	movsd  -0x8(%rax),%xmm0
 	movsd  %xmm2,(%rax)
 	movsd  (%r12),%xmm1
 	add    $0x8,%rbx
-	jmp    efb0 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x80>
+	jmp    ef70 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x80>
 	comisd %xmm1,%xmm3
-	ja     ef95 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x65>
+	ja     ef55 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x65>
 	comisd %xmm2,%xmm3
-	jbe    f04a <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x11a>
+	jbe    f00a <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x11a>
 	movsd  %xmm3,(%r12)
 	movsd  %xmm0,-0x8(%rsi)
 	movsd  (%r12),%xmm1
-	jmp    efa7 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x77>
+	jmp    ef67 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x77>
 	nopl   0x0(%rax)
 	mov    %r14,%rdx
 	mov    %rbx,%rdi
-	call   ef30 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   eef0 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	mov    %rbx,%rax
 	sub    %r12,%rax
 	cmp    $0x80,%rax
-	jle    f0e1 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1b1>
+	jle    f0a1 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x1b1>
 	test   %r14,%r14
-	je     f067 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x137>
+	je     f027 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x137>
 	mov    %rbx,%rsi
-	jmp    ef5d <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x2d>
+	jmp    ef1d <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x2d>
 	movsd  %xmm2,(%r12)
 	movsd  %xmm0,(%rax)
 	movsd  (%r12),%xmm1
 	movsd  -0x8(%rsi),%xmm0
-	jmp    efa7 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x77>
+	jmp    ef67 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x77>
 	mov    %rsi,%rbp
 	sar    $0x3,%rax
 	mov    %r12,%rdi
 	lea    -0x2(%rax),%r13
 	mov    %rax,%rdx
 	mov    %rax,%rbx
 	sar    %r13
 	movsd  (%r12,%r13,8),%xmm0
 	mov    %r13,%rsi
-	call   e8c0 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   e880 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	sub    $0x1,%r13
 	mov    %rbx,%rdx
 	mov    %r12,%rdi
 	movsd  (%r12,%r13,8),%xmm0
 	mov    %r13,%rsi
-	call   e8c0 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   e880 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	test   %r13,%r13
-	jne    f089 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x159>
+	jne    f049 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x159>
 	cs nopw 0x0(%rax,%rax,1)
 	sub    $0x8,%rbp
 	movsd  (%r12),%xmm1
 	xor    %esi,%esi
 	mov    %r12,%rdi
 	mov    %rbp,%rbx
 	movsd  0x0(%rbp),%xmm0
 	sub    %r12,%rbx
 	movsd  %xmm1,0x0(%rbp)
 	mov    %rbx,%rdx
 	sar    $0x3,%rdx
-	call   e8c0 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   e880 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_less_iter>(double*, long, long, double, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	cmp    $0x8,%rbx
-	jg     f0b0 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x180>
+	jg     f070 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]+0x180>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-000000000000f0f0 <where_more_than>:
+000000000000f0b0 <where_more_than>:
 where_more_than():
 	test   %esi,%esi
-	jle    f112 <where_more_than+0x22>
+	jle    f0d2 <where_more_than+0x22>
 	movslq %esi,%rsi
 	xor    %eax,%eax
 	nopl   0x0(%rax)
 	comisd (%rdi,%rax,8),%xmm0
 	setb   (%rdx,%rax,1)
 	add    $0x1,%rax
 	cmp    %rax,%rsi
-	jne    f100 <where_more_than+0x10>
+	jne    f0c0 <where_more_than+0x10>
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	xchg   %ax,%ax
 
-000000000000f120 <where_less_than>:
+000000000000f0e0 <where_less_than>:
 where_less_than():
 	test   %esi,%esi
-	jle    f142 <where_less_than+0x22>
+	jle    f102 <where_less_than+0x22>
 	movslq %esi,%rsi
 	xor    %eax,%eax
 	nopl   0x0(%rax)
 	comisd (%rdi,%rax,8),%xmm0
 	seta   (%rdx,%rax,1)
 	add    $0x1,%rax
 	cmp    %rax,%rsi
-	jne    f130 <where_less_than+0x10>
+	jne    f0f0 <where_less_than+0x10>
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	xchg   %ax,%ax
 
-000000000000f150 <where_more_less_than>:
+000000000000f110 <where_more_less_than>:
 where_more_less_than():
 	movapd %xmm0,%xmm2
 	mov    %rdx,%r8
 	test   %esi,%esi
-	jle    f182 <where_more_less_than+0x32>
+	jle    f142 <where_more_less_than+0x32>
 	movslq %esi,%rsi
 	xor    %eax,%eax
 	movsd  (%rdi,%rax,8),%xmm0
 	comisd %xmm0,%xmm1
 	seta   %dl
 	comisd %xmm2,%xmm0
 	seta   %cl
 	and    %ecx,%edx
 	mov    %dl,(%r8,%rax,1)
 	add    $0x1,%rax
 	cmp    %rax,%rsi
-	jne    f160 <where_more_less_than+0x10>
+	jne    f120 <where_more_less_than+0x10>
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	xchg   %ax,%ax
 
-000000000000f190 <where_more_thanf>:
+000000000000f150 <where_more_thanf>:
 where_more_thanf():
 	movaps %xmm0,%xmm7
 	mov    %rdx,%r8
 	test   %esi,%esi
-	jle    f3a4 <where_more_thanf+0x214>
+	jle    f364 <where_more_thanf+0x214>
 	lea    -0x1(%rsi),%eax
 	cmp    $0xe,%eax
-	jbe    f3a5 <where_more_thanf+0x215>
+	jbe    f365 <where_more_thanf+0x215>
 	mov    %esi,%ecx
-	movdqa 0x8e6c(%rip),%xmm3        
+	movdqa 0x8eac(%rip),%xmm3        
 	movaps %xmm0,%xmm4
 	mov    %rdi,%rax
 	shr    $0x4,%ecx
-	movdqa 0x920b(%rip),%xmm5        
+	movdqa 0x924b(%rip),%xmm5        
 	shufps $0x0,%xmm4,%xmm4
 	shl    $0x6,%rcx
 	add    %rdi,%rcx
 	movups (%rax),%xmm6
 	movaps %xmm4,%xmm0
 	movaps %xmm4,%xmm1
 	add    $0x40,%rax
@@ -11176,127 +11170,127 @@
 	punpcklwd %xmm6,%xmm1
 	punpckhwd %xmm6,%xmm2
 	punpcklwd %xmm2,%xmm1
 	pand   %xmm5,%xmm1
 	packuswb %xmm1,%xmm0
 	movups %xmm0,-0x10(%rdx)
 	cmp    %rcx,%rax
-	jne    f1d0 <where_more_thanf+0x40>
+	jne    f190 <where_more_thanf+0x40>
 	mov    %esi,%eax
 	and    $0xfffffff0,%eax
 	test   $0xf,%sil
-	je     f3ac <where_more_thanf+0x21c>
+	je     f36c <where_more_thanf+0x21c>
 	movslq %eax,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	setb   (%r8,%rdx,1)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%esi
-	jle    f3a4 <where_more_thanf+0x214>
+	jle    f364 <where_more_thanf+0x214>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	setb   (%r8,%rdx,1)
 	lea    0x2(%rax),%edx
 	cmp    %edx,%esi
-	jle    f3a4 <where_more_thanf+0x214>
+	jle    f364 <where_more_thanf+0x214>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	setb   (%r8,%rdx,1)
 	lea    0x3(%rax),%edx
 	cmp    %edx,%esi
-	jle    f3a4 <where_more_thanf+0x214>
+	jle    f364 <where_more_thanf+0x214>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	setb   (%r8,%rdx,1)
 	lea    0x4(%rax),%edx
 	cmp    %edx,%esi
-	jle    f3a4 <where_more_thanf+0x214>
+	jle    f364 <where_more_thanf+0x214>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	setb   (%r8,%rdx,1)
 	lea    0x5(%rax),%edx
 	cmp    %edx,%esi
-	jle    f3a4 <where_more_thanf+0x214>
+	jle    f364 <where_more_thanf+0x214>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	setb   (%r8,%rdx,1)
 	lea    0x6(%rax),%edx
 	cmp    %edx,%esi
-	jle    f3a4 <where_more_thanf+0x214>
+	jle    f364 <where_more_thanf+0x214>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	setb   (%r8,%rdx,1)
 	lea    0x7(%rax),%edx
 	cmp    %edx,%esi
-	jle    f3a4 <where_more_thanf+0x214>
+	jle    f364 <where_more_thanf+0x214>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	setb   (%r8,%rdx,1)
 	lea    0x8(%rax),%edx
 	cmp    %edx,%esi
-	jle    f3a4 <where_more_thanf+0x214>
+	jle    f364 <where_more_thanf+0x214>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	setb   (%r8,%rdx,1)
 	lea    0x9(%rax),%edx
 	cmp    %edx,%esi
-	jle    f3a4 <where_more_thanf+0x214>
+	jle    f364 <where_more_thanf+0x214>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	setb   (%r8,%rdx,1)
 	lea    0xa(%rax),%edx
 	cmp    %edx,%esi
-	jle    f3a4 <where_more_thanf+0x214>
+	jle    f364 <where_more_thanf+0x214>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	setb   (%r8,%rdx,1)
 	lea    0xb(%rax),%edx
 	cmp    %edx,%esi
-	jle    f3a4 <where_more_thanf+0x214>
+	jle    f364 <where_more_thanf+0x214>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	setb   (%r8,%rdx,1)
 	lea    0xc(%rax),%edx
 	cmp    %edx,%esi
-	jle    f3a4 <where_more_thanf+0x214>
+	jle    f364 <where_more_thanf+0x214>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	setb   (%r8,%rdx,1)
 	lea    0xd(%rax),%edx
 	cmp    %edx,%esi
-	jle    f3a4 <where_more_thanf+0x214>
+	jle    f364 <where_more_thanf+0x214>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	setb   (%r8,%rdx,1)
 	add    $0xe,%eax
 	cmp    %eax,%esi
-	jle    f3a4 <where_more_thanf+0x214>
+	jle    f364 <where_more_thanf+0x214>
 	cltq
 	comiss (%rdi,%rax,4),%xmm7
 	setb   (%r8,%rax,1)
 	ret
 	xor    %eax,%eax
-	jmp    f273 <where_more_thanf+0xe3>
+	jmp    f233 <where_more_thanf+0xe3>
 	ret
 	nopl   (%rax)
 
-000000000000f3b0 <where_less_thanf>:
+000000000000f370 <where_less_thanf>:
 where_less_thanf():
 	movaps %xmm0,%xmm7
 	mov    %rdx,%r8
 	test   %esi,%esi
-	jle    f5b8 <where_less_thanf+0x208>
+	jle    f578 <where_less_thanf+0x208>
 	lea    -0x1(%rsi),%eax
 	cmp    $0xe,%eax
-	jbe    f5b9 <where_less_thanf+0x209>
+	jbe    f579 <where_less_thanf+0x209>
 	mov    %esi,%ecx
-	movdqa 0x8c4c(%rip),%xmm3        
+	movdqa 0x8c8c(%rip),%xmm3        
 	movaps %xmm0,%xmm4
 	mov    %rdi,%rax
 	shr    $0x4,%ecx
-	movdqa 0x8feb(%rip),%xmm5        
+	movdqa 0x902b(%rip),%xmm5        
 	shufps $0x0,%xmm4,%xmm4
 	shl    $0x6,%rcx
 	add    %rdi,%rcx
 	movups (%rax),%xmm0
 	movups 0x10(%rax),%xmm1
 	add    $0x40,%rax
 	add    $0x10,%rdx
@@ -11325,131 +11319,131 @@
 	punpckhwd %xmm6,%xmm2
 	punpcklwd %xmm6,%xmm1
 	punpcklwd %xmm2,%xmm1
 	pand   %xmm5,%xmm1
 	packuswb %xmm1,%xmm0
 	movups %xmm0,-0x10(%rdx)
 	cmp    %rcx,%rax
-	jne    f3f0 <where_less_thanf+0x40>
+	jne    f3b0 <where_less_thanf+0x40>
 	mov    %esi,%eax
 	and    $0xfffffff0,%eax
 	test   $0xf,%sil
-	je     f5c0 <where_less_thanf+0x210>
+	je     f580 <where_less_thanf+0x210>
 	movslq %eax,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	seta   (%r8,%rdx,1)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%esi
-	jle    f5b8 <where_less_thanf+0x208>
+	jle    f578 <where_less_thanf+0x208>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	seta   (%r8,%rdx,1)
 	lea    0x2(%rax),%edx
 	cmp    %edx,%esi
-	jle    f5b8 <where_less_thanf+0x208>
+	jle    f578 <where_less_thanf+0x208>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	seta   (%r8,%rdx,1)
 	lea    0x3(%rax),%edx
 	cmp    %edx,%esi
-	jle    f5b8 <where_less_thanf+0x208>
+	jle    f578 <where_less_thanf+0x208>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	seta   (%r8,%rdx,1)
 	lea    0x4(%rax),%edx
 	cmp    %edx,%esi
-	jle    f5b8 <where_less_thanf+0x208>
+	jle    f578 <where_less_thanf+0x208>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	seta   (%r8,%rdx,1)
 	lea    0x5(%rax),%edx
 	cmp    %edx,%esi
-	jle    f5b8 <where_less_thanf+0x208>
+	jle    f578 <where_less_thanf+0x208>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	seta   (%r8,%rdx,1)
 	lea    0x6(%rax),%edx
 	cmp    %edx,%esi
-	jle    f5b8 <where_less_thanf+0x208>
+	jle    f578 <where_less_thanf+0x208>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	seta   (%r8,%rdx,1)
 	lea    0x7(%rax),%edx
 	cmp    %edx,%esi
-	jle    f5b8 <where_less_thanf+0x208>
+	jle    f578 <where_less_thanf+0x208>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	seta   (%r8,%rdx,1)
 	lea    0x8(%rax),%edx
 	cmp    %edx,%esi
-	jle    f5b8 <where_less_thanf+0x208>
+	jle    f578 <where_less_thanf+0x208>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	seta   (%r8,%rdx,1)
 	lea    0x9(%rax),%edx
 	cmp    %edx,%esi
-	jle    f5b8 <where_less_thanf+0x208>
+	jle    f578 <where_less_thanf+0x208>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	seta   (%r8,%rdx,1)
 	lea    0xa(%rax),%edx
 	cmp    %edx,%esi
-	jle    f5b8 <where_less_thanf+0x208>
+	jle    f578 <where_less_thanf+0x208>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	seta   (%r8,%rdx,1)
 	lea    0xb(%rax),%edx
 	cmp    %edx,%esi
-	jle    f5b8 <where_less_thanf+0x208>
+	jle    f578 <where_less_thanf+0x208>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	seta   (%r8,%rdx,1)
 	lea    0xc(%rax),%edx
 	cmp    %edx,%esi
-	jle    f5b8 <where_less_thanf+0x208>
+	jle    f578 <where_less_thanf+0x208>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	seta   (%r8,%rdx,1)
 	lea    0xd(%rax),%edx
 	cmp    %edx,%esi
-	jle    f5b8 <where_less_thanf+0x208>
+	jle    f578 <where_less_thanf+0x208>
 	movslq %edx,%rdx
 	comiss (%rdi,%rdx,4),%xmm7
 	seta   (%r8,%rdx,1)
 	add    $0xe,%eax
 	cmp    %eax,%esi
-	jle    f5b8 <where_less_thanf+0x208>
+	jle    f578 <where_less_thanf+0x208>
 	cltq
 	comiss (%rdi,%rax,4),%xmm7
 	seta   (%r8,%rax,1)
 	ret
 	xor    %eax,%eax
-	jmp    f487 <where_less_thanf+0xd7>
+	jmp    f447 <where_less_thanf+0xd7>
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
-000000000000f5d0 <where_more_less_thanf>:
+000000000000f590 <where_more_less_thanf>:
 where_more_less_thanf():
 	movaps %xmm0,%xmm7
 	mov    %rdx,%r8
 	test   %esi,%esi
-	jle    f930 <where_more_less_thanf+0x360>
+	jle    f8f0 <where_more_less_thanf+0x360>
 	lea    -0x1(%rsi),%eax
 	cmp    $0xe,%eax
-	jbe    f931 <where_more_less_thanf+0x361>
+	jbe    f8f1 <where_more_less_thanf+0x361>
 	mov    %esi,%ecx
-	movdqa 0x8a2c(%rip),%xmm4        
+	movdqa 0x8a6c(%rip),%xmm4        
 	movaps %xmm1,%xmm6
 	movaps %xmm0,%xmm5
 	shr    $0x4,%ecx
 	mov    %rdi,%rax
 	shufps $0x0,%xmm6,%xmm6
 	shufps $0x0,%xmm5,%xmm5
-	movdqa 0x8dbf(%rip),%xmm8        
+	movdqa 0x8dff(%rip),%xmm8        
 	shl    $0x6,%rcx
 	add    %rdi,%rcx
 	nopl   0x0(%rax,%rax,1)
 	movups (%rax),%xmm3
 	movups (%rax),%xmm2
 	movaps %xmm5,%xmm0
 	add    $0x40,%rax
@@ -11494,223 +11488,223 @@
 	punpcklwd %xmm9,%xmm2
 	punpckhwd %xmm9,%xmm3
 	punpcklwd %xmm3,%xmm2
 	pand   %xmm8,%xmm2
 	packuswb %xmm2,%xmm0
 	movups %xmm0,-0x10(%rdx)
 	cmp    %rcx,%rax
-	jne    f620 <where_more_less_thanf+0x50>
+	jne    f5e0 <where_more_less_thanf+0x50>
 	mov    %esi,%eax
 	and    $0xfffffff0,%eax
 	test   $0xf,%sil
-	je     f938 <where_more_less_thanf+0x368>
+	je     f8f8 <where_more_less_thanf+0x368>
 	movslq %eax,%rcx
 	movss  (%rdi,%rcx,4),%xmm0
 	comiss %xmm0,%xmm1
 	seta   %dl
 	comiss %xmm7,%xmm0
 	seta   %r9b
 	and    %r9d,%edx
 	mov    %dl,(%r8,%rcx,1)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%esi
-	jle    f930 <where_more_less_thanf+0x360>
+	jle    f8f0 <where_more_less_thanf+0x360>
 	movslq %edx,%rdx
 	movss  (%rdi,%rdx,4),%xmm0
 	comiss %xmm0,%xmm1
 	seta   %cl
 	comiss %xmm7,%xmm0
 	seta   %r9b
 	and    %r9d,%ecx
 	mov    %cl,(%r8,%rdx,1)
 	lea    0x2(%rax),%edx
 	cmp    %edx,%esi
-	jle    f930 <where_more_less_thanf+0x360>
+	jle    f8f0 <where_more_less_thanf+0x360>
 	movslq %edx,%rdx
 	movss  (%rdi,%rdx,4),%xmm0
 	comiss %xmm0,%xmm1
 	seta   %cl
 	comiss %xmm7,%xmm0
 	seta   %r9b
 	and    %r9d,%ecx
 	mov    %cl,(%r8,%rdx,1)
 	lea    0x3(%rax),%edx
 	cmp    %edx,%esi
-	jle    f930 <where_more_less_thanf+0x360>
+	jle    f8f0 <where_more_less_thanf+0x360>
 	movslq %edx,%rdx
 	movss  (%rdi,%rdx,4),%xmm0
 	comiss %xmm0,%xmm1
 	seta   %cl
 	comiss %xmm7,%xmm0
 	seta   %r9b
 	and    %r9d,%ecx
 	mov    %cl,(%r8,%rdx,1)
 	lea    0x4(%rax),%edx
 	cmp    %edx,%esi
-	jle    f930 <where_more_less_thanf+0x360>
+	jle    f8f0 <where_more_less_thanf+0x360>
 	movslq %edx,%rdx
 	movss  (%rdi,%rdx,4),%xmm0
 	comiss %xmm0,%xmm1
 	seta   %cl
 	comiss %xmm7,%xmm0
 	seta   %r9b
 	and    %r9d,%ecx
 	mov    %cl,(%r8,%rdx,1)
 	lea    0x5(%rax),%edx
 	cmp    %edx,%esi
-	jle    f930 <where_more_less_thanf+0x360>
+	jle    f8f0 <where_more_less_thanf+0x360>
 	movslq %edx,%rdx
 	movss  (%rdi,%rdx,4),%xmm0
 	comiss %xmm0,%xmm1
 	seta   %cl
 	comiss %xmm7,%xmm0
 	seta   %r9b
 	and    %r9d,%ecx
 	mov    %cl,(%r8,%rdx,1)
 	lea    0x6(%rax),%edx
 	cmp    %edx,%esi
-	jle    f930 <where_more_less_thanf+0x360>
+	jle    f8f0 <where_more_less_thanf+0x360>
 	movslq %edx,%rdx
 	movss  (%rdi,%rdx,4),%xmm0
 	comiss %xmm0,%xmm1
 	seta   %cl
 	comiss %xmm7,%xmm0
 	seta   %r9b
 	and    %r9d,%ecx
 	mov    %cl,(%r8,%rdx,1)
 	lea    0x7(%rax),%edx
 	cmp    %edx,%esi
-	jle    f930 <where_more_less_thanf+0x360>
+	jle    f8f0 <where_more_less_thanf+0x360>
 	movslq %edx,%rdx
 	movss  (%rdi,%rdx,4),%xmm0
 	comiss %xmm0,%xmm1
 	seta   %cl
 	comiss %xmm7,%xmm0
 	seta   %r9b
 	and    %r9d,%ecx
 	mov    %cl,(%r8,%rdx,1)
 	lea    0x8(%rax),%edx
 	cmp    %edx,%esi
-	jle    f930 <where_more_less_thanf+0x360>
+	jle    f8f0 <where_more_less_thanf+0x360>
 	movslq %edx,%rdx
 	movss  (%rdi,%rdx,4),%xmm0
 	comiss %xmm0,%xmm1
 	seta   %cl
 	comiss %xmm7,%xmm0
 	seta   %r9b
 	and    %r9d,%ecx
 	mov    %cl,(%r8,%rdx,1)
 	lea    0x9(%rax),%edx
 	cmp    %edx,%esi
-	jle    f930 <where_more_less_thanf+0x360>
+	jle    f8f0 <where_more_less_thanf+0x360>
 	movslq %edx,%rdx
 	movss  (%rdi,%rdx,4),%xmm0
 	comiss %xmm0,%xmm1
 	seta   %cl
 	comiss %xmm7,%xmm0
 	seta   %r9b
 	and    %r9d,%ecx
 	mov    %cl,(%r8,%rdx,1)
 	lea    0xa(%rax),%edx
 	cmp    %edx,%esi
-	jle    f930 <where_more_less_thanf+0x360>
+	jle    f8f0 <where_more_less_thanf+0x360>
 	movslq %edx,%rdx
 	movss  (%rdi,%rdx,4),%xmm0
 	comiss %xmm0,%xmm1
 	seta   %cl
 	comiss %xmm7,%xmm0
 	seta   %r9b
 	and    %r9d,%ecx
 	mov    %cl,(%r8,%rdx,1)
 	lea    0xb(%rax),%edx
 	cmp    %edx,%esi
-	jle    f930 <where_more_less_thanf+0x360>
+	jle    f8f0 <where_more_less_thanf+0x360>
 	movslq %edx,%rdx
 	movss  (%rdi,%rdx,4),%xmm0
 	comiss %xmm0,%xmm1
 	seta   %cl
 	comiss %xmm7,%xmm0
 	seta   %r9b
 	and    %r9d,%ecx
 	mov    %cl,(%r8,%rdx,1)
 	lea    0xc(%rax),%edx
 	cmp    %edx,%esi
-	jle    f930 <where_more_less_thanf+0x360>
+	jle    f8f0 <where_more_less_thanf+0x360>
 	movslq %edx,%rdx
 	movss  (%rdi,%rdx,4),%xmm0
 	comiss %xmm0,%xmm1
 	seta   %cl
 	comiss %xmm7,%xmm0
 	seta   %r9b
 	and    %r9d,%ecx
 	mov    %cl,(%r8,%rdx,1)
 	lea    0xd(%rax),%edx
 	cmp    %edx,%esi
-	jle    f930 <where_more_less_thanf+0x360>
+	jle    f8f0 <where_more_less_thanf+0x360>
 	movslq %edx,%rdx
 	movss  (%rdi,%rdx,4),%xmm0
 	comiss %xmm0,%xmm1
 	seta   %cl
 	comiss %xmm7,%xmm0
 	seta   %r9b
 	add    $0xe,%eax
 	and    %r9d,%ecx
 	mov    %cl,(%r8,%rdx,1)
 	cmp    %eax,%esi
-	jle    f930 <where_more_less_thanf+0x360>
+	jle    f8f0 <where_more_less_thanf+0x360>
 	cltq
 	movss  (%rdi,%rax,4),%xmm0
 	comiss %xmm7,%xmm0
 	seta   %dl
 	comiss %xmm0,%xmm1
 	seta   %cl
 	and    %ecx,%edx
 	mov    %dl,(%r8,%rax,1)
 	ret
 	xor    %eax,%eax
-	jmp    f701 <where_more_less_thanf+0x131>
+	jmp    f6c1 <where_more_less_thanf+0x131>
 	ret
 	nopl   0x0(%rax)
 
-000000000000f940 <where>:
+000000000000f900 <where>:
 where():
 	movapd %xmm0,%xmm2
 	test   %esi,%esi
-	jle    f980 <where+0x40>
+	jle    f940 <where+0x40>
 	lea    -0x1(%rsi),%eax
 	xor    %r8d,%r8d
 	lea    0x8(%rdi,%rax,8),%rcx
 	nopl   0x0(%rax,%rax,1)
 	movsd  (%rdi),%xmm0
 	comisd %xmm2,%xmm0
 	seta   %dl
 	xor    %eax,%eax
 	comisd %xmm0,%xmm1
 	seta   %al
 	add    $0x8,%rdi
 	and    %edx,%eax
 	add    %eax,%r8d
 	cmp    %rdi,%rcx
-	jne    f958 <where+0x18>
+	jne    f918 <where+0x18>
 	mov    %r8d,%eax
 	ret
 	xchg   %ax,%ax
 	xor    %r8d,%r8d
 	mov    %r8d,%eax
 	ret
 	nopw   0x0(%rax,%rax,1)
 
-000000000000f990 <wheref>:
+000000000000f950 <wheref>:
 wheref():
 	movaps %xmm0,%xmm4
 	test   %esi,%esi
-	jle    fa80 <wheref+0xf0>
+	jle    fa40 <wheref+0xf0>
 	lea    -0x1(%rsi),%eax
 	cmp    $0x2,%eax
-	jbe    fa89 <wheref+0xf9>
+	jbe    fa49 <wheref+0xf9>
 	mov    %esi,%edx
 	movaps %xmm0,%xmm6
 	movaps %xmm1,%xmm5
 	mov    %rdi,%rax
 	shr    $0x2,%edx
 	pxor   %xmm2,%xmm2
 	shufps $0x0,%xmm6,%xmm6
@@ -11723,50 +11717,50 @@
 	add    $0x10,%rax
 	movaps %xmm7,%xmm0
 	cmpltps %xmm7,%xmm3
 	cmpltps %xmm5,%xmm0
 	pand   %xmm3,%xmm0
 	psubd  %xmm0,%xmm2
 	cmp    %rdx,%rax
-	jne    f9d0 <wheref+0x40>
+	jne    f990 <wheref+0x40>
 	movdqa %xmm2,%xmm0
 	mov    %esi,%edx
 	psrldq $0x8,%xmm0
 	and    $0xfffffffc,%edx
 	paddd  %xmm0,%xmm2
 	movdqa %xmm2,%xmm0
 	psrldq $0x4,%xmm0
 	paddd  %xmm0,%xmm2
 	movd   %xmm2,%eax
 	test   $0x3,%sil
-	je     fa88 <wheref+0xf8>
+	je     fa48 <wheref+0xf8>
 	movslq %edx,%rcx
 	movss  (%rdi,%rcx,4),%xmm0
 	comiss %xmm4,%xmm0
 	seta   %r8b
 	xor    %ecx,%ecx
 	comiss %xmm0,%xmm1
 	seta   %cl
 	and    %r8d,%ecx
 	add    %ecx,%eax
 	lea    0x1(%rdx),%ecx
 	cmp    %ecx,%esi
-	jle    fa82 <wheref+0xf2>
+	jle    fa42 <wheref+0xf2>
 	movslq %ecx,%rcx
 	movss  (%rdi,%rcx,4),%xmm0
 	comiss %xmm4,%xmm0
 	seta   %r8b
 	xor    %ecx,%ecx
 	comiss %xmm0,%xmm1
 	seta   %cl
 	add    $0x2,%edx
 	and    %r8d,%ecx
 	add    %ecx,%eax
 	cmp    %edx,%esi
-	jle    fa82 <wheref+0xf2>
+	jle    fa42 <wheref+0xf2>
 	movslq %edx,%rdx
 	movss  (%rdi,%rdx,4),%xmm0
 	comiss %xmm0,%xmm1
 	seta   %cl
 	xor    %edx,%edx
 	comiss %xmm4,%xmm0
 	seta   %dl
@@ -11776,594 +11770,594 @@
 	nopl   0x0(%rax)
 	xor    %eax,%eax
 	ret
 	nopl   0x0(%rax,%rax,1)
 	ret
 	xor    %edx,%edx
 	xor    %eax,%eax
-	jmp    fa1b <wheref+0x8b>
+	jmp    f9db <wheref+0x8b>
 	nop
 
-000000000000fa90 <add_int_vector>:
+000000000000fa50 <add_int_vector>:
 add_int_vector():
 	mov    %edx,%r8d
 	test   %edx,%edx
-	jle    fb10 <add_int_vector+0x80>
+	jle    fad0 <add_int_vector+0x80>
 	lea    -0x1(%rdx),%eax
 	cmp    $0x2,%eax
-	jbe    fb19 <add_int_vector+0x89>
+	jbe    fad9 <add_int_vector+0x89>
 	shr    $0x2,%edx
 	xor    %eax,%eax
 	shl    $0x4,%rdx
 	nopl   0x0(%rax,%rax,1)
 	movdqu (%rdi,%rax,1),%xmm0
 	movdqu (%rsi,%rax,1),%xmm1
 	paddd  %xmm1,%xmm0
 	movups %xmm0,(%rcx,%rax,1)
 	add    $0x10,%rax
 	cmp    %rdx,%rax
-	jne    fab0 <add_int_vector+0x20>
+	jne    fa70 <add_int_vector+0x20>
 	mov    %r8d,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%r8b
-	je     fb18 <add_int_vector+0x88>
+	je     fad8 <add_int_vector+0x88>
 	movslq %eax,%rdx
 	mov    (%rsi,%rdx,4),%r9d
 	add    (%rdi,%rdx,4),%r9d
 	mov    %r9d,(%rcx,%rdx,4)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%r8d
-	jle    fb10 <add_int_vector+0x80>
+	jle    fad0 <add_int_vector+0x80>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	mov    (%rsi,%rdx,4),%r9d
 	add    (%rdi,%rdx,4),%r9d
 	mov    %r9d,(%rcx,%rdx,4)
 	cmp    %eax,%r8d
-	jle    fb10 <add_int_vector+0x80>
+	jle    fad0 <add_int_vector+0x80>
 	cltq
 	mov    (%rdi,%rax,4),%edx
 	add    (%rsi,%rax,4),%edx
 	mov    %edx,(%rcx,%rax,4)
 	ret
 	nopl   0x0(%rax)
 	ret
 	xor    %eax,%eax
-	jmp    fad7 <add_int_vector+0x47>
+	jmp    fa97 <add_int_vector+0x47>
 	nopl   (%rax)
 
-000000000000fb20 <add_uint16_vector>:
+000000000000fae0 <add_uint16_vector>:
 add_uint16_vector():
 	test   %edx,%edx
-	jle    fbe9 <add_uint16_vector+0xc9>
+	jle    fba9 <add_uint16_vector+0xc9>
 	lea    -0x1(%rdx),%r9d
 	cmp    $0x6,%r9d
-	jbe    fbf1 <add_uint16_vector+0xd1>
+	jbe    fbb1 <add_uint16_vector+0xd1>
 	mov    %edx,%r8d
 	xor    %eax,%eax
 	shr    $0x3,%r8d
 	shl    $0x4,%r8
 	nopl   0x0(%rax,%rax,1)
 	movdqu (%rdi,%rax,1),%xmm0
 	movdqu (%rsi,%rax,1),%xmm2
 	paddw  %xmm2,%xmm0
 	movups %xmm0,(%rcx,%rax,1)
 	add    $0x10,%rax
 	cmp    %r8,%rax
-	jne    fb48 <add_uint16_vector+0x28>
+	jne    fb08 <add_uint16_vector+0x28>
 	mov    %edx,%eax
 	and    $0xfffffff8,%eax
 	mov    %eax,%r8d
 	cmp    %eax,%edx
-	je     fbf0 <add_uint16_vector+0xd0>
+	je     fbb0 <add_uint16_vector+0xd0>
 	mov    %edx,%r10d
 	sub    %eax,%r9d
 	sub    %eax,%r10d
 	cmp    $0x2,%r9d
-	jbe    fba3 <add_uint16_vector+0x83>
+	jbe    fb63 <add_uint16_vector+0x83>
 	movq   (%rdi,%rax,2),%xmm0
 	movq   (%rsi,%rax,2),%xmm1
 	paddw  %xmm1,%xmm0
 	movq   %xmm0,(%rcx,%rax,2)
 	mov    %r10d,%eax
 	and    $0xfffffffc,%eax
 	add    %eax,%r8d
 	cmp    %eax,%r10d
-	je     fbe9 <add_uint16_vector+0xc9>
+	je     fba9 <add_uint16_vector+0xc9>
 	movslq %r8d,%rax
 	movzwl (%rsi,%rax,2),%r9d
 	add    (%rdi,%rax,2),%r9w
 	mov    %r9w,(%rcx,%rax,2)
 	lea    0x1(%r8),%eax
 	cmp    %eax,%edx
-	jle    fbe9 <add_uint16_vector+0xc9>
+	jle    fba9 <add_uint16_vector+0xc9>
 	cltq
 	add    $0x2,%r8d
 	movzwl (%rsi,%rax,2),%r9d
 	add    (%rdi,%rax,2),%r9w
 	mov    %r9w,(%rcx,%rax,2)
 	cmp    %r8d,%edx
-	jle    fbe9 <add_uint16_vector+0xc9>
+	jle    fba9 <add_uint16_vector+0xc9>
 	movslq %r8d,%r8
 	movzwl (%rsi,%r8,2),%eax
 	add    (%rdi,%r8,2),%ax
 	mov    %ax,(%rcx,%r8,2)
 	ret
 	nopw   0x0(%rax,%rax,1)
 	ret
 	xor    %eax,%eax
 	xor    %r8d,%r8d
-	jmp    fb73 <add_uint16_vector+0x53>
+	jmp    fb33 <add_uint16_vector+0x53>
 	nopl   0x0(%rax,%rax,1)
 
-000000000000fc00 <add_uint32_vector>:
+000000000000fbc0 <add_uint32_vector>:
 add_uint32_vector():
 	mov    %edx,%r8d
 	test   %edx,%edx
-	jle    fc80 <add_uint32_vector+0x80>
+	jle    fc40 <add_uint32_vector+0x80>
 	lea    -0x1(%rdx),%eax
 	cmp    $0x2,%eax
-	jbe    fc89 <add_uint32_vector+0x89>
+	jbe    fc49 <add_uint32_vector+0x89>
 	shr    $0x2,%edx
 	xor    %eax,%eax
 	shl    $0x4,%rdx
 	nopl   0x0(%rax,%rax,1)
 	movdqu (%rdi,%rax,1),%xmm0
 	movdqu (%rsi,%rax,1),%xmm1
 	paddd  %xmm1,%xmm0
 	movups %xmm0,(%rcx,%rax,1)
 	add    $0x10,%rax
 	cmp    %rdx,%rax
-	jne    fc20 <add_uint32_vector+0x20>
+	jne    fbe0 <add_uint32_vector+0x20>
 	mov    %r8d,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%r8b
-	je     fc88 <add_uint32_vector+0x88>
+	je     fc48 <add_uint32_vector+0x88>
 	movslq %eax,%rdx
 	mov    (%rsi,%rdx,4),%r9d
 	add    (%rdi,%rdx,4),%r9d
 	mov    %r9d,(%rcx,%rdx,4)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%r8d
-	jle    fc80 <add_uint32_vector+0x80>
+	jle    fc40 <add_uint32_vector+0x80>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	mov    (%rsi,%rdx,4),%r9d
 	add    (%rdi,%rdx,4),%r9d
 	mov    %r9d,(%rcx,%rdx,4)
 	cmp    %eax,%r8d
-	jle    fc80 <add_uint32_vector+0x80>
+	jle    fc40 <add_uint32_vector+0x80>
 	cltq
 	mov    (%rdi,%rax,4),%edx
 	add    (%rsi,%rax,4),%edx
 	mov    %edx,(%rcx,%rax,4)
 	ret
 	nopl   0x0(%rax)
 	ret
 	xor    %eax,%eax
-	jmp    fc47 <add_uint32_vector+0x47>
+	jmp    fc07 <add_uint32_vector+0x47>
 	nopl   (%rax)
 
-000000000000fc90 <add_longint_vector>:
+000000000000fc50 <add_longint_vector>:
 add_longint_vector():
 	mov    %edx,%r8d
 	test   %edx,%edx
-	jle    fcdd <add_longint_vector+0x4d>
+	jle    fc9d <add_longint_vector+0x4d>
 	cmp    $0x1,%edx
-	je     fce1 <add_longint_vector+0x51>
+	je     fca1 <add_longint_vector+0x51>
 	shr    %edx
 	xor    %eax,%eax
 	shl    $0x4,%rdx
 	nopl   0x0(%rax)
 	movdqu (%rdi,%rax,1),%xmm0
 	movdqu (%rsi,%rax,1),%xmm1
 	paddq  %xmm1,%xmm0
 	movups %xmm0,(%rcx,%rax,1)
 	add    $0x10,%rax
 	cmp    %rax,%rdx
-	jne    fca8 <add_longint_vector+0x18>
+	jne    fc68 <add_longint_vector+0x18>
 	mov    %r8d,%eax
 	and    $0xfffffffe,%eax
 	and    $0x1,%r8d
-	je     fce0 <add_longint_vector+0x50>
+	je     fca0 <add_longint_vector+0x50>
 	cltq
 	mov    (%rdi,%rax,8),%rdx
 	add    (%rsi,%rax,8),%rdx
 	mov    %rdx,(%rcx,%rax,8)
 	ret
 	xchg   %ax,%ax
 	ret
 	xor    %eax,%eax
-	jmp    fccf <add_longint_vector+0x3f>
+	jmp    fc8f <add_longint_vector+0x3f>
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-000000000000fcf0 <add_double_vector>:
+000000000000fcb0 <add_double_vector>:
 add_double_vector():
 	mov    %edx,%r8d
 	test   %edx,%edx
-	jle    fd40 <add_double_vector+0x50>
+	jle    fd00 <add_double_vector+0x50>
 	cmp    $0x1,%edx
-	je     fd49 <add_double_vector+0x59>
+	je     fd09 <add_double_vector+0x59>
 	shr    %edx
 	xor    %eax,%eax
 	shl    $0x4,%rdx
 	nopl   0x0(%rax)
 	movupd (%rdi,%rax,1),%xmm0
 	movupd (%rsi,%rax,1),%xmm1
 	addpd  %xmm1,%xmm0
 	movups %xmm0,(%rcx,%rax,1)
 	add    $0x10,%rax
 	cmp    %rax,%rdx
-	jne    fd08 <add_double_vector+0x18>
+	jne    fcc8 <add_double_vector+0x18>
 	mov    %r8d,%eax
 	and    $0xfffffffe,%eax
 	and    $0x1,%r8d
-	je     fd48 <add_double_vector+0x58>
+	je     fd08 <add_double_vector+0x58>
 	cltq
 	movsd  (%rsi,%rax,8),%xmm0
 	addsd  (%rdi,%rax,8),%xmm0
 	movsd  %xmm0,(%rcx,%rax,8)
 	ret
 	nopl   0x0(%rax)
 	ret
 	xor    %eax,%eax
-	jmp    fd2f <add_double_vector+0x3f>
+	jmp    fcef <add_double_vector+0x3f>
 	nopl   (%rax)
 
-000000000000fd50 <add_float_vector>:
+000000000000fd10 <add_float_vector>:
 add_float_vector():
 	mov    %edx,%r8d
 	test   %edx,%edx
-	jle    fdd9 <add_float_vector+0x89>
+	jle    fd99 <add_float_vector+0x89>
 	lea    -0x1(%rdx),%eax
 	cmp    $0x2,%eax
-	jbe    fde1 <add_float_vector+0x91>
+	jbe    fda1 <add_float_vector+0x91>
 	shr    $0x2,%edx
 	xor    %eax,%eax
 	shl    $0x4,%rdx
 	nopl   0x0(%rax)
 	movups (%rdi,%rax,1),%xmm0
 	movups (%rsi,%rax,1),%xmm1
 	addps  %xmm1,%xmm0
 	movups %xmm0,(%rcx,%rax,1)
 	add    $0x10,%rax
 	cmp    %rdx,%rax
-	jne    fd70 <add_float_vector+0x20>
+	jne    fd30 <add_float_vector+0x20>
 	mov    %r8d,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%r8b
-	je     fde0 <add_float_vector+0x90>
+	je     fda0 <add_float_vector+0x90>
 	movslq %eax,%rdx
 	movss  (%rdi,%rdx,4),%xmm0
 	addss  (%rsi,%rdx,4),%xmm0
 	movss  %xmm0,(%rcx,%rdx,4)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%r8d
-	jle    fdd9 <add_float_vector+0x89>
+	jle    fd99 <add_float_vector+0x89>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	movss  (%rdi,%rdx,4),%xmm0
 	addss  (%rsi,%rdx,4),%xmm0
 	movss  %xmm0,(%rcx,%rdx,4)
 	cmp    %eax,%r8d
-	jle    fdd9 <add_float_vector+0x89>
+	jle    fd99 <add_float_vector+0x89>
 	cltq
 	movss  (%rsi,%rax,4),%xmm0
 	addss  (%rdi,%rax,4),%xmm0
 	movss  %xmm0,(%rcx,%rax,4)
 	ret
 	nopw   0x0(%rax,%rax,1)
 	ret
 	xor    %eax,%eax
-	jmp    fd94 <add_float_vector+0x44>
+	jmp    fd54 <add_float_vector+0x44>
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-000000000000fdf0 <add_int_vector_inplace>:
+000000000000fdb0 <add_int_vector_inplace>:
 add_int_vector_inplace():
 	mov    %edx,%ecx
 	test   %edx,%edx
-	jle    fe61 <add_int_vector_inplace+0x71>
+	jle    fe21 <add_int_vector_inplace+0x71>
 	lea    -0x1(%rdx),%eax
 	cmp    $0x2,%eax
-	jbe    fe69 <add_int_vector_inplace+0x79>
+	jbe    fe29 <add_int_vector_inplace+0x79>
 	shr    $0x2,%edx
 	xor    %eax,%eax
 	shl    $0x4,%rdx
 	nopw   0x0(%rax,%rax,1)
 	movdqu (%rdi,%rax,1),%xmm0
 	movdqu (%rsi,%rax,1),%xmm1
 	paddd  %xmm1,%xmm0
 	movups %xmm0,(%rdi,%rax,1)
 	add    $0x10,%rax
 	cmp    %rdx,%rax
-	jne    fe10 <add_int_vector_inplace+0x20>
+	jne    fdd0 <add_int_vector_inplace+0x20>
 	mov    %ecx,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%cl
-	je     fe68 <add_int_vector_inplace+0x78>
+	je     fe28 <add_int_vector_inplace+0x78>
 	movslq %eax,%rdx
 	mov    (%rsi,%rdx,4),%r8d
 	add    %r8d,(%rdi,%rdx,4)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%ecx
-	jle    fe61 <add_int_vector_inplace+0x71>
+	jle    fe21 <add_int_vector_inplace+0x71>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	mov    (%rsi,%rdx,4),%r8d
 	add    %r8d,(%rdi,%rdx,4)
 	cmp    %eax,%ecx
-	jle    fe61 <add_int_vector_inplace+0x71>
+	jle    fe21 <add_int_vector_inplace+0x71>
 	cltq
 	mov    (%rsi,%rax,4),%edx
 	add    %edx,(%rdi,%rax,4)
 	ret
 	nopw   0x0(%rax,%rax,1)
 	ret
 	xor    %eax,%eax
-	jmp    fe35 <add_int_vector_inplace+0x45>
+	jmp    fdf5 <add_int_vector_inplace+0x45>
 	nopl   (%rax)
 
-000000000000fe70 <add_uint16_vector_inplace>:
+000000000000fe30 <add_uint16_vector_inplace>:
 add_uint16_vector_inplace():
 	test   %edx,%edx
-	jle    ff23 <add_uint16_vector_inplace+0xb3>
+	jle    fee3 <add_uint16_vector_inplace+0xb3>
 	lea    -0x1(%rdx),%r8d
 	cmp    $0x6,%r8d
-	jbe    ff29 <add_uint16_vector_inplace+0xb9>
+	jbe    fee9 <add_uint16_vector_inplace+0xb9>
 	mov    %edx,%ecx
 	xor    %eax,%eax
 	shr    $0x3,%ecx
 	shl    $0x4,%rcx
 	nopl   0x0(%rax)
 	movdqu (%rdi,%rax,1),%xmm0
 	movdqu (%rsi,%rax,1),%xmm2
 	paddw  %xmm2,%xmm0
 	movups %xmm0,(%rdi,%rax,1)
 	add    $0x10,%rax
 	cmp    %rcx,%rax
-	jne    fe98 <add_uint16_vector_inplace+0x28>
+	jne    fe58 <add_uint16_vector_inplace+0x28>
 	mov    %edx,%eax
 	and    $0xfffffff8,%eax
 	mov    %eax,%ecx
 	cmp    %eax,%edx
-	je     ff28 <add_uint16_vector_inplace+0xb8>
+	je     fee8 <add_uint16_vector_inplace+0xb8>
 	mov    %edx,%r9d
 	sub    %eax,%r8d
 	sub    %eax,%r9d
 	cmp    $0x2,%r8d
-	jbe    fef1 <add_uint16_vector_inplace+0x81>
+	jbe    feb1 <add_uint16_vector_inplace+0x81>
 	lea    (%rdi,%rax,2),%r8
 	movq   (%rsi,%rax,2),%xmm0
 	mov    %r9d,%eax
 	movq   (%r8),%xmm1
 	and    $0xfffffffc,%eax
 	add    %eax,%ecx
 	paddw  %xmm1,%xmm0
 	movq   %xmm0,(%r8)
 	cmp    %eax,%r9d
-	je     ff23 <add_uint16_vector_inplace+0xb3>
+	je     fee3 <add_uint16_vector_inplace+0xb3>
 	movslq %ecx,%rax
 	movzwl (%rsi,%rax,2),%r8d
 	add    %r8w,(%rdi,%rax,2)
 	lea    0x1(%rcx),%eax
 	cmp    %eax,%edx
-	jle    ff23 <add_uint16_vector_inplace+0xb3>
+	jle    fee3 <add_uint16_vector_inplace+0xb3>
 	cltq
 	add    $0x2,%ecx
 	movzwl (%rsi,%rax,2),%r8d
 	add    %r8w,(%rdi,%rax,2)
 	cmp    %ecx,%edx
-	jle    ff23 <add_uint16_vector_inplace+0xb3>
+	jle    fee3 <add_uint16_vector_inplace+0xb3>
 	movslq %ecx,%rcx
 	movzwl (%rsi,%rcx,2),%eax
 	add    %ax,(%rdi,%rcx,2)
 	ret
 	nopl   0x0(%rax)
 	ret
 	xor    %eax,%eax
 	xor    %ecx,%ecx
-	jmp    febe <add_uint16_vector_inplace+0x4e>
+	jmp    fe7e <add_uint16_vector_inplace+0x4e>
 	nop
 
-000000000000ff30 <add_uint32_vector_inplace>:
+000000000000fef0 <add_uint32_vector_inplace>:
 add_uint32_vector_inplace():
 	mov    %edx,%ecx
 	test   %edx,%edx
-	jle    ffa1 <add_uint32_vector_inplace+0x71>
+	jle    ff61 <add_uint32_vector_inplace+0x71>
 	lea    -0x1(%rdx),%eax
 	cmp    $0x2,%eax
-	jbe    ffa9 <add_uint32_vector_inplace+0x79>
+	jbe    ff69 <add_uint32_vector_inplace+0x79>
 	shr    $0x2,%edx
 	xor    %eax,%eax
 	shl    $0x4,%rdx
 	nopw   0x0(%rax,%rax,1)
 	movdqu (%rdi,%rax,1),%xmm0
 	movdqu (%rsi,%rax,1),%xmm1
 	paddd  %xmm1,%xmm0
 	movups %xmm0,(%rdi,%rax,1)
 	add    $0x10,%rax
 	cmp    %rdx,%rax
-	jne    ff50 <add_uint32_vector_inplace+0x20>
+	jne    ff10 <add_uint32_vector_inplace+0x20>
 	mov    %ecx,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%cl
-	je     ffa8 <add_uint32_vector_inplace+0x78>
+	je     ff68 <add_uint32_vector_inplace+0x78>
 	movslq %eax,%rdx
 	mov    (%rsi,%rdx,4),%r8d
 	add    %r8d,(%rdi,%rdx,4)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%ecx
-	jle    ffa1 <add_uint32_vector_inplace+0x71>
+	jle    ff61 <add_uint32_vector_inplace+0x71>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	mov    (%rsi,%rdx,4),%r8d
 	add    %r8d,(%rdi,%rdx,4)
 	cmp    %eax,%ecx
-	jle    ffa1 <add_uint32_vector_inplace+0x71>
+	jle    ff61 <add_uint32_vector_inplace+0x71>
 	cltq
 	mov    (%rsi,%rax,4),%edx
 	add    %edx,(%rdi,%rax,4)
 	ret
 	nopw   0x0(%rax,%rax,1)
 	ret
 	xor    %eax,%eax
-	jmp    ff75 <add_uint32_vector_inplace+0x45>
+	jmp    ff35 <add_uint32_vector_inplace+0x45>
 	nopl   (%rax)
 
-000000000000ffb0 <add_longint_vector_inplace>:
+000000000000ff70 <add_longint_vector_inplace>:
 add_longint_vector_inplace():
 	mov    %edx,%ecx
 	test   %edx,%edx
-	jle    fff7 <add_longint_vector_inplace+0x47>
+	jle    ffb7 <add_longint_vector_inplace+0x47>
 	cmp    $0x1,%edx
-	je     10001 <add_longint_vector_inplace+0x51>
+	je     ffc1 <add_longint_vector_inplace+0x51>
 	shr    %edx
 	xor    %eax,%eax
 	shl    $0x4,%rdx
 	nopl   0x0(%rax,%rax,1)
 	movdqu (%rdi,%rax,1),%xmm0
 	movdqu (%rsi,%rax,1),%xmm1
 	paddq  %xmm1,%xmm0
 	movups %xmm0,(%rdi,%rax,1)
 	add    $0x10,%rax
 	cmp    %rax,%rdx
-	jne    ffc8 <add_longint_vector_inplace+0x18>
+	jne    ff88 <add_longint_vector_inplace+0x18>
 	mov    %ecx,%eax
 	and    $0xfffffffe,%eax
 	and    $0x1,%ecx
-	je     10000 <add_longint_vector_inplace+0x50>
+	je     ffc0 <add_longint_vector_inplace+0x50>
 	cltq
 	mov    (%rsi,%rax,8),%rdx
 	add    %rdx,(%rdi,%rax,8)
 	ret
 	nopl   0x0(%rax,%rax,1)
 	ret
 	xor    %eax,%eax
-	jmp    ffed <add_longint_vector_inplace+0x3d>
+	jmp    ffad <add_longint_vector_inplace+0x3d>
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-0000000000010010 <add_double_vector_inplace>:
+000000000000ffd0 <add_double_vector_inplace>:
 add_double_vector_inplace():
 	mov    %edx,%ecx
 	test   %edx,%edx
-	jle    10060 <add_double_vector_inplace+0x50>
+	jle    10020 <add_double_vector_inplace+0x50>
 	cmp    $0x1,%edx
-	je     10069 <add_double_vector_inplace+0x59>
+	je     10029 <add_double_vector_inplace+0x59>
 	shr    %edx
 	xor    %eax,%eax
 	shl    $0x4,%rdx
 	nopl   0x0(%rax,%rax,1)
 	movupd (%rdi,%rax,1),%xmm0
 	movupd (%rsi,%rax,1),%xmm1
 	addpd  %xmm1,%xmm0
 	movups %xmm0,(%rdi,%rax,1)
 	add    $0x10,%rax
 	cmp    %rax,%rdx
-	jne    10028 <add_double_vector_inplace+0x18>
+	jne    ffe8 <add_double_vector_inplace+0x18>
 	mov    %ecx,%eax
 	and    $0xfffffffe,%eax
 	and    $0x1,%ecx
-	je     10068 <add_double_vector_inplace+0x58>
+	je     10028 <add_double_vector_inplace+0x58>
 	cltq
 	lea    (%rdi,%rax,8),%rdx
 	movsd  (%rdx),%xmm0
 	addsd  (%rsi,%rax,8),%xmm0
 	movsd  %xmm0,(%rdx)
 	ret
 	nopl   0x0(%rax)
 	ret
 	xor    %eax,%eax
-	jmp    1004d <add_double_vector_inplace+0x3d>
+	jmp    1000d <add_double_vector_inplace+0x3d>
 	nopl   (%rax)
 
-0000000000010070 <add_float_vector_inplace>:
+0000000000010030 <add_float_vector_inplace>:
 add_float_vector_inplace():
 	mov    %edx,%ecx
 	test   %edx,%edx
-	jle    100fe <add_float_vector_inplace+0x8e>
+	jle    100be <add_float_vector_inplace+0x8e>
 	lea    -0x1(%rdx),%eax
 	cmp    $0x2,%eax
-	jbe    10101 <add_float_vector_inplace+0x91>
+	jbe    100c1 <add_float_vector_inplace+0x91>
 	shr    $0x2,%edx
 	xor    %eax,%eax
 	shl    $0x4,%rdx
 	nopl   0x0(%rax,%rax,1)
 	movups (%rdi,%rax,1),%xmm0
 	movups (%rsi,%rax,1),%xmm1
 	addps  %xmm1,%xmm0
 	movups %xmm0,(%rdi,%rax,1)
 	add    $0x10,%rax
 	cmp    %rdx,%rax
-	jne    10090 <add_float_vector_inplace+0x20>
+	jne    10050 <add_float_vector_inplace+0x20>
 	mov    %ecx,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%cl
-	je     10100 <add_float_vector_inplace+0x90>
+	je     100c0 <add_float_vector_inplace+0x90>
 	movslq %eax,%r8
 	lea    (%rdi,%r8,4),%rdx
 	movss  (%rdx),%xmm0
 	addss  (%rsi,%r8,4),%xmm0
 	movss  %xmm0,(%rdx)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%ecx
-	jle    100fe <add_float_vector_inplace+0x8e>
+	jle    100be <add_float_vector_inplace+0x8e>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	lea    (%rdi,%rdx,4),%r8
 	movss  (%r8),%xmm0
 	addss  (%rsi,%rdx,4),%xmm0
 	movss  %xmm0,(%r8)
 	cmp    %eax,%ecx
-	jle    100fe <add_float_vector_inplace+0x8e>
+	jle    100be <add_float_vector_inplace+0x8e>
 	cltq
 	lea    (%rdi,%rax,4),%rdx
 	movss  (%rdx),%xmm0
 	addss  (%rsi,%rax,4),%xmm0
 	movss  %xmm0,(%rdx)
 	ret
 	nop
 	ret
 	xor    %eax,%eax
-	jmp    100b2 <add_float_vector_inplace+0x42>
+	jmp    10072 <add_float_vector_inplace+0x42>
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-0000000000010110 <convolution>:
+00000000000100d0 <convolution>:
 convolution():
 	push   %r15
 	mov    %esi,%r10d
 	push   %r14
 	push   %r13
 	push   %r12
 	movslq %ecx,%r12
 	push   %rbp
 	push   %rbx
 	lea    -0x1(%rsi,%r12,1),%ebx
 	test   %ebx,%ebx
-	jle    102ef <convolution+0x1df>
+	jle    102af <convolution+0x1df>
 	lea    -0x1(%r12),%r11d
 	mov    %rdx,%rsi
 	sub    $0x1,%r10d
 	test   %r11d,%r11d
-	jle    10300 <convolution+0x1f0>
+	jle    102c0 <convolution+0x1f0>
 	cmp    %r11d,%ebx
 	mov    %r11d,%r13d
 	lea    -0x8(%rdx),%rbp
 	mov    %r8,%r9
 	cmovle %ebx,%r13d
 	pxor   %xmm3,%xmm3
 	xor    %ecx,%ecx
 	nopl   0x0(%rax)
 	cmp    %r10d,%ecx
 	mov    %r10d,%eax
 	movq   $0x0,(%r9)
 	cmovle %ecx,%eax
 	test   %eax,%eax
-	js     101ee <convolution+0xde>
+	js     101ae <convolution+0xde>
 	lea    0x1(%rax),%r14d
-	je     10311 <convolution+0x201>
+	je     102d1 <convolution+0x201>
 	mov    %r14d,%r15d
 	mov    %rdi,%rax
 	pxor   %xmm2,%xmm2
 	mov    %rbp,%rdx
 	shr    %r15d
 	shl    $0x4,%r15
 	add    %rdi,%r15
@@ -12372,37 +12366,37 @@
 	movupd (%rax),%xmm5
 	add    $0x10,%rax
 	sub    $0x10,%rdx
 	shufpd $0x1,%xmm0,%xmm0
 	mulpd  %xmm5,%xmm0
 	addpd  %xmm0,%xmm2
 	cmp    %rax,%r15
-	jne    10198 <convolution+0x88>
+	jne    10158 <convolution+0x88>
 	mov    %r14d,%eax
 	movapd %xmm2,%xmm1
 	unpckhpd %xmm2,%xmm1
 	and    $0xfffffffe,%eax
 	and    $0x1,%r14d
 	addpd  %xmm2,%xmm1
-	je     101e9 <convolution+0xd9>
+	je     101a9 <convolution+0xd9>
 	mov    %ecx,%edx
 	sub    %eax,%edx
 	cltq
 	movslq %edx,%rdx
 	movsd  (%rsi,%rdx,8),%xmm0
 	mulsd  (%rdi,%rax,8),%xmm0
 	addsd  %xmm0,%xmm1
 	movsd  %xmm1,(%r9)
 	add    $0x1,%ecx
 	add    $0x8,%r9
 	add    $0x8,%rbp
 	cmp    %r13d,%ecx
-	jl     10160 <convolution+0x50>
+	jl     10120 <convolution+0x50>
 	cmp    %ecx,%ebx
-	jle    102ef <convolution+0x1df>
+	jle    102af <convolution+0x1df>
 	movslq %ecx,%r9
 	sub    %r11d,%ecx
 	movslq %r11d,%r11
 	mov    $0x1,%ebp
 	mov    %r9,%rax
 	lea    -0x10(,%r12,8),%r12
 	sub    %r11,%rax
@@ -12411,20 +12405,20 @@
 	cmp    %r9d,%r10d
 	mov    %r9d,%r13d
 	movq   $0x0,(%r8,%r9,8)
 	mov    %ecx,%edx
 	cmovle %r10d,%r13d
 	mov    %r9d,%eax
 	cmp    %ecx,%r13d
-	jl     102db <convolution+0x1cb>
+	jl     1029b <convolution+0x1cb>
 	mov    %ebp,%r14d
 	sub    %ecx,%r14d
 	add    %r13d,%r14d
 	cmp    %ecx,%r13d
-	je     1030b <convolution+0x1fb>
+	je     102cb <convolution+0x1fb>
 	mov    %r14d,%r15d
 	lea    (%rsi,%r12,1),%r13
 	pxor   %xmm2,%xmm2
 	mov    %r11,%rdx
 	shr    %r15d
 	shl    $0x4,%r15
 	add    %r11,%r15
@@ -12433,86 +12427,86 @@
 	movupd (%rdx),%xmm7
 	add    $0x10,%rdx
 	sub    $0x10,%r13
 	shufpd $0x1,%xmm0,%xmm0
 	mulpd  %xmm7,%xmm0
 	addpd  %xmm0,%xmm2
 	cmp    %rdx,%r15
-	jne    10280 <convolution+0x170>
+	jne    10240 <convolution+0x170>
 	movapd %xmm2,%xmm1
 	mov    %r14d,%r13d
 	unpckhpd %xmm2,%xmm1
 	and    $0xfffffffe,%r13d
 	addpd  %xmm2,%xmm1
 	lea    (%rcx,%r13,1),%edx
 	cmp    %r13d,%r14d
-	je     102d5 <convolution+0x1c5>
+	je     10295 <convolution+0x1c5>
 	sub    %edx,%eax
 	movslq %edx,%rdx
 	cltq
 	movsd  (%rsi,%rax,8),%xmm0
 	mulsd  (%rdi,%rdx,8),%xmm0
 	addsd  %xmm0,%xmm1
 	movsd  %xmm1,(%r8,%r9,8)
 	add    $0x1,%r9
 	add    $0x1,%ecx
 	add    $0x8,%r11
 	cmp    %r9d,%ebx
-	jg     10230 <convolution+0x120>
+	jg     101f0 <convolution+0x120>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopw   0x0(%rax,%rax,1)
 	xor    %ecx,%ecx
 	pxor   %xmm3,%xmm3
-	jmp    1020a <convolution+0xfa>
+	jmp    101ca <convolution+0xfa>
 	movapd %xmm3,%xmm1
-	jmp    102c0 <convolution+0x1b0>
+	jmp    10280 <convolution+0x1b0>
 	movapd %xmm3,%xmm1
-	jmp    101d2 <convolution+0xc2>
+	jmp    10192 <convolution+0xc2>
 	nopw   0x0(%rax,%rax,1)
 
-0000000000010320 <convolutionf>:
+00000000000102e0 <convolutionf>:
 convolutionf():
 	push   %r15
 	push   %r14
 	push   %r13
 	lea    -0x1(%rsi,%rcx,1),%r13d
 	push   %r12
 	push   %rbp
 	push   %rbx
 	mov    %ecx,-0xc(%rsp)
 	test   %r13d,%r13d
-	jle    1059b <convolutionf+0x27b>
+	jle    1055b <convolutionf+0x27b>
 	lea    -0x1(%rcx),%r15d
 	mov    %rdx,%r10
 	lea    -0x1(%rsi),%r11d
 	mov    %r8,%r12
 	test   %r15d,%r15d
-	jle    105b0 <convolutionf+0x290>
+	jle    10570 <convolutionf+0x290>
 	cmp    %r15d,%r13d
 	lea    -0xc(%rdx),%rbp
 	pxor   %xmm2,%xmm2
 	mov    %r15d,%r14d
 	cmovle %r13d,%r14d
 	xor    %ecx,%ecx
 	nopw   0x0(%rax,%rax,1)
 	cmp    %r11d,%ecx
 	mov    %r11d,%r9d
 	movl   $0x0,(%r8)
 	cmovle %ecx,%r9d
 	test   %r9d,%r9d
-	js     1044e <convolutionf+0x12e>
+	js     1040e <convolutionf+0x12e>
 	lea    0x1(%r9),%ebx
 	cmp    $0x2,%r9d
-	jle    105c3 <convolutionf+0x2a3>
+	jle    10583 <convolutionf+0x2a3>
 	mov    %ebx,%esi
 	mov    %rdi,%rax
 	pxor   %xmm1,%xmm1
 	mov    %rbp,%rdx
 	shr    $0x2,%esi
 	shl    $0x4,%rsi
 	add    %rdi,%rsi
@@ -12521,59 +12515,59 @@
 	movups (%rax),%xmm4
 	add    $0x10,%rax
 	sub    $0x10,%rdx
 	shufps $0x1b,%xmm0,%xmm0
 	mulps  %xmm4,%xmm0
 	addps  %xmm0,%xmm1
 	cmp    %rsi,%rax
-	jne    103b0 <convolutionf+0x90>
+	jne    10370 <convolutionf+0x90>
 	movaps %xmm1,%xmm0
 	mov    %ebx,%eax
 	movhlps %xmm1,%xmm0
 	and    $0xfffffffc,%eax
 	and    $0x3,%ebx
 	addps  %xmm1,%xmm0
 	movaps %xmm0,%xmm1
 	shufps $0x55,%xmm0,%xmm1
 	addps  %xmm0,%xmm1
-	je     10449 <convolutionf+0x129>
+	je     10409 <convolutionf+0x129>
 	mov    %ecx,%ebx
 	movslq %eax,%rdx
 	sub    %eax,%ebx
 	lea    0x0(,%rdx,4),%rsi
 	movslq %ebx,%rbx
 	movss  (%r10,%rbx,4),%xmm0
 	mulss  (%rdi,%rdx,4),%xmm0
 	lea    0x1(%rax),%ebx
 	addss  %xmm0,%xmm1
 	cmp    %ebx,%r9d
-	jl     10449 <convolutionf+0x129>
+	jl     10409 <convolutionf+0x129>
 	mov    %ecx,%edx
 	add    $0x2,%eax
 	sub    %ebx,%edx
 	movslq %edx,%rdx
 	movss  (%r10,%rdx,4),%xmm0
 	mulss  0x4(%rdi,%rsi,1),%xmm0
 	addss  %xmm0,%xmm1
 	cmp    %eax,%r9d
-	jl     10449 <convolutionf+0x129>
+	jl     10409 <convolutionf+0x129>
 	mov    %ecx,%edx
 	sub    %eax,%edx
 	movslq %edx,%rax
 	movss  (%r10,%rax,4),%xmm0
 	mulss  0x8(%rdi,%rsi,1),%xmm0
 	addss  %xmm0,%xmm1
 	movss  %xmm1,(%r8)
 	add    $0x1,%ecx
 	add    $0x4,%r8
 	add    $0x4,%rbp
 	cmp    %r14d,%ecx
-	jl     10370 <convolutionf+0x50>
+	jl     10330 <convolutionf+0x50>
 	cmp    %ecx,%r13d
-	jle    1059b <convolutionf+0x27b>
+	jle    1055b <convolutionf+0x27b>
 	movslq %ecx,%r8
 	sub    %r15d,%ecx
 	movslq %r15d,%r15
 	mov    %r8,%rax
 	sub    %r15,%rax
 	lea    (%rdi,%rax,4),%rbx
 	movslq -0xc(%rsp),%rax
@@ -12582,20 +12576,20 @@
 	cmp    %r8d,%r11d
 	mov    %r8d,%r14d
 	movl   $0x0,(%r12,%r8,4)
 	mov    %ecx,%eax
 	cmovle %r11d,%r14d
 	mov    %r8d,%r9d
 	cmp    %ecx,%r14d
-	jl     10587 <convolutionf+0x267>
+	jl     10547 <convolutionf+0x267>
 	mov    %r14d,%edx
 	sub    %ecx,%edx
 	lea    0x1(%rdx),%r15d
 	cmp    $0x2,%edx
-	jbe    105bb <convolutionf+0x29b>
+	jbe    1057b <convolutionf+0x29b>
 	mov    %r15d,%esi
 	lea    (%r10,%rbp,1),%rdx
 	pxor   %xmm1,%xmm1
 	mov    %rbx,%rax
 	shr    $0x2,%esi
 	shl    $0x4,%rsi
 	add    %rbx,%rsi
@@ -12604,147 +12598,147 @@
 	movups (%rax),%xmm6
 	add    $0x10,%rax
 	sub    $0x10,%rdx
 	shufps $0x1b,%xmm0,%xmm0
 	mulps  %xmm6,%xmm0
 	addps  %xmm0,%xmm1
 	cmp    %rax,%rsi
-	jne    104e0 <convolutionf+0x1c0>
+	jne    104a0 <convolutionf+0x1c0>
 	movaps %xmm1,%xmm0
 	mov    %r15d,%edx
 	movhlps %xmm1,%xmm0
 	and    $0xfffffffc,%edx
 	addps  %xmm1,%xmm0
 	lea    (%rcx,%rdx,1),%eax
 	movaps %xmm0,%xmm1
 	shufps $0x55,%xmm0,%xmm1
 	addps  %xmm0,%xmm1
 	cmp    %edx,%r15d
-	je     10581 <convolutionf+0x261>
+	je     10541 <convolutionf+0x261>
 	mov    %r9d,%r15d
 	movslq %eax,%rsi
 	sub    %eax,%r15d
 	lea    0x0(,%rsi,4),%rdx
 	movslq %r15d,%r15
 	movss  (%r10,%r15,4),%xmm0
 	mulss  (%rdi,%rsi,4),%xmm0
 	lea    0x1(%rax),%r15d
 	addss  %xmm0,%xmm1
 	cmp    %r14d,%r15d
-	jg     10581 <convolutionf+0x261>
+	jg     10541 <convolutionf+0x261>
 	mov    %r9d,%esi
 	add    $0x2,%eax
 	sub    %r15d,%esi
 	movslq %esi,%rsi
 	movss  (%r10,%rsi,4),%xmm0
 	mulss  0x4(%rdi,%rdx,1),%xmm0
 	addss  %xmm0,%xmm1
 	cmp    %eax,%r14d
-	jl     10581 <convolutionf+0x261>
+	jl     10541 <convolutionf+0x261>
 	sub    %eax,%r9d
 	movslq %r9d,%r9
 	movss  (%r10,%r9,4),%xmm0
 	mulss  0x8(%rdi,%rdx,1),%xmm0
 	addss  %xmm0,%xmm1
 	movss  %xmm1,(%r12,%r8,4)
 	add    $0x1,%r8
 	add    $0x1,%ecx
 	add    $0x4,%rbx
 	cmp    %r8d,%r13d
-	jg     10490 <convolutionf+0x170>
+	jg     10450 <convolutionf+0x170>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 	xor    %ecx,%ecx
 	pxor   %xmm2,%xmm2
-	jmp    1046b <convolutionf+0x14b>
+	jmp    1042b <convolutionf+0x14b>
 	movaps %xmm2,%xmm1
-	jmp    1051e <convolutionf+0x1fe>
+	jmp    104de <convolutionf+0x1fe>
 	movaps %xmm2,%xmm1
 	xor    %eax,%eax
-	jmp    103ea <convolutionf+0xca>
+	jmp    103aa <convolutionf+0xca>
 	nopl   (%rax)
 
-00000000000105d0 <mean>:
+0000000000010590 <mean>:
 mean():
 	test   %esi,%esi
-	jle    10670 <mean+0xa0>
+	jle    10630 <mean+0xa0>
 	lea    -0x1(%rsi),%eax
 	cmp    $0x3,%eax
-	jbe    10681 <mean+0xb1>
+	jbe    10641 <mean+0xb1>
 	mov    %esi,%edx
 	mov    %rdi,%rax
 	pxor   %xmm0,%xmm0
 	shr    %edx
 	shl    $0x4,%rdx
 	add    %rdi,%rdx
 	cs nopw 0x0(%rax,%rax,1)
 	movupd (%rax),%xmm2
 	add    $0x10,%rax
 	addpd  %xmm2,%xmm0
 	cmp    %rdx,%rax
-	jne    10600 <mean+0x30>
+	jne    105c0 <mean+0x30>
 	movapd %xmm0,%xmm1
 	mov    %esi,%eax
 	unpckhpd %xmm0,%xmm1
 	and    $0xfffffffe,%eax
 	addpd  %xmm1,%xmm0
 	test   $0x1,%sil
-	je     1065c <mean+0x8c>
+	je     1061c <mean+0x8c>
 	movslq %eax,%rdx
 	addsd  (%rdi,%rdx,8),%xmm0
 	lea    0x1(%rax),%edx
 	cmp    %edx,%esi
-	jle    1065c <mean+0x8c>
+	jle    1061c <mean+0x8c>
 	movslq %edx,%rdx
 	addsd  (%rdi,%rdx,8),%xmm0
 	lea    0x2(%rax),%edx
 	cmp    %edx,%esi
-	jle    1065c <mean+0x8c>
+	jle    1061c <mean+0x8c>
 	movslq %edx,%rdx
 	add    $0x3,%eax
 	addsd  (%rdi,%rdx,8),%xmm0
 	cmp    %eax,%esi
-	jle    1065c <mean+0x8c>
+	jle    1061c <mean+0x8c>
 	cltq
 	addsd  (%rdi,%rax,8),%xmm0
 	pxor   %xmm1,%xmm1
 	cvtsi2sd %esi,%xmm1
 	divsd  %xmm1,%xmm0
 	ret
 	nopl   0x0(%rax)
 	pxor   %xmm1,%xmm1
 	pxor   %xmm0,%xmm0
 	cvtsi2sd %esi,%xmm1
 	divsd  %xmm1,%xmm0
 	ret
 	xor    %eax,%eax
 	pxor   %xmm0,%xmm0
-	jmp    10628 <mean+0x58>
+	jmp    105e8 <mean+0x58>
 	nopl   0x0(%rax)
 
-0000000000010690 <stdev>:
+0000000000010650 <stdev>:
 stdev():
 	push   %rbp
 	mov    %rdi,%rbp
 	push   %rbx
 	mov    %esi,%ebx
 	sub    $0x8,%rsp
 	call   30e0 <mean@plt>
 	test   %ebx,%ebx
-	jle    10758 <stdev+0xc8>
+	jle    10718 <stdev+0xc8>
 	lea    -0x1(%rbx),%eax
 	movapd %xmm0,%xmm3
 	cmp    $0x1,%eax
-	jbe    1075e <stdev+0xce>
+	jbe    1071e <stdev+0xce>
 	mov    %ebx,%edx
 	movapd %xmm0,%xmm2
 	pxor   %xmm1,%xmm1
 	mov    %rbp,%rax
 	shr    %edx
 	unpcklpd %xmm2,%xmm2
 	shl    $0x4,%rdx
@@ -12752,30 +12746,30 @@
 	nopw   0x0(%rax,%rax,1)
 	movupd (%rax),%xmm0
 	add    $0x10,%rax
 	subpd  %xmm2,%xmm0
 	mulpd  %xmm0,%xmm0
 	addpd  %xmm0,%xmm1
 	cmp    %rdx,%rax
-	jne    106d8 <stdev+0x48>
+	jne    10698 <stdev+0x48>
 	movapd %xmm1,%xmm0
 	mov    %ebx,%eax
 	unpckhpd %xmm1,%xmm0
 	and    $0xfffffffe,%eax
 	addpd  %xmm0,%xmm1
 	test   $0x1,%bl
-	je     10737 <stdev+0xa7>
+	je     106f7 <stdev+0xa7>
 	movslq %eax,%rdx
 	add    $0x1,%eax
 	movsd  0x0(%rbp,%rdx,8),%xmm0
 	subsd  %xmm3,%xmm0
 	mulsd  %xmm0,%xmm0
 	addsd  %xmm0,%xmm1
 	cmp    %eax,%ebx
-	jle    10737 <stdev+0xa7>
+	jle    106f7 <stdev+0xa7>
 	cltq
 	movsd  0x0(%rbp,%rax,8),%xmm0
 	subsd  %xmm3,%xmm0
 	mulsd  %xmm0,%xmm0
 	addsd  %xmm0,%xmm1
 	pxor   %xmm0,%xmm0
 	add    $0x8,%rsp
@@ -12784,90 +12778,90 @@
 	pop    %rbp
 	divsd  %xmm0,%xmm1
 	sqrtsd %xmm1,%xmm1
 	movapd %xmm1,%xmm0
 	ret
 	nopw   0x0(%rax,%rax,1)
 	pxor   %xmm1,%xmm1
-	jmp    10737 <stdev+0xa7>
+	jmp    106f7 <stdev+0xa7>
 	xor    %eax,%eax
 	pxor   %xmm1,%xmm1
-	jmp    10707 <stdev+0x77>
+	jmp    106c7 <stdev+0x77>
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000010770 <meanf>:
+0000000000010730 <meanf>:
 meanf():
 	test   %esi,%esi
-	jle    10800 <meanf+0x90>
+	jle    107c0 <meanf+0x90>
 	lea    -0x1(%rsi),%eax
 	cmp    $0x2,%eax
-	jbe    10811 <meanf+0xa1>
+	jbe    107d1 <meanf+0xa1>
 	mov    %esi,%edx
 	mov    %rdi,%rax
 	pxor   %xmm0,%xmm0
 	shr    $0x2,%edx
 	shl    $0x4,%rdx
 	add    %rdi,%rdx
 	nopw   0x0(%rax,%rax,1)
 	movups (%rax),%xmm2
 	add    $0x10,%rax
 	addps  %xmm2,%xmm0
 	cmp    %rdx,%rax
-	jne    107a0 <meanf+0x30>
+	jne    10760 <meanf+0x30>
 	movaps %xmm0,%xmm1
 	mov    %esi,%eax
 	movhlps %xmm0,%xmm1
 	and    $0xfffffffc,%eax
 	addps  %xmm0,%xmm1
 	movaps %xmm1,%xmm0
 	shufps $0x55,%xmm1,%xmm0
 	addps  %xmm1,%xmm0
 	test   $0x3,%sil
-	je     107f2 <meanf+0x82>
+	je     107b2 <meanf+0x82>
 	movslq %eax,%rdx
 	addss  (%rdi,%rdx,4),%xmm0
 	lea    0x1(%rax),%edx
 	cmp    %edx,%esi
-	jle    107f2 <meanf+0x82>
+	jle    107b2 <meanf+0x82>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	addss  (%rdi,%rdx,4),%xmm0
 	cmp    %eax,%esi
-	jle    107f2 <meanf+0x82>
+	jle    107b2 <meanf+0x82>
 	cltq
 	addss  (%rdi,%rax,4),%xmm0
 	pxor   %xmm1,%xmm1
 	cvtsi2ss %esi,%xmm1
 	divss  %xmm1,%xmm0
 	ret
 	nop
 	pxor   %xmm1,%xmm1
 	pxor   %xmm0,%xmm0
 	cvtsi2ss %esi,%xmm1
 	divss  %xmm1,%xmm0
 	ret
 	xor    %eax,%eax
 	pxor   %xmm0,%xmm0
-	jmp    107cd <meanf+0x5d>
+	jmp    1078d <meanf+0x5d>
 	nopl   0x0(%rax)
 
-0000000000010820 <stdevf>:
+00000000000107e0 <stdevf>:
 stdevf():
 	push   %rbp
 	mov    %rdi,%rbp
 	push   %rbx
 	mov    %esi,%ebx
 	sub    $0x8,%rsp
 	call   3200 <meanf@plt>
 	test   %ebx,%ebx
-	jle    10900 <stdevf+0xe0>
+	jle    108c0 <stdevf+0xe0>
 	lea    -0x1(%rbx),%eax
 	movaps %xmm0,%xmm2
 	cmp    $0x2,%eax
-	jbe    10906 <stdevf+0xe6>
+	jbe    108c6 <stdevf+0xe6>
 	mov    %ebx,%edx
 	movaps %xmm0,%xmm3
 	pxor   %xmm1,%xmm1
 	mov    %rbp,%rax
 	shr    $0x2,%edx
 	shufps $0x0,%xmm3,%xmm3
 	shl    $0x4,%rdx
@@ -12875,41 +12869,41 @@
 	nopl   0x0(%rax)
 	movups (%rax),%xmm0
 	add    $0x10,%rax
 	subps  %xmm3,%xmm0
 	mulps  %xmm0,%xmm0
 	addps  %xmm0,%xmm1
 	cmp    %rdx,%rax
-	jne    10868 <stdevf+0x48>
+	jne    10828 <stdevf+0x48>
 	movaps %xmm1,%xmm0
 	mov    %ebx,%eax
 	movhlps %xmm1,%xmm0
 	and    $0xfffffffc,%eax
 	addps  %xmm0,%xmm1
 	movaps %xmm1,%xmm0
 	shufps $0x55,%xmm1,%xmm0
 	addps  %xmm1,%xmm0
 	test   $0x3,%bl
-	je     108e6 <stdevf+0xc6>
+	je     108a6 <stdevf+0xc6>
 	movslq %eax,%rdx
 	movss  0x0(%rbp,%rdx,4),%xmm1
 	lea    0x1(%rax),%edx
 	subss  %xmm2,%xmm1
 	mulss  %xmm1,%xmm1
 	addss  %xmm1,%xmm0
 	cmp    %edx,%ebx
-	jle    108e6 <stdevf+0xc6>
+	jle    108a6 <stdevf+0xc6>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	movss  0x0(%rbp,%rdx,4),%xmm1
 	subss  %xmm2,%xmm1
 	mulss  %xmm1,%xmm1
 	addss  %xmm1,%xmm0
 	cmp    %eax,%ebx
-	jle    108e6 <stdevf+0xc6>
+	jle    108a6 <stdevf+0xc6>
 	cltq
 	movss  0x0(%rbp,%rax,4),%xmm1
 	subss  %xmm2,%xmm1
 	mulss  %xmm1,%xmm1
 	addss  %xmm1,%xmm0
 	pxor   %xmm1,%xmm1
 	add    $0x8,%rsp
@@ -12917,309 +12911,309 @@
 	pop    %rbx
 	pop    %rbp
 	divss  %xmm1,%xmm0
 	sqrtss %xmm0,%xmm0
 	ret
 	nopl   (%rax)
 	pxor   %xmm0,%xmm0
-	jmp    108e6 <stdevf+0xc6>
+	jmp    108a6 <stdevf+0xc6>
 	xor    %eax,%eax
 	pxor   %xmm0,%xmm0
-	jmp    1089a <stdevf+0x7a>
+	jmp    1085a <stdevf+0x7a>
 	xchg   %ax,%ax
 
-0000000000010910 <fast_sin>:
+00000000000108d0 <fast_sin>:
 fast_sin():
 	movapd %xmm0,%xmm3
-	movsd  0x7944(%rip),%xmm1        
-	andpd  0x783c(%rip),%xmm3        
+	movsd  0x7984(%rip),%xmm1        
+	andpd  0x787c(%rip),%xmm3        
 	movapd %xmm0,%xmm2
 	mulsd  %xmm3,%xmm1
 	cvttsd2si %xmm1,%eax
 	pxor   %xmm1,%xmm1
 	add    $0x1,%eax
 	mov    %eax,%edx
 	and    $0x4,%eax
 	and    $0xfffffffe,%edx
 	cvtsi2sd %edx,%xmm1
-	mulsd  0x791d(%rip),%xmm1        
+	mulsd  0x795d(%rip),%xmm1        
 	and    $0x2,%edx
 	subsd  %xmm1,%xmm3
 	movapd %xmm3,%xmm1
 	mulsd  %xmm3,%xmm1
 	movapd %xmm1,%xmm0
-	jne    109c8 <fast_sin+0xb8>
-	mulsd  0x7908(%rip),%xmm0        
-	subsd  0x7908(%rip),%xmm0        
+	jne    10988 <fast_sin+0xb8>
+	mulsd  0x7948(%rip),%xmm0        
+	subsd  0x7948(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
-	addsd  0x7904(%rip),%xmm0        
+	addsd  0x7944(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
-	subsd  0x7900(%rip),%xmm0        
+	subsd  0x7940(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
-	addsd  0x78fc(%rip),%xmm0        
+	addsd  0x793c(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
 	mulsd  %xmm3,%xmm1
-	subsd  0x78f4(%rip),%xmm0        
+	subsd  0x7934(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
 	addsd  %xmm3,%xmm0
 	test   %eax,%eax
-	je     109b8 <fast_sin+0xa8>
-	xorpd  0x77b8(%rip),%xmm0        
+	je     10978 <fast_sin+0xa8>
+	xorpd  0x77f8(%rip),%xmm0        
 	pxor   %xmm1,%xmm1
 	comisd %xmm2,%xmm1
-	ja     10a38 <fast_sin+0x128>
+	ja     109f8 <fast_sin+0x128>
 	ret
 	nopl   0x0(%rax,%rax,1)
-	mulsd  0x78d0(%rip),%xmm0        
+	mulsd  0x7910(%rip),%xmm0        
 	movapd %xmm1,%xmm3
-	addsd  0x78cc(%rip),%xmm0        
+	addsd  0x790c(%rip),%xmm0        
 	mulsd  %xmm1,%xmm3
 	mulsd  %xmm1,%xmm0
-	subsd  0x78c4(%rip),%xmm0        
+	subsd  0x7904(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
-	addsd  0x78c0(%rip),%xmm0        
+	addsd  0x7900(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
-	subsd  0x78bc(%rip),%xmm0        
+	subsd  0x78fc(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
-	addsd  0x78b8(%rip),%xmm0        
-	mulsd  0x78b8(%rip),%xmm1        
+	addsd  0x78f8(%rip),%xmm0        
+	mulsd  0x78f8(%rip),%xmm1        
 	mulsd  %xmm3,%xmm0
-	movsd  0x78b4(%rip),%xmm3        
+	movsd  0x78f4(%rip),%xmm3        
 	subsd  %xmm1,%xmm3
 	addsd  %xmm3,%xmm0
-	jmp    109ac <fast_sin+0x9c>
+	jmp    1096c <fast_sin+0x9c>
 	nopl   0x0(%rax)
-	xorpd  0x7730(%rip),%xmm0        
+	xorpd  0x7770(%rip),%xmm0        
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
-0000000000010a50 <fast_cos>:
+0000000000010a10 <fast_cos>:
 fast_cos():
-	andpd  0x7708(%rip),%xmm0        
-	movsd  0x7800(%rip),%xmm1        
+	andpd  0x7748(%rip),%xmm0        
+	movsd  0x7840(%rip),%xmm1        
 	mulsd  %xmm0,%xmm1
 	movapd %xmm0,%xmm3
 	cvttsd2si %xmm1,%edx
 	pxor   %xmm1,%xmm1
 	add    $0x1,%edx
 	and    $0xfffffffe,%edx
 	cvtsi2sd %edx,%xmm1
-	mulsd  0x77e6(%rip),%xmm1        
+	mulsd  0x7826(%rip),%xmm1        
 	sub    $0x2,%edx
 	mov    %edx,%eax
 	and    $0x4,%eax
 	and    $0x2,%edx
 	subsd  %xmm1,%xmm3
 	movapd %xmm3,%xmm0
 	mulsd  %xmm3,%xmm0
-	je     10b18 <fast_cos+0xc8>
-	movsd  0x77fd(%rip),%xmm1        
+	je     10ad8 <fast_cos+0xc8>
+	movsd  0x783d(%rip),%xmm1        
 	movapd %xmm0,%xmm2
 	mulsd  %xmm0,%xmm2
 	mulsd  %xmm0,%xmm1
-	addsd  0x77f1(%rip),%xmm1        
+	addsd  0x7831(%rip),%xmm1        
 	mulsd  %xmm0,%xmm1
-	subsd  0x77ed(%rip),%xmm1        
+	subsd  0x782d(%rip),%xmm1        
 	mulsd  %xmm0,%xmm1
-	addsd  0x77e9(%rip),%xmm1        
+	addsd  0x7829(%rip),%xmm1        
 	mulsd  %xmm0,%xmm1
-	subsd  0x77e5(%rip),%xmm1        
+	subsd  0x7825(%rip),%xmm1        
 	mulsd  %xmm0,%xmm1
-	addsd  0x77e1(%rip),%xmm1        
+	addsd  0x7821(%rip),%xmm1        
 	mulsd  %xmm2,%xmm1
-	movsd  0x77dd(%rip),%xmm2        
+	movsd  0x781d(%rip),%xmm2        
 	mulsd  %xmm0,%xmm2
-	movsd  0x77d9(%rip),%xmm0        
+	movsd  0x7819(%rip),%xmm0        
 	subsd  %xmm2,%xmm0
 	addsd  %xmm1,%xmm0
 	test   %eax,%eax
-	jne    10b13 <fast_cos+0xc3>
-	xorpd  0x765d(%rip),%xmm0        
+	jne    10ad3 <fast_cos+0xc3>
+	xorpd  0x769d(%rip),%xmm0        
 	ret
 	nopl   0x0(%rax)
-	movsd  0x7750(%rip),%xmm2        
+	movsd  0x7790(%rip),%xmm2        
 	movapd %xmm0,%xmm1
 	mulsd  %xmm3,%xmm1
 	mulsd  %xmm0,%xmm2
-	subsd  0x7744(%rip),%xmm2        
+	subsd  0x7784(%rip),%xmm2        
 	mulsd  %xmm0,%xmm2
-	addsd  0x7740(%rip),%xmm2        
+	addsd  0x7780(%rip),%xmm2        
 	mulsd  %xmm0,%xmm2
-	subsd  0x773c(%rip),%xmm2        
+	subsd  0x777c(%rip),%xmm2        
 	mulsd  %xmm0,%xmm2
-	addsd  0x7738(%rip),%xmm2        
+	addsd  0x7778(%rip),%xmm2        
 	mulsd  %xmm0,%xmm2
-	subsd  0x7734(%rip),%xmm2        
+	subsd  0x7774(%rip),%xmm2        
 	movapd %xmm2,%xmm0
 	mulsd  %xmm1,%xmm0
 	addsd  %xmm3,%xmm0
-	jmp    10b07 <fast_cos+0xb7>
+	jmp    10ac7 <fast_cos+0xb7>
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-0000000000010b80 <fast_exp>:
+0000000000010b40 <fast_exp>:
 fast_exp():
 	movapd %xmm0,%xmm2
-	comisd 0x77ec(%rip),%xmm2        
-	movsd  0x77dc(%rip),%xmm0        
-	ja     10c5c <fast_exp+0xdc>
-	movsd  0x77de(%rip),%xmm0        
+	comisd 0x782c(%rip),%xmm2        
+	movsd  0x781c(%rip),%xmm0        
+	ja     10c1c <fast_exp+0xdc>
+	movsd  0x781e(%rip),%xmm0        
 	pxor   %xmm5,%xmm5
 	movapd %xmm2,%xmm1
-	movsd  0x77de(%rip),%xmm4        
+	movsd  0x781e(%rip),%xmm4        
 	mulsd  %xmm2,%xmm0
-	addsd  0x7712(%rip),%xmm0        
+	addsd  0x7752(%rip),%xmm0        
 	cvttsd2si %xmm0,%eax
 	cvtsd2ss %xmm0,%xmm5
 	movd   %xmm5,%edx
 	pxor   %xmm0,%xmm0
 	shr    $0x1f,%edx
 	sub    %edx,%eax
 	cvtsi2sd %eax,%xmm0
-	mulsd  0x77a9(%rip),%xmm0        
+	mulsd  0x77e9(%rip),%xmm0        
 	cltq
 	add    $0x3ff,%rax
 	shl    $0x34,%rax
 	subsd  %xmm0,%xmm1
-	movsd  0x76e1(%rip),%xmm0        
+	movsd  0x7721(%rip),%xmm0        
 	movapd %xmm1,%xmm3
 	mulsd  %xmm1,%xmm3
 	mulsd  %xmm3,%xmm4
-	addsd  0x778d(%rip),%xmm4        
+	addsd  0x77cd(%rip),%xmm4        
 	mulsd  %xmm3,%xmm4
 	addsd  %xmm0,%xmm4
 	mulsd  %xmm4,%xmm1
-	movsd  0x7781(%rip),%xmm4        
+	movsd  0x77c1(%rip),%xmm4        
 	mulsd  %xmm3,%xmm4
-	addsd  0x777d(%rip),%xmm4        
+	addsd  0x77bd(%rip),%xmm4        
 	mulsd  %xmm3,%xmm4
-	addsd  0x7779(%rip),%xmm4        
+	addsd  0x77b9(%rip),%xmm4        
 	mulsd  %xmm4,%xmm3
-	addsd  0x7775(%rip),%xmm3        
+	addsd  0x77b5(%rip),%xmm3        
 	subsd  %xmm1,%xmm3
 	divsd  %xmm3,%xmm1
 	addsd  %xmm1,%xmm1
 	addsd  %xmm0,%xmm1
 	movq   %rax,%xmm0
 	mulsd  %xmm1,%xmm0
-	movsd  0x775c(%rip),%xmm1        
+	movsd  0x779c(%rip),%xmm1        
 	comisd %xmm2,%xmm1
-	jbe    10c6e <fast_exp+0xee>
+	jbe    10c2e <fast_exp+0xee>
 	pxor   %xmm0,%xmm0
 	ret
 	nop
 
-0000000000010c70 <fast_sinf>:
+0000000000010c30 <fast_sinf>:
 fast_sinf():
-	movss  0x7668(%rip),%xmm1        
+	movss  0x76a8(%rip),%xmm1        
 	movaps %xmm0,%xmm2
 	movaps %xmm0,%xmm3
-	andps  0x75bb(%rip),%xmm2        
+	andps  0x75fb(%rip),%xmm2        
 	mulss  %xmm2,%xmm1
 	cvttss2si %xmm1,%eax
 	pxor   %xmm1,%xmm1
 	add    $0x1,%eax
 	mov    %eax,%edx
 	and    $0x4,%eax
 	and    $0xfffffffe,%edx
 	cvtsi2ss %edx,%xmm1
-	mulss  0x763c(%rip),%xmm1        
+	mulss  0x767c(%rip),%xmm1        
 	and    $0x2,%edx
 	subss  %xmm1,%xmm2
 	movaps %xmm2,%xmm4
 	mulss  %xmm2,%xmm4
-	jne    10d00 <fast_sinf+0x90>
-	movss  0x763c(%rip),%xmm1        
+	jne    10cc0 <fast_sinf+0x90>
+	movss  0x767c(%rip),%xmm1        
 	mulss  %xmm4,%xmm1
-	addss  0x7634(%rip),%xmm1        
+	addss  0x7674(%rip),%xmm1        
 	mulss  %xmm4,%xmm1
-	subss  0x762c(%rip),%xmm1        
+	subss  0x766c(%rip),%xmm1        
 	mulss  %xmm4,%xmm1
 	movaps %xmm1,%xmm0
 	mulss  %xmm2,%xmm0
 	addss  %xmm2,%xmm0
 	test   %eax,%eax
-	je     10cf2 <fast_sinf+0x82>
-	xorps  0x755e(%rip),%xmm0        
+	je     10cb2 <fast_sinf+0x82>
+	xorps  0x759e(%rip),%xmm0        
 	pxor   %xmm1,%xmm1
 	comiss %xmm3,%xmm1
-	ja     10d40 <fast_sinf+0xd0>
+	ja     10d00 <fast_sinf+0xd0>
 	ret
 	nopl   0x0(%rax)
-	movss  0x75e0(%rip),%xmm0        
+	movss  0x7620(%rip),%xmm0        
 	mulss  %xmm4,%xmm0
-	subss  0x75d8(%rip),%xmm0        
+	subss  0x7618(%rip),%xmm0        
 	mulss  %xmm4,%xmm0
-	addss  0x75d0(%rip),%xmm0        
+	addss  0x7610(%rip),%xmm0        
 	mulss  %xmm4,%xmm0
-	subss  0x75c8(%rip),%xmm0        
+	subss  0x7608(%rip),%xmm0        
 	mulss  %xmm4,%xmm0
-	addss  0x75c0(%rip),%xmm0        
-	jmp    10ce7 <fast_sinf+0x77>
+	addss  0x7600(%rip),%xmm0        
+	jmp    10ca7 <fast_sinf+0x77>
 	nopw   0x0(%rax,%rax,1)
-	xorps  0x7509(%rip),%xmm0        
+	xorps  0x7549(%rip),%xmm0        
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-0000000000010d50 <fast_cosf>:
+0000000000010d10 <fast_cosf>:
 fast_cosf():
-	andps  0x74e9(%rip),%xmm0        
-	movss  0x7581(%rip),%xmm1        
+	andps  0x7529(%rip),%xmm0        
+	movss  0x75c1(%rip),%xmm1        
 	mulss  %xmm0,%xmm1
 	movaps %xmm0,%xmm3
 	cvttss2si %xmm1,%eax
 	pxor   %xmm1,%xmm1
 	add    $0x1,%eax
 	and    $0xfffffffe,%eax
 	cvtsi2ss %eax,%xmm1
-	mulss  0x7564(%rip),%xmm1        
+	mulss  0x75a4(%rip),%xmm1        
 	sub    $0x2,%eax
 	mov    %eax,%edx
 	and    $0x4,%edx
 	subss  %xmm1,%xmm3
 	movaps %xmm3,%xmm0
 	mulss  %xmm3,%xmm0
 	test   $0x2,%al
-	je     10de0 <fast_cosf+0x90>
-	movss  0x7549(%rip),%xmm2        
+	je     10da0 <fast_cosf+0x90>
+	movss  0x7589(%rip),%xmm2        
 	mulss  %xmm0,%xmm2
-	subss  0x7541(%rip),%xmm2        
+	subss  0x7581(%rip),%xmm2        
 	mulss  %xmm0,%xmm2
-	addss  0x7539(%rip),%xmm2        
+	addss  0x7579(%rip),%xmm2        
 	mulss  %xmm0,%xmm2
-	subss  0x7531(%rip),%xmm2        
+	subss  0x7571(%rip),%xmm2        
 	mulss  %xmm2,%xmm0
-	addss  0x7529(%rip),%xmm0        
+	addss  0x7569(%rip),%xmm0        
 	test   %edx,%edx
-	jne    10dda <fast_cosf+0x8a>
-	xorps  0x7476(%rip),%xmm0        
+	jne    10d9a <fast_cosf+0x8a>
+	xorps  0x74b6(%rip),%xmm0        
 	ret
 	nopl   0x0(%rax,%rax,1)
-	movss  0x7514(%rip),%xmm1        
+	movss  0x7554(%rip),%xmm1        
 	mulss  %xmm0,%xmm1
-	addss  0x750c(%rip),%xmm1        
+	addss  0x754c(%rip),%xmm1        
 	mulss  %xmm0,%xmm1
-	subss  0x7504(%rip),%xmm1        
+	subss  0x7544(%rip),%xmm1        
 	mulss  %xmm1,%xmm0
 	mulss  %xmm3,%xmm0
 	addss  %xmm3,%xmm0
-	jmp    10dcf <fast_cosf+0x7f>
+	jmp    10d8f <fast_cosf+0x7f>
 	xchg   %ax,%ax
 
-0000000000010e10 <fast_expf>:
+0000000000010dd0 <fast_expf>:
 fast_expf():
 	movaps %xmm0,%xmm2
-	comiss 0x75da(%rip),%xmm2        
-	movss  0x75ce(%rip),%xmm0        
-	ja     10ede <fast_expf+0xce>
-	movss  0x75c8(%rip),%xmm3        
-	movss  0x74bc(%rip),%xmm4        
-	movss  0x75bc(%rip),%xmm0        
-	movss  0x75b8(%rip),%xmm1        
+	comiss 0x761a(%rip),%xmm2        
+	movss  0x760e(%rip),%xmm0        
+	ja     10e9e <fast_expf+0xce>
+	movss  0x7608(%rip),%xmm3        
+	movss  0x74fc(%rip),%xmm4        
+	movss  0x75fc(%rip),%xmm0        
+	movss  0x75f8(%rip),%xmm1        
 	mulss  %xmm2,%xmm3
 	addss  %xmm4,%xmm3
 	cvttss2si %xmm3,%edx
 	movd   %xmm3,%eax
 	pxor   %xmm3,%xmm3
 	shr    $0x1f,%eax
 	sub    %eax,%edx
@@ -13227,42 +13221,42 @@
 	mulss  %xmm3,%xmm0
 	cvttss2si %xmm3,%eax
 	mulss  %xmm3,%xmm1
 	add    $0x7f,%eax
 	addss  %xmm2,%xmm0
 	shl    $0x17,%eax
 	subss  %xmm1,%xmm0
-	movss  0x757d(%rip),%xmm1        
+	movss  0x75bd(%rip),%xmm1        
 	mulss  %xmm0,%xmm1
-	addss  0x7575(%rip),%xmm1        
+	addss  0x75b5(%rip),%xmm1        
 	mulss  %xmm0,%xmm1
-	addss  0x756d(%rip),%xmm1        
+	addss  0x75ad(%rip),%xmm1        
 	mulss  %xmm0,%xmm1
-	addss  0x7565(%rip),%xmm1        
+	addss  0x75a5(%rip),%xmm1        
 	mulss  %xmm0,%xmm1
-	addss  0x755d(%rip),%xmm1        
+	addss  0x759d(%rip),%xmm1        
 	mulss  %xmm0,%xmm1
 	addss  %xmm4,%xmm1
 	movaps %xmm0,%xmm4
 	mulss  %xmm0,%xmm4
-	addss  0x742a(%rip),%xmm0        
+	addss  0x746a(%rip),%xmm0        
 	mulss  %xmm4,%xmm1
 	addss  %xmm0,%xmm1
 	movd   %eax,%xmm0
 	mulss  %xmm1,%xmm0
-	movss  0x7532(%rip),%xmm1        
+	movss  0x7572(%rip),%xmm1        
 	comiss %xmm2,%xmm1
-	jbe    10eef <fast_expf+0xdf>
+	jbe    10eaf <fast_expf+0xdf>
 	pxor   %xmm0,%xmm0
 	ret
 
-0000000000010ef0 <fast_sinv>:
+0000000000010eb0 <fast_sinv>:
 fast_sinv():
 	test   %esi,%esi
-	jle    10f40 <fast_sinv+0x50>
+	jle    10f00 <fast_sinv+0x50>
 	push   %r13
 	mov    %rdx,%r13
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	movslq %esi,%rbp
 	push   %rbx
@@ -13270,30 +13264,30 @@
 	sub    $0x8,%rsp
 	nopl   0x0(%rax)
 	movsd  (%r12,%rbx,8),%xmm0
 	call   3220 <fast_sin@plt>
 	movsd  %xmm0,0x0(%r13,%rbx,8)
 	add    $0x1,%rbx
 	cmp    %rbx,%rbp
-	jne    10f10 <fast_sinv+0x20>
+	jne    10ed0 <fast_sinv+0x20>
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
-0000000000010f50 <fast_cosv>:
+0000000000010f10 <fast_cosv>:
 fast_cosv():
 	test   %esi,%esi
-	jle    10fa0 <fast_cosv+0x50>
+	jle    10f60 <fast_cosv+0x50>
 	push   %r13
 	mov    %rdx,%r13
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	movslq %esi,%rbp
 	push   %rbx
@@ -13301,30 +13295,30 @@
 	sub    $0x8,%rsp
 	nopl   0x0(%rax)
 	movsd  (%r12,%rbx,8),%xmm0
 	call   3050 <fast_cos@plt>
 	movsd  %xmm0,0x0(%r13,%rbx,8)
 	add    $0x1,%rbx
 	cmp    %rbx,%rbp
-	jne    10f70 <fast_cosv+0x20>
+	jne    10f30 <fast_cosv+0x20>
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
-0000000000010fb0 <fast_expv>:
+0000000000010f70 <fast_expv>:
 fast_expv():
 	test   %esi,%esi
-	jle    11000 <fast_expv+0x50>
+	jle    10fc0 <fast_expv+0x50>
 	push   %r13
 	mov    %rdx,%r13
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	movslq %esi,%rbp
 	push   %rbx
@@ -13332,30 +13326,30 @@
 	sub    $0x8,%rsp
 	nopl   0x0(%rax)
 	movsd  (%r12,%rbx,8),%xmm0
 	call   3170 <fast_exp@plt>
 	movsd  %xmm0,0x0(%r13,%rbx,8)
 	add    $0x1,%rbx
 	cmp    %rbx,%rbp
-	jne    10fd0 <fast_expv+0x20>
+	jne    10f90 <fast_expv+0x20>
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
-0000000000011010 <fast_sinvf>:
+0000000000010fd0 <fast_sinvf>:
 fast_sinvf():
 	test   %esi,%esi
-	jle    11060 <fast_sinvf+0x50>
+	jle    11020 <fast_sinvf+0x50>
 	push   %r13
 	mov    %rdx,%r13
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	movslq %esi,%rbp
 	push   %rbx
@@ -13365,30 +13359,30 @@
 	pxor   %xmm0,%xmm0
 	cvtss2sd (%r12,%rbx,4),%xmm0
 	call   3220 <fast_sin@plt>
 	cvtsd2ss %xmm0,%xmm0
 	movss  %xmm0,0x0(%r13,%rbx,4)
 	add    $0x1,%rbx
 	cmp    %rbx,%rbp
-	jne    11030 <fast_sinvf+0x20>
+	jne    10ff0 <fast_sinvf+0x20>
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	xchg   %ax,%ax
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
-0000000000011070 <fast_cosvf>:
+0000000000011030 <fast_cosvf>:
 fast_cosvf():
 	test   %esi,%esi
-	jle    110c0 <fast_cosvf+0x50>
+	jle    11080 <fast_cosvf+0x50>
 	push   %r13
 	mov    %rdx,%r13
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	movslq %esi,%rbp
 	push   %rbx
@@ -13398,30 +13392,30 @@
 	pxor   %xmm0,%xmm0
 	cvtss2sd (%r12,%rbx,4),%xmm0
 	call   3050 <fast_cos@plt>
 	cvtsd2ss %xmm0,%xmm0
 	movss  %xmm0,0x0(%r13,%rbx,4)
 	add    $0x1,%rbx
 	cmp    %rbx,%rbp
-	jne    11090 <fast_cosvf+0x20>
+	jne    11050 <fast_cosvf+0x20>
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	xchg   %ax,%ax
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
-00000000000110d0 <fast_expvf>:
+0000000000011090 <fast_expvf>:
 fast_expvf():
 	test   %esi,%esi
-	jle    11120 <fast_expvf+0x50>
+	jle    110e0 <fast_expvf+0x50>
 	push   %r13
 	mov    %rdx,%r13
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	movslq %esi,%rbp
 	push   %rbx
@@ -13431,344 +13425,344 @@
 	pxor   %xmm0,%xmm0
 	cvtss2sd (%r12,%rbx,4),%xmm0
 	call   3170 <fast_exp@plt>
 	cvtsd2ss %xmm0,%xmm0
 	movss  %xmm0,0x0(%r13,%rbx,4)
 	add    $0x1,%rbx
 	cmp    %rbx,%rbp
-	jne    110f0 <fast_expvf+0x20>
+	jne    110b0 <fast_expvf+0x20>
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	xchg   %ax,%ax
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
-0000000000011130 <interp>:
+00000000000110f0 <interp>:
 interp():
 	test   %esi,%esi
-	jle    11221 <interp+0xf1>
+	jle    111e1 <interp+0xf1>
 	lea    -0x1(%rsi),%eax
 	push   %rbp
 	mov    %rdx,%r10
 	mov    %ecx,%r11d
 	push   %rbx
 	movapd %xmm0,%xmm4
 	mov    %r8,%rbx
 	movslq %ecx,%rbp
 	lea    0x8(%rdi,%rax,8),%r8
 	nopw   0x0(%rax,%rax,1)
 	mov    %rbp,%rax
 	mov    %r10,%rsi
 	xchg   %ax,%ax
 	test   %rax,%rax
-	jle    11189 <interp+0x59>
+	jle    11149 <interp+0x59>
 	mov    %rax,%rdx
 	movsd  (%rdi),%xmm0
 	sar    %rdx
 	lea    (%rsi,%rdx,8),%rcx
 	comisd (%rcx),%xmm0
-	jbe    111d0 <interp+0xa0>
+	jbe    11190 <interp+0xa0>
 	sub    %rdx,%rax
 	lea    0x8(%rcx),%rsi
 	sub    $0x1,%rax
 	test   %rax,%rax
-	jg     11165 <interp+0x35>
+	jg     11125 <interp+0x35>
 	sub    %r10,%rsi
 	sar    $0x3,%rsi
 	cmp    %esi,%r11d
-	je     111d8 <interp+0xa8>
+	je     11198 <interp+0xa8>
 	movslq %esi,%rax
 	movsd  (%rdi),%xmm2
 	movsd  (%r10,%rax,8),%xmm0
 	lea    0x0(,%rax,8),%rdx
 	comisd %xmm2,%xmm0
-	jne    111e0 <interp+0xb0>
+	jne    111a0 <interp+0xb0>
 	movsd  (%rbx,%rax,8),%xmm0
 	movsd  %xmm0,(%r9)
 	add    $0x8,%rdi
 	add    $0x8,%r9
 	cmp    %r8,%rdi
-	jne    11158 <interp+0x28>
+	jne    11118 <interp+0x28>
 	pop    %rbx
 	pop    %rbp
 	ret
 	nopw   0x0(%rax,%rax,1)
 	mov    %rdx,%rax
-	jmp    11160 <interp+0x30>
+	jmp    11120 <interp+0x30>
 	nopl   (%rax)
 	movsd  %xmm1,(%r9)
-	jmp    111ba <interp+0x8a>
+	jmp    1117a <interp+0x8a>
 	nop
 	test   %esi,%esi
-	jne    111f0 <interp+0xc0>
+	jne    111b0 <interp+0xc0>
 	movsd  %xmm4,(%r9)
-	jmp    111ba <interp+0x8a>
+	jmp    1117a <interp+0x8a>
 	nopl   0x0(%rax,%rax,1)
 	movsd  -0x8(%rbx,%rdx,1),%xmm5
 	movsd  -0x8(%r10,%rdx,1),%xmm6
 	movsd  (%rbx,%rax,8),%xmm3
 	subsd  %xmm6,%xmm2
 	subsd  %xmm6,%xmm0
 	subsd  %xmm5,%xmm3
 	mulsd  %xmm3,%xmm2
 	divsd  %xmm0,%xmm2
 	addsd  %xmm5,%xmm2
 	movsd  %xmm2,(%r9)
-	jmp    111ba <interp+0x8a>
+	jmp    1117a <interp+0x8a>
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-0000000000011230 <interpf>:
+00000000000111f0 <interpf>:
 interpf():
 	test   %esi,%esi
-	jle    11321 <interpf+0xf1>
+	jle    112e1 <interpf+0xf1>
 	lea    -0x1(%rsi),%eax
 	push   %rbp
 	mov    %rdx,%r10
 	mov    %ecx,%r11d
 	push   %rbx
 	movaps %xmm0,%xmm4
 	mov    %r8,%rbx
 	movslq %ecx,%rbp
 	lea    0x4(%rdi,%rax,4),%r8
 	nopl   0x0(%rax)
 	mov    %rbp,%rax
 	mov    %r10,%rsi
 	xchg   %ax,%ax
 	test   %rax,%rax
-	jle    11288 <interpf+0x58>
+	jle    11248 <interpf+0x58>
 	mov    %rax,%rdx
 	movss  (%rdi),%xmm0
 	sar    %rdx
 	lea    (%rsi,%rdx,4),%rcx
 	comiss (%rcx),%xmm0
-	jbe    112d0 <interpf+0xa0>
+	jbe    11290 <interpf+0xa0>
 	sub    %rdx,%rax
 	lea    0x4(%rcx),%rsi
 	sub    $0x1,%rax
 	test   %rax,%rax
-	jg     11265 <interpf+0x35>
+	jg     11225 <interpf+0x35>
 	sub    %r10,%rsi
 	sar    $0x2,%rsi
 	cmp    %esi,%r11d
-	je     112d8 <interpf+0xa8>
+	je     11298 <interpf+0xa8>
 	movslq %esi,%rax
 	movss  (%rdi),%xmm2
 	movss  (%r10,%rax,4),%xmm0
 	lea    0x0(,%rax,4),%rdx
 	comiss %xmm2,%xmm0
-	jne    112e0 <interpf+0xb0>
+	jne    112a0 <interpf+0xb0>
 	movss  (%rbx,%rax,4),%xmm0
 	movss  %xmm0,(%r9)
 	add    $0x4,%rdi
 	add    $0x4,%r9
 	cmp    %r8,%rdi
-	jne    11258 <interpf+0x28>
+	jne    11218 <interpf+0x28>
 	pop    %rbx
 	pop    %rbp
 	ret
 	nopl   0x0(%rax,%rax,1)
 	mov    %rdx,%rax
-	jmp    11260 <interpf+0x30>
+	jmp    11220 <interpf+0x30>
 	nopl   (%rax)
 	movss  %xmm1,(%r9)
-	jmp    112b8 <interpf+0x88>
+	jmp    11278 <interpf+0x88>
 	nop
 	test   %esi,%esi
-	jne    112f0 <interpf+0xc0>
+	jne    112b0 <interpf+0xc0>
 	movss  %xmm4,(%r9)
-	jmp    112b8 <interpf+0x88>
+	jmp    11278 <interpf+0x88>
 	nopl   0x0(%rax,%rax,1)
 	movss  -0x4(%rbx,%rdx,1),%xmm5
 	movss  -0x4(%r10,%rdx,1),%xmm6
 	movss  (%rbx,%rax,4),%xmm3
 	subss  %xmm6,%xmm2
 	subss  %xmm6,%xmm0
 	subss  %xmm5,%xmm3
 	mulss  %xmm3,%xmm2
 	divss  %xmm0,%xmm2
 	addss  %xmm5,%xmm2
 	movss  %xmm2,(%r9)
-	jmp    112b8 <interpf+0x88>
+	jmp    11278 <interpf+0x88>
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-0000000000011330 <interp_const_space>:
+00000000000112f0 <interp_const_space>:
 interp_const_space():
 	push   %rbp
 	mov    %rdi,%rbp
 	movslq %ecx,%rax
 	movapd %xmm0,%xmm4
 	movsd  0x0(%rbp),%xmm0
 	mov    %esi,%edi
 	mov    %rdx,%r11
 	mov    %rax,%r10
 	mov    %rdx,%rsi
 	nopl   0x0(%rax,%rax,1)
 	test   %rax,%rax
-	jle    11379 <interp_const_space+0x49>
+	jle    11339 <interp_const_space+0x49>
 	mov    %rax,%rdx
 	sar    %rdx
 	lea    (%rsi,%rdx,8),%rcx
 	comisd (%rcx),%xmm0
-	jbe    11410 <interp_const_space+0xe0>
+	jbe    113d0 <interp_const_space+0xe0>
 	sub    %rdx,%rax
 	lea    0x8(%rcx),%rsi
 	sub    $0x1,%rax
 	test   %rax,%rax
-	jg     11355 <interp_const_space+0x25>
+	jg     11315 <interp_const_space+0x25>
 	sub    %r11,%rsi
 	mov    $0x1,%eax
 	movsd  (%r11),%xmm5
 	movsd  0x8(%r11),%xmm3
 	sar    $0x3,%rsi
 	pxor   %xmm2,%xmm2
 	sub    %esi,%eax
 	subsd  %xmm5,%xmm3
 	subsd  %xmm5,%xmm0
 	cvtsi2sd %eax,%xmm2
 	mulsd  %xmm3,%xmm2
 	addsd  %xmm0,%xmm2
 	divsd  %xmm3,%xmm2
 	test   %edi,%edi
-	jle    11407 <interp_const_space+0xd7>
+	jle    113c7 <interp_const_space+0xd7>
 	movslq %esi,%rdx
 	mov    %esi,%eax
 	add    %edi,%esi
 	lea    (%r8,%rdx,8),%rdx
-	jmp    113d4 <interp_const_space+0xa4>
+	jmp    11394 <interp_const_space+0xa4>
 	nop
 	movsd  %xmm1,(%r9)
 	add    $0x1,%eax
 	add    $0x8,%r9
 	add    $0x8,%rdx
 	cmp    %eax,%esi
-	je     11407 <interp_const_space+0xd7>
+	je     113c7 <interp_const_space+0xd7>
 	cmp    %eax,%r10d
-	jle    113c0 <interp_const_space+0x90>
+	jle    11380 <interp_const_space+0x90>
 	test   %eax,%eax
-	je     11420 <interp_const_space+0xf0>
+	je     113e0 <interp_const_space+0xf0>
 	movsd  -0x8(%rdx),%xmm3
 	movsd  (%rdx),%xmm0
 	add    $0x1,%eax
 	add    $0x8,%r9
 	add    $0x8,%rdx
 	subsd  %xmm3,%xmm0
 	mulsd  %xmm2,%xmm0
 	addsd  %xmm3,%xmm0
 	movsd  %xmm0,-0x8(%r9)
 	cmp    %eax,%esi
-	jne    113d4 <interp_const_space+0xa4>
+	jne    11394 <interp_const_space+0xa4>
 	pop    %rbp
 	ret
 	nopl   0x0(%rax)
 	mov    %rdx,%rax
-	jmp    11350 <interp_const_space+0x20>
+	jmp    11310 <interp_const_space+0x20>
 	nopl   0x0(%rax,%rax,1)
 	movsd  %xmm4,(%r9)
-	jmp    113c5 <interp_const_space+0x95>
+	jmp    11385 <interp_const_space+0x95>
 	nopw   0x0(%rax,%rax,1)
 
-0000000000011430 <interp_const_spacef>:
+00000000000113f0 <interp_const_spacef>:
 interp_const_spacef():
 	push   %rbp
 	mov    %rdi,%rbp
 	movslq %ecx,%rax
 	movaps %xmm0,%xmm4
 	movss  0x0(%rbp),%xmm0
 	mov    %esi,%edi
 	mov    %rdx,%r11
 	mov    %rax,%r10
 	mov    %rdx,%rsi
 	nopw   0x0(%rax,%rax,1)
 	test   %rax,%rax
-	jle    11478 <interp_const_spacef+0x48>
+	jle    11438 <interp_const_spacef+0x48>
 	mov    %rax,%rdx
 	sar    %rdx
 	lea    (%rsi,%rdx,4),%rcx
 	comiss (%rcx),%xmm0
-	jbe    11510 <interp_const_spacef+0xe0>
+	jbe    114d0 <interp_const_spacef+0xe0>
 	sub    %rdx,%rax
 	lea    0x4(%rcx),%rsi
 	sub    $0x1,%rax
 	test   %rax,%rax
-	jg     11455 <interp_const_spacef+0x25>
+	jg     11415 <interp_const_spacef+0x25>
 	sub    %r11,%rsi
 	mov    $0x1,%eax
 	movss  (%r11),%xmm5
 	movss  0x4(%r11),%xmm3
 	sar    $0x2,%rsi
 	pxor   %xmm2,%xmm2
 	sub    %esi,%eax
 	subss  %xmm5,%xmm3
 	subss  %xmm5,%xmm0
 	cvtsi2ss %eax,%xmm2
 	mulss  %xmm3,%xmm2
 	addss  %xmm0,%xmm2
 	divss  %xmm3,%xmm2
 	test   %edi,%edi
-	jle    11507 <interp_const_spacef+0xd7>
+	jle    114c7 <interp_const_spacef+0xd7>
 	movslq %esi,%rdx
 	mov    %esi,%eax
 	add    %edi,%esi
 	lea    (%r8,%rdx,4),%rdx
-	jmp    114d4 <interp_const_spacef+0xa4>
+	jmp    11494 <interp_const_spacef+0xa4>
 	xchg   %ax,%ax
 	movss  %xmm1,(%r9)
 	add    $0x1,%eax
 	add    $0x4,%r9
 	add    $0x4,%rdx
 	cmp    %eax,%esi
-	je     11507 <interp_const_spacef+0xd7>
+	je     114c7 <interp_const_spacef+0xd7>
 	cmp    %eax,%r10d
-	jle    114c0 <interp_const_spacef+0x90>
+	jle    11480 <interp_const_spacef+0x90>
 	test   %eax,%eax
-	je     11520 <interp_const_spacef+0xf0>
+	je     114e0 <interp_const_spacef+0xf0>
 	movss  -0x4(%rdx),%xmm3
 	movss  (%rdx),%xmm0
 	add    $0x1,%eax
 	add    $0x4,%r9
 	add    $0x4,%rdx
 	subss  %xmm3,%xmm0
 	mulss  %xmm2,%xmm0
 	addss  %xmm3,%xmm0
 	movss  %xmm0,-0x4(%r9)
 	cmp    %eax,%esi
-	jne    114d4 <interp_const_spacef+0xa4>
+	jne    11494 <interp_const_spacef+0xa4>
 	pop    %rbp
 	ret
 	nopl   0x0(%rax)
 	mov    %rdx,%rax
-	jmp    11450 <interp_const_spacef+0x20>
+	jmp    11410 <interp_const_spacef+0x20>
 	nopl   0x0(%rax,%rax,1)
 	movss  %xmm4,(%r9)
-	jmp    114c5 <interp_const_spacef+0x95>
+	jmp    11485 <interp_const_spacef+0x95>
 	nopw   0x0(%rax,%rax,1)
 
-0000000000011530 <cumtrapz_wo_initial>:
+00000000000114f0 <cumtrapz_wo_initial>:
 cumtrapz_wo_initial():
-	movsd  0x6d98(%rip),%xmm1        
+	movsd  0x6dd8(%rip),%xmm1        
 	movsd  0x8(%rdi),%xmm3
 	lea    -0x1(%rsi),%ecx
 	mulsd  %xmm0,%xmm1
 	movsd  (%rdi),%xmm0
 	addsd  %xmm3,%xmm0
 	mulsd  %xmm1,%xmm0
 	movsd  %xmm0,(%rdx)
 	cmp    $0x1,%ecx
-	jle    115d2 <cumtrapz_wo_initial+0xa2>
+	jle    11592 <cumtrapz_wo_initial+0xa2>
 	cmp    $0x4,%esi
-	jle    115d3 <cumtrapz_wo_initial+0xa3>
+	jle    11593 <cumtrapz_wo_initial+0xa3>
 	sub    $0x5,%esi
 	shr    %esi
 	lea    0x5(%rsi,%rsi,1),%r8
 	mov    $0x3,%esi
 	movsd  -0x8(%rdi,%rsi,8),%xmm4
 	movslq %esi,%rax
 	addsd  %xmm4,%xmm3
@@ -13780,42 +13774,42 @@
 	movapd %xmm4,%xmm0
 	mulsd  %xmm1,%xmm0
 	movsd  %xmm2,-0x10(%rdx,%rsi,8)
 	addsd  %xmm2,%xmm0
 	movsd  %xmm0,-0x8(%rdx,%rsi,8)
 	add    $0x2,%rsi
 	cmp    %r8,%rsi
-	jne    1156d <cumtrapz_wo_initial+0x3d>
+	jne    1152d <cumtrapz_wo_initial+0x3d>
 	movsd  (%rdi,%rax,8),%xmm0
 	addsd  0x8(%rdi,%rax,8),%xmm0
 	mulsd  %xmm1,%xmm0
 	addsd  -0x8(%rdx,%rax,8),%xmm0
 	movsd  %xmm0,(%rdx,%rax,8)
 	add    $0x1,%rax
 	cmp    %eax,%ecx
-	jg     115b0 <cumtrapz_wo_initial+0x80>
+	jg     11570 <cumtrapz_wo_initial+0x80>
 	ret
 	mov    $0x1,%eax
-	jmp    115b0 <cumtrapz_wo_initial+0x80>
+	jmp    11570 <cumtrapz_wo_initial+0x80>
 	nopw   0x0(%rax,%rax,1)
 
-00000000000115e0 <cumtrapz_w_initial>:
+00000000000115a0 <cumtrapz_w_initial>:
 cumtrapz_w_initial():
-	movsd  0x6ce8(%rip),%xmm2        
+	movsd  0x6d28(%rip),%xmm2        
 	movsd  0x8(%rdi),%xmm3
 	movsd  %xmm1,(%rdx)
 	mulsd  %xmm0,%xmm2
 	movsd  (%rdi),%xmm0
 	addsd  %xmm3,%xmm0
 	mulsd  %xmm2,%xmm0
 	movsd  %xmm0,0x8(%rdx)
 	cmp    $0x2,%esi
-	jle    1168a <cumtrapz_w_initial+0xaa>
+	jle    1164a <cumtrapz_w_initial+0xaa>
 	cmp    $0x4,%esi
-	jle    1168b <cumtrapz_w_initial+0xab>
+	jle    1164b <cumtrapz_w_initial+0xab>
 	lea    -0x5(%rsi),%eax
 	mov    $0x4,%ecx
 	shr    %eax
 	lea    0x3(%rax),%r8d
 	add    %r8,%r8
 	movsd  -0x10(%rdi,%rcx,8),%xmm4
 	movslq %ecx,%rax
@@ -13828,37 +13822,37 @@
 	movapd %xmm4,%xmm0
 	mulsd  %xmm2,%xmm0
 	movsd  %xmm1,-0x10(%rdx,%rcx,8)
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rdx,%rcx,8)
 	add    $0x2,%rcx
 	cmp    %r8,%rcx
-	jne    11621 <cumtrapz_w_initial+0x41>
+	jne    115e1 <cumtrapz_w_initial+0x41>
 	nopl   (%rax)
 	movsd  -0x8(%rdi,%rax,8),%xmm0
 	addsd  (%rdi,%rax,8),%xmm0
 	mulsd  %xmm2,%xmm0
 	addsd  -0x8(%rdx,%rax,8),%xmm0
 	movsd  %xmm0,(%rdx,%rax,8)
 	add    $0x1,%rax
 	cmp    %eax,%esi
-	jg     11668 <cumtrapz_w_initial+0x88>
+	jg     11628 <cumtrapz_w_initial+0x88>
 	ret
 	mov    $0x2,%eax
-	jmp    11668 <cumtrapz_w_initial+0x88>
+	jmp    11628 <cumtrapz_w_initial+0x88>
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-00000000000116a0 <trapz_var_delta>:
+0000000000011660 <trapz_var_delta>:
 trapz_var_delta():
 	cmp    $0x1,%edx
-	jle    11740 <trapz_var_delta+0xa0>
+	jle    11700 <trapz_var_delta+0xa0>
 	lea    -0x1(%rdx),%ecx
 	cmp    $0x2,%edx
-	je     11745 <trapz_var_delta+0xa5>
+	je     11705 <trapz_var_delta+0xa5>
 	mov    %ecx,%edx
 	xor    %eax,%eax
 	pxor   %xmm3,%xmm3
 	shr    %edx
 	shl    $0x4,%rdx
 	nopl   0x0(%rax,%rax,1)
 	movupd 0x8(%rdi,%rax,1),%xmm0
@@ -13867,177 +13861,177 @@
 	movupd (%rsi,%rax,1),%xmm5
 	add    $0x10,%rax
 	addpd  %xmm4,%xmm0
 	subpd  %xmm5,%xmm1
 	mulpd  %xmm1,%xmm0
 	addpd  %xmm0,%xmm3
 	cmp    %rax,%rdx
-	jne    116c8 <trapz_var_delta+0x28>
+	jne    11688 <trapz_var_delta+0x28>
 	mov    %ecx,%eax
 	movapd %xmm3,%xmm2
 	unpckhpd %xmm3,%xmm2
 	or     $0x1,%eax
 	and    $0x1,%ecx
 	addpd  %xmm3,%xmm2
-	je     1172d <trapz_var_delta+0x8d>
+	je     116ed <trapz_var_delta+0x8d>
 	cltq
 	movsd  (%rsi,%rax,8),%xmm0
 	movsd  -0x8(%rdi,%rax,8),%xmm1
 	subsd  -0x8(%rsi,%rax,8),%xmm0
 	addsd  (%rdi,%rax,8),%xmm1
 	mulsd  %xmm1,%xmm0
 	addsd  %xmm0,%xmm2
-	mulsd  0x6b9b(%rip),%xmm2        
+	mulsd  0x6bdb(%rip),%xmm2        
 	movapd %xmm2,%xmm0
 	ret
 	nopw   0x0(%rax,%rax,1)
 	pxor   %xmm0,%xmm0
 	ret
 	mov    $0x1,%eax
 	pxor   %xmm2,%xmm2
-	jmp    1170d <trapz_var_delta+0x6d>
+	jmp    116cd <trapz_var_delta+0x6d>
 
-0000000000011750 <trapz_const_delta>:
+0000000000011710 <trapz_const_delta>:
 trapz_const_delta():
 	movslq %esi,%rax
 	lea    -0x1(%rsi),%ecx
 	movapd %xmm0,%xmm2
 	movsd  -0x8(%rdi,%rax,8),%xmm1
 	addsd  (%rdi),%xmm1
-	mulsd  0x6b64(%rip),%xmm1        
+	mulsd  0x6ba4(%rip),%xmm1        
 	cmp    $0x1,%ecx
-	jle    11802 <trapz_const_delta+0xb2>
+	jle    117c2 <trapz_const_delta+0xb2>
 	lea    -0x2(%rsi),%r8d
 	sub    $0x3,%esi
 	cmp    $0x3,%esi
-	jbe    1180b <trapz_const_delta+0xbb>
+	jbe    117cb <trapz_const_delta+0xbb>
 	mov    %r8d,%edx
 	mov    %rdi,%rax
 	pxor   %xmm0,%xmm0
 	shr    %edx
 	shl    $0x4,%rdx
 	add    %rdi,%rdx
 	nopl   0x0(%rax,%rax,1)
 	movupd 0x8(%rax),%xmm4
 	add    $0x10,%rax
 	addpd  %xmm4,%xmm0
 	cmp    %rdx,%rax
-	jne    117a0 <trapz_const_delta+0x50>
+	jne    11760 <trapz_const_delta+0x50>
 	movapd %xmm0,%xmm3
 	mov    %r8d,%eax
 	unpckhpd %xmm0,%xmm3
 	or     $0x1,%eax
 	and    $0x1,%r8d
 	addpd  %xmm3,%xmm0
 	addsd  %xmm0,%xmm1
-	je     11802 <trapz_const_delta+0xb2>
+	je     117c2 <trapz_const_delta+0xb2>
 	movslq %eax,%rdx
 	addsd  (%rdi,%rdx,8),%xmm1
 	lea    0x1(%rax),%edx
 	cmp    %ecx,%edx
-	jge    11802 <trapz_const_delta+0xb2>
+	jge    117c2 <trapz_const_delta+0xb2>
 	movslq %edx,%rdx
 	addsd  (%rdi,%rdx,8),%xmm1
 	lea    0x2(%rax),%edx
 	cmp    %edx,%ecx
-	jle    11802 <trapz_const_delta+0xb2>
+	jle    117c2 <trapz_const_delta+0xb2>
 	movslq %edx,%rdx
 	add    $0x3,%eax
 	addsd  (%rdi,%rdx,8),%xmm1
 	cmp    %eax,%ecx
-	jle    11802 <trapz_const_delta+0xb2>
+	jle    117c2 <trapz_const_delta+0xb2>
 	cltq
 	addsd  (%rdi,%rax,8),%xmm1
 	mulsd  %xmm1,%xmm2
 	movapd %xmm2,%xmm0
 	ret
 	mov    $0x1,%eax
-	jmp    117ce <trapz_const_delta+0x7e>
+	jmp    1178e <trapz_const_delta+0x7e>
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-0000000000011820 <min_idx>:
+00000000000117e0 <min_idx>:
 min_idx():
 	movslq %esi,%rsi
 	lea    (%rdi,%rsi,8),%rcx
 	cmp    %rdi,%rcx
-	je     11868 <min_idx+0x48>
+	je     11828 <min_idx+0x48>
 	lea    0x8(%rdi),%rax
 	cmp    %rax,%rcx
-	je     11868 <min_idx+0x48>
+	je     11828 <min_idx+0x48>
 	movsd  (%rdi),%xmm0
 	mov    %rdi,%rdx
 	nopl   0x0(%rax)
 	movsd  (%rax),%xmm1
 	comisd %xmm1,%xmm0
 	minsd  %xmm1,%xmm0
 	cmova  %rax,%rdx
 	add    $0x8,%rax
 	cmp    %rax,%rcx
-	jne    11840 <min_idx+0x20>
+	jne    11800 <min_idx+0x20>
 	mov    %rdx,%rax
 	sub    %rdi,%rax
 	sar    $0x3,%rax
 	ret
 	nopl   0x0(%rax)
 	xor    %eax,%eax
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-0000000000011870 <max_idx>:
+0000000000011830 <max_idx>:
 max_idx():
 	movslq %esi,%rsi
 	lea    (%rdi,%rsi,8),%rcx
 	cmp    %rdi,%rcx
-	je     118b8 <max_idx+0x48>
+	je     11878 <max_idx+0x48>
 	lea    0x8(%rdi),%rax
 	cmp    %rax,%rcx
-	je     118b8 <max_idx+0x48>
+	je     11878 <max_idx+0x48>
 	movsd  (%rdi),%xmm0
 	mov    %rdi,%rdx
 	nopl   0x0(%rax)
 	movsd  (%rax),%xmm1
 	comisd %xmm0,%xmm1
 	maxsd  %xmm1,%xmm0
 	cmova  %rax,%rdx
 	add    $0x8,%rax
 	cmp    %rax,%rcx
-	jne    11890 <max_idx+0x20>
+	jne    11850 <max_idx+0x20>
 	mov    %rdx,%rax
 	sub    %rdi,%rax
 	sar    $0x3,%rax
 	ret
 	nopl   0x0(%rax)
 	xor    %eax,%eax
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-00000000000118c0 <linspace>:
+0000000000011880 <linspace>:
 linspace():
 	subsd  %xmm0,%xmm1
 	movapd %xmm0,%xmm6
 	lea    -0x1(%rdi),%eax
 	pxor   %xmm0,%xmm0
 	cvtsi2sd %eax,%xmm0
 	movapd %xmm1,%xmm5
 	divsd  %xmm0,%xmm5
 	test   %edi,%edi
-	jle    119b7 <linspace+0xf7>
+	jle    11977 <linspace+0xf7>
 	cmp    $0x2,%eax
-	jbe    119c1 <linspace+0x101>
+	jbe    11981 <linspace+0x101>
 	mov    %edi,%edx
 	movapd %xmm5,%xmm4
 	movapd %xmm6,%xmm3
 	mov    %rsi,%rax
 	shr    $0x2,%edx
-	movdqa 0x6adc(%rip),%xmm2        
+	movdqa 0x6b1c(%rip),%xmm2        
 	unpcklpd %xmm4,%xmm4
 	unpcklpd %xmm3,%xmm3
 	shl    $0x5,%rdx
-	movdqa 0x6828(%rip),%xmm7        
+	movdqa 0x6868(%rip),%xmm7        
 	add    %rsi,%rdx
 	nopl   0x0(%rax,%rax,1)
 	movdqa %xmm2,%xmm0
 	add    $0x20,%rax
 	paddd  %xmm7,%xmm2
 	cvtdq2pd %xmm0,%xmm1
 	mulpd  %xmm4,%xmm1
@@ -14045,76 +14039,76 @@
 	cvtdq2pd %xmm0,%xmm0
 	mulpd  %xmm4,%xmm0
 	addpd  %xmm3,%xmm1
 	addpd  %xmm3,%xmm0
 	movups %xmm1,-0x20(%rax)
 	movups %xmm0,-0x10(%rax)
 	cmp    %rdx,%rax
-	jne    11920 <linspace+0x60>
+	jne    118e0 <linspace+0x60>
 	mov    %edi,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%dil
-	je     119c0 <linspace+0x100>
+	je     11980 <linspace+0x100>
 	pxor   %xmm0,%xmm0
 	movslq %eax,%rdx
 	cvtsi2sd %eax,%xmm0
 	mulsd  %xmm5,%xmm0
 	addsd  %xmm6,%xmm0
 	movsd  %xmm0,(%rsi,%rdx,8)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%edi
-	jle    119b7 <linspace+0xf7>
+	jle    11977 <linspace+0xf7>
 	pxor   %xmm0,%xmm0
 	movslq %edx,%rcx
 	add    $0x2,%eax
 	cvtsi2sd %edx,%xmm0
 	mulsd  %xmm5,%xmm0
 	addsd  %xmm6,%xmm0
 	movsd  %xmm0,(%rsi,%rcx,8)
 	cmp    %eax,%edi
-	jle    119b7 <linspace+0xf7>
+	jle    11977 <linspace+0xf7>
 	pxor   %xmm0,%xmm0
 	movslq %eax,%rdx
 	cvtsi2sd %eax,%xmm0
 	mulsd  %xmm0,%xmm5
 	addsd  %xmm6,%xmm5
 	movsd  %xmm5,(%rsi,%rdx,8)
 	ret
 	nopl   0x0(%rax,%rax,1)
 	ret
 	xor    %eax,%eax
-	jmp    11961 <linspace+0xa1>
+	jmp    11921 <linspace+0xa1>
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-00000000000119d0 <arange_double>:
+0000000000011990 <arange_double>:
 arange_double():
 	subsd  %xmm0,%xmm1
 	movapd %xmm0,%xmm6
 	pxor   %xmm0,%xmm0
 	divsd  %xmm2,%xmm1
 	cvttsd2si %xmm1,%edx
 	cvtsi2sd %edx,%xmm0
 	lea    0x1(%rdx),%eax
 	comisd %xmm0,%xmm1
 	cmova  %eax,%edx
 	test   %edx,%edx
-	jle    11ace <arange_double+0xfe>
+	jle    11a8e <arange_double+0xfe>
 	lea    -0x1(%rdx),%eax
 	cmp    $0x2,%eax
-	jbe    11ad1 <arange_double+0x101>
+	jbe    11a91 <arange_double+0x101>
 	mov    %edx,%ecx
 	movapd %xmm2,%xmm5
 	movapd %xmm6,%xmm4
 	mov    %rdi,%rax
 	shr    $0x2,%ecx
-	movdqa 0x69c2(%rip),%xmm3        
+	movdqa 0x6a02(%rip),%xmm3        
 	unpcklpd %xmm5,%xmm5
 	unpcklpd %xmm4,%xmm4
 	shl    $0x5,%rcx
-	movdqa 0x670e(%rip),%xmm7        
+	movdqa 0x674e(%rip),%xmm7        
 	add    %rdi,%rcx
 	nopl   (%rax)
 	movdqa %xmm3,%xmm0
 	add    $0x20,%rax
 	paddd  %xmm7,%xmm3
 	cvtdq2pd %xmm0,%xmm1
 	mulpd  %xmm5,%xmm1
@@ -14122,64 +14116,64 @@
 	cvtdq2pd %xmm0,%xmm0
 	mulpd  %xmm5,%xmm0
 	addpd  %xmm4,%xmm1
 	addpd  %xmm4,%xmm0
 	movups %xmm1,-0x20(%rax)
 	movups %xmm0,-0x10(%rax)
 	cmp    %rcx,%rax
-	jne    11a38 <arange_double+0x68>
+	jne    119f8 <arange_double+0x68>
 	mov    %edx,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%dl
-	je     11ad0 <arange_double+0x100>
+	je     11a90 <arange_double+0x100>
 	pxor   %xmm0,%xmm0
 	movslq %eax,%rcx
 	cvtsi2sd %eax,%xmm0
 	mulsd  %xmm2,%xmm0
 	addsd  %xmm6,%xmm0
 	movsd  %xmm0,(%rdi,%rcx,8)
 	lea    0x1(%rax),%ecx
 	cmp    %ecx,%edx
-	jle    11ace <arange_double+0xfe>
+	jle    11a8e <arange_double+0xfe>
 	pxor   %xmm0,%xmm0
 	movslq %ecx,%rsi
 	add    $0x2,%eax
 	cvtsi2sd %ecx,%xmm0
 	mulsd  %xmm2,%xmm0
 	addsd  %xmm6,%xmm0
 	movsd  %xmm0,(%rdi,%rsi,8)
 	cmp    %eax,%edx
-	jle    11ace <arange_double+0xfe>
+	jle    11a8e <arange_double+0xfe>
 	pxor   %xmm0,%xmm0
 	movslq %eax,%rdx
 	cvtsi2sd %eax,%xmm0
 	mulsd  %xmm0,%xmm2
 	addsd  %xmm6,%xmm2
 	movsd  %xmm2,(%rdi,%rdx,8)
 	ret
 	nop
 	ret
 	xor    %eax,%eax
-	jmp    11a78 <arange_double+0xa8>
+	jmp    11a38 <arange_double+0xa8>
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-0000000000011ae0 <cumtrapz_wo_initialf>:
+0000000000011aa0 <cumtrapz_wo_initialf>:
 cumtrapz_wo_initialf():
-	movss  0x680c(%rip),%xmm1        
+	movss  0x684c(%rip),%xmm1        
 	movss  0x4(%rdi),%xmm3
 	lea    -0x1(%rsi),%ecx
 	mulss  %xmm0,%xmm1
 	movss  (%rdi),%xmm0
 	addss  %xmm3,%xmm0
 	mulss  %xmm1,%xmm0
 	movss  %xmm0,(%rdx)
 	cmp    $0x1,%ecx
-	jle    11b82 <cumtrapz_wo_initialf+0xa2>
+	jle    11b42 <cumtrapz_wo_initialf+0xa2>
 	cmp    $0x4,%esi
-	jle    11b83 <cumtrapz_wo_initialf+0xa3>
+	jle    11b43 <cumtrapz_wo_initialf+0xa3>
 	sub    $0x5,%esi
 	shr    %esi
 	lea    0x5(%rsi,%rsi,1),%r8
 	mov    $0x3,%esi
 	movss  -0x4(%rdi,%rsi,4),%xmm4
 	movslq %esi,%rax
 	addss  %xmm4,%xmm3
@@ -14191,43 +14185,43 @@
 	movaps %xmm4,%xmm0
 	mulss  %xmm1,%xmm0
 	movss  %xmm2,-0x8(%rdx,%rsi,4)
 	addss  %xmm2,%xmm0
 	movss  %xmm0,-0x4(%rdx,%rsi,4)
 	add    $0x2,%rsi
 	cmp    %r8,%rsi
-	jne    11b1d <cumtrapz_wo_initialf+0x3d>
+	jne    11add <cumtrapz_wo_initialf+0x3d>
 	xchg   %ax,%ax
 	movss  (%rdi,%rax,4),%xmm0
 	addss  0x4(%rdi,%rax,4),%xmm0
 	mulss  %xmm1,%xmm0
 	addss  -0x4(%rdx,%rax,4),%xmm0
 	movss  %xmm0,(%rdx,%rax,4)
 	add    $0x1,%rax
 	cmp    %eax,%ecx
-	jg     11b60 <cumtrapz_wo_initialf+0x80>
+	jg     11b20 <cumtrapz_wo_initialf+0x80>
 	ret
 	mov    $0x1,%eax
-	jmp    11b60 <cumtrapz_wo_initialf+0x80>
+	jmp    11b20 <cumtrapz_wo_initialf+0x80>
 	nopw   0x0(%rax,%rax,1)
 
-0000000000011b90 <cumtrapz_w_initialf>:
+0000000000011b50 <cumtrapz_w_initialf>:
 cumtrapz_w_initialf():
-	movss  0x675c(%rip),%xmm2        
+	movss  0x679c(%rip),%xmm2        
 	movss  0x4(%rdi),%xmm3
 	movss  %xmm1,(%rdx)
 	mulss  %xmm0,%xmm2
 	movss  (%rdi),%xmm0
 	addss  %xmm3,%xmm0
 	mulss  %xmm2,%xmm0
 	movss  %xmm0,0x4(%rdx)
 	cmp    $0x2,%esi
-	jle    11c3a <cumtrapz_w_initialf+0xaa>
+	jle    11bfa <cumtrapz_w_initialf+0xaa>
 	cmp    $0x4,%esi
-	jle    11c3b <cumtrapz_w_initialf+0xab>
+	jle    11bfb <cumtrapz_w_initialf+0xab>
 	lea    -0x5(%rsi),%eax
 	mov    $0x4,%ecx
 	shr    %eax
 	lea    0x3(%rax),%r8d
 	add    %r8,%r8
 	movss  -0x8(%rdi,%rcx,4),%xmm4
 	movslq %ecx,%rax
@@ -14240,39 +14234,39 @@
 	movaps %xmm4,%xmm0
 	mulss  %xmm2,%xmm0
 	movss  %xmm1,-0x8(%rdx,%rcx,4)
 	addss  %xmm1,%xmm0
 	movss  %xmm0,-0x4(%rdx,%rcx,4)
 	add    $0x2,%rcx
 	cmp    %r8,%rcx
-	jne    11bd1 <cumtrapz_w_initialf+0x41>
+	jne    11b91 <cumtrapz_w_initialf+0x41>
 	nopl   0x0(%rax,%rax,1)
 	movss  -0x4(%rdi,%rax,4),%xmm0
 	addss  (%rdi,%rax,4),%xmm0
 	mulss  %xmm2,%xmm0
 	addss  -0x4(%rdx,%rax,4),%xmm0
 	movss  %xmm0,(%rdx,%rax,4)
 	add    $0x1,%rax
 	cmp    %eax,%esi
-	jg     11c18 <cumtrapz_w_initialf+0x88>
+	jg     11bd8 <cumtrapz_w_initialf+0x88>
 	ret
 	mov    $0x2,%eax
-	jmp    11c18 <cumtrapz_w_initialf+0x88>
+	jmp    11bd8 <cumtrapz_w_initialf+0x88>
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-0000000000011c50 <trapz_var_deltaf>:
+0000000000011c10 <trapz_var_deltaf>:
 trapz_var_deltaf():
 	mov    %edx,%ecx
 	cmp    $0x1,%edx
-	jle    11e60 <trapz_var_deltaf+0x210>
+	jle    11e20 <trapz_var_deltaf+0x210>
 	lea    -0x2(%rdx),%eax
 	lea    -0x1(%rdx),%r8d
 	cmp    $0x2,%eax
-	jbe    11e65 <trapz_var_deltaf+0x215>
+	jbe    11e25 <trapz_var_deltaf+0x215>
 	mov    %r8d,%edx
 	xor    %eax,%eax
 	pxor   %xmm2,%xmm2
 	shr    $0x2,%edx
 	shl    $0x4,%rdx
 	nopl   0x0(%rax,%rax,1)
 	movups (%rdi,%rax,1),%xmm0
@@ -14281,36 +14275,36 @@
 	movups (%rsi,%rax,1),%xmm7
 	add    $0x10,%rax
 	addps  %xmm6,%xmm0
 	subps  %xmm7,%xmm1
 	mulps  %xmm1,%xmm0
 	addps  %xmm0,%xmm2
 	cmp    %rdx,%rax
-	jne    11c80 <trapz_var_deltaf+0x30>
+	jne    11c40 <trapz_var_deltaf+0x30>
 	movaps %xmm2,%xmm0
 	mov    %r8d,%eax
 	movhlps %xmm2,%xmm0
 	and    $0xfffffffc,%eax
 	addps  %xmm0,%xmm2
 	lea    0x1(%rax),%edx
 	movaps %xmm2,%xmm0
 	shufps $0x55,%xmm2,%xmm0
 	addps  %xmm0,%xmm2
 	movaps %xmm2,%xmm0
 	cmp    %r8d,%eax
-	je     11db3 <trapz_var_deltaf+0x163>
+	je     11d73 <trapz_var_deltaf+0x163>
 	movslq %edx,%rax
 	lea    0x1(%rdx),%r11d
 	shl    $0x2,%rax
 	lea    (%rsi,%rax,1),%r9
 	lea    (%rdi,%rax,1),%r10
 	cmp    %r8d,%r11d
-	jge    11e73 <trapz_var_deltaf+0x223>
+	jge    11e33 <trapz_var_deltaf+0x223>
 	cmp    %edx,%ecx
-	jle    11e73 <trapz_var_deltaf+0x223>
+	jle    11e33 <trapz_var_deltaf+0x223>
 	movss  (%r9),%xmm4
 	movss  (%r10),%xmm1
 	movss  -0x4(%r10),%xmm2
 	movss  0x4(%rsi,%rax,1),%xmm5
 	movaps %xmm4,%xmm3
 	subss  -0x4(%r9),%xmm3
 	lea    0x3(%rdx),%r9d
@@ -14321,43 +14315,43 @@
 	addss  %xmm3,%xmm1
 	addss  %xmm0,%xmm2
 	movaps %xmm5,%xmm0
 	subss  %xmm4,%xmm0
 	mulss  %xmm1,%xmm0
 	addss  %xmm2,%xmm0
 	cmp    %r9d,%r8d
-	jg     11dc0 <trapz_var_deltaf+0x170>
+	jg     11d80 <trapz_var_deltaf+0x170>
 	movslq %eax,%rdx
 	movss  (%rdi,%rdx,4),%xmm1
 	movss  (%rsi,%rdx,4),%xmm2
 	addss  -0x4(%rdi,%rdx,4),%xmm1
 	subss  -0x4(%rsi,%rdx,4),%xmm2
 	lea    0x1(%rax),%edx
 	mulss  %xmm2,%xmm1
 	addss  %xmm1,%xmm0
 	cmp    %edx,%ecx
-	jle    11db3 <trapz_var_deltaf+0x163>
+	jle    11d73 <trapz_var_deltaf+0x163>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	movss  (%rdi,%rdx,4),%xmm1
 	movss  (%rsi,%rdx,4),%xmm2
 	addss  -0x4(%rdi,%rdx,4),%xmm1
 	subss  -0x4(%rsi,%rdx,4),%xmm2
 	mulss  %xmm2,%xmm1
 	addss  %xmm1,%xmm0
 	cmp    %eax,%ecx
-	jle    11db3 <trapz_var_deltaf+0x163>
+	jle    11d73 <trapz_var_deltaf+0x163>
 	cltq
 	movss  (%rdi,%rax,4),%xmm1
 	movss  (%rsi,%rax,4),%xmm2
 	addss  -0x4(%rdi,%rax,4),%xmm1
 	subss  -0x4(%rsi,%rax,4),%xmm2
 	mulss  %xmm2,%xmm1
 	addss  %xmm1,%xmm0
-	mulss  0x6539(%rip),%xmm0        
+	mulss  0x6579(%rip),%xmm0        
 	ret
 	nopl   0x0(%rax)
 	cltq
 	movss  (%rsi,%rax,4),%xmm4
 	movss  (%rdi,%rax,4),%xmm1
 	lea    0x0(,%rax,4),%r9
 	lea    0x4(%rdx),%eax
@@ -14371,321 +14365,321 @@
 	addss  %xmm2,%xmm1
 	addss  %xmm3,%xmm0
 	movaps %xmm5,%xmm3
 	subss  %xmm4,%xmm3
 	mulss  %xmm3,%xmm1
 	addss  %xmm1,%xmm0
 	cmp    %r9d,%r8d
-	jle    11d43 <trapz_var_deltaf+0xf3>
+	jle    11d03 <trapz_var_deltaf+0xf3>
 	cltq
 	movss  (%rsi,%rax,4),%xmm4
 	movss  (%rdi,%rax,4),%xmm1
 	movaps %xmm4,%xmm3
 	addss  %xmm1,%xmm2
 	addss  0x4(%rdi,%rax,4),%xmm1
 	subss  %xmm5,%xmm3
 	mulss  %xmm3,%xmm2
 	addss  %xmm0,%xmm2
 	movss  0x4(%rsi,%rax,4),%xmm0
 	lea    0x6(%rdx),%eax
 	subss  %xmm4,%xmm0
 	mulss  %xmm1,%xmm0
 	addss  %xmm2,%xmm0
-	jmp    11d43 <trapz_var_deltaf+0xf3>
+	jmp    11d03 <trapz_var_deltaf+0xf3>
 	nopw   0x0(%rax,%rax,1)
 	pxor   %xmm0,%xmm0
 	ret
 	mov    $0x1,%edx
 	pxor   %xmm0,%xmm0
-	jmp    11ccf <trapz_var_deltaf+0x7f>
+	jmp    11c8f <trapz_var_deltaf+0x7f>
 	mov    %edx,%eax
-	jmp    11d43 <trapz_var_deltaf+0xf3>
+	jmp    11d03 <trapz_var_deltaf+0xf3>
 	nopw   0x0(%rax,%rax,1)
 
-0000000000011e80 <trapz_const_deltaf>:
+0000000000011e40 <trapz_const_deltaf>:
 trapz_const_deltaf():
 	movslq %esi,%rax
 	lea    -0x1(%rsi),%ecx
 	movaps %xmm0,%xmm2
 	movss  -0x4(%rdi,%rax,4),%xmm1
 	addss  (%rdi),%xmm1
-	mulss  0x6459(%rip),%xmm1        
+	mulss  0x6499(%rip),%xmm1        
 	cmp    $0x1,%ecx
-	jle    11f1a <trapz_const_deltaf+0x9a>
+	jle    11eda <trapz_const_deltaf+0x9a>
 	lea    -0x2(%rsi),%r8d
 	sub    $0x3,%esi
 	cmp    $0x2,%esi
-	jbe    11f22 <trapz_const_deltaf+0xa2>
+	jbe    11ee2 <trapz_const_deltaf+0xa2>
 	mov    %r8d,%edx
 	mov    %rdi,%rax
 	pxor   %xmm0,%xmm0
 	shr    $0x2,%edx
 	shl    $0x4,%rdx
 	add    %rdi,%rdx
 	movups 0x4(%rax),%xmm4
 	add    $0x10,%rax
 	addps  %xmm4,%xmm0
 	cmp    %rdx,%rax
-	jne    11ec0 <trapz_const_deltaf+0x40>
+	jne    11e80 <trapz_const_deltaf+0x40>
 	movaps %xmm0,%xmm3
 	mov    %r8d,%edx
 	movhlps %xmm0,%xmm3
 	and    $0xfffffffc,%edx
 	addps  %xmm0,%xmm3
 	lea    0x1(%rdx),%eax
 	movaps %xmm3,%xmm0
 	shufps $0x55,%xmm3,%xmm0
 	addps  %xmm3,%xmm0
 	addss  %xmm0,%xmm1
 	cmp    %edx,%r8d
-	je     11f1a <trapz_const_deltaf+0x9a>
+	je     11eda <trapz_const_deltaf+0x9a>
 	movslq %eax,%rdx
 	addss  (%rdi,%rdx,4),%xmm1
 	lea    0x1(%rax),%edx
 	cmp    %ecx,%edx
-	jge    11f1a <trapz_const_deltaf+0x9a>
+	jge    11eda <trapz_const_deltaf+0x9a>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	addss  (%rdi,%rdx,4),%xmm1
 	cmp    %eax,%ecx
-	jle    11f1a <trapz_const_deltaf+0x9a>
+	jle    11eda <trapz_const_deltaf+0x9a>
 	cltq
 	addss  (%rdi,%rax,4),%xmm1
 	mulss  %xmm1,%xmm2
 	movaps %xmm2,%xmm0
 	ret
 	mov    $0x1,%eax
-	jmp    11ef5 <trapz_const_deltaf+0x75>
+	jmp    11eb5 <trapz_const_deltaf+0x75>
 	nopl   0x0(%rax)
 
-0000000000011f30 <min_idxf>:
+0000000000011ef0 <min_idxf>:
 min_idxf():
 	movslq %esi,%rsi
 	lea    (%rdi,%rsi,4),%rcx
 	cmp    %rdi,%rcx
-	je     11f78 <min_idxf+0x48>
+	je     11f38 <min_idxf+0x48>
 	lea    0x4(%rdi),%rax
 	cmp    %rax,%rcx
-	je     11f78 <min_idxf+0x48>
+	je     11f38 <min_idxf+0x48>
 	movss  (%rdi),%xmm0
 	mov    %rdi,%rdx
 	nopl   0x0(%rax)
 	movss  (%rax),%xmm1
 	comiss %xmm1,%xmm0
 	minss  %xmm1,%xmm0
 	cmova  %rax,%rdx
 	add    $0x4,%rax
 	cmp    %rax,%rcx
-	jne    11f50 <min_idxf+0x20>
+	jne    11f10 <min_idxf+0x20>
 	mov    %rdx,%rax
 	sub    %rdi,%rax
 	sar    $0x2,%rax
 	ret
 	nopl   0x0(%rax,%rax,1)
 	xor    %eax,%eax
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-0000000000011f80 <max_idxf>:
+0000000000011f40 <max_idxf>:
 max_idxf():
 	movslq %esi,%rsi
 	lea    (%rdi,%rsi,4),%rcx
 	cmp    %rdi,%rcx
-	je     11fc8 <max_idxf+0x48>
+	je     11f88 <max_idxf+0x48>
 	lea    0x4(%rdi),%rax
 	cmp    %rax,%rcx
-	je     11fc8 <max_idxf+0x48>
+	je     11f88 <max_idxf+0x48>
 	movss  (%rdi),%xmm0
 	mov    %rdi,%rdx
 	nopl   0x0(%rax)
 	movss  (%rax),%xmm1
 	comiss %xmm0,%xmm1
 	maxss  %xmm1,%xmm0
 	cmova  %rax,%rdx
 	add    $0x4,%rax
 	cmp    %rax,%rcx
-	jne    11fa0 <max_idxf+0x20>
+	jne    11f60 <max_idxf+0x20>
 	mov    %rdx,%rax
 	sub    %rdi,%rax
 	sar    $0x2,%rax
 	ret
 	nopl   0x0(%rax,%rax,1)
 	xor    %eax,%eax
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-0000000000011fd0 <linspacef>:
+0000000000011f90 <linspacef>:
 linspacef():
 	subss  %xmm0,%xmm1
 	movaps %xmm0,%xmm6
 	lea    -0x1(%rdi),%eax
 	pxor   %xmm0,%xmm0
 	cvtsi2ss %eax,%xmm0
 	movaps %xmm1,%xmm2
 	divss  %xmm0,%xmm2
 	test   %edi,%edi
-	jle    120af <linspacef+0xdf>
+	jle    1206f <linspacef+0xdf>
 	cmp    $0x2,%eax
-	jbe    120b1 <linspacef+0xe1>
+	jbe    12071 <linspacef+0xe1>
 	mov    %edi,%edx
-	movdqa 0x63dc(%rip),%xmm1        
+	movdqa 0x641c(%rip),%xmm1        
 	movaps %xmm2,%xmm5
 	movaps %xmm6,%xmm4
 	shr    $0x2,%edx
 	mov    %rsi,%rax
 	shufps $0x0,%xmm5,%xmm5
 	shufps $0x0,%xmm4,%xmm4
 	shl    $0x4,%rdx
-	movdqa 0x611c(%rip),%xmm3        
+	movdqa 0x615c(%rip),%xmm3        
 	add    %rsi,%rdx
 	nopw   0x0(%rax,%rax,1)
 	movdqa %xmm1,%xmm0
 	add    $0x10,%rax
 	paddd  %xmm3,%xmm1
 	cvtdq2ps %xmm0,%xmm0
 	mulps  %xmm5,%xmm0
 	addps  %xmm4,%xmm0
 	movups %xmm0,-0x10(%rax)
 	cmp    %rdx,%rax
-	jne    12030 <linspacef+0x60>
+	jne    11ff0 <linspacef+0x60>
 	mov    %edi,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%dil
-	je     120b0 <linspacef+0xe0>
+	je     12070 <linspacef+0xe0>
 	pxor   %xmm0,%xmm0
 	movslq %eax,%rdx
 	cvtsi2ss %eax,%xmm0
 	mulss  %xmm2,%xmm0
 	addss  %xmm6,%xmm0
 	movss  %xmm0,(%rsi,%rdx,4)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%edi
-	jle    120af <linspacef+0xdf>
+	jle    1206f <linspacef+0xdf>
 	pxor   %xmm0,%xmm0
 	movslq %edx,%rcx
 	add    $0x2,%eax
 	cvtsi2ss %edx,%xmm0
 	mulss  %xmm2,%xmm0
 	addss  %xmm6,%xmm0
 	movss  %xmm0,(%rsi,%rcx,4)
 	cmp    %eax,%edi
-	jle    120af <linspacef+0xdf>
+	jle    1206f <linspacef+0xdf>
 	pxor   %xmm0,%xmm0
 	movslq %eax,%rdx
 	cvtsi2ss %eax,%xmm0
 	mulss  %xmm0,%xmm2
 	addss  %xmm6,%xmm2
 	movss  %xmm2,(%rsi,%rdx,4)
 	ret
 	ret
 	xor    %eax,%eax
-	jmp    12059 <linspacef+0x89>
+	jmp    12019 <linspacef+0x89>
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-00000000000120c0 <arange_float>:
+0000000000012080 <arange_float>:
 arange_float():
 	subss  %xmm0,%xmm1
 	movaps %xmm0,%xmm3
-	movss  0x6171(%rip),%xmm0        
-	movss  0x6269(%rip),%xmm4        
+	movss  0x61b1(%rip),%xmm0        
+	movss  0x62a9(%rip),%xmm4        
 	divss  %xmm2,%xmm1
 	andps  %xmm1,%xmm0
 	comiss %xmm0,%xmm4
-	jbe    12103 <arange_float+0x43>
+	jbe    120c3 <arange_float+0x43>
 	cvttss2si %xmm1,%eax
 	pxor   %xmm0,%xmm0
-	movss  0x6205(%rip),%xmm4        
+	movss  0x6245(%rip),%xmm4        
 	cvtsi2ss %eax,%xmm0
 	cmpnless %xmm0,%xmm1
 	andps  %xmm4,%xmm1
 	addss  %xmm0,%xmm1
 	cvttss2si %xmm1,%ecx
 	test   %ecx,%ecx
-	jle    121ce <arange_float+0x10e>
+	jle    1218e <arange_float+0x10e>
 	lea    -0x1(%rcx),%eax
 	cmp    $0x2,%eax
-	jbe    121d1 <arange_float+0x111>
+	jbe    12191 <arange_float+0x111>
 	mov    %ecx,%edx
-	movdqa 0x62bb(%rip),%xmm1        
+	movdqa 0x62fb(%rip),%xmm1        
 	movaps %xmm2,%xmm6
 	movaps %xmm3,%xmm5
 	shr    $0x2,%edx
 	mov    %rdi,%rax
 	shufps $0x0,%xmm6,%xmm6
 	shufps $0x0,%xmm5,%xmm5
 	shl    $0x4,%rdx
-	movdqa 0x5ffb(%rip),%xmm4        
+	movdqa 0x603b(%rip),%xmm4        
 	add    %rdi,%rdx
 	nopl   0x0(%rax,%rax,1)
 	movdqa %xmm1,%xmm0
 	add    $0x10,%rax
 	paddd  %xmm4,%xmm1
 	cvtdq2ps %xmm0,%xmm0
 	mulps  %xmm6,%xmm0
 	addps  %xmm5,%xmm0
 	movups %xmm0,-0x10(%rax)
 	cmp    %rdx,%rax
-	jne    12150 <arange_float+0x90>
+	jne    12110 <arange_float+0x90>
 	mov    %ecx,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%cl
-	je     121d0 <arange_float+0x110>
+	je     12190 <arange_float+0x110>
 	pxor   %xmm0,%xmm0
 	movslq %eax,%rdx
 	cvtsi2ss %eax,%xmm0
 	mulss  %xmm2,%xmm0
 	addss  %xmm3,%xmm0
 	movss  %xmm0,(%rdi,%rdx,4)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%ecx
-	jle    121ce <arange_float+0x10e>
+	jle    1218e <arange_float+0x10e>
 	pxor   %xmm0,%xmm0
 	movslq %edx,%rsi
 	add    $0x2,%eax
 	cvtsi2ss %edx,%xmm0
 	mulss  %xmm2,%xmm0
 	addss  %xmm3,%xmm0
 	movss  %xmm0,(%rdi,%rsi,4)
 	cmp    %eax,%ecx
-	jle    121ce <arange_float+0x10e>
+	jle    1218e <arange_float+0x10e>
 	pxor   %xmm0,%xmm0
 	movslq %eax,%rdx
 	cvtsi2ss %eax,%xmm0
 	mulss  %xmm0,%xmm2
 	addss  %xmm3,%xmm2
 	movss  %xmm2,(%rdi,%rdx,4)
 	ret
 	nop
 	ret
 	xor    %eax,%eax
-	jmp    12178 <arange_float+0xb8>
+	jmp    12138 <arange_float+0xb8>
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-00000000000121e0 <arange_int>:
+00000000000121a0 <arange_int>:
 arange_int():
 	mov    %edi,%r8d
 	mov    %esi,%eax
 	mov    %edx,%edi
 	mov    %rcx,%r9
 	sub    %r8d,%eax
 	cltd
 	idiv   %edi
 	test   %eax,%eax
-	jle    122bc <arange_int+0xdc>
+	jle    1227c <arange_int+0xdc>
 	lea    -0x1(%rax),%edx
 	cmp    $0x2,%edx
-	jbe    122c1 <arange_int+0xe1>
+	jbe    12281 <arange_int+0xe1>
 	movd   %edi,%xmm7
 	mov    %rcx,%rdx
 	mov    %eax,%ecx
-	movdqa 0x61cb(%rip),%xmm2        
+	movdqa 0x620b(%rip),%xmm2        
 	pshufd $0x0,%xmm7,%xmm3
 	shr    $0x2,%ecx
 	movd   %r8d,%xmm7
-	movdqa 0x5f16(%rip),%xmm5        
+	movdqa 0x5f56(%rip),%xmm5        
 	shl    $0x4,%rcx
 	movdqa %xmm3,%xmm4
 	pshufd $0x0,%xmm7,%xmm6
 	add    %r9,%rcx
 	psrlq  $0x20,%xmm4
 	nop
 	movdqa %xmm2,%xmm0
@@ -14698,160 +14692,160 @@
 	pshufd $0x8,%xmm1,%xmm1
 	pshufd $0x8,%xmm0,%xmm0
 	punpckldq %xmm0,%xmm1
 	movdqa %xmm1,%xmm0
 	paddd  %xmm6,%xmm0
 	movups %xmm0,-0x10(%rdx)
 	cmp    %rcx,%rdx
-	jne    12240 <arange_int+0x60>
+	jne    12200 <arange_int+0x60>
 	mov    %eax,%edx
 	and    $0xfffffffc,%edx
 	test   $0x3,%al
-	je     122c0 <arange_int+0xe0>
+	je     12280 <arange_int+0xe0>
 	mov    %edi,%ecx
 	movslq %edx,%rsi
 	imul   %edx,%ecx
 	lea    (%rcx,%r8,1),%r10d
 	mov    %r10d,(%r9,%rsi,4)
 	lea    0x1(%rdx),%esi
 	cmp    %esi,%eax
-	jle    122bc <arange_int+0xdc>
+	jle    1227c <arange_int+0xdc>
 	add    %edi,%ecx
 	movslq %esi,%rsi
 	add    $0x2,%edx
 	lea    (%r8,%rcx,1),%r10d
 	mov    %r10d,(%r9,%rsi,4)
 	cmp    %edx,%eax
-	jle    122bc <arange_int+0xdc>
+	jle    1227c <arange_int+0xdc>
 	add    %ecx,%edi
 	movslq %edx,%rdx
 	add    %r8d,%edi
 	mov    %edi,(%r9,%rdx,4)
 	ret
 	nopl   (%rax)
 	ret
 	xor    %edx,%edx
-	jmp    12285 <arange_int+0xa5>
+	jmp    12245 <arange_int+0xa5>
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-00000000000122d0 <sum>:
+0000000000012290 <sum>:
 sum():
 	test   %esi,%esi
-	jle    12350 <sum+0x80>
+	jle    12310 <sum+0x80>
 	lea    -0x1(%rsi),%eax
 	cmp    $0x3,%eax
-	jbe    12359 <sum+0x89>
+	jbe    12319 <sum+0x89>
 	mov    %esi,%edx
 	mov    %rdi,%rax
 	pxor   %xmm0,%xmm0
 	shr    %edx
 	shl    $0x4,%rdx
 	add    %rdi,%rdx
 	xchg   %ax,%ax
 	movupd (%rax),%xmm2
 	add    $0x10,%rax
 	addpd  %xmm2,%xmm0
 	cmp    %rdx,%rax
-	jne    122f0 <sum+0x20>
+	jne    122b0 <sum+0x20>
 	movapd %xmm0,%xmm1
 	mov    %esi,%eax
 	unpckhpd %xmm0,%xmm1
 	and    $0xfffffffe,%eax
 	addpd  %xmm1,%xmm0
 	test   $0x1,%sil
-	je     12358 <sum+0x88>
+	je     12318 <sum+0x88>
 	movslq %eax,%rdx
 	addsd  (%rdi,%rdx,8),%xmm0
 	lea    0x1(%rax),%edx
 	cmp    %edx,%esi
-	jle    12354 <sum+0x84>
+	jle    12314 <sum+0x84>
 	movslq %edx,%rdx
 	addsd  (%rdi,%rdx,8),%xmm0
 	lea    0x2(%rax),%edx
 	cmp    %edx,%esi
-	jle    12354 <sum+0x84>
+	jle    12314 <sum+0x84>
 	movslq %edx,%rdx
 	add    $0x3,%eax
 	addsd  (%rdi,%rdx,8),%xmm0
 	cmp    %eax,%esi
-	jle    12354 <sum+0x84>
+	jle    12314 <sum+0x84>
 	cltq
 	addsd  (%rdi,%rax,8),%xmm0
 	ret
 	nopl   (%rax)
 	pxor   %xmm0,%xmm0
 	ret
 	nopl   (%rax)
 	ret
 	xor    %eax,%eax
 	pxor   %xmm0,%xmm0
-	jmp    12318 <sum+0x48>
+	jmp    122d8 <sum+0x48>
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
-0000000000012370 <sumf>:
+0000000000012330 <sumf>:
 sumf():
 	test   %esi,%esi
-	jle    123e8 <sumf+0x78>
+	jle    123a8 <sumf+0x78>
 	lea    -0x1(%rsi),%eax
 	cmp    $0x2,%eax
-	jbe    123f1 <sumf+0x81>
+	jbe    123b1 <sumf+0x81>
 	mov    %esi,%edx
 	mov    %rdi,%rax
 	pxor   %xmm0,%xmm0
 	shr    $0x2,%edx
 	shl    $0x4,%rdx
 	add    %rdi,%rdx
 	nop
 	movups (%rax),%xmm2
 	add    $0x10,%rax
 	addps  %xmm2,%xmm0
 	cmp    %rdx,%rax
-	jne    12390 <sumf+0x20>
+	jne    12350 <sumf+0x20>
 	movaps %xmm0,%xmm1
 	mov    %esi,%eax
 	movhlps %xmm0,%xmm1
 	and    $0xfffffffc,%eax
 	addps  %xmm0,%xmm1
 	movaps %xmm1,%xmm0
 	shufps $0x55,%xmm1,%xmm0
 	addps  %xmm1,%xmm0
 	test   $0x3,%sil
-	je     123f0 <sumf+0x80>
+	je     123b0 <sumf+0x80>
 	movslq %eax,%rdx
 	addss  (%rdi,%rdx,4),%xmm0
 	lea    0x1(%rax),%edx
 	cmp    %edx,%esi
-	jle    123ec <sumf+0x7c>
+	jle    123ac <sumf+0x7c>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	addss  (%rdi,%rdx,4),%xmm0
 	cmp    %eax,%esi
-	jle    123ec <sumf+0x7c>
+	jle    123ac <sumf+0x7c>
 	cltq
 	addss  (%rdi,%rax,4),%xmm0
 	ret
 	nopl   0x0(%rax,%rax,1)
 	pxor   %xmm0,%xmm0
 	ret
 	nopl   (%rax)
 	ret
 	xor    %eax,%eax
 	pxor   %xmm0,%xmm0
-	jmp    123bd <sumf+0x4d>
+	jmp    1237d <sumf+0x4d>
 	nopl   0x0(%rax)
 
-0000000000012400 <scalar_mul_int32>:
+00000000000123c0 <scalar_mul_int32>:
 scalar_mul_int32():
 	mov    %edx,%r8d
 	test   %edx,%edx
-	jle    124ad <scalar_mul_int32+0xad>
+	jle    1246d <scalar_mul_int32+0xad>
 	lea    -0x1(%rdx),%eax
 	cmp    $0x2,%eax
-	jbe    124b1 <scalar_mul_int32+0xb1>
+	jbe    12471 <scalar_mul_int32+0xb1>
 	movd   %esi,%xmm4
 	shr    $0x2,%edx
 	xor    %eax,%eax
 	pshufd $0x0,%xmm4,%xmm2
 	shl    $0x4,%rdx
 	movdqa %xmm2,%xmm3
 	psrlq  $0x20,%xmm3
@@ -14863,152 +14857,152 @@
 	pmuludq %xmm3,%xmm0
 	pshufd $0x8,%xmm1,%xmm1
 	pshufd $0x8,%xmm0,%xmm0
 	punpckldq %xmm0,%xmm1
 	movups %xmm1,(%rcx,%rax,1)
 	add    $0x10,%rax
 	cmp    %rdx,%rax
-	jne    12438 <scalar_mul_int32+0x38>
+	jne    123f8 <scalar_mul_int32+0x38>
 	mov    %r8d,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%r8b
-	je     124b0 <scalar_mul_int32+0xb0>
+	je     12470 <scalar_mul_int32+0xb0>
 	movslq %eax,%rdx
 	mov    (%rdi,%rdx,4),%r9d
 	imul   %esi,%r9d
 	mov    %r9d,(%rcx,%rdx,4)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%r8d
-	jle    124ad <scalar_mul_int32+0xad>
+	jle    1246d <scalar_mul_int32+0xad>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	mov    (%rdi,%rdx,4),%r9d
 	imul   %esi,%r9d
 	mov    %r9d,(%rcx,%rdx,4)
 	cmp    %eax,%r8d
-	jle    124ad <scalar_mul_int32+0xad>
+	jle    1246d <scalar_mul_int32+0xad>
 	cltq
 	imul   (%rdi,%rax,4),%esi
 	mov    %esi,(%rcx,%rax,4)
 	ret
 	xchg   %ax,%ax
 	ret
 	xor    %eax,%eax
-	jmp    12476 <scalar_mul_int32+0x76>
+	jmp    12436 <scalar_mul_int32+0x76>
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-00000000000124c0 <scalar_mul_int64>:
+0000000000012480 <scalar_mul_int64>:
 scalar_mul_int64():
 	mov    %rcx,%r8
 	test   %edx,%edx
-	jle    124e5 <scalar_mul_int64+0x25>
+	jle    124a5 <scalar_mul_int64+0x25>
 	movslq %edx,%rcx
 	xor    %eax,%eax
 	nopl   0x0(%rax)
 	mov    (%rdi,%rax,8),%rdx
 	imul   %rsi,%rdx
 	mov    %rdx,(%r8,%rax,8)
 	add    $0x1,%rax
 	cmp    %rax,%rcx
-	jne    124d0 <scalar_mul_int64+0x10>
+	jne    12490 <scalar_mul_int64+0x10>
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 
-00000000000124f0 <scalar_mul_float32>:
+00000000000124b0 <scalar_mul_float32>:
 scalar_mul_float32():
 	movaps %xmm0,%xmm1
 	test   %esi,%esi
-	jle    12573 <scalar_mul_float32+0x83>
+	jle    12533 <scalar_mul_float32+0x83>
 	lea    -0x1(%rsi),%eax
 	cmp    $0x2,%eax
-	jbe    12579 <scalar_mul_float32+0x89>
+	jbe    12539 <scalar_mul_float32+0x89>
 	mov    %esi,%ecx
 	movaps %xmm0,%xmm2
 	xor    %eax,%eax
 	shr    $0x2,%ecx
 	shufps $0x0,%xmm2,%xmm2
 	shl    $0x4,%rcx
 	nopl   0x0(%rax)
 	movups (%rdi,%rax,1),%xmm0
 	mulps  %xmm2,%xmm0
 	movups %xmm0,(%rdx,%rax,1)
 	add    $0x10,%rax
 	cmp    %rcx,%rax
-	jne    12518 <scalar_mul_float32+0x28>
+	jne    124d8 <scalar_mul_float32+0x28>
 	mov    %esi,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%sil
-	je     12578 <scalar_mul_float32+0x88>
+	je     12538 <scalar_mul_float32+0x88>
 	movslq %eax,%rcx
 	movss  (%rdi,%rcx,4),%xmm0
 	mulss  %xmm1,%xmm0
 	movss  %xmm0,(%rdx,%rcx,4)
 	lea    0x1(%rax),%ecx
 	cmp    %ecx,%esi
-	jle    12573 <scalar_mul_float32+0x83>
+	jle    12533 <scalar_mul_float32+0x83>
 	movslq %ecx,%rcx
 	add    $0x2,%eax
 	movss  (%rdi,%rcx,4),%xmm0
 	mulss  %xmm1,%xmm0
 	movss  %xmm0,(%rdx,%rcx,4)
 	cmp    %eax,%esi
-	jle    12573 <scalar_mul_float32+0x83>
+	jle    12533 <scalar_mul_float32+0x83>
 	cltq
 	mulss  (%rdi,%rax,4),%xmm1
 	movss  %xmm1,(%rdx,%rax,4)
 	ret
 	nopl   0x0(%rax)
 	ret
 	xor    %eax,%eax
-	jmp    12537 <scalar_mul_float32+0x47>
+	jmp    124f7 <scalar_mul_float32+0x47>
 	nopl   (%rax)
 
-0000000000012580 <scalar_mul_float64>:
+0000000000012540 <scalar_mul_float64>:
 scalar_mul_float64():
 	test   %esi,%esi
-	jle    125cc <scalar_mul_float64+0x4c>
+	jle    1258c <scalar_mul_float64+0x4c>
 	cmp    $0x1,%esi
-	je     125d1 <scalar_mul_float64+0x51>
+	je     12591 <scalar_mul_float64+0x51>
 	mov    %esi,%ecx
 	movapd %xmm0,%xmm2
 	xor    %eax,%eax
 	shr    %ecx
 	unpcklpd %xmm2,%xmm2
 	shl    $0x4,%rcx
 	nopl   0x0(%rax,%rax,1)
 	movupd (%rdi,%rax,1),%xmm1
 	mulpd  %xmm2,%xmm1
 	movups %xmm1,(%rdx,%rax,1)
 	add    $0x10,%rax
 	cmp    %rax,%rcx
-	jne    125a0 <scalar_mul_float64+0x20>
+	jne    12560 <scalar_mul_float64+0x20>
 	mov    %esi,%eax
 	and    $0xfffffffe,%eax
 	and    $0x1,%esi
-	je     125d0 <scalar_mul_float64+0x50>
+	je     12590 <scalar_mul_float64+0x50>
 	cltq
 	mulsd  (%rdi,%rax,8),%xmm0
 	movsd  %xmm0,(%rdx,%rax,8)
 	ret
 	nopl   (%rax)
 	ret
 	xor    %eax,%eax
-	jmp    125c0 <scalar_mul_float64+0x40>
+	jmp    12580 <scalar_mul_float64+0x40>
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-00000000000125e0 <scalar_mul_complex64>:
+00000000000125a0 <scalar_mul_complex64>:
 scalar_mul_complex64():
 	movq   %xmm0,-0x10(%rsp)
 	movss  -0x10(%rsp),%xmm6
 	movss  -0xc(%rsp),%xmm7
 	test   %esi,%esi
-	jle    12744 <scalar_mul_complex64+0x164>
+	jle    12704 <scalar_mul_complex64+0x164>
 	lea    -0x1(%rsi),%eax
 	cmp    $0x2,%eax
-	jbe    12749 <scalar_mul_complex64+0x169>
+	jbe    12709 <scalar_mul_complex64+0x169>
 	mov    %esi,%ecx
 	movaps %xmm6,%xmm4
 	movaps %xmm7,%xmm3
 	xor    %eax,%eax
 	shr    $0x2,%ecx
 	shufps $0x0,%xmm4,%xmm4
 	shufps $0x0,%xmm3,%xmm3
@@ -15030,19 +15024,19 @@
 	movaps %xmm2,%xmm1
 	unpcklps %xmm0,%xmm1
 	unpckhps %xmm0,%xmm2
 	movups %xmm1,(%rdx,%rax,1)
 	movups %xmm2,0x10(%rdx,%rax,1)
 	add    $0x20,%rax
 	cmp    %rax,%rcx
-	jne    12620 <scalar_mul_complex64+0x40>
+	jne    125e0 <scalar_mul_complex64+0x40>
 	mov    %esi,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%sil
-	je     12748 <scalar_mul_complex64+0x168>
+	je     12708 <scalar_mul_complex64+0x168>
 	movslq %eax,%rcx
 	movaps %xmm7,%xmm3
 	shl    $0x3,%rcx
 	lea    (%rdi,%rcx,1),%r8
 	add    %rdx,%rcx
 	movss  (%r8),%xmm0
 	movss  0x4(%r8),%xmm1
@@ -15053,15 +15047,15 @@
 	mulss  %xmm6,%xmm1
 	subss  %xmm3,%xmm2
 	addss  %xmm1,%xmm0
 	movss  %xmm2,(%rcx)
 	movss  %xmm0,0x4(%rcx)
 	lea    0x1(%rax),%ecx
 	cmp    %ecx,%esi
-	jle    12744 <scalar_mul_complex64+0x164>
+	jle    12704 <scalar_mul_complex64+0x164>
 	movslq %ecx,%rcx
 	movaps %xmm6,%xmm2
 	movaps %xmm7,%xmm3
 	add    $0x2,%eax
 	shl    $0x3,%rcx
 	lea    (%rdi,%rcx,1),%r8
 	add    %rdx,%rcx
@@ -15072,15 +15066,15 @@
 	mulss  %xmm7,%xmm0
 	mulss  %xmm6,%xmm1
 	subss  %xmm3,%xmm2
 	addss  %xmm1,%xmm0
 	movss  %xmm2,(%rcx)
 	movss  %xmm0,0x4(%rcx)
 	cmp    %eax,%esi
-	jle    12744 <scalar_mul_complex64+0x164>
+	jle    12704 <scalar_mul_complex64+0x164>
 	cltq
 	movaps %xmm6,%xmm0
 	movaps %xmm7,%xmm3
 	shl    $0x3,%rax
 	add    %rax,%rdi
 	add    %rax,%rdx
 	movss  (%rdi),%xmm1
@@ -15093,20 +15087,20 @@
 	addss  %xmm7,%xmm6
 	movss  %xmm0,(%rdx)
 	movss  %xmm6,0x4(%rdx)
 	ret
 	nopl   (%rax)
 	ret
 	xor    %eax,%eax
-	jmp    12676 <scalar_mul_complex64+0x96>
+	jmp    12636 <scalar_mul_complex64+0x96>
 
-0000000000012750 <scalar_mul_complex128>:
+0000000000012710 <scalar_mul_complex128>:
 scalar_mul_complex128():
 	test   %esi,%esi
-	jle    127ab <scalar_mul_complex128+0x5b>
+	jle    1276b <scalar_mul_complex128+0x5b>
 	movapd %xmm0,%xmm4
 	movapd %xmm1,%xmm3
 	movslq %esi,%rsi
 	xor    %eax,%eax
 	unpcklpd %xmm1,%xmm4
 	unpcklpd %xmm0,%xmm3
 	shl    $0x4,%rsi
@@ -15121,26 +15115,26 @@
 	movapd %xmm1,%xmm2
 	subpd  %xmm0,%xmm2
 	addpd  %xmm1,%xmm0
 	movsd  %xmm2,%xmm0
 	movups %xmm0,(%rdx,%rax,1)
 	add    $0x10,%rax
 	cmp    %rsi,%rax
-	jne    12770 <scalar_mul_complex128+0x20>
+	jne    12730 <scalar_mul_complex128+0x20>
 	ret
 	nopl   0x0(%rax)
 
-00000000000127b0 <vector_mul_int32>:
+0000000000012770 <vector_mul_int32>:
 vector_mul_int32():
 	mov    %edx,%r8d
 	test   %edx,%edx
-	jle    12859 <vector_mul_int32+0xa9>
+	jle    12819 <vector_mul_int32+0xa9>
 	lea    -0x1(%rdx),%eax
 	cmp    $0x2,%eax
-	jbe    12861 <vector_mul_int32+0xb1>
+	jbe    12821 <vector_mul_int32+0xb1>
 	shr    $0x2,%edx
 	xor    %eax,%eax
 	shl    $0x4,%rdx
 	movdqu (%rdi,%rax,1),%xmm0
 	movdqu (%rsi,%rax,1),%xmm2
 	movdqu (%rdi,%rax,1),%xmm1
 	movdqu (%rsi,%rax,1),%xmm3
@@ -15150,150 +15144,150 @@
 	pmuludq %xmm2,%xmm0
 	pshufd $0x8,%xmm1,%xmm1
 	pshufd $0x8,%xmm0,%xmm0
 	punpckldq %xmm0,%xmm1
 	movups %xmm1,(%rcx,%rax,1)
 	add    $0x10,%rax
 	cmp    %rdx,%rax
-	jne    127d0 <vector_mul_int32+0x20>
+	jne    12790 <vector_mul_int32+0x20>
 	mov    %r8d,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%r8b
-	je     12860 <vector_mul_int32+0xb0>
+	je     12820 <vector_mul_int32+0xb0>
 	movslq %eax,%rdx
 	mov    (%rdi,%rdx,4),%r9d
 	imul   (%rsi,%rdx,4),%r9d
 	mov    %r9d,(%rcx,%rdx,4)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%r8d
-	jle    12859 <vector_mul_int32+0xa9>
+	jle    12819 <vector_mul_int32+0xa9>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	mov    (%rdi,%rdx,4),%r9d
 	imul   (%rsi,%rdx,4),%r9d
 	mov    %r9d,(%rcx,%rdx,4)
 	cmp    %eax,%r8d
-	jle    12859 <vector_mul_int32+0xa9>
+	jle    12819 <vector_mul_int32+0xa9>
 	cltq
 	mov    (%rsi,%rax,4),%edx
 	imul   (%rdi,%rax,4),%edx
 	mov    %edx,(%rcx,%rax,4)
 	ret
 	nopw   0x0(%rax,%rax,1)
 	ret
 	xor    %eax,%eax
-	jmp    1281d <vector_mul_int32+0x6d>
+	jmp    127dd <vector_mul_int32+0x6d>
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-0000000000012870 <vector_mul_int64>:
+0000000000012830 <vector_mul_int64>:
 vector_mul_int64():
 	mov    %rcx,%r8
 	test   %edx,%edx
-	jle    12896 <vector_mul_int64+0x26>
+	jle    12856 <vector_mul_int64+0x26>
 	movslq %edx,%rcx
 	xor    %eax,%eax
 	nopl   0x0(%rax)
 	mov    (%rdi,%rax,8),%rdx
 	imul   (%rsi,%rax,8),%rdx
 	mov    %rdx,(%r8,%rax,8)
 	add    $0x1,%rax
 	cmp    %rax,%rcx
-	jne    12880 <vector_mul_int64+0x10>
+	jne    12840 <vector_mul_int64+0x10>
 	ret
 	nopw   0x0(%rax,%rax,1)
 
-00000000000128a0 <vector_mul_float32>:
+0000000000012860 <vector_mul_float32>:
 vector_mul_float32():
 	mov    %edx,%r8d
 	test   %edx,%edx
-	jle    12929 <vector_mul_float32+0x89>
+	jle    128e9 <vector_mul_float32+0x89>
 	lea    -0x1(%rdx),%eax
 	cmp    $0x2,%eax
-	jbe    12931 <vector_mul_float32+0x91>
+	jbe    128f1 <vector_mul_float32+0x91>
 	shr    $0x2,%edx
 	xor    %eax,%eax
 	shl    $0x4,%rdx
 	nopl   0x0(%rax)
 	movups (%rdi,%rax,1),%xmm0
 	movups (%rsi,%rax,1),%xmm1
 	mulps  %xmm1,%xmm0
 	movups %xmm0,(%rcx,%rax,1)
 	add    $0x10,%rax
 	cmp    %rdx,%rax
-	jne    128c0 <vector_mul_float32+0x20>
+	jne    12880 <vector_mul_float32+0x20>
 	mov    %r8d,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%r8b
-	je     12930 <vector_mul_float32+0x90>
+	je     128f0 <vector_mul_float32+0x90>
 	movslq %eax,%rdx
 	movss  (%rdi,%rdx,4),%xmm0
 	mulss  (%rsi,%rdx,4),%xmm0
 	movss  %xmm0,(%rcx,%rdx,4)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%r8d
-	jle    12929 <vector_mul_float32+0x89>
+	jle    128e9 <vector_mul_float32+0x89>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	movss  (%rdi,%rdx,4),%xmm0
 	mulss  (%rsi,%rdx,4),%xmm0
 	movss  %xmm0,(%rcx,%rdx,4)
 	cmp    %eax,%r8d
-	jle    12929 <vector_mul_float32+0x89>
+	jle    128e9 <vector_mul_float32+0x89>
 	cltq
 	movss  (%rsi,%rax,4),%xmm0
 	mulss  (%rdi,%rax,4),%xmm0
 	movss  %xmm0,(%rcx,%rax,4)
 	ret
 	nopw   0x0(%rax,%rax,1)
 	ret
 	xor    %eax,%eax
-	jmp    128e4 <vector_mul_float32+0x44>
+	jmp    128a4 <vector_mul_float32+0x44>
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-0000000000012940 <vector_mul_float64>:
+0000000000012900 <vector_mul_float64>:
 vector_mul_float64():
 	mov    %edx,%r8d
 	test   %edx,%edx
-	jle    12990 <vector_mul_float64+0x50>
+	jle    12950 <vector_mul_float64+0x50>
 	cmp    $0x1,%edx
-	je     12999 <vector_mul_float64+0x59>
+	je     12959 <vector_mul_float64+0x59>
 	shr    %edx
 	xor    %eax,%eax
 	shl    $0x4,%rdx
 	nopl   0x0(%rax)
 	movupd (%rdi,%rax,1),%xmm0
 	movupd (%rsi,%rax,1),%xmm1
 	mulpd  %xmm1,%xmm0
 	movups %xmm0,(%rcx,%rax,1)
 	add    $0x10,%rax
 	cmp    %rax,%rdx
-	jne    12958 <vector_mul_float64+0x18>
+	jne    12918 <vector_mul_float64+0x18>
 	mov    %r8d,%eax
 	and    $0xfffffffe,%eax
 	and    $0x1,%r8d
-	je     12998 <vector_mul_float64+0x58>
+	je     12958 <vector_mul_float64+0x58>
 	cltq
 	movsd  (%rsi,%rax,8),%xmm0
 	mulsd  (%rdi,%rax,8),%xmm0
 	movsd  %xmm0,(%rcx,%rax,8)
 	ret
 	nopl   0x0(%rax)
 	ret
 	xor    %eax,%eax
-	jmp    1297f <vector_mul_float64+0x3f>
+	jmp    1293f <vector_mul_float64+0x3f>
 	nopl   (%rax)
 
-00000000000129a0 <vector_mul_complex64>:
+0000000000012960 <vector_mul_complex64>:
 vector_mul_complex64():
 	mov    %edx,%r8d
 	test   %edx,%edx
-	jle    12b28 <vector_mul_complex64+0x188>
+	jle    12ae8 <vector_mul_complex64+0x188>
 	lea    -0x1(%rdx),%eax
 	cmp    $0x2,%eax
-	jbe    12b31 <vector_mul_complex64+0x191>
+	jbe    12af1 <vector_mul_complex64+0x191>
 	shr    $0x2,%edx
 	xor    %eax,%eax
 	shl    $0x5,%rdx
 	movups (%rdi,%rax,1),%xmm2
 	movups 0x10(%rdi,%rax,1),%xmm6
 	movups (%rsi,%rax,1),%xmm0
 	movaps %xmm2,%xmm1
@@ -15315,19 +15309,19 @@
 	movaps %xmm3,%xmm1
 	unpcklps %xmm0,%xmm1
 	unpckhps %xmm0,%xmm3
 	movups %xmm1,(%rcx,%rax,1)
 	movups %xmm3,0x10(%rcx,%rax,1)
 	add    $0x20,%rax
 	cmp    %rax,%rdx
-	jne    129c0 <vector_mul_complex64+0x20>
+	jne    12980 <vector_mul_complex64+0x20>
 	mov    %r8d,%eax
 	and    $0xfffffffc,%eax
 	test   $0x3,%r8b
-	je     12b30 <vector_mul_complex64+0x190>
+	je     12af0 <vector_mul_complex64+0x190>
 	movslq %eax,%rdx
 	shl    $0x3,%rdx
 	lea    (%rdi,%rdx,1),%r10
 	lea    (%rsi,%rdx,1),%r9
 	add    %rcx,%rdx
 	movss  (%r10),%xmm0
 	movss  0x4(%r10),%xmm3
@@ -15341,15 +15335,15 @@
 	mulss  %xmm3,%xmm1
 	subss  %xmm5,%xmm2
 	addss  %xmm1,%xmm0
 	movss  %xmm2,(%rdx)
 	movss  %xmm0,0x4(%rdx)
 	lea    0x1(%rax),%edx
 	cmp    %edx,%r8d
-	jle    12b28 <vector_mul_complex64+0x188>
+	jle    12ae8 <vector_mul_complex64+0x188>
 	movslq %edx,%rdx
 	add    $0x2,%eax
 	shl    $0x3,%rdx
 	lea    (%rdi,%rdx,1),%r10
 	lea    (%rsi,%rdx,1),%r9
 	add    %rcx,%rdx
 	movss  (%r10),%xmm0
@@ -15363,15 +15357,15 @@
 	mulss  %xmm4,%xmm0
 	mulss  %xmm3,%xmm1
 	subss  %xmm5,%xmm2
 	addss  %xmm1,%xmm0
 	movss  %xmm2,(%rdx)
 	movss  %xmm0,0x4(%rdx)
 	cmp    %eax,%r8d
-	jle    12b28 <vector_mul_complex64+0x188>
+	jle    12ae8 <vector_mul_complex64+0x188>
 	cltq
 	shl    $0x3,%rax
 	add    %rax,%rsi
 	add    %rax,%rdi
 	add    %rax,%rcx
 	movss  (%rsi),%xmm0
 	movss  0x4(%rsi),%xmm1
@@ -15387,21 +15381,21 @@
 	addss  %xmm1,%xmm0
 	movss  %xmm2,(%rcx)
 	movss  %xmm0,0x4(%rcx)
 	ret
 	nopl   0x0(%rax)
 	ret
 	xor    %eax,%eax
-	jmp    12a2e <vector_mul_complex64+0x8e>
+	jmp    129ee <vector_mul_complex64+0x8e>
 	nopl   0x0(%rax,%rax,1)
 
-0000000000012b40 <vector_mul_complex128>:
+0000000000012b00 <vector_mul_complex128>:
 vector_mul_complex128():
 	test   %edx,%edx
-	jle    12b91 <vector_mul_complex128+0x51>
+	jle    12b51 <vector_mul_complex128+0x51>
 	movslq %edx,%rdx
 	xor    %eax,%eax
 	shl    $0x4,%rdx
 	nopl   (%rax)
 	movupd (%rdi,%rax,1),%xmm2
 	movupd (%rsi,%rax,1),%xmm0
 	movupd (%rdi,%rax,1),%xmm1
@@ -15413,1874 +15407,1874 @@
 	movapd %xmm2,%xmm1
 	subpd  %xmm0,%xmm1
 	addpd  %xmm2,%xmm0
 	movsd  %xmm1,%xmm0
 	movups %xmm0,(%rcx,%rax,1)
 	add    $0x10,%rax
 	cmp    %rdx,%rax
-	jne    12b50 <vector_mul_complex128+0x10>
+	jne    12b10 <vector_mul_complex128+0x10>
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-0000000000012ba0 <sort_double>:
+0000000000012b60 <sort_double>:
 sort_double():
 	push   %r14
 	movslq %esi,%rsi
 	push   %r13
 	push   %r12
 	lea    0x0(,%rsi,8),%r12
 	push   %rbp
 	lea    (%rdi,%r12,1),%r13
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
 	test   %dl,%dl
-	jne    12ca8 <sort_double+0x108>
+	jne    12c68 <sort_double+0x108>
 	cmp    %r13,%rdi
-	je     12c94 <sort_double+0xf4>
+	je     12c54 <sort_double+0xf4>
 	mov    %r12,%rax
 	mov    $0x3f,%edx
 	lea    0x8(%rbx),%rbp
 	mov    %r13,%rsi
 	sar    $0x3,%rax
 	bsr    %rax,%rax
 	xor    $0x3f,%rax
 	sub    %eax,%edx
 	movslq %edx,%rdx
 	add    %rdx,%rdx
-	call   ef30 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   eef0 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_less_iter>(double*, double*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	cmp    $0x80,%r12
-	jg     12d68 <sort_double+0x1c8>
+	jg     12d28 <sort_double+0x1c8>
 	cmp    %r13,%rbp
-	je     12c94 <sort_double+0xf4>
+	je     12c54 <sort_double+0xf4>
 	mov    $0x8,%r12d
-	jmp    12c48 <sort_double+0xa8>
+	jmp    12c08 <sort_double+0xa8>
 	nopl   (%rax)
 	cmp    %rbp,%rbx
-	je     12c3b <sort_double+0x9b>
+	je     12bfb <sort_double+0x9b>
 	mov    %rbp,%rdx
 	lea    (%rbx,%r12,1),%rdi
 	mov    %rbx,%rsi
 	movsd  %xmm1,0x8(%rsp)
 	sub    %rbx,%rdx
 	call   31f0 <memmove@plt>
 	movsd  0x8(%rsp),%xmm1
 	add    $0x8,%rbp
 	movsd  %xmm1,(%rbx)
 	cmp    %r13,%rbp
-	je     12c94 <sort_double+0xf4>
+	je     12c54 <sort_double+0xf4>
 	movsd  0x0(%rbp),%xmm1
 	comisd (%rbx),%xmm1
-	jb     12c18 <sort_double+0x78>
+	jb     12bd8 <sort_double+0x78>
 	movsd  -0x8(%rbp),%xmm0
 	lea    -0x8(%rbp),%rax
 	comisd %xmm1,%xmm0
-	jbe    12f29 <sort_double+0x389>
+	jbe    12ee9 <sort_double+0x389>
 	cs nopw 0x0(%rax,%rax,1)
 	movsd  %xmm0,0x8(%rax)
 	mov    %rax,%rdx
 	movsd  -0x8(%rax),%xmm0
 	sub    $0x8,%rax
 	comisd %xmm1,%xmm0
-	ja     12c70 <sort_double+0xd0>
+	ja     12c30 <sort_double+0xd0>
 	add    $0x8,%rbp
 	movsd  %xmm1,(%rdx)
 	cmp    %r13,%rbp
-	jne    12c48 <sort_double+0xa8>
+	jne    12c08 <sort_double+0xa8>
 	add    $0x10,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	nopl   0x0(%rax)
 	cmp    %r13,%rdi
-	je     12c94 <sort_double+0xf4>
+	je     12c54 <sort_double+0xf4>
 	mov    %r12,%rax
 	mov    $0x3f,%edx
 	lea    0x8(%rbx),%r14
 	mov    %r13,%rsi
 	sar    $0x3,%rax
 	bsr    %rax,%rax
 	xor    $0x3f,%rax
 	sub    %eax,%edx
 	movslq %edx,%rdx
 	add    %rdx,%rdx
 	call   3250 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)@plt>
 	cmp    $0x80,%r12
-	jg     12e55 <sort_double+0x2b5>
+	jg     12e15 <sort_double+0x2b5>
 	cmp    %r13,%r14
-	je     12c94 <sort_double+0xf4>
+	je     12c54 <sort_double+0xf4>
 	mov    $0x8,%ebp
-	jmp    12d24 <sort_double+0x184>
+	jmp    12ce4 <sort_double+0x184>
 	xchg   %ax,%ax
 	cmp    %r14,%rbx
-	je     12d13 <sort_double+0x173>
+	je     12cd3 <sort_double+0x173>
 	mov    %r14,%rdx
 	lea    (%rbx,%rbp,1),%rdi
 	mov    %rbx,%rsi
 	movsd  %xmm1,0x8(%rsp)
 	sub    %rbx,%rdx
 	call   31f0 <memmove@plt>
 	movsd  0x8(%rsp),%xmm1
 	movsd  %xmm1,(%rbx)
 	add    $0x8,%r14
 	cmp    %r13,%r14
-	je     12c94 <sort_double+0xf4>
+	je     12c54 <sort_double+0xf4>
 	movsd  (%r14),%xmm1
 	comisd (%rbx),%xmm1
-	ja     12cf0 <sort_double+0x150>
+	ja     12cb0 <sort_double+0x150>
 	movsd  -0x8(%r14),%xmm0
 	lea    -0x8(%r14),%rax
 	comisd %xmm0,%xmm1
-	jbe    12f36 <sort_double+0x396>
+	jbe    12ef6 <sort_double+0x396>
 	nopl   0x0(%rax,%rax,1)
 	movsd  %xmm0,0x8(%rax)
 	mov    %rax,%rdx
 	movsd  -0x8(%rax),%xmm0
 	sub    $0x8,%rax
 	comisd %xmm0,%xmm1
-	ja     12d48 <sort_double+0x1a8>
+	ja     12d08 <sort_double+0x1a8>
 	movsd  %xmm1,(%rdx)
-	jmp    12d17 <sort_double+0x177>
+	jmp    12cd7 <sort_double+0x177>
 	nopl   (%rax)
 	lea    0x80(%rbx),%r12
 	mov    $0x8,%r14d
-	jmp    12db0 <sort_double+0x210>
+	jmp    12d70 <sort_double+0x210>
 	nopw   0x0(%rax,%rax,1)
 	cmp    %rbp,%rbx
-	je     12da3 <sort_double+0x203>
+	je     12d63 <sort_double+0x203>
 	mov    %rbp,%rdx
 	lea    (%rbx,%r14,1),%rdi
 	mov    %rbx,%rsi
 	movsd  %xmm1,0x8(%rsp)
 	sub    %rbx,%rdx
 	call   31f0 <memmove@plt>
 	movsd  0x8(%rsp),%xmm1
 	add    $0x8,%rbp
 	movsd  %xmm1,(%rbx)
 	cmp    %rbp,%r12
-	je     12df8 <sort_double+0x258>
+	je     12db8 <sort_double+0x258>
 	movsd  0x0(%rbp),%xmm1
 	comisd (%rbx),%xmm1
-	jb     12d80 <sort_double+0x1e0>
+	jb     12d40 <sort_double+0x1e0>
 	movsd  -0x8(%rbp),%xmm0
 	lea    -0x8(%rbp),%rax
 	comisd %xmm1,%xmm0
-	jbe    12f21 <sort_double+0x381>
+	jbe    12ee1 <sort_double+0x381>
 	xchg   %ax,%ax
 	movsd  %xmm0,0x8(%rax)
 	mov    %rax,%rdx
 	movsd  -0x8(%rax),%xmm0
 	sub    $0x8,%rax
 	comisd %xmm1,%xmm0
-	ja     12dd0 <sort_double+0x230>
+	ja     12d90 <sort_double+0x230>
 	add    $0x8,%rbp
 	movsd  %xmm1,(%rdx)
 	cmp    %rbp,%r12
-	jne    12db0 <sort_double+0x210>
+	jne    12d70 <sort_double+0x210>
 	nopl   0x0(%rax)
 	cmp    %r13,%r12
-	je     12c94 <sort_double+0xf4>
+	je     12c54 <sort_double+0xf4>
 	movsd  (%r12),%xmm1
 	movsd  -0x8(%r12),%xmm0
 	lea    -0x8(%r12),%rax
 	comisd %xmm1,%xmm0
-	jbe    12e48 <sort_double+0x2a8>
+	jbe    12e08 <sort_double+0x2a8>
 	nopl   0x0(%rax)
 	movsd  %xmm0,0x8(%rax)
 	mov    %rax,%rdx
 	movsd  -0x8(%rax),%xmm0
 	sub    $0x8,%rax
 	comisd %xmm1,%xmm0
-	ja     12e20 <sort_double+0x280>
+	ja     12de0 <sort_double+0x280>
 	movsd  %xmm1,(%rdx)
 	add    $0x8,%r12
-	jmp    12df8 <sort_double+0x258>
+	jmp    12db8 <sort_double+0x258>
 	nopl   0x0(%rax)
 	mov    %r12,%rdx
 	add    $0x8,%r12
 	movsd  %xmm1,(%rdx)
-	jmp    12df8 <sort_double+0x258>
+	jmp    12db8 <sort_double+0x258>
 	lea    0x80(%rbx),%rbp
 	mov    $0x8,%r12d
-	jmp    12e98 <sort_double+0x2f8>
+	jmp    12e58 <sort_double+0x2f8>
 	nopl   0x0(%rax)
 	cmp    %r14,%rbx
-	je     12e8b <sort_double+0x2eb>
+	je     12e4b <sort_double+0x2eb>
 	mov    %r14,%rdx
 	lea    (%rbx,%r12,1),%rdi
 	mov    %rbx,%rsi
 	movsd  %xmm1,0x8(%rsp)
 	sub    %rbx,%rdx
 	call   31f0 <memmove@plt>
 	movsd  0x8(%rsp),%xmm1
 	movsd  %xmm1,(%rbx)
 	add    $0x8,%r14
 	cmp    %r14,%rbp
-	je     12ee0 <sort_double+0x340>
+	je     12ea0 <sort_double+0x340>
 	movsd  (%r14),%xmm1
 	comisd (%rbx),%xmm1
-	ja     12e68 <sort_double+0x2c8>
+	ja     12e28 <sort_double+0x2c8>
 	movsd  -0x8(%r14),%xmm0
 	lea    -0x8(%r14),%rax
 	comisd %xmm0,%xmm1
-	jbe    12f31 <sort_double+0x391>
+	jbe    12ef1 <sort_double+0x391>
 	nopl   0x0(%rax,%rax,1)
 	movsd  %xmm0,0x8(%rax)
 	mov    %rax,%rdx
 	movsd  -0x8(%rax),%xmm0
 	sub    $0x8,%rax
 	comisd %xmm0,%xmm1
-	ja     12eb8 <sort_double+0x318>
+	ja     12e78 <sort_double+0x318>
 	movsd  %xmm1,(%rdx)
-	jmp    12e8f <sort_double+0x2ef>
+	jmp    12e4f <sort_double+0x2ef>
 	mov    %rbp,%rdx
 	add    $0x8,%rbp
 	movsd  %xmm1,(%rdx)
 	cmp    %r13,%rbp
-	je     12c94 <sort_double+0xf4>
+	je     12c54 <sort_double+0xf4>
 	movsd  0x0(%rbp),%xmm1
 	movsd  -0x8(%rbp),%xmm0
 	lea    -0x8(%rbp),%rax
 	comisd %xmm0,%xmm1
-	jbe    12ed5 <sort_double+0x335>
+	jbe    12e95 <sort_double+0x335>
 	nopl   (%rax)
 	movsd  %xmm0,0x8(%rax)
 	mov    %rax,%rdx
 	movsd  -0x8(%rax),%xmm0
 	sub    $0x8,%rax
 	comisd %xmm0,%xmm1
-	ja     12f00 <sort_double+0x360>
+	ja     12ec0 <sort_double+0x360>
 	movsd  %xmm1,(%rdx)
 	add    $0x8,%rbp
-	jmp    12ee0 <sort_double+0x340>
+	jmp    12ea0 <sort_double+0x340>
 	mov    %rbp,%rdx
-	jmp    12de7 <sort_double+0x247>
+	jmp    12da7 <sort_double+0x247>
 	mov    %rbp,%rdx
-	jmp    12c87 <sort_double+0xe7>
+	jmp    12c47 <sort_double+0xe7>
 	mov    %r14,%rdx
-	jmp    12ecf <sort_double+0x32f>
+	jmp    12e8f <sort_double+0x32f>
 	mov    %r14,%rdx
-	jmp    12d5f <sort_double+0x1bf>
+	jmp    12d1f <sort_double+0x1bf>
 	xchg   %ax,%ax
 
-0000000000012f40 <sort_float>:
+0000000000012f00 <sort_float>:
 sort_float():
 	push   %r14
 	movslq %esi,%rsi
 	push   %r13
 	push   %r12
 	lea    0x0(,%rsi,4),%r12
 	push   %rbp
 	lea    (%rdi,%r12,1),%r13
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
 	test   %dl,%dl
-	jne    13030 <sort_float+0xf0>
+	jne    12ff0 <sort_float+0xf0>
 	cmp    %r13,%rdi
-	je     13023 <sort_float+0xe3>
+	je     12fe3 <sort_float+0xe3>
 	mov    %r12,%rax
 	mov    $0x3f,%edx
 	lea    0x4(%rbx),%rbp
 	mov    %r13,%rsi
 	sar    $0x2,%rax
 	bsr    %rax,%rax
 	xor    $0x3f,%rax
 	sub    %eax,%edx
 	movslq %edx,%rdx
 	add    %rdx,%rdx
-	call   ed80 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   ed40 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_less_iter>(float*, float*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	cmp    $0x40,%r12
-	jg     130f0 <sort_float+0x1b0>
+	jg     130b0 <sort_float+0x1b0>
 	cmp    %r13,%rbp
-	je     13023 <sort_float+0xe3>
+	je     12fe3 <sort_float+0xe3>
 	mov    $0x4,%r12d
-	jmp    12fe0 <sort_float+0xa0>
+	jmp    12fa0 <sort_float+0xa0>
 	xchg   %ax,%ax
 	cmp    %rbp,%rbx
-	je     12fd3 <sort_float+0x93>
+	je     12f93 <sort_float+0x93>
 	mov    %rbp,%rdx
 	lea    (%rbx,%r12,1),%rdi
 	mov    %rbx,%rsi
 	movss  %xmm1,0xc(%rsp)
 	sub    %rbx,%rdx
 	call   31f0 <memmove@plt>
 	movss  0xc(%rsp),%xmm1
 	add    $0x4,%rbp
 	movss  %xmm1,(%rbx)
 	cmp    %r13,%rbp
-	je     13023 <sort_float+0xe3>
+	je     12fe3 <sort_float+0xe3>
 	movss  0x0(%rbp),%xmm1
 	comiss (%rbx),%xmm1
-	jb     12fb0 <sort_float+0x70>
+	jb     12f70 <sort_float+0x70>
 	movss  -0x4(%rbp),%xmm0
 	lea    -0x4(%rbp),%rax
 	comiss %xmm1,%xmm0
-	jbe    132a8 <sort_float+0x368>
+	jbe    13268 <sort_float+0x368>
 	nopl   0x0(%rax)
 	movss  %xmm0,0x4(%rax)
 	mov    %rax,%rdx
 	movss  -0x4(%rax),%xmm0
 	sub    $0x4,%rax
 	comiss %xmm1,%xmm0
-	ja     13000 <sort_float+0xc0>
+	ja     12fc0 <sort_float+0xc0>
 	add    $0x4,%rbp
 	movss  %xmm1,(%rdx)
 	cmp    %r13,%rbp
-	jne    12fe0 <sort_float+0xa0>
+	jne    12fa0 <sort_float+0xa0>
 	add    $0x10,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	cmp    %r13,%rdi
-	je     13023 <sort_float+0xe3>
+	je     12fe3 <sort_float+0xe3>
 	mov    %r12,%rax
 	mov    $0x3f,%edx
 	lea    0x4(%rbx),%r14
 	mov    %r13,%rsi
 	sar    $0x2,%rax
 	bsr    %rax,%rax
 	xor    $0x3f,%rax
 	sub    %eax,%edx
 	movslq %edx,%rdx
 	add    %rdx,%rdx
 	call   3080 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)@plt>
 	cmp    $0x40,%r12
-	jg     131cd <sort_float+0x28d>
+	jg     1318d <sort_float+0x28d>
 	cmp    %r13,%r14
-	je     13023 <sort_float+0xe3>
+	je     12fe3 <sort_float+0xe3>
 	mov    $0x4,%ebp
-	jmp    130ac <sort_float+0x16c>
+	jmp    1306c <sort_float+0x16c>
 	nopl   0x0(%rax,%rax,1)
 	cmp    %r14,%rbx
-	je     1309b <sort_float+0x15b>
+	je     1305b <sort_float+0x15b>
 	mov    %r14,%rdx
 	lea    (%rbx,%rbp,1),%rdi
 	mov    %rbx,%rsi
 	movss  %xmm1,0xc(%rsp)
 	sub    %rbx,%rdx
 	call   31f0 <memmove@plt>
 	movss  0xc(%rsp),%xmm1
 	movss  %xmm1,(%rbx)
 	add    $0x4,%r14
 	cmp    %r13,%r14
-	je     13023 <sort_float+0xe3>
+	je     12fe3 <sort_float+0xe3>
 	movss  (%r14),%xmm1
 	comiss (%rbx),%xmm1
-	ja     13078 <sort_float+0x138>
+	ja     13038 <sort_float+0x138>
 	movss  -0x4(%r14),%xmm0
 	lea    -0x4(%r14),%rax
 	comiss %xmm0,%xmm1
-	jbe    132b5 <sort_float+0x375>
+	jbe    13275 <sort_float+0x375>
 	nopl   0x0(%rax)
 	movss  %xmm0,0x4(%rax)
 	mov    %rax,%rdx
 	movss  -0x4(%rax),%xmm0
 	sub    $0x4,%rax
 	comiss %xmm0,%xmm1
-	ja     130d0 <sort_float+0x190>
+	ja     13090 <sort_float+0x190>
 	movss  %xmm1,(%rdx)
-	jmp    1309f <sort_float+0x15f>
+	jmp    1305f <sort_float+0x15f>
 	nopl   0x0(%rax)
 	lea    0x40(%rbx),%r12
 	mov    $0x4,%r14d
-	jmp    13130 <sort_float+0x1f0>
+	jmp    130f0 <sort_float+0x1f0>
 	nopl   0x0(%rax)
 	cmp    %rbp,%rbx
-	je     13123 <sort_float+0x1e3>
+	je     130e3 <sort_float+0x1e3>
 	mov    %rbp,%rdx
 	lea    (%rbx,%r14,1),%rdi
 	mov    %rbx,%rsi
 	movss  %xmm1,0xc(%rsp)
 	sub    %rbx,%rdx
 	call   31f0 <memmove@plt>
 	movss  0xc(%rsp),%xmm1
 	add    $0x4,%rbp
 	movss  %xmm1,(%rbx)
 	cmp    %rbp,%r12
-	je     13178 <sort_float+0x238>
+	je     13138 <sort_float+0x238>
 	movss  0x0(%rbp),%xmm1
 	comiss (%rbx),%xmm1
-	jb     13100 <sort_float+0x1c0>
+	jb     130c0 <sort_float+0x1c0>
 	movss  -0x4(%rbp),%xmm0
 	lea    -0x4(%rbp),%rax
 	comiss %xmm1,%xmm0
-	jbe    132a0 <sort_float+0x360>
+	jbe    13260 <sort_float+0x360>
 	nopl   0x0(%rax)
 	movss  %xmm0,0x4(%rax)
 	mov    %rax,%rdx
 	movss  -0x4(%rax),%xmm0
 	sub    $0x4,%rax
 	comiss %xmm1,%xmm0
-	ja     13150 <sort_float+0x210>
+	ja     13110 <sort_float+0x210>
 	add    $0x4,%rbp
 	movss  %xmm1,(%rdx)
 	cmp    %rbp,%r12
-	jne    13130 <sort_float+0x1f0>
+	jne    130f0 <sort_float+0x1f0>
 	nopl   0x0(%rax,%rax,1)
 	cmp    %r13,%r12
-	je     13023 <sort_float+0xe3>
+	je     12fe3 <sort_float+0xe3>
 	movss  (%r12),%xmm1
 	movss  -0x4(%r12),%xmm0
 	lea    -0x4(%r12),%rax
 	comiss %xmm1,%xmm0
-	jbe    131c0 <sort_float+0x280>
+	jbe    13180 <sort_float+0x280>
 	nopl   0x0(%rax,%rax,1)
 	movss  %xmm0,0x4(%rax)
 	mov    %rax,%rdx
 	movss  -0x4(%rax),%xmm0
 	sub    $0x4,%rax
 	comiss %xmm1,%xmm0
-	ja     131a0 <sort_float+0x260>
+	ja     13160 <sort_float+0x260>
 	movss  %xmm1,(%rdx)
 	add    $0x4,%r12
-	jmp    13178 <sort_float+0x238>
+	jmp    13138 <sort_float+0x238>
 	mov    %r12,%rdx
 	add    $0x4,%r12
 	movss  %xmm1,(%rdx)
-	jmp    13178 <sort_float+0x238>
+	jmp    13138 <sort_float+0x238>
 	lea    0x40(%rbx),%rbp
 	mov    $0x4,%r12d
-	jmp    13210 <sort_float+0x2d0>
+	jmp    131d0 <sort_float+0x2d0>
 	nopl   0x0(%rax)
 	cmp    %r14,%rbx
-	je     13203 <sort_float+0x2c3>
+	je     131c3 <sort_float+0x2c3>
 	mov    %r14,%rdx
 	lea    (%rbx,%r12,1),%rdi
 	mov    %rbx,%rsi
 	movss  %xmm1,0xc(%rsp)
 	sub    %rbx,%rdx
 	call   31f0 <memmove@plt>
 	movss  0xc(%rsp),%xmm1
 	movss  %xmm1,(%rbx)
 	add    $0x4,%r14
 	cmp    %r14,%rbp
-	je     13260 <sort_float+0x320>
+	je     13220 <sort_float+0x320>
 	movss  (%r14),%xmm1
 	comiss (%rbx),%xmm1
-	ja     131e0 <sort_float+0x2a0>
+	ja     131a0 <sort_float+0x2a0>
 	movss  -0x4(%r14),%xmm0
 	lea    -0x4(%r14),%rax
 	comiss %xmm0,%xmm1
-	jbe    132b0 <sort_float+0x370>
+	jbe    13270 <sort_float+0x370>
 	nopl   (%rax)
 	movss  %xmm0,0x4(%rax)
 	mov    %rax,%rdx
 	movss  -0x4(%rax),%xmm0
 	sub    $0x4,%rax
 	comiss %xmm0,%xmm1
-	ja     13230 <sort_float+0x2f0>
+	ja     131f0 <sort_float+0x2f0>
 	movss  %xmm1,(%rdx)
-	jmp    13207 <sort_float+0x2c7>
+	jmp    131c7 <sort_float+0x2c7>
 	mov    %rbp,%rdx
 	add    $0x4,%rbp
 	movss  %xmm1,(%rdx)
 	nopw   0x0(%rax,%rax,1)
 	cmp    %r13,%rbp
-	je     13023 <sort_float+0xe3>
+	je     12fe3 <sort_float+0xe3>
 	movss  0x0(%rbp),%xmm1
 	movss  -0x4(%rbp),%xmm0
 	lea    -0x4(%rbp),%rax
 	comiss %xmm0,%xmm1
-	jbe    1324c <sort_float+0x30c>
+	jbe    1320c <sort_float+0x30c>
 	nopl   0x0(%rax)
 	movss  %xmm0,0x4(%rax)
 	mov    %rax,%rdx
 	movss  -0x4(%rax),%xmm0
 	sub    $0x4,%rax
 	comiss %xmm0,%xmm1
-	ja     13280 <sort_float+0x340>
+	ja     13240 <sort_float+0x340>
 	movss  %xmm1,(%rdx)
 	add    $0x4,%rbp
-	jmp    13260 <sort_float+0x320>
+	jmp    13220 <sort_float+0x320>
 	mov    %rbp,%rdx
-	jmp    13166 <sort_float+0x226>
+	jmp    13126 <sort_float+0x226>
 	mov    %rbp,%rdx
-	jmp    13016 <sort_float+0xd6>
+	jmp    12fd6 <sort_float+0xd6>
 	mov    %r14,%rdx
-	jmp    13246 <sort_float+0x306>
+	jmp    13206 <sort_float+0x306>
 	mov    %r14,%rdx
-	jmp    130e6 <sort_float+0x1a6>
+	jmp    130a6 <sort_float+0x1a6>
 	nopl   (%rax)
 
-00000000000132c0 <sort_int>:
+0000000000013280 <sort_int>:
 sort_int():
 	push   %r15
 	movslq %esi,%rsi
 	push   %r14
 	push   %r13
 	lea    0x0(,%rsi,4),%r13
 	push   %r12
 	lea    (%rdi,%r13,1),%r12
 	push   %rbp
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x8,%rsp
 	test   %dl,%dl
-	jne    133a0 <sort_int+0xe0>
+	jne    13360 <sort_int+0xe0>
 	cmp    %r12,%rdi
-	je     1338e <sort_int+0xce>
+	je     1334e <sort_int+0xce>
 	mov    %r13,%rax
 	mov    $0x3f,%edx
 	lea    0x4(%rbx),%rbp
 	mov    %r12,%rsi
 	sar    $0x2,%rax
 	bsr    %rax,%rax
 	xor    $0x3f,%rax
 	sub    %eax,%edx
 	movslq %edx,%rdx
 	add    %rdx,%rdx
-	call   ebc0 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   eb80 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_less_iter>(int*, int*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	cmp    $0x40,%r13
-	jg     13440 <sort_int+0x180>
+	jg     13400 <sort_int+0x180>
 	cmp    %r12,%rbp
-	je     1338e <sort_int+0xce>
+	je     1334e <sort_int+0xce>
 	mov    $0x4,%r13d
-	jmp    13353 <sort_int+0x93>
+	jmp    13313 <sort_int+0x93>
 	cmp    %rbp,%rbx
-	je     13347 <sort_int+0x87>
+	je     13307 <sort_int+0x87>
 	mov    %rbp,%rdx
 	lea    (%rbx,%r13,1),%rdi
 	mov    %rbx,%rsi
 	sub    %rbx,%rdx
 	call   31f0 <memmove@plt>
 	add    $0x4,%rbp
 	mov    %r14d,(%rbx)
 	cmp    %r12,%rbp
-	je     1338e <sort_int+0xce>
+	je     1334e <sort_int+0xce>
 	mov    0x0(%rbp),%r14d
 	cmp    (%rbx),%r14d
-	jl     13330 <sort_int+0x70>
+	jl     132f0 <sort_int+0x70>
 	mov    -0x4(%rbp),%edx
 	lea    -0x4(%rbp),%rax
 	cmp    %edx,%r14d
-	jge    135b1 <sort_int+0x2f1>
+	jge    13571 <sort_int+0x2f1>
 	nopl   0x0(%rax)
 	mov    %edx,0x4(%rax)
 	mov    %rax,%rcx
 	mov    -0x4(%rax),%edx
 	sub    $0x4,%rax
 	cmp    %edx,%r14d
-	jl     13370 <sort_int+0xb0>
+	jl     13330 <sort_int+0xb0>
 	add    $0x4,%rbp
 	mov    %r14d,(%rcx)
 	cmp    %r12,%rbp
-	jne    13353 <sort_int+0x93>
+	jne    13313 <sort_int+0x93>
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopl   (%rax)
 	cmp    %r12,%rdi
-	je     1338e <sort_int+0xce>
+	je     1334e <sort_int+0xce>
 	mov    %r13,%rax
 	mov    $0x3f,%edx
 	lea    0x4(%rbx),%rbp
 	mov    %r12,%rsi
 	sar    $0x2,%rax
 	bsr    %rax,%rax
 	xor    $0x3f,%rax
 	sub    %eax,%edx
 	movslq %edx,%rdx
 	add    %rdx,%rdx
 	call   3150 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)@plt>
 	cmp    $0x40,%r13
-	jg     134fb <sort_int+0x23b>
+	jg     134bb <sort_int+0x23b>
 	cmp    %r12,%rbp
-	je     1338e <sort_int+0xce>
+	je     1334e <sort_int+0xce>
 	mov    $0x4,%r13d
-	jmp    1340b <sort_int+0x14b>
+	jmp    133cb <sort_int+0x14b>
 	nopl   0x0(%rax)
 	cmp    %rbp,%rbx
-	je     133ff <sort_int+0x13f>
+	je     133bf <sort_int+0x13f>
 	mov    %rbp,%rdx
 	lea    (%rbx,%r13,1),%rdi
 	mov    %rbx,%rsi
 	sub    %rbx,%rdx
 	call   31f0 <memmove@plt>
 	mov    %r14d,(%rbx)
 	add    $0x4,%rbp
 	cmp    %r12,%rbp
-	je     1338e <sort_int+0xce>
+	je     1334e <sort_int+0xce>
 	mov    0x0(%rbp),%r14d
 	cmp    (%rbx),%r14d
-	jg     133e8 <sort_int+0x128>
+	jg     133a8 <sort_int+0x128>
 	mov    -0x4(%rbp),%edx
 	lea    -0x4(%rbp),%rax
 	cmp    %edx,%r14d
-	jle    135be <sort_int+0x2fe>
+	jle    1357e <sort_int+0x2fe>
 	nopl   0x0(%rax)
 	mov    %edx,0x4(%rax)
 	mov    %rax,%rcx
 	mov    -0x4(%rax),%edx
 	sub    $0x4,%rax
 	cmp    %edx,%r14d
-	jg     13428 <sort_int+0x168>
+	jg     133e8 <sort_int+0x168>
 	mov    %r14d,(%rcx)
-	jmp    13402 <sort_int+0x142>
+	jmp    133c2 <sort_int+0x142>
 	nop
 	lea    0x40(%rbx),%r13
 	mov    $0x4,%r14d
-	jmp    13473 <sort_int+0x1b3>
+	jmp    13433 <sort_int+0x1b3>
 	nopl   0x0(%rax)
 	cmp    %rbp,%rbx
-	je     13467 <sort_int+0x1a7>
+	je     13427 <sort_int+0x1a7>
 	mov    %rbp,%rdx
 	lea    (%rbx,%r14,1),%rdi
 	mov    %rbx,%rsi
 	sub    %rbx,%rdx
 	call   31f0 <memmove@plt>
 	add    $0x4,%rbp
 	mov    %r15d,(%rbx)
 	cmp    %rbp,%r13
-	je     134b0 <sort_int+0x1f0>
+	je     13470 <sort_int+0x1f0>
 	mov    0x0(%rbp),%r15d
 	cmp    (%rbx),%r15d
-	jl     13450 <sort_int+0x190>
+	jl     13410 <sort_int+0x190>
 	mov    -0x4(%rbp),%edx
 	lea    -0x4(%rbp),%rax
 	cmp    %edx,%r15d
-	jge    135a9 <sort_int+0x2e9>
+	jge    13569 <sort_int+0x2e9>
 	nopl   0x0(%rax)
 	mov    %edx,0x4(%rax)
 	mov    %rax,%rcx
 	mov    -0x4(%rax),%edx
 	sub    $0x4,%rax
 	cmp    %edx,%r15d
-	jl     13490 <sort_int+0x1d0>
+	jl     13450 <sort_int+0x1d0>
 	add    $0x4,%rbp
 	mov    %r15d,(%rcx)
 	cmp    %rbp,%r13
-	jne    13473 <sort_int+0x1b3>
+	jne    13433 <sort_int+0x1b3>
 	xchg   %ax,%ax
 	cmp    %r12,%r13
-	je     1338e <sort_int+0xce>
+	je     1334e <sort_int+0xce>
 	mov    0x0(%r13),%ecx
 	mov    -0x4(%r13),%edx
 	lea    -0x4(%r13),%rax
 	cmp    %edx,%ecx
-	jge    134f0 <sort_int+0x230>
+	jge    134b0 <sort_int+0x230>
 	nopl   0x0(%rax)
 	mov    %edx,0x4(%rax)
 	mov    %rax,%rsi
 	mov    -0x4(%rax),%edx
 	sub    $0x4,%rax
 	cmp    %edx,%ecx
-	jl     134d0 <sort_int+0x210>
+	jl     13490 <sort_int+0x210>
 	mov    %ecx,(%rsi)
 	add    $0x4,%r13
-	jmp    134b0 <sort_int+0x1f0>
+	jmp    13470 <sort_int+0x1f0>
 	nopl   0x0(%rax)
 	mov    %r13,%rsi
 	add    $0x4,%r13
 	mov    %ecx,(%rsi)
-	jmp    134b0 <sort_int+0x1f0>
+	jmp    13470 <sort_int+0x1f0>
 	lea    0x40(%rbx),%r14
 	mov    $0x4,%r13d
-	jmp    13533 <sort_int+0x273>
+	jmp    134f3 <sort_int+0x273>
 	nopw   0x0(%rax,%rax,1)
 	cmp    %rbp,%rbx
-	je     13527 <sort_int+0x267>
+	je     134e7 <sort_int+0x267>
 	mov    %rbp,%rdx
 	lea    (%rbx,%r13,1),%rdi
 	mov    %rbx,%rsi
 	sub    %rbx,%rdx
 	call   31f0 <memmove@plt>
 	mov    %r15d,(%rbx)
 	add    $0x4,%rbp
 	cmp    %rbp,%r14
-	je     13570 <sort_int+0x2b0>
+	je     13530 <sort_int+0x2b0>
 	mov    0x0(%rbp),%r15d
 	cmp    (%rbx),%r15d
-	jg     13510 <sort_int+0x250>
+	jg     134d0 <sort_int+0x250>
 	mov    -0x4(%rbp),%edx
 	lea    -0x4(%rbp),%rax
 	cmp    %edx,%r15d
-	jle    135b9 <sort_int+0x2f9>
+	jle    13579 <sort_int+0x2f9>
 	nopl   0x0(%rax,%rax,1)
 	mov    %edx,0x4(%rax)
 	mov    %rax,%rcx
 	mov    -0x4(%rax),%edx
 	sub    $0x4,%rax
 	cmp    %edx,%r15d
-	jg     13550 <sort_int+0x290>
+	jg     13510 <sort_int+0x290>
 	mov    %r15d,(%rcx)
-	jmp    1352a <sort_int+0x26a>
+	jmp    134ea <sort_int+0x26a>
 	mov    %r14,%rsi
 	add    $0x4,%r14
 	mov    %ecx,(%rsi)
 	cmp    %r12,%r14
-	je     1338e <sort_int+0xce>
+	je     1334e <sort_int+0xce>
 	mov    (%r14),%ecx
 	mov    -0x4(%r14),%edx
 	lea    -0x4(%r14),%rax
 	cmp    %edx,%ecx
-	jle    13567 <sort_int+0x2a7>
+	jle    13527 <sort_int+0x2a7>
 	nopl   0x0(%rax,%rax,1)
 	mov    %edx,0x4(%rax)
 	mov    %rax,%rsi
 	mov    -0x4(%rax),%edx
 	sub    $0x4,%rax
 	cmp    %edx,%ecx
-	jg     13590 <sort_int+0x2d0>
+	jg     13550 <sort_int+0x2d0>
 	mov    %ecx,(%rsi)
 	add    $0x4,%r14
-	jmp    13570 <sort_int+0x2b0>
+	jmp    13530 <sort_int+0x2b0>
 	mov    %rbp,%rcx
-	jmp    134a2 <sort_int+0x1e2>
+	jmp    13462 <sort_int+0x1e2>
 	mov    %rbp,%rcx
-	jmp    13382 <sort_int+0xc2>
+	jmp    13342 <sort_int+0xc2>
 	mov    %rbp,%rcx
-	jmp    13562 <sort_int+0x2a2>
+	jmp    13522 <sort_int+0x2a2>
 	mov    %rbp,%rcx
-	jmp    1343a <sort_int+0x17a>
+	jmp    133fa <sort_int+0x17a>
 	cs nopw 0x0(%rax,%rax,1)
 
-00000000000135d0 <sort_longint>:
+0000000000013590 <sort_longint>:
 sort_longint():
 	push   %r15
 	movslq %esi,%rsi
 	push   %r14
 	push   %r13
 	lea    0x0(,%rsi,8),%r13
 	push   %r12
 	lea    (%rdi,%r13,1),%r12
 	push   %rbp
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x8,%rsp
 	test   %dl,%dl
-	jne    136c0 <sort_longint+0xf0>
+	jne    13680 <sort_longint+0xf0>
 	cmp    %r12,%rdi
-	je     136a8 <sort_longint+0xd8>
+	je     13668 <sort_longint+0xd8>
 	mov    %r13,%rax
 	mov    $0x3f,%edx
 	lea    0x8(%rbx),%rbp
 	mov    %r12,%rsi
 	sar    $0x3,%rax
 	bsr    %rax,%rax
 	xor    $0x3f,%rax
 	sub    %eax,%edx
 	movslq %edx,%rdx
 	add    %rdx,%rdx
-	call   e9f0 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
+	call   e9b0 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_less_iter>(long*, long*, long, __gnu_cxx::__ops::_Iter_less_iter) [clone .isra.0]>
 	cmp    $0x80,%r13
-	jg     13778 <sort_longint+0x1a8>
+	jg     13738 <sort_longint+0x1a8>
 	cmp    %r12,%rbp
-	je     136a8 <sort_longint+0xd8>
+	je     13668 <sort_longint+0xd8>
 	mov    $0x8,%r13d
-	jmp    1366b <sort_longint+0x9b>
+	jmp    1362b <sort_longint+0x9b>
 	nopl   0x0(%rax,%rax,1)
 	cmp    %rbp,%rbx
-	je     1365f <sort_longint+0x8f>
+	je     1361f <sort_longint+0x8f>
 	mov    %rbp,%rdx
 	lea    (%rbx,%r13,1),%rdi
 	mov    %rbx,%rsi
 	sub    %rbx,%rdx
 	call   31f0 <memmove@plt>
 	add    $0x8,%rbp
 	mov    %r14,(%rbx)
 	cmp    %r12,%rbp
-	je     136a8 <sort_longint+0xd8>
+	je     13668 <sort_longint+0xd8>
 	mov    0x0(%rbp),%r14
 	cmp    (%rbx),%r14
-	jl     13648 <sort_longint+0x78>
+	jl     13608 <sort_longint+0x78>
 	mov    -0x8(%rbp),%rdx
 	lea    -0x8(%rbp),%rax
 	cmp    %rdx,%r14
-	jge    138fd <sort_longint+0x32d>
+	jge    138bd <sort_longint+0x32d>
 	nopl   (%rax)
 	mov    %rdx,0x8(%rax)
 	mov    %rax,%rcx
 	mov    -0x8(%rax),%rdx
 	sub    $0x8,%rax
 	cmp    %rdx,%r14
-	jl     13688 <sort_longint+0xb8>
+	jl     13648 <sort_longint+0xb8>
 	add    $0x8,%rbp
 	mov    %r14,(%rcx)
 	cmp    %r12,%rbp
-	jne    1366b <sort_longint+0x9b>
+	jne    1362b <sort_longint+0x9b>
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopw   0x0(%rax,%rax,1)
 	cmp    %r12,%rdi
-	je     136a8 <sort_longint+0xd8>
+	je     13668 <sort_longint+0xd8>
 	mov    %r13,%rax
 	mov    $0x3f,%edx
 	lea    0x8(%rbx),%rbp
 	mov    %r12,%rsi
 	sar    $0x3,%rax
 	bsr    %rax,%rax
 	xor    $0x3f,%rax
 	sub    %eax,%edx
 	movslq %edx,%rdx
 	add    %rdx,%rdx
 	call   32a0 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)@plt>
 	cmp    $0x80,%r13
-	jg     1383c <sort_longint+0x26c>
+	jg     137fc <sort_longint+0x26c>
 	cmp    %r12,%rbp
-	je     136a8 <sort_longint+0xd8>
+	je     13668 <sort_longint+0xd8>
 	mov    $0x8,%r13d
-	jmp    13737 <sort_longint+0x167>
+	jmp    136f7 <sort_longint+0x167>
 	nopw   0x0(%rax,%rax,1)
 	cmp    %rbp,%rbx
-	je     13727 <sort_longint+0x157>
+	je     136e7 <sort_longint+0x157>
 	mov    %rbp,%rdx
 	lea    (%rbx,%r13,1),%rdi
 	mov    %rbx,%rsi
 	sub    %rbx,%rdx
 	call   31f0 <memmove@plt>
 	mov    %r14,(%rbx)
 	add    $0x8,%rbp
 	cmp    %r12,%rbp
-	je     136a8 <sort_longint+0xd8>
+	je     13668 <sort_longint+0xd8>
 	mov    0x0(%rbp),%r14
 	cmp    (%rbx),%r14
-	jg     13710 <sort_longint+0x140>
+	jg     136d0 <sort_longint+0x140>
 	mov    -0x8(%rbp),%rdx
 	lea    -0x8(%rbp),%rax
 	cmp    %rdx,%r14
-	jle    1390a <sort_longint+0x33a>
+	jle    138ca <sort_longint+0x33a>
 	nopl   0x0(%rax)
 	mov    %rdx,0x8(%rax)
 	mov    %rax,%rcx
 	mov    -0x8(%rax),%rdx
 	sub    $0x8,%rax
 	cmp    %rdx,%r14
-	jg     13758 <sort_longint+0x188>
+	jg     13718 <sort_longint+0x188>
 	mov    %r14,(%rcx)
-	jmp    1372a <sort_longint+0x15a>
+	jmp    136ea <sort_longint+0x15a>
 	nopl   0x0(%rax)
 	lea    0x80(%rbx),%r13
 	mov    $0x8,%r14d
-	jmp    137b3 <sort_longint+0x1e3>
+	jmp    13773 <sort_longint+0x1e3>
 	nopw   0x0(%rax,%rax,1)
 	cmp    %rbp,%rbx
-	je     137a7 <sort_longint+0x1d7>
+	je     13767 <sort_longint+0x1d7>
 	mov    %rbp,%rdx
 	lea    (%rbx,%r14,1),%rdi
 	mov    %rbx,%rsi
 	sub    %rbx,%rdx
 	call   31f0 <memmove@plt>
 	add    $0x8,%rbp
 	mov    %r15,(%rbx)
 	cmp    %rbp,%r13
-	je     137f0 <sort_longint+0x220>
+	je     137b0 <sort_longint+0x220>
 	mov    0x0(%rbp),%r15
 	cmp    (%rbx),%r15
-	jl     13790 <sort_longint+0x1c0>
+	jl     13750 <sort_longint+0x1c0>
 	mov    -0x8(%rbp),%rdx
 	lea    -0x8(%rbp),%rax
 	cmp    %rdx,%r15
-	jge    138f5 <sort_longint+0x325>
+	jge    138b5 <sort_longint+0x325>
 	nopl   (%rax)
 	mov    %rdx,0x8(%rax)
 	mov    %rax,%rcx
 	mov    -0x8(%rax),%rdx
 	sub    $0x8,%rax
 	cmp    %rdx,%r15
-	jl     137d0 <sort_longint+0x200>
+	jl     13790 <sort_longint+0x200>
 	add    $0x8,%rbp
 	mov    %r15,(%rcx)
 	cmp    %rbp,%r13
-	jne    137b3 <sort_longint+0x1e3>
+	jne    13773 <sort_longint+0x1e3>
 	cmp    %r12,%r13
-	je     136a8 <sort_longint+0xd8>
+	je     13668 <sort_longint+0xd8>
 	mov    0x0(%r13),%rcx
 	mov    -0x8(%r13),%rdx
 	lea    -0x8(%r13),%rax
 	cmp    %rdx,%rcx
-	jge    13830 <sort_longint+0x260>
+	jge    137f0 <sort_longint+0x260>
 	nopw   0x0(%rax,%rax,1)
 	mov    %rdx,0x8(%rax)
 	mov    %rax,%rsi
 	mov    -0x8(%rax),%rdx
 	sub    $0x8,%rax
 	cmp    %rdx,%rcx
-	jl     13810 <sort_longint+0x240>
+	jl     137d0 <sort_longint+0x240>
 	mov    %rcx,(%rsi)
 	add    $0x8,%r13
-	jmp    137f0 <sort_longint+0x220>
+	jmp    137b0 <sort_longint+0x220>
 	nopl   (%rax)
 	mov    %r13,%rsi
 	add    $0x8,%r13
 	mov    %rcx,(%rsi)
-	jmp    137f0 <sort_longint+0x220>
+	jmp    137b0 <sort_longint+0x220>
 	lea    0x80(%rbx),%r14
 	mov    $0x8,%r13d
-	jmp    13873 <sort_longint+0x2a3>
+	jmp    13833 <sort_longint+0x2a3>
 	nopl   0x0(%rax,%rax,1)
 	cmp    %rbp,%rbx
-	je     13867 <sort_longint+0x297>
+	je     13827 <sort_longint+0x297>
 	mov    %rbp,%rdx
 	lea    (%rbx,%r13,1),%rdi
 	mov    %rbx,%rsi
 	sub    %rbx,%rdx
 	call   31f0 <memmove@plt>
 	mov    %r15,(%rbx)
 	add    $0x8,%rbp
 	cmp    %rbp,%r14
-	je     138b8 <sort_longint+0x2e8>
+	je     13878 <sort_longint+0x2e8>
 	mov    0x0(%rbp),%r15
 	cmp    (%rbx),%r15
-	jg     13850 <sort_longint+0x280>
+	jg     13810 <sort_longint+0x280>
 	mov    -0x8(%rbp),%rdx
 	lea    -0x8(%rbp),%rax
 	cmp    %rdx,%r15
-	jle    13905 <sort_longint+0x335>
+	jle    138c5 <sort_longint+0x335>
 	nopl   0x0(%rax)
 	mov    %rdx,0x8(%rax)
 	mov    %rax,%rcx
 	mov    -0x8(%rax),%rdx
 	sub    $0x8,%rax
 	cmp    %rdx,%r15
-	jg     13890 <sort_longint+0x2c0>
+	jg     13850 <sort_longint+0x2c0>
 	mov    %r15,(%rcx)
-	jmp    1386a <sort_longint+0x29a>
+	jmp    1382a <sort_longint+0x29a>
 	mov    %r14,%rsi
 	add    $0x8,%r14
 	mov    %rcx,(%rsi)
 	nopl   0x0(%rax,%rax,1)
 	cmp    %r12,%r14
-	je     136a8 <sort_longint+0xd8>
+	je     13668 <sort_longint+0xd8>
 	mov    (%r14),%rcx
 	mov    -0x8(%r14),%rdx
 	lea    -0x8(%r14),%rax
 	cmp    %rdx,%rcx
-	jle    138a9 <sort_longint+0x2d9>
+	jle    13869 <sort_longint+0x2d9>
 	nopl   0x0(%rax)
 	mov    %rdx,0x8(%rax)
 	mov    %rax,%rsi
 	mov    -0x8(%rax),%rdx
 	sub    $0x8,%rax
 	cmp    %rdx,%rcx
-	jg     138d8 <sort_longint+0x308>
+	jg     13898 <sort_longint+0x308>
 	mov    %rcx,(%rsi)
 	add    $0x8,%r14
-	jmp    138b8 <sort_longint+0x2e8>
+	jmp    13878 <sort_longint+0x2e8>
 	mov    %rbp,%rcx
-	jmp    137e4 <sort_longint+0x214>
+	jmp    137a4 <sort_longint+0x214>
 	mov    %rbp,%rcx
-	jmp    1369c <sort_longint+0xcc>
+	jmp    1365c <sort_longint+0xcc>
 	mov    %rbp,%rcx
-	jmp    138a4 <sort_longint+0x2d4>
+	jmp    13864 <sort_longint+0x2d4>
 	mov    %rbp,%rcx
-	jmp    1376c <sort_longint+0x19c>
+	jmp    1372c <sort_longint+0x19c>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
-0000000000013920 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]>:
+00000000000138e0 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]>:
 void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]:
 	lea    -0x1(%rdx),%rax
 	push   %rbp
 	mov    %rdx,%rbp
 	mov    %rsi,%r8
 	mov    %rax,%r11
 	push   %rbx
 	mov    %rcx,%r9
 	mov    %rdx,%rbx
 	shr    $0x3f,%r11
 	and    $0x1,%ebp
 	add    %rax,%r11
 	sar    %r11
 	cmp    %r11,%rsi
-	jl     13967 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0x47>
-	jmp    139f0 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0xd0>
+	jl     13927 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0x47>
+	jmp    139b0 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0xd0>
 	nopl   0x0(%rax)
 	sub    $0x1,%rax
 	lea    (%rdi,%rax,8),%rcx
 	mov    (%rcx),%rdx
 	mov    %rdx,(%rdi,%rsi,8)
 	cmp    %r11,%rax
-	jge    1398a <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0x6a>
+	jge    1394a <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0x6a>
 	mov    %rax,%rsi
 	lea    0x1(%rsi),%rdx
 	lea    (%rdx,%rdx,1),%rax
 	shl    $0x4,%rdx
 	lea    (%rdi,%rdx,1),%rcx
 	mov    (%rcx),%r10
 	cmp    -0x8(%rdi,%rdx,1),%r10
-	jg     13950 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0x30>
+	jg     13910 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0x30>
 	mov    %r10,(%rdi,%rsi,8)
 	cmp    %r11,%rax
-	jl     13964 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0x44>
+	jl     13924 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0x44>
 	test   %rbp,%rbp
-	je     13a00 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0xe0>
+	je     139c0 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0xe0>
 	lea    -0x1(%rax),%rdx
 	mov    %rdx,%rsi
 	shr    $0x3f,%rsi
 	add    %rdx,%rsi
 	sar    %rsi
 	cmp    %r8,%rax
-	jg     139d2 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0xb2>
-	jmp    139e2 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0xc2>
+	jg     13992 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0xb2>
+	jmp    139a2 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0xc2>
 	nopw   0x0(%rax,%rax,1)
 	mov    %rdx,(%rcx)
 	lea    -0x1(%rsi),%rdx
 	mov    %rdx,%rax
 	shr    $0x3f,%rax
 	add    %rdx,%rax
 	sar    %rax
 	mov    %rax,%rdx
 	mov    %rsi,%rax
 	cmp    %rsi,%r8
-	jge    13a38 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0x118>
+	jge    139f8 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0x118>
 	mov    %rdx,%rsi
 	lea    (%rdi,%rsi,8),%r10
 	lea    (%rdi,%rax,8),%rcx
 	mov    (%r10),%rdx
 	cmp    %r9,%rdx
-	jg     139b0 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0x90>
+	jg     13970 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0x90>
 	mov    %r9,(%rcx)
 	pop    %rbx
 	pop    %rbp
 	ret
 	nopl   0x0(%rax,%rax,1)
 	lea    (%rdi,%rsi,8),%rcx
 	test   %rbp,%rbp
-	jne    139e2 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0xc2>
+	jne    139a2 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0xc2>
 	mov    %r8,%rax
 	nopl   0x0(%rax)
 	lea    -0x2(%rbx),%rdx
 	mov    %rdx,%rbx
 	shr    $0x3f,%rbx
 	add    %rdx,%rbx
 	sar    %rbx
 	cmp    %rbx,%rax
-	jne    1398f <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0x6f>
+	jne    1394f <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0x6f>
 	lea    0x2(%rax,%rax,1),%rax
 	mov    -0x8(%rdi,%rax,8),%rdx
 	sub    $0x1,%rax
 	mov    %rdx,(%rcx)
 	lea    (%rdi,%rax,8),%rcx
-	jmp    1398f <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0x6f>
+	jmp    1394f <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]+0x6f>
 	nopl   0x0(%rax)
 	mov    %r10,%rcx
 	mov    %r9,(%rcx)
 	pop    %rbx
 	pop    %rbp
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax,%rax,1)
 
-0000000000013a50 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]>:
+0000000000013a10 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]>:
 void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]:
 	lea    -0x1(%rdx),%rax
 	push   %rbp
 	mov    %rdx,%rbp
 	mov    %rsi,%r8
 	mov    %rax,%r11
 	push   %rbx
 	mov    %ecx,%r9d
 	mov    %rdx,%rbx
 	shr    $0x3f,%r11
 	and    $0x1,%ebp
 	add    %rax,%r11
 	sar    %r11
 	cmp    %r11,%rsi
-	jl     13a95 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0x45>
-	jmp    13b10 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0xc0>
+	jl     13a55 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0x45>
+	jmp    13ad0 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0xc0>
 	nopl   0x0(%rax)
 	sub    $0x1,%rax
 	lea    (%rdi,%rax,4),%rcx
 	mov    (%rcx),%edx
 	mov    %edx,(%rdi,%rsi,4)
 	cmp    %r11,%rax
-	jge    13ab8 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0x68>
+	jge    13a78 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0x68>
 	mov    %rax,%rsi
 	lea    0x1(%rsi),%rdx
 	lea    (%rdx,%rdx,1),%rax
 	shl    $0x3,%rdx
 	lea    (%rdi,%rdx,1),%rcx
 	mov    (%rcx),%r10d
 	cmp    -0x4(%rdi,%rdx,1),%r10d
-	jg     13a80 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0x30>
+	jg     13a40 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0x30>
 	mov    %r10d,(%rdi,%rsi,4)
 	cmp    %r11,%rax
-	jl     13a92 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0x42>
+	jl     13a52 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0x42>
 	test   %rbp,%rbp
-	je     13b20 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0xd0>
+	je     13ae0 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0xd0>
 	lea    -0x1(%rax),%rdx
 	mov    %rdx,%rsi
 	shr    $0x3f,%rsi
 	add    %rdx,%rsi
 	sar    %rsi
 	cmp    %r8,%rax
-	jg     13af9 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0xa9>
-	jmp    13b09 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0xb9>
+	jg     13ab9 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0xa9>
+	jmp    13ac9 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0xb9>
 	nopl   (%rax)
 	mov    %edx,(%rcx)
 	lea    -0x1(%rsi),%rdx
 	mov    %rdx,%rax
 	shr    $0x3f,%rax
 	add    %rdx,%rax
 	sar    %rax
 	mov    %rax,%rdx
 	mov    %rsi,%rax
 	cmp    %rsi,%r8
-	jge    13b50 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0x100>
+	jge    13b10 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0x100>
 	mov    %rdx,%rsi
 	lea    (%rdi,%rsi,4),%r10
 	lea    (%rdi,%rax,4),%rcx
 	mov    (%r10),%edx
 	cmp    %r9d,%edx
-	jg     13ad8 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0x88>
+	jg     13a98 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0x88>
 	mov    %r9d,(%rcx)
 	pop    %rbx
 	pop    %rbp
 	ret
 	nop
 	lea    (%rdi,%rsi,4),%rcx
 	test   %rbp,%rbp
-	jne    13b09 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0xb9>
+	jne    13ac9 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0xb9>
 	mov    %r8,%rax
 	nopl   0x0(%rax)
 	lea    -0x2(%rbx),%rdx
 	mov    %rdx,%rbx
 	shr    $0x3f,%rbx
 	add    %rdx,%rbx
 	sar    %rbx
 	cmp    %rbx,%rax
-	jne    13abd <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0x6d>
+	jne    13a7d <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0x6d>
 	lea    0x2(%rax,%rax,1),%rax
 	mov    -0x4(%rdi,%rax,4),%edx
 	sub    $0x1,%rax
 	mov    %edx,(%rcx)
 	lea    (%rdi,%rax,4),%rcx
-	jmp    13abd <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0x6d>
+	jmp    13a7d <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]+0x6d>
 	xchg   %ax,%ax
 	mov    %r10,%rcx
 	mov    %r9d,(%rcx)
 	pop    %rbx
 	pop    %rbp
 	ret
 	nopl   0x0(%rax)
 
-0000000000013b60 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]>:
+0000000000013b20 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]>:
 void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]:
 	lea    -0x1(%rdx),%rax
 	mov    %rdx,%r11
 	mov    %rsi,%r8
 	mov    %rdx,%r10
 	mov    %rax,%r9
 	movaps %xmm0,%xmm1
 	and    $0x1,%r11d
 	shr    $0x3f,%r9
 	add    %rax,%r9
 	sar    %r9
 	cmp    %r9,%rsi
-	jl     13ba9 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0x49>
-	jmp    13c30 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0xd0>
+	jl     13b69 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0x49>
+	jmp    13bf0 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0xd0>
 	nopl   0x0(%rax,%rax,1)
 	sub    $0x1,%rax
 	lea    (%rdi,%rax,4),%rcx
 	movss  (%rcx),%xmm0
 	movss  %xmm0,(%rdi,%rsi,4)
 	cmp    %r9,%rax
-	jge    13bce <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0x6e>
+	jge    13b8e <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0x6e>
 	mov    %rax,%rsi
 	lea    0x1(%rsi),%rdx
 	lea    (%rdx,%rdx,1),%rax
 	shl    $0x3,%rdx
 	lea    (%rdi,%rdx,1),%rcx
 	movss  (%rcx),%xmm0
 	comiss -0x4(%rdi,%rdx,1),%xmm0
-	ja     13b90 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0x30>
+	ja     13b50 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0x30>
 	movss  %xmm0,(%rdi,%rsi,4)
 	cmp    %r9,%rax
-	jl     13ba6 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0x46>
+	jl     13b66 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0x46>
 	test   %r11,%r11
-	je     13c40 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0xe0>
+	je     13c00 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0xe0>
 	lea    -0x1(%rax),%rdx
 	mov    %rdx,%rsi
 	shr    $0x3f,%rsi
 	add    %rdx,%rsi
 	sar    %rsi
 	cmp    %r8,%rax
-	jg     13c13 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0xb3>
-	jmp    13c25 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0xc5>
+	jg     13bd3 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0xb3>
+	jmp    13be5 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0xc5>
 	nopl   0x0(%rax,%rax,1)
 	lea    -0x1(%rsi),%rdx
 	movss  %xmm0,(%rcx)
 	mov    %rdx,%rax
 	shr    $0x3f,%rax
 	add    %rdx,%rax
 	sar    %rax
 	mov    %rax,%rdx
 	mov    %rsi,%rax
 	cmp    %rsi,%r8
-	jge    13c80 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0x120>
+	jge    13c40 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0x120>
 	mov    %rdx,%rsi
 	lea    (%rdi,%rsi,4),%r9
 	lea    (%rdi,%rax,4),%rcx
 	movss  (%r9),%xmm0
 	comiss %xmm1,%xmm0
-	ja     13bf0 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0x90>
+	ja     13bb0 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0x90>
 	movss  %xmm1,(%rcx)
 	ret
 	nopw   0x0(%rax,%rax,1)
 	lea    (%rdi,%rsi,4),%rcx
 	test   %r11,%r11
-	jne    13c25 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0xc5>
+	jne    13be5 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0xc5>
 	mov    %r8,%rax
 	nopl   0x0(%rax)
 	sub    $0x2,%r10
 	mov    %r10,%rdx
 	shr    $0x3f,%rdx
 	add    %rdx,%r10
 	sar    %r10
 	cmp    %r10,%rax
-	jne    13bd3 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0x73>
+	jne    13b93 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0x73>
 	lea    0x2(%rax,%rax,1),%rax
 	movss  -0x4(%rdi,%rax,4),%xmm0
 	sub    $0x1,%rax
 	movss  %xmm0,(%rcx)
 	lea    (%rdi,%rax,4),%rcx
-	jmp    13bd3 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0x73>
+	jmp    13b93 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]+0x73>
 	cs nopw 0x0(%rax,%rax,1)
 	mov    %r9,%rcx
 	movss  %xmm1,(%rcx)
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-0000000000013c90 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]>:
+0000000000013c50 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]>:
 void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]:
 	lea    -0x1(%rdx),%rax
 	mov    %rdx,%r11
 	mov    %rsi,%r8
 	mov    %rdx,%r10
 	mov    %rax,%r9
 	movapd %xmm0,%xmm1
 	and    $0x1,%r11d
 	shr    $0x3f,%r9
 	add    %rax,%r9
 	sar    %r9
 	cmp    %r9,%rsi
-	jl     13cd9 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0x49>
-	jmp    13d60 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0xd0>
+	jl     13c99 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0x49>
+	jmp    13d20 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0xd0>
 	nopl   0x0(%rax)
 	sub    $0x1,%rax
 	lea    (%rdi,%rax,8),%rcx
 	movsd  (%rcx),%xmm0
 	movsd  %xmm0,(%rdi,%rsi,8)
 	cmp    %r9,%rax
-	jge    13cff <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0x6f>
+	jge    13cbf <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0x6f>
 	mov    %rax,%rsi
 	lea    0x1(%rsi),%rdx
 	lea    (%rdx,%rdx,1),%rax
 	shl    $0x4,%rdx
 	lea    (%rdi,%rdx,1),%rcx
 	movsd  (%rcx),%xmm0
 	comisd -0x8(%rdi,%rdx,1),%xmm0
-	ja     13cc0 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0x30>
+	ja     13c80 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0x30>
 	movsd  %xmm0,(%rdi,%rsi,8)
 	cmp    %r9,%rax
-	jl     13cd6 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0x46>
+	jl     13c96 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0x46>
 	test   %r11,%r11
-	je     13d70 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0xe0>
+	je     13d30 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0xe0>
 	lea    -0x1(%rax),%rdx
 	mov    %rdx,%rsi
 	shr    $0x3f,%rsi
 	add    %rdx,%rsi
 	sar    %rsi
 	cmp    %r8,%rax
-	jg     13d43 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0xb3>
-	jmp    13d56 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0xc6>
+	jg     13d03 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0xb3>
+	jmp    13d16 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0xc6>
 	nopl   0x0(%rax)
 	lea    -0x1(%rsi),%rdx
 	movsd  %xmm0,(%rcx)
 	mov    %rdx,%rax
 	shr    $0x3f,%rax
 	add    %rdx,%rax
 	sar    %rax
 	mov    %rax,%rdx
 	mov    %rsi,%rax
 	cmp    %rsi,%r8
-	jge    13db0 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0x120>
+	jge    13d70 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0x120>
 	mov    %rdx,%rsi
 	lea    (%rdi,%rsi,8),%r9
 	lea    (%rdi,%rax,8),%rcx
 	movsd  (%r9),%xmm0
 	comisd %xmm1,%xmm0
-	ja     13d20 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0x90>
+	ja     13ce0 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0x90>
 	movsd  %xmm1,(%rcx)
 	ret
 	nopl   0x0(%rax,%rax,1)
 	lea    (%rdi,%rsi,8),%rcx
 	test   %r11,%r11
-	jne    13d56 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0xc6>
+	jne    13d16 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0xc6>
 	mov    %r8,%rax
 	nopl   0x0(%rax)
 	sub    $0x2,%r10
 	mov    %r10,%rdx
 	shr    $0x3f,%rdx
 	add    %rdx,%r10
 	sar    %r10
 	cmp    %r10,%rax
-	jne    13d04 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0x74>
+	jne    13cc4 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0x74>
 	lea    0x2(%rax,%rax,1),%rax
 	movsd  -0x8(%rdi,%rax,8),%xmm0
 	sub    $0x1,%rax
 	movsd  %xmm0,(%rcx)
 	lea    (%rdi,%rax,8),%rcx
-	jmp    13d04 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0x74>
+	jmp    13cc4 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]+0x74>
 	cs nopw 0x0(%rax,%rax,1)
 	mov    %r9,%rcx
 	movsd  %xmm1,(%rcx)
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-0000000000013dc0 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)>:
+0000000000013d80 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)>:
 void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >):
 	mov    %rsi,%rax
 	sub    %rdi,%rax
 	cmp    $0x80,%rax
-	jle    13f7a <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x1ba>
+	jle    13f3a <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x1ba>
 	push   %r14
 	mov    %rdx,%r14
 	push   %r13
 	lea    0x8(%rdi),%r13
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	push   %rbx
 	test   %rdx,%rdx
-	je     13ef4 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x134>
+	je     13eb4 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x134>
 	sar    $0x4,%rax
 	movsd  0x8(%r12),%xmm1
 	sub    $0x1,%r14
 	movsd  -0x8(%rsi),%xmm3
 	lea    (%r12,%rax,8),%rax
 	movsd  (%r12),%xmm0
 	movsd  (%rax),%xmm2
 	comisd %xmm2,%xmm1
-	jbe    13e8d <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0xcd>
+	jbe    13e4d <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0xcd>
 	comisd %xmm3,%xmm2
-	ja     13eda <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x11a>
+	ja     13e9a <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x11a>
 	comisd %xmm3,%xmm1
-	ja     13e99 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0xd9>
+	ja     13e59 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0xd9>
 	movapd %xmm1,%xmm2
 	unpcklpd %xmm0,%xmm2
 	movups %xmm2,(%r12)
 	movsd  -0x8(%rsi),%xmm0
 	mov    %r13,%rbx
 	mov    %rsi,%rax
 	nopl   (%rax)
 	movsd  (%rbx),%xmm2
 	mov    %rbx,%rbp
 	comisd %xmm1,%xmm2
-	ja     13e87 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0xc7>
+	ja     13e47 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0xc7>
 	sub    $0x8,%rax
 	comisd %xmm0,%xmm1
-	jbe    13e6f <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0xaf>
+	jbe    13e2f <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0xaf>
 	nopw   0x0(%rax,%rax,1)
 	movsd  -0x8(%rax),%xmm0
 	sub    $0x8,%rax
 	comisd %xmm0,%xmm1
-	ja     13e60 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0xa0>
+	ja     13e20 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0xa0>
 	cmp    %rax,%rbx
-	jae    13eb0 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0xf0>
+	jae    13e70 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0xf0>
 	movsd  %xmm0,(%rbx)
 	movsd  -0x8(%rax),%xmm0
 	movsd  %xmm2,(%rax)
 	movsd  (%r12),%xmm1
 	add    $0x8,%rbx
-	jmp    13e40 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x80>
+	jmp    13e00 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x80>
 	comisd %xmm3,%xmm1
-	ja     13e25 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x65>
+	ja     13de5 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x65>
 	comisd %xmm3,%xmm2
-	jbe    13eda <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x11a>
+	jbe    13e9a <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x11a>
 	movsd  %xmm3,(%r12)
 	movsd  %xmm0,-0x8(%rsi)
 	movsd  (%r12),%xmm1
-	jmp    13e37 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x77>
+	jmp    13df7 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x77>
 	nopl   0x0(%rax)
 	mov    %r14,%rdx
 	mov    %rbx,%rdi
 	call   3250 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)@plt>
 	mov    %rbx,%rax
 	sub    %r12,%rax
 	cmp    $0x80,%rax
-	jle    13f71 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x1b1>
+	jle    13f31 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x1b1>
 	test   %r14,%r14
-	je     13ef7 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x137>
+	je     13eb7 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x137>
 	mov    %rbx,%rsi
-	jmp    13ded <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x2d>
+	jmp    13dad <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x2d>
 	movsd  %xmm2,(%r12)
 	movsd  %xmm0,(%rax)
 	movsd  (%r12),%xmm1
 	movsd  -0x8(%rsi),%xmm0
-	jmp    13e37 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x77>
+	jmp    13df7 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x77>
 	mov    %rsi,%rbp
 	sar    $0x3,%rax
 	mov    %r12,%rdi
 	lea    -0x2(%rax),%r13
 	mov    %rax,%rdx
 	mov    %rax,%rbx
 	sar    %r13
 	movsd  (%r12,%r13,8),%xmm0
 	mov    %r13,%rsi
-	call   13c90 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]>
+	call   13c50 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]>
 	sub    $0x1,%r13
 	mov    %rbx,%rdx
 	mov    %r12,%rdi
 	movsd  (%r12,%r13,8),%xmm0
 	mov    %r13,%rsi
-	call   13c90 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]>
+	call   13c50 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]>
 	test   %r13,%r13
-	jne    13f19 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x159>
+	jne    13ed9 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x159>
 	cs nopw 0x0(%rax,%rax,1)
 	sub    $0x8,%rbp
 	movsd  (%r12),%xmm1
 	xor    %esi,%esi
 	mov    %r12,%rdi
 	mov    %rbp,%rbx
 	movsd  0x0(%rbp),%xmm0
 	sub    %r12,%rbx
 	movsd  %xmm1,0x0(%rbp)
 	mov    %rbx,%rdx
 	sar    $0x3,%rdx
-	call   13c90 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]>
+	call   13c50 <void std::__adjust_heap<double*, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, long, long, double, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >) [clone .isra.0]>
 	cmp    $0x8,%rbx
-	jg     13f40 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x180>
+	jg     13f00 <void std::__introsort_loop<double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> > >(double*, double*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<double> >)+0x180>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-0000000000013f80 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)>:
+0000000000013f40 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)>:
 void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >):
 	mov    %rsi,%rax
 	sub    %rdi,%rax
 	cmp    $0x40,%rax
-	jle    1412a <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x1aa>
+	jle    140ea <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x1aa>
 	push   %r14
 	mov    %rdx,%r14
 	push   %r13
 	lea    0x4(%rdi),%r13
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	push   %rbx
 	test   %rdx,%rdx
-	je     140aa <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x12a>
+	je     1406a <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x12a>
 	sar    $0x3,%rax
 	movss  0x4(%r12),%xmm1
 	sub    $0x1,%r14
 	movss  -0x4(%rsi),%xmm3
 	lea    (%r12,%rax,4),%rax
 	movss  (%r12),%xmm0
 	movss  (%rax),%xmm2
 	comiss %xmm2,%xmm1
-	jbe    14044 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0xc4>
+	jbe    14004 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0xc4>
 	comiss %xmm3,%xmm2
-	ja     14090 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x110>
+	ja     14050 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x110>
 	comiss %xmm3,%xmm1
-	ja     1404e <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0xce>
+	ja     1400e <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0xce>
 	movss  %xmm1,(%r12)
 	movss  %xmm0,0x4(%r12)
 	movss  -0x4(%rsi),%xmm0
 	mov    %r13,%rbx
 	mov    %rsi,%rax
 	nopl   0x0(%rax,%rax,1)
 	movss  (%rbx),%xmm2
 	mov    %rbx,%rbp
 	comiss %xmm1,%xmm2
-	ja     1403e <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0xbe>
+	ja     13ffe <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0xbe>
 	sub    $0x4,%rax
 	comiss %xmm0,%xmm1
-	jbe    14026 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0xa6>
+	jbe    13fe6 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0xa6>
 	nopl   (%rax)
 	movss  -0x4(%rax),%xmm0
 	sub    $0x4,%rax
 	comiss %xmm0,%xmm1
-	ja     14018 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x98>
+	ja     13fd8 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x98>
 	cmp    %rax,%rbx
-	jae    14068 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0xe8>
+	jae    14028 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0xe8>
 	movss  %xmm0,(%rbx)
 	movss  -0x4(%rax),%xmm0
 	movss  %xmm2,(%rax)
 	movss  (%r12),%xmm1
 	add    $0x4,%rbx
-	jmp    14000 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x80>
+	jmp    13fc0 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x80>
 	comiss %xmm3,%xmm1
-	ja     13fe0 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x60>
+	ja     13fa0 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x60>
 	comiss %xmm3,%xmm2
-	jbe    14090 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x110>
+	jbe    14050 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x110>
 	movss  %xmm3,(%r12)
 	movss  %xmm0,-0x4(%rsi)
 	movss  (%r12),%xmm1
-	jmp    13ff2 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x72>
+	jmp    13fb2 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x72>
 	nopl   0x0(%rax)
 	mov    %r14,%rdx
 	mov    %rbx,%rdi
 	call   3080 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)@plt>
 	mov    %rbx,%rax
 	sub    %r12,%rax
 	cmp    $0x40,%rax
-	jle    14121 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x1a1>
+	jle    140e1 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x1a1>
 	test   %r14,%r14
-	je     140ad <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x12d>
+	je     1406d <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x12d>
 	mov    %rbx,%rsi
-	jmp    13fab <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x2b>
+	jmp    13f6b <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x2b>
 	movss  %xmm2,(%r12)
 	movss  %xmm0,(%rax)
 	movss  (%r12),%xmm1
 	movss  -0x4(%rsi),%xmm0
-	jmp    13ff2 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x72>
+	jmp    13fb2 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x72>
 	mov    %rsi,%rbp
 	sar    $0x2,%rax
 	mov    %r12,%rdi
 	lea    -0x2(%rax),%r13
 	mov    %rax,%rdx
 	mov    %rax,%rbx
 	sar    %r13
 	movss  (%r12,%r13,4),%xmm0
 	mov    %r13,%rsi
-	call   13b60 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]>
+	call   13b20 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]>
 	sub    $0x1,%r13
 	mov    %rbx,%rdx
 	mov    %r12,%rdi
 	movss  (%r12,%r13,4),%xmm0
 	mov    %r13,%rsi
-	call   13b60 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]>
+	call   13b20 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]>
 	test   %r13,%r13
-	jne    140cf <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x14f>
+	jne    1408f <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x14f>
 	nopl   0x0(%rax)
 	sub    $0x4,%rbp
 	movss  (%r12),%xmm1
 	xor    %esi,%esi
 	mov    %r12,%rdi
 	mov    %rbp,%rbx
 	movss  0x0(%rbp),%xmm0
 	sub    %r12,%rbx
 	movss  %xmm1,0x0(%rbp)
 	mov    %rbx,%rdx
 	sar    $0x2,%rdx
-	call   13b60 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]>
+	call   13b20 <void std::__adjust_heap<float*, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, long, long, float, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >) [clone .isra.0]>
 	cmp    $0x4,%rbx
-	jg     140f0 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x170>
+	jg     140b0 <void std::__introsort_loop<float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> > >(float*, float*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<float> >)+0x170>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	ret
 	nopl   0x0(%rax,%rax,1)
 
-0000000000014130 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)>:
+00000000000140f0 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)>:
 void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >):
 	mov    %rsi,%rax
 	sub    %rdi,%rax
 	cmp    $0x40,%rax
-	jle    142e1 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x1b1>
+	jle    142a1 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x1b1>
 	push   %r14
 	mov    %rsi,%r8
 	mov    %rdx,%r14
 	push   %r13
 	mov    %rdi,%r13
 	push   %r12
 	push   %rbp
 	lea    0x4(%rdi),%rbp
 	push   %rbx
 	test   %rdx,%rdx
-	je     1424d <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x11d>
+	je     1420d <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x11d>
 	sar    $0x3,%rax
 	mov    0x4(%r13),%ecx
 	mov    -0x4(%r8),%esi
 	sub    $0x1,%r14
 	lea    0x0(%r13,%rax,4),%rdi
 	mov    0x0(%r13),%edx
 	mov    (%rdi),%eax
 	cmp    %eax,%ecx
-	jle    14213 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0xe3>
+	jle    141d3 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0xe3>
 	cmp    %esi,%eax
-	jg     1423a <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x10a>
+	jg     141fa <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x10a>
 	cmp    %esi,%ecx
-	jle    142c6 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x196>
+	jle    14286 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x196>
 	mov    %esi,0x0(%r13)
 	mov    %edx,-0x4(%r8)
 	mov    0x0(%r13),%ecx
 	mov    %rbp,%rbx
 	mov    %r8,%rax
 	nopl   0x0(%rax,%rax,1)
 	mov    (%rbx),%esi
 	mov    %rbx,%r12
 	cmp    %ecx,%esi
-	jg     141db <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0xab>
+	jg     1419b <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0xab>
 	sub    $0x4,%rax
 	cmp    %edx,%ecx
-	jle    141cb <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x9b>
+	jle    1418b <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x9b>
 	nopl   0x0(%rax)
 	mov    -0x4(%rax),%edx
 	sub    $0x4,%rax
 	cmp    %ecx,%edx
-	jl     141c0 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x90>
+	jl     14180 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x90>
 	cmp    %rax,%rbx
-	jae    141e8 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0xb8>
+	jae    141a8 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0xb8>
 	mov    %edx,(%rbx)
 	mov    -0x4(%rax),%edx
 	mov    %esi,(%rax)
 	mov    0x0(%r13),%ecx
 	add    $0x4,%rbx
-	jmp    141a8 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x78>
+	jmp    14168 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x78>
 	nopl   0x0(%rax)
 	mov    %r14,%rdx
 	mov    %r8,%rsi
 	mov    %rbx,%rdi
 	call   3150 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)@plt>
 	mov    %rbx,%rax
 	sub    %r13,%rax
 	cmp    $0x40,%rax
-	jle    142bd <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x18d>
+	jle    1427d <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x18d>
 	test   %r14,%r14
-	je     14250 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x120>
+	je     14210 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x120>
 	mov    %rbx,%r8
-	jmp    1415e <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x2e>
+	jmp    1411e <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x2e>
 	cmp    %esi,%ecx
-	jle    14232 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x102>
+	jle    141f2 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x102>
 	movd   %edx,%xmm1
 	movd   %ecx,%xmm0
 	punpckldq %xmm1,%xmm0
 	movq   %xmm0,0x0(%r13)
 	mov    -0x4(%r8),%edx
-	jmp    1419d <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x6d>
+	jmp    1415d <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x6d>
 	cmp    %esi,%eax
-	jg     14191 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x61>
+	jg     14151 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x61>
 	mov    %eax,0x0(%r13)
 	mov    %edx,(%rdi)
 	mov    0x0(%r13),%ecx
 	mov    -0x4(%r8),%edx
-	jmp    1419d <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x6d>
+	jmp    1415d <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x6d>
 	mov    %rsi,%r12
 	sar    $0x2,%rax
 	mov    %r13,%rdi
 	lea    -0x2(%rax),%rbp
 	mov    %rax,%rdx
 	mov    %rax,%rbx
 	sar    %rbp
 	mov    0x0(%r13,%rbp,4),%ecx
 	mov    %rbp,%rsi
-	call   13a50 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]>
+	call   13a10 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]>
 	sub    $0x1,%rbp
 	mov    %rbx,%rdx
 	mov    %r13,%rdi
 	mov    0x0(%r13,%rbp,4),%ecx
 	mov    %rbp,%rsi
-	call   13a50 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]>
+	call   13a10 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]>
 	test   %rbp,%rbp
-	jne    14271 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x141>
+	jne    14231 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x141>
 	nopl   (%rax)
 	sub    $0x4,%r12
 	mov    0x0(%r13),%eax
 	mov    (%r12),%ecx
 	xor    %esi,%esi
 	mov    %r12,%rbx
 	mov    %r13,%rdi
 	sub    %r13,%rbx
 	mov    %eax,(%r12)
 	mov    %rbx,%rdx
 	sar    $0x2,%rdx
-	call   13a50 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]>
+	call   13a10 <void std::__adjust_heap<int*, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, long, long, int, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >) [clone .isra.0]>
 	cmp    $0x4,%rbx
-	jg     14290 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x160>
+	jg     14250 <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x160>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	movd   %edx,%xmm2
 	movd   %ecx,%xmm0
 	punpckldq %xmm2,%xmm0
 	movq   %xmm0,0x0(%r13)
 	mov    -0x4(%r8),%edx
-	jmp    1419d <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x6d>
+	jmp    1415d <void std::__introsort_loop<int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> > >(int*, int*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<int> >)+0x6d>
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
-00000000000142f0 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)>:
+00000000000142b0 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)>:
 void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >):
 	mov    %rsi,%rax
 	sub    %rdi,%rax
 	cmp    $0x80,%rax
-	jle    144b2 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x1c2>
+	jle    14472 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x1c2>
 	push   %r14
 	mov    %rsi,%r8
 	mov    %rdx,%r14
 	push   %r13
 	mov    %rdi,%r13
 	push   %r12
 	push   %rbp
 	lea    0x8(%rdi),%rbp
 	push   %rbx
 	test   %rdx,%rdx
-	je     1441b <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x12b>
+	je     143db <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x12b>
 	sar    $0x4,%rax
 	mov    0x8(%r13),%rcx
 	mov    -0x8(%r8),%rsi
 	sub    $0x1,%r14
 	lea    0x0(%r13,%rax,8),%rdi
 	mov    0x0(%r13),%rdx
 	mov    (%rdi),%rax
 	cmp    %rax,%rcx
-	jle    143dd <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0xed>
+	jle    1439d <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0xed>
 	cmp    %rsi,%rax
-	jg     14407 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x117>
+	jg     143c7 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x117>
 	cmp    %rsi,%rcx
-	jle    14496 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x1a6>
+	jle    14456 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x1a6>
 	mov    %rsi,0x0(%r13)
 	mov    %rdx,-0x8(%r8)
 	mov    0x0(%r13),%rcx
 	mov    %rbp,%rbx
 	mov    %r8,%rax
 	nopl   0x0(%rax)
 	mov    (%rbx),%rsi
 	mov    %rbx,%r12
 	cmp    %rcx,%rsi
-	jg     143a8 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0xb8>
+	jg     14368 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0xb8>
 	sub    $0x8,%rax
 	cmp    %rdx,%rcx
-	jle    14395 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0xa5>
+	jle    14355 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0xa5>
 	nopl   0x0(%rax)
 	mov    -0x8(%rax),%rdx
 	sub    $0x8,%rax
 	cmp    %rcx,%rdx
-	jl     14388 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x98>
+	jl     14348 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x98>
 	cmp    %rax,%rbx
-	jae    143b0 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0xc0>
+	jae    14370 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0xc0>
 	mov    %rdx,(%rbx)
 	mov    -0x8(%rax),%rdx
 	mov    %rsi,(%rax)
 	mov    0x0(%r13),%rcx
 	add    $0x8,%rbx
-	jmp    14370 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x80>
+	jmp    14330 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x80>
 	xchg   %ax,%ax
 	mov    %r14,%rdx
 	mov    %r8,%rsi
 	mov    %rbx,%rdi
 	call   32a0 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)@plt>
 	mov    %rbx,%rax
 	sub    %r13,%rax
 	cmp    $0x80,%rax
-	jle    1448d <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x19d>
+	jle    1444d <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x19d>
 	test   %r14,%r14
-	je     1441e <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x12e>
+	je     143de <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x12e>
 	mov    %rbx,%r8
-	jmp    14320 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x30>
+	jmp    142e0 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x30>
 	cmp    %rsi,%rcx
-	jle    143fe <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x10e>
+	jle    143be <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x10e>
 	movq   %rdx,%xmm1
 	movq   %rcx,%xmm0
 	punpcklqdq %xmm1,%xmm0
 	movups %xmm0,0x0(%r13)
 	mov    -0x8(%r8),%rdx
-	jmp    14363 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x73>
+	jmp    14323 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x73>
 	cmp    %rsi,%rax
-	jg     14357 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x67>
+	jg     14317 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x67>
 	mov    %rax,0x0(%r13)
 	mov    %rdx,(%rdi)
 	mov    0x0(%r13),%rcx
 	mov    -0x8(%r8),%rdx
-	jmp    14363 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x73>
+	jmp    14323 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x73>
 	mov    %rsi,%r12
 	sar    $0x3,%rax
 	mov    %r13,%rdi
 	lea    -0x2(%rax),%rbp
 	mov    %rax,%rdx
 	mov    %rax,%rbx
 	sar    %rbp
 	mov    0x0(%r13,%rbp,8),%rcx
 	mov    %rbp,%rsi
-	call   13920 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]>
+	call   138e0 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]>
 	sub    $0x1,%rbp
 	mov    %rbx,%rdx
 	mov    %r13,%rdi
 	mov    0x0(%r13,%rbp,8),%rcx
 	mov    %rbp,%rsi
-	call   13920 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]>
+	call   138e0 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]>
 	test   %rbp,%rbp
-	jne    1443f <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x14f>
+	jne    143ff <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x14f>
 	nopl   0x0(%rax,%rax,1)
 	sub    $0x8,%r12
 	mov    0x0(%r13),%rax
 	mov    (%r12),%rcx
 	xor    %esi,%esi
 	mov    %r12,%rbx
 	mov    %r13,%rdi
 	sub    %r13,%rbx
 	mov    %rax,(%r12)
 	mov    %rbx,%rdx
 	sar    $0x3,%rdx
-	call   13920 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]>
+	call   138e0 <void std::__adjust_heap<long*, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long, long, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >) [clone .isra.0]>
 	cmp    $0x8,%rbx
-	jg     14460 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x170>
+	jg     14420 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x170>
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	movq   %rdx,%xmm2
 	movq   %rcx,%xmm0
 	punpcklqdq %xmm2,%xmm0
 	movups %xmm0,0x0(%r13)
 	mov    -0x8(%r8),%rdx
-	jmp    14363 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x73>
+	jmp    14323 <void std::__introsort_loop<long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> > >(long*, long*, long, __gnu_cxx::__ops::_Iter_comp_iter<std::greater<long> >)+0x73>
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-00000000000144c0 <fast_resonator_real_imag>:
+0000000000014480 <fast_resonator_real_imag>:
 fast_resonator_real_imag():
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
 	sub    $0x30,%rsp
 	mov    0x68(%rsp),%r10d
 	mov    0x70(%rsp),%eax
 	test   %r10d,%r10d
-	jle    14bee <fast_resonator_real_imag+0x72e>
+	jle    14bae <fast_resonator_real_imag+0x72e>
 	cmp    $0x1,%eax
-	jle    14bee <fast_resonator_real_imag+0x72e>
+	jle    14bae <fast_resonator_real_imag+0x72e>
 	lea    -0x1(%r10),%ebx
 	mov    %ebx,(%rsp)
 	cmp    $0x2,%r10d
-	jle    14c08 <fast_resonator_real_imag+0x748>
+	jle    14bc8 <fast_resonator_real_imag+0x748>
 	lea    -0x1(%rax),%r11d
 	lea    -0x2(%rax),%ebx
 	mov    %r10d,%r14d
-	movsd  0x3dcb(%rip),%xmm14        
-	movapd 0x3bba(%rip),%xmm10        
+	movsd  0x3e0b(%rip),%xmm14        
+	movapd 0x3bfa(%rip),%xmm10        
 	mov    %ebx,0x4(%rsp)
 	mov    %r11d,%r15d
 	mov    %r11d,%ebx
 	and    $0xfffffffc,%ebx
 	shr    $0x2,%r15d
 	movl   $0x1,-0x34(%rsp)
 	mov    %ebx,0x20(%rsp)
@@ -17300,15 +17294,15 @@
 	movsd  -0x28(%rsp),%xmm6
 	divsd  %xmm7,%xmm6
 	movsd  %xmm6,-0x10(%rsp)
 	movsd  -0x10(%rcx,%rbx,8),%xmm6
 	mulsd  %xmm6,%xmm0
 	movsd  %xmm6,-0x18(%rsp)
 	movsd  %xmm0,-0x30(%rsp)
-	jbe    14c1c <fast_resonator_real_imag+0x75c>
+	jbe    14bdc <fast_resonator_real_imag+0x75c>
 	movapd %xmm6,%xmm11
 	movapd %xmm7,%xmm13
 	movsd  -0x8(%r8,%rbx,8),%xmm6
 	movsd  -0x8(%r9,%rbx,8),%xmm3
 	movsd  -0x30(%rsp),%xmm7
 	movsd  -0x10(%rsp),%xmm14
 	unpcklpd %xmm13,%xmm13
@@ -17419,17 +17413,17 @@
 	movups %xmm7,-0x20(%r10)
 	divpd  %xmm2,%xmm0
 	addpd  %xmm15,%xmm4
 	movups %xmm4,-0x20(%rbp)
 	subpd  %xmm0,%xmm6
 	movups %xmm6,-0x10(%r10)
 	cmp    %r15,%r12
-	jne    14668 <fast_resonator_real_imag+0x1a8>
+	jne    14628 <fast_resonator_real_imag+0x1a8>
 	cmp    0x20(%rsp),%r11d
-	je     14a4f <fast_resonator_real_imag+0x58f>
+	je     14a0f <fast_resonator_real_imag+0x58f>
 	mov    0x24(%rsp),%ebp
 	movslq %ebp,%r12
 	movsd  -0x20(%rsp),%xmm13
 	movsd  -0x10(%rsp),%xmm12
 	movsd  (%rdx,%r12,8),%xmm2
 	movsd  -0x8(%rsp),%xmm15
 	lea    0x0(,%r12,8),%r10
@@ -17478,15 +17472,15 @@
 	divsd  %xmm2,%xmm6
 	subsd  %xmm0,%xmm7
 	movsd  %xmm7,(%r12)
 	lea    0x1(%rbp),%r12d
 	addsd  %xmm6,%xmm3
 	movsd  %xmm3,0x0(%r13)
 	cmp    %r12d,%eax
-	jle    14a4f <fast_resonator_real_imag+0x58f>
+	jle    14a0f <fast_resonator_real_imag+0x58f>
 	movsd  0x8(%rdx,%r10,1),%xmm6
 	movapd %xmm13,%xmm2
 	lea    0x8(%r10),%r12
 	add    $0x2,%ebp
 	movapd %xmm12,%xmm0
 	lea    (%rdi,%r12,1),%r13
 	add    %rsi,%r12
@@ -17519,15 +17513,15 @@
 	movapd %xmm11,%xmm6
 	divsd  %xmm2,%xmm6
 	subsd  %xmm0,%xmm7
 	movsd  %xmm7,(%r12)
 	addsd  %xmm6,%xmm3
 	movsd  %xmm3,0x0(%r13)
 	cmp    %ebp,%eax
-	jle    14a4f <fast_resonator_real_imag+0x58f>
+	jle    14a0f <fast_resonator_real_imag+0x58f>
 	movsd  0x10(%rdx,%r10,1),%xmm2
 	lea    0x10(%r10),%rbp
 	lea    (%rdi,%rbp,1),%r10
 	add    %rsi,%rbp
 	divsd  %xmm2,%xmm13
 	movsd  0x0(%rbp),%xmm6
 	mulsd  %xmm2,%xmm12
@@ -17560,21 +17554,21 @@
 	subsd  %xmm5,%xmm6
 	movsd  %xmm6,0x0(%rbp)
 	addl   $0x2,-0x34(%rsp)
 	movslq %ebx,%rbp
 	mov    -0x34(%rsp),%r10d
 	add    $0x2,%rbx
 	cmp    %r10d,(%rsp)
-	jg     1454d <fast_resonator_real_imag+0x8d>
+	jg     1450d <fast_resonator_real_imag+0x8d>
 	movsd  -0x28(%rsp),%xmm14
 	mov    %r14d,%r10d
 	mov    %r11d,%r12d
 	mov    %r11d,%r13d
 	mov    %r11d,%r14d
-	movapd 0x364b(%rip),%xmm6        
+	movapd 0x368b(%rip),%xmm6        
 	shr    %r12d
 	and    $0xfffffffe,%r13d
 	or     $0x1,%r14d
 	shl    $0x4,%r12
 	add    $0x8,%r12
 	nopl   0x0(%rax,%rax,1)
 	movsd  (%r8,%rbp,8),%xmm0
@@ -17583,15 +17577,15 @@
 	movsd  (%rcx,%rbp,8),%xmm5
 	divsd  %xmm8,%xmm3
 	movapd %xmm0,%xmm9
 	movapd %xmm0,%xmm7
 	mulsd  %xmm0,%xmm9
 	mulsd  %xmm5,%xmm7
 	cmp    $0x2,%eax
-	je     14bfd <fast_resonator_real_imag+0x73d>
+	je     14bbd <fast_resonator_real_imag+0x73d>
 	movapd %xmm3,%xmm13
 	movapd %xmm8,%xmm12
 	movapd %xmm9,%xmm11
 	mov    $0x8,%ebx
 	movapd %xmm5,%xmm10
 	movapd %xmm7,%xmm1
 	unpcklpd %xmm13,%xmm13
@@ -17619,18 +17613,18 @@
 	movapd %xmm0,%xmm2
 	movupd (%rsi,%rbx,1),%xmm0
 	divpd  %xmm4,%xmm2
 	subpd  %xmm2,%xmm0
 	movups %xmm0,(%rsi,%rbx,1)
 	add    $0x10,%rbx
 	cmp    %rbx,%r12
-	jne    14b10 <fast_resonator_real_imag+0x650>
+	jne    14ad0 <fast_resonator_real_imag+0x650>
 	movslq %r14d,%r15
 	cmp    %r13d,%r11d
-	je     14be1 <fast_resonator_real_imag+0x721>
+	je     14ba1 <fast_resonator_real_imag+0x721>
 	movsd  (%rdx,%r15,8),%xmm1
 	movapd %xmm8,%xmm2
 	lea    0x0(,%r15,8),%rbx
 	lea    (%rdi,%rbx,1),%r15
 	add    %rsi,%rbx
 	divsd  %xmm1,%xmm2
 	mulsd  %xmm1,%xmm3
@@ -17647,73 +17641,73 @@
 	movsd  (%rbx),%xmm1
 	addsd  %xmm5,%xmm2
 	movsd  %xmm2,(%r15)
 	subsd  %xmm0,%xmm1
 	movsd  %xmm1,(%rbx)
 	add    $0x1,%rbp
 	cmp    %ebp,%r10d
-	jg     14aa0 <fast_resonator_real_imag+0x5e0>
+	jg     14a60 <fast_resonator_real_imag+0x5e0>
 	add    $0x30,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	mov    $0x1,%r15d
-	jmp    14b7f <fast_resonator_real_imag+0x6bf>
-	movsd  0x36c7(%rip),%xmm14        
+	jmp    14b3f <fast_resonator_real_imag+0x6bf>
+	movsd  0x3707(%rip),%xmm14        
 	xor    %ebp,%ebp
 	lea    -0x1(%rax),%r11d
-	jmp    14a74 <fast_resonator_real_imag+0x5b4>
+	jmp    14a34 <fast_resonator_real_imag+0x5b4>
 	movsd  -0x8(%rcx,%rbx,8),%xmm7
 	mov    $0x1,%ebp
 	movsd  %xmm7,0x8(%rsp)
 	movsd  -0x8(%r9,%rbx,8),%xmm7
 	movsd  %xmm7,0x18(%rsp)
 	movsd  -0x8(%r8,%rbx,8),%xmm7
 	movsd  %xmm7,0x10(%rsp)
-	jmp    147e8 <fast_resonator_real_imag+0x328>
+	jmp    147a8 <fast_resonator_real_imag+0x328>
 	nopl   0x0(%rax)
 
-0000000000014c50 <fast_resonator_real_imagf>:
+0000000000014c10 <fast_resonator_real_imagf>:
 fast_resonator_real_imagf():
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
 	sub    $0xf0,%rsp
 	mov    0x128(%rsp),%r10d
 	mov    0x130(%rsp),%eax
 	test   %r10d,%r10d
-	jle    156cd <fast_resonator_real_imagf+0xa7d>
+	jle    1568d <fast_resonator_real_imagf+0xa7d>
 	cmp    $0x1,%eax
-	jle    156cd <fast_resonator_real_imagf+0xa7d>
+	jle    1568d <fast_resonator_real_imagf+0xa7d>
 	mov    0x128(%rsp),%ebx
 	mov    %r9,%r12
 	sub    $0x1,%ebx
 	cmpl   $0x2,0x128(%rsp)
 	mov    %ebx,0x84(%rsp)
-	jle    156e9 <fast_resonator_real_imagf+0xa99>
+	jle    156a9 <fast_resonator_real_imagf+0xa99>
 	lea    -0x1(%rax),%r15d
 	lea    -0x2(%rax),%ebx
 	mov    $0x2,%r9d
 	mov    %eax,%ebp
 	mov    %r15d,%r13d
 	movaps %xmm5,%xmm7
 	movaps %xmm3,%xmm8
 	mov    $0x1,%r14d
 	mov    %ebx,0x80(%rsp)
 	mov    %r15d,%ebx
 	shr    $0x2,%r13d
-	movss  0x361f(%rip),%xmm6        
-	movapd 0x33ee(%rip),%xmm14        
+	movss  0x365f(%rip),%xmm6        
+	movapd 0x342e(%rip),%xmm14        
 	and    $0xfffffffc,%ebx
 	shl    $0x4,%r13
 	movaps %xmm11,0xa8(%rsp)
 	mov    %ebx,0x98(%rsp)
 	add    $0x1,%ebx
 	add    $0x4,%r13
 	movaps %xmm2,%xmm11
@@ -17736,15 +17730,15 @@
 	movss  %xmm0,0x74(%rsp)
 	divss  %xmm6,%xmm5
 	movss  %xmm6,0x64(%rsp)
 	pxor   %xmm6,%xmm6
 	cvtss2sd %xmm1,%xmm6
 	movsd  %xmm6,0x68(%rsp)
 	movss  %xmm5,0x70(%rsp)
-	jbe    1570d <fast_resonator_real_imagf+0xabd>
+	jbe    156cd <fast_resonator_real_imagf+0xabd>
 	movaps %xmm5,%xmm6
 	movss  -0x4(%r12,%r9,4),%xmm4
 	movss  -0x4(%rcx,%r9,4),%xmm3
 	mov    $0x4,%r10d
 	shufps $0x0,%xmm6,%xmm6
 	movaps %xmm6,-0x48(%rsp)
 	movss  0x64(%rsp),%xmm6
@@ -17874,18 +17868,18 @@
 	cvtpd2ps %xmm1,%xmm1
 	subpd  %xmm0,%xmm2
 	cvtpd2ps %xmm2,%xmm2
 	movlhps %xmm2,%xmm1
 	movups %xmm1,(%rsi,%r10,1)
 	add    $0x10,%r10
 	cmp    %r13,%r10
-	jne    14e78 <fast_resonator_real_imagf+0x228>
+	jne    14e38 <fast_resonator_real_imagf+0x228>
 	movaps %xmm13,0x88(%rsp)
 	cmp    0x98(%rsp),%r15d
-	je     1532b <fast_resonator_real_imagf+0x6db>
+	je     152eb <fast_resonator_real_imagf+0x6db>
 	mov    0xa4(%rsp),%eax
 	movslq %eax,%r11
 	movss  0x64(%rsp),%xmm1
 	movss  0x70(%rsp),%xmm0
 	pxor   %xmm4,%xmm4
 	movss  (%rdx,%r11,4),%xmm2
 	movss  0x7c(%rsp),%xmm3
@@ -17906,15 +17900,15 @@
 	mulss  %xmm0,%xmm6
 	mulss  0x74(%rsp),%xmm0
 	mulss  %xmm6,%xmm1
 	pxor   %xmm6,%xmm6
 	cvtss2sd %xmm0,%xmm0
 	divss  %xmm2,%xmm3
 	cvtss2sd %xmm1,%xmm1
-	addsd  0x323f(%rip),%xmm1        
+	addsd  0x327f(%rip),%xmm1        
 	divsd  %xmm1,%xmm0
 	subsd  %xmm0,%xmm4
 	movss  0x9c(%rsp),%xmm0
 	mulss  %xmm0,%xmm5
 	cvtss2sd %xmm0,%xmm6
 	movaps %xmm2,%xmm0
 	mulss  %xmm13,%xmm0
@@ -17928,30 +17922,30 @@
 	movaps %xmm0,%xmm2
 	cvtss2sd (%rbx),%xmm1
 	mulss  %xmm0,%xmm2
 	mulss  %xmm5,%xmm0
 	mulss  %xmm15,%xmm2
 	cvtss2sd %xmm0,%xmm0
 	cvtss2sd %xmm2,%xmm2
-	addsd  0x31da(%rip),%xmm2        
+	addsd  0x321a(%rip),%xmm2        
 	divsd  %xmm2,%xmm0
 	addsd  %xmm3,%xmm1
 	movapd %xmm6,%xmm3
 	cvtsd2ss %xmm1,%xmm1
 	cvtss2sd %xmm1,%xmm1
 	divsd  %xmm2,%xmm3
 	subsd  %xmm0,%xmm4
 	cvtsd2ss %xmm4,%xmm4
 	movss  %xmm4,(%r11)
 	lea    0x1(%rax),%r11d
 	addsd  %xmm3,%xmm1
 	cvtsd2ss %xmm1,%xmm1
 	movss  %xmm1,(%rbx)
 	cmp    %r11d,%ebp
-	jle    1532b <fast_resonator_real_imagf+0x6db>
+	jle    152eb <fast_resonator_real_imagf+0x6db>
 	movss  0x4(%rdx,%r10,1),%xmm2
 	movss  0x64(%rsp),%xmm1
 	lea    0x4(%r10),%r11
 	pxor   %xmm5,%xmm5
 	movss  0x70(%rsp),%xmm0
 	movss  0x78(%rsp),%xmm3
 	lea    (%rdi,%r11,1),%rbx
@@ -17965,15 +17959,15 @@
 	movaps %xmm0,%xmm4
 	mulss  %xmm0,%xmm4
 	mulss  0x74(%rsp),%xmm0
 	mulss  %xmm4,%xmm3
 	movsd  0x68(%rsp),%xmm4
 	cvtss2sd %xmm0,%xmm0
 	cvtss2sd %xmm3,%xmm3
-	addsd  0x3132(%rip),%xmm3        
+	addsd  0x3172(%rip),%xmm3        
 	divsd  %xmm3,%xmm0
 	divsd  %xmm3,%xmm4
 	movapd %xmm6,%xmm3
 	subsd  %xmm0,%xmm5
 	movaps %xmm13,%xmm0
 	mulss  %xmm2,%xmm0
 	cvtsd2ss %xmm5,%xmm5
@@ -17983,29 +17977,29 @@
 	cvtss2sd (%rbx),%xmm1
 	movaps %xmm0,%xmm2
 	mulss  %xmm0,%xmm2
 	mulss  -0x78(%rsp),%xmm0
 	mulss  %xmm15,%xmm2
 	cvtss2sd %xmm0,%xmm0
 	cvtss2sd %xmm2,%xmm2
-	addsd  0x30e4(%rip),%xmm2        
+	addsd  0x3124(%rip),%xmm2        
 	addsd  %xmm4,%xmm1
 	divsd  %xmm2,%xmm0
 	cvtsd2ss %xmm1,%xmm1
 	cvtss2sd %xmm1,%xmm1
 	divsd  %xmm2,%xmm3
 	subsd  %xmm0,%xmm5
 	cvtsd2ss %xmm5,%xmm5
 	movss  %xmm5,(%r11)
 	lea    0x2(%rax),%r11d
 	addsd  %xmm3,%xmm1
 	cvtsd2ss %xmm1,%xmm1
 	movss  %xmm1,(%rbx)
 	cmp    %r11d,%ebp
-	jle    1532b <fast_resonator_real_imagf+0x6db>
+	jle    152eb <fast_resonator_real_imagf+0x6db>
 	movss  0x8(%rdx,%r10,1),%xmm0
 	movss  0x64(%rsp),%xmm2
 	lea    0x8(%r10),%rbx
 	pxor   %xmm3,%xmm3
 	movss  0x70(%rsp),%xmm4
 	lea    (%rsi,%rbx,1),%r10
 	lea    (%rdi,%rbx,1),%r11
@@ -18017,15 +18011,15 @@
 	pxor   %xmm4,%xmm4
 	subss  %xmm2,%xmm1
 	movaps %xmm1,%xmm2
 	mulss  %xmm1,%xmm2
 	mulss  0x78(%rsp),%xmm2
 	mulss  0x74(%rsp),%xmm1
 	cvtss2sd %xmm2,%xmm2
-	addsd  0x304b(%rip),%xmm2        
+	addsd  0x308b(%rip),%xmm2        
 	cvtss2sd %xmm1,%xmm4
 	pxor   %xmm1,%xmm1
 	divsd  %xmm2,%xmm4
 	subsd  %xmm4,%xmm3
 	pxor   %xmm4,%xmm4
 	cvtsd2ss %xmm3,%xmm1
 	movss  0x7c(%rsp),%xmm3
@@ -18039,15 +18033,15 @@
 	movaps %xmm13,%xmm3
 	mulss  %xmm15,%xmm3
 	movsd  0x68(%rsp),%xmm15
 	cvtss2sd %xmm0,%xmm0
 	divsd  %xmm2,%xmm15
 	pxor   %xmm2,%xmm2
 	cvtss2sd %xmm3,%xmm4
-	addsd  0x2fe5(%rip),%xmm4        
+	addsd  0x3025(%rip),%xmm4        
 	pxor   %xmm3,%xmm3
 	cvtss2sd (%r11),%xmm3
 	divsd  %xmm4,%xmm6
 	addsd  %xmm15,%xmm3
 	cvtsd2ss %xmm3,%xmm2
 	cvtss2sd %xmm2,%xmm2
 	divsd  %xmm4,%xmm0
@@ -18057,27 +18051,27 @@
 	subsd  %xmm0,%xmm1
 	cvtsd2ss %xmm1,%xmm1
 	movss  %xmm1,(%r10)
 	mov    %r9d,%r10d
 	add    $0x2,%r14d
 	add    $0x2,%r9
 	cmp    %r14d,0x84(%rsp)
-	jg     14d34 <fast_resonator_real_imagf+0xe4>
+	jg     14cf4 <fast_resonator_real_imagf+0xe4>
 	movaps 0xa8(%rsp),%xmm11
 	mov    %ebp,%eax
 	movaps 0xb8(%rsp),%xmm12
 	movaps 0xc8(%rsp),%xmm13
 	movaps 0xd8(%rsp),%xmm10
 	mov    %r15d,%r11d
 	movslq %r10d,%r9
 	mov    %r15d,%r10d
 	mov    %r15d,-0x18(%rsp)
 	and    $0xfffffffc,%r11d
 	shr    $0x2,%r10d
-	movapd 0x2d48(%rip),%xmm6        
+	movapd 0x2d88(%rip),%xmm6        
 	mov    0x80(%rsp),%r15d
 	lea    0x1(%r11),%ebx
 	mov    %r11d,-0x28(%rsp)
 	shl    $0x4,%r10
 	mov    0x128(%rsp),%r11d
 	mov    %ebx,-0x8(%rsp)
 	add    $0x4,%r10
@@ -18095,15 +18089,15 @@
 	movsd  %xmm2,-0x68(%rsp)
 	mulss  %xmm0,%xmm5
 	mulss  %xmm0,%xmm4
 	movss  %xmm5,-0x38(%rsp)
 	movss  %xmm4,-0x78(%rsp)
 	movss  %xmm3,-0x58(%rsp)
 	cmp    $0x2,%r15d
-	jbe    156df <fast_resonator_real_imagf+0xa8f>
+	jbe    1569f <fast_resonator_real_imagf+0xa8f>
 	movaps %xmm5,%xmm9
 	movapd %xmm2,%xmm5
 	movaps %xmm3,%xmm15
 	mov    $0x4,%ebx
 	movaps %xmm7,%xmm14
 	movaps %xmm4,%xmm8
 	unpcklpd %xmm5,%xmm5
@@ -18157,18 +18151,18 @@
 	cvtpd2ps %xmm0,%xmm0
 	subpd  %xmm3,%xmm1
 	cvtpd2ps %xmm1,%xmm1
 	movlhps %xmm1,%xmm0
 	movups %xmm0,(%rsi,%rbx,1)
 	add    $0x10,%rbx
 	cmp    %r10,%rbx
-	jne    15440 <fast_resonator_real_imagf+0x7f0>
+	jne    15400 <fast_resonator_real_imagf+0x7f0>
 	mov    -0x28(%rsp),%r14d
 	cmp    %r14d,-0x18(%rsp)
-	je     156c0 <fast_resonator_real_imagf+0xa70>
+	je     15680 <fast_resonator_real_imagf+0xa70>
 	mov    -0x8(%rsp),%ebp
 	movslq %ebp,%r13
 	movss  -0x48(%rsp),%xmm7
 	movss  -0x58(%rsp),%xmm5
 	movss  (%rdx,%r13,4),%xmm1
 	movss  -0x38(%rsp),%xmm8
 	lea    0x0(,%r13,4),%rbx
@@ -18185,29 +18179,29 @@
 	cvtss2sd 0x0(%r13),%xmm2
 	movaps %xmm0,%xmm1
 	mulss  %xmm0,%xmm1
 	mulss  %xmm9,%xmm0
 	mulss  %xmm8,%xmm1
 	cvtss2sd %xmm0,%xmm0
 	cvtss2sd %xmm1,%xmm1
-	addsd  0x2d4f(%rip),%xmm1        
+	addsd  0x2d8f(%rip),%xmm1        
 	divsd  %xmm1,%xmm3
 	divsd  %xmm1,%xmm0
 	addsd  %xmm3,%xmm2
 	cvtsd2ss %xmm2,%xmm2
 	movss  %xmm2,0x0(%r13)
 	lea    (%rsi,%rbx,1),%r13
 	pxor   %xmm2,%xmm2
 	cvtss2sd 0x0(%r13),%xmm2
 	subsd  %xmm0,%xmm2
 	cvtsd2ss %xmm2,%xmm2
 	movss  %xmm2,0x0(%r13)
 	lea    0x1(%rbp),%r13d
 	cmp    %r13d,%eax
-	jle    156c0 <fast_resonator_real_imagf+0xa70>
+	jle    15680 <fast_resonator_real_imagf+0xa70>
 	movss  0x4(%rdx,%rbx,1),%xmm1
 	movaps %xmm7,%xmm2
 	movaps %xmm5,%xmm0
 	lea    0x4(%rbx),%r13
 	lea    (%rdi,%r13,1),%r14
 	pxor   %xmm3,%xmm3
 	add    %rsi,%r13
@@ -18219,27 +18213,27 @@
 	movapd %xmm4,%xmm2
 	movaps %xmm0,%xmm1
 	mulss  %xmm0,%xmm1
 	mulss  %xmm9,%xmm0
 	mulss  %xmm8,%xmm1
 	cvtss2sd %xmm0,%xmm0
 	cvtss2sd %xmm1,%xmm1
-	addsd  0x2cbc(%rip),%xmm1        
+	addsd  0x2cfc(%rip),%xmm1        
 	divsd  %xmm1,%xmm2
 	divsd  %xmm1,%xmm0
 	addsd  %xmm3,%xmm2
 	cvtsd2ss %xmm2,%xmm2
 	movss  %xmm2,(%r14)
 	pxor   %xmm2,%xmm2
 	cvtss2sd 0x0(%r13),%xmm2
 	subsd  %xmm0,%xmm2
 	cvtsd2ss %xmm2,%xmm2
 	movss  %xmm2,0x0(%r13)
 	cmp    %ebp,%eax
-	jle    156c0 <fast_resonator_real_imagf+0xa70>
+	jle    15680 <fast_resonator_real_imagf+0xa70>
 	movss  0x8(%rdx,%rbx,1),%xmm2
 	lea    0x8(%rbx),%rbp
 	pxor   %xmm3,%xmm3
 	pxor   %xmm1,%xmm1
 	lea    (%rdi,%rbp,1),%rbx
 	add    %rsi,%rbp
 	divss  %xmm2,%xmm7
@@ -18250,55 +18244,55 @@
 	subss  %xmm7,%xmm0
 	movaps %xmm0,%xmm2
 	mulss  %xmm0,%xmm2
 	mulss  %xmm9,%xmm0
 	mulss  %xmm8,%xmm2
 	cvtss2sd %xmm0,%xmm0
 	cvtss2sd %xmm2,%xmm2
-	addsd  0x2c39(%rip),%xmm2        
+	addsd  0x2c79(%rip),%xmm2        
 	divsd  %xmm2,%xmm4
 	divsd  %xmm2,%xmm0
 	addsd  %xmm4,%xmm3
 	cvtsd2ss %xmm3,%xmm3
 	movss  %xmm3,(%rbx)
 	subsd  %xmm0,%xmm1
 	cvtsd2ss %xmm1,%xmm1
 	movss  %xmm1,0x0(%rbp)
 	add    $0x1,%r9
 	cmp    %r9d,%r11d
-	jg     153b0 <fast_resonator_real_imagf+0x760>
+	jg     15370 <fast_resonator_real_imagf+0x760>
 	add    $0xf0,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	mov    $0x1,%ebp
-	jmp    15513 <fast_resonator_real_imagf+0x8c3>
-	movss  0x2c07(%rip),%xmm6        
+	jmp    154d3 <fast_resonator_real_imagf+0x8c3>
+	movss  0x2c47(%rip),%xmm6        
 	lea    -0x2(%rax),%ebx
 	xor    %r10d,%r10d
 	lea    -0x1(%rax),%r15d
 	mov    %ebx,0x80(%rsp)
 	movss  %xmm6,0x60(%rsp)
-	jmp    1536a <fast_resonator_real_imagf+0x71a>
+	jmp    1532a <fast_resonator_real_imagf+0x71a>
 	movss  -0x4(%rcx,%r9,4),%xmm6
 	mov    $0x1,%eax
 	movss  %xmm6,0x9c(%rsp)
 	movss  -0x4(%r12,%r9,4),%xmm6
 	movss  %xmm6,0x7c(%rsp)
 	movss  -0x4(%r8,%r9,4),%xmm6
 	movss  %xmm6,0xa0(%rsp)
-	jmp    1500c <fast_resonator_real_imagf+0x3bc>
+	jmp    14fcc <fast_resonator_real_imagf+0x3bc>
 	cs nopw 0x0(%rax,%rax,1)
 	xchg   %ax,%ax
 
-0000000000015750 <beam_phase>:
+0000000000015710 <beam_phase>:
 beam_phase():
 	movabs $0xfffffffffffffff,%rax
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
@@ -18321,26 +18315,26 @@
 	mov    %rax,%rbp
 	call   3030 <operator new[](unsigned long)@plt>
 	mov    %r13,%rdi
 	mov    %rax,%r14
 	call   3030 <operator new[](unsigned long)@plt>
 	mov    %rax,%r13
 	test   %ebx,%ebx
-	jle    15868 <beam_phase+0x118>
+	jle    15828 <beam_phase+0x118>
 	xor    %r15d,%r15d
 	nopl   0x0(%rax,%rax,1)
 	movsd  0x8(%rsp),%xmm0
 	mulsd  (%r12,%r15,8),%xmm0
 	call   3170 <fast_exp@plt>
 	mov    (%rsp),%rax
 	mulsd  (%rax,%r15,8),%xmm0
 	movsd  %xmm0,0x0(%rbp,%r15,8)
 	add    $0x1,%r15
 	cmp    %r15,%rbx
-	jne    157d0 <beam_phase+0x80>
+	jne    15790 <beam_phase+0x80>
 	xor    %r15d,%r15d
 	xchg   %ax,%ax
 	movsd  0x10(%rsp),%xmm1
 	mulsd  (%r12,%r15,8),%xmm1
 	addsd  0x18(%rsp),%xmm1
 	movsd  0x0(%rbp,%r15,8),%xmm5
 	movsd  %xmm5,(%rsp)
@@ -18354,15 +18348,15 @@
 	movsd  %xmm0,(%r14,%r15,8)
 	movapd %xmm1,%xmm0
 	call   3050 <fast_cos@plt>
 	mulsd  (%rsp),%xmm0
 	movsd  %xmm0,0x0(%r13,%r15,8)
 	add    $0x1,%r15
 	cmp    %r15,%rbx
-	jne    15800 <beam_phase+0xb0>
+	jne    157c0 <beam_phase+0xb0>
 	mov    0x2c(%rsp),%r15d
 	movsd  0x20(%rsp),%xmm0
 	mov    %r14,%rdi
 	mov    %r15d,%esi
 	call   3280 <trapz_const_delta@plt>
 	mov    %r15d,%esi
 	mov    %r13,%rdi
@@ -18385,15 +18379,15 @@
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	xchg   %ax,%ax
 
-00000000000158d0 <beam_phase_fast>:
+0000000000015890 <beam_phase_fast>:
 beam_phase_fast():
 	movabs $0xfffffffffffffff,%rax
 	push   %r15
 	push   %r14
 	push   %r13
 	movslq %edx,%r13
 	push   %r12
@@ -18412,15 +18406,15 @@
 	mov    %rbp,%rdi
 	call   3030 <operator new[](unsigned long)@plt>
 	mov    %rbp,%rdi
 	mov    %rax,%r12
 	call   3030 <operator new[](unsigned long)@plt>
 	mov    %rax,%rbp
 	test   %r13d,%r13d
-	jle    159a6 <beam_phase_fast+0xd6>
+	jle    15966 <beam_phase_fast+0xd6>
 	xor    %r15d,%r15d
 	nopw   0x0(%rax,%rax,1)
 	movsd  0x10(%rsp),%xmm1
 	mulsd  (%r14,%r15,8),%xmm1
 	addsd  0x18(%rsp),%xmm1
 	movsd  (%rbx,%r15,8),%xmm4
 	movsd  %xmm4,(%rsp)
@@ -18434,15 +18428,15 @@
 	movsd  %xmm0,(%r12,%r15,8)
 	movapd %xmm1,%xmm0
 	call   3050 <fast_cos@plt>
 	mulsd  (%rsp),%xmm0
 	movsd  %xmm0,0x0(%rbp,%r15,8)
 	add    $0x1,%r15
 	cmp    %r15,%r13
-	jne    15940 <beam_phase_fast+0x70>
+	jne    15900 <beam_phase_fast+0x70>
 	mov    0x2c(%rsp),%r14d
 	movsd  0x20(%rsp),%xmm0
 	mov    %r12,%rdi
 	mov    %r14d,%esi
 	call   3280 <trapz_const_delta@plt>
 	mov    %r14d,%esi
 	mov    %rbp,%rdi
@@ -18464,15 +18458,15 @@
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nop
 
-0000000000015a10 <beam_phasef>:
+00000000000159d0 <beam_phasef>:
 beam_phasef():
 	movabs $0x1ffffffffffffffe,%rax
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
@@ -18495,26 +18489,26 @@
 	mov    %rax,%rbp
 	call   3030 <operator new[](unsigned long)@plt>
 	mov    %r13,%rdi
 	mov    %rax,%r14
 	call   3030 <operator new[](unsigned long)@plt>
 	mov    %rax,%r13
 	test   %ebx,%ebx
-	jle    15b26 <beam_phasef+0x116>
+	jle    15ae6 <beam_phasef+0x116>
 	xor    %r15d,%r15d
 	nopl   0x0(%rax,%rax,1)
 	movss  0xc(%rsp),%xmm0
 	mulss  (%r12,%r15,4),%xmm0
 	call   3230 <fast_expf@plt>
 	mov    (%rsp),%rax
 	mulss  (%rax,%r15,4),%xmm0
 	movss  %xmm0,0x0(%rbp,%r15,4)
 	add    $0x1,%r15
 	cmp    %r15,%rbx
-	jne    15a90 <beam_phasef+0x80>
+	jne    15a50 <beam_phasef+0x80>
 	xor    %r15d,%r15d
 	xchg   %ax,%ax
 	movss  0x10(%rsp),%xmm1
 	mulss  (%r12,%r15,4),%xmm1
 	addss  0x14(%rsp),%xmm1
 	movss  0x0(%rbp,%r15,4),%xmm5
 	movss  %xmm5,(%rsp)
@@ -18528,15 +18522,15 @@
 	movss  %xmm0,(%r14,%r15,4)
 	movaps %xmm1,%xmm0
 	call   30c0 <fast_cosf@plt>
 	mulss  (%rsp),%xmm0
 	movss  %xmm0,0x0(%r13,%r15,4)
 	add    $0x1,%r15
 	cmp    %r15,%rbx
-	jne    15ac0 <beam_phasef+0xb0>
+	jne    15a80 <beam_phasef+0xb0>
 	mov    0x1c(%rsp),%r15d
 	movss  0x18(%rsp),%xmm0
 	mov    %r14,%rdi
 	mov    %r15d,%esi
 	call   32b0 <trapz_const_deltaf@plt>
 	mov    %r15d,%esi
 	mov    %r13,%rdi
@@ -18559,45 +18553,45 @@
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopl   0x0(%rax)
 
-0000000000015b90 <omp_get_max_threads()>:
+0000000000015b50 <omp_get_max_threads()>:
 omp_get_max_threads():
 	mov    $0x1,%eax
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000015ba0 <omp_get_num_threads()>:
+0000000000015b60 <omp_get_num_threads()>:
 omp_get_num_threads():
 	mov    $0x1,%eax
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000015bb0 <omp_get_thread_num()>:
+0000000000015b70 <omp_get_thread_num()>:
 omp_get_thread_num():
 	xor    %eax,%eax
 	ret
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-0000000000015bc0 <randd()>:
+0000000000015b80 <randd()>:
 randd():
 	sub    $0x8,%rsp
 	call   3060 <rand@plt>
 	pxor   %xmm0,%xmm0
 	cvtsi2sd %eax,%xmm0
-	mulsd  0x2847(%rip),%xmm0        
+	mulsd  0x2887(%rip),%xmm0        
 	add    $0x8,%rsp
 	ret
 	xchg   %ax,%ax
 
-0000000000015be0 <generate_distribution>:
+0000000000015ba0 <generate_distribution>:
 generate_distribution():
 	push   %rbp
 	mov    %rsp,%rbp
 	push   %r15
 	mov    %r9d,%r15d
 	push   %r14
 	push   %r13
@@ -18623,72 +18617,72 @@
 	mulsd  %xmm0,%xmm0
 	shr    $0x4,%rax
 	shl    $0x4,%rax
 	sub    %rax,%rsp
 	mov    %rsp,%rbx
 	movsd  %xmm0,-0x48(%rbp)
 	test   %r14d,%r14d
-	je     15ccb <generate_distribution+0xeb>
+	je     15c8b <generate_distribution+0xeb>
 	mov    -0x50(%rbp),%rdx
 	xor    %eax,%eax
 	pxor   %xmm0,%xmm0
 	nop
 	addsd  (%rdx,%rax,8),%xmm0
 	movsd  %xmm0,(%rbx,%rax,8)
 	add    $0x1,%rax
 	cmp    %rsi,%rax
-	jne    15c60 <generate_distribution+0x80>
-	movsd  0x265d(%rip),%xmm1        
+	jne    15c20 <generate_distribution+0x80>
+	movsd  0x269d(%rip),%xmm1        
 	divsd  %xmm0,%xmm1
 	cmp    $0x1,%r14d
-	je     15e28 <generate_distribution+0x248>
+	je     15de8 <generate_distribution+0x248>
 	mov    %r14d,%edx
 	movapd %xmm1,%xmm2
 	mov    %rbx,%rax
 	shr    %edx
 	unpcklpd %xmm2,%xmm2
 	shl    $0x4,%rdx
 	add    %rbx,%rdx
 	movupd (%rax),%xmm0
 	add    $0x10,%rax
 	mulpd  %xmm2,%xmm0
 	movups %xmm0,-0x10(%rax)
 	cmp    %rdx,%rax
-	jne    15ca0 <generate_distribution+0xc0>
+	jne    15c60 <generate_distribution+0xc0>
 	mov    %r14d,%eax
 	and    $0xfffffffe,%eax
 	test   $0x1,%r14b
-	je     15ccb <generate_distribution+0xeb>
+	je     15c8b <generate_distribution+0xeb>
 	mulsd  (%rbx,%rax,8),%xmm1
 	movsd  %xmm1,(%rbx,%rax,8)
-	movsd  0x2755(%rip),%xmm0        
+	movsd  0x2795(%rip),%xmm0        
 	mov    -0x38(%rbp),%rax
 	lea    0x0(%r13,%r15,8),%r15
 	movapd %xmm0,%xmm7
 	subsd  -0x58(%rbp),%xmm0
 	subsd  -0x40(%rbp),%xmm7
 	mov    %rax,-0x60(%rbp)
 	movsd  %xmm7,-0x50(%rbp)
 	movsd  %xmm0,-0x58(%rbp)
 	nopl   0x0(%rax,%rax,1)
 	cmp    %r15,%r13
-	je     15dd6 <generate_distribution+0x1f6>
+	je     15d96 <generate_distribution+0x1f6>
 	call   3070 <randd()@plt>
 	test   %r14d,%r14d
-	je     15e13 <generate_distribution+0x233>
+	je     15dd3 <generate_distribution+0x233>
 	mov    %rbx,%rdx
 	xor    %eax,%eax
-	jmp    15d30 <generate_distribution+0x150>
+	jmp    15cf0 <generate_distribution+0x150>
 	xchg   %ax,%ax
 	add    $0x1,%eax
 	add    $0x8,%rdx
 	cmp    %eax,%r14d
-	je     15de8 <generate_distribution+0x208>
+	je     15da8 <generate_distribution+0x208>
 	comisd (%rdx),%xmm0
-	jae    15d20 <generate_distribution+0x140>
+	jae    15ce0 <generate_distribution+0x140>
 	xor    %edx,%edx
 	pxor   %xmm5,%xmm5
 	pxor   %xmm6,%xmm6
 	div    %r12d
 	mov    %edx,%edx
 	cvtsi2sd %rax,%xmm5
 	cvtsi2sd %rdx,%xmm6
@@ -18706,25 +18700,25 @@
 	movsd  -0x48(%rbp),%xmm4
 	movapd %xmm1,%xmm2
 	movapd %xmm0,%xmm3
 	mulsd  %xmm1,%xmm2
 	mulsd  %xmm0,%xmm3
 	addsd  %xmm3,%xmm2
 	comisd %xmm2,%xmm4
-	jbe    15d00 <generate_distribution+0x120>
+	jbe    15cc0 <generate_distribution+0x120>
 	mulsd  -0x68(%rbp),%xmm1
 	mov    -0x60(%rbp),%rax
 	add    $0x8,%r13
 	mulsd  -0x70(%rbp),%xmm0
 	add    $0x8,%rax
 	movsd  %xmm1,-0x8(%r13)
 	movsd  %xmm0,-0x8(%rax)
 	mov    %rax,-0x60(%rbp)
 	cmp    %r15,%r13
-	jne    15d09 <generate_distribution+0x129>
+	jne    15cc9 <generate_distribution+0x129>
 	lea    -0x28(%rbp),%rsp
 	pop    %rbx
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	pop    %rbp
@@ -18736,53 +18730,53 @@
 	xor    %edx,%edx
 	div    %r12d
 	mov    %edx,%edx
 	cvtsi2sd %rax,%xmm7
 	cvtsi2sd %rdx,%xmm4
 	movsd  %xmm7,-0x38(%rbp)
 	movsd  %xmm4,-0x40(%rbp)
-	jmp    15d59 <generate_distribution+0x179>
+	jmp    15d19 <generate_distribution+0x179>
 	movq   $0x0,-0x40(%rbp)
 	movq   $0x0,-0x38(%rbp)
-	jmp    15d59 <generate_distribution+0x179>
+	jmp    15d19 <generate_distribution+0x179>
 	xor    %eax,%eax
-	jmp    15cc1 <generate_distribution+0xe1>
+	jmp    15c81 <generate_distribution+0xe1>
 	nop
 
-0000000000015e30 <synchrotron_radiation>:
+0000000000015df0 <synchrotron_radiation>:
 synchrotron_radiation():
 	movapd %xmm0,%xmm2
-	movsd  0x257c(%rip),%xmm0        
+	movsd  0x25bc(%rip),%xmm0        
 	divsd  %xmm1,%xmm0
-	movsd  0x2490(%rip),%xmm1        
+	movsd  0x24d0(%rip),%xmm1        
 	subsd  %xmm0,%xmm1
 	test   %edx,%edx
-	jle    15fe4 <synchrotron_radiation+0x1b4>
+	jle    15fa4 <synchrotron_radiation+0x1b4>
 	test   %esi,%esi
-	jle    15fe4 <synchrotron_radiation+0x1b4>
+	jle    15fa4 <synchrotron_radiation+0x1b4>
 	push   %rbp
 	mov    %edx,%r8d
 	lea    -0x1(%rdx),%r9d
 	push   %rbx
 	cmp    $0x2,%edx
-	jle    15fe5 <synchrotron_radiation+0x1b5>
+	jle    15fa5 <synchrotron_radiation+0x1b5>
 	mov    %esi,%edx
 	mov    %esi,%ebx
 	movapd %xmm1,%xmm5
 	mov    $0x1,%r11d
 	shr    $0x2,%edx
 	movapd %xmm2,%xmm4
 	lea    -0x1(%rsi),%r10d
 	and    $0xfffffffc,%ebx
 	shl    $0x5,%rdx
 	unpcklpd %xmm5,%xmm5
 	unpcklpd %xmm4,%xmm4
 	add    %rdi,%rdx
 	cmp    $0x2,%r10d
-	jbe    15fe9 <synchrotron_radiation+0x1b9>
+	jbe    15fa9 <synchrotron_radiation+0x1b9>
 	mov    %rdi,%rax
 	cs nopw 0x0(%rax,%rax,1)
 	movupd 0x10(%rax),%xmm0
 	movupd (%rax),%xmm3
 	add    $0x20,%rax
 	mulpd  %xmm5,%xmm0
 	mulpd  %xmm5,%xmm3
@@ -18791,336 +18785,336 @@
 	mulpd  %xmm5,%xmm0
 	mulpd  %xmm5,%xmm3
 	subpd  %xmm4,%xmm0
 	subpd  %xmm4,%xmm3
 	movups %xmm0,-0x10(%rax)
 	movups %xmm3,-0x20(%rax)
 	cmp    %rdx,%rax
-	jne    15eb0 <synchrotron_radiation+0x80>
+	jne    15e70 <synchrotron_radiation+0x80>
 	mov    %ebx,%ecx
 	cmp    %ebx,%esi
-	je     15f5f <synchrotron_radiation+0x12f>
+	je     15f1f <synchrotron_radiation+0x12f>
 	movslq %ecx,%rax
 	shl    $0x3,%rax
 	lea    (%rdi,%rax,1),%rbp
 	movsd  0x0(%rbp),%xmm0
 	mulsd  %xmm1,%xmm0
 	subsd  %xmm2,%xmm0
 	mulsd  %xmm1,%xmm0
 	subsd  %xmm2,%xmm0
 	movsd  %xmm0,0x0(%rbp)
 	lea    0x1(%rcx),%ebp
 	cmp    %ebp,%esi
-	jle    15f5f <synchrotron_radiation+0x12f>
+	jle    15f1f <synchrotron_radiation+0x12f>
 	lea    0x8(%rdi,%rax,1),%rbp
 	add    $0x2,%ecx
 	movsd  0x0(%rbp),%xmm0
 	mulsd  %xmm1,%xmm0
 	subsd  %xmm2,%xmm0
 	mulsd  %xmm1,%xmm0
 	subsd  %xmm2,%xmm0
 	movsd  %xmm0,0x0(%rbp)
 	cmp    %ecx,%esi
-	jle    15f5f <synchrotron_radiation+0x12f>
+	jle    15f1f <synchrotron_radiation+0x12f>
 	lea    0x10(%rdi,%rax,1),%rax
 	movsd  (%rax),%xmm0
 	mulsd  %xmm1,%xmm0
 	subsd  %xmm2,%xmm0
 	mulsd  %xmm1,%xmm0
 	subsd  %xmm2,%xmm0
 	movsd  %xmm0,(%rax)
 	lea    0x1(%r11),%ecx
 	add    $0x2,%r11d
 	cmp    %r11d,%r9d
-	jg     15e99 <synchrotron_radiation+0x69>
+	jg     15e59 <synchrotron_radiation+0x69>
 	mov    %esi,%edx
 	movapd %xmm1,%xmm4
 	movapd %xmm2,%xmm3
 	mov    %esi,%r9d
 	shr    %edx
 	unpcklpd %xmm4,%xmm4
 	unpcklpd %xmm3,%xmm3
 	and    $0xfffffffe,%r9d
 	shl    $0x4,%rdx
 	add    %rdi,%rdx
 	nopw   0x0(%rax,%rax,1)
 	cmp    $0x1,%esi
-	je     15fe0 <synchrotron_radiation+0x1b0>
+	je     15fa0 <synchrotron_radiation+0x1b0>
 	mov    %rdi,%rax
 	movupd (%rax),%xmm0
 	add    $0x10,%rax
 	mulpd  %xmm4,%xmm0
 	subpd  %xmm3,%xmm0
 	movups %xmm0,-0x10(%rax)
 	cmp    %rax,%rdx
-	jne    15fa0 <synchrotron_radiation+0x170>
+	jne    15f60 <synchrotron_radiation+0x170>
 	movslq %r9d,%rax
 	cmp    %r9d,%esi
-	je     15fd5 <synchrotron_radiation+0x1a5>
+	je     15f95 <synchrotron_radiation+0x1a5>
 	lea    (%rdi,%rax,8),%rax
 	movsd  (%rax),%xmm0
 	mulsd  %xmm1,%xmm0
 	subsd  %xmm2,%xmm0
 	movsd  %xmm0,(%rax)
 	add    $0x1,%ecx
 	cmp    %ecx,%r8d
-	jg     15f98 <synchrotron_radiation+0x168>
+	jg     15f58 <synchrotron_radiation+0x168>
 	pop    %rbx
 	pop    %rbp
 	ret
 	xor    %eax,%eax
-	jmp    15fc1 <synchrotron_radiation+0x191>
+	jmp    15f81 <synchrotron_radiation+0x191>
 	ret
 	xor    %ecx,%ecx
-	jmp    15f70 <synchrotron_radiation+0x140>
+	jmp    15f30 <synchrotron_radiation+0x140>
 	xor    %ecx,%ecx
-	jmp    15ef0 <synchrotron_radiation+0xc0>
+	jmp    15eb0 <synchrotron_radiation+0xc0>
 
-0000000000015ff0 <synchrotron_radiationf>:
+0000000000015fb0 <synchrotron_radiationf>:
 synchrotron_radiationf():
 	movaps %xmm0,%xmm4
-	movsd  0x23bd(%rip),%xmm0        
+	movsd  0x23fd(%rip),%xmm0        
 	cvtss2sd %xmm1,%xmm1
-	movsd  0x22d1(%rip),%xmm3        
+	movsd  0x2311(%rip),%xmm3        
 	divsd  %xmm1,%xmm0
 	subsd  %xmm0,%xmm3
 	test   %edx,%edx
-	jle    161d5 <synchrotron_radiationf+0x1e5>
+	jle    16195 <synchrotron_radiationf+0x1e5>
 	test   %esi,%esi
-	jle    161d5 <synchrotron_radiationf+0x1e5>
+	jle    16195 <synchrotron_radiationf+0x1e5>
 	push   %rbp
 	mov    %edx,%r9d
 	lea    -0x1(%rdx),%ecx
 	cvtsd2ss %xmm3,%xmm3
 	push   %rbx
 	cmp    $0x2,%edx
-	jle    161d6 <synchrotron_radiationf+0x1e6>
+	jle    16196 <synchrotron_radiationf+0x1e6>
 	mov    %esi,%edx
 	mov    %esi,%ebx
 	movaps %xmm3,%xmm2
 	mov    $0x1,%r11d
 	shr    $0x2,%edx
 	movaps %xmm4,%xmm1
 	lea    -0x1(%rsi),%r10d
 	and    $0xfffffffc,%ebx
 	shl    $0x4,%rdx
 	shufps $0x0,%xmm2,%xmm2
 	shufps $0x0,%xmm1,%xmm1
 	add    %rdi,%rdx
 	cmp    $0x2,%r10d
-	jbe    161e2 <synchrotron_radiationf+0x1f2>
+	jbe    161a2 <synchrotron_radiationf+0x1f2>
 	mov    %rdi,%rax
 	nopw   0x0(%rax,%rax,1)
 	movups (%rax),%xmm0
 	add    $0x10,%rax
 	mulps  %xmm2,%xmm0
 	subps  %xmm1,%xmm0
 	mulps  %xmm2,%xmm0
 	subps  %xmm1,%xmm0
 	movups %xmm0,-0x10(%rax)
 	cmp    %rdx,%rax
-	jne    16070 <synchrotron_radiationf+0x80>
+	jne    16030 <synchrotron_radiationf+0x80>
 	mov    %ebx,%r8d
 	cmp    %ebx,%esi
-	je     16105 <synchrotron_radiationf+0x115>
+	je     160c5 <synchrotron_radiationf+0x115>
 	movslq %r8d,%rax
 	shl    $0x2,%rax
 	lea    (%rdi,%rax,1),%rbp
 	movss  0x0(%rbp),%xmm0
 	mulss  %xmm3,%xmm0
 	subss  %xmm4,%xmm0
 	mulss  %xmm3,%xmm0
 	subss  %xmm4,%xmm0
 	movss  %xmm0,0x0(%rbp)
 	lea    0x1(%r8),%ebp
 	cmp    %ebp,%esi
-	jle    16105 <synchrotron_radiationf+0x115>
+	jle    160c5 <synchrotron_radiationf+0x115>
 	lea    0x4(%rdi,%rax,1),%rbp
 	add    $0x2,%r8d
 	movss  0x0(%rbp),%xmm0
 	mulss  %xmm3,%xmm0
 	subss  %xmm4,%xmm0
 	mulss  %xmm3,%xmm0
 	subss  %xmm4,%xmm0
 	movss  %xmm0,0x0(%rbp)
 	cmp    %r8d,%esi
-	jle    16105 <synchrotron_radiationf+0x115>
+	jle    160c5 <synchrotron_radiationf+0x115>
 	lea    0x8(%rdi,%rax,1),%rax
 	movss  (%rax),%xmm0
 	mulss  %xmm3,%xmm0
 	subss  %xmm4,%xmm0
 	mulss  %xmm3,%xmm0
 	subss  %xmm4,%xmm0
 	movss  %xmm0,(%rax)
 	lea    0x1(%r11),%r8d
 	add    $0x2,%r11d
 	cmp    %r11d,%ecx
-	jg     1605d <synchrotron_radiationf+0x6d>
+	jg     1601d <synchrotron_radiationf+0x6d>
 	mov    %esi,%edx
 	movaps %xmm3,%xmm2
 	movaps %xmm4,%xmm1
 	mov    %esi,%r11d
 	shr    $0x2,%edx
 	and    $0xfffffffc,%r11d
 	shufps $0x0,%xmm2,%xmm2
 	shufps $0x0,%xmm1,%xmm1
 	shl    $0x4,%rdx
 	add    %rdi,%rdx
 	nopw   0x0(%rax,%rax,1)
 	cmp    $0x2,%r10d
-	jbe    161d1 <synchrotron_radiationf+0x1e1>
+	jbe    16191 <synchrotron_radiationf+0x1e1>
 	mov    %rdi,%rax
 	nopl   (%rax)
 	movups (%rax),%xmm0
 	add    $0x10,%rax
 	mulps  %xmm2,%xmm0
 	subps  %xmm1,%xmm0
 	movups %xmm0,-0x10(%rax)
 	cmp    %rax,%rdx
-	jne    16150 <synchrotron_radiationf+0x160>
+	jne    16110 <synchrotron_radiationf+0x160>
 	mov    %r11d,%ecx
 	cmp    %r11d,%esi
-	je     161c1 <synchrotron_radiationf+0x1d1>
+	je     16181 <synchrotron_radiationf+0x1d1>
 	movslq %ecx,%rax
 	shl    $0x2,%rax
 	lea    (%rdi,%rax,1),%rbx
 	movss  (%rbx),%xmm0
 	mulss  %xmm3,%xmm0
 	subss  %xmm4,%xmm0
 	movss  %xmm0,(%rbx)
 	lea    0x1(%rcx),%ebx
 	cmp    %ebx,%esi
-	jle    161c1 <synchrotron_radiationf+0x1d1>
+	jle    16181 <synchrotron_radiationf+0x1d1>
 	lea    0x4(%rdi,%rax,1),%rbx
 	add    $0x2,%ecx
 	movss  (%rbx),%xmm0
 	mulss  %xmm3,%xmm0
 	subss  %xmm4,%xmm0
 	movss  %xmm0,(%rbx)
 	cmp    %ecx,%esi
-	jle    161c1 <synchrotron_radiationf+0x1d1>
+	jle    16181 <synchrotron_radiationf+0x1d1>
 	lea    0x8(%rdi,%rax,1),%rax
 	movss  (%rax),%xmm0
 	mulss  %xmm3,%xmm0
 	subss  %xmm4,%xmm0
 	movss  %xmm0,(%rax)
 	add    $0x1,%r8d
 	cmp    %r8d,%r9d
-	jg     16140 <synchrotron_radiationf+0x150>
+	jg     16100 <synchrotron_radiationf+0x150>
 	pop    %rbx
 	pop    %rbp
 	ret
 	xor    %ecx,%ecx
-	jmp    1616e <synchrotron_radiationf+0x17e>
+	jmp    1612e <synchrotron_radiationf+0x17e>
 	ret
 	xor    %r8d,%r8d
 	lea    -0x1(%rsi),%r10d
-	jmp    16116 <synchrotron_radiationf+0x126>
+	jmp    160d6 <synchrotron_radiationf+0x126>
 	xor    %r8d,%r8d
-	jmp    16093 <synchrotron_radiationf+0xa3>
+	jmp    16053 <synchrotron_radiationf+0xa3>
 	nopw   0x0(%rax,%rax,1)
 
-00000000000161f0 <set_random_seed>:
+00000000000161b0 <set_random_seed>:
 set_random_seed():
-	mov    0x5dd9(%rip),%rax        
+	mov    0x5e19(%rip),%rax        
 	movslq %edi,%rdi
 	mov    %rdi,(%rax)
 	ret
 	xchg   %ax,%ax
 
-0000000000016200 <synchrotron_radiation_full>:
+00000000000161c0 <synchrotron_radiation_full>:
 synchrotron_radiation_full():
 	push   %r15
 	addsd  %xmm1,%xmm1
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
 	sub    $0x58,%rsp
-	movsd  0x20be(%rip),%xmm4        
+	movsd  0x20fe(%rip),%xmm4        
 	movsd  %xmm0,0x28(%rsp)
 	movapd %xmm2,%xmm0
 	sqrtsd %xmm0,%xmm0
 	movapd %xmm4,%xmm6
 	mov    %rdi,0x48(%rsp)
 	mov    %esi,0x40(%rsp)
 	mov    %edx,0x44(%rsp)
 	divsd  %xmm0,%xmm1
-	movsd  0x2173(%rip),%xmm0        
+	movsd  0x21b3(%rip),%xmm0        
 	divsd  %xmm2,%xmm0
 	mulsd  %xmm3,%xmm1
 	movsd  %xmm1,0x18(%rsp)
 	subsd  %xmm0,%xmm6
 	movsd  %xmm6,0x20(%rsp)
 	test   %edx,%edx
-	jle    1665b <synchrotron_radiation_full+0x45b>
+	jle    1661b <synchrotron_radiation_full+0x45b>
 	movabs $0x5555555555555555,%rbp
 	mov    %rdi,%r14
 	mov    %esi,%ebx
-	lea    0x5d45(%rip),%rdi        
+	lea    0x5d85(%rip),%rdi        
 	call   3240 <__tls_get_addr@plt>
 	movl   $0x0,0x3c(%rsp)
 	mov    0x60(%rax),%r15
 	lea    -0x1(%rbx),%eax
 	lea    0x8(%r14,%rax,8),%r13
 	nopw   0x0(%rax,%rax,1)
 	test   %r15,%r15
-	je     1666a <synchrotron_radiation_full+0x46a>
-	lea    0x5d10(%rip),%rdi        
+	je     1662a <synchrotron_radiation_full+0x46a>
+	lea    0x5d50(%rip),%rdi        
 	call   3240 <__tls_get_addr@plt>
 	cmpb   $0x0,0x38(%rax)
-	jne    162db <synchrotron_radiation_full+0xdb>
-	movapd 0x21aa(%rip),%xmm6        
+	jne    1629b <synchrotron_radiation_full+0xdb>
+	movapd 0x21ea(%rip),%xmm6        
 	movb   $0x0,0x58(%rax)
 	movb   $0x1,0x38(%rax)
 	movaps %xmm6,0x40(%rax)
 	mov    0x40(%rsp),%eax
 	test   %eax,%eax
-	jle    16648 <synchrotron_radiation_full+0x448>
-	lea    0x5cd2(%rip),%rdi        
+	jle    16608 <synchrotron_radiation_full+0x448>
+	lea    0x5d12(%rip),%rdi        
 	call   3240 <__tls_get_addr@plt>
 	mov    0x48(%rsp),%r12
 	movabs $0x71d67fffeda60000,%rbx
 	movzbl 0x58(%rax),%r14d
-	mov    0x1fc7(%rip),%rax        
+	mov    0x2007(%rip),%rax        
 	movq   %rax,%xmm4
-	jmp    1639a <synchrotron_radiation_full+0x19a>
+	jmp    1635a <synchrotron_radiation_full+0x19a>
 	nopl   0x0(%rax,%rax,1)
-	lea    0x5c99(%rip),%rdi        
+	lea    0x5cd9(%rip),%rdi        
 	call   3240 <__tls_get_addr@plt>
 	xor    %r14d,%r14d
 	movb   $0x0,0x58(%rax)
 	movsd  0x50(%rax),%xmm2
 	movsd  %xmm2,(%rsp)
 	add    $0x8,%r12
-	lea    0x5c72(%rip),%rdi        
+	lea    0x5cb2(%rip),%rdi        
 	call   3240 <__tls_get_addr@plt>
 	movsd  (%rsp),%xmm2
 	movsd  0x10(%rsp),%xmm0
 	subsd  0x28(%rsp),%xmm0
 	mulsd  0x48(%rax),%xmm2
 	addsd  0x40(%rax),%xmm2
 	mulsd  0x18(%rsp),%xmm2
-	mov    0x1f57(%rip),%rax        
+	mov    0x1f97(%rip),%rax        
 	movq   %rax,%xmm4
 	addsd  %xmm0,%xmm2
 	movsd  %xmm2,-0x8(%r12)
 	cmp    %r13,%r12
-	je     16648 <synchrotron_radiation_full+0x448>
+	je     16608 <synchrotron_radiation_full+0x448>
 	movsd  0x20(%rsp),%xmm6
 	mulsd  (%r12),%xmm6
 	movsd  %xmm6,0x10(%rsp)
 	test   %r14b,%r14b
-	jne    16320 <synchrotron_radiation_full+0x120>
+	jne    162e0 <synchrotron_radiation_full+0x120>
 	mov    0x9c0(%r15),%rsi
 	movabs $0xfff7eee000000000,%r14
 	cs nopw 0x0(%rax,%rax,1)
 	cmp    $0x137,%rsi
-	ja     165d0 <synchrotron_radiation_full+0x3d0>
+	ja     16590 <synchrotron_radiation_full+0x3d0>
 	mov    (%r15,%rsi,8),%rax
 	lea    0x1(%rsi),%rdi
 	pxor   %xmm1,%xmm1
 	mov    %rdi,0x9c0(%r15)
 	mov    %rax,%rsi
 	shr    $0x1d,%rsi
 	and    %rbp,%rsi
@@ -19133,30 +19127,30 @@
 	shl    $0x25,%rsi
 	and    %r14,%rsi
 	xor    %rsi,%rax
 	mov    %rax,%rsi
 	shr    $0x2b,%rsi
 	xor    %rsi,%rax
 	cvtsi2sd %rax,%xmm1
-	jns    16441 <synchrotron_radiation_full+0x241>
+	jns    16401 <synchrotron_radiation_full+0x241>
 	mov    %rax,%rsi
 	and    $0x1,%eax
 	pxor   %xmm1,%xmm1
 	shr    %rsi
 	or     %rax,%rsi
 	cvtsi2sd %rsi,%xmm1
 	addsd  %xmm1,%xmm1
-	comisd 0x1ff7(%rip),%xmm1        
-	jae    16628 <synchrotron_radiation_full+0x428>
-	mulsd  0x1ff1(%rip),%xmm1        
+	comisd 0x2037(%rip),%xmm1        
+	jae    165e8 <synchrotron_radiation_full+0x428>
+	mulsd  0x2031(%rip),%xmm1        
 	subsd  %xmm4,%xmm1
 	movapd %xmm1,%xmm5
 	mulsd  %xmm1,%xmm5
 	cmp    $0x137,%rdi
-	ja     16590 <synchrotron_radiation_full+0x390>
+	ja     16550 <synchrotron_radiation_full+0x390>
 	mov    (%r15,%rdi,8),%rax
 	lea    0x1(%rdi),%rsi
 	pxor   %xmm0,%xmm0
 	mov    %rsi,0x9c0(%r15)
 	mov    %rax,%rdi
 	shr    $0x1d,%rdi
 	and    %rbp,%rdi
@@ -19169,101 +19163,101 @@
 	shl    $0x25,%rdi
 	and    %r14,%rdi
 	xor    %rdi,%rax
 	mov    %rax,%rdi
 	shr    $0x2b,%rdi
 	xor    %rdi,%rax
 	cvtsi2sd %rax,%xmm0
-	jns    164d4 <synchrotron_radiation_full+0x2d4>
+	jns    16494 <synchrotron_radiation_full+0x2d4>
 	mov    %rax,%rdi
 	and    $0x1,%eax
 	pxor   %xmm0,%xmm0
 	shr    %rdi
 	or     %rax,%rdi
 	cvtsi2sd %rdi,%xmm0
 	addsd  %xmm0,%xmm0
-	comisd 0x1f64(%rip),%xmm0        
-	jae    165f0 <synchrotron_radiation_full+0x3f0>
-	mulsd  0x1f5e(%rip),%xmm0        
+	comisd 0x1fa4(%rip),%xmm0        
+	jae    165b0 <synchrotron_radiation_full+0x3f0>
+	mulsd  0x1f9e(%rip),%xmm0        
 	movapd %xmm0,%xmm2
 	subsd  %xmm4,%xmm2
 	movapd %xmm2,%xmm3
 	mulsd  %xmm2,%xmm3
 	addsd  %xmm5,%xmm3
 	comisd %xmm3,%xmm4
-	jb     163d0 <synchrotron_radiation_full+0x1d0>
-	comisd 0x1e08(%rip),%xmm3        
-	je     163d0 <synchrotron_radiation_full+0x1d0>
+	jb     16390 <synchrotron_radiation_full+0x1d0>
+	comisd 0x1e48(%rip),%xmm3        
+	je     16390 <synchrotron_radiation_full+0x1d0>
 	movapd %xmm3,%xmm0
 	movsd  %xmm3,(%rsp)
 	mov    $0x1,%r14d
 	movsd  %xmm1,0x30(%rsp)
 	movsd  %xmm2,0x8(%rsp)
 	call   3100 <log@plt>
-	mulsd  0x1f22(%rip),%xmm0        
+	mulsd  0x1f62(%rip),%xmm0        
 	movsd  (%rsp),%xmm3
 	divsd  %xmm3,%xmm0
 	sqrtsd %xmm0,%xmm0
 	movsd  %xmm0,(%rsp)
-	lea    0x5a69(%rip),%rdi        
+	lea    0x5aa9(%rip),%rdi        
 	call   3240 <__tls_get_addr@plt>
 	movsd  (%rsp),%xmm0
 	movsd  0x30(%rsp),%xmm1
 	movsd  0x8(%rsp),%xmm2
 	mulsd  %xmm0,%xmm1
 	mulsd  %xmm0,%xmm2
 	movb   $0x1,0x58(%rax)
 	movsd  %xmm1,0x50(%rax)
-	jmp    1633e <synchrotron_radiation_full+0x13e>
+	jmp    162fe <synchrotron_radiation_full+0x13e>
 	nopl   0x0(%rax)
 	mov    %r15,%rdi
 	movsd  %xmm5,0x8(%rsp)
 	movsd  %xmm1,(%rsp)
 	call   3270 <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()@plt>
 	movsd  0x8(%rsp),%xmm5
 	movsd  (%rsp),%xmm1
-	mov    0x1d23(%rip),%rax        
+	mov    0x1d63(%rip),%rax        
 	mov    0x9c0(%r15),%rdi
 	movq   %rax,%xmm4
-	jmp    16470 <synchrotron_radiation_full+0x270>
+	jmp    16430 <synchrotron_radiation_full+0x270>
 	cs nopw 0x0(%rax,%rax,1)
 	mov    %r15,%rdi
 	call   3270 <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()@plt>
-	mov    0x1cf9(%rip),%rax        
+	mov    0x1d39(%rip),%rax        
 	mov    0x9c0(%r15),%rsi
 	movq   %rax,%xmm4
-	jmp    163dd <synchrotron_radiation_full+0x1dd>
-	comisd 0x1e58(%rip),%xmm5        
-	movsd  0x1e30(%rip),%xmm3        
+	jmp    1639d <synchrotron_radiation_full+0x1dd>
+	comisd 0x1e98(%rip),%xmm5        
+	movsd  0x1e70(%rip),%xmm3        
 	addsd  %xmm5,%xmm3
-	ja     163d0 <synchrotron_radiation_full+0x1d0>
-	comisd 0x1e46(%rip),%xmm5        
-	je     163d0 <synchrotron_radiation_full+0x1d0>
-	movsd  0x1e18(%rip),%xmm2        
-	jmp    16516 <synchrotron_radiation_full+0x316>
+	ja     16390 <synchrotron_radiation_full+0x1d0>
+	comisd 0x1e86(%rip),%xmm5        
+	je     16390 <synchrotron_radiation_full+0x1d0>
+	movsd  0x1e58(%rip),%xmm2        
+	jmp    164d6 <synchrotron_radiation_full+0x316>
 	nopl   (%rax)
-	mov    0x1e01(%rip),%rax        
-	movsd  0x1e01(%rip),%xmm1        
+	mov    0x1e41(%rip),%rax        
+	movsd  0x1e41(%rip),%xmm1        
 	movq   %rax,%xmm5
-	jmp    16463 <synchrotron_radiation_full+0x263>
+	jmp    16423 <synchrotron_radiation_full+0x263>
 	nopl   0x0(%rax)
 	addl   $0x1,0x3c(%rsp)
 	mov    0x3c(%rsp),%eax
 	cmp    %eax,0x44(%rsp)
-	jne    162a0 <synchrotron_radiation_full+0xa0>
+	jne    16260 <synchrotron_radiation_full+0xa0>
 	add    $0x58,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	call   3040 <omp_get_thread_num()@plt>
-	mov    0x595a(%rip),%rdx        
+	mov    0x599a(%rip),%rdx        
 	mov    $0x9c8,%edi
 	cltq
 	add    (%rdx),%rax
 	mov    %rax,%rbx
 	call   3160 <operator new(unsigned long)@plt>
 	mov    $0x1,%ecx
 	movabs $0x5851f42d4c957f2d,%rsi
@@ -19274,23 +19268,23 @@
 	shr    $0x3e,%rax
 	xor    %rbx,%rax
 	imul   %rsi,%rax
 	lea    (%rax,%rcx,1),%rbx
 	mov    %rbx,(%r15,%rcx,8)
 	add    $0x1,%rcx
 	cmp    $0x138,%rcx
-	jne    166a0 <synchrotron_radiation_full+0x4a0>
+	jne    16660 <synchrotron_radiation_full+0x4a0>
 	movq   $0x138,0x9c0(%r15)
-	lea    0x58eb(%rip),%rdi        
+	lea    0x592b(%rip),%rdi        
 	call   3240 <__tls_get_addr@plt>
 	mov    %r15,0x60(%rax)
-	jmp    162a9 <synchrotron_radiation_full+0xa9>
+	jmp    16269 <synchrotron_radiation_full+0xa9>
 	cs nopw 0x0(%rax,%rax,1)
 
-00000000000166f0 <synchrotron_radiation_fullf>:
+00000000000166b0 <synchrotron_radiation_fullf>:
 synchrotron_radiation_fullf():
 	movaps %xmm2,%xmm4
 	cvtss2sd %xmm1,%xmm1
 	addsd  %xmm1,%xmm1
 	push   %r15
 	sqrtss %xmm4,%xmm4
 	push   %r14
@@ -19300,103 +19294,103 @@
 	pxor   %xmm7,%xmm7
 	push   %r12
 	cvtss2sd %xmm4,%xmm4
 	divsd  %xmm4,%xmm1
 	push   %rbp
 	push   %rbx
 	sub    $0x58,%rsp
-	movsd  0x1baf(%rip),%xmm4        
+	movsd  0x1bef(%rip),%xmm4        
 	mov    %rdi,0x48(%rsp)
 	mov    %esi,0x40(%rsp)
 	mov    %edx,0x44(%rsp)
 	movss  %xmm0,0x10(%rsp)
 	mulsd  %xmm3,%xmm1
-	movsd  0x1c70(%rip),%xmm3        
+	movsd  0x1cb0(%rip),%xmm3        
 	divsd  %xmm2,%xmm3
 	movapd %xmm4,%xmm2
 	cvtsd2ss %xmm1,%xmm1
 	movss  %xmm1,0x8(%rsp)
 	subsd  %xmm3,%xmm2
 	cvtsd2ss %xmm2,%xmm7
 	movss  %xmm7,0x38(%rsp)
 	test   %edx,%edx
-	jle    16b8b <synchrotron_radiation_fullf+0x49b>
+	jle    16b4b <synchrotron_radiation_fullf+0x49b>
 	mov    %rdi,%r14
 	mov    %esi,%ebx
-	lea    0x5844(%rip),%rdi        
+	lea    0x5884(%rip),%rdi        
 	call   3240 <__tls_get_addr@plt>
 	movss  0x8(%rsp),%xmm1
 	movss  0x10(%rsp),%xmm0
 	pxor   %xmm7,%xmm7
 	movl   $0x0,0x3c(%rsp)
 	cvtss2sd %xmm1,%xmm7
 	movsd  %xmm7,0x20(%rsp)
 	pxor   %xmm7,%xmm7
 	cvtss2sd %xmm0,%xmm7
 	movsd  %xmm7,0x28(%rsp)
 	mov    0x30(%rax),%r15
 	lea    -0x1(%rbx),%eax
 	lea    0x4(%r14,%rax,4),%r13
 	test   %r15,%r15
-	je     16b9a <synchrotron_radiation_fullf+0x4aa>
-	lea    0x57f0(%rip),%rdi        
+	je     16b5a <synchrotron_radiation_fullf+0x4aa>
+	lea    0x5830(%rip),%rdi        
 	call   3240 <__tls_get_addr@plt>
 	cmpb   $0x0,0x0(%rax)
-	jne    167fb <synchrotron_radiation_fullf+0x10b>
-	movapd 0x1c8a(%rip),%xmm7        
+	jne    167bb <synchrotron_radiation_fullf+0x10b>
+	movapd 0x1cca(%rip),%xmm7        
 	movb   $0x0,0x28(%rax)
 	movb   $0x1,0x0(%rax)
 	movaps %xmm7,0x10(%rax)
 	mov    0x40(%rsp),%eax
 	test   %eax,%eax
-	jle    16b78 <synchrotron_radiation_fullf+0x488>
-	lea    0x57b2(%rip),%rdi        
+	jle    16b38 <synchrotron_radiation_fullf+0x488>
+	lea    0x57f2(%rip),%rdi        
 	call   3240 <__tls_get_addr@plt>
 	mov    0x48(%rsp),%r12
 	movabs $0x5555555555555555,%rbp
 	movabs $0x71d67fffeda60000,%rbx
 	movzbl 0x28(%rax),%r14d
-	mov    0x1a9d(%rip),%rax        
+	mov    0x1add(%rip),%rax        
 	movq   %rax,%xmm4
-	jmp    168c8 <synchrotron_radiation_fullf+0x1d8>
+	jmp    16888 <synchrotron_radiation_fullf+0x1d8>
 	nopl   (%rax)
-	lea    0x5771(%rip),%rdi        
+	lea    0x57b1(%rip),%rdi        
 	call   3240 <__tls_get_addr@plt>
 	xor    %r14d,%r14d
 	movb   $0x0,0x28(%rax)
 	movsd  0x20(%rax),%xmm2
 	movsd  %xmm2,0x8(%rsp)
 	add    $0x4,%r12
-	lea    0x5749(%rip),%rdi        
+	lea    0x5789(%rip),%rdi        
 	call   3240 <__tls_get_addr@plt>
 	movsd  0x8(%rsp),%xmm2
 	movsd  0x18(%rsp),%xmm0
 	subsd  0x28(%rsp),%xmm0
 	mulsd  0x18(%rax),%xmm2
 	addsd  0x10(%rax),%xmm2
 	mulsd  0x20(%rsp),%xmm2
-	mov    0x1a2d(%rip),%rax        
+	mov    0x1a6d(%rip),%rax        
 	movq   %rax,%xmm4
 	addsd  %xmm2,%xmm0
 	cvtsd2ss %xmm0,%xmm0
 	movss  %xmm0,-0x4(%r12)
 	cmp    %r13,%r12
-	je     16b78 <synchrotron_radiation_fullf+0x488>
+	je     16b38 <synchrotron_radiation_fullf+0x488>
 	movss  0x38(%rsp),%xmm0
 	mulss  (%r12),%xmm0
 	pxor   %xmm6,%xmm6
 	cvtss2sd %xmm0,%xmm6
 	movsd  %xmm6,0x18(%rsp)
 	test   %r14b,%r14b
-	jne    16848 <synchrotron_radiation_fullf+0x158>
+	jne    16808 <synchrotron_radiation_fullf+0x158>
 	mov    0x9c0(%r15),%rdx
 	movabs $0xfff7eee000000000,%r14
 	nopl   0x0(%rax)
 	cmp    $0x137,%rdx
-	ja     16b00 <synchrotron_radiation_fullf+0x410>
+	ja     16ac0 <synchrotron_radiation_fullf+0x410>
 	mov    (%r15,%rdx,8),%rax
 	lea    0x1(%rdx),%rcx
 	pxor   %xmm1,%xmm1
 	mov    %rcx,0x9c0(%r15)
 	mov    %rax,%rdx
 	shr    $0x1d,%rdx
 	and    %rbp,%rdx
@@ -19409,30 +19403,30 @@
 	shl    $0x25,%rdx
 	and    %r14,%rdx
 	xor    %rdx,%rax
 	mov    %rax,%rdx
 	shr    $0x2b,%rdx
 	xor    %rdx,%rax
 	cvtsi2sd %rax,%xmm1
-	jns    16971 <synchrotron_radiation_fullf+0x281>
+	jns    16931 <synchrotron_radiation_fullf+0x281>
 	mov    %rax,%rdx
 	and    $0x1,%eax
 	pxor   %xmm1,%xmm1
 	shr    %rdx
 	or     %rax,%rdx
 	cvtsi2sd %rdx,%xmm1
 	addsd  %xmm1,%xmm1
-	comisd 0x1ac7(%rip),%xmm1        
-	jae    16b58 <synchrotron_radiation_fullf+0x468>
-	mulsd  0x1ac1(%rip),%xmm1        
+	comisd 0x1b07(%rip),%xmm1        
+	jae    16b18 <synchrotron_radiation_fullf+0x468>
+	mulsd  0x1b01(%rip),%xmm1        
 	subsd  %xmm4,%xmm1
 	movapd %xmm1,%xmm5
 	mulsd  %xmm1,%xmm5
 	cmp    $0x137,%rcx
-	ja     16ac0 <synchrotron_radiation_fullf+0x3d0>
+	ja     16a80 <synchrotron_radiation_fullf+0x3d0>
 	mov    (%r15,%rcx,8),%rax
 	lea    0x1(%rcx),%rdx
 	pxor   %xmm0,%xmm0
 	mov    %rdx,0x9c0(%r15)
 	mov    %rax,%rcx
 	shr    $0x1d,%rcx
 	and    %rbp,%rcx
@@ -19445,103 +19439,103 @@
 	shl    $0x25,%rcx
 	and    %r14,%rcx
 	xor    %rcx,%rax
 	mov    %rax,%rcx
 	shr    $0x2b,%rcx
 	xor    %rcx,%rax
 	cvtsi2sd %rax,%xmm0
-	jns    16a04 <synchrotron_radiation_fullf+0x314>
+	jns    169c4 <synchrotron_radiation_fullf+0x314>
 	mov    %rax,%rcx
 	and    $0x1,%eax
 	pxor   %xmm0,%xmm0
 	shr    %rcx
 	or     %rax,%rcx
 	cvtsi2sd %rcx,%xmm0
 	addsd  %xmm0,%xmm0
-	comisd 0x1a34(%rip),%xmm0        
-	jae    16b20 <synchrotron_radiation_fullf+0x430>
-	mulsd  0x1a2e(%rip),%xmm0        
+	comisd 0x1a74(%rip),%xmm0        
+	jae    16ae0 <synchrotron_radiation_fullf+0x430>
+	mulsd  0x1a6e(%rip),%xmm0        
 	movapd %xmm0,%xmm2
 	subsd  %xmm4,%xmm2
 	movapd %xmm2,%xmm3
 	mulsd  %xmm2,%xmm3
 	addsd  %xmm5,%xmm3
 	comisd %xmm3,%xmm4
-	jb     16900 <synchrotron_radiation_fullf+0x210>
-	comisd 0x18d8(%rip),%xmm3        
-	je     16900 <synchrotron_radiation_fullf+0x210>
+	jb     168c0 <synchrotron_radiation_fullf+0x210>
+	comisd 0x1918(%rip),%xmm3        
+	je     168c0 <synchrotron_radiation_fullf+0x210>
 	movapd %xmm3,%xmm0
 	movsd  %xmm1,0x30(%rsp)
 	mov    $0x1,%r14d
 	movsd  %xmm2,0x10(%rsp)
 	movsd  %xmm3,0x8(%rsp)
 	call   3100 <log@plt>
-	mulsd  0x19f1(%rip),%xmm0        
+	mulsd  0x1a31(%rip),%xmm0        
 	movsd  0x8(%rsp),%xmm3
 	divsd  %xmm3,%xmm0
 	sqrtsd %xmm0,%xmm0
 	movsd  %xmm0,0x8(%rsp)
-	lea    0x5536(%rip),%rdi        
+	lea    0x5576(%rip),%rdi        
 	call   3240 <__tls_get_addr@plt>
 	movsd  0x8(%rsp),%xmm0
 	movsd  0x30(%rsp),%xmm1
 	movsd  0x10(%rsp),%xmm2
 	mulsd  %xmm0,%xmm1
 	mulsd  %xmm0,%xmm2
 	movb   $0x1,0x28(%rax)
 	movsd  %xmm1,0x20(%rax)
-	jmp    16866 <synchrotron_radiation_fullf+0x176>
+	jmp    16826 <synchrotron_radiation_fullf+0x176>
 	nopl   (%rax)
 	mov    %r15,%rdi
 	movsd  %xmm5,0x10(%rsp)
 	movsd  %xmm1,0x8(%rsp)
 	call   3270 <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()@plt>
-	mov    0x17fd(%rip),%rax        
+	mov    0x183d(%rip),%rax        
 	mov    0x9c0(%r15),%rcx
 	movsd  0x10(%rsp),%xmm5
 	movsd  0x8(%rsp),%xmm1
 	movq   %rax,%xmm4
-	jmp    169a0 <synchrotron_radiation_fullf+0x2b0>
+	jmp    16960 <synchrotron_radiation_fullf+0x2b0>
 	nopl   0x0(%rax,%rax,1)
 	mov    %r15,%rdi
 	call   3270 <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()@plt>
-	mov    0x17c9(%rip),%rax        
+	mov    0x1809(%rip),%rax        
 	mov    0x9c0(%r15),%rdx
 	movq   %rax,%xmm4
-	jmp    1690d <synchrotron_radiation_fullf+0x21d>
-	comisd 0x1928(%rip),%xmm5        
-	movsd  0x1900(%rip),%xmm3        
+	jmp    168cd <synchrotron_radiation_fullf+0x21d>
+	comisd 0x1968(%rip),%xmm5        
+	movsd  0x1940(%rip),%xmm3        
 	addsd  %xmm5,%xmm3
-	ja     16900 <synchrotron_radiation_fullf+0x210>
-	comisd 0x1916(%rip),%xmm5        
-	je     16900 <synchrotron_radiation_fullf+0x210>
-	movsd  0x18e8(%rip),%xmm2        
-	jmp    16a46 <synchrotron_radiation_fullf+0x356>
+	ja     168c0 <synchrotron_radiation_fullf+0x210>
+	comisd 0x1956(%rip),%xmm5        
+	je     168c0 <synchrotron_radiation_fullf+0x210>
+	movsd  0x1928(%rip),%xmm2        
+	jmp    16a06 <synchrotron_radiation_fullf+0x356>
 	nopl   (%rax)
-	mov    0x18d1(%rip),%rax        
-	movsd  0x18d1(%rip),%xmm1        
+	mov    0x1911(%rip),%rax        
+	movsd  0x1911(%rip),%xmm1        
 	movq   %rax,%xmm5
-	jmp    16993 <synchrotron_radiation_fullf+0x2a3>
+	jmp    16953 <synchrotron_radiation_fullf+0x2a3>
 	nopl   0x0(%rax)
 	addl   $0x1,0x3c(%rsp)
 	mov    0x3c(%rsp),%eax
 	cmp    %eax,0x44(%rsp)
-	jne    167c0 <synchrotron_radiation_fullf+0xd0>
+	jne    16780 <synchrotron_radiation_fullf+0xd0>
 	add    $0x58,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	call   3040 <omp_get_thread_num()@plt>
 	mov    $0x9c8,%edi
 	movslq %eax,%rbx
-	mov    0x5422(%rip),%rax        
+	mov    0x5462(%rip),%rax        
 	add    (%rax),%rbx
 	call   3160 <operator new(unsigned long)@plt>
 	mov    $0x1,%ecx
 	mov    %rbx,(%rax)
 	mov    %rax,%r15
 	nopl   0x0(%rax)
 	movabs $0x5851f42d4c957f2d,%rsi
@@ -19549,23 +19543,23 @@
 	shr    $0x3e,%rax
 	xor    %rbx,%rax
 	imul   %rsi,%rax
 	lea    (%rax,%rcx,1),%rbx
 	mov    %rbx,(%r15,%rcx,8)
 	add    $0x1,%rcx
 	cmp    $0x138,%rcx
-	jne    16bc8 <synchrotron_radiation_fullf+0x4d8>
+	jne    16b88 <synchrotron_radiation_fullf+0x4d8>
 	movq   $0x138,0x9c0(%r15)
-	lea    0x53b9(%rip),%rdi        
+	lea    0x53f9(%rip),%rdi        
 	call   3240 <__tls_get_addr@plt>
 	mov    %r15,0x30(%rax)
-	jmp    167c9 <synchrotron_radiation_fullf+0xd9>
+	jmp    16789 <synchrotron_radiation_fullf+0xd9>
 	nopl   0x0(%rax,%rax,1)
 
-0000000000016c20 <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()>:
+0000000000016be0 <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()>:
 std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand():
 	movabs $0xb5026f5aa96619e9,%r10
 	mov    %rdi,%r8
 	mov    (%rdi),%rdi
 	mov    %r8,%rax
 	lea    0x4e0(%r8),%r9
 	mov    %r8,%rdx
@@ -19576,71 +19570,71 @@
 	mov    %rdi,%rsi
 	and    $0x7fffffff,%esi
 	or     %rcx,%rsi
 	mov    %rsi,%rcx
 	shr    %rcx
 	xor    0x4e0(%rdx),%rcx
 	and    $0x1,%esi
-	je     16c6f <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()+0x4f>
+	je     16c2f <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()+0x4f>
 	xor    %r10,%rcx
 	mov    %rcx,(%rdx)
 	add    $0x8,%rdx
 	cmp    %r9,%rdx
-	jne    16c40 <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()+0x20>
+	jne    16c00 <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()+0x20>
 	mov    0x4e0(%r8),%rsi
 	lea    0x4d8(%r8),%rdi
 	movabs $0xb5026f5aa96619e9,%r9
 	nopl   0x0(%rax,%rax,1)
 	and    $0xffffffff80000000,%rsi
 	mov    %rsi,%rdx
 	mov    0x4e8(%rax),%rsi
 	mov    %rsi,%rcx
 	and    $0x7fffffff,%ecx
 	or     %rdx,%rcx
 	mov    %rcx,%rdx
 	shr    %rdx
 	xor    (%rax),%rdx
 	and    $0x1,%ecx
-	je     16cc6 <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()+0xa6>
+	je     16c86 <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()+0xa6>
 	xor    %r9,%rdx
 	mov    %rdx,0x4e0(%rax)
 	add    $0x8,%rax
 	cmp    %rdi,%rax
-	jne    16c98 <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()+0x78>
+	jne    16c58 <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()+0x78>
 	mov    0x9b8(%r8),%rax
 	mov    (%r8),%rdx
 	and    $0xffffffff80000000,%rax
 	and    $0x7fffffff,%edx
 	or     %rdx,%rax
 	mov    %rax,%rdx
 	shr    %rdx
 	xor    0x4d8(%r8),%rdx
 	test   $0x1,%al
-	je     16d0d <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()+0xed>
+	je     16ccd <std::mersenne_twister_engine<unsigned long, 64ul, 312ul, 156ul, 31ul, 13043109905998158313ul, 29ul, 6148914691236517205ul, 17ul, 8202884508482404352ul, 37ul, 18444473444759240704ul, 43ul, 6364136223846793005ul>::_M_gen_rand()+0xed>
 	movabs $0xb5026f5aa96619e9,%rax
 	xor    %rax,%rdx
 	mov    %rdx,0x9b8(%r8)
 	movq   $0x0,0x9c0(%r8)
 	ret
 
-0000000000016d20 <sparse_histogram>:
+0000000000016ce0 <sparse_histogram>:
 sparse_histogram():
 	push   %r15
 	mov    %r9d,%r15d
 	push   %r14
 	xor    %r14d,%r14d
 	push   %r13
 	mov    %rsi,%r13
 	push   %r12
 	push   %rbp
 	push   %rbx
 	sub    $0x58,%rsp
 	movsd  (%rcx),%xmm0
 	subsd  (%rdx),%xmm0
-	movsd  0x1591(%rip),%xmm5        
+	movsd  0x15d1(%rip),%xmm5        
 	mov    0x90(%rsp),%ebx
 	mov    %rdx,0x20(%rsp)
 	mov    0x98(%rsp),%eax
 	mov    %rcx,0x38(%rsp)
 	divsd  %xmm0,%xmm5
 	pxor   %xmm0,%xmm0
 	mov    %r8,0x48(%rsp)
@@ -19667,24 +19661,24 @@
 	shl    $0x3,%rdi
 	call   31a0 <malloc@plt>
 	mov    %ebx,0x34(%rsp)
 	movslq %ebx,%rbx
 	mov    %rax,(%r12)
 	mov    %rax,%rbp
 	shl    $0x3,%rbx
-	jmp    16df2 <sparse_histogram+0xd2>
+	jmp    16db2 <sparse_histogram+0xd2>
 	nopl   0x0(%rax)
 	add    %r15,%rbp
 	add    %rbx,%r15
 	mov    %rbp,(%r12,%r14,8)
 	mov    (%r12),%rbp
 	add    $0x1,%r14
 	call   31c0 <omp_get_max_threads()@plt>
 	cmp    %r14d,%eax
-	jg     16de0 <sparse_histogram+0xc0>
+	jg     16da0 <sparse_histogram+0xc0>
 	call   3040 <omp_get_thread_num()@plt>
 	movslq %eax,%rbx
 	call   3090 <omp_get_num_threads()@plt>
 	mov    0x18(%rsp),%ecx
 	imul   0x1c(%rsp),%ecx
 	xor    %esi,%esi
 	mov    (%r12,%rbx,8),%r9
@@ -19695,83 +19689,83 @@
 	shl    $0x3,%rdx
 	call   30f0 <memset@plt>
 	mov    0x2c(%rsp),%ecx
 	mov    0x30(%rsp),%r8d
 	mov    %rax,%r9
 	mov    0x28(%rsp),%eax
 	test   %eax,%eax
-	jle    16eeb <sparse_histogram+0x1cb>
+	jle    16eab <sparse_histogram+0x1cb>
 	mov    0x20(%rsp),%rax
 	mov    0x38(%rsp),%rdi
 	mov    0x20(%rsp),%r11
 	mov    0x48(%rsp),%r10
 	movsd  (%rax),%xmm1
 	movslq 0x1c(%rsp),%rax
 	lea    -0x8(%rdi,%rax,8),%rsi
 	mov    0x28(%rsp),%eax
 	mov    0x40(%rsp),%rdi
 	sub    $0x1,%eax
 	cmpl   $0x1,0x18(%rsp)
 	lea    0x8(%rdi,%rax,8),%rdx
-	jne    16f6f <sparse_histogram+0x24f>
+	jne    16f2f <sparse_histogram+0x24f>
 	nopl   (%rax)
 	movsd  (%rdi),%xmm0
 	comisd %xmm0,%xmm1
-	ja     16ee2 <sparse_histogram+0x1c2>
+	ja     16ea2 <sparse_histogram+0x1c2>
 	comisd (%rsi),%xmm0
-	ja     16ee2 <sparse_histogram+0x1c2>
+	ja     16ea2 <sparse_histogram+0x1c2>
 	movapd %xmm0,%xmm2
 	subsd  %xmm1,%xmm2
 	mulsd  0x8(%rsp),%xmm2
 	cvttsd2si %xmm2,%eax
 	cltq
 	cvttsd2si (%r10,%rax,8),%ebx
 	cmp    $0xffffffff,%ebx
-	je     16ee2 <sparse_histogram+0x1c2>
+	je     16ea2 <sparse_histogram+0x1c2>
 	movslq %ebx,%rax
 	subsd  (%r11,%rax,8),%xmm0
 	mulsd  0x10(%rsp),%xmm0
 	cvttsd2si %xmm0,%eax
-	movsd  0x1406(%rip),%xmm0        
+	movsd  0x1446(%rip),%xmm0        
 	add    %ebx,%eax
 	cltq
 	lea    (%r9,%rax,8),%rax
 	addsd  (%rax),%xmm0
 	movsd  %xmm0,(%rax)
 	add    $0x8,%rdi
 	cmp    %rdi,%rdx
-	jne    16e88 <sparse_histogram+0x168>
+	jne    16e48 <sparse_histogram+0x168>
 	test   %ecx,%ecx
-	jle    16f51 <sparse_histogram+0x231>
+	jle    16f11 <sparse_histogram+0x231>
 	mov    0x34(%rsp),%eax
 	xor    %esi,%esi
 	mov    %r13,%rdi
 	mov    %r8d,0x8(%rsp)
 	sub    $0x1,%eax
 	lea    0x8(,%rax,8),%rbx
 	mov    %rbx,%rdx
 	call   30f0 <memset@plt>
 	mov    0x8(%rsp),%r8d
 	xor    %ecx,%ecx
 	lea    -0x1(%r8),%eax
 	lea    0x8(%r12,%rax,8),%rsi
 	test   %r8d,%r8d
-	jle    16f48 <sparse_histogram+0x228>
+	jle    16f08 <sparse_histogram+0x228>
 	mov    %r12,%rax
 	pxor   %xmm0,%xmm0
 	nopl   0x0(%rax)
 	mov    (%rax),%rdx
 	add    $0x8,%rax
 	addsd  (%rdx,%rcx,1),%xmm0
 	cmp    %rsi,%rax
-	jne    16f30 <sparse_histogram+0x210>
+	jne    16ef0 <sparse_histogram+0x210>
 	movsd  %xmm0,0x0(%r13,%rcx,1)
 	add    $0x8,%rcx
 	cmp    %rcx,%rbx
-	jne    16f20 <sparse_histogram+0x200>
+	jne    16ee0 <sparse_histogram+0x200>
 	mov    %rbp,%rdi
 	call   3180 <free@plt>
 	add    $0x58,%rsp
 	mov    %r12,%rdi
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
@@ -19779,57 +19773,57 @@
 	pop    %r14
 	pop    %r15
 	jmp    3180 <free@plt>
 	mov    0x18(%rsp),%ebx
 	nopl   0x0(%rax,%rax,1)
 	movsd  (%rdi),%xmm0
 	comisd %xmm0,%xmm1
-	ja     16fd7 <sparse_histogram+0x2b7>
+	ja     16f97 <sparse_histogram+0x2b7>
 	comisd (%rsi),%xmm0
-	ja     16fd7 <sparse_histogram+0x2b7>
+	ja     16f97 <sparse_histogram+0x2b7>
 	movapd %xmm0,%xmm2
 	subsd  %xmm1,%xmm2
 	mulsd  0x8(%rsp),%xmm2
 	cvttsd2si %xmm2,%eax
 	cltq
 	cvttsd2si (%r10,%rax,8),%eax
 	cmp    $0xffffffff,%eax
-	je     16fd7 <sparse_histogram+0x2b7>
+	je     16f97 <sparse_histogram+0x2b7>
 	movslq %eax,%r14
 	imul   %ebx,%eax
 	subsd  (%r11,%r14,8),%xmm0
 	mulsd  0x10(%rsp),%xmm0
 	cvttsd2si %xmm0,%r14d
-	movsd  0x1312(%rip),%xmm0        
+	movsd  0x1352(%rip),%xmm0        
 	add    %r14d,%eax
 	cltq
 	lea    (%r9,%rax,8),%rax
 	addsd  (%rax),%xmm0
 	movsd  %xmm0,(%rax)
 	add    $0x8,%rdi
 	cmp    %rdx,%rdi
-	jne    16f78 <sparse_histogram+0x258>
-	jmp    16eeb <sparse_histogram+0x1cb>
+	jne    16f38 <sparse_histogram+0x258>
+	jmp    16eab <sparse_histogram+0x1cb>
 	data16 cs nopw 0x0(%rax,%rax,1)
 
-0000000000016ff0 <sparse_histogramf>:
+0000000000016fb0 <sparse_histogramf>:
 sparse_histogramf():
 	push   %r15
 	mov    %r9d,%r15d
 	push   %r14
 	xor    %r14d,%r14d
 	push   %r13
 	mov    %rsi,%r13
 	push   %r12
 	push   %rbp
 	push   %rbx
 	sub    $0x48,%rsp
 	movss  (%rcx),%xmm0
 	subss  (%rdx),%xmm0
-	movss  0x12e1(%rip),%xmm5        
+	movss  0x1321(%rip),%xmm5        
 	mov    0x80(%rsp),%ebx
 	mov    %rdx,0x10(%rsp)
 	mov    0x88(%rsp),%eax
 	mov    %rcx,0x28(%rsp)
 	divss  %xmm0,%xmm5
 	pxor   %xmm0,%xmm0
 	mov    %r8,0x38(%rsp)
@@ -19856,24 +19850,24 @@
 	shl    $0x2,%rdi
 	call   31a0 <malloc@plt>
 	mov    %ebx,0x24(%rsp)
 	movslq %ebx,%rbx
 	mov    %rax,(%r12)
 	mov    %rax,%rbp
 	shl    $0x2,%rbx
-	jmp    170c2 <sparse_histogramf+0xd2>
+	jmp    17082 <sparse_histogramf+0xd2>
 	nopl   0x0(%rax,%rax,1)
 	add    %r15,%rbp
 	add    %rbx,%r15
 	mov    %rbp,(%r12,%r14,8)
 	mov    (%r12),%rbp
 	add    $0x1,%r14
 	call   31c0 <omp_get_max_threads()@plt>
 	cmp    %r14d,%eax
-	jg     170b0 <sparse_histogramf+0xc0>
+	jg     17070 <sparse_histogramf+0xc0>
 	call   3040 <omp_get_thread_num()@plt>
 	movslq %eax,%rbx
 	call   3090 <omp_get_num_threads()@plt>
 	mov    0x8(%rsp),%ecx
 	imul   0xc(%rsp),%ecx
 	xor    %esi,%esi
 	mov    (%r12,%rbx,8),%r9
@@ -19884,84 +19878,84 @@
 	shl    $0x2,%rdx
 	call   30f0 <memset@plt>
 	mov    0x1c(%rsp),%ecx
 	mov    0x20(%rsp),%r8d
 	mov    %rax,%r9
 	mov    0x18(%rsp),%eax
 	test   %eax,%eax
-	jle    171b7 <sparse_histogramf+0x1c7>
+	jle    17177 <sparse_histogramf+0x1c7>
 	mov    0x10(%rsp),%rax
 	mov    0x28(%rsp),%rdi
 	mov    0x10(%rsp),%r11
 	mov    0x38(%rsp),%r10
 	movss  (%rax),%xmm1
 	movslq 0xc(%rsp),%rax
 	lea    -0x4(%rdi,%rax,4),%rsi
 	mov    0x18(%rsp),%eax
 	mov    0x30(%rsp),%rdi
 	sub    $0x1,%eax
 	cmpl   $0x1,0x8(%rsp)
 	lea    0x4(%rdi,%rax,4),%rdx
-	jne    1723f <sparse_histogramf+0x24f>
+	jne    171ff <sparse_histogramf+0x24f>
 	nopl   (%rax)
 	movss  (%rdi),%xmm0
 	comiss %xmm0,%xmm1
-	ja     171ae <sparse_histogramf+0x1be>
+	ja     1716e <sparse_histogramf+0x1be>
 	comiss (%rsi),%xmm0
-	ja     171ae <sparse_histogramf+0x1be>
+	ja     1716e <sparse_histogramf+0x1be>
 	movaps %xmm0,%xmm2
 	subss  %xmm1,%xmm2
 	mulss  (%rsp),%xmm2
 	cvttss2si %xmm2,%eax
 	cltq
 	cvttss2si (%r10,%rax,4),%ebx
 	cmp    $0xffffffff,%ebx
-	je     171ae <sparse_histogramf+0x1be>
+	je     1716e <sparse_histogramf+0x1be>
 	movslq %ebx,%rax
 	subss  (%r11,%rax,4),%xmm0
 	mulss  0x4(%rsp),%xmm0
 	cvttss2si %xmm0,%eax
-	movss  0x115a(%rip),%xmm0        
+	movss  0x119a(%rip),%xmm0        
 	add    %ebx,%eax
 	cltq
 	lea    (%r9,%rax,4),%rax
 	addss  (%rax),%xmm0
 	movss  %xmm0,(%rax)
 	add    $0x4,%rdi
 	cmp    %rdi,%rdx
-	jne    17158 <sparse_histogramf+0x168>
+	jne    17118 <sparse_histogramf+0x168>
 	test   %ecx,%ecx
-	jle    17221 <sparse_histogramf+0x231>
+	jle    171e1 <sparse_histogramf+0x231>
 	mov    0x24(%rsp),%eax
 	xor    %esi,%esi
 	mov    %r13,%rdi
 	mov    %r8d,(%rsp)
 	sub    $0x1,%eax
 	lea    0x4(,%rax,4),%rbx
 	mov    %rbx,%rdx
 	call   30f0 <memset@plt>
 	mov    (%rsp),%r8d
 	xor    %ecx,%ecx
 	lea    -0x1(%r8),%eax
 	lea    0x8(%r12,%rax,8),%rsi
 	nopw   0x0(%rax,%rax,1)
 	test   %r8d,%r8d
-	jle    17218 <sparse_histogramf+0x228>
+	jle    171d8 <sparse_histogramf+0x228>
 	mov    %r12,%rax
 	pxor   %xmm0,%xmm0
 	nopl   0x0(%rax)
 	mov    (%rax),%rdx
 	add    $0x8,%rax
 	addss  (%rdx,%rcx,1),%xmm0
 	cmp    %rsi,%rax
-	jne    17200 <sparse_histogramf+0x210>
+	jne    171c0 <sparse_histogramf+0x210>
 	movss  %xmm0,0x0(%r13,%rcx,1)
 	add    $0x4,%rcx
 	cmp    %rcx,%rbx
-	jne    171f0 <sparse_histogramf+0x200>
+	jne    171b0 <sparse_histogramf+0x200>
 	mov    %rbp,%rdi
 	call   3180 <free@plt>
 	add    $0x48,%rsp
 	mov    %r12,%rdi
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
@@ -19969,33 +19963,33 @@
 	pop    %r14
 	pop    %r15
 	jmp    3180 <free@plt>
 	mov    0x8(%rsp),%ebx
 	nopl   0x0(%rax,%rax,1)
 	movss  (%rdi),%xmm0
 	comiss %xmm0,%xmm1
-	ja     172a3 <sparse_histogramf+0x2b3>
+	ja     17263 <sparse_histogramf+0x2b3>
 	comiss (%rsi),%xmm0
-	ja     172a3 <sparse_histogramf+0x2b3>
+	ja     17263 <sparse_histogramf+0x2b3>
 	movaps %xmm0,%xmm2
 	subss  %xmm1,%xmm2
 	mulss  (%rsp),%xmm2
 	cvttss2si %xmm2,%eax
 	cltq
 	cvttss2si (%r10,%rax,4),%eax
 	cmp    $0xffffffff,%eax
-	je     172a3 <sparse_histogramf+0x2b3>
+	je     17263 <sparse_histogramf+0x2b3>
 	movslq %eax,%r14
 	imul   %ebx,%eax
 	subss  (%r11,%r14,4),%xmm0
 	mulss  0x4(%rsp),%xmm0
 	cvttss2si %xmm0,%r14d
-	movss  0x1066(%rip),%xmm0        
+	movss  0x10a6(%rip),%xmm0        
 	add    %r14d,%eax
 	cltq
 	lea    (%r9,%rax,4),%rax
 	addss  (%rax),%xmm0
 	movss  %xmm0,(%rax)
 	add    $0x4,%rdi
 	cmp    %rdx,%rdi
-	jne    17248 <sparse_histogramf+0x258>
-	jmp    171b7 <sparse_histogramf+0x1c7>
+	jne    17208 <sparse_histogramf+0x258>
+	jmp    17177 <sparse_histogramf+0x1c7>
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.fini {}

```diff
@@ -1,10 +1,10 @@
 
 
 
 Disassembly of section .fini:
 
-00000000000172b4 <_fini>:
+0000000000017274 <_fini>:
 _fini():
 	sub    $0x8,%rsp
 	add    $0x8,%rsp
 	ret
```

#### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,78 +1,78 @@
 
 Hex dump of section '.eh_frame_hdr':
   0x00018480 011b033b ac040000 94000000 a0abfeff ...;............
   0x00018490 c8040000 40aefeff f0040000 50aefeff ....@.......P...
-  0x000184a0 380b0000 6aaefeff a40b0000 84aefeff 8...j...........
-  0x000184b0 8c0c0000 9baefeff f80c0000 b2aefeff ................
-  0x000184c0 101a0000 b7aefeff 701a0000 bcaefeff ........p.......
-  0x000184d0 f41a0000 d0aefeff 100d0000 00affeff ................
-  0x000184e0 601d0000 e0affeff 08050000 b0c5feff `...............
+  0x000184a0 300b0000 6aaefeff 9c0b0000 84aefeff 0...j...........
+  0x000184b0 840c0000 9baefeff f00c0000 b2aefeff ................
+  0x000184c0 081a0000 b7aefeff 681a0000 bcaefeff ........h.......
+  0x000184d0 ec1a0000 d0aefeff 080d0000 00affeff ................
+  0x000184e0 581d0000 e0affeff 08050000 b0c5feff X...............
   0x000184f0 58050000 00dbfeff a8050000 40ebfeff X...........@...
   0x00018500 f8050000 d0fafeff 48060000 9000ffff ........H.......
   0x00018510 5c060000 000effff 88060000 c010ffff \...............
   0x00018520 d8060000 d011ffff 08070000 7016ffff ............p...
-  0x00018530 58070000 0018ffff 98070000 0023ffff X............#..
-  0x00018540 e4070000 5025ffff 30080000 a02fffff ....P%..0..../..
-  0x00018550 80080000 2032ffff d0080000 7033ffff .... 2......p3..
-  0x00018560 fc080000 d034ffff 20090000 d036ffff .....4.. ....6..
-  0x00018570 64090000 f038ffff b40a0000 e042ffff d....8.......B..
-  0x00018580 500b0000 604affff 080c0000 d054ffff P...`J.......T..
-  0x00018590 a40c0000 b05cffff a8090000 705dffff .....\......p]..
-  0x000185a0 f8090000 305effff 480a0000 805fffff ....0^..H...._..
-  0x000185b0 bc0b0000 d060ffff 280d0000 0062ffff .....`..(....b..
-  0x000185c0 800d0000 1063ffff d80d0000 4064ffff .....c......@d..
-  0x000185d0 000e0000 7065ffff 280e0000 4067ffff ....pe..(...@g..
-  0x000185e0 700e0000 0069ffff b80e0000 b06affff p....i.......j..
-  0x000185f0 fc0e0000 706cffff 400f0000 a06cffff ....pl..@....l..
-  0x00018600 540f0000 d06cffff 680f0000 106dffff T....l..h....m..
-  0x00018610 7c0f0000 306fffff 900f0000 5071ffff |...0o......Pq..
-  0x00018620 a40f0000 c074ffff b80f0000 1075ffff .....t.......u..
-  0x00018630 cc0f0000 1076ffff e00f0000 a076ffff .....v.......v..
-  0x00018640 f40f0000 8077ffff 08100000 1078ffff .....w.......x..
-  0x00018650 1c100000 7078ffff 30100000 d078ffff ....px..0....x..
-  0x00018660 44100000 7079ffff 58100000 f079ffff D...py..X....y..
-  0x00018670 6c100000 b07affff 80100000 307bffff l....z......0{..
-  0x00018680 94100000 907bffff a8100000 f07bffff .....{.......{..
-  0x00018690 bc100000 907cffff d0100000 a07effff .....|.......~..
-  0x000186a0 18110000 5081ffff 60110000 1082ffff ....P...`.......
-  0x000186b0 74110000 f082ffff a0110000 a083ffff t...............
-  0x000186c0 b4110000 9084ffff e0110000 d085ffff ................
-  0x000186d0 f4110000 0087ffff 08120000 f087ffff ................
-  0x000186e0 1c120000 d088ffff 30120000 9089ffff ........0.......
-  0x000186f0 44120000 708affff 58120000 d08affff D...p...X.......
-  0x00018700 94120000 308bffff d0120000 908bffff ....0...........
-  0x00018710 0c130000 f08bffff 48130000 508cffff ........H...P...
-  0x00018720 84130000 b08cffff c0130000 b08dffff ................
-  0x00018730 ec130000 b08effff 18140000 b08fffff ................
-  0x00018740 38140000 b090ffff 58140000 6091ffff 8.......X...`...
-  0x00018750 6c140000 2092ffff 80140000 d092ffff l... ...........
-  0x00018760 94140000 a093ffff a8140000 f093ffff ................
-  0x00018770 bc140000 4094ffff d0140000 5095ffff ....@.......P...
-  0x00018780 e4140000 6096ffff f8140000 1097ffff ....`...........
-  0x00018790 0c150000 d097ffff 20150000 009affff ........ .......
-  0x000187a0 34150000 b09affff 48150000 009bffff 4.......H.......
-  0x000187b0 5c150000 509bffff 70150000 409cffff \...P...p...@...
-  0x000187c0 84150000 609dffff 98150000 509effff ....`.......P...
-  0x000187d0 ac150000 f09effff c0150000 809fffff ................
-  0x000187e0 d4150000 40a0ffff e8150000 70a0ffff ....@.......p...
-  0x000187f0 fc150000 00a1ffff 10160000 60a1ffff ............`...
-  0x00018800 24160000 d0a2ffff 38160000 30a3ffff $.......8...0...
-  0x00018810 4c160000 f0a3ffff 60160000 20a4ffff L.......`... ...
-  0x00018820 74160000 c0a4ffff 88160000 20a5ffff t........... ...
-  0x00018830 9c160000 c0a6ffff b0160000 20a7ffff ............ ...
-  0x00018840 08170000 c0aaffff 90170000 40aeffff ............@...
-  0x00018850 1c180000 50b1ffff b0180000 a0b4ffff ....P...........
-  0x00018860 540d0000 d0b5ffff ac0d0000 e0b6ffff T...............
-  0x00018870 ec0d0000 10b8ffff 140e0000 40b9ffff ............@...
-  0x00018880 c4160000 00bbffff 4c170000 b0bcffff ........L.......
-  0x00018890 d4170000 70beffff 68180000 40c0ffff ....p...h...@...
-  0x000188a0 00190000 d0c7ffff 4c190000 d0d2ffff ........L.......
-  0x000188b0 a0190000 50d4ffff 241a0000 90d5ffff ....P...$.......
-  0x000188c0 841a0000 10d7ffff 081b0000 20d7ffff ............ ...
-  0x000188d0 1c1b0000 30d7ffff 301b0000 40d7ffff ....0...0...@...
-  0x000188e0 481b0000 60d7ffff 601b0000 b0d9ffff H...`...`.......
-  0x000188f0 901b0000 70dbffff c41b0000 70ddffff ....p.......p...
-  0x00018900 f81b0000 80ddffff 201c0000 70e2ffff ........ ...p...
-  0x00018910 701c0000 a0e7ffff 0c1c0000 a0e8ffff p...............
-  0x00018920 c01c0000 70ebffff 101d0000          ....p.......
+  0x00018530 58070000 0018ffff 98070000 e022ffff X............"..
+  0x00018540 e4070000 3025ffff 30080000 602fffff ....0%..0...`/..
+  0x00018550 7c080000 e031ffff c8080000 3033ffff |....1......03..
+  0x00018560 f4080000 9034ffff 18090000 9036ffff .....4.......6..
+  0x00018570 5c090000 b038ffff ac0a0000 a042ffff \....8.......B..
+  0x00018580 480b0000 204affff 000c0000 9054ffff H... J.......T..
+  0x00018590 9c0c0000 705cffff a0090000 305dffff ....p\......0]..
+  0x000185a0 f0090000 f05dffff 400a0000 405fffff .....]..@...@_..
+  0x000185b0 b40b0000 9060ffff 200d0000 c061ffff .....`.. ....a..
+  0x000185c0 780d0000 d062ffff d00d0000 0064ffff x....b.......d..
+  0x000185d0 f80d0000 3065ffff 200e0000 0067ffff ....0e.. ....g..
+  0x000185e0 680e0000 c068ffff b00e0000 706affff h....h......pj..
+  0x000185f0 f40e0000 306cffff 380f0000 606cffff ....0l..8...`l..
+  0x00018600 4c0f0000 906cffff 600f0000 d06cffff L....l..`....l..
+  0x00018610 740f0000 f06effff 880f0000 1071ffff t....n.......q..
+  0x00018620 9c0f0000 8074ffff b00f0000 d074ffff .....t.......t..
+  0x00018630 c40f0000 d075ffff d80f0000 6076ffff .....u......`v..
+  0x00018640 ec0f0000 4077ffff 00100000 d077ffff ....@w.......w..
+  0x00018650 14100000 3078ffff 28100000 9078ffff ....0x..(....x..
+  0x00018660 3c100000 3079ffff 50100000 b079ffff <...0y..P....y..
+  0x00018670 64100000 707affff 78100000 f07affff d...pz..x....z..
+  0x00018680 8c100000 507bffff a0100000 b07bffff ....P{.......{..
+  0x00018690 b4100000 507cffff c8100000 607effff ....P|......`~..
+  0x000186a0 10110000 1081ffff 58110000 d081ffff ........X.......
+  0x000186b0 6c110000 b082ffff 98110000 6083ffff l...........`...
+  0x000186c0 ac110000 5084ffff d8110000 9085ffff ....P...........
+  0x000186d0 ec110000 c086ffff 00120000 b087ffff ................
+  0x000186e0 14120000 9088ffff 28120000 5089ffff ........(...P...
+  0x000186f0 3c120000 308affff 50120000 908affff <...0...P.......
+  0x00018700 8c120000 f08affff c8120000 508bffff ............P...
+  0x00018710 04130000 b08bffff 40130000 108cffff ........@.......
+  0x00018720 7c130000 708cffff b8130000 708dffff |...p.......p...
+  0x00018730 e4130000 708effff 10140000 708fffff ....p.......p...
+  0x00018740 30140000 7090ffff 50140000 2091ffff 0...p...P... ...
+  0x00018750 64140000 e091ffff 78140000 9092ffff d.......x.......
+  0x00018760 8c140000 6093ffff a0140000 b093ffff ....`...........
+  0x00018770 b4140000 0094ffff c8140000 1095ffff ................
+  0x00018780 dc140000 2096ffff f0140000 d096ffff .... ...........
+  0x00018790 04150000 9097ffff 18150000 c099ffff ................
+  0x000187a0 2c150000 709affff 40150000 c09affff ,...p...@.......
+  0x000187b0 54150000 109bffff 68150000 009cffff T.......h.......
+  0x000187c0 7c150000 209dffff 90150000 109effff |... ...........
+  0x000187d0 a4150000 b09effff b8150000 409fffff ............@...
+  0x000187e0 cc150000 00a0ffff e0150000 30a0ffff ............0...
+  0x000187f0 f4150000 c0a0ffff 08160000 20a1ffff ............ ...
+  0x00018800 1c160000 90a2ffff 30160000 f0a2ffff ........0.......
+  0x00018810 44160000 b0a3ffff 58160000 e0a3ffff D.......X.......
+  0x00018820 6c160000 80a4ffff 80160000 e0a4ffff l...............
+  0x00018830 94160000 80a6ffff a8160000 e0a6ffff ................
+  0x00018840 00170000 80aaffff 88170000 00aeffff ................
+  0x00018850 14180000 10b1ffff a8180000 60b4ffff ............`...
+  0x00018860 4c0d0000 90b5ffff a40d0000 a0b6ffff L...............
+  0x00018870 e40d0000 d0b7ffff 0c0e0000 00b9ffff ................
+  0x00018880 bc160000 c0baffff 44170000 70bcffff ........D...p...
+  0x00018890 cc170000 30beffff 60180000 00c0ffff ....0...`.......
+  0x000188a0 f8180000 90c7ffff 44190000 90d2ffff ........D.......
+  0x000188b0 98190000 10d4ffff 1c1a0000 50d5ffff ............P...
+  0x000188c0 7c1a0000 d0d6ffff 001b0000 e0d6ffff |...............
+  0x000188d0 141b0000 f0d6ffff 281b0000 00d7ffff ........(.......
+  0x000188e0 401b0000 20d7ffff 581b0000 70d9ffff @... ...X...p...
+  0x000188f0 881b0000 30dbffff bc1b0000 30ddffff ....0.......0...
+  0x00018900 f01b0000 40ddffff 181c0000 30e2ffff ....@.......0...
+  0x00018910 681c0000 60e7ffff 041c0000 60e8ffff h...`.......`...
+  0x00018920 b81c0000 30ebffff 081d0000          ....0.......
```

#### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -43,358 +43,357 @@
   0x00018bb0 86064c0e 38830751 0ef00203 5a030a0e ..L.8..Q....Z...
   0x00018bc0 38440e30 410e2842 0e20420e 18420e10 8D.0A.(B. B..B..
   0x00018bd0 420e0845 0b000000 3c000000 ac020000 B..E....<.......
   0x00018be0 100fffff 8b010000 0002480e 108c0244 ..........H....D
   0x00018bf0 0e188603 410e2083 04032501 0e18410e ....A. ...%...A.
   0x00018c00 10420e08 4bc3c6cc 410e2083 0486038c .B..K...A. .....
   0x00018c10 02000000 00000000 48000000 ec020000 ........H.......
-  0x00018c20 6010ffff f90a0000 004a0e10 8f02490e `........J....I.
+  0x00018c20 6010ffff d60a0000 004a0e10 8f02490e `........J....I.
   0x00018c30 188e0345 0e208d04 420e288c 05410e30 ...E. ..B.(..A.0
-  0x00018c40 8606450e 38830749 0ec00103 be0a0e38 ..E.8..I.......8
+  0x00018c40 8606450e 38830746 0e800103 9e0a0e38 ..E.8..F.......8
   0x00018c50 440e3041 0e28420e 20420e18 420e1042 D.0A.(B. B..B..B
-  0x00018c60 0e080000 48000000 38030000 141bffff ....H...8.......
+  0x00018c60 0e080000 48000000 38030000 f41affff ....H...8.......
   0x00018c70 4d020000 00420e10 8f024d0e 188e0349 M....B....M....I
   0x00018c80 0e208d04 420e288c 05410e30 8606410e . ..B.(..A.0..A.
   0x00018c90 3883074b 0e800103 14020e38 440e3041 8..K.......8D.0A
   0x00018ca0 0e28420e 20420e18 420e1042 0e080000 .(B. B..B..B....
-  0x00018cb0 4c000000 84030000 181dffff 4b0a0000 L...........K...
+  0x00018cb0 48000000 84030000 f81cffff 2b0a0000 H...........+...
   0x00018cc0 00420e10 8f024d0e 188e0345 0e208d04 .B....M....E. ..
   0x00018cd0 420e288c 05410e30 8606410e 3883074e B.(..A.0..A.8..N
-  0x00018ce0 0ea00103 8e090a0e 38410e30 410e2842 ........8A.0A.(B
-  0x00018cf0 0e20420e 18420e10 420e0841 0b000000 . B..B..B..A....
-  0x00018d00 4c000000 d4030000 1827ffff 7d020000 L........'..}...
-  0x00018d10 00420e10 8f024d0e 188e034c 0e208d04 .B....M....L. ..
-  0x00018d20 420e288c 05410e30 8606410e 3883074a B.(..A.0..A.8..J
-  0x00018d30 0e700342 020e3844 0e30410e 28420e20 .p.B..8D.0A.(B. 
-  0x00018d40 420e1842 0e10420e 08000000 00000000 B..B..B.........
-  0x00018d50 28000000 24040000 4829ffff 41010000 (...$...H)..A...
-  0x00018d60 00450e10 86024a0e 18830302 d50a0e10 .E....J.........
-  0x00018d70 410e084b 0b024f0e 10410e08 20000000 A..K..O..A.. ...
-  0x00018d80 50040000 6c2affff 5c010000 00450e10 P...l*..\....E..
-  0x00018d90 830202f3 0a0e0848 0b025b0e 08000000 .......H..[.....
-  0x00018da0 40000000 74040000 a82bffff 00020000 @...t....+......
-  0x00018db0 00540e10 8e02450e 188d0342 0e208c04 .T....E....B. ..
-  0x00018dc0 440e2886 05440e30 830603d4 010e2841 D.(..D.0......(A
-  0x00018dd0 0e20420e 18420e10 420e0841 c3c6cccd . B..B..B..A....
-  0x00018de0 ce000000 40000000 b8040000 642dffff ....@.......d-..
-  0x00018df0 1f020000 00540e10 8e02450e 188d0345 .....T....E....E
-  0x00018e00 0e208c04 410e2886 05440e30 830603f3 . ..A.(..D.0....
-  0x00018e10 010e2841 0e20420e 18420e10 420e0841 ..(A. B..B..B..A
-  0x00018e20 c3c6cccd ce000000 4c000000 fc040000 ........L.......
-  0x00018e30 0053ffff bc000000 004c0e10 8e02420e .S.......L....B.
-  0x00018e40 188d0342 0e208c04 410e2886 05410e30 ...B. ..A.(..A.0
-  0x00018e50 8306600a 0e28410e 20420e18 420e1042 ..`..(A. B..B..B
-  0x00018e60 0e08470b 02440a0e 28410e20 420e1842 ..G..D..(A. B..B
-  0x00018e70 0e10420e 08450b00 4c000000 4c050000 ..B..E..L...L...
-  0x00018e80 7053ffff bc000000 004c0e10 8e02420e pS.......L....B.
-  0x00018e90 188d0342 0e208c04 410e2886 05410e30 ...B. ..A.(..A.0
-  0x00018ea0 8306600a 0e28410e 20420e18 420e1042 ..`..(A. B..B..B
-  0x00018eb0 0e08470b 02450a0e 28410e20 420e1842 ..G..E..(A. B..B
-  0x00018ec0 0e10420e 08440b00 48000000 9c050000 ..B..D..H.......
-  0x00018ed0 e053ffff 48010000 00420e10 8f02420e .S..H....B....B.
-  0x00018ee0 188e0342 0e208d04 420e288c 05410e30 ...B. ..B.(..A.0
-  0x00018ef0 8606410e 3883074e 0e500293 0a0e3841 ..A.8..N.P....8A
-  0x00018f00 0e30410e 28420e20 420e1842 0e10420e .0A.(B. B..B..B.
-  0x00018f10 084b0b00 1c000000 00000000 017a504c .K...........zPL
-  0x00018f20 52000178 10079b41 3200001b 1b0c0708 R..x...A2.......
-  0x00018f30 90010000 50000000 24000000 342effff ....P...$...4...
-  0x00018f40 e2090000 04b31200 00420e10 8f02420e .........B....B.
-  0x00018f50 188e0342 0e208d04 450e288c 05440e30 ...B. ..E.(..D.0
-  0x00018f60 8606470e 38830747 0ee00103 88080a0e ..G.8..G........
-  0x00018f70 38410e30 410e2842 0e20420e 18420e10 8A.0A.(B. B..B..
-  0x00018f80 420e0841 0b000000 2c000000 00000000 B..A....,.......
-  0x00018f90 017a504c 52000178 10079bcd 3100001b .zPLR..x....1...
-  0x00018fa0 1b0c0708 90010ee0 01830786 068c058d ................
-  0x00018fb0 048e038f 02000000 14000000 34000000 ............4...
-  0x00018fc0 10a3feff 1a000000 04381200 00000000 .........8......
-  0x00018fd0 50000000 c0000000 8837ffff 7a070000 P........7..z...
-  0x00018fe0 04281200 00420e10 8f02450e 188e0345 .(...B....E....E
-  0x00018ff0 0e208d04 450e288c 05440e30 8606410e . ..E.(..D.0..A.
-  0x00019000 3883074d 0ee00103 e2050a0e 38410e30 8..M........8A.0
-  0x00019010 410e2842 0e20420e 18420e10 420e0841 A.(B. B..B..B..A
-  0x00019020 0b000000 14000000 a0000000 bea2feff ................
-  0x00019030 1a000000 04dd1100 00000000 48000000 ............H...
-  0x00019040 10070000 bc53ffff 50010000 00420e10 .....S..P....B..
-  0x00019050 8f02420e 188e0342 0e208d04 420e288c ..B....B. ..B.(.
-  0x00019060 05410e30 8606410e 3883074e 0e500292 .A.0..A.8..N.P..
-  0x00019070 0a0e3841 0e30410e 28420e20 420e1842 ..8A.0A.(B. B..B
-  0x00019080 0e10420e 08440b00 50000000 78010000 ..B..D..P...x...
-  0x00019090 503effff 6f0a0000 04811100 00420e10 P>..o........B..
-  0x000190a0 8f02420e 188e0342 0e208d04 450e288c ..B....B. ..E.(.
-  0x000190b0 05440e30 8606470e 38830747 0ec00103 .D.0..G.8..G....
-  0x000190c0 f6080a0e 38410e30 410e2842 0e20420e ....8A.0A.(B. B.
-  0x000190d0 18420e10 420e0843 0b000000 2c000000 .B..B..C....,...
-  0x000190e0 00000000 017a504c 52000178 10079b79 .....zPLR..x...y
-  0x000190f0 3000001b 1b0c0708 90010ec0 01830786 0...............
-  0x00019100 068c058d 048e038f 02000000 14000000 ................
-  0x00019110 34000000 f0a1feff 17000000 04061100 4...............
-  0x00019120 00000000 50000000 14020000 2448ffff ....P.......$H..
-  0x00019130 d2070000 04f61000 00420e10 8f02420e .........B....B.
-  0x00019140 188e0342 0e208d04 450e288c 05440e30 ...B. ..E.(..D.0
-  0x00019150 8606470e 38830747 0ec00103 36060a0e ..G.8..G....6...
-  0x00019160 38410e30 410e2842 0e20420e 18420e10 8A.0A.(B. B..B..
-  0x00019170 420e0843 0b000000 14000000 a0000000 B..C............
-  0x00019180 9ba1feff 17000000 04ab1000 00000000 ................
-  0x00019190 14000000 64080000 b8a1feff 2e000000 ....d...........
-  0x000191a0 00440e10 570e0800 28000000 7c080000 .D..W...(...|...
-  0x000191b0 a053ffff 21010000 00450e10 86024a0e .S..!....E....J.
-  0x000191c0 18830302 b70a0e10 410e0849 0b024f0e ........A..I..O.
-  0x000191d0 10410e08 28000000 a8080000 44a7ffff .A..(.......D...
-  0x000191e0 21010000 00450e10 86024a0e 18830302 !....E....J.....
-  0x000191f0 b70a0e10 410e0849 0b024f0e 10410e08 ....A..I..O..A..
-  0x00019200 28000000 d4080000 7854ffff 09010000 (.......xT......
-  0x00019210 00450e10 86024a0e 18830302 ae0a0e10 .E....J.........
-  0x00019220 410e0842 0b02470e 10410e08 28000000 A..B..G..A..(...
-  0x00019230 00090000 1ca8ffff 09010000 00450e10 .............E..
-  0x00019240 86024a0e 18830302 ae0a0e10 410e0842 ..J.........A..B
-  0x00019250 0b02470e 10410e08 10000000 2c090000 ..G..A......,...
-  0x00019260 3055ffff 28010000 00000000 10000000 0U..(...........
-  0x00019270 40090000 eca8ffff 28010000 00000000 @.......(.......
-  0x00019280 10000000 54090000 3856ffff 28010000 ....T...8V..(...
-  0x00019290 00000000 10000000 68090000 f4a9ffff ........h.......
-  0x000192a0 28010000 00000000 44000000 7c090000 (.......D...|...
-  0x000192b0 4057ffff c3010000 00540e10 8e02480e @W.......T....H.
-  0x000192c0 188d0345 0e208c04 410e2886 05450e30 ...E. ..A.(..E.0
-  0x000192d0 83060377 010a0e28 410e2042 0e18420e ...w...(A. B..B.
-  0x000192e0 10420e08 410b5c0e 08c3c6cc cdce0000 .B..A.\.........
-  0x000192f0 44000000 c4090000 c858ffff b2010000 D........X......
-  0x00019300 00520e10 8e02480e 188d0345 0e208c04 .R....H....E. ..
-  0x00019310 410e2886 05450e30 83060369 010a0e28 A.(..E.0...i...(
-  0x00019320 410e2042 0e18420e 10420e08 410b5b0e A. B..B..B..A.[.
-  0x00019330 08c3c6cc cdce0000 40000000 0c0a0000 ........@.......
-  0x00019340 405affff ab010000 00520e10 8e02450e @Z.......R....E.
-  0x00019350 188d0346 0e208c04 440e2886 05410e30 ...F. ..D.(..A.0
-  0x00019360 83060380 010e2841 0e20420e 18420e10 ......(A. B..B..
-  0x00019370 420e0841 c3c6cccd ce000000 40000000 B..A........@...
-  0x00019380 500a0000 ac5bffff bb010000 00540e10 P....[.......T..
-  0x00019390 8e02450e 188d0346 0e208c04 440e2886 ..E....F. ..D.(.
-  0x000193a0 05410e30 8306038e 010e2841 0e20420e .A.0......(A. B.
-  0x000193b0 18420e10 420e0841 c3c6cccd ce000000 .B..B..A........
-  0x000193c0 10000000 940a0000 285dffff 23000000 ........(]..#...
-  0x000193d0 00000000 10000000 a80a0000 445dffff ............D]..
-  0x000193e0 23000000 00000000 10000000 bc0a0000 #...............
-  0x000193f0 605dffff 33000000 00000000 10000000 `]..3...........
-  0x00019400 d00a0000 8c5dffff 1d020000 00000000 .....]..........
-  0x00019410 10000000 e40a0000 985fffff 11020000 ........._......
-  0x00019420 00000000 10000000 f80a0000 a461ffff .............a..
-  0x00019430 69030000 00000000 10000000 0c0b0000 i...............
-  0x00019440 0065ffff 47000000 00000000 10000000 .e..G...........
-  0x00019450 200b0000 3c65ffff ff000000 00000000  ...<e..........
-  0x00019460 10000000 340b0000 2866ffff 8d000000 ....4...(f......
-  0x00019470 00000000 10000000 480b0000 a466ffff ........H....f..
-  0x00019480 db000000 00000000 10000000 5c0b0000 ............\...
-  0x00019490 7067ffff 8d000000 00000000 10000000 pg..............
-  0x000194a0 700b0000 ec67ffff 55000000 00000000 p....g..U.......
-  0x000194b0 10000000 840b0000 3868ffff 5d000000 ........8h..]...
-  0x000194c0 00000000 10000000 980b0000 8468ffff .............h..
-  0x000194d0 95000000 00000000 10000000 ac0b0000 ................
-  0x000194e0 1069ffff 7d000000 00000000 10000000 .i..}...........
-  0x000194f0 c00b0000 7c69ffff bf000000 00000000 ....|i..........
-  0x00019500 10000000 d40b0000 286affff 7d000000 ........(j..}...
-  0x00019510 00000000 10000000 e80b0000 946affff .............j..
-  0x00019520 55000000 00000000 10000000 fc0b0000 U...............
-  0x00019530 e06affff 5d000000 00000000 10000000 .j..]...........
-  0x00019540 100c0000 2c6bffff 95000000 00000000 ....,k..........
-  0x00019550 44000000 240c0000 b86bffff 0a020000 D...$....k......
-  0x00019560 00420e10 8f02450e 188e0342 0e208d04 .B....E....B. ..
-  0x00019570 420e288c 05440e30 8606410e 38830703 B.(..D.0..A.8...
-  0x00019580 d0010a0e 30410e28 420e2042 0e18420e ....0A.(B. B..B.
-  0x00019590 10420e08 470b0000 44000000 6c0c0000 .B..G...D...l...
-  0x000195a0 806dffff ad020000 00420e10 8f02420e .m.......B....B.
-  0x000195b0 188e0342 0e208d04 470e288c 05410e30 ...B. ..G.(..A.0
-  0x000195c0 8606410e 38830703 6d020a0e 30410e28 ..A.8...m...0A.(
-  0x000195d0 420e2042 0e18420e 10420e08 4b0b0000 B. B..B..B..K...
-  0x000195e0 10000000 b40c0000 e86fffff b9000000 .........o......
-  0x000195f0 00000000 28000000 c80c0000 9470ffff ....(........p..
-  0x00019600 d6000000 00410e10 8602440e 18830346 .....A....D....F
-  0x00019610 0e2002a4 0a0e1845 0e10410e 08530b00 . .....E..A..S..
-  0x00019620 10000000 f40c0000 4871ffff a9000000 ........Hq......
-  0x00019630 00000000 28000000 080d0000 e471ffff ....(........q..
-  0x00019640 ee000000 00410e10 8602440e 18830346 .....A....D....F
-  0x00019650 0e2002c3 0a0e1845 0e10410e 084c0b00 . .....E..A..L..
-  0x00019660 10000000 340d0000 a872ffff 31010000 ....4....r..1...
-  0x00019670 00000000 10000000 480d0000 d473ffff ........H....s..
-  0x00019680 22010000 00000000 10000000 5c0d0000 "...........\...
-  0x00019690 f074ffff ef000000 00000000 10000000 .t..............
-  0x000196a0 700d0000 cc75ffff d8000000 00000000 p....u..........
-  0x000196b0 10000000 840d0000 9876ffff be000000 .........v......
-  0x000196c0 00000000 10000000 980d0000 4477ffff ............Dw..
-  0x000196d0 e0000000 00000000 38000000 ac0d0000 ........8.......
-  0x000196e0 1078ffff 51000000 00460e10 8d02450e .x..Q....F....E.
-  0x000196f0 188c0344 0e208604 440e2883 05460e30 ...D. ..D.(..F.0
-  0x00019700 660e2841 0e20410e 18420e10 420e084b f.(A. A..B..B..K
-  0x00019710 c3c6cccd 38000000 e80d0000 3478ffff ....8.......4x..
-  0x00019720 51000000 00460e10 8d02450e 188c0344 Q....F....E....D
-  0x00019730 0e208604 440e2883 05460e30 660e2841 . ..D.(..F.0f.(A
-  0x00019740 0e20410e 18420e10 420e084b c3c6cccd . A..B..B..K....
-  0x00019750 38000000 240e0000 5878ffff 51000000 8...$...Xx..Q...
-  0x00019760 00460e10 8d02450e 188c0344 0e208604 .F....E....D. ..
-  0x00019770 440e2883 05460e30 660e2841 0e20410e D.(..F.0f.(A. A.
-  0x00019780 18420e10 420e084b c3c6cccd 38000000 .B..B..K....8...
-  0x00019790 600e0000 7c78ffff 51000000 00460e10 `...|x..Q....F..
-  0x000197a0 8d02450e 188c0344 0e208604 440e2883 ..E....D. ..D.(.
-  0x000197b0 05460e30 6e0e2841 0e20410e 18420e10 .F.0n.(A. A..B..
-  0x000197c0 420e0843 c3c6cccd 38000000 9c0e0000 B..C....8.......
-  0x000197d0 a078ffff 51000000 00460e10 8d02450e .x..Q....F....E.
-  0x000197e0 188c0344 0e208604 440e2883 05460e30 ...D. ..D.(..F.0
-  0x000197f0 6e0e2841 0e20410e 18420e10 420e0843 n.(A. A..B..B..C
-  0x00019800 c3c6cccd 38000000 d80e0000 c478ffff ....8........x..
-  0x00019810 51000000 00460e10 8d02450e 188c0344 Q....F....E....D
-  0x00019820 0e208604 440e2883 05460e30 6e0e2841 . ..D.(..F.0n.(A
-  0x00019830 0e20410e 18420e10 420e0843 c3c6cccd . A..B..B..C....
-  0x00019840 28000000 140f0000 e878ffff f2000000 (........x......
-  0x00019850 004c0e10 8602470e 18830302 850a0e10 .L....G.........
-  0x00019860 410e0847 0b02510e 08c3c600 28000000 A..G..Q.....(...
-  0x00019870 400f0000 bc79ffff f2000000 004c0e10 @....y.......L..
-  0x00019880 8602470e 18830302 830a0e10 410e0849 ..G.........A..I
-  0x00019890 0b02510e 08c3c600 1c000000 6c0f0000 ..Q.........l...
-  0x000198a0 907affff f7000000 00410e10 860202d7 .z.......A......
-  0x000198b0 0a0e0848 0b000000 1c000000 8c0f0000 ...H............
-  0x000198c0 707bffff f7000000 00410e10 860202d7 p{.......A......
-  0x000198d0 0a0e0848 0b000000 10000000 ac0f0000 ...H............
-  0x000198e0 507cffff aa000000 00000000 10000000 P|..............
-  0x000198f0 c00f0000 ec7cffff b2000000 00000000 .....|..........
-  0x00019900 10000000 d40f0000 987dffff b0000000 .........}......
-  0x00019910 00000000 10000000 e80f0000 347effff ............4~..
-  0x00019920 c2000000 00000000 10000000 fc0f0000 ................
-  0x00019930 f07effff 4b000000 00000000 10000000 .~..K...........
-  0x00019940 10100000 2c7fffff 4b000000 00000000 ....,...K.......
-  0x00019950 10000000 24100000 687fffff 05010000 ....$...h.......
-  0x00019960 00000000 10000000 38100000 6480ffff ........8...d...
-  0x00019970 05010000 00000000 10000000 4c100000 ............L...
-  0x00019980 6081ffff aa000000 00000000 10000000 `...............
-  0x00019990 60100000 fc81ffff b2000000 00000000 `...............
-  0x000199a0 10000000 74100000 a882ffff 2a020000 ....t.......*...
-  0x000199b0 00000000 10000000 88100000 c484ffff ................
-  0x000199c0 a9000000 00000000 10000000 9c100000 ................
-  0x000199d0 6085ffff 4b000000 00000000 10000000 `...K...........
-  0x000199e0 b0100000 9c85ffff 4b000000 00000000 ........K.......
-  0x000199f0 10000000 c4100000 d885ffff e5000000 ................
-  0x00019a00 00000000 10000000 d8100000 b486ffff ................
-  0x00019a10 15010000 00000000 10000000 ec100000 ................
-  0x00019a20 c087ffff e5000000 00000000 10000000 ................
-  0x00019a30 00110000 9c88ffff 91000000 00000000 ................
-  0x00019a40 10000000 14110000 2889ffff 89000000 ........(.......
-  0x00019a50 00000000 10000000 28110000 a489ffff ........(.......
-  0x00019a60 b5000000 00000000 10000000 3c110000 ............<...
-  0x00019a70 508affff 26000000 00000000 10000000 P...&...........
-  0x00019a80 50110000 6c8affff 8d000000 00000000 P...l...........
-  0x00019a90 10000000 64110000 e88affff 55000000 ....d.......U...
-  0x00019aa0 00000000 10000000 78110000 348bffff ........x...4...
-  0x00019ab0 70010000 00000000 10000000 8c110000 p...............
-  0x00019ac0 908cffff 5c000000 00000000 10000000 ....\...........
-  0x00019ad0 a0110000 dc8cffff b5000000 00000000 ................
-  0x00019ae0 10000000 b4110000 888dffff 27000000 ............'...
-  0x00019af0 00000000 10000000 c8110000 a48dffff ................
-  0x00019b00 95000000 00000000 10000000 dc110000 ................
-  0x00019b10 308effff 5d000000 00000000 10000000 0...]...........
-  0x00019b20 f0110000 7c8effff 98010000 00000000 ....|...........
-  0x00019b30 10000000 04120000 0890ffff 52000000 ............R...
-  0x00019b40 00000000 40000000 18120000 74a2ffff ....@.......t...
-  0x00019b50 bb010000 00540e10 8e02450e 188d0346 .....T....E....F
-  0x00019b60 0e208c04 440e2886 05410e30 8306038e . ..D.(..A.0....
-  0x00019b70 010e2841 0e20420e 18420e10 420e0841 ..(A. B..B..B..A
-  0x00019b80 c3c6cccd ce000000 40000000 5c120000 ........@...\...
-  0x00019b90 1090ffff 9e030000 00420e10 8e02450e .........B....E.
-  0x00019ba0 188d0342 0e208c04 490e2886 05450e30 ...B. ..I.(..E.0
-  0x00019bb0 8306470e 4002da0a 0e30410e 28410e20 ..G.@....0A.(A. 
-  0x00019bc0 420e1842 0e10420e 08480b00 40000000 B..B..B..H..@...
-  0x00019bd0 a0120000 aca3ffff ab010000 00520e10 .............R..
-  0x00019be0 8e02450e 188d0346 0e208c04 440e2886 ..E....F. ..D.(.
-  0x00019bf0 05410e30 83060380 010e2841 0e20420e .A.0......(A. B.
-  0x00019c00 18420e10 420e0841 c3c6cccd ce000000 .B..B..A........
-  0x00019c10 40000000 e4120000 2893ffff 7d030000 @.......(...}...
-  0x00019c20 00420e10 8e02450e 188d0342 0e208c04 .B....E....B. ..
-  0x00019c30 490e2886 05450e30 8306470e 4002c90a I.(..E.0..G.@...
-  0x00019c40 0e30410e 28410e20 420e1842 0e10420e .0A.(A. B..B..B.
-  0x00019c50 08410b00 44000000 28130000 d4a4ffff .A..D...(.......
-  0x00019c60 b2010000 00520e10 8e02480e 188d0345 .....R....H....E
-  0x00019c70 0e208c04 410e2886 05450e30 83060369 . ..A.(..E.0...i
-  0x00019c80 010a0e28 410e2042 0e18420e 10420e08 ...(A. B..B..B..
-  0x00019c90 410b5b0e 08c3c6cc cdce0000 48000000 A.[.........H...
-  0x00019ca0 70130000 1c96ffff 06030000 00420e10 p............B..
-  0x00019cb0 8f02450e 188e0342 0e208d04 4a0e288c ..E....B. ..J.(.
-  0x00019cc0 05450e30 8606410e 38830747 0e4002b2 .E.0..A.8..G.@..
-  0x00019cd0 0a0e3841 0e30410e 28420e20 420e1842 ..8A.0A.(B. B..B
-  0x00019ce0 0e10420e 08440b00 44000000 bc130000 ..B..D..D.......
-  0x00019cf0 00a6ffff c3010000 00540e10 8e02480e .........T....H.
-  0x00019d00 188d0345 0e208c04 410e2886 05450e30 ...E. ..A.(..E.0
-  0x00019d10 83060377 010a0e28 410e2042 0e18420e ...w...(A. B..B.
-  0x00019d20 10420e08 410b5c0e 08c3c6cc cdce0000 .B..A.\.........
-  0x00019d30 4c000000 04140000 9898ffff 42030000 L...........B...
-  0x00019d40 00420e10 8f02450e 188e0342 0e208d04 .B....E....B. ..
-  0x00019d50 4a0e288c 05450e30 8606410e 38830747 J.(..E.0..A.8..G
-  0x00019d60 0e4002bc 0a0e3841 0e30410e 28420e20 .@....8A.0A.(B. 
-  0x00019d70 420e1842 0e10420e 084a0b00 00000000 B..B..B..J......
-  0x00019d80 48000000 54140000 38a7ffff 8c070000 H...T...8.......
-  0x00019d90 00420e10 8f02420e 188e0342 0e208d04 .B....B....B. ..
-  0x00019da0 420e288c 05410e30 8606410e 38830744 B.(..A.0..A.8..D
-  0x00019db0 0e680324 070a0e38 410e3041 0e28420e .h.$...8A.0A.(B.
-  0x00019dc0 20420e18 420e1042 0e08410b 50000000  B..B..B..A.P...
-  0x00019dd0 a0140000 7caeffff f40a0000 00420e10 ....|........B..
-  0x00019de0 8f02420e 188e0342 0e208d04 420e288c ..B....B. ..B.(.
-  0x00019df0 05410e30 8606410e 38830747 0ea80203 .A.0..A.8..G....
-  0x00019e00 730a0a0e 38410e30 410e2842 0e20420e s...8A.0A.(B. B.
-  0x00019e10 18420e10 420e0841 0b000000 00000000 .B..B..A........
-  0x00019e20 48000000 f4140000 28b9ffff 7e010000 H.......(...~...
-  0x00019e30 004c0e10 8f02420e 188e0342 0e208d04 .L....B....B. ..
-  0x00019e40 420e288c 05410e30 8606410e 38830747 B.(..A.0..A.8..G
-  0x00019e50 0e700354 010e3841 0e30450e 28420e20 .p.T..8A.0E.(B. 
-  0x00019e60 420e1842 0e10420e 08000000 20000000 B..B..B..... ...
-  0x00019e70 00000000 017a5200 01781001 1b0c0708 .....zR..x......
-  0x00019e80 90010e70 83078606 8c058d04 8e038f02 ...p............
-  0x00019e90 10000000 28000000 9a94feff 05000000 ....(...........
-  0x00019ea0 00000000 48000000 78150000 24baffff ....H...x...$...
-  0x00019eb0 34010000 004c0e10 8f02420e 188e0342 4....L....B....B
-  0x00019ec0 0e208d04 450e288c 05410e30 8606410e . ..E.(..A.0..A.
-  0x00019ed0 38830744 0e70030a 010e3841 0e30450e 8..D.p....8A.0E.
-  0x00019ee0 28420e20 420e1842 0e10420e 08000000 (B. B..B..B.....
-  0x00019ef0 10000000 88000000 3f94feff 05000000 ........?.......
-  0x00019f00 00000000 48000000 d8150000 04bbffff ....H...........
-  0x00019f10 79010000 004c0e10 8f02420e 188e0342 y....L....B....B
-  0x00019f20 0e208d04 420e288c 05410e30 8606410e . ..B.(..A.0..A.
-  0x00019f30 38830747 0e600350 010e3841 0e30440e 8..G.`.P..8A.0D.
-  0x00019f40 28420e20 420e1842 0e10420e 08000000 (B. B..B..B.....
-  0x00019f50 20000000 00000000 017a5200 01781001  ........zR..x..
-  0x00019f60 1b0c0708 90010e60 83078606 8c058d04 .......`........
-  0x00019f70 8e038f02 10000000 28000000 c093feff ........(.......
-  0x00019f80 05000000 00000000 10000000 5c160000 ............\...
-  0x00019f90 00bcffff 06000000 00000000 10000000 ................
-  0x00019fa0 70160000 fcbbffff 06000000 00000000 p...............
-  0x00019fb0 14000000 84160000 f8bbffff 03000000 ................
-  0x00019fc0 00000000 00000000 14000000 9c160000 ................
-  0x00019fd0 f0bbffff 1e000000 00440e10 590e0800 .........D..Y...
-  0x00019fe0 2c000000 b4160000 f8bbffff 4f020000 ,...........O...
-  0x00019ff0 00410e10 8602430d 06428f03 478e048d .A....C..B..G...
-  0x0001a000 05478c06 4f830703 e1010a0c 0708440b .G..O.........D.
-  0x0001a010 30000000 e4160000 18beffff c0010000 0...............
-  0x0001a020 006d0e10 8602480e 18830303 79010a0e .m....H.....y...
-  0x0001a030 10410e08 410b440e 08c3c641 0e188303 .A..A.D....A....
-  0x0001a040 86020000 30000000 18170000 a4bfffff ....0...........
-  0x0001a050 fa010000 00700e10 86024b0e 18830303 .....p....K.....
-  0x0001a060 a4010a0e 10410e08 410b440e 08c3c641 .....A..A.D....A
-  0x0001a070 0e188303 86020000 10000000 4c170000 ............L...
-  0x0001a080 70c1ffff 0e000000 00000000 10000000 p...............
-  0x0001a090 60170000 8ccbffff 00010000 00000000 `...............
-  0x0001a0a0 4c000000 74170000 58c1ffff e6040000 L...t...X.......
-  0x0001a0b0 00420e10 8f02460e 188e0342 0e208d04 .B....F....B. ..
-  0x0001a0c0 420e288c 05410e30 8606410e 38830744 B.(..A.0..A.8..D
-  0x0001a0d0 0e900103 4d040a0e 38410e30 410e2842 ....M...8A.0A.(B
-  0x0001a0e0 0e20420e 18420e10 420e0841 0b000000 . B..B..B..A....
-  0x0001a0f0 4c000000 c4170000 f8c5ffff 28050000 L...........(...
-  0x0001a100 004d0e10 8f02460e 188e034a 0e208d04 .M....F....J. ..
-  0x0001a110 460e288c 05490e30 8606410e 38830744 F.(..I.0..A.8..D
-  0x0001a120 0e900103 6e040a0e 38410e30 410e2842 ....n...8A.0A.(B
-  0x0001a130 0e20420e 18420e10 420e0841 0b000000 . B..B..B..A....
-  0x0001a140 4c000000 14180000 d8cbffff c5020000 L...............
-  0x0001a150 00420e10 8f02450e 188e0345 0e208d04 .B....E....E. ..
-  0x0001a160 450e288c 05410e30 8606410e 38830744 E.(..A.0..A.8..D
-  0x0001a170 0e900103 26020a0e 38440e30 410e2842 ....&...8D.0A.(B
-  0x0001a180 0e20420e 18420e10 420e0845 0b000000 . B..B..B..E....
-  0x0001a190 4c000000 64180000 58ceffff c1020000 L...d...X.......
-  0x0001a1a0 00420e10 8f02450e 188e0345 0e208d04 .B....E....E. ..
-  0x0001a1b0 450e288c 05410e30 8606410e 38830744 E.(..A.0..A.8..D
-  0x0001a1c0 0e800103 26020a0e 38440e30 410e2842 ....&...8D.0A.(B
-  0x0001a1d0 0e20420e 18420e10 420e0845 0b000000 . B..B..B..E....
-  0x0001a1e0 10000000 b4180000 9891feff 13000000 ................
-  0x0001a1f0 00000000 00000000                   ........
+  0x00018ce0 0e60036e 090a0e38 410e3041 0e28420e .`.n...8A.0A.(B.
+  0x00018cf0 20420e18 420e1042 0e08410b 48000000  B..B..B..A.H...
+  0x00018d00 d0030000 dc26ffff 7d020000 00420e10 .....&..}....B..
+  0x00018d10 8f024d0e 188e034c 0e208d04 420e288c ..M....L. ..B.(.
+  0x00018d20 05410e30 8606410e 3883074a 0e700342 .A.0..A.8..J.p.B
+  0x00018d30 020e3844 0e30410e 28420e20 420e1842 ..8D.0A.(B. B..B
+  0x00018d40 0e10420e 08000000 28000000 1c040000 ..B.....(.......
+  0x00018d50 1029ffff 41010000 00450e10 86024a0e .)..A....E....J.
+  0x00018d60 18830302 d50a0e10 410e084b 0b024f0e ........A..K..O.
+  0x00018d70 10410e08 20000000 48040000 342affff .A.. ...H...4*..
+  0x00018d80 5c010000 00450e10 830202f3 0a0e0848 \....E.........H
+  0x00018d90 0b025b0e 08000000 40000000 6c040000 ..[.....@...l...
+  0x00018da0 702bffff 00020000 00540e10 8e02450e p+.......T....E.
+  0x00018db0 188d0342 0e208c04 440e2886 05440e30 ...B. ..D.(..D.0
+  0x00018dc0 830603d4 010e2841 0e20420e 18420e10 ......(A. B..B..
+  0x00018dd0 420e0841 c3c6cccd ce000000 40000000 B..A........@...
+  0x00018de0 b0040000 2c2dffff 1f020000 00540e10 ....,-.......T..
+  0x00018df0 8e02450e 188d0345 0e208c04 410e2886 ..E....E. ..A.(.
+  0x00018e00 05440e30 830603f3 010e2841 0e20420e .D.0......(A. B.
+  0x00018e10 18420e10 420e0841 c3c6cccd ce000000 .B..B..A........
+  0x00018e20 4c000000 f4040000 c852ffff bc000000 L........R......
+  0x00018e30 004c0e10 8e02420e 188d0342 0e208c04 .L....B....B. ..
+  0x00018e40 410e2886 05410e30 8306600a 0e28410e A.(..A.0..`..(A.
+  0x00018e50 20420e18 420e1042 0e08470b 02440a0e  B..B..B..G..D..
+  0x00018e60 28410e20 420e1842 0e10420e 08450b00 (A. B..B..B..E..
+  0x00018e70 4c000000 44050000 3853ffff bc000000 L...D...8S......
+  0x00018e80 004c0e10 8e02420e 188d0342 0e208c04 .L....B....B. ..
+  0x00018e90 410e2886 05410e30 8306600a 0e28410e A.(..A.0..`..(A.
+  0x00018ea0 20420e18 420e1042 0e08470b 02450a0e  B..B..B..G..E..
+  0x00018eb0 28410e20 420e1842 0e10420e 08440b00 (A. B..B..B..D..
+  0x00018ec0 48000000 94050000 a853ffff 48010000 H........S..H...
+  0x00018ed0 00420e10 8f02420e 188e0342 0e208d04 .B....B....B. ..
+  0x00018ee0 420e288c 05410e30 8606410e 3883074e B.(..A.0..A.8..N
+  0x00018ef0 0e500293 0a0e3841 0e30410e 28420e20 .P....8A.0A.(B. 
+  0x00018f00 420e1842 0e10420e 084b0b00 1c000000 B..B..B..K......
+  0x00018f10 00000000 017a504c 52000178 10079b49 .....zPLR..x...I
+  0x00018f20 3200001b 1b0c0708 90010000 50000000 2...........P...
+  0x00018f30 24000000 fc2dffff e2090000 04b31200 $....-..........
+  0x00018f40 00420e10 8f02420e 188e0342 0e208d04 .B....B....B. ..
+  0x00018f50 450e288c 05440e30 8606470e 38830747 E.(..D.0..G.8..G
+  0x00018f60 0ee00103 88080a0e 38410e30 410e2842 ........8A.0A.(B
+  0x00018f70 0e20420e 18420e10 420e0841 0b000000 . B..B..B..A....
+  0x00018f80 2c000000 00000000 017a504c 52000178 ,........zPLR..x
+  0x00018f90 10079bd5 3100001b 1b0c0708 90010ee0 ....1...........
+  0x00018fa0 01830786 068c058d 048e038f 02000000 ................
+  0x00018fb0 14000000 34000000 18a3feff 1a000000 ....4...........
+  0x00018fc0 04381200 00000000 50000000 c0000000 .8......P.......
+  0x00018fd0 5037ffff 7a070000 04281200 00420e10 P7..z....(...B..
+  0x00018fe0 8f02450e 188e0345 0e208d04 450e288c ..E....E. ..E.(.
+  0x00018ff0 05440e30 8606410e 3883074d 0ee00103 .D.0..A.8..M....
+  0x00019000 e2050a0e 38410e30 410e2842 0e20420e ....8A.0A.(B. B.
+  0x00019010 18420e10 420e0841 0b000000 14000000 .B..B..A........
+  0x00019020 a0000000 c6a2feff 1a000000 04dd1100 ................
+  0x00019030 00000000 48000000 08070000 8453ffff ....H........S..
+  0x00019040 50010000 00420e10 8f02420e 188e0342 P....B....B....B
+  0x00019050 0e208d04 420e288c 05410e30 8606410e . ..B.(..A.0..A.
+  0x00019060 3883074e 0e500292 0a0e3841 0e30410e 8..N.P....8A.0A.
+  0x00019070 28420e20 420e1842 0e10420e 08440b00 (B. B..B..B..D..
+  0x00019080 50000000 78010000 183effff 6f0a0000 P...x....>..o...
+  0x00019090 04811100 00420e10 8f02420e 188e0342 .....B....B....B
+  0x000190a0 0e208d04 450e288c 05440e30 8606470e . ..E.(..D.0..G.
+  0x000190b0 38830747 0ec00103 f6080a0e 38410e30 8..G........8A.0
+  0x000190c0 410e2842 0e20420e 18420e10 420e0843 A.(B. B..B..B..C
+  0x000190d0 0b000000 2c000000 00000000 017a504c ....,........zPL
+  0x000190e0 52000178 10079b81 3000001b 1b0c0708 R..x....0.......
+  0x000190f0 90010ec0 01830786 068c058d 048e038f ................
+  0x00019100 02000000 14000000 34000000 f8a1feff ........4.......
+  0x00019110 17000000 04061100 00000000 50000000 ............P...
+  0x00019120 14020000 ec47ffff d2070000 04f61000 .....G..........
+  0x00019130 00420e10 8f02420e 188e0342 0e208d04 .B....B....B. ..
+  0x00019140 450e288c 05440e30 8606470e 38830747 E.(..D.0..G.8..G
+  0x00019150 0ec00103 36060a0e 38410e30 410e2842 ....6...8A.0A.(B
+  0x00019160 0e20420e 18420e10 420e0843 0b000000 . B..B..B..C....
+  0x00019170 14000000 a0000000 a3a1feff 17000000 ................
+  0x00019180 04ab1000 00000000 14000000 5c080000 ............\...
+  0x00019190 c0a1feff 2e000000 00440e10 570e0800 .........D..W...
+  0x000191a0 28000000 74080000 6853ffff 21010000 (...t...hS..!...
+  0x000191b0 00450e10 86024a0e 18830302 b70a0e10 .E....J.........
+  0x000191c0 410e0849 0b024f0e 10410e08 28000000 A..I..O..A..(...
+  0x000191d0 a0080000 0ca7ffff 21010000 00450e10 ........!....E..
+  0x000191e0 86024a0e 18830302 b70a0e10 410e0849 ..J.........A..I
+  0x000191f0 0b024f0e 10410e08 28000000 cc080000 ..O..A..(.......
+  0x00019200 4054ffff 09010000 00450e10 86024a0e @T.......E....J.
+  0x00019210 18830302 ae0a0e10 410e0842 0b02470e ........A..B..G.
+  0x00019220 10410e08 28000000 f8080000 e4a7ffff .A..(...........
+  0x00019230 09010000 00450e10 86024a0e 18830302 .....E....J.....
+  0x00019240 ae0a0e10 410e0842 0b02470e 10410e08 ....A..B..G..A..
+  0x00019250 10000000 24090000 f854ffff 28010000 ....$....T..(...
+  0x00019260 00000000 10000000 38090000 b4a8ffff ........8.......
+  0x00019270 28010000 00000000 10000000 4c090000 (...........L...
+  0x00019280 0056ffff 28010000 00000000 10000000 .V..(...........
+  0x00019290 60090000 bca9ffff 28010000 00000000 `.......(.......
+  0x000192a0 44000000 74090000 0857ffff c3010000 D...t....W......
+  0x000192b0 00540e10 8e02480e 188d0345 0e208c04 .T....H....E. ..
+  0x000192c0 410e2886 05450e30 83060377 010a0e28 A.(..E.0...w...(
+  0x000192d0 410e2042 0e18420e 10420e08 410b5c0e A. B..B..B..A.\.
+  0x000192e0 08c3c6cc cdce0000 44000000 bc090000 ........D.......
+  0x000192f0 9058ffff b2010000 00520e10 8e02480e .X.......R....H.
+  0x00019300 188d0345 0e208c04 410e2886 05450e30 ...E. ..A.(..E.0
+  0x00019310 83060369 010a0e28 410e2042 0e18420e ...i...(A. B..B.
+  0x00019320 10420e08 410b5b0e 08c3c6cc cdce0000 .B..A.[.........
+  0x00019330 40000000 040a0000 085affff ab010000 @........Z......
+  0x00019340 00520e10 8e02450e 188d0346 0e208c04 .R....E....F. ..
+  0x00019350 440e2886 05410e30 83060380 010e2841 D.(..A.0......(A
+  0x00019360 0e20420e 18420e10 420e0841 c3c6cccd . B..B..B..A....
+  0x00019370 ce000000 40000000 480a0000 745bffff ....@...H...t[..
+  0x00019380 bb010000 00540e10 8e02450e 188d0346 .....T....E....F
+  0x00019390 0e208c04 440e2886 05410e30 8306038e . ..D.(..A.0....
+  0x000193a0 010e2841 0e20420e 18420e10 420e0841 ..(A. B..B..B..A
+  0x000193b0 c3c6cccd ce000000 10000000 8c0a0000 ................
+  0x000193c0 f05cffff 23000000 00000000 10000000 .\..#...........
+  0x000193d0 a00a0000 0c5dffff 23000000 00000000 .....]..#.......
+  0x000193e0 10000000 b40a0000 285dffff 33000000 ........(]..3...
+  0x000193f0 00000000 10000000 c80a0000 545dffff ............T]..
+  0x00019400 1d020000 00000000 10000000 dc0a0000 ................
+  0x00019410 605fffff 11020000 00000000 10000000 `_..............
+  0x00019420 f00a0000 6c61ffff 69030000 00000000 ....la..i.......
+  0x00019430 10000000 040b0000 c864ffff 47000000 .........d..G...
+  0x00019440 00000000 10000000 180b0000 0465ffff .............e..
+  0x00019450 ff000000 00000000 10000000 2c0b0000 ............,...
+  0x00019460 f065ffff 8d000000 00000000 10000000 .e..............
+  0x00019470 400b0000 6c66ffff db000000 00000000 @...lf..........
+  0x00019480 10000000 540b0000 3867ffff 8d000000 ....T...8g......
+  0x00019490 00000000 10000000 680b0000 b467ffff ........h....g..
+  0x000194a0 55000000 00000000 10000000 7c0b0000 U...........|...
+  0x000194b0 0068ffff 5d000000 00000000 10000000 .h..]...........
+  0x000194c0 900b0000 4c68ffff 95000000 00000000 ....Lh..........
+  0x000194d0 10000000 a40b0000 d868ffff 7d000000 .........h..}...
+  0x000194e0 00000000 10000000 b80b0000 4469ffff ............Di..
+  0x000194f0 bf000000 00000000 10000000 cc0b0000 ................
+  0x00019500 f069ffff 7d000000 00000000 10000000 .i..}...........
+  0x00019510 e00b0000 5c6affff 55000000 00000000 ....\j..U.......
+  0x00019520 10000000 f40b0000 a86affff 5d000000 .........j..]...
+  0x00019530 00000000 10000000 080c0000 f46affff .............j..
+  0x00019540 95000000 00000000 44000000 1c0c0000 ........D.......
+  0x00019550 806bffff 0a020000 00420e10 8f02450e .k.......B....E.
+  0x00019560 188e0342 0e208d04 420e288c 05440e30 ...B. ..B.(..D.0
+  0x00019570 8606410e 38830703 d0010a0e 30410e28 ..A.8.......0A.(
+  0x00019580 420e2042 0e18420e 10420e08 470b0000 B. B..B..B..G...
+  0x00019590 44000000 640c0000 486dffff ad020000 D...d...Hm......
+  0x000195a0 00420e10 8f02420e 188e0342 0e208d04 .B....B....B. ..
+  0x000195b0 470e288c 05410e30 8606410e 38830703 G.(..A.0..A.8...
+  0x000195c0 6d020a0e 30410e28 420e2042 0e18420e m...0A.(B. B..B.
+  0x000195d0 10420e08 4b0b0000 10000000 ac0c0000 .B..K...........
+  0x000195e0 b06fffff b9000000 00000000 28000000 .o..........(...
+  0x000195f0 c00c0000 5c70ffff d6000000 00410e10 ....\p.......A..
+  0x00019600 8602440e 18830346 0e2002a4 0a0e1845 ..D....F. .....E
+  0x00019610 0e10410e 08530b00 10000000 ec0c0000 ..A..S..........
+  0x00019620 1071ffff a9000000 00000000 28000000 .q..........(...
+  0x00019630 000d0000 ac71ffff ee000000 00410e10 .....q.......A..
+  0x00019640 8602440e 18830346 0e2002c3 0a0e1845 ..D....F. .....E
+  0x00019650 0e10410e 084c0b00 10000000 2c0d0000 ..A..L......,...
+  0x00019660 7072ffff 31010000 00000000 10000000 pr..1...........
+  0x00019670 400d0000 9c73ffff 22010000 00000000 @....s..".......
+  0x00019680 10000000 540d0000 b874ffff ef000000 ....T....t......
+  0x00019690 00000000 10000000 680d0000 9475ffff ........h....u..
+  0x000196a0 d8000000 00000000 10000000 7c0d0000 ............|...
+  0x000196b0 6076ffff be000000 00000000 10000000 `v..............
+  0x000196c0 900d0000 0c77ffff e0000000 00000000 .....w..........
+  0x000196d0 38000000 a40d0000 d877ffff 51000000 8........w..Q...
+  0x000196e0 00460e10 8d02450e 188c0344 0e208604 .F....E....D. ..
+  0x000196f0 440e2883 05460e30 660e2841 0e20410e D.(..F.0f.(A. A.
+  0x00019700 18420e10 420e084b c3c6cccd 38000000 .B..B..K....8...
+  0x00019710 e00d0000 fc77ffff 51000000 00460e10 .....w..Q....F..
+  0x00019720 8d02450e 188c0344 0e208604 440e2883 ..E....D. ..D.(.
+  0x00019730 05460e30 660e2841 0e20410e 18420e10 .F.0f.(A. A..B..
+  0x00019740 420e084b c3c6cccd 38000000 1c0e0000 B..K....8.......
+  0x00019750 2078ffff 51000000 00460e10 8d02450e  x..Q....F....E.
+  0x00019760 188c0344 0e208604 440e2883 05460e30 ...D. ..D.(..F.0
+  0x00019770 660e2841 0e20410e 18420e10 420e084b f.(A. A..B..B..K
+  0x00019780 c3c6cccd 38000000 580e0000 4478ffff ....8...X...Dx..
+  0x00019790 51000000 00460e10 8d02450e 188c0344 Q....F....E....D
+  0x000197a0 0e208604 440e2883 05460e30 6e0e2841 . ..D.(..F.0n.(A
+  0x000197b0 0e20410e 18420e10 420e0843 c3c6cccd . A..B..B..C....
+  0x000197c0 38000000 940e0000 6878ffff 51000000 8.......hx..Q...
+  0x000197d0 00460e10 8d02450e 188c0344 0e208604 .F....E....D. ..
+  0x000197e0 440e2883 05460e30 6e0e2841 0e20410e D.(..F.0n.(A. A.
+  0x000197f0 18420e10 420e0843 c3c6cccd 38000000 .B..B..C....8...
+  0x00019800 d00e0000 8c78ffff 51000000 00460e10 .....x..Q....F..
+  0x00019810 8d02450e 188c0344 0e208604 440e2883 ..E....D. ..D.(.
+  0x00019820 05460e30 6e0e2841 0e20410e 18420e10 .F.0n.(A. A..B..
+  0x00019830 420e0843 c3c6cccd 28000000 0c0f0000 B..C....(.......
+  0x00019840 b078ffff f2000000 004c0e10 8602470e .x.......L....G.
+  0x00019850 18830302 850a0e10 410e0847 0b02510e ........A..G..Q.
+  0x00019860 08c3c600 28000000 380f0000 8479ffff ....(...8....y..
+  0x00019870 f2000000 004c0e10 8602470e 18830302 .....L....G.....
+  0x00019880 830a0e10 410e0849 0b02510e 08c3c600 ....A..I..Q.....
+  0x00019890 1c000000 640f0000 587affff f7000000 ....d...Xz......
+  0x000198a0 00410e10 860202d7 0a0e0848 0b000000 .A.........H....
+  0x000198b0 1c000000 840f0000 387bffff f7000000 ........8{......
+  0x000198c0 00410e10 860202d7 0a0e0848 0b000000 .A.........H....
+  0x000198d0 10000000 a40f0000 187cffff aa000000 .........|......
+  0x000198e0 00000000 10000000 b80f0000 b47cffff .............|..
+  0x000198f0 b2000000 00000000 10000000 cc0f0000 ................
+  0x00019900 607dffff b0000000 00000000 10000000 `}..............
+  0x00019910 e00f0000 fc7dffff c2000000 00000000 .....}..........
+  0x00019920 10000000 f40f0000 b87effff 4b000000 .........~..K...
+  0x00019930 00000000 10000000 08100000 f47effff .............~..
+  0x00019940 4b000000 00000000 10000000 1c100000 K...............
+  0x00019950 307fffff 05010000 00000000 10000000 0...............
+  0x00019960 30100000 2c80ffff 05010000 00000000 0...,...........
+  0x00019970 10000000 44100000 2881ffff aa000000 ....D...(.......
+  0x00019980 00000000 10000000 58100000 c481ffff ........X.......
+  0x00019990 b2000000 00000000 10000000 6c100000 ............l...
+  0x000199a0 7082ffff 2a020000 00000000 10000000 p...*...........
+  0x000199b0 80100000 8c84ffff a9000000 00000000 ................
+  0x000199c0 10000000 94100000 2885ffff 4b000000 ........(...K...
+  0x000199d0 00000000 10000000 a8100000 6485ffff ............d...
+  0x000199e0 4b000000 00000000 10000000 bc100000 K...............
+  0x000199f0 a085ffff e5000000 00000000 10000000 ................
+  0x00019a00 d0100000 7c86ffff 15010000 00000000 ....|...........
+  0x00019a10 10000000 e4100000 8887ffff e5000000 ................
+  0x00019a20 00000000 10000000 f8100000 6488ffff ............d...
+  0x00019a30 91000000 00000000 10000000 0c110000 ................
+  0x00019a40 f088ffff 89000000 00000000 10000000 ................
+  0x00019a50 20110000 6c89ffff b5000000 00000000  ...l...........
+  0x00019a60 10000000 34110000 188affff 26000000 ....4.......&...
+  0x00019a70 00000000 10000000 48110000 348affff ........H...4...
+  0x00019a80 8d000000 00000000 10000000 5c110000 ............\...
+  0x00019a90 b08affff 55000000 00000000 10000000 ....U...........
+  0x00019aa0 70110000 fc8affff 70010000 00000000 p.......p.......
+  0x00019ab0 10000000 84110000 588cffff 5c000000 ........X...\...
+  0x00019ac0 00000000 10000000 98110000 a48cffff ................
+  0x00019ad0 b5000000 00000000 10000000 ac110000 ................
+  0x00019ae0 508dffff 27000000 00000000 10000000 P...'...........
+  0x00019af0 c0110000 6c8dffff 95000000 00000000 ....l...........
+  0x00019b00 10000000 d4110000 f88dffff 5d000000 ............]...
+  0x00019b10 00000000 10000000 e8110000 448effff ............D...
+  0x00019b20 98010000 00000000 10000000 fc110000 ................
+  0x00019b30 d08fffff 52000000 00000000 40000000 ....R.......@...
+  0x00019b40 10120000 3ca2ffff bb010000 00540e10 ....<........T..
+  0x00019b50 8e02450e 188d0346 0e208c04 440e2886 ..E....F. ..D.(.
+  0x00019b60 05410e30 8306038e 010e2841 0e20420e .A.0......(A. B.
+  0x00019b70 18420e10 420e0841 c3c6cccd ce000000 .B..B..A........
+  0x00019b80 40000000 54120000 d88fffff 9e030000 @...T...........
+  0x00019b90 00420e10 8e02450e 188d0342 0e208c04 .B....E....B. ..
+  0x00019ba0 490e2886 05450e30 8306470e 4002da0a I.(..E.0..G.@...
+  0x00019bb0 0e30410e 28410e20 420e1842 0e10420e .0A.(A. B..B..B.
+  0x00019bc0 08480b00 40000000 98120000 74a3ffff .H..@.......t...
+  0x00019bd0 ab010000 00520e10 8e02450e 188d0346 .....R....E....F
+  0x00019be0 0e208c04 440e2886 05410e30 83060380 . ..D.(..A.0....
+  0x00019bf0 010e2841 0e20420e 18420e10 420e0841 ..(A. B..B..B..A
+  0x00019c00 c3c6cccd ce000000 40000000 dc120000 ........@.......
+  0x00019c10 f092ffff 7d030000 00420e10 8e02450e ....}....B....E.
+  0x00019c20 188d0342 0e208c04 490e2886 05450e30 ...B. ..I.(..E.0
+  0x00019c30 8306470e 4002c90a 0e30410e 28410e20 ..G.@....0A.(A. 
+  0x00019c40 420e1842 0e10420e 08410b00 44000000 B..B..B..A..D...
+  0x00019c50 20130000 9ca4ffff b2010000 00520e10  ............R..
+  0x00019c60 8e02480e 188d0345 0e208c04 410e2886 ..H....E. ..A.(.
+  0x00019c70 05450e30 83060369 010a0e28 410e2042 .E.0...i...(A. B
+  0x00019c80 0e18420e 10420e08 410b5b0e 08c3c6cc ..B..B..A.[.....
+  0x00019c90 cdce0000 48000000 68130000 e495ffff ....H...h.......
+  0x00019ca0 06030000 00420e10 8f02450e 188e0342 .....B....E....B
+  0x00019cb0 0e208d04 4a0e288c 05450e30 8606410e . ..J.(..E.0..A.
+  0x00019cc0 38830747 0e4002b2 0a0e3841 0e30410e 8..G.@....8A.0A.
+  0x00019cd0 28420e20 420e1842 0e10420e 08440b00 (B. B..B..B..D..
+  0x00019ce0 44000000 b4130000 c8a5ffff c3010000 D...............
+  0x00019cf0 00540e10 8e02480e 188d0345 0e208c04 .T....H....E. ..
+  0x00019d00 410e2886 05450e30 83060377 010a0e28 A.(..E.0...w...(
+  0x00019d10 410e2042 0e18420e 10420e08 410b5c0e A. B..B..B..A.\.
+  0x00019d20 08c3c6cc cdce0000 4c000000 fc130000 ........L.......
+  0x00019d30 6098ffff 42030000 00420e10 8f02450e `...B....B....E.
+  0x00019d40 188e0342 0e208d04 4a0e288c 05450e30 ...B. ..J.(..E.0
+  0x00019d50 8606410e 38830747 0e4002bc 0a0e3841 ..A.8..G.@....8A
+  0x00019d60 0e30410e 28420e20 420e1842 0e10420e .0A.(B. B..B..B.
+  0x00019d70 084a0b00 00000000 48000000 4c140000 .J......H...L...
+  0x00019d80 00a7ffff 8c070000 00420e10 8f02420e .........B....B.
+  0x00019d90 188e0342 0e208d04 420e288c 05410e30 ...B. ..B.(..A.0
+  0x00019da0 8606410e 38830744 0e680324 070a0e38 ..A.8..D.h.$...8
+  0x00019db0 410e3041 0e28420e 20420e18 420e1042 A.0A.(B. B..B..B
+  0x00019dc0 0e08410b 50000000 98140000 44aeffff ..A.P.......D...
+  0x00019dd0 f40a0000 00420e10 8f02420e 188e0342 .....B....B....B
+  0x00019de0 0e208d04 420e288c 05410e30 8606410e . ..B.(..A.0..A.
+  0x00019df0 38830747 0ea80203 730a0a0e 38410e30 8..G....s...8A.0
+  0x00019e00 410e2842 0e20420e 18420e10 420e0841 A.(B. B..B..B..A
+  0x00019e10 0b000000 00000000 48000000 ec140000 ........H.......
+  0x00019e20 f0b8ffff 7e010000 004c0e10 8f02420e ....~....L....B.
+  0x00019e30 188e0342 0e208d04 420e288c 05410e30 ...B. ..B.(..A.0
+  0x00019e40 8606410e 38830747 0e700354 010e3841 ..A.8..G.p.T..8A
+  0x00019e50 0e30450e 28420e20 420e1842 0e10420e .0E.(B. B..B..B.
+  0x00019e60 08000000 20000000 00000000 017a5200 .... ........zR.
+  0x00019e70 01781001 1b0c0708 90010e70 83078606 .x.........p....
+  0x00019e80 8c058d04 8e038f02 10000000 28000000 ............(...
+  0x00019e90 a294feff 05000000 00000000 48000000 ............H...
+  0x00019ea0 70150000 ecb9ffff 34010000 004c0e10 p.......4....L..
+  0x00019eb0 8f02420e 188e0342 0e208d04 450e288c ..B....B. ..E.(.
+  0x00019ec0 05410e30 8606410e 38830744 0e70030a .A.0..A.8..D.p..
+  0x00019ed0 010e3841 0e30450e 28420e20 420e1842 ..8A.0E.(B. B..B
+  0x00019ee0 0e10420e 08000000 10000000 88000000 ..B.............
+  0x00019ef0 4794feff 05000000 00000000 48000000 G...........H...
+  0x00019f00 d0150000 ccbaffff 79010000 004c0e10 ........y....L..
+  0x00019f10 8f02420e 188e0342 0e208d04 420e288c ..B....B. ..B.(.
+  0x00019f20 05410e30 8606410e 38830747 0e600350 .A.0..A.8..G.`.P
+  0x00019f30 010e3841 0e30440e 28420e20 420e1842 ..8A.0D.(B. B..B
+  0x00019f40 0e10420e 08000000 20000000 00000000 ..B..... .......
+  0x00019f50 017a5200 01781001 1b0c0708 90010e60 .zR..x.........`
+  0x00019f60 83078606 8c058d04 8e038f02 10000000 ................
+  0x00019f70 28000000 c893feff 05000000 00000000 (...............
+  0x00019f80 10000000 54160000 c8bbffff 06000000 ....T...........
+  0x00019f90 00000000 10000000 68160000 c4bbffff ........h.......
+  0x00019fa0 06000000 00000000 14000000 7c160000 ............|...
+  0x00019fb0 c0bbffff 03000000 00000000 00000000 ................
+  0x00019fc0 14000000 94160000 b8bbffff 1e000000 ................
+  0x00019fd0 00440e10 590e0800 2c000000 ac160000 .D..Y...,.......
+  0x00019fe0 c0bbffff 4f020000 00410e10 8602430d ....O....A....C.
+  0x00019ff0 06428f03 478e048d 05478c06 4f830703 .B..G....G..O...
+  0x0001a000 e1010a0c 0708440b 30000000 dc160000 ......D.0.......
+  0x0001a010 e0bdffff c0010000 006d0e10 8602480e .........m....H.
+  0x0001a020 18830303 79010a0e 10410e08 410b440e ....y....A..A.D.
+  0x0001a030 08c3c641 0e188303 86020000 30000000 ...A........0...
+  0x0001a040 10170000 6cbfffff fa010000 00700e10 ....l........p..
+  0x0001a050 86024b0e 18830303 a4010a0e 10410e08 ..K..........A..
+  0x0001a060 410b440e 08c3c641 0e188303 86020000 A.D....A........
+  0x0001a070 10000000 44170000 38c1ffff 0e000000 ....D...8.......
+  0x0001a080 00000000 10000000 58170000 54cbffff ........X...T...
+  0x0001a090 00010000 00000000 4c000000 6c170000 ........L...l...
+  0x0001a0a0 20c1ffff e6040000 00420e10 8f02460e  ........B....F.
+  0x0001a0b0 188e0342 0e208d04 420e288c 05410e30 ...B. ..B.(..A.0
+  0x0001a0c0 8606410e 38830744 0e900103 4d040a0e ..A.8..D....M...
+  0x0001a0d0 38410e30 410e2842 0e20420e 18420e10 8A.0A.(B. B..B..
+  0x0001a0e0 420e0841 0b000000 4c000000 bc170000 B..A....L.......
+  0x0001a0f0 c0c5ffff 28050000 004d0e10 8f02460e ....(....M....F.
+  0x0001a100 188e034a 0e208d04 460e288c 05490e30 ...J. ..F.(..I.0
+  0x0001a110 8606410e 38830744 0e900103 6e040a0e ..A.8..D....n...
+  0x0001a120 38410e30 410e2842 0e20420e 18420e10 8A.0A.(B. B..B..
+  0x0001a130 420e0841 0b000000 4c000000 0c180000 B..A....L.......
+  0x0001a140 a0cbffff c5020000 00420e10 8f02450e .........B....E.
+  0x0001a150 188e0345 0e208d04 450e288c 05410e30 ...E. ..E.(..A.0
+  0x0001a160 8606410e 38830744 0e900103 26020a0e ..A.8..D....&...
+  0x0001a170 38440e30 410e2842 0e20420e 18420e10 8D.0A.(B. B..B..
+  0x0001a180 420e0845 0b000000 4c000000 5c180000 B..E....L...\...
+  0x0001a190 20ceffff c1020000 00420e10 8f02450e  ........B....E.
+  0x0001a1a0 188e0345 0e208d04 450e288c 05410e30 ...E. ..E.(..A.0
+  0x0001a1b0 8606410e 38830744 0e800103 26020a0e ..A.8..D....&...
+  0x0001a1c0 38440e30 410e2842 0e20420e 18420e10 8D.0A.(B. B..B..
+  0x0001a1d0 420e0845 0b000000 10000000 ac180000 B..E............
+  0x0001a1e0 a091feff 13000000 00000000 00000000 ................
```

#### readelf --wide --decompress --hex-dump=.gcc_except_table {}

```diff
@@ -1,8 +1,8 @@
 
 Hex dump of section '.gcc_except_table':
-  0x0001a1f8 ffff0105 7968da13 00ffff01 04150500 ....yh..........
-  0x0001a208 00ffff01 057e6cf2 0e00ffff 01041505 .....~l.........
-  0x0001a218 0000ffff 01057068 e71400ff ff010412 ......ph........
-  0x0001a228 050000ff ff010570 68ca0f00 ffff0104 .......ph.......
-  0x0001a238 12050000                            ....
+  0x0001a1f0 ffff0105 7968da13 00ffff01 04150500 ....yh..........
+  0x0001a200 00ffff01 057e6cf2 0e00ffff 01041505 .....~l.........
+  0x0001a210 0000ffff 01057068 e71400ff ff010412 ......ph........
+  0x0001a220 050000ff ff010570 68ca0f00 ffff0104 .......ph.......
+  0x0001a230 12050000                            ....
```

### Comparing `blond-2.1.1/blond/cpp_routines/linear_interp_kick.cpp` & `blond-2.1.2/blond/cpp_routines/linear_interp_kick.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/cpp_routines/music_track.cpp` & `blond-2.1.2/blond/cpp_routines/music_track.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/cpp_routines/sin.h` & `blond-2.1.2/blond/cpp_routines/sin.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/cpp_routines/sincos.h` & `blond-2.1.2/blond/cpp_routines/sincos.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/cpp_routines/vdtcore_common.h` & `blond-2.1.2/blond/cpp_routines/vdtcore_common.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/gpu/cuda_kernels/kernels_double.cu` & `blond-2.1.2/blond/gpu/cuda_kernels/kernels_double.cu`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/gpu/cuda_kernels/kernels_single.cu` & `blond-2.1.2/blond/gpu/cuda_kernels/kernels_single.cu`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/gpu/cupy_butils_wrap.py` & `blond-2.1.2/blond/gpu/cupy_butils_wrap.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/impedances/impedance.py` & `blond-2.1.2/blond/impedances/impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/impedances/impedance_sources.py` & `blond-2.1.2/blond/impedances/impedance_sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,21 +545,21 @@
 
         Z(f) = \frac{Z_0 c L}{ \pi } \frac{ 1 }{ \left[1 - i \text{sign} f \right] 2  b  c
                                     \sqrt{ \frac{\sigma_c Z_0 c }{ 4 \pi |f| } + i 2 \pi b^2 f } }
 
     Parameters
     ----------
     pipe_radius : float
-        Beam pipe radius in m
+        Beam pipe radius in m 
     pipe_length : float
-        Beam pipe length in m
+        Beam pipe length in m 
     resistivity : float
-        Beam pipe resistivity in :math:`m / s`
+        Beam pipe resistivity in :math:`m / s` 
     conductivity : float
-        Beam pipe conductivity in :math:`s / m`
+        Beam pipe conductivity in :math:`s / m` 
 
     Attributes
     ----------
     pipe_radius : float
         Beam pipe radius in m
     pipe_length : float
         Beam pipe length in m
```

### Comparing `blond-2.1.1/blond/impedances/induced_voltage_analytical.py` & `blond-2.1.2/blond/impedances/induced_voltage_analytical.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,16 +60,15 @@
     launch:
 
     .. code-block:: mathematica
     
         output2 = Integrate[wake * lambda, t]
         outputreal2 = Simplify[ComplexExpand[Re[output2]],
                                {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in Reals, t > 0}]
-        d/dt output2;
-        Simplify[ComplexExpand[Re[%]],
+        Simplify[ComplexExpand[Re[d/dt output2]],
                  {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in Reals, t > 0}]
     
 
     and check that applying the fundamental calculus theorem to outputreal2, 
     one obtains back outputreal; the formula [5] in 
     
     H. E. Salzer, "Formulas for Calculating the Error Function of a Complex
```

### Comparing `blond-2.1.1/blond/impedances/music.py` & `blond-2.1.2/blond/impedances/music.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/input_parameters/rf_parameters.py` & `blond-2.1.2/blond/input_parameters/rf_parameters.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/input_parameters/rf_parameters_options.py` & `blond-2.1.2/blond/input_parameters/rf_parameters_options.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/input_parameters/ring.py` & `blond-2.1.2/blond/input_parameters/ring.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/input_parameters/ring_options.py` & `blond-2.1.2/blond/input_parameters/ring_options.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/llrf/beam_feedback.py` & `blond-2.1.2/blond/llrf/beam_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/llrf/cavity_feedback.py` & `blond-2.1.2/blond/llrf/cavity_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/llrf/impulse_response.py` & `blond-2.1.2/blond/llrf/impulse_response.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/llrf/notch_filter.py` & `blond-2.1.2/blond/llrf/notch_filter.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/llrf/offset_frequency.py` & `blond-2.1.2/blond/llrf/offset_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/llrf/rf_modulation.py` & `blond-2.1.2/blond/llrf/rf_modulation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/llrf/rf_noise.py` & `blond-2.1.2/blond/llrf/rf_noise.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/llrf/signal_processing.py` & `blond-2.1.2/blond/llrf/signal_processing.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/monitors/monitors.py` & `blond-2.1.2/blond/monitors/monitors.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/plots/plot.py` & `blond-2.1.2/blond/plots/plot.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/plots/plot_beams.py` & `blond-2.1.2/blond/plots/plot_beams.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/plots/plot_impedance.py` & `blond-2.1.2/blond/plots/plot_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/plots/plot_llrf.py` & `blond-2.1.2/blond/plots/plot_llrf.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/plots/plot_parameters.py` & `blond-2.1.2/blond/plots/plot_parameters.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/plots/plot_slices.py` & `blond-2.1.2/blond/plots/plot_slices.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/sanity_check.py` & `blond-2.1.2/blond/sanity_check.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/synchrotron_radiation/synchrotron_radiation.cpp` & `blond-2.1.2/blond/synchrotron_radiation/synchrotron_radiation.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/synchrotron_radiation/synchrotron_radiation.py` & `blond-2.1.2/blond/synchrotron_radiation/synchrotron_radiation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/toolbox/action.py` & `blond-2.1.2/blond/toolbox/action.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/toolbox/diffusion.py` & `blond-2.1.2/blond/toolbox/diffusion.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/toolbox/filters_and_fitting.py` & `blond-2.1.2/blond/toolbox/filters_and_fitting.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
 '''
 **Fitting and filters routines to be used alone or with the Profile class in
-    the beam package. **
+the beam package.**
 
 :Authors: **Danilo Quartullo**, **Alexandre Lasheen**,
           **Juan F. Esteban Mueller**
 '''
 
 import numpy as np
 from scipy.signal import cheb2ord, cheby2, filtfilt, freqz
```

### Comparing `blond-2.1.1/blond/toolbox/logger.py` & `blond-2.1.2/blond/toolbox/logger.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/toolbox/next_regular.py` & `blond-2.1.2/blond/toolbox/next_regular.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/toolbox/parameter_scaling.py` & `blond-2.1.2/blond/toolbox/parameter_scaling.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/toolbox/tomoscope.cpp` & `blond-2.1.2/blond/toolbox/tomoscope.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/toolbox/tomoscope.py` & `blond-2.1.2/blond/toolbox/tomoscope.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/trackers/tracker.py` & `blond-2.1.2/blond/trackers/tracker.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/trackers/utilities.py` & `blond-2.1.2/blond/trackers/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+# coding: utf8
 # Copyright 2016 CERN. This software is distributed under the
 # terms of the GNU General Public Licence version 3 (GPL Version 3),
 # copied verbatim in the file LICENCE.md.
 # In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
@@ -279,15 +279,15 @@
 
     def frequency_calculation(self, n_sampling=100000, start_turn=None, end_turn=None):
         '''
         *Method to compute the fft of the particle oscillations in theta and dE
         to obtain their synchrotron frequencies. The particles for which
         the amplitude of oscillations is extending the minimum and maximum
         theta from user input are considered to be lost and their synchrotron
-        frequencies are not calculated.
+        frequencies are not calculated.*
         '''
 
         n_sampling = int(n_sampling)
 
         #: *Saving the synchrotron frequency from the theta oscillations for each particle*
         self.frequency_theta_save = np.zeros(int(self.n_macroparticles))
```

### Comparing `blond-2.1.1/blond/utils/bmath.py` & `blond-2.1.2/blond/utils/bmath.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/utils/butils_wrap.py` & `blond-2.1.2/blond/utils/butils_wrap.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/utils/data_check.py` & `blond-2.1.2/blond/utils/data_check.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/utils/exceptions.py` & `blond-2.1.2/blond/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/utils/input_parser.py` & `blond-2.1.2/blond/utils/input_parser.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/utils/mpi_config.py` & `blond-2.1.2/blond/utils/mpi_config.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/utils/profile_mock.py` & `blond-2.1.2/blond/utils/profile_mock.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/blond/utils/track_iteration.py` & `blond-2.1.2/blond/utils/track_iteration.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         for i in range(n_turns):
             next(self)
 
 
     def add_function(self, predicate, repetionRate, *args, **kwargs):
         '''
         Takes a user defined callable and calls it every repetionRate
-        number of turns with predicate(trackMap, turnNumber, *args, **kwargs)
+        number of turns with predicate(trackMap, turnNumber, ``*args``, ``**kwargs``)
         '''
         
         self.functionList.append((self._partial(predicate, args, kwargs)
                                   , repetionRate))
         
 
     def __next__(self):
```

### Comparing `blond-2.1.1/blond.egg-info/PKG-INFO` & `blond-2.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,10 @@
-Metadata-Version: 2.1
-Name: blond
-Version: 2.1.1
-Summary: CERN code for simulating longitudinal beam dynamics in synchrotrons.
-Home-page: https://gitlab.cern.ch/blond/BLonD
-Author: Helga Timko et al.
-Author-email: helga.timko@cern.ch
-Maintainer: Konstantinos Iliakis
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: core
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: doc
-Provides-Extra: all
-License-File: LICENSE.txt
+[![Pipeline Status](https://gitlab.cern.ch/blond/BLonD/badges/master/pipeline.svg)](https://gitlab.cern.ch/blond/BLonD/-/commits/master) [![Coverage Report](https://gitlab.cern.ch/blond/BLonD/badges/master/coverage.svg)](https://gitlab.cern.ch/blond/BLonD/-/commits/master) [![Latest Release](https://gitlab.cern.ch/blond/BLonD/-/badges/release.svg)](https://gitlab.cern.ch/blond/BLonD/-/releases) [![PyPi](https://img.shields.io/pypi/v/blond.svg)](https://pypi.org/project/blond/) [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org) [![Documentation Pages](https://img.shields.io/badge/docs-sphinx-blue)](https://blond-code.docs.cern.ch/)
 
-# Code Name
-
-BLonD (Beam Longitudinal Dynamics)
+# Beam Longitudinal Dynamics Code (BLonD)
 
 # Copyright Notice
 
 *Copyright 2019 CERN. This software is distributed under the terms of the
 GNU General Public Licence version 3 (GPL Version 3), copied verbatim in
 the file LICENCE.txt. In applying this licence, CERN does not waive the
 privileges and immunities granted to it by virtue of its status as an
@@ -36,17 +13,17 @@
 # Description
 
 CERN code for the simulation of longitudinal beam dynamics in
 synchrotrons.
 
 # Useful Links
 
-Repository: <https://github.com/blond-admin/BLonD>
+Repository: <https://gitlab.cern.ch/blond/BLonD>
 
-Documentation: <http://blond-admin.github.io/BLonD/>
+Documentation: <https://blond-code.docs.cern.ch/>
 
 Project website: <http://blond.web.cern.ch>
 
 # Install
 
 ## Requirements
```

### Comparing `blond-2.1.1/blond.egg-info/SOURCES.txt` & `blond-2.1.2/blond.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 __doc/modules/llrf.rst
 __doc/modules/monitors.rst
 __doc/modules/plots.rst
 __doc/modules/ring_and_RFstation.gle
 __doc/modules/ring_and_RFstation.png
 __doc/modules/sample.dat
 __doc/modules/sample2.dat
+__doc/modules/sanity_check.rst
 __doc/modules/sps_cavity_loop.rst
 __doc/modules/synchrotron_radiation.rst
 __doc/modules/toolbox.rst
 __doc/modules/trackers.rst
 __doc/modules/utils.rst
 __doc/themes/sphinx_rtd_theme/__init__.py
 __doc/themes/sphinx_rtd_theme/breadcrumbs.html
```

### Comparing `blond-2.1.1/setup.py` & `blond-2.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,79 +29,91 @@
         'pytest',
     ],
     'dev': [
         # 'requirement-for-development-purposes-only',
     ],
     'doc': [
         'sphinx',
-        'acc-py-sphinx',
+        'sphinx-rtd-theme',
+        'sphinxcontrib-napoleon',
+        'sphinx-autopackagesummary',
+        'pyqt5',
     ],
 }
 
 
 class Compile_and_Egg_Info(_egg_info):
     description = 'Compile the C++ sources before installing'
     user_options = _egg_info.user_options
     user_options += [
         ('parallel', 'p', 'Enable Multi-threaded code'),
         ('compiler=', 'c', 'Specify the compiler type'),
+        ('gpu=', None, 'Compile the CUDA backend'),
         ('boost=', None, 'Compile with the Boost Library')]
 
     def initialize_options(self):
         _egg_info.initialize_options(self)
         self.parallel = None
         self.boost = None
         self.compiler = None
+        self.gpu = None
 
     def finalize_options(self):
         """Post-process options."""
         _egg_info.finalize_options(self)
 
     def run(self):
         cmd = ['python3', 'blond/compile.py']
         if self.parallel:
             cmd.append('-p')
         if self.boost:
             cmd += ['-b', self.boost]
         if self.compiler:
             cmd += ['-c', self.compiler]
+        if self.gpu:
+            cmd += ['-gpu', self.gpu]
 
         subprocess.run(cmd, check=True, env=os.environ.copy())
                 # self.run_command('compile')
         return _egg_info.run(self)
 
 class CompileLibrary(distutils.cmd.Command):
     """Compile all C/C++ source files."""
 
     description = 'Compile the shared libraries. Use blond/compile.py for advanced options.'
     user_options = [
         ('parallel', 'p', 'Enable Multi-threaded code'),
         ('compiler=', 'c', 'Specify the compiler type'),
+        ('gpu=', None, 'Compile the CUDA backend'),
         ('boost=', None, 'Compile with the Boost Library')]
 
     def initialize_options(self):
         """Set default values for options."""
         # Each user option must be listed here with their default value.
         self.openmp = None
         self.boost = None
         self.compiler = None
+        self.gpu = None
 
     def finalize_options(self):
         """Post-process options."""
         pass
 
     def run(self):
         """Run command."""
         cmd = ['python3', 'blond/compile.py']
         if self.openmp:
             cmd.append('-p')
         if self.boost:
             cmd += ['-b', self.boost]
         if self.compiler:
             cmd += ['-c', self.compiler]
+        if self.gpu:
+            cmd += ['-gpu', self.gpu]
+
         subprocess.run(cmd, check=True, env=os.environ.copy())
 
 
 setup(
     name='blond',
     # version=__version__,
     description='CERN code for simulating longitudinal beam dynamics in synchrotrons.',
```

### Comparing `blond-2.1.1/unittests/beam_profile/dt_coordinates.npz` & `blond-2.1.2/unittests/beam_profile/dt_coordinates.npz`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/beam_profile/test_beam_profile_object.py` & `blond-2.1.2/unittests/beam_profile/test_beam_profile_object.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/beam_profile/test_sparse_profile.py` & `blond-2.1.2/unittests/beam_profile/test_sparse_profile.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/beams/test_beam_object.py` & `blond-2.1.2/unittests/beams/test_beam_object.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/beams/test_coasting_beam.py` & `blond-2.1.2/unittests/beams/test_coasting_beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/general/test_separatrix_bigaussian.py` & `blond-2.1.2/unittests/general/test_separatrix_bigaussian.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/gpu/test_ffts.py` & `blond-2.1.2/unittests/gpu/test_ffts.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/gpu/test_impedance.py` & `blond-2.1.2/unittests/gpu/test_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/gpu/test_physics_kernels.py` & `blond-2.1.2/unittests/gpu/test_physics_kernels.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/impedances/test_impedance.py` & `blond-2.1.2/unittests/impedances/test_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/impedances/test_impedance_sources.py` & `blond-2.1.2/unittests/impedances/test_impedance_sources.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/input_parameters/test_preprocess.py` & `blond-2.1.2/unittests/input_parameters/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/input_parameters/test_rf_params_object.py` & `blond-2.1.2/unittests/input_parameters/test_rf_params_object.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/input_parameters/test_ring.py` & `blond-2.1.2/unittests/input_parameters/test_ring.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/integration/test_examples.py` & `blond-2.1.2/unittests/integration/test_examples.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/integration/test_gpu_examples.py` & `blond-2.1.2/unittests/integration/test_gpu_examples.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/integration/test_mpi_examples.py` & `blond-2.1.2/unittests/integration/test_mpi_examples.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/integration/test_validate_gpu.py` & `blond-2.1.2/unittests/integration/test_validate_gpu.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/integration/test_validate_mpi.py` & `blond-2.1.2/unittests/integration/test_validate_mpi.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/llrf/ref_DV_MOD_FR.npy` & `blond-2.1.2/unittests/llrf/ref_DV_MOD_FR.npy`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/llrf/ref_DV_MOD_FRF.npy` & `blond-2.1.2/unittests/llrf/ref_DV_MOD_FRF.npy`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/llrf/ref_V_IND_COARSE_GEN.npy` & `blond-2.1.2/unittests/llrf/ref_V_IND_COARSE_GEN.npy`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/llrf/test_beam_feedback.py` & `blond-2.1.2/unittests/llrf/test_beam_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/llrf/test_cavity_feedback.py` & `blond-2.1.2/unittests/llrf/test_cavity_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/llrf/test_impulse_response.py` & `blond-2.1.2/unittests/llrf/test_impulse_response.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/llrf/test_offset_frequency.py` & `blond-2.1.2/unittests/llrf/test_offset_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/llrf/test_rf_modulation.py` & `blond-2.1.2/unittests/llrf/test_rf_modulation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/llrf/test_signal_processing.py` & `blond-2.1.2/unittests/llrf/test_signal_processing.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/synchrotron_radiation/test_synch_rad.py` & `blond-2.1.2/unittests/synchrotron_radiation/test_synch_rad.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/trackers/comparison_drift.py` & `blond-2.1.2/unittests/trackers/comparison_drift.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/trackers/test_drift.py` & `blond-2.1.2/unittests/trackers/test_drift.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/trackers/test_tracker.py` & `blond-2.1.2/unittests/trackers/test_tracker.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/utils/test_blondmath.py` & `blond-2.1.2/unittests/utils/test_blondmath.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/utils/test_data_check.py` & `blond-2.1.2/unittests/utils/test_data_check.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/utils/test_ffts.py` & `blond-2.1.2/unittests/utils/test_ffts.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.1/unittests/utils/test_iteration.py` & `blond-2.1.2/unittests/utils/test_iteration.py`

 * *Files identical despite different names*

