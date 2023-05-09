# Comparing `tmp/pyasd-0.0.4.tar.gz` & `tmp/pyasd-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyasd-0.0.4.tar", last modified: Wed May  3 11:06:49 2023, max compression
+gzip compressed data, was "pyasd-0.0.5.tar", last modified: Tue May  9 02:33:46 2023, max compression
```

## Comparing `pyasd-0.0.4.tar` & `pyasd-0.0.5.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.759330 pyasd-0.0.4/
--rw-r--r--   0 zsh       (1000) zsh       (1000)     1468 2023-01-05 06:57:53.000000 pyasd-0.0.4/LICENSE
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      488 2023-01-06 02:20:47.000000 pyasd-0.0.4/MANIFEST.in
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      425 2023-05-03 11:06:49.759330 pyasd-0.0.4/PKG-INFO
--rw-r--r--   0 zsh       (1000) zsh       (1000)     1350 2023-04-26 14:54:49.000000 pyasd-0.0.4/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.711331 pyasd-0.0.4/asd/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      311 2023-05-03 11:06:49.000000 pyasd-0.0.4/asd/__init__.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.719330 pyasd-0.0.4/asd/core/
--rw-r--r--   0 zsh       (1000) zsh       (1000)        0 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/__init__.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      537 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/constants.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      902 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/dipolar_interactions.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    14970 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/geometry.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    34800 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/gneb.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    28461 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/hamiltonian.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13407 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/llg_advanced.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    34609 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/llg_simple.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6394 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/log_general.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    35175 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/monte_carlo.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7330 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/random_vectors.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    28028 2023-05-01 09:54:36.000000 pyasd-0.0.4/asd/core/shell_exchange.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    20217 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/spin_configurations.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13692 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/spin_correlations.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4455 2023-05-01 09:00:05.000000 pyasd-0.0.4/asd/core/topological_charge.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.719330 pyasd-0.0.4/asd/data_base/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4160 2022-11-27 16:42:32.000000 pyasd-0.0.4/asd/data_base/exchange_for_Cr2I3X3.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1657 2022-11-03 04:08:41.000000 pyasd-0.0.4/asd/data_base/exchange_for_CrI3.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3216 2022-10-04 07:38:22.000000 pyasd-0.0.4/asd/data_base/exchange_for_CrMnI6_U2.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6933 2022-11-17 08:49:56.000000 pyasd-0.0.4/asd/data_base/exchange_for_CrMnI6_U4.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3873 2023-01-05 11:41:58.000000 pyasd-0.0.4/asd/data_base/exchange_for_CrMnI6_rect.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1295 2022-11-14 15:25:58.000000 pyasd-0.0.4/asd/data_base/exchange_for_Gd2C.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4390 2022-12-24 03:07:21.000000 pyasd-0.0.4/asd/data_base/exchange_for_MnI2.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2594 2022-12-24 03:07:20.000000 pyasd-0.0.4/asd/data_base/exchange_for_NiI2.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5909 2022-11-14 15:08:43.000000 pyasd-0.0.4/asd/data_base/exchange_for_RuCl3.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2188 2022-02-21 08:35:16.000000 pyasd-0.0.4/asd/data_base/exchange_for_VOI2.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1468 2022-11-27 16:26:00.000000 pyasd-0.0.4/asd/data_base/exchange_for_kagome.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1066 2022-02-21 07:00:49.000000 pyasd-0.0.4/asd/data_base/exchange_for_skx.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.719330 pyasd-0.0.4/asd/mpi/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2556 2022-11-26 03:52:08.000000 pyasd-0.0.4/asd/mpi/mpi_tools.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.731330 pyasd-0.0.4/asd/utility/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12245 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/Swq.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)        0 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/__init__.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     8824 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/analyze_Spirit_results.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9225 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/asd_arguments.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    55462 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/auxiliary_colormaps.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     2143 2023-02-03 13:19:28.000000 pyasd-0.0.4/asd/utility/curve_fit.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5328 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/four_state_tools.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1880 2023-04-17 02:00:31.000000 pyasd-0.0.4/asd/utility/head_figlet.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6688 2023-02-07 02:54:27.000000 pyasd-0.0.4/asd/utility/mag_thermal.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     7606 2023-02-08 03:42:14.000000 pyasd-0.0.4/asd/utility/ovf_tools.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7753 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/plot_tools_3d.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13553 2023-05-01 09:39:25.000000 pyasd-0.0.4/asd/utility/post_llg.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5437 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/post_mc.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    19392 2023-04-07 12:17:17.000000 pyasd-0.0.4/asd/utility/spin_visualize_tools.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2442 2023-02-03 13:19:13.000000 pyasd-0.0.4/asd/utility/spirit_tool.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.731330 pyasd-0.0.4/examples/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      266 2023-01-11 07:09:44.000000 pyasd-0.0.4/examples/README
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.731330 pyasd-0.0.4/examples/example1/
--rw-r--r--   0 zsh       (1000) zsh       (1000)    53248 2022-11-27 08:16:32.000000 pyasd-0.0.4/examples/example1/.coverage
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2626 2023-01-05 02:33:47.000000 pyasd-0.0.4/examples/example1/single_spin_LLG.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.731330 pyasd-0.0.4/examples/example2/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      392 2023-01-11 07:10:07.000000 pyasd-0.0.4/examples/example2/README.md
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1305 2023-01-05 02:34:09.000000 pyasd-0.0.4/examples/example2/llg.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.735330 pyasd-0.0.4/examples/example3/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      385 2023-01-11 07:09:55.000000 pyasd-0.0.4/examples/example3/README.md
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1306 2022-11-27 08:14:55.000000 pyasd-0.0.4/examples/example3/llg.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.735330 pyasd-0.0.4/examples/example4/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       59 2022-10-28 23:58:00.000000 pyasd-0.0.4/examples/example4/README
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1319 2022-11-27 08:14:55.000000 pyasd-0.0.4/examples/example4/llg.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.707330 pyasd-0.0.4/misc/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.735330 pyasd-0.0.4/misc/archives/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)   492671 2022-11-26 13:27:45.000000 pyasd-0.0.4/misc/archives/ovf-0.4.3.tar.gz
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)   691395 2021-09-12 03:38:59.000000 pyasd-0.0.4/misc/archives/pyfiglet-0.7.tar.gz
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.739330 pyasd-0.0.4/pyasd.egg-info/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      425 2023-05-03 11:06:49.000000 pyasd-0.0.4/pyasd.egg-info/PKG-INFO
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     4686 2023-05-03 11:06:49.000000 pyasd-0.0.4/pyasd.egg-info/SOURCES.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-05-03 11:06:49.000000 pyasd-0.0.4/pyasd.egg-info/dependency_links.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       43 2023-05-03 11:06:49.000000 pyasd-0.0.4/pyasd.egg-info/requires.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     1083 2023-05-03 11:06:49.000000 pyasd-0.0.4/pyasd.egg-info/top_level.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-05-03 11:06:49.759330 pyasd-0.0.4/setup.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3339 2023-05-03 11:06:42.000000 pyasd-0.0.4/setup.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.707330 pyasd-0.0.4/tests_basic/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.743330 pyasd-0.0.4/tests_basic/B_eff/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      219 2023-01-05 07:15:01.000000 pyasd-0.0.4/tests_basic/B_eff/README
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1238 2023-01-05 07:14:20.000000 pyasd-0.0.4/tests_basic/B_eff/test_B_eff.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.743330 pyasd-0.0.4/tests_basic/OVF/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       64 2023-02-08 03:42:29.000000 pyasd-0.0.4/tests_basic/OVF/README
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     3532 2023-02-08 03:43:05.000000 pyasd-0.0.4/tests_basic/OVF/pyasd_ovf_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2777 2023-02-08 03:42:25.000000 pyasd-0.0.4/tests_basic/OVF/test_ovf.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.743330 pyasd-0.0.4/tests_basic/mag_confs/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.743330 pyasd-0.0.4/tests_basic/mag_confs/Potts/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      880 2022-12-11 16:02:18.000000 pyasd-0.0.4/tests_basic/mag_confs/Potts/Potts_test.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.743330 pyasd-0.0.4/tests_basic/mag_confs/domain_walls/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      916 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/domain_walls/analytical_single_domain.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1983 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/domain_walls/dw_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1558 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/interpolate_images.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.747330 pyasd-0.0.4/tests_basic/mag_confs/meron/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1229 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3213 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/meron/bimeron.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2055 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1475 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/meron/meron.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.747330 pyasd-0.0.4/tests_basic/mag_confs/misc/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1359 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/misc/interpolate_images.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1055 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/misc/mpi_topo.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1067 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/misc/regular_order_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1680 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/misc/struct_factor.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      768 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/misc/test_pbc_shell.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.751330 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1289 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/Skyrmion.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3902 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1935 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/a2sk.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1809 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/afm_skyrmion.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5572 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/firework.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4145 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2021-07-10 08:59:53.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/input.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2196 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/mpi_firework.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1241 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/skyrmionium.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      831 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/skyrmion/view_3d_skyr.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.751330 pyasd-0.0.4/tests_basic/mag_confs/spirals/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1511 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/spirals/CrMnI6_spiral.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2021-09-21 08:17:22.000000 pyasd-0.0.4/tests_basic/mag_confs/spirals/input.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4060 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/spirals/spiral_test.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1337 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/mag_confs/test_regular_orders_honeycomb.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.751330 pyasd-0.0.4/tests_basic/mpi/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      460 2023-01-05 15:02:33.000000 pyasd-0.0.4/tests_basic/mpi/test_group_rank.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.711331 pyasd-0.0.4/tests_basic/total_energy/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.707330 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.751330 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.755330 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      443 2022-11-20 00:54:15.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/input.cfg
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      120 2022-11-19 15:36:27.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/post
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      462 2022-11-20 00:54:36.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/quadruplet
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3625 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5188 2023-05-01 09:01:00.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.755330 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      363 2022-11-20 00:26:00.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/input.cfg
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      120 2022-11-19 15:38:35.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/post
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      449 2022-11-20 00:22:35.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/quadruplet
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      751 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.755330 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/simple/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7818 2022-11-19 12:09:07.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/simple/input.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3923 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.755330 pyasd-0.0.4/tests_basic/total_energy/chiral_confs/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1972 2023-01-05 11:42:50.000000 pyasd-0.0.4/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.755330 pyasd-0.0.4/tests_basic/total_energy/large_test/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      136 2023-01-05 15:00:27.000000 pyasd-0.0.4/tests_basic/total_energy/large_test/README
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1854 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/large_test/large_cell.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.755330 pyasd-0.0.4/tests_basic/total_energy/large_test/test_loop_methods/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1506 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1998 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.759330 pyasd-0.0.4/tests_basic/total_energy/local_energy/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      413 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/local_energy/CrMnI6_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4098 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/local_energy/test_local_en.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-03 11:06:49.759330 pyasd-0.0.4/tests_basic/total_energy/regular_orders/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7050 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/regular_orders/honeycomb_Heisenberg_phase_diagram.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1851 2023-01-05 07:16:05.000000 pyasd-0.0.4/tests_basic/total_energy/regular_orders/llg.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2685 2022-11-28 02:21:11.000000 pyasd-0.0.4/tests_basic/total_energy/regular_orders/phase_diagram_tri.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.038809 pyasd-0.0.5/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1468 2023-01-05 06:57:53.000000 pyasd-0.0.5/LICENSE
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      488 2023-01-06 02:20:47.000000 pyasd-0.0.5/MANIFEST.in
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      425 2023-05-09 02:33:46.038809 pyasd-0.0.5/PKG-INFO
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1350 2023-04-26 14:54:49.000000 pyasd-0.0.5/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:45.974808 pyasd-0.0.5/asd/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      344 2023-05-09 02:33:45.000000 pyasd-0.0.5/asd/__init__.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:45.978808 pyasd-0.0.5/asd/core/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)        0 2023-05-01 09:00:05.000000 pyasd-0.0.5/asd/core/__init__.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      537 2023-05-01 09:00:05.000000 pyasd-0.0.5/asd/core/constants.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      902 2023-05-01 09:00:05.000000 pyasd-0.0.5/asd/core/dipolar_interactions.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    14970 2023-05-01 09:00:05.000000 pyasd-0.0.5/asd/core/geometry.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    34800 2023-05-01 09:00:05.000000 pyasd-0.0.5/asd/core/gneb.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    28461 2023-05-01 09:00:05.000000 pyasd-0.0.5/asd/core/hamiltonian.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13407 2023-05-01 09:00:05.000000 pyasd-0.0.5/asd/core/llg_advanced.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    34609 2023-05-09 01:11:38.000000 pyasd-0.0.5/asd/core/llg_simple.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6394 2023-05-01 09:00:05.000000 pyasd-0.0.5/asd/core/log_general.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    35175 2023-05-01 09:00:05.000000 pyasd-0.0.5/asd/core/monte_carlo.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7330 2023-05-01 09:00:05.000000 pyasd-0.0.5/asd/core/random_vectors.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    28028 2023-05-03 15:39:15.000000 pyasd-0.0.5/asd/core/shell_exchange.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    20217 2023-05-01 09:00:05.000000 pyasd-0.0.5/asd/core/spin_configurations.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13692 2023-05-01 09:00:05.000000 pyasd-0.0.5/asd/core/spin_correlations.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4455 2023-05-07 01:15:42.000000 pyasd-0.0.5/asd/core/topological_charge.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:45.982808 pyasd-0.0.5/asd/data_base/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4160 2022-11-27 16:42:32.000000 pyasd-0.0.5/asd/data_base/exchange_for_Cr2I3X3.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1657 2022-11-03 04:08:41.000000 pyasd-0.0.5/asd/data_base/exchange_for_CrI3.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3216 2022-10-04 07:38:22.000000 pyasd-0.0.5/asd/data_base/exchange_for_CrMnI6_U2.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6933 2022-11-17 08:49:56.000000 pyasd-0.0.5/asd/data_base/exchange_for_CrMnI6_U4.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3873 2023-01-05 11:41:58.000000 pyasd-0.0.5/asd/data_base/exchange_for_CrMnI6_rect.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1295 2022-11-14 15:25:58.000000 pyasd-0.0.5/asd/data_base/exchange_for_Gd2C.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4390 2022-12-24 03:07:21.000000 pyasd-0.0.5/asd/data_base/exchange_for_MnI2.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2594 2022-12-24 03:07:20.000000 pyasd-0.0.5/asd/data_base/exchange_for_NiI2.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5909 2022-11-14 15:08:43.000000 pyasd-0.0.5/asd/data_base/exchange_for_RuCl3.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2188 2022-02-21 08:35:16.000000 pyasd-0.0.5/asd/data_base/exchange_for_VOI2.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1468 2022-11-27 16:26:00.000000 pyasd-0.0.5/asd/data_base/exchange_for_kagome.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1066 2022-02-21 07:00:49.000000 pyasd-0.0.5/asd/data_base/exchange_for_skx.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:45.982808 pyasd-0.0.5/asd/mpi/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2556 2023-05-09 02:04:47.000000 pyasd-0.0.5/asd/mpi/mpi_tools.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:45.994808 pyasd-0.0.5/asd/utility/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12245 2023-02-03 13:19:13.000000 pyasd-0.0.5/asd/utility/Swq.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)        0 2023-02-03 13:19:13.000000 pyasd-0.0.5/asd/utility/__init__.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     8709 2023-05-07 06:58:07.000000 pyasd-0.0.5/asd/utility/analyze_Spirit_results.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9134 2023-05-07 06:52:31.000000 pyasd-0.0.5/asd/utility/asd_arguments.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    55462 2023-02-03 13:19:13.000000 pyasd-0.0.5/asd/utility/auxiliary_colormaps.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     2143 2023-02-03 13:19:28.000000 pyasd-0.0.5/asd/utility/curve_fit.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5328 2023-02-03 13:19:13.000000 pyasd-0.0.5/asd/utility/four_state_tools.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1880 2023-04-17 02:00:31.000000 pyasd-0.0.5/asd/utility/head_figlet.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6688 2023-02-07 02:54:27.000000 pyasd-0.0.5/asd/utility/mag_thermal.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     7619 2023-05-09 02:11:15.000000 pyasd-0.0.5/asd/utility/ovf_tools.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7753 2023-02-03 13:19:13.000000 pyasd-0.0.5/asd/utility/plot_tools_3d.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13553 2023-05-07 06:40:57.000000 pyasd-0.0.5/asd/utility/post_llg.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5470 2023-05-07 06:40:40.000000 pyasd-0.0.5/asd/utility/post_mc.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    19392 2023-05-09 02:10:46.000000 pyasd-0.0.5/asd/utility/spin_visualize_tools.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2442 2023-05-09 02:10:36.000000 pyasd-0.0.5/asd/utility/spirit_tool.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:45.994808 pyasd-0.0.5/examples/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      266 2023-01-11 07:09:44.000000 pyasd-0.0.5/examples/README
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:45.998808 pyasd-0.0.5/examples/example1/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    53248 2022-11-27 08:16:32.000000 pyasd-0.0.5/examples/example1/.coverage
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2626 2023-01-05 02:33:47.000000 pyasd-0.0.5/examples/example1/single_spin_LLG.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:45.998808 pyasd-0.0.5/examples/example2/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      392 2023-01-11 07:10:07.000000 pyasd-0.0.5/examples/example2/README.md
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1305 2023-01-05 02:34:09.000000 pyasd-0.0.5/examples/example2/llg.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:45.998808 pyasd-0.0.5/examples/example3/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      385 2023-01-11 07:09:55.000000 pyasd-0.0.5/examples/example3/README.md
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1306 2022-11-27 08:14:55.000000 pyasd-0.0.5/examples/example3/llg.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.002808 pyasd-0.0.5/examples/example4/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       59 2022-10-28 23:58:00.000000 pyasd-0.0.5/examples/example4/README
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1319 2022-11-27 08:14:55.000000 pyasd-0.0.5/examples/example4/llg.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:45.966808 pyasd-0.0.5/misc/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.002808 pyasd-0.0.5/misc/archives/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)   492671 2022-11-26 13:27:45.000000 pyasd-0.0.5/misc/archives/ovf-0.4.3.tar.gz
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)   691395 2021-09-12 03:38:59.000000 pyasd-0.0.5/misc/archives/pyfiglet-0.7.tar.gz
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.010808 pyasd-0.0.5/pyasd.egg-info/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      425 2023-05-09 02:33:45.000000 pyasd-0.0.5/pyasd.egg-info/PKG-INFO
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     4686 2023-05-09 02:33:45.000000 pyasd-0.0.5/pyasd.egg-info/SOURCES.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-05-09 02:33:45.000000 pyasd-0.0.5/pyasd.egg-info/dependency_links.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       43 2023-05-09 02:33:45.000000 pyasd-0.0.5/pyasd.egg-info/requires.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1083 2023-05-09 02:33:45.000000 pyasd-0.0.5/pyasd.egg-info/top_level.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-05-09 02:33:46.038809 pyasd-0.0.5/setup.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3490 2023-05-09 02:33:38.000000 pyasd-0.0.5/setup.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:45.970808 pyasd-0.0.5/tests_basic/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.014808 pyasd-0.0.5/tests_basic/B_eff/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      219 2023-01-05 07:15:01.000000 pyasd-0.0.5/tests_basic/B_eff/README
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1238 2023-01-05 07:14:20.000000 pyasd-0.0.5/tests_basic/B_eff/test_B_eff.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.014808 pyasd-0.0.5/tests_basic/OVF/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       64 2023-02-08 03:42:29.000000 pyasd-0.0.5/tests_basic/OVF/README
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     3532 2023-02-08 03:43:05.000000 pyasd-0.0.5/tests_basic/OVF/pyasd_ovf_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2777 2023-02-08 03:42:25.000000 pyasd-0.0.5/tests_basic/OVF/test_ovf.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.014808 pyasd-0.0.5/tests_basic/mag_confs/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.018808 pyasd-0.0.5/tests_basic/mag_confs/Potts/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      880 2022-12-11 16:02:18.000000 pyasd-0.0.5/tests_basic/mag_confs/Potts/Potts_test.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.018808 pyasd-0.0.5/tests_basic/mag_confs/domain_walls/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      916 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/domain_walls/analytical_single_domain.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1983 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/domain_walls/dw_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1558 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/interpolate_images.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.022808 pyasd-0.0.5/tests_basic/mag_confs/meron/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1229 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3213 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/meron/bimeron.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2055 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1475 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/meron/meron.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.022808 pyasd-0.0.5/tests_basic/mag_confs/misc/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1359 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/misc/interpolate_images.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1055 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/misc/mpi_topo.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1067 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/misc/regular_order_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1680 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/misc/struct_factor.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      768 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/misc/test_pbc_shell.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.026808 pyasd-0.0.5/tests_basic/mag_confs/skyrmion/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1289 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/skyrmion/Skyrmion.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3902 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1935 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/skyrmion/a2sk.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1809 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/skyrmion/afm_skyrmion.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5572 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/skyrmion/firework.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4145 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2021-07-10 08:59:53.000000 pyasd-0.0.5/tests_basic/mag_confs/skyrmion/input.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2196 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/skyrmion/mpi_firework.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1241 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/skyrmion/skyrmionium.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      831 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/skyrmion/view_3d_skyr.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.030809 pyasd-0.0.5/tests_basic/mag_confs/spirals/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1511 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/spirals/CrMnI6_spiral.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2021-09-21 08:17:22.000000 pyasd-0.0.5/tests_basic/mag_confs/spirals/input.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4060 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/spirals/spiral_test.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1337 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/mag_confs/test_regular_orders_honeycomb.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.030809 pyasd-0.0.5/tests_basic/mpi/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      460 2023-01-05 15:02:33.000000 pyasd-0.0.5/tests_basic/mpi/test_group_rank.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:45.970808 pyasd-0.0.5/tests_basic/total_energy/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:45.970808 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.030809 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.030809 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      443 2022-11-20 00:54:15.000000 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/input.cfg
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      120 2022-11-19 15:36:27.000000 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/post
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      462 2022-11-20 00:54:36.000000 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/quadruplet
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3625 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5188 2023-05-01 09:01:00.000000 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.034808 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      363 2022-11-20 00:26:00.000000 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/input.cfg
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      120 2022-11-19 15:38:35.000000 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/post
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      449 2022-11-20 00:22:35.000000 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/quadruplet
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      751 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.034808 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/simple/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7818 2022-11-19 12:09:07.000000 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/simple/input.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3923 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.034808 pyasd-0.0.5/tests_basic/total_energy/chiral_confs/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1972 2023-01-05 11:42:50.000000 pyasd-0.0.5/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.034808 pyasd-0.0.5/tests_basic/total_energy/large_test/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      136 2023-01-05 15:00:27.000000 pyasd-0.0.5/tests_basic/total_energy/large_test/README
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1854 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/total_energy/large_test/large_cell.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.034808 pyasd-0.0.5/tests_basic/total_energy/large_test/test_loop_methods/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1506 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1998 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.034808 pyasd-0.0.5/tests_basic/total_energy/local_energy/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      413 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/total_energy/local_energy/CrMnI6_test.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4098 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/total_energy/local_energy/test_local_en.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 02:33:46.038809 pyasd-0.0.5/tests_basic/total_energy/regular_orders/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7050 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/total_energy/regular_orders/honeycomb_Heisenberg_phase_diagram.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1851 2023-01-05 07:16:05.000000 pyasd-0.0.5/tests_basic/total_energy/regular_orders/llg.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2685 2022-11-28 02:21:11.000000 pyasd-0.0.5/tests_basic/total_energy/regular_orders/phase_diagram_tri.py
```

### Comparing `pyasd-0.0.4/LICENSE` & `pyasd-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/README.md` & `pyasd-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/core/constants.py` & `pyasd-0.0.5/asd/core/constants.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/core/dipolar_interactions.py` & `pyasd-0.0.5/asd/core/dipolar_interactions.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/core/geometry.py` & `pyasd-0.0.5/asd/core/geometry.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/core/gneb.py` & `pyasd-0.0.5/asd/core/gneb.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/core/hamiltonian.py` & `pyasd-0.0.5/asd/core/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/core/llg_advanced.py` & `pyasd-0.0.5/asd/core/llg_advanced.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/core/llg_simple.py` & `pyasd-0.0.5/asd/core/llg_simple.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/core/log_general.py` & `pyasd-0.0.5/asd/core/log_general.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/core/monte_carlo.py` & `pyasd-0.0.5/asd/core/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/core/random_vectors.py` & `pyasd-0.0.5/asd/core/random_vectors.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/core/shell_exchange.py` & `pyasd-0.0.5/asd/core/shell_exchange.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/core/spin_configurations.py` & `pyasd-0.0.5/asd/core/spin_configurations.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/core/spin_correlations.py` & `pyasd-0.0.5/asd/core/spin_correlations.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/core/topological_charge.py` & `pyasd-0.0.5/asd/core/topological_charge.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/data_base/exchange_for_Cr2I3X3.py` & `pyasd-0.0.5/asd/data_base/exchange_for_Cr2I3X3.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/data_base/exchange_for_CrI3.py` & `pyasd-0.0.5/asd/data_base/exchange_for_CrI3.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/data_base/exchange_for_CrMnI6_U2.py` & `pyasd-0.0.5/asd/data_base/exchange_for_CrMnI6_U2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/data_base/exchange_for_CrMnI6_U4.py` & `pyasd-0.0.5/asd/data_base/exchange_for_CrMnI6_U4.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/data_base/exchange_for_CrMnI6_rect.py` & `pyasd-0.0.5/asd/data_base/exchange_for_CrMnI6_rect.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/data_base/exchange_for_Gd2C.py` & `pyasd-0.0.5/asd/data_base/exchange_for_Gd2C.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/data_base/exchange_for_MnI2.py` & `pyasd-0.0.5/asd/data_base/exchange_for_MnI2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/data_base/exchange_for_NiI2.py` & `pyasd-0.0.5/asd/data_base/exchange_for_NiI2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/data_base/exchange_for_RuCl3.py` & `pyasd-0.0.5/asd/data_base/exchange_for_RuCl3.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/data_base/exchange_for_VOI2.py` & `pyasd-0.0.5/asd/data_base/exchange_for_VOI2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/data_base/exchange_for_kagome.py` & `pyasd-0.0.5/asd/data_base/exchange_for_kagome.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/data_base/exchange_for_skx.py` & `pyasd-0.0.5/asd/data_base/exchange_for_skx.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/mpi/mpi_tools.py` & `pyasd-0.0.5/asd/mpi/mpi_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/utility/Swq.py` & `pyasd-0.0.5/asd/utility/Swq.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/utility/analyze_Spirit_results.py` & `pyasd-0.0.5/asd/utility/analyze_Spirit_results.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 other scirpts are not affected
 Please install Spirit properly
 if you want ot use this script\n'''.format(__file__.split('/')[-1])
 
 try:    from spirit import state,system,geometry,parameters
 except: exit(import_spirit_err)
 
-outdir='output'
-
 
 def collect_confs_from_ovfs(outdir,prefix):
     confs=[]
     fils = glob.glob('{}/{}*Spins_*.ovf'.format(outdir,prefix))
     if len(fils)==0: exit('Cannot find ovf files in the directory\n{}'.format(outdir))
     indices = sorted([int(fil.split('_')[-1].rstrip('.ovf')) for fil in fils])
     nn = len(fils[-1].rstrip('.ovf').split('_')[-1])+1
@@ -80,16 +78,17 @@
         if fil_cfg=='': geometry.set_bravais_lattice_type(p_state, lat_type)
         if nx*ny*nz!=0: geometry.set_n_cells(p_state,[nx,ny,nz])
         pos=geometry.get_positions(p_state)
         nx,ny,nz=geometry.get_n_cells(p_state)
         nat=geometry.get_n_cell_atoms(p_state)
         latt=geometry.get_bravais_vectors(p_state)
         if dt==0: dt = parameters.llg.get_timestep(p_state)
-    latt = lattice_constant*np.array(latt)
-    return latt,pos,nx,ny,nz,nat,dt
+        latt = lattice_constant*np.array(latt)
+        np.savetxt('Positions.dat',pos,fmt='%10.5f')
+        return latt,pos,nx,ny,nz,nat,dt
 
 
 def analyze_GNEB_results(scatter_size=10):
     Rx, Etot = plot_GNEB(outdir)
 
     fil_ovf=glob.glob('{}/*Spins-initial.ovf'.format(outdir))[0]
     print (fil_ovf)
@@ -100,14 +99,15 @@
 
     nx = params['xnodes']
     ny = params['ynodes']
     nz = params['znodes']
 
     latt,pos,nx,ny,nz,nat,dt = get_params_from_cfg(fil_cfg,nx,ny,nz)
 
+    print (spins_init.shape,spins_final.shape,scatter_size)
     plot_spin_2d(pos,spins_init, scatter_size=scatter_size,title='initial')
     plot_spin_2d(pos,spins_final,scatter_size=scatter_size,title='final'  )
     plt.show()
 
     fil = sorted(glob.glob('{}/*Chain*final.ovf'.format(outdir)))[0]
     print ('confs from file {}'.format(fil))
     Iter = np.array([line.split()[-1] for line in os.popen('grep Iteration {}'.format(fil)).readlines()],int)
@@ -121,26 +121,27 @@
     assert len(fil)>0, 'Energy file out found!'
     lines = open(fil[0]).readlines()[3:][start_conf:]
     iters = np.array([line.split()[0] for line in lines],float)
     ens = np.array([line.split()[2] for line in lines],float)
     return iters,ens
 
 
-def analyze_LLG_results(args,lat_type=1,dt=0,
-    outdir='.',prefix='',fil_cfg='',jump=1,quiver_kws=None,anim=True):
+def analyze_LLG_results(args,lat_type=1,
+    quiver_kws=None):
 
     spin_plot_kwargs = get_spin_plot_kwargs(args)
     spin_anim_kwargs = get_spin_anim_kwargs(args)
     spin_plot_kwargs.update(quiver_kws=quiver_kws)
     spin_anim_kwargs.update(quiver_kws=quiver_kws)
 
 
+    outdir = args.outdir
     if outdir=='.': outdir=os.getcwd()
-    print ('spirit input file: {}\n'.format(fil_cfg))
-    latt,pos,nx,ny,nz,nat,dt = get_params_from_cfg(fil_cfg,args.nx,args.ny,args.nz,dt=dt)
+    print ('spirit input file: {}\n'.format(args.spirit_input_file))
+    latt,pos,nx,ny,nz,nat,dt = get_params_from_cfg(args.spirit_input_file,args.nx,args.ny,args.nz,dt=args.dt)
 
     def display_snapshot(pos,latt,outdir,prefix,status='initial',show=False):
         superlatt = np.dot(np.diag([nx,ny]),latt)
         fils=glob.glob('{}/{}*Spins-{}.ovf'.format(outdir,prefix,status))
         if len(fils)>0: 
             fil_ovf = fils[0]
             print ('\nDisplay config of file {}'.format(fil_ovf))
@@ -161,50 +162,49 @@
         ax.set_xlabel('t (ps)')
         ax.set_ylabel('E (meV/site)')
         fig.tight_layout()
         fig.savefig('LLG_energies_profile',dpi=300)
         if show: plt.show()
 
     try: 
-        iters,ens = get_energy_from_txt(0,outdir,prefix)
+        iters,ens = get_energy_from_txt(0,outdir,args.prefix)
         plot_energy(iters,dt,ens)
     except:
         print ('Fail to read energy from txt file, skip plotting energy')
 
     latt = np.array(latt)[:2,:2].T
+    pos = np.loadtxt('Positions.dat')
     if nx*ny*nz!=0:
-        nat = pos.shape[0]//(nx*ny)
-        pos=pos.reshape(ny,nx,nat,3)
+        pos=pos.reshape(ny,nx,-1,3)
         pos = np.swapaxes(pos,0,1)
-        display_snapshot(pos,latt,outdir,prefix,'initial')
-        display_snapshot(pos,latt,outdir,prefix,'final',show=True)
+        display_snapshot(pos,latt,outdir,args.prefix,'initial')
+        display_snapshot(pos,latt,outdir,args.prefix,'final',show=True)
 
-    if anim:
+    if args.make_ani:
         titles = None
-        fil = glob.glob('{}/{}*Spins-archive.ovf'.format(outdir,prefix))
+        fil = glob.glob('{}/{}*Spins-archive.ovf'.format(outdir,args.prefix))
         if len(fil)==1:
             fil = fil[0]
             print ('\nSpin configs from achive file {}'.format(fil))
             Iter = np.array([line.split()[-1] for line in os.popen('grep Iteration {}'.format(fil)).readlines()],int)
-            titles = ['t = {:10.4f} ps'.format(tt) for tt in Iter*dt]
             confs = parse_ovf_1(fil,parse_params=False)[1]
+            titles = ['t = {:10.4f} ps'.format(tt) for tt in Iter*dt]
         else:
-            confs = collect_confs_from_ovfs(outdir,prefix)
+            confs = collect_confs_from_ovfs(outdir,args.prefix)
         confs = confs.reshape(-1,ny,nx,nat,3)
+        if args.topo_chg:
+            from asd.core.topological_charge import calc_topo_chg
+            print ('Set topo_chg=T, calculate the topological charge')
+            print ('This might take several minutes')
+            Qs = [calc_topo_chg(conf,pos[...,:2]) for conf in confs]
+            titles = ['{}, Q = {:6.3f}'.format(tl,Q) for (tl,Q) in zip(titles,Qs)]
         confs = np.swapaxes(confs,1,2)
         spin_anim_kwargs.update(latt=latt)
         make_ani(pos, confs, titles=titles, **spin_anim_kwargs)
     
-        #under development
-        #confs_repeat = np.array([get_repeated_conf(conf,args.repeat_x,args.repeat_y) for conf in confs])
-        #pos_repeat = np.tile(pos,(args.repeat_x,args.repeat_y,1,1))
-        #for ix,iy in np.ndindex(args.repeat_x,arge.repeat_y):
-        #    pos_repeat[ny*ii:ny*(ii+1),:,:,1] += ii*latt[1,1]
-        #make_ani(pos_repeat, confs_repeat, titles=titles, **spin_anim_kwargs)
-
     return 1
 
 
 def gen_args():
     import argparse
     prog='analyze_Spirit_results.py'
     description = 'post-processing of Spirit LLG simulations'
@@ -214,25 +214,18 @@
     add_spirit_arguments(parser)
     add_quiver_arguments(parser)
     add_spin_plot_arguments(parser)
     add_common_arguments(parser)
     args = parser.parse_args()
     return args
 
+
 if __name__=='__main__':
     args = gen_args()
     quiver_kws = dict([(k.split('_')[1],v) for (k,v) in vars(args).items() if k.startswith('quiver')])
     quiver_kws.update(pivot='mid',units='x')
     print ('keyword arguments for quivers\n')
     for key in quiver_kws.keys(): print ('{:>15s} = {}'.format(key,quiver_kws[key]))
 
-    fil_cfg = args.spirit_input_file
     print ('\ntask = {}\n'.format(args.job))
-    if args.job=='llg':     
-        kwargs = dict(
-        fil_cfg=args.spirit_input_file,
-        outdir=args.outdir,prefix=args.prefix,
-        quiver_kws=quiver_kws,
-        anim=args.make_ani,
-        dt=args.dt)
-        analyze_LLG_results(args,**kwargs)
+    if args.job=='llg':     analyze_LLG_results(args,quiver_kws=quiver_kws)
     elif args.job=='gneb':  analyze_GNEB_results()
```

### Comparing `pyasd-0.0.4/asd/utility/asd_arguments.py` & `pyasd-0.0.5/asd/utility/asd_arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
 def add_mc_arguments(parser):
     parser.add_argument('--task',type=str,default='thermal',help='task for post processing of MC simulation results')
     parser.add_argument('--mc_file',type=str,default='mc.py',help='scirpt name for Monte Carlo simulation, used in post-processing')
     parser.add_argument('--start_conf_idx',type=int,default=0,help='index of the first snapshot to calculate ensemble average')
     parser.add_argument('--itemp',type=int,default=0,help='index for temperature points')
     parser.add_argument('--iconf',type=int,default=0,help='index for snapshot configuration')
-    parser.add_argument('--outdir',type=str,default='.',help='directory to store MC data')
 
 
 def add_llg_arguments(parser):
     #parser.add_argument('--',type=,default=,help='')
     parser.add_argument('--dt',type=float,default=0.001,help='time step for LLG')
     parser.add_argument('--lat_type',type=str,default='honeycomb',help='type of spin lattice')
     parser.add_argument('--solid_angle_method',type=int,default=2,help='method to calculate the solid angle (for topological charge)')
```

### Comparing `pyasd-0.0.4/asd/utility/auxiliary_colormaps.py` & `pyasd-0.0.5/asd/utility/auxiliary_colormaps.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/utility/curve_fit.py` & `pyasd-0.0.5/asd/utility/curve_fit.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/utility/four_state_tools.py` & `pyasd-0.0.5/asd/utility/four_state_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/utility/head_figlet.py` & `pyasd-0.0.5/asd/utility/head_figlet.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/utility/mag_thermal.py` & `pyasd-0.0.5/asd/utility/mag_thermal.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/utility/ovf_tools.py` & `pyasd-0.0.5/asd/utility/ovf_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 ovf_exception = '''
 ovf not installed! 
 Install it via pip or manually 
 A tarball package can be found in
 pyasd/misc/archives
 '''
 
-import numpy as np
 try: from ovf import ovf
-except: raise Exception(ovf_exception)
+except: print (ovf_exception)
+#except: raise Exception(ovf_exception)
+
 import numpy as np
 import os
 import re
 
 ###################################
 # Following: the new part
 # invoking the ovf package
```

### Comparing `pyasd-0.0.4/asd/utility/plot_tools_3d.py` & `pyasd-0.0.5/asd/utility/plot_tools_3d.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/utility/post_llg.py` & `pyasd-0.0.5/asd/utility/post_llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/utility/post_mc.py` & `pyasd-0.0.5/asd/utility/post_mc.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import importlib
 import re
 import glob
 
 def get_args():
     import argparse
     parser = argparse.ArgumentParser(prog='asd_arguments.py', description = 'post-processing of llg')
+    add_common_arguments(parser)
     add_mc_arguments(parser)
     add_switch_arguments(parser)
     add_quiver_arguments(parser)
     add_spin_plot_arguments(parser)
     args = parser.parse_args()
     return args
```

### Comparing `pyasd-0.0.4/asd/utility/spin_visualize_tools.py` & `pyasd-0.0.5/asd/utility/spin_visualize_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/asd/utility/spirit_tool.py` & `pyasd-0.0.5/asd/utility/spirit_tool.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/examples/example1/.coverage` & `pyasd-0.0.5/examples/example1/.coverage`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/examples/example1/single_spin_LLG.py` & `pyasd-0.0.5/examples/example1/single_spin_LLG.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/examples/example2/llg.py` & `pyasd-0.0.5/examples/example2/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/examples/example3/llg.py` & `pyasd-0.0.5/examples/example3/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/examples/example4/llg.py` & `pyasd-0.0.5/examples/example4/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/misc/archives/ovf-0.4.3.tar.gz` & `pyasd-0.0.5/misc/archives/ovf-0.4.3.tar.gz`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/misc/archives/pyfiglet-0.7.tar.gz` & `pyasd-0.0.5/misc/archives/pyfiglet-0.7.tar.gz`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/pyasd.egg-info/SOURCES.txt` & `pyasd-0.0.5/pyasd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/pyasd.egg-info/top_level.txt` & `pyasd-0.0.5/pyasd.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/setup.py` & `pyasd-0.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,17 +59,18 @@
 core_modules  = ['asd/core/{}'.format(item) for item in core_modules]
 utility_modules  = ['asd/utility/{}'.format(item) for item in utility_modules]
 mpi_modules = ['asd/mpi/mpi_tools']
 
 
 kwargs_setup = dict(
 name='pyasd',
-version='0.0.4',
+version='0.0.5',
 author='Shunhong Zhang',
 author_email='zhangshunhong.pku@gmail.com',
+platform=sys.platform,
 url='https://to_be_posted',
 download_url='https://on_request',
 keywords='spin dynamics simulation',
 py_modules = utility_modules + core_modules + database_modules + mpi_modules + init_files,
 packages = setuptools.find_packages(),
 license='LICENSE',
 license_file='LICENSE',
@@ -88,20 +89,23 @@
 )
 
       
 bindirs = ['{}/asd/utility'.format(os.getcwd())]
 
 
 def set_build_time_stamp(kwargs_setup):
+    import locale
     with open('asd/__init__.py','r') as fw: lines = fw.readlines()
-    __doc__ = '{:<20s}  =  "built at {} {}"\n'.format('__built_time__',time.ctime(),time.tzname[1])
+    __doc__ = '{:<20s}  =  "built at {}'.format('__built_time__',time.ctime())
+    if locale.getdefaultlocale()[0]=='en_US': __doc__ += '_{}"\n'.format(time.tzname[1])
+    else: __doc__ += '"\n'
     lines = [__doc__] + [line for line in lines if '__built_time__' not in line]
     with open('asd/__init__.py','w') as fw: 
         fw.write(__doc__)
-        for key in ['__name__','__version__','__author__','__author_email__','__url__','__license__']:
+        for key in ['__name__','__version__','__author__','__author_email__','__url__','__license__','__platform__']:
             print ('{:<20s}  =  "{}"'.format(key,kwargs_setup[key.strip('__')]),file=fw)
  
  
  
 if __name__=='__main__':
     set_build_time_stamp(kwargs_setup)
     print('\n{0}\nINSTALL\n{0}'.format('='*50))
```

### Comparing `pyasd-0.0.4/tests_basic/B_eff/test_B_eff.py` & `pyasd-0.0.5/tests_basic/B_eff/test_B_eff.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/OVF/pyasd_ovf_test.py` & `pyasd-0.0.5/tests_basic/OVF/pyasd_ovf_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/OVF/test_ovf.py` & `pyasd-0.0.5/tests_basic/OVF/test_ovf.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/Potts/Potts_test.py` & `pyasd-0.0.5/tests_basic/mag_confs/Potts/Potts_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/domain_walls/analytical_single_domain.py` & `pyasd-0.0.5/tests_basic/mag_confs/domain_walls/analytical_single_domain.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/domain_walls/dw_test.py` & `pyasd-0.0.5/tests_basic/mag_confs/domain_walls/dw_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/interpolate_images.py` & `pyasd-0.0.5/tests_basic/mag_confs/interpolate_images.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py` & `pyasd-0.0.5/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/meron/bimeron.py` & `pyasd-0.0.5/tests_basic/mag_confs/meron/bimeron.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py` & `pyasd-0.0.5/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/meron/meron.py` & `pyasd-0.0.5/tests_basic/mag_confs/meron/meron.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/misc/interpolate_images.py` & `pyasd-0.0.5/tests_basic/mag_confs/misc/interpolate_images.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/misc/mpi_topo.py` & `pyasd-0.0.5/tests_basic/mag_confs/misc/mpi_topo.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/misc/regular_order_test.py` & `pyasd-0.0.5/tests_basic/mag_confs/misc/regular_order_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/misc/struct_factor.py` & `pyasd-0.0.5/tests_basic/mag_confs/misc/struct_factor.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/misc/test_pbc_shell.py` & `pyasd-0.0.5/tests_basic/mag_confs/misc/test_pbc_shell.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/Skyrmion.py` & `pyasd-0.0.5/tests_basic/mag_confs/skyrmion/Skyrmion.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py` & `pyasd-0.0.5/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/a2sk.py` & `pyasd-0.0.5/tests_basic/mag_confs/skyrmion/a2sk.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/afm_skyrmion.py` & `pyasd-0.0.5/tests_basic/mag_confs/skyrmion/afm_skyrmion.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/firework.py` & `pyasd-0.0.5/tests_basic/mag_confs/skyrmion/firework.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py` & `pyasd-0.0.5/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/mpi_firework.py` & `pyasd-0.0.5/tests_basic/mag_confs/skyrmion/mpi_firework.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/skyrmionium.py` & `pyasd-0.0.5/tests_basic/mag_confs/skyrmion/skyrmionium.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/skyrmion/view_3d_skyr.py` & `pyasd-0.0.5/tests_basic/mag_confs/skyrmion/view_3d_skyr.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/spirals/CrMnI6_spiral.py` & `pyasd-0.0.5/tests_basic/mag_confs/spirals/CrMnI6_spiral.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/spirals/spiral_test.py` & `pyasd-0.0.5/tests_basic/mag_confs/spirals/spiral_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/mag_confs/test_regular_orders_honeycomb.py` & `pyasd-0.0.5/tests_basic/mag_confs/test_regular_orders_honeycomb.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py` & `pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py` & `pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py` & `pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py` & `pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py` & `pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/simple/input.cfg` & `pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/simple/input.cfg`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py` & `pyasd-0.0.5/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py` & `pyasd-0.0.5/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/total_energy/large_test/large_cell.py` & `pyasd-0.0.5/tests_basic/total_energy/large_test/large_cell.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py` & `pyasd-0.0.5/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py` & `pyasd-0.0.5/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/total_energy/local_energy/test_local_en.py` & `pyasd-0.0.5/tests_basic/total_energy/local_energy/test_local_en.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/total_energy/regular_orders/honeycomb_Heisenberg_phase_diagram.py` & `pyasd-0.0.5/tests_basic/total_energy/regular_orders/honeycomb_Heisenberg_phase_diagram.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/total_energy/regular_orders/llg.py` & `pyasd-0.0.5/tests_basic/total_energy/regular_orders/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.4/tests_basic/total_energy/regular_orders/phase_diagram_tri.py` & `pyasd-0.0.5/tests_basic/total_energy/regular_orders/phase_diagram_tri.py`

 * *Files identical despite different names*

