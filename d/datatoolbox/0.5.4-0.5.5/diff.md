# Comparing `tmp/datatoolbox-0.5.4.tar.gz` & `tmp/datatoolbox-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatoolbox-0.5.4.tar", last modified: Thu Dec  1 09:42:22 2022, max compression
+gzip compressed data, was "datatoolbox-0.5.5.tar", last modified: Tue May  9 08:11:42 2023, max compression
```

## Comparing `datatoolbox-0.5.4.tar` & `datatoolbox-0.5.5.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-12-01 09:42:22.000000 datatoolbox-0.5.4/
--rwxrwx---   0 root         (0) vboxsf     (999)      159 2022-05-25 07:15:53.000000 datatoolbox-0.5.4/.gitignore
--rwxrwx---   0 root         (0) vboxsf     (999)      950 2022-10-19 13:17:33.000000 datatoolbox-0.5.4/.gitlab-ci.yml
--rwxrwx---   0 root         (0) vboxsf     (999)      703 2020-10-14 14:04:18.000000 datatoolbox-0.5.4/.travis.yml
--rwxrwx---   0 root         (0) vboxsf     (999)     1073 2020-10-14 14:04:18.000000 datatoolbox-0.5.4/LICENSE
--rwxrwx---   0 root         (0) vboxsf     (999)     1037 2022-12-01 09:42:22.000000 datatoolbox-0.5.4/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (999)      771 2022-05-25 07:15:53.000000 datatoolbox-0.5.4/README.md
--rwxrwx---   0 root         (0) vboxsf     (999)     1225 2020-10-14 14:04:18.000000 datatoolbox-0.5.4/appveyor.yml
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-12-01 09:42:21.000000 datatoolbox-0.5.4/ci/
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-12-01 09:42:21.000000 datatoolbox-0.5.4/ci/appveyor/
--rwxrwx---   0 root         (0) vboxsf     (999)     3111 2020-10-14 14:04:18.000000 datatoolbox-0.5.4/ci/appveyor/install.ps1
--rwxrwx---   0 root         (0) vboxsf     (999)     1842 2020-10-14 14:04:18.000000 datatoolbox-0.5.4/ci/appveyor/run_with_env.cmd
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-12-01 09:42:21.000000 datatoolbox-0.5.4/datatoolbox/
--rwxrwx---   0 root         (0) vboxsf     (999)     4240 2022-11-22 09:51:24.000000 datatoolbox-0.5.4/datatoolbox/__init__.py
--rwxrwx---   0 root         (0) vboxsf     (999)    14979 2022-12-01 09:27:15.000000 datatoolbox-0.5.4/datatoolbox/admin.py
--rwxrwx---   0 root         (0) vboxsf     (999)     6655 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/config.py
--rwxrwx---   0 root         (0) vboxsf     (999)    18640 2022-12-01 09:27:15.000000 datatoolbox-0.5.4/datatoolbox/converters.py
--rwxrwx---   0 root         (0) vboxsf     (999)    11628 2022-11-22 09:52:38.000000 datatoolbox-0.5.4/datatoolbox/core.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-12-01 09:42:21.000000 datatoolbox-0.5.4/datatoolbox/data/
--rwxrwx---   0 root         (0) vboxsf     (999)    15781 2020-10-14 14:04:18.000000 datatoolbox-0.5.4/datatoolbox/data/GHG_alternative_naming.pkl
--rwxrwx---   0 root         (0) vboxsf     (999)    13482 2020-10-14 14:04:18.000000 datatoolbox-0.5.4/datatoolbox/data/GHG_properties_2019_CA.csv
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-12-01 09:42:21.000000 datatoolbox-0.5.4/datatoolbox/data/SANDBOX_datashelf/
--rwxrwx---   0 root         (0) vboxsf     (999)      286 2022-11-22 10:09:45.000000 datatoolbox-0.5.4/datatoolbox/data/SANDBOX_datashelf/inventory.csv
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-12-01 09:42:21.000000 datatoolbox-0.5.4/datatoolbox/data/SANDBOX_datashelf/mappings/
--rwxrwx---   0 root         (0) vboxsf     (999)    10757 2022-11-22 10:09:44.000000 datatoolbox-0.5.4/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv
--rwxrwx---   0 root         (0) vboxsf     (999)     8466 2022-11-22 10:09:44.000000 datatoolbox-0.5.4/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv
--rwxrwx---   0 root         (0) vboxsf     (999)      999 2022-11-22 10:09:44.000000 datatoolbox-0.5.4/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv
--rwxrwx---   0 root         (0) vboxsf     (999)      161 2022-11-22 10:09:45.000000 datatoolbox-0.5.4/datatoolbox/data/SANDBOX_datashelf/sources.csv
--rwxrwx---   0 root         (0) vboxsf     (999)    22865 2020-10-14 14:04:18.000000 datatoolbox-0.5.4/datatoolbox/data/all.csv
--rwxrwx---   0 root         (0) vboxsf     (999)    14615 2020-10-14 14:04:18.000000 datatoolbox-0.5.4/datatoolbox/data/compatible1_5_unfiltered.xlsx
--rwxrwx---   0 root         (0) vboxsf     (999)    10757 2020-04-20 12:32:09.000000 datatoolbox-0.5.4/datatoolbox/data/continent.csv
--rwxrwx---   0 root         (0) vboxsf     (999)     8466 2021-09-15 15:48:16.000000 datatoolbox-0.5.4/datatoolbox/data/country_codes.csv
--rwxrwx---   0 root         (0) vboxsf     (999)     1711 2022-05-25 07:15:53.000000 datatoolbox-0.5.4/datatoolbox/data/datashelf_contents.csv
--rwxrwx---   0 root         (0) vboxsf     (999)     2923 2021-12-16 12:32:58.000000 datatoolbox-0.5.4/datatoolbox/data/external_mappings.py
--rwxrwx---   0 root         (0) vboxsf     (999)      178 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/data/personal_template.py
--rwxrwx---   0 root         (0) vboxsf     (999)      999 2019-08-14 10:00:22.000000 datatoolbox-0.5.4/datatoolbox/data/regions.csv
--rwxrwx---   0 root         (0) vboxsf     (999)   236966 2022-11-22 09:50:04.000000 datatoolbox-0.5.4/datatoolbox/data_readers.py
--rwxrwx---   0 root         (0) vboxsf     (999)    67094 2022-11-22 09:53:24.000000 datatoolbox-0.5.4/datatoolbox/data_structures.py
--rwxrwx---   0 root         (0) vboxsf     (999)    61993 2022-12-01 09:27:15.000000 datatoolbox-0.5.4/datatoolbox/database.py
--rwxrwx---   0 root         (0) vboxsf     (999)     6730 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/greenhouse_gas_database.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3542 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/init_tools.py
--rwxrwx---   0 root         (0) vboxsf     (999)    21652 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/interfaces.py
--rwxrwx---   0 root         (0) vboxsf     (999)    10991 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/io_tools.py
--rwxrwx---   0 root         (0) vboxsf     (999)    41818 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/mapping.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2854 2022-12-01 09:27:15.000000 datatoolbox-0.5.4/datatoolbox/naming_convention.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3305 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/patches.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2175 2022-11-16 12:15:23.000000 datatoolbox-0.5.4/datatoolbox/pint_definitions.txt
--rwxrwx---   0 root         (0) vboxsf     (999)        0 2020-06-08 07:09:19.000000 datatoolbox-0.5.4/datatoolbox/relations.py
--rwxrwx---   0 root         (0) vboxsf     (999)    26522 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/sets.py
--rwxrwx---   0 root         (0) vboxsf     (999)        0 2020-06-08 07:09:19.000000 datatoolbox-0.5.4/datatoolbox/storage.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1632 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/templates.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-12-01 09:42:21.000000 datatoolbox-0.5.4/datatoolbox/tools/
--rwxrwx---   0 root         (0) vboxsf     (999)    16351 2021-04-19 11:31:45.000000 datatoolbox-0.5.4/datatoolbox/tools/CRF_extract_CA_2021.xlsx
--rwxrwx---   0 root         (0) vboxsf     (999)    28022 2021-02-02 15:17:26.000000 datatoolbox-0.5.4/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN
--rwxrwx---   0 root         (0) vboxsf     (999)    17445 2021-02-02 12:48:44.000000 datatoolbox-0.5.4/datatoolbox/tools/IEA_B2DS_4.SCEN
--rwxrwx---   0 root         (0) vboxsf     (999)    17375 2019-12-20 11:46:57.000000 datatoolbox-0.5.4/datatoolbox/tools/WEO_2019_test.SCEN
--rwxrwx---   0 root         (0) vboxsf     (999)      390 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/tools/__init__.py
--rwxrwx---   0 root         (0) vboxsf     (999)     4320 2022-11-17 09:58:39.000000 datatoolbox-0.5.4/datatoolbox/tools/conversion_to_v0.3.py
--rwxrwx---   0 root         (0) vboxsf     (999)    42729 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/tools/excel.py
--rwxrwx---   0 root         (0) vboxsf     (999)      370 2022-11-17 09:58:39.000000 datatoolbox-0.5.4/datatoolbox/tools/export_all.py
--rwxrwx---   0 root         (0) vboxsf     (999)     4441 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/tools/for_datatables.py
--rwxrwx---   0 root         (0) vboxsf     (999)     8132 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/tools/html.py
--rwxrwx---   0 root         (0) vboxsf     (999)      182 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/tools/install_support.py
--rwxrwx---   0 root         (0) vboxsf     (999)     7188 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/tools/kaya_idendentiy_decomposition.py
--rwxrwx---   0 root         (0) vboxsf     (999)     4283 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/tools/magicc6.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5931 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/tools/matplotlib.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3797 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/tools/pandas.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5533 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/tools/py_magicc_tools.py
--rwxrwx---   0 root         (0) vboxsf     (999)     7869 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/tools/pyam.py
--rwxrwx---   0 root         (0) vboxsf     (999)      965 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/tools/renaming_DB.py
--rwxrwx---   0 root         (0) vboxsf     (999)    84992 2019-08-14 10:26:08.000000 datatoolbox-0.5.4/datatoolbox/tools/run_MAGICC_startup_simple.xlsx
--rwxrwx---   0 root         (0) vboxsf     (999)     1830 2021-02-02 14:03:36.000000 datatoolbox-0.5.4/datatoolbox/tools/run_magicc6.m
--rwxrwx---   0 root         (0) vboxsf     (999)     1044 2022-11-17 09:58:40.000000 datatoolbox-0.5.4/datatoolbox/tools/statistics.py
--rwxrwx---   0 root         (0) vboxsf     (999)    61174 2021-06-03 14:06:07.000000 datatoolbox-0.5.4/datatoolbox/tools/test.docx
--rwxrwx---   0 root         (0) vboxsf     (999)     8625 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/tools/word.py
--rwxrwx---   0 root         (0) vboxsf     (999)     9607 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/tools/xarray.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-12-01 09:42:21.000000 datatoolbox-0.5.4/datatoolbox/tutorials/
--rwxrwx---   0 root         (0) vboxsf     (999)     2996 2022-05-25 07:15:53.000000 datatoolbox-0.5.4/datatoolbox/tutorials/00_search_find_and_access_data.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1019 2020-10-14 14:04:18.000000 datatoolbox-0.5.4/datatoolbox/tutorials/01_emission_comparison.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2096 2022-05-25 07:15:53.000000 datatoolbox-0.5.4/datatoolbox/tutorials/02_unit_conversion.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5685 2020-10-14 14:04:18.000000 datatoolbox-0.5.4/datatoolbox/tutorials/03_intermediate_example.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1416 2020-10-14 14:04:19.000000 datatoolbox-0.5.4/datatoolbox/tutorials/04_sources.py
--rwxrwx---   0 root         (0) vboxsf     (999)      382 2020-10-14 14:04:19.000000 datatoolbox-0.5.4/datatoolbox/tutorials/05_plot_source_content.py
--rwxrwx---   0 root         (0) vboxsf     (999)      734 2020-12-22 15:09:15.000000 datatoolbox-0.5.4/datatoolbox/tutorials/06_xarray_examples.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1142 2021-05-11 13:19:29.000000 datatoolbox-0.5.4/datatoolbox/tutorials/07_renewable_share_compuation.py
--rwxrwx---   0 root         (0) vboxsf     (999)      793 2021-05-11 12:59:38.000000 datatoolbox-0.5.4/datatoolbox/tutorials/08_low_carbon_fuel_computation.py
--rwxrwx---   0 root         (0) vboxsf     (999)   137631 2020-10-14 14:04:19.000000 datatoolbox-0.5.4/datatoolbox/tutorials/introduction_v1.ipynb
--rwxrwx---   0 root         (0) vboxsf     (999)     4631 2022-03-22 14:54:50.000000 datatoolbox-0.5.4/datatoolbox/tutorials/jump_start.py
--rwxrwx---   0 root         (0) vboxsf     (999)      300 2022-11-21 13:35:45.000000 datatoolbox-0.5.4/datatoolbox/units.py
--rwxrwx---   0 root         (0) vboxsf     (999)    43915 2022-11-22 09:50:19.000000 datatoolbox-0.5.4/datatoolbox/util.py
--rwxrwx---   0 root         (0) vboxsf     (999)      176 2022-12-01 09:42:21.000000 datatoolbox-0.5.4/datatoolbox/version.py
--rwxrwx---   0 root         (0) vboxsf     (999)      746 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/datatoolbox/workflows.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-12-01 09:42:21.000000 datatoolbox-0.5.4/datatoolbox.egg-info/
--rwxrwx---   0 root         (0) vboxsf     (999)     1037 2022-12-01 09:42:21.000000 datatoolbox-0.5.4/datatoolbox.egg-info/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (999)     3714 2022-12-01 09:42:21.000000 datatoolbox-0.5.4/datatoolbox.egg-info/SOURCES.txt
--rwxrwx---   0 root         (0) vboxsf     (999)        1 2022-12-01 09:42:21.000000 datatoolbox-0.5.4/datatoolbox.egg-info/dependency_links.txt
--rwxrwx---   0 root         (0) vboxsf     (999)      140 2022-12-01 09:42:21.000000 datatoolbox-0.5.4/datatoolbox.egg-info/requires.txt
--rwxrwx---   0 root         (0) vboxsf     (999)       12 2022-12-01 09:42:21.000000 datatoolbox-0.5.4/datatoolbox.egg-info/top_level.txt
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-12-01 09:42:21.000000 datatoolbox-0.5.4/doc/
--rwxrwx---   0 root         (0) vboxsf     (999)     7755 2020-10-14 14:04:19.000000 datatoolbox-0.5.4/doc/Makefile
--rwxrwx---   0 root         (0) vboxsf     (999)     9684 2020-12-22 15:09:15.000000 datatoolbox-0.5.4/doc/conf.py
--rwxrwx---   0 root         (0) vboxsf     (999)       79 2021-01-05 10:54:01.000000 datatoolbox-0.5.4/doc/core.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      149 2020-12-22 15:09:15.000000 datatoolbox-0.5.4/doc/data_structures.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      122 2021-01-11 16:19:59.000000 datatoolbox-0.5.4/doc/database.rst
--rwxrwx---   0 root         (0) vboxsf     (999)       91 2021-01-11 16:18:53.000000 datatoolbox-0.5.4/doc/database_database.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      130 2021-01-11 16:21:50.000000 datatoolbox-0.5.4/doc/database_gitrepomanager.rst
--rwxrwx---   0 root         (0) vboxsf     (999)       93 2021-01-11 16:03:03.000000 datatoolbox-0.5.4/doc/excel.rst
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-12-01 09:42:22.000000 datatoolbox-0.5.4/doc/figures/
--rwxrwx---   0 root         (0) vboxsf     (999)    21579 2020-11-09 13:08:35.000000 datatoolbox-0.5.4/doc/figures/ID_meta_data.svg
--rwxrwx---   0 root         (0) vboxsf     (999)    67463 2021-05-17 15:08:58.000000 datatoolbox-0.5.4/doc/figures/config_input.png
--rwxrwx---   0 root         (0) vboxsf     (999)     7157 2021-05-17 15:04:37.000000 datatoolbox-0.5.4/doc/first_steps.md
--rwxrwx---   0 root         (0) vboxsf     (999)      100 2020-12-22 15:09:15.000000 datatoolbox-0.5.4/doc/foo.rst_template
--rwxrwx---   0 root         (0) vboxsf     (999)       77 2020-12-22 15:09:15.000000 datatoolbox-0.5.4/doc/help.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      463 2021-01-11 16:06:28.000000 datatoolbox-0.5.4/doc/index.rst
--rwxrwx---   0 root         (0) vboxsf     (999)     1754 2021-05-21 08:03:28.000000 datatoolbox-0.5.4/doc/installation.md
--rwxrwx---   0 root         (0) vboxsf     (999)     1080 2020-12-22 15:09:15.000000 datatoolbox-0.5.4/doc/license.rst
--rwxrwx---   0 root         (0) vboxsf     (999)     7353 2020-10-14 14:04:19.000000 datatoolbox-0.5.4/doc/make.bat
--rwxrwx---   0 root         (0) vboxsf     (999)      103 2021-01-11 16:09:22.000000 datatoolbox-0.5.4/doc/matplotlib.rst
--rwxrwx---   0 root         (0) vboxsf     (999)       95 2021-01-11 16:10:43.000000 datatoolbox-0.5.4/doc/pandas.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      133 2021-01-11 16:20:57.000000 datatoolbox-0.5.4/doc/tools.rst
--rwxrwx---   0 root         (0) vboxsf     (999)       95 2021-01-11 16:09:13.000000 datatoolbox-0.5.4/doc/xarray.rst
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-12-01 09:42:22.000000 datatoolbox-0.5.4/documentation/
--rwxrwx---   0 root         (0) vboxsf     (999)     7761 2020-12-22 15:09:15.000000 datatoolbox-0.5.4/documentation/Datatoolbox - First steps.md
--rwxrwx---   0 root         (0) vboxsf     (999)      381 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/environment.yml
--rwxrwx---   0 root         (0) vboxsf     (999)      418 2020-10-14 14:04:19.000000 datatoolbox-0.5.4/make_proj.sh
--rwxrwx---   0 root         (0) vboxsf     (999)      558 2021-01-12 15:45:18.000000 datatoolbox-0.5.4/readthedocs.yml
--rwxrwx---   0 root         (0) vboxsf     (999)      215 2022-10-19 13:17:33.000000 datatoolbox-0.5.4/requirements.txt
--rwxrwx---   0 root         (0) vboxsf     (999)       38 2022-12-01 09:42:22.000000 datatoolbox-0.5.4/setup.cfg
--rwxrwx---   0 root         (0) vboxsf     (999)     1815 2022-10-19 13:17:33.000000 datatoolbox-0.5.4/setup.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-12-01 09:42:22.000000 datatoolbox-0.5.4/tests/
--rwxrwx---   0 root         (0) vboxsf     (999)     6986 2020-10-14 14:04:19.000000 datatoolbox-0.5.4/tests/test_calculations.py
--rwxrwx---   0 root         (0) vboxsf     (999)      696 2022-11-18 16:16:07.000000 datatoolbox-0.5.4/tests/test_converters.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2836 2022-11-21 11:08:31.000000 datatoolbox-0.5.4/tests/test_database.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1532 2022-10-19 13:17:33.000000 datatoolbox-0.5.4/tests/test_dataset.py
--rwxrwx---   0 root         (0) vboxsf     (999)     7741 2022-05-25 07:15:53.000000 datatoolbox-0.5.4/tests/test_datatable.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1063 2022-11-16 11:59:46.000000 datatoolbox-0.5.4/tests/test_io.py
--rwxrwx---   0 root         (0) vboxsf     (999)      390 2022-11-22 09:54:34.000000 datatoolbox-0.5.4/tests/test_linked_functions.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1527 2022-05-25 07:15:53.000000 datatoolbox-0.5.4/tests/test_pyam.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3570 2022-05-25 07:15:53.000000 datatoolbox-0.5.4/tests/test_tableset.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2610 2022-05-25 07:15:53.000000 datatoolbox-0.5.4/tests/test_tools.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1227 2022-11-21 13:23:54.000000 datatoolbox-0.5.4/tests/test_units.py
--rwxrwx---   0 root         (0) vboxsf     (999)      870 2020-10-14 14:04:19.000000 datatoolbox-0.5.4/tests/test_utilities.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2437 2022-10-19 13:17:33.000000 datatoolbox-0.5.4/tests/test_xarray.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2959 2022-05-25 07:15:53.000000 datatoolbox-0.5.4/tests/util_for_testing.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:42.000000 datatoolbox-0.5.5/
+-rwxrwx---   0 root         (0) vboxsf     (999)      159 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/.gitignore
+-rwxrwx---   0 root         (0) vboxsf     (999)      950 2022-10-19 13:17:33.000000 datatoolbox-0.5.5/.gitlab-ci.yml
+-rwxrwx---   0 root         (0) vboxsf     (999)      703 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/.travis.yml
+-rwxrwx---   0 root         (0) vboxsf     (999)     1073 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/LICENSE
+-rwxrwx---   0 root         (0) vboxsf     (999)     1037 2023-05-09 08:11:42.000000 datatoolbox-0.5.5/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (999)      771 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/README.md
+-rwxrwx---   0 root         (0) vboxsf     (999)     1225 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/appveyor.yml
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/ci/
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/ci/appveyor/
+-rwxrwx---   0 root         (0) vboxsf     (999)     3111 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/ci/appveyor/install.ps1
+-rwxrwx---   0 root         (0) vboxsf     (999)     1842 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/ci/appveyor/run_with_env.cmd
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/datatoolbox/
+-rwxrwx---   0 root         (0) vboxsf     (999)     4362 2023-05-04 12:41:44.000000 datatoolbox-0.5.5/datatoolbox/__init__.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    15385 2023-03-30 07:48:47.000000 datatoolbox-0.5.5/datatoolbox/admin.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     6655 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/config.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    18640 2022-12-01 09:27:15.000000 datatoolbox-0.5.5/datatoolbox/converters.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    11733 2022-12-19 11:17:33.000000 datatoolbox-0.5.5/datatoolbox/core.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/datatoolbox/data/
+-rwxrwx---   0 root         (0) vboxsf     (999)    15781 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/datatoolbox/data/GHG_alternative_naming.pkl
+-rwxrwx---   0 root         (0) vboxsf     (999)    13482 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/datatoolbox/data/GHG_properties_2019_CA.csv
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/
+-rwxrwx---   0 root         (0) vboxsf     (999)      286 2023-05-04 13:24:49.000000 datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/inventory.csv
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/mappings/
+-rwxrwx---   0 root         (0) vboxsf     (999)    10757 2023-05-04 13:24:48.000000 datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)     8466 2023-05-04 13:24:48.000000 datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)      999 2023-05-04 13:24:48.000000 datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)      161 2023-05-04 13:24:49.000000 datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/sources.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)    22865 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/datatoolbox/data/all.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)    14615 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/datatoolbox/data/compatible1_5_unfiltered.xlsx
+-rwxrwx---   0 root         (0) vboxsf     (999)    10757 2020-04-20 12:32:09.000000 datatoolbox-0.5.5/datatoolbox/data/continent.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)     8466 2021-09-15 15:48:16.000000 datatoolbox-0.5.5/datatoolbox/data/country_codes.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)     1711 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/datatoolbox/data/datashelf_contents.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)     2923 2021-12-16 12:32:58.000000 datatoolbox-0.5.5/datatoolbox/data/external_mappings.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      178 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/data/personal_template.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      999 2019-08-14 10:00:22.000000 datatoolbox-0.5.5/datatoolbox/data/regions.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)   237054 2023-04-28 11:35:43.000000 datatoolbox-0.5.5/datatoolbox/data_readers.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    68067 2023-05-04 07:37:43.000000 datatoolbox-0.5.5/datatoolbox/data_structures.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    63785 2023-05-09 07:33:41.000000 datatoolbox-0.5.5/datatoolbox/database.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     6730 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/greenhouse_gas_database.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3542 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/init_tools.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    21652 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/interfaces.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    10991 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/io_tools.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    41818 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/mapping.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2854 2022-12-01 09:27:15.000000 datatoolbox-0.5.5/datatoolbox/naming_convention.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3305 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/patches.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2175 2022-11-16 12:15:23.000000 datatoolbox-0.5.5/datatoolbox/pint_definitions.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)        0 2020-06-08 07:09:19.000000 datatoolbox-0.5.5/datatoolbox/relations.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    26527 2023-04-05 07:52:48.000000 datatoolbox-0.5.5/datatoolbox/sets.py
+-rwxrwx---   0 root         (0) vboxsf     (999)        0 2020-06-08 07:09:19.000000 datatoolbox-0.5.5/datatoolbox/storage.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1632 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/templates.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/datatoolbox/tools/
+-rwxrwx---   0 root         (0) vboxsf     (999)    16351 2021-04-19 11:31:45.000000 datatoolbox-0.5.5/datatoolbox/tools/CRF_extract_CA_2021.xlsx
+-rwxrwx---   0 root         (0) vboxsf     (999)    28022 2021-02-02 15:17:26.000000 datatoolbox-0.5.5/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN
+-rwxrwx---   0 root         (0) vboxsf     (999)    17445 2021-02-02 12:48:44.000000 datatoolbox-0.5.5/datatoolbox/tools/IEA_B2DS_4.SCEN
+-rwxrwx---   0 root         (0) vboxsf     (999)    17375 2019-12-20 11:46:57.000000 datatoolbox-0.5.5/datatoolbox/tools/WEO_2019_test.SCEN
+-rwxrwx---   0 root         (0) vboxsf     (999)      390 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/__init__.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     4320 2022-11-17 09:58:39.000000 datatoolbox-0.5.5/datatoolbox/tools/conversion_to_v0.3.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    42729 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/excel.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      370 2022-11-17 09:58:39.000000 datatoolbox-0.5.5/datatoolbox/tools/export_all.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     4441 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/for_datatables.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     8132 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/html.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      182 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/install_support.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     7188 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/kaya_idendentiy_decomposition.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     4283 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/magicc6.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5931 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/matplotlib.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3797 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/pandas.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5533 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/py_magicc_tools.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     7869 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/pyam.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      965 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/renaming_DB.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    84992 2019-08-14 10:26:08.000000 datatoolbox-0.5.5/datatoolbox/tools/run_MAGICC_startup_simple.xlsx
+-rwxrwx---   0 root         (0) vboxsf     (999)     1830 2021-02-02 14:03:36.000000 datatoolbox-0.5.5/datatoolbox/tools/run_magicc6.m
+-rwxrwx---   0 root         (0) vboxsf     (999)     1044 2022-11-17 09:58:40.000000 datatoolbox-0.5.5/datatoolbox/tools/statistics.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    61174 2021-06-03 14:06:07.000000 datatoolbox-0.5.5/datatoolbox/tools/test.docx
+-rwxrwx---   0 root         (0) vboxsf     (999)     8625 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/word.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     9617 2023-03-30 13:29:22.000000 datatoolbox-0.5.5/datatoolbox/tools/xarray.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/datatoolbox/tutorials/
+-rwxrwx---   0 root         (0) vboxsf     (999)     2996 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/datatoolbox/tutorials/00_search_find_and_access_data.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1019 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/datatoolbox/tutorials/01_emission_comparison.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2096 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/datatoolbox/tutorials/02_unit_conversion.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5685 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/datatoolbox/tutorials/03_intermediate_example.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1416 2020-10-14 14:04:19.000000 datatoolbox-0.5.5/datatoolbox/tutorials/04_sources.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      382 2020-10-14 14:04:19.000000 datatoolbox-0.5.5/datatoolbox/tutorials/05_plot_source_content.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      734 2020-12-22 15:09:15.000000 datatoolbox-0.5.5/datatoolbox/tutorials/06_xarray_examples.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1142 2021-05-11 13:19:29.000000 datatoolbox-0.5.5/datatoolbox/tutorials/07_renewable_share_compuation.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      793 2021-05-11 12:59:38.000000 datatoolbox-0.5.5/datatoolbox/tutorials/08_low_carbon_fuel_computation.py
+-rwxrwx---   0 root         (0) vboxsf     (999)   137631 2020-10-14 14:04:19.000000 datatoolbox-0.5.5/datatoolbox/tutorials/introduction_v1.ipynb
+-rwxrwx---   0 root         (0) vboxsf     (999)     4631 2022-03-22 14:54:50.000000 datatoolbox-0.5.5/datatoolbox/tutorials/jump_start.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      300 2022-11-21 13:35:45.000000 datatoolbox-0.5.5/datatoolbox/units.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    43915 2022-11-22 09:50:19.000000 datatoolbox-0.5.5/datatoolbox/util.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      176 2023-05-09 08:11:40.000000 datatoolbox-0.5.5/datatoolbox/version.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      746 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/workflows.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/datatoolbox.egg-info/
+-rwxrwx---   0 root         (0) vboxsf     (999)     1037 2023-05-09 08:11:40.000000 datatoolbox-0.5.5/datatoolbox.egg-info/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (999)     3714 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/datatoolbox.egg-info/SOURCES.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)        1 2023-05-09 08:11:40.000000 datatoolbox-0.5.5/datatoolbox.egg-info/dependency_links.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)      149 2023-05-09 08:11:40.000000 datatoolbox-0.5.5/datatoolbox.egg-info/requires.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)       12 2023-05-09 08:11:40.000000 datatoolbox-0.5.5/datatoolbox.egg-info/top_level.txt
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:42.000000 datatoolbox-0.5.5/doc/
+-rwxrwx---   0 root         (0) vboxsf     (999)     7755 2020-10-14 14:04:19.000000 datatoolbox-0.5.5/doc/Makefile
+-rwxrwx---   0 root         (0) vboxsf     (999)     9684 2020-12-22 15:09:15.000000 datatoolbox-0.5.5/doc/conf.py
+-rwxrwx---   0 root         (0) vboxsf     (999)       79 2021-01-05 10:54:01.000000 datatoolbox-0.5.5/doc/core.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      149 2020-12-22 15:09:15.000000 datatoolbox-0.5.5/doc/data_structures.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      122 2021-01-11 16:19:59.000000 datatoolbox-0.5.5/doc/database.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)       91 2021-01-11 16:18:53.000000 datatoolbox-0.5.5/doc/database_database.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      130 2021-01-11 16:21:50.000000 datatoolbox-0.5.5/doc/database_gitrepomanager.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)       93 2021-01-11 16:03:03.000000 datatoolbox-0.5.5/doc/excel.rst
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:42.000000 datatoolbox-0.5.5/doc/figures/
+-rwxrwx---   0 root         (0) vboxsf     (999)    21579 2020-11-09 13:08:35.000000 datatoolbox-0.5.5/doc/figures/ID_meta_data.svg
+-rwxrwx---   0 root         (0) vboxsf     (999)    67463 2021-05-17 15:08:58.000000 datatoolbox-0.5.5/doc/figures/config_input.png
+-rwxrwx---   0 root         (0) vboxsf     (999)     7157 2021-05-17 15:04:37.000000 datatoolbox-0.5.5/doc/first_steps.md
+-rwxrwx---   0 root         (0) vboxsf     (999)      100 2020-12-22 15:09:15.000000 datatoolbox-0.5.5/doc/foo.rst_template
+-rwxrwx---   0 root         (0) vboxsf     (999)       77 2020-12-22 15:09:15.000000 datatoolbox-0.5.5/doc/help.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      463 2021-01-11 16:06:28.000000 datatoolbox-0.5.5/doc/index.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)     1754 2021-05-21 08:03:28.000000 datatoolbox-0.5.5/doc/installation.md
+-rwxrwx---   0 root         (0) vboxsf     (999)     1080 2020-12-22 15:09:15.000000 datatoolbox-0.5.5/doc/license.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)     7353 2020-10-14 14:04:19.000000 datatoolbox-0.5.5/doc/make.bat
+-rwxrwx---   0 root         (0) vboxsf     (999)      103 2021-01-11 16:09:22.000000 datatoolbox-0.5.5/doc/matplotlib.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)       95 2021-01-11 16:10:43.000000 datatoolbox-0.5.5/doc/pandas.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      133 2021-01-11 16:20:57.000000 datatoolbox-0.5.5/doc/tools.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)       95 2021-01-11 16:09:13.000000 datatoolbox-0.5.5/doc/xarray.rst
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:42.000000 datatoolbox-0.5.5/documentation/
+-rwxrwx---   0 root         (0) vboxsf     (999)     7761 2020-12-22 15:09:15.000000 datatoolbox-0.5.5/documentation/Datatoolbox - First steps.md
+-rwxrwx---   0 root         (0) vboxsf     (999)      381 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/environment.yml
+-rwxrwx---   0 root         (0) vboxsf     (999)      418 2020-10-14 14:04:19.000000 datatoolbox-0.5.5/make_proj.sh
+-rwxrwx---   0 root         (0) vboxsf     (999)      558 2021-01-12 15:45:18.000000 datatoolbox-0.5.5/readthedocs.yml
+-rwxrwx---   0 root         (0) vboxsf     (999)      215 2022-10-19 13:17:33.000000 datatoolbox-0.5.5/requirements.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)       38 2023-05-09 08:11:42.000000 datatoolbox-0.5.5/setup.cfg
+-rwxrwx---   0 root         (0) vboxsf     (999)     1839 2023-05-03 11:16:28.000000 datatoolbox-0.5.5/setup.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:42.000000 datatoolbox-0.5.5/tests/
+-rwxrwx---   0 root         (0) vboxsf     (999)     7292 2022-12-19 11:29:58.000000 datatoolbox-0.5.5/tests/test_calculations.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      696 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/tests/test_converters.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2836 2022-11-21 11:08:31.000000 datatoolbox-0.5.5/tests/test_database.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1640 2023-03-30 13:32:13.000000 datatoolbox-0.5.5/tests/test_dataset.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     7741 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/tests/test_datatable.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1063 2022-11-16 11:59:46.000000 datatoolbox-0.5.5/tests/test_io.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      390 2022-11-22 09:54:34.000000 datatoolbox-0.5.5/tests/test_linked_functions.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1563 2023-05-04 07:49:24.000000 datatoolbox-0.5.5/tests/test_pyam.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3570 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/tests/test_tableset.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2610 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/tests/test_tools.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1227 2022-11-21 13:23:54.000000 datatoolbox-0.5.5/tests/test_units.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      870 2020-10-14 14:04:19.000000 datatoolbox-0.5.5/tests/test_utilities.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2437 2022-10-19 13:17:33.000000 datatoolbox-0.5.5/tests/test_xarray.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2959 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/tests/util_for_testing.py
```

### Comparing `datatoolbox-0.5.4/.gitlab-ci.yml` & `datatoolbox-0.5.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/.travis.yml` & `datatoolbox-0.5.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/LICENSE` & `datatoolbox-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/PKG-INFO` & `datatoolbox-0.5.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatoolbox
-Version: 0.5.4
+Version: 0.5.5
 Summary: The Python Data Toolbox
 Home-page: https://gitlab.com/climateanalytics/datatoolbox
 Author: Andreas Geiges
 Author-email: a.geiges@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `datatoolbox-0.5.4/README.md` & `datatoolbox-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/appveyor.yml` & `datatoolbox-0.5.5/appveyor.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/ci/appveyor/install.ps1` & `datatoolbox-0.5.5/ci/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/ci/appveyor/run_with_env.cmd` & `datatoolbox-0.5.5/ci/appveyor/run_with_env.cmd`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/__init__.py` & `datatoolbox-0.5.5/datatoolbox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,16 @@
     import_new_source_from_remote = core.DB.importSourceFromRemote
     export_new_source_to_remote = core.DB.exportSourceToRemote
     remove_source = core.DB.removeSource
     push_source_to_remote = core.DB.gitManager.push_to_remote_datashelf
     pull_source_from_remote = core.DB.pull_update_from_remote
 
     #show available remote data sources
-    available_remote_data = core.DB.remote_sourceInfo
+    remote_sourceInfo = core.DB.remote_sourceInfo
+    available_remote_data_updates = core.DB.gitManager.available_remote_data_updates
     
 #%% TOOLS
 # Tools related to packages
 import datatoolbox.tools as tools
 from .tools import pandas as pd
 from .tools import matplotlib as plt
 from .tools import xarray as xr
@@ -114,15 +115,15 @@
 from .tools import pyam as pyam
 
 insertDataIntoExcelFile = io.insertDataIntoExcelFile
 
 
 #%% UNITS
 from . import units
-
+conversionFactor = units.conversionFactor
 
 # get country ISO code
 getCountryISO = util.getCountryISO
```

### Comparing `datatoolbox-0.5.4/datatoolbox/admin.py` & `datatoolbox-0.5.5/datatoolbox/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 import pandas as pd
 import platform
 import git
 import os
 
 OS = platform.system()
 # from . import config
-# from datatoolbox import config
+from datatoolbox import config
 import git
 import shutil
 import datatoolbox as dt
-
+import subprocess
 
 def create_empty_datashelf(pathToDataself, force_new=False):
     """
     User funciton to create a empty datashelf
 
     Parameters
     ----------
@@ -410,14 +410,23 @@
 
     dt.isAvailable = dt.core.DB._tableExists
     dt.validate_ID = dt.core.DB.validate_ID
     dt.sourceInfo = dt.core.DB.sourceInfo
 
     dt.updateExcelInput = dt.core.DB.updateExcelInput
 
+def open_config_file():
+    filepath = os.path.join(config.CONFIG_DIR,'personal.py')#
+   
+    if platform.system() == 'Darwin':       # macOS
+        subprocess.run(['open', filepath], check=True)
+    elif platform.system() == 'Windows':    # Windows
+        os.startfile(filepath)
+    else:                                   # linux variants
+        subprocess.call(('xdg-open', filepath))
 
 def set_autoload_source(boolean):
     """
     Admin funtion to change permanently the personal configuration "AUTOLOAD_SOURCES".
     If set to True and if the database is connecte to a remote git repository,
     datatoolbox is try to import missing sources if a table is loaded that is locally
     not available.
```

### Comparing `datatoolbox-0.5.4/datatoolbox/config.py` & `datatoolbox-0.5.5/datatoolbox/config.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/converters.py` & `datatoolbox-0.5.5/datatoolbox/converters.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/core.py` & `datatoolbox-0.5.5/datatoolbox/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,14 +294,17 @@
 
     Returns
     -------
     unit : pint unit
     """
     # if not isinstance(string, str):
     #     string = str(string)
+    # capture if already is pint unit
+    if isinstance(string, pint.Unit):
+        string = str(string)
     if string is None:
         string = ''
     else:
         string = string.replace('$', 'USD').replace('€', 'EUR').replace('%', 'percent')
     return ur(string)
```

### Comparing `datatoolbox-0.5.4/datatoolbox/data/GHG_alternative_naming.pkl` & `datatoolbox-0.5.5/datatoolbox/data/GHG_alternative_naming.pkl`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/data/GHG_properties_2019_CA.csv` & `datatoolbox-0.5.5/datatoolbox/data/GHG_properties_2019_CA.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv` & `datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv` & `datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv` & `datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/data/all.csv` & `datatoolbox-0.5.5/datatoolbox/data/all.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/data/compatible1_5_unfiltered.xlsx` & `datatoolbox-0.5.5/datatoolbox/data/compatible1_5_unfiltered.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/data/continent.csv` & `datatoolbox-0.5.5/datatoolbox/data/continent.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/data/country_codes.csv` & `datatoolbox-0.5.5/datatoolbox/data/country_codes.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/data/datashelf_contents.csv` & `datatoolbox-0.5.5/datatoolbox/data/datashelf_contents.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/data/external_mappings.py` & `datatoolbox-0.5.5/datatoolbox/data/external_mappings.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/data/regions.csv` & `datatoolbox-0.5.5/datatoolbox/data/regions.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/data_readers.py` & `datatoolbox-0.5.5/datatoolbox/data_readers.py`

 * *Files 1% similar despite different names*

```diff
@@ -9751,5061 +9751,5066 @@
 00026160: 7365 7475 702e 534f 5552 4345 5f50 4154  setup.SOURCE_PAT
 00026170: 4829 0a20 2020 2020 2020 2020 2020 2069  H).            i
 00026180: 6620 6f73 2e70 6174 682e 6973 6469 7228  f os.path.isdir(
 00026190: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
 000261a0: 662e 7365 7475 702e 534f 5552 4345 5f50  f.setup.SOURCE_P
 000261b0: 4154 482c 206e 616d 6529 290a 2020 2020  ATH, name)).    
 000261c0: 2020 2020 5d0a 2020 2020 2020 2020 666f      ].        fo
-000261d0: 7220 666f 6c64 6572 2069 6e20 666f 6c64  r folder in fold
-000261e0: 6572 4c69 7374 3a0a 2020 2020 2020 2020  erList:.        
-000261f0: 2020 2020 636f 4953 4f20 3d20 666f 6c64      coISO = fold
-00026200: 6572 0a20 2020 2020 2020 2020 2020 2063  er.            c
-00026210: 6f75 6e74 7279 5061 7468 203d 206f 732e  ountryPath = os.
-00026220: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e73  path.join(self.s
-00026230: 6574 7570 2e53 4f55 5243 455f 5041 5448  etup.SOURCE_PATH
-00026240: 2c20 666f 6c64 6572 290a 2020 2020 2020  , folder).      
-00026250: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00026260: 2020 2020 2020 2020 2020 2063 6f75 6e74             count
-00026270: 7279 4c69 7374 2e61 7070 656e 6428 6474  ryList.append(dt
-00026280: 2e6d 6170 702e 636f 756e 7472 6965 732e  .mapp.countries.
-00026290: 636f 6465 732e 6c6f 635b 636f 4953 4f2c  codes.loc[coISO,
-000262a0: 2027 6e61 6d65 275d 290a 2020 2020 2020   'name']).      
-000262b0: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-000262c0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000262d0: 756e 7472 794c 6973 742e 6170 7065 6e64  untryList.append
-000262e0: 2863 6f49 534f 290a 2020 2020 2020 2020  (coISO).        
-000262f0: 2020 2020 7072 696e 7428 636f 4953 4f29      print(coISO)
-00026300: 0a0a 2020 2020 2020 2020 2020 2020 6669  ..            fi
-00026310: 6c65 4c69 7374 203d 206f 732e 6c69 7374  leList = os.list
-00026320: 6469 7228 636f 756e 7472 7950 6174 6829  dir(countryPath)
-00026330: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00026340: 2066 696c 654e 616d 6520 696e 2066 696c   fileName in fil
-00026350: 654c 6973 743a 0a20 2020 2020 2020 2020  eList:.         
-00026360: 2020 2020 2020 2079 6561 7220 3d20 696e         year = in
-00026370: 7428 6669 6c65 4e61 6d65 2e73 706c 6974  t(fileName.split
-00026380: 2827 5f27 295b 325d 290a 2020 2020 2020  ('_')[2]).      
-00026390: 2020 2020 2020 2020 2020 7365 7475 7020            setup 
-000263a0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-000263b0: 2020 2020 2020 2020 2073 6574 7570 5b27           setup['
-000263c0: 6669 6c65 5061 7468 275d 203d 2063 6f75  filePath'] = cou
-000263d0: 6e74 7279 5061 7468 0a20 2020 2020 2020  ntryPath.       
-000263e0: 2020 2020 2020 2020 2073 6574 7570 5b27           setup['
-000263f0: 6669 6c65 4e61 6d65 275d 203d 2066 696c  fileName'] = fil
-00026400: 654e 616d 650a 2020 2020 2020 2020 2020  eName.          
-00026410: 2020 2020 2020 7365 7475 705b 2773 6865        setup['she
-00026420: 6574 4e61 6d65 275d 203d 2027 5375 6d6d  etName'] = 'Summ
-00026430: 6172 7932 270a 0a20 2020 2020 2020 2020  ary2'..         
-00026440: 2020 2020 2020 2072 6561 6465 7220 3d20         reader = 
-00026450: 6474 2e69 6f2e 4578 6365 6c52 6561 6465  dt.io.ExcelReade
-00026460: 7228 7365 7475 7029 0a0a 2020 2020 2020  r(setup)..      
-00026470: 2020 2020 2020 2020 2020 666f 7220 7365            for se
-00026480: 6374 6f72 2069 6e20 7365 6c66 2e6d 6170  ctor in self.map
-00026490: 7069 6e67 4469 6374 5b27 7365 6374 6f72  pingDict['sector
-000264a0: 7327 5d3a 0a20 2020 2020 2020 2020 2020  s']:.           
-000264b0: 2020 2020 2020 2020 2066 6f72 2067 6173           for gas
-000264c0: 2069 6e20 7365 6c66 2e6d 6170 7069 6e67   in self.mapping
-000264d0: 4469 6374 5b27 6761 7365 7327 5d3a 0a20  Dict['gases']:. 
-000264e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000264f0: 2020 2020 2020 2076 6172 6961 626c 6520         variable 
-00026500: 3d20 2745 6d69 7373 696f 6e73 7c27 202b  = 'Emissions|' +
-00026510: 2067 6173 202b 2027 7c27 202b 2073 6563   gas + '|' + sec
-00026520: 746f 720a 0a20 2020 2020 2020 2020 2020  tor..           
-00026530: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00026540: 7661 7269 6162 6c65 206e 6f74 2069 6e20  variable not in 
-00026550: 6461 7461 5461 626c 6573 2e6b 6579 7328  dataTables.keys(
-00026560: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00026570: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00026580: 2063 7265 6174 6520 7461 626c 650a 2020   create table.  
-00026590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000265a0: 2020 2020 2020 2020 2020 6d65 7461 203d            meta =
-000265b0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000261d0: 7220 666f 6c64 6572 2069 6e20 7471 646d  r folder in tqdm
+000261e0: 2866 6f6c 6465 724c 6973 7429 3a0a 2020  (folderList):.  
+000261f0: 2020 2020 2020 2020 2020 636f 4953 4f20            coISO 
+00026200: 3d20 666f 6c64 6572 0a20 2020 2020 2020  = folder.       
+00026210: 2020 2020 2063 6f75 6e74 7279 5061 7468       countryPath
+00026220: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00026230: 7365 6c66 2e73 6574 7570 2e53 4f55 5243  self.setup.SOURC
+00026240: 455f 5041 5448 2c20 666f 6c64 6572 290a  E_PATH, folder).
+00026250: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00026260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00026270: 2063 6f75 6e74 7279 4c69 7374 2e61 7070   countryList.app
+00026280: 656e 6428 6474 2e6d 6170 702e 636f 756e  end(dt.mapp.coun
+00026290: 7472 6965 732e 636f 6465 732e 6c6f 635b  tries.codes.loc[
+000262a0: 636f 4953 4f2c 2027 6e61 6d65 275d 290a  coISO, 'name']).
+000262b0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+000262c0: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
+000262d0: 2020 2020 636f 756e 7472 794c 6973 742e      countryList.
+000262e0: 6170 7065 6e64 2863 6f49 534f 290a 2020  append(coISO).  
+000262f0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00026300: 636f 4953 4f29 0a0a 2020 2020 2020 2020  coISO)..        
+00026310: 2020 2020 6669 6c65 4c69 7374 203d 206f      fileList = o
+00026320: 732e 6c69 7374 6469 7228 636f 756e 7472  s.listdir(countr
+00026330: 7950 6174 6829 0a20 2020 2020 2020 2020  yPath).         
+00026340: 2020 2066 6f72 2066 696c 654e 616d 6520     for fileName 
+00026350: 696e 2066 696c 654c 6973 743a 0a20 2020  in fileList:.   
+00026360: 2020 2020 2020 2020 2020 2020 2079 6561               yea
+00026370: 7220 3d20 696e 7428 6669 6c65 4e61 6d65  r = int(fileName
+00026380: 2e73 706c 6974 2827 5f27 295b 325d 290a  .split('_')[2]).
+00026390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000263a0: 7365 7475 7020 3d20 6469 6374 2829 0a20  setup = dict(). 
+000263b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000263c0: 6574 7570 5b27 6669 6c65 5061 7468 275d  etup['filePath']
+000263d0: 203d 2063 6f75 6e74 7279 5061 7468 0a20   = countryPath. 
+000263e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000263f0: 6574 7570 5b27 6669 6c65 4e61 6d65 275d  etup['fileName']
+00026400: 203d 2066 696c 654e 616d 650a 2020 2020   = fileName.    
+00026410: 2020 2020 2020 2020 2020 2020 7365 7475              setu
+00026420: 705b 2773 6865 6574 4e61 6d65 275d 203d  p['sheetName'] =
+00026430: 2027 5375 6d6d 6172 7932 270a 0a20 2020   'Summary2'..   
+00026440: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+00026450: 6465 7220 3d20 6474 2e69 6f2e 4578 6365  der = dt.io.Exce
+00026460: 6c52 6561 6465 7228 7365 7475 7029 0a0a  lReader(setup)..
+00026470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026480: 666f 7220 7365 6374 6f72 2069 6e20 7365  for sector in se
+00026490: 6c66 2e6d 6170 7069 6e67 4469 6374 5b27  lf.mappingDict['
+000264a0: 7365 6374 6f72 7327 5d3a 0a20 2020 2020  sectors']:.     
+000264b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000264c0: 6f72 2067 6173 2069 6e20 7365 6c66 2e6d  or gas in self.m
+000264d0: 6170 7069 6e67 4469 6374 5b27 6761 7365  appingDict['gase
+000264e0: 7327 5d3a 0a20 2020 2020 2020 2020 2020  s']:.           
+000264f0: 2020 2020 2020 2020 2020 2020 2076 6172               var
+00026500: 6961 626c 6520 3d20 2745 6d69 7373 696f  iable = 'Emissio
+00026510: 6e73 7c27 202b 2067 6173 202b 2027 7c27  ns|' + gas + '|'
+00026520: 202b 2073 6563 746f 720a 0a20 2020 2020   + sector..     
+00026530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026540: 2020 2069 6620 7661 7269 6162 6c65 206e     if variable n
+00026550: 6f74 2069 6e20 6461 7461 5461 626c 6573  ot in dataTables
+00026560: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
+00026570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026580: 2020 2020 2023 2063 7265 6174 6520 7461       # create ta
+00026590: 626c 650a 2020 2020 2020 2020 2020 2020  ble.            
+000265a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000265b0: 6d65 7461 203d 2064 6963 7428 290a 2020  meta = dict().  
 000265c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000265d0: 2020 2020 6d65 7461 5b27 656e 7469 7479      meta['entity
-000265e0: 275d 203d 2027 456d 6973 7369 6f6e 737c  '] = 'Emissions|
-000265f0: 2720 2b20 6761 730a 2020 2020 2020 2020  ' + gas.        
+000265d0: 2020 2020 2020 2020 2020 6d65 7461 5b27            meta['
+000265e0: 656e 7469 7479 275d 203d 2027 456d 6973  entity'] = 'Emis
+000265f0: 7369 6f6e 737c 2720 2b20 6761 730a 2020  sions|' + gas.  
 00026600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026610: 2020 2020 6d65 7461 5b27 6361 7465 676f      meta['catego
-00026620: 7279 275d 203d 2073 6563 746f 720a 2020  ry'] = sector.  
-00026630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026640: 2020 2020 2020 2020 2020 6d65 7461 5b27            meta['
-00026650: 7363 656e 6172 696f 275d 203d 2027 4869  scenario'] = 'Hi
-00026660: 7374 6f72 6963 7c63 6f75 6e74 7279 5f72  storic|country_r
-00026670: 6570 6f72 7465 6427 0a20 2020 2020 2020  eported'.       
+00026610: 2020 2020 2020 2020 2020 6d65 7461 5b27            meta['
+00026620: 6361 7465 676f 7279 275d 203d 2073 6563  category'] = sec
+00026630: 746f 720a 2020 2020 2020 2020 2020 2020  tor.            
+00026640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026650: 6d65 7461 5b27 7363 656e 6172 696f 275d  meta['scenario']
+00026660: 203d 2027 4869 7374 6f72 6963 7c63 6f75   = 'Historic|cou
+00026670: 6e74 7279 5f72 6570 6f72 7465 6427 0a20  ntry_reported'. 
 00026680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026690: 2020 2020 206d 6574 615b 2773 6f75 7263       meta['sourc
-000266a0: 6527 5d20 3d20 7365 6c66 2e73 6574 7570  e'] = self.setup
-000266b0: 2e53 4f55 5243 455f 4944 0a20 2020 2020  .SOURCE_ID.     
-000266c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000266d0: 2020 2020 2020 206d 6574 615b 2775 6e69         meta['uni
-000266e0: 7427 5d20 3d20 274d 7443 4f32 6571 270a  t'] = 'MtCO2eq'.
-000266f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026700: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00026710: 5461 626c 6573 5b76 6172 6961 626c 655d  Tables[variable]
-00026720: 203d 2064 742e 4461 7461 7461 626c 6528   = dt.Datatable(
-00026730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00026690: 2020 2020 2020 2020 2020 206d 6574 615b             meta[
+000266a0: 2773 6f75 7263 6527 5d20 3d20 7365 6c66  'source'] = self
+000266b0: 2e73 6574 7570 2e53 4f55 5243 455f 4944  .setup.SOURCE_ID
+000266c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000266d0: 2020 2020 2020 2020 2020 2020 206d 6574               met
+000266e0: 615b 2775 6e69 7427 5d20 3d20 274d 7443  a['unit'] = 'MtC
+000266f0: 4f32 6571 270a 2020 2020 2020 2020 2020  O2eq'.          
+00026700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026710: 2020 6461 7461 5461 626c 6573 5b76 6172    dataTables[var
+00026720: 6961 626c 655d 203d 2064 742e 4461 7461  iable] = dt.Data
+00026730: 7461 626c 6528 0a20 2020 2020 2020 2020  table(.         
 00026740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026750: 2063 6f6c 756d 6e73 3d6c 6973 7428 7261   columns=list(ra
-00026760: 6e67 6528 3139 3930 2c20 3230 3137 2929  nge(1990, 2017))
-00026770: 2c20 6d65 7461 3d6d 6574 610a 2020 2020  , meta=meta.    
-00026780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026790: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00026750: 2020 2020 2020 2063 6f6c 756d 6e73 3d6c         columns=l
+00026760: 6973 7428 7261 6e67 6528 3139 3930 2c20  ist(range(1990, 
+00026770: 3230 3137 2929 2c20 6d65 7461 3d6d 6574  2017)), meta=met
+00026780: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
+00026790: 2020 2020 2020 2020 2020 2020 2020 290a                ).
 000267a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000267b0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000267b0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
 000267c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000267d0: 2020 2064 6174 6154 6162 6c65 735b 7661     dataTables[va
-000267e0: 7269 6162 6c65 5d2e 6c6f 635b 636f 4953  riable].loc[coIS
-000267f0: 4f2c 2079 6561 725d 203d 2028 0a20 2020  O, year] = (.   
-00026800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026810: 2020 2020 2020 2020 2020 2020 2072 6561               rea
-00026820: 6465 722e 6761 7468 6572 5661 6c75 6528  der.gatherValue(
-00026830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000267d0: 2020 2020 2020 2020 2064 6174 6154 6162           dataTab
+000267e0: 6c65 735b 7661 7269 6162 6c65 5d2e 6c6f  les[variable].lo
+000267f0: 635b 636f 4953 4f2c 2079 6561 725d 203d  c[coISO, year] =
+00026800: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00026810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026820: 2020 2072 6561 6465 722e 6761 7468 6572     reader.gather
+00026830: 5661 6c75 6528 0a20 2020 2020 2020 2020  Value(.         
 00026840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026850: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
-00026860: 6744 6963 745b 2767 6173 6573 275d 5b67  gDict['gases'][g
-00026870: 6173 5d0a 2020 2020 2020 2020 2020 2020  as].            
+00026850: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00026860: 6d61 7070 696e 6744 6963 745b 2767 6173  mappingDict['gas
+00026870: 6573 275d 5b67 6173 5d0a 2020 2020 2020  es'][gas].      
 00026880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026890: 2020 2020 2020 2020 2b20 7365 6c66 2e6d          + self.m
-000268a0: 6170 7069 6e67 4469 6374 5b27 7365 6374  appingDict['sect
-000268b0: 6f72 7327 5d5b 7365 6374 6f72 5d0a 2020  ors'][sector].  
-000268c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000268d0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-000268e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026890: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+000268a0: 7365 6c66 2e6d 6170 7069 6e67 4469 6374  self.mappingDict
+000268b0: 5b27 7365 6374 6f72 7327 5d5b 7365 6374  ['sectors'][sect
+000268c0: 6f72 5d0a 2020 2020 2020 2020 2020 2020  or].            
+000268d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000268e0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
 000268f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026900: 2f20 3130 3030 0a20 2020 2020 2020 2020  / 1000.         
+00026900: 2020 2020 2020 2f20 3130 3030 0a20 2020        / 1000.   
 00026910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026920: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00026930: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00026940: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
+00026920: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00026930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026940: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
 00026950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026960: 2070 6173 730a 0a20 2020 2020 2020 2069   pass..        i
-00026970: 6d70 6f72 7420 636f 7079 0a0a 2020 2020  mport copy..    
-00026980: 2020 2020 666f 7220 6761 7320 696e 2073      for gas in s
-00026990: 656c 662e 6d61 7070 696e 6744 6963 745b  elf.mappingDict[
-000269a0: 2767 6173 6573 275d 3a0a 2020 2020 2020  'gases']:.      
-000269b0: 2020 2020 2020 6966 2027 456d 6973 7369        if 'Emissi
-000269c0: 6f6e 737c 2720 2b20 6761 7320 2b20 277c  ons|' + gas + '|
-000269d0: 4c55 4c55 4346 2720 696e 2064 6174 6154  LULUCF' in dataT
-000269e0: 6162 6c65 732e 6b65 7973 2829 3a0a 2020  ables.keys():.  
-000269f0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00026a00: 7461 5461 626c 6573 5b27 456d 6973 7369  taTables['Emissi
-00026a10: 6f6e 737c 2720 2b20 6761 7320 2b20 277c  ons|' + gas + '|
-00026a20: 4950 434d 3045 4c27 5d20 3d20 280a 2020  IPCM0EL'] = (.  
-00026a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026a40: 2020 6461 7461 5461 626c 6573 5b27 456d    dataTables['Em
-00026a50: 6973 7369 6f6e 737c 2720 2b20 6761 7320  issions|' + gas 
-00026a60: 2b20 277c 4950 4330 275d 0a20 2020 2020  + '|IPC0'].     
-00026a70: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-00026a80: 2064 6174 6154 6162 6c65 735b 2745 6d69   dataTables['Emi
-00026a90: 7373 696f 6e73 7c27 202b 2067 6173 202b  ssions|' + gas +
-00026aa0: 2027 7c4c 554c 5543 4627 5d0a 2020 2020   '|LULUCF'].    
-00026ab0: 2020 2020 2020 2020 2020 2020 2920 2023              )  #
-00026ac0: 206e 6174 696f 6e61 6c20 746f 7461 6c20   national total 
-00026ad0: 6578 636c 7564 696e 6720 6c75 6c75 6366  excluding lulucf
-00026ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026af0: 2064 6174 6154 6162 6c65 735b 2745 6d69   dataTables['Emi
-00026b00: 7373 696f 6e73 7c27 202b 2067 6173 202b  ssions|' + gas +
-00026b10: 2027 7c49 5043 4d30 454c 275d 2e6d 6574   '|IPCM0EL'].met
-00026b20: 6120 3d20 636f 7079 2e63 6f70 7928 0a20  a = copy.copy(. 
-00026b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026b40: 2020 2064 6174 6154 6162 6c65 735b 2745     dataTables['E
-00026b50: 6d69 7373 696f 6e73 7c27 202b 2067 6173  missions|' + gas
-00026b60: 202b 2027 7c49 5043 3027 5d2e 6d65 7461   + '|IPC0'].meta
-00026b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026b80: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00026b90: 2020 2064 6174 6154 6162 6c65 735b 2745     dataTables['E
-00026ba0: 6d69 7373 696f 6e73 7c27 202b 2067 6173  missions|' + gas
-00026bb0: 202b 2027 7c49 5043 4d30 454c 275d 2e6d   + '|IPCM0EL'].m
-00026bc0: 6574 615b 2763 6174 6567 6f72 7927 5d20  eta['category'] 
-00026bd0: 3d20 2249 5043 4d30 454c 220a 2020 2020  = "IPCM0EL".    
-00026be0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00026bf0: 5461 626c 6573 5b27 456d 6973 7369 6f6e  Tables['Emission
-00026c00: 737c 2720 2b20 6761 7320 2b20 277c 4950  s|' + gas + '|IP
-00026c10: 4333 275d 203d 2028 0a20 2020 2020 2020  C3'] = (.       
-00026c20: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-00026c30: 6154 6162 6c65 735b 2745 6d69 7373 696f  aTables['Emissio
-00026c40: 6e73 7c27 202b 2067 6173 202b 2027 7c49  ns|' + gas + '|I
-00026c50: 5043 4d41 4727 5d0a 2020 2020 2020 2020  PCMAG'].        
-00026c60: 2020 2020 2020 2020 2020 2020 2b20 6461              + da
-00026c70: 7461 5461 626c 6573 5b27 456d 6973 7369  taTables['Emissi
-00026c80: 6f6e 737c 2720 2b20 6761 7320 2b20 277c  ons|' + gas + '|
-00026c90: 4c55 4c55 4346 275d 0a20 2020 2020 2020  LULUCF'].       
-00026ca0: 2020 2020 2020 2020 2029 2020 2320 4146           )  # AF
-00026cb0: 4f4c 550a 2020 2020 2020 2020 2020 2020  OLU.            
-00026cc0: 2020 2020 6461 7461 5461 626c 6573 5b27      dataTables['
-00026cd0: 456d 6973 7369 6f6e 737c 2720 2b20 6761  Emissions|' + ga
-00026ce0: 7320 2b20 277c 4950 4333 275d 2e6d 6574  s + '|IPC3'].met
-00026cf0: 6120 3d20 636f 7079 2e63 6f70 7928 0a20  a = copy.copy(. 
-00026d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026d10: 2020 2064 6174 6154 6162 6c65 735b 2745     dataTables['E
-00026d20: 6d69 7373 696f 6e73 7c27 202b 2067 6173  missions|' + gas
-00026d30: 202b 2027 7c49 5043 3027 5d2e 6d65 7461   + '|IPC0'].meta
-00026d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026d50: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00026d60: 2020 2064 6174 6154 6162 6c65 735b 2745     dataTables['E
-00026d70: 6d69 7373 696f 6e73 7c27 202b 2067 6173  missions|' + gas
-00026d80: 202b 2027 7c49 5043 3327 5d2e 6d65 7461   + '|IPC3'].meta
-00026d90: 5b27 6361 7465 676f 7279 275d 203d 2022  ['category'] = "
-00026da0: 4950 434d 3322 0a0a 2020 2020 2020 2020  IPCM3"..        
-00026db0: 7461 626c 6573 546f 436f 6d6d 6974 203d  tablesToCommit =
-00026dc0: 206c 6973 7428 290a 2020 2020 2020 2020   list().        
-00026dd0: 666f 7220 6b65 7920 696e 2064 6174 6154  for key in dataT
-00026de0: 6162 6c65 732e 6b65 7973 2829 3a0a 2020  ables.keys():.  
-00026df0: 2020 2020 2020 2020 2020 6461 7461 5461            dataTa
-00026e00: 626c 6573 5b6b 6579 5d20 3d20 6461 7461  bles[key] = data
-00026e10: 5461 626c 6573 5b6b 6579 5d2e 6173 7479  Tables[key].asty
-00026e20: 7065 2866 6c6f 6174 290a 2020 2020 2020  pe(float).      
-00026e30: 2020 2020 2020 6461 7461 5461 626c 6573        dataTables
-00026e40: 5b6b 6579 5d2e 6765 6e65 7261 7465 5461  [key].generateTa
-00026e50: 626c 6549 4428 290a 2020 2020 2020 2020  bleID().        
-00026e60: 2020 2020 7461 626c 6573 546f 436f 6d6d      tablesToComm
-00026e70: 6974 2e61 7070 656e 6428 6461 7461 5461  it.append(dataTa
-00026e80: 626c 6573 5b6b 6579 5d29 0a20 2020 2020  bles[key]).     
-00026e90: 2020 2072 6574 7572 6e20 7461 626c 6573     return tables
-00026ea0: 546f 436f 6d6d 6974 0a0a 0a63 6c61 7373  ToCommit...class
-00026eb0: 2053 4447 5f44 4154 415f 3230 3139 2842   SDG_DATA_2019(B
-00026ec0: 6173 6549 6d70 6f72 7454 6f6f 6c29 3a0a  aseImportTool):.
-00026ed0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00026ee0: 2873 656c 6629 3a0a 0a20 2020 2020 2020  (self):..       
-00026ef0: 2073 656c 662e 7365 7475 7020 3d20 7365   self.setup = se
-00026f00: 7475 7053 7472 7563 7428 290a 0a20 2020  tupStruct()..   
-00026f10: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
-00026f20: 534f 5552 4345 5f49 4420 3d20 2253 4447  SOURCE_ID = "SDG
-00026f30: 5f44 425f 3230 3139 220a 2020 2020 2020  _DB_2019".      
-00026f40: 2020 7365 6c66 2e73 6574 7570 2e53 4f55    self.setup.SOU
-00026f50: 5243 455f 5041 5448 203d 206f 732e 7061  RCE_PATH = os.pa
-00026f60: 7468 2e6a 6f69 6e28 0a20 2020 2020 2020  th.join(.       
-00026f70: 2020 2020 2063 6f6e 6669 672e 5041 5448       config.PATH
-00026f80: 5f54 4f5f 4441 5441 5348 454c 462c 2027  _TO_DATASHELF, '
-00026f90: 7261 7764 6174 612f 5344 475f 4442 5f32  rawdata/SDG_DB_2
-00026fa0: 3031 3927 0a20 2020 2020 2020 2029 0a20  019'.        ). 
-00026fb0: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
-00026fc0: 702e 4441 5441 5f46 494c 4520 3d20 6f73  p.DATA_FILE = os
-00026fd0: 2e70 6174 682e 6a6f 696e 280a 2020 2020  .path.join(.    
-00026fe0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00026ff0: 7570 2e53 4f55 5243 455f 5041 5448 2c20  up.SOURCE_PATH, 
-00027000: 2765 7874 7261 6374 5f30 355f 3230 3139  'extract_05_2019
-00027010: 2e63 7376 270a 2020 2020 2020 2020 290a  .csv'.        ).
-00027020: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00027030: 7570 2e4d 4150 5049 4e47 5f46 494c 4520  up.MAPPING_FILE 
-00027040: 3d20 6f73 2e70 6174 682e 6a6f 696e 2873  = os.path.join(s
-00027050: 656c 662e 7365 7475 702e 534f 5552 4345  elf.setup.SOURCE
-00027060: 5f50 4154 482c 2027 6d61 7070 696e 672e  _PATH, 'mapping.
-00027070: 786c 7378 2729 0a20 2020 2020 2020 2073  xlsx').        s
-00027080: 656c 662e 7365 7475 702e 4c49 4345 4e43  elf.setup.LICENC
-00027090: 4520 3d20 276f 7065 6e20 6163 6365 7373  E = 'open access
-000270a0: 2028 554e 2927 0a20 2020 2020 2020 2073   (UN)'.        s
-000270b0: 656c 662e 7365 7475 702e 5552 4c20 3d20  elf.setup.URL = 
-000270c0: 2768 7474 7073 3a2f 2f75 6e73 7461 7473  'https://unstats
-000270d0: 2e75 6e2e 6f72 672f 7364 6773 2f69 6e64  .un.org/sdgs/ind
-000270e0: 6963 6174 6f72 732f 6461 7461 6261 7365  icators/database
-000270f0: 2f27 0a0a 2020 2020 2020 2020 7365 6c66  /'..        self
-00027100: 2e73 6574 7570 2e49 4e44 4558 5f43 4f4c  .setup.INDEX_COL
-00027110: 554d 4e5f 4e41 4d45 203d 2027 5365 7269  UMN_NAME = 'Seri
-00027120: 6573 436f 6465 270a 2020 2020 2020 2020  esCode'.        
-00027130: 7365 6c66 2e73 6574 7570 2e53 5041 5449  self.setup.SPATI
-00027140: 414c 5f43 4f4c 554d 5f4e 414d 4520 3d20  AL_COLUM_NAME = 
-00027150: 2747 656f 4172 6561 436f 6465 270a 0a20  'GeoAreaCode'.. 
-00027160: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
-00027170: 702e 434f 4c55 4d4e 535f 544f 5f44 524f  p.COLUMNS_TO_DRO
-00027180: 5020 3d20 5b27 436f 756e 7472 7920 4e61  P = ['Country Na
-00027190: 6d65 272c 2027 496e 6469 6361 746f 7220  me', 'Indicator 
-000271a0: 4e61 6d65 275d 0a0a 2020 2020 2020 2020  Name']..        
-000271b0: 7365 6c66 2e63 7265 6174 6553 6f75 7263  self.createSourc
-000271c0: 654d 6574 6128 290a 0a20 2020 2020 2020  eMeta()..       
-000271d0: 2069 6620 6e6f 7420 286f 732e 7061 7468   if not (os.path
-000271e0: 2e65 7869 7374 7328 7365 6c66 2e73 6574  .exists(self.set
-000271f0: 7570 2e4d 4150 5049 4e47 5f46 494c 4529  up.MAPPING_FILE)
-00027200: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00027210: 656c 662e 6372 6561 7465 5661 7269 6162  elf.createVariab
-00027220: 6c65 4d61 7070 696e 6728 290a 2020 2020  leMapping().    
-00027230: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00027240: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
-00027250: 6e67 203d 2070 642e 7265 6164 5f65 7863  ng = pd.read_exc
-00027260: 656c 280a 2020 2020 2020 2020 2020 2020  el(.            
-00027270: 2020 2020 7365 6c66 2e73 6574 7570 2e4d      self.setup.M
-00027280: 4150 5049 4e47 5f46 494c 452c 2073 6865  APPING_FILE, she
-00027290: 6574 5f6e 616d 653d 5641 525f 4d41 5050  et_name=VAR_MAPP
-000272a0: 494e 475f 5348 4545 542c 2069 6e64 6578  ING_SHEET, index
-000272b0: 5f63 6f6c 3d30 0a20 2020 2020 2020 2020  _col=0.         
-000272c0: 2020 2029 0a0a 2020 2020 6465 6620 6c6f     )..    def lo
-000272d0: 6164 4461 7461 2873 656c 6629 3a0a 2020  adData(self):.  
-000272e0: 2020 2020 2020 7365 6c66 2e64 6174 6120        self.data 
-000272f0: 3d20 7064 2e72 6561 645f 6373 7628 7365  = pd.read_csv(se
-00027300: 6c66 2e73 6574 7570 2e44 4154 415f 4649  lf.setup.DATA_FI
-00027310: 4c45 2c20 6865 6164 6572 3d30 290a 2020  LE, header=0).  
-00027320: 2020 2020 2020 7365 6c66 2e64 6174 615b        self.data[
-00027330: 2770 7269 6d61 7279 5f63 6f64 6527 5d20  'primary_code'] 
-00027340: 3d20 7365 6c66 2e64 6174 612e 696e 6465  = self.data.inde
-00027350: 780a 2020 2020 2020 2020 6d6f 6469 6669  x.        modifi
-00027360: 6572 436f 6c75 6d6e 7320 3d20 5b73 656c  erColumns = [sel
-00027370: 662e 7365 7475 702e 494e 4445 585f 434f  f.setup.INDEX_CO
-00027380: 4c55 4d4e 5f4e 414d 455d 202b 206c 6973  LUMN_NAME] + lis
-00027390: 7428 0a20 2020 2020 2020 2020 2020 2073  t(.            s
-000273a0: 656c 662e 6461 7461 2e63 6f6c 756d 6e73  elf.data.columns
-000273b0: 5b31 343a 2d31 5d0a 2020 2020 2020 2020  [14:-1].        
-000273c0: 290a 2020 2020 2020 2020 6d6f 6469 6669  ).        modifi
-000273d0: 6572 436f 6c75 6d6e 732e 7265 6d6f 7665  erColumns.remove
-000273e0: 2827 5b52 6570 6f72 7469 6e67 2054 7970  ('[Reporting Typ
-000273f0: 655d 2729 0a20 2020 2020 2020 2023 2073  e]').        # s
-00027400: 656c 662e 6461 7461 5b6d 6f64 6966 6965  elf.data[modifie
-00027410: 7243 6f6c 756d 6e73 5d20 3d20 7365 6c66  rColumns] = self
-00027420: 2e64 6174 615b 6d6f 6469 6669 6572 436f  .data[modifierCo
-00027430: 6c75 6d6e 735d 2e66 696c 6c6e 6128 274e  lumns].fillna('N
-00027440: 614e 2729 0a20 2020 2020 2020 2023 2073  aN').        # s
-00027450: 656c 662e 6461 7461 5b6d 6f64 6966 6965  elf.data[modifie
-00027460: 7243 6f6c 756d 6e73 5d2e 6170 706c 7928  rColumns].apply(
-00027470: 6c61 6d62 6461 2078 3a20 275f 272e 6a6f  lambda x: '_'.jo
-00027480: 696e 2878 292c 2061 7869 733d 3129 0a20  in(x), axis=1). 
-00027490: 2020 2020 2020 2023 2073 656c 662e 6461         # self.da
-000274a0: 7461 5b6d 6f64 6966 6965 7243 6f6c 756d  ta[modifierColum
-000274b0: 6e73 5d2e 6173 7479 7065 2873 7472 292e  ns].astype(str).
-000274c0: 6170 706c 7928 6c61 6d62 6461 2078 3a20  apply(lambda x: 
-000274d0: 782e 7374 722e 6361 7428 7365 703d 275f  x.str.cat(sep='_
-000274e0: 2729 2c20 6178 6973 3d31 290a 2020 2020  '), axis=1).    
-000274f0: 2020 2020 7365 6c66 2e64 6174 612e 696e      self.data.in
-00027500: 6465 7820 3d20 280a 2020 2020 2020 2020  dex = (.        
-00027510: 2020 2020 7365 6c66 2e64 6174 615b 6d6f      self.data[mo
-00027520: 6469 6669 6572 436f 6c75 6d6e 735d 0a20  difierColumns]. 
-00027530: 2020 2020 2020 2020 2020 202e 6669 6c6c             .fill
-00027540: 6e61 2827 2729 0a20 2020 2020 2020 2020  na('').         
-00027550: 2020 202e 6173 7479 7065 2873 7472 290a     .astype(str).
-00027560: 2020 2020 2020 2020 2020 2020 2e61 7070              .app
-00027570: 6c79 286c 616d 6264 6120 783a 2027 5f27  ly(lambda x: '_'
-00027580: 2e6a 6f69 6e28 6669 6c74 6572 284e 6f6e  .join(filter(Non
-00027590: 652c 2078 2929 2c20 6178 6973 3d31 290a  e, x)), axis=1).
-000275a0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-000275b0: 6566 2063 7265 6174 6556 6172 6961 626c  ef createVariabl
-000275c0: 654d 6170 7069 6e67 2873 656c 6629 3a0a  eMapping(self):.
-000275d0: 2020 2020 2020 2020 7772 6974 6572 203d          writer =
-000275e0: 2070 642e 4578 6365 6c57 7269 7465 7228   pd.ExcelWriter(
-000275f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00027600: 662e 7365 7475 702e 4d41 5050 494e 475f  f.setup.MAPPING_
-00027610: 4649 4c45 2c0a 2020 2020 2020 2020 2020  FILE,.          
-00027620: 2020 656e 6769 6e65 3d27 786c 7378 7772    engine='xlsxwr
-00027630: 6974 6572 272c 0a20 2020 2020 2020 2020  iter',.         
-00027640: 2020 2064 6174 6574 696d 655f 666f 726d     datetime_form
-00027650: 6174 3d27 6d6d 6d20 6420 7979 7979 2068  at='mmm d yyyy h
-00027660: 683a 6d6d 3a73 7327 2c0a 2020 2020 2020  h:mm:ss',.      
-00027670: 2020 2020 2020 6461 7465 5f66 6f72 6d61        date_forma
-00027680: 743d 276d 6d6d 6d20 6464 2079 7979 7927  t='mmmm dd yyyy'
-00027690: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-000276a0: 2020 2020 2069 6620 6e6f 7420 6861 7361       if not hasa
-000276b0: 7474 7228 7365 6c66 2c20 2764 6174 6127  ttr(self, 'data'
-000276c0: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
-000276d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000276e0: 2e64 6174 6120 3d20 7064 2e72 6561 645f  .data = pd.read_
-000276f0: 6373 7628 7365 6c66 2e73 6574 7570 2e44  csv(self.setup.D
-00027700: 4154 415f 4649 4c45 2c20 656e 636f 6469  ATA_FILE, encodi
-00027710: 6e67 3d27 7574 6638 272c 2065 6e67 696e  ng='utf8', engin
-00027720: 653d 2770 7974 686f 6e27 2c20 696e 6465  e='python', inde
-00027730: 785f 636f 6c20 3d20 4e6f 6e65 2c20 6865  x_col = None, he
-00027740: 6164 6572 203d 302c 206e 615f 7661 6c75  ader =0, na_valu
-00027750: 6573 3d27 2e2e 2729 0a20 2020 2020 2020  es='..').       
-00027760: 2020 2020 2023 2020 2020 2020 2020 2020       #          
-00027770: 2020 7365 6c66 2e64 6174 615b 2763 6f6d    self.data['com
-00027780: 6269 6e65 6427 5d20 3d20 7365 6c66 2e64  bined'] = self.d
-00027790: 6174 615b 7365 6c66 2e73 6574 7570 2e49  ata[self.setup.I
-000277a0: 4e44 4558 5f43 4f4c 554d 4e5f 4e41 4d45  NDEX_COLUMN_NAME
-000277b0: 5d2e 6170 706c 7928 6c61 6d62 6461 2078  ].apply(lambda x
-000277c0: 3a20 275f 272e 6a6f 696e 2878 292c 2061  : '_'.join(x), a
-000277d0: 7869 733d 3129 0a20 2020 2020 2020 2020  xis=1).         
-000277e0: 2020 2073 656c 662e 6c6f 6164 4461 7461     self.loadData
-000277f0: 2829 0a0a 2020 2020 2020 2020 2320 7365  ()..        # se
-00027800: 6c66 2e64 6174 615b 7365 6c66 2e73 6574  lf.data[self.set
-00027810: 7570 2e49 4e44 4558 5f43 4f4c 554d 4e5f  up.INDEX_COLUMN_
-00027820: 4e41 4d45 5d2e 6170 706c 7928 6c61 6d62  NAME].apply(lamb
-00027830: 6461 2078 3a20 275f 272e 6a6f 696e 2878  da x: '_'.join(x
-00027840: 292c 2061 7869 733d 3129 0a20 2020 2020  ), axis=1).     
-00027850: 2020 2061 7661 696c 6162 6c65 5365 7269     availableSeri
-00027860: 6573 203d 2073 656c 662e 6461 7461 2e69  es = self.data.i
-00027870: 6e64 6578 2e75 6e69 7175 6528 290a 2020  ndex.unique().  
-00027880: 2020 2020 2020 6465 7363 7244 6620 3d20        descrDf = 
-00027890: 7365 6c66 2e64 6174 615b 2753 6572 6965  self.data['Serie
-000278a0: 7344 6573 6372 6970 7469 6f6e 275d 2e64  sDescription'].d
-000278b0: 726f 705f 6475 706c 6963 6174 6573 2829  rop_duplicates()
-000278c0: 0a0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-000278d0: 6170 7069 6e67 203d 2070 642e 4461 7461  apping = pd.Data
-000278e0: 4672 616d 6528 0a20 2020 2020 2020 2020  Frame(.         
-000278f0: 2020 2069 6e64 6578 3d61 7661 696c 6162     index=availab
-00027900: 6c65 5365 7269 6573 2c20 636f 6c75 6d6e  leSeries, column
-00027910: 733d 4d41 5050 494e 475f 434f 4c55 4d4e  s=MAPPING_COLUMN
-00027920: 5320 2b20 5b27 6465 7363 7269 7074 696f  S + ['descriptio
-00027930: 6e27 5d0a 2020 2020 2020 2020 290a 2020  n'].        ).  
-00027940: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
-00027950: 6e67 2e73 6f75 7263 6520 3d20 7365 6c66  ng.source = self
-00027960: 2e73 6574 7570 2e53 4f55 5243 455f 4944  .setup.SOURCE_ID
-00027970: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
-00027980: 7070 696e 672e 7363 656e 6172 696f 203d  pping.scenario =
-00027990: 2027 6869 7374 6f72 6963 270a 2020 2020   'historic'.    
-000279a0: 2020 2020 7365 6c66 2e6d 6170 7069 6e67      self.mapping
-000279b0: 2e64 6573 6372 6970 7469 6f6e 203d 2064  .description = d
-000279c0: 6573 6372 4466 0a20 2020 2020 2020 2073  escrDf.        s
-000279d0: 656c 662e 6d61 7070 696e 672e 6465 7363  elf.mapping.desc
-000279e0: 7269 7074 696f 6e20 3d20 7365 6c66 2e6d  ription = self.m
-000279f0: 6170 7069 6e67 2e64 6573 6372 6970 7469  apping.descripti
-00027a00: 6f6e 2e66 696c 6c6e 6128 6d65 7468 6f64  on.fillna(method
-00027a10: 3d27 6666 696c 6c27 290a 2020 2020 2020  ='ffill').      
-00027a20: 2020 7365 6c66 2e6d 6170 7069 6e67 2e74    self.mapping.t
-00027a30: 6f5f 6578 6365 6c28 7772 6974 6572 2c20  o_excel(writer, 
-00027a40: 7368 6565 745f 6e61 6d65 3d56 4152 5f4d  sheet_name=VAR_M
-00027a50: 4150 5049 4e47 5f53 4845 4554 290a 2020  APPING_SHEET).  
-00027a60: 2020 2020 2020 7772 6974 6572 2e63 6c6f        writer.clo
-00027a70: 7365 2829 0a0a 2020 2020 6465 6620 6761  se()..    def ga
-00027a80: 7468 6572 4d61 7070 6564 4461 7461 2873  therMappedData(s
-00027a90: 656c 662c 2073 7061 7469 616c 5375 6253  elf, spatialSubS
-00027aa0: 6574 3d4e 6f6e 6529 3a0a 2020 2020 2020  et=None):.      
-00027ab0: 2020 2320 6c6f 6164 696e 6720 6461 7461    # loading data
-00027ac0: 2069 6620 6e65 6365 7373 6172 790a 2020   if necessary.  
-00027ad0: 2020 2020 2020 6966 206e 6f74 2068 6173        if not has
-00027ae0: 6174 7472 2873 656c 662c 2027 6461 7461  attr(self, 'data
-00027af0: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
-00027b00: 7365 6c66 2e6c 6f61 6444 6174 6128 290a  self.loadData().
-00027b10: 0a20 2020 2020 2020 2069 6e64 6578 4461  .        indexDa
-00027b20: 7461 546f 436f 6c6c 6563 7420 3d20 7365  taToCollect = se
-00027b30: 6c66 2e6d 6170 7069 6e67 2e69 6e64 6578  lf.mapping.index
-00027b40: 5b7e 7064 2e69 736e 756c 6c28 7365 6c66  [~pd.isnull(self
-00027b50: 2e6d 6170 7069 6e67 5b27 656e 7469 7479  .mapping['entity
-00027b60: 275d 295d 0a0a 2020 2020 2020 2020 7461  '])]..        ta
-00027b70: 626c 6573 546f 436f 6d6d 6974 203d 205b  blesToCommit = [
-00027b80: 5d0a 2020 2020 2020 2020 666f 7220 6964  ].        for id
-00027b90: 7820 696e 2069 6e64 6578 4461 7461 546f  x in indexDataTo
-00027ba0: 436f 6c6c 6563 743a 0a20 2020 2020 2020  Collect:.       
-00027bb0: 2020 2020 206d 6574 6144 6620 3d20 7365       metaDf = se
-00027bc0: 6c66 2e6d 6170 7069 6e67 2e6c 6f63 5b69  lf.mapping.loc[i
-00027bd0: 6478 5d0a 2020 2020 2020 2020 2020 2020  dx].            
-00027be0: 7072 696e 7428 6964 7829 0a0a 2020 2020  print(idx)..    
-00027bf0: 2020 2020 2020 2020 2320 7072 696e 7428          # print(
-00027c00: 6d65 7461 4466 5b63 6f6e 6669 672e 5245  metaDf[config.RE
-00027c10: 5155 4952 4544 5f4d 4554 415f 4649 454c  QUIRED_META_FIEL
-00027c20: 4453 5d2e 6973 6e75 6c6c 2829 2e61 6c6c  DS].isnull().all
-00027c30: 2829 203d 3d20 4661 6c73 6529 0a20 2020  () == False).   
-00027c40: 2020 2020 2020 2020 2023 2070 7269 6e74           # print
-00027c50: 286d 6574 6144 6174 615b 7365 6c66 2e73  (metaData[self.s
-00027c60: 6574 7570 2e49 4e44 4558 5f43 4f4c 554d  etup.INDEX_COLUM
-00027c70: 4e5f 4e41 4d45 5d29 0a0a 2020 2020 2020  N_NAME])..      
-00027c80: 2020 2020 2020 6d65 7461 4469 6374 203d        metaDict =
-00027c90: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00027ca0: 2020 206b 6579 3a20 6d65 7461 4466 5b6b     key: metaDf[k
-00027cb0: 6579 5d0a 2020 2020 2020 2020 2020 2020  ey].            
-00027cc0: 2020 2020 666f 7220 6b65 7920 696e 2063      for key in c
-00027cd0: 6f6e 6669 672e 5245 5155 4952 4544 5f4d  onfig.REQUIRED_M
-00027ce0: 4554 415f 4649 454c 4453 2e75 6e69 6f6e  ETA_FIELDS.union
-00027cf0: 287b 2775 6e69 7454 6f27 7d29 0a20 2020  ({'unitTo'}).   
-00027d00: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
-00027d10: 2020 2020 2020 2020 6d65 7461 4469 6374          metaDict
-00027d20: 5b27 6f72 6967 696e 616c 2063 6f64 6527  ['original code'
-00027d30: 5d20 3d20 6964 780a 2020 2020 2020 2020  ] = idx.        
-00027d40: 2020 2020 2320 6d65 7461 4469 6374 5b27      # metaDict['
-00027d50: 6f72 6967 696e 616c 206e 616d 6527 5d20  original name'] 
-00027d60: 3d20 6d65 7461 4466 5b27 496e 6469 6361  = metaDf['Indica
-00027d70: 746f 7220 4e61 6d65 275d 0a0a 2020 2020  tor Name']..    
-00027d80: 2020 2020 2020 2020 7365 7269 6573 4964          seriesId
-00027d90: 7820 3d20 6964 780a 0a20 2020 2020 2020  x = idx..       
-00027da0: 2020 2020 2064 6174 6166 7261 6d65 203d       dataframe =
-00027db0: 2073 656c 662e 6461 7461 2e6c 6f63 5b73   self.data.loc[s
-00027dc0: 6572 6965 7349 6478 2c20 5b27 4765 6f41  eriesIdx, ['GeoA
-00027dd0: 7265 6143 6f64 6527 2c20 2754 696d 6550  reaCode', 'TimeP
-00027de0: 6572 696f 6427 2c20 2756 616c 7565 275d  eriod', 'Value']
-00027df0: 5d0a 2020 2020 2020 2020 2020 2020 6461  ].            da
-00027e00: 7461 6672 616d 6520 3d20 6461 7461 6672  taframe = datafr
-00027e10: 616d 652e 7069 766f 7428 0a20 2020 2020  ame.pivot(.     
-00027e20: 2020 2020 2020 2020 2020 2069 6e64 6578             index
-00027e30: 3d27 4765 6f41 7265 6143 6f64 6527 2c20  ='GeoAreaCode', 
-00027e40: 636f 6c75 6d6e 733d 2754 696d 6550 6572  columns='TimePer
-00027e50: 696f 6427 2c20 7661 6c75 6573 3d27 5661  iod', values='Va
-00027e60: 6c75 6527 0a20 2020 2020 2020 2020 2020  lue'.           
-00027e70: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-00027e80: 6461 7461 6672 616d 6520 3d20 6461 7461  dataframe = data
-00027e90: 6672 616d 652e 6173 7479 7065 2866 6c6f  frame.astype(flo
-00027ea0: 6174 290a 0a20 2020 2020 2020 2020 2020  at)..           
-00027eb0: 206e 6577 4461 7461 203d 206c 6973 7428   newData = list(
-00027ec0: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-00027ed0: 7220 6952 6f77 2069 6e20 7261 6e67 6528  r iRow in range(
-00027ee0: 6c65 6e28 6461 7461 6672 616d 6529 293a  len(dataframe)):
-00027ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00027f00: 2049 534f 5f49 4420 3d20 6474 2e6d 6170   ISO_ID = dt.map
-00027f10: 702e 6765 7453 7061 7469 616c 4944 2864  p.getSpatialID(d
-00027f20: 6174 6166 7261 6d65 2e69 6e64 6578 5b69  ataframe.index[i
-00027f30: 526f 775d 290a 2020 2020 2020 2020 2020  Row]).          
-00027f40: 2020 2020 2020 6966 2064 6174 6166 7261        if datafra
-00027f50: 6d65 2e69 6e64 6578 5b69 526f 775d 203d  me.index[iRow] =
-00027f60: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
-00027f70: 2020 2020 2020 2020 2049 534f 5f49 4420           ISO_ID 
-00027f80: 3d20 2257 6f72 6c64 220a 2020 2020 2020  = "World".      
-00027f90: 2020 2020 2020 2020 2020 6966 2049 534f            if ISO
-00027fa0: 5f49 443a 0a20 2020 2020 2020 2020 2020  _ID:.           
-00027fb0: 2020 2020 2020 2020 206e 6577 4461 7461           newData
-00027fc0: 2e61 7070 656e 6428 4953 4f5f 4944 290a  .append(ISO_ID).
-00027fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027fe0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00027ff0: 2020 2020 2020 2020 2020 6e65 7744 6174            newDat
-00028000: 612e 6170 7065 6e64 2870 642e 6e70 2e6e  a.append(pd.np.n
-00028010: 616e 290a 2020 2020 2020 2020 2020 2020  an).            
-00028020: 6461 7461 6672 616d 652e 696e 6465 7820  dataframe.index 
-00028030: 3d20 6e65 7744 6174 610a 0a20 2020 2020  = newData..     
-00028040: 2020 2020 2020 2069 6620 7370 6174 6961         if spatia
-00028050: 6c53 7562 5365 743a 0a20 2020 2020 2020  lSubSet:.       
-00028060: 2020 2020 2020 2020 2073 7061 7449 6478           spatIdx
-00028070: 203d 2064 6174 6166 7261 6d65 2e69 6e64   = dataframe.ind
-00028080: 6578 2e69 7369 6e28 7370 6174 6961 6c53  ex.isin(spatialS
-00028090: 7562 5365 7429 0a20 2020 2020 2020 2020  ubSet).         
-000280a0: 2020 2020 2020 2064 6174 6166 7261 6d65         dataframe
-000280b0: 203d 2064 6174 6166 7261 6d65 2e6c 6f63   = dataframe.loc
-000280c0: 5b73 7061 7449 6478 5d0a 0a20 2020 2020  [spatIdx]..     
-000280d0: 2020 2020 2020 2064 6174 6166 7261 6d65         dataframe
-000280e0: 203d 2064 6174 6166 7261 6d65 2e64 726f   = dataframe.dro
-000280f0: 706e 6128 6178 6973 3d31 2c20 686f 773d  pna(axis=1, how=
-00028100: 2761 6c6c 2729 0a20 2020 2020 2020 2020  'all').         
-00028110: 2020 2064 6174 6166 7261 6d65 203d 2064     dataframe = d
-00028120: 6174 6166 7261 6d65 2e6c 6f63 5b7e 7064  ataframe.loc[~pd
-00028130: 2e69 736e 6128 6461 7461 6672 616d 652e  .isna(dataframe.
-00028140: 696e 6465 7829 5d0a 2020 2020 2020 2020  index)].        
-00028150: 2020 2020 6461 7461 5461 626c 6520 3d20      dataTable = 
-00028160: 4461 7461 7461 626c 6528 6461 7461 6672  Datatable(datafr
-00028170: 616d 652c 206d 6574 613d 6d65 7461 4469  ame, meta=metaDi
-00028180: 6374 290a 2020 2020 2020 2020 2020 2020  ct).            
-00028190: 2320 706f 7373 6962 6c65 2072 6571 7569  # possible requi
-000281a0: 7265 6420 756e 6974 2063 6f6e 7665 7273  red unit convers
-000281b0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-000281c0: 6966 206e 6f74 2070 642e 6973 6e61 286d  if not pd.isna(m
-000281d0: 6574 6144 6963 745b 2775 6e69 7454 6f27  etaDict['unitTo'
-000281e0: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
-000281f0: 2020 2020 6461 7461 5461 626c 6520 3d20      dataTable = 
-00028200: 6461 7461 5461 626c 652e 636f 6e76 6572  dataTable.conver
-00028210: 7428 6d65 7461 4469 6374 5b27 756e 6974  t(metaDict['unit
-00028220: 546f 275d 290a 2020 2020 2020 2020 2020  To']).          
-00028230: 2020 7461 626c 6573 546f 436f 6d6d 6974    tablesToCommit
-00028240: 2e61 7070 656e 6428 6461 7461 5461 626c  .append(dataTabl
-00028250: 6529 0a0a 2020 2020 2020 2020 7265 7475  e)..        retu
-00028260: 726e 2074 6162 6c65 7354 6f43 6f6d 6d69  rn tablesToCommi
-00028270: 740a 0a0a 636c 6173 7320 484f 4553 4c59  t...class HOESLY
-00028280: 3230 3138 2842 6173 6549 6d70 6f72 7454  2018(BaseImportT
-00028290: 6f6f 6c29 3a0a 2020 2020 6465 6620 5f5f  ool):.    def __
-000282a0: 696e 6974 5f5f 2873 656c 6629 3a0a 2020  init__(self):.  
-000282b0: 2020 2020 2020 7365 6c66 2e73 6574 7570        self.setup
-000282c0: 203d 2073 6574 7570 5374 7275 6374 2829   = setupStruct()
-000282d0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-000282e0: 7475 702e 534f 5552 4345 5f49 4420 3d20  tup.SOURCE_ID = 
-000282f0: 2248 4f45 534c 5932 3031 3822 0a20 2020  "HOESLY2018".   
-00028300: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
-00028310: 534f 5552 4345 5f50 4154 4820 3d20 6f73  SOURCE_PATH = os
-00028320: 2e70 6174 682e 6a6f 696e 280a 2020 2020  .path.join(.    
-00028330: 2020 2020 2020 2020 636f 6e66 6967 2e50          config.P
-00028340: 4154 485f 544f 5f44 4154 4153 4845 4c46  ATH_TO_DATASHELF
-00028350: 2c20 2772 6177 6461 7461 2f48 4f45 534c  , 'rawdata/HOESL
-00028360: 5932 3031 3827 0a20 2020 2020 2020 2029  Y2018'.        )
-00028370: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00028380: 7475 702e 4441 5441 5f46 494c 4520 3d20  tup.DATA_FILE = 
-00028390: 6f73 2e70 6174 682e 6a6f 696e 280a 2020  os.path.join(.  
-000283a0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000283b0: 6574 7570 2e53 4f55 5243 455f 5041 5448  etup.SOURCE_PATH
-000283c0: 2c20 2763 6f6d 7069 6c65 645f 7261 775f  , 'compiled_raw_
-000283d0: 686f 6573 6c79 2e63 7376 270a 2020 2020  hoesly.csv'.    
-000283e0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-000283f0: 6c66 2e73 6574 7570 2e4d 4150 5049 4e47  lf.setup.MAPPING
-00028400: 5f46 494c 4520 3d20 6f73 2e70 6174 682e  _FILE = os.path.
-00028410: 6a6f 696e 2873 656c 662e 7365 7475 702e  join(self.setup.
-00028420: 534f 5552 4345 5f50 4154 482c 2027 6d61  SOURCE_PATH, 'ma
-00028430: 7070 696e 672e 786c 7378 2729 0a20 2020  pping.xlsx').   
-00028440: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
-00028450: 4c49 4345 4e43 4520 3d20 2720 4372 6561  LICENCE = ' Crea
-00028460: 7469 7665 2043 6f6d 6d6f 6e73 2041 7474  tive Commons Att
-00028470: 7269 6275 7469 6f6e 2033 2e30 204c 6963  ribution 3.0 Lic
-00028480: 656e 7365 270a 2020 2020 2020 2020 7365  ense'.        se
-00028490: 6c66 2e73 6574 7570 2e55 524c 203d 2027  lf.setup.URL = '
-000284a0: 6874 7470 733a 2f2f 7777 772e 6765 6f73  https://www.geos
-000284b0: 6369 2d6d 6f64 656c 2d64 6576 2e6e 6574  ci-model-dev.net
-000284c0: 2f31 312f 3336 392f 3230 3138 2f27 0a0a  /11/369/2018/'..
-000284d0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-000284e0: 7570 2e4d 4f44 454c 5f43 4f4c 554d 4e5f  up.MODEL_COLUMN_
-000284f0: 4e41 4d45 203d 2027 6d6f 6465 6c27 0a20  NAME = 'model'. 
-00028500: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
-00028510: 702e 5343 454e 4152 494f 5f43 4f4c 554d  p.SCENARIO_COLUM
-00028520: 4e5f 4e41 4d45 203d 2027 7363 656e 6172  N_NAME = 'scenar
-00028530: 696f 270a 2020 2020 2020 2020 7365 6c66  io'.        self
-00028540: 2e73 6574 7570 2e52 4547 494f 4e5f 434f  .setup.REGION_CO
-00028550: 4c55 4d4e 5f4e 414d 4520 3d20 2772 6567  LUMN_NAME = 'reg
-00028560: 696f 6e27 0a20 2020 2020 2020 2073 656c  ion'.        sel
-00028570: 662e 7365 7475 702e 5641 5249 4142 4c45  f.setup.VARIABLE
-00028580: 5f43 4f4c 554d 4e5f 4e41 4d45 203d 2027  _COLUMN_NAME = '
-00028590: 7661 7269 6162 6c65 270a 0a20 2020 2020  variable'..     
-000285a0: 2020 2069 6620 6e6f 7420 286f 732e 7061     if not (os.pa
-000285b0: 7468 2e65 7869 7374 7328 7365 6c66 2e73  th.exists(self.s
-000285c0: 6574 7570 2e4d 4150 5049 4e47 5f46 494c  etup.MAPPING_FIL
-000285d0: 4529 293a 0a20 2020 2020 2020 2020 2020  E)):.           
-000285e0: 2073 656c 662e 6372 6561 7465 5661 7269   self.createVari
-000285f0: 6162 6c65 4d61 7070 696e 6728 290a 2020  ableMapping().  
-00028600: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00028610: 226e 6f20 6d61 7070 696e 6720 6669 6c65  "no mapping file
-00028620: 2066 6f75 6e64 2229 0a20 2020 2020 2020   found").       
-00028630: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00028640: 2020 2073 656c 662e 6d61 7070 696e 6720     self.mapping 
-00028650: 3d20 6469 6374 2829 0a0a 2020 2020 2020  = dict()..      
-00028660: 2020 2020 2020 666f 7220 7661 7220 696e        for var in
-00028670: 205b 2776 6172 6961 626c 6527 2c20 2773   ['variable', 's
-00028680: 6365 6e61 7269 6f27 2c20 276d 6f64 656c  cenario', 'model
-00028690: 272c 2027 7265 6769 6f6e 275d 3a0a 2020  ', 'region']:.  
-000286a0: 2020 2020 2020 2020 2020 2020 2020 6466                df
-000286b0: 203d 2070 642e 7265 6164 5f65 7863 656c   = pd.read_excel
-000286c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000286d0: 2020 2020 2020 7365 6c66 2e73 6574 7570        self.setup
-000286e0: 2e4d 4150 5049 4e47 5f46 494c 452c 2073  .MAPPING_FILE, s
-000286f0: 6865 6574 5f6e 616d 653d 7661 7220 2b20  heet_name=var + 
-00028700: 275f 6d61 7070 696e 6727 2c20 696e 6465  '_mapping', inde
-00028710: 785f 636f 6c3d 300a 2020 2020 2020 2020  x_col=0.        
-00028720: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00028730: 2020 2020 2020 2020 2020 6466 203d 2064            df = d
-00028740: 662e 6c6f 635b 7e64 662e 6c6f 635b 3a2c  f.loc[~df.loc[:,
-00028750: 2076 6172 5d2e 6973 6e61 2829 5d0a 2020   var].isna()].  
-00028760: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00028770: 6c66 2e6d 6170 7069 6e67 2e75 7064 6174  lf.mapping.updat
-00028780: 6528 6466 2e74 6f5f 6469 6374 2829 290a  e(df.to_dict()).
-00028790: 0a20 2020 2020 2020 2073 656c 662e 6372  .        self.cr
-000287a0: 6561 7465 536f 7572 6365 4d65 7461 2829  eateSourceMeta()
-000287b0: 0a0a 2020 2020 6465 6620 6c6f 6164 4461  ..    def loadDa
-000287c0: 7461 2873 656c 6629 3a0a 2020 2020 2020  ta(self):.      
-000287d0: 2020 7365 6c66 2e64 6174 6120 3d20 7064    self.data = pd
-000287e0: 2e72 6561 645f 6373 7628 7365 6c66 2e73  .read_csv(self.s
-000287f0: 6574 7570 2e44 4154 415f 4649 4c45 2c20  etup.DATA_FILE, 
-00028800: 696e 6465 785f 636f 6c3d 4e6f 6e65 2c20  index_col=None, 
-00028810: 6865 6164 6572 3d30 290a 0a20 2020 2064  header=0)..    d
-00028820: 6566 2063 7265 6174 6556 6172 6961 626c  ef createVariabl
-00028830: 654d 6170 7069 6e67 2873 656c 6629 3a0a  eMapping(self):.
-00028840: 0a20 2020 2020 2020 2023 206c 6f61 6469  .        # loadi
-00028850: 6e67 2064 6174 6120 6966 206e 6563 6573  ng data if neces
-00028860: 7361 7279 0a20 2020 2020 2020 2069 6620  sary.        if 
-00028870: 6e6f 7420 6861 7361 7474 7228 7365 6c66  not hasattr(self
-00028880: 2c20 2764 6174 6127 293a 0a20 2020 2020  , 'data'):.     
-00028890: 2020 2020 2020 2073 656c 662e 6c6f 6164         self.load
-000288a0: 4461 7461 2829 0a0a 2020 2020 2020 2020  Data()..        
-000288b0: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
-000288c0: 6e70 0a0a 2020 2020 2020 2020 7772 6974  np..        writ
-000288d0: 6572 203d 2070 642e 4578 6365 6c57 7269  er = pd.ExcelWri
-000288e0: 7465 7228 0a20 2020 2020 2020 2020 2020  ter(.           
-000288f0: 2073 656c 662e 7365 7475 702e 4d41 5050   self.setup.MAPP
-00028900: 494e 475f 4649 4c45 2c0a 2020 2020 2020  ING_FILE,.      
-00028910: 2020 2020 2020 656e 6769 6e65 3d27 786c        engine='xl
-00028920: 7378 7772 6974 6572 272c 0a20 2020 2020  sxwriter',.     
-00028930: 2020 2020 2020 2064 6174 6574 696d 655f         datetime_
-00028940: 666f 726d 6174 3d27 6d6d 6d20 6420 7979  format='mmm d yy
-00028950: 7979 2068 683a 6d6d 3a73 7327 2c0a 2020  yy hh:mm:ss',.  
-00028960: 2020 2020 2020 2020 2020 6461 7465 5f66            date_f
-00028970: 6f72 6d61 743d 276d 6d6d 6d20 6464 2079  ormat='mmmm dd y
-00028980: 7979 7927 2c0a 2020 2020 2020 2020 290a  yyy',.        ).
-00028990: 0a20 2020 2020 2020 2023 2076 6172 6961  .        # varia
-000289a0: 626c 6573 0a20 2020 2020 2020 2023 2069  bles.        # i
-000289b0: 6e64 6578 203d 2073 656c 662e 6461 7461  ndex = self.data
-000289c0: 5b73 656c 662e 7365 7475 702e 5641 5249  [self.setup.VARI
-000289d0: 4142 4c45 5f43 4f4c 554d 4e5f 4e41 4d45  ABLE_COLUMN_NAME
-000289e0: 5d2e 756e 6971 7565 2829 0a20 2020 2020  ].unique().     
-000289f0: 2020 2073 656c 662e 6176 6169 6c61 626c     self.availabl
-00028a00: 6553 6572 6965 7320 3d20 7365 6c66 2e64  eSeries = self.d
-00028a10: 6174 612e 6472 6f70 5f64 7570 6c69 6361  ata.drop_duplica
-00028a20: 7465 7328 2776 6172 6961 626c 6527 292e  tes('variable').
-00028a30: 7365 745f 696e 6465 7828 0a20 2020 2020  set_index(.     
-00028a40: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
-00028a50: 702e 5641 5249 4142 4c45 5f43 4f4c 554d  p.VARIABLE_COLUM
-00028a60: 4e5f 4e41 4d45 0a20 2020 2020 2020 2029  N_NAME.        )
-00028a70: 5b27 756e 6974 275d 0a20 2020 2020 2020  ['unit'].       
-00028a80: 2073 656c 662e 6d61 7070 696e 6720 3d20   self.mapping = 
-00028a90: 7064 2e44 6174 6146 7261 6d65 280a 2020  pd.DataFrame(.  
-00028aa0: 2020 2020 2020 2020 2020 696e 6465 783d            index=
-00028ab0: 7365 6c66 2e61 7661 696c 6162 6c65 5365  self.availableSe
-00028ac0: 7269 6573 2e69 6e64 6578 2c20 636f 6c75  ries.index, colu
-00028ad0: 6d6e 733d 5b73 656c 662e 7365 7475 702e  mns=[self.setup.
-00028ae0: 5641 5249 4142 4c45 5f43 4f4c 554d 4e5f  VARIABLE_COLUMN_
-00028af0: 4e41 4d45 5d0a 2020 2020 2020 2020 290a  NAME].        ).
-00028b00: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
-00028b10: 7069 6e67 203d 2070 642e 636f 6e63 6174  ping = pd.concat
-00028b20: 285b 7365 6c66 2e6d 6170 7069 6e67 2c20  ([self.mapping, 
-00028b30: 7365 6c66 2e61 7661 696c 6162 6c65 5365  self.availableSe
-00028b40: 7269 6573 5d2c 2061 7869 733d 3129 0a20  ries], axis=1). 
-00028b50: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
-00028b60: 696e 6720 3d20 7365 6c66 2e6d 6170 7069  ing = self.mappi
-00028b70: 6e67 2e73 6f72 745f 696e 6465 7828 290a  ng.sort_index().
-00028b80: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
-00028b90: 7069 6e67 2e74 6f5f 6578 6365 6c28 7772  ping.to_excel(wr
-00028ba0: 6974 6572 2c20 656e 6769 6e65 3d27 6f70  iter, engine='op
-00028bb0: 656e 7079 786c 272c 2073 6865 6574 5f6e  enpyxl', sheet_n
-00028bc0: 616d 653d 5641 525f 4d41 5050 494e 475f  ame=VAR_MAPPING_
-00028bd0: 5348 4545 5429 0a0a 2020 2020 2020 2020  SHEET)..        
-00028be0: 2320 6d6f 6465 6c73 0a20 2020 2020 2020  # models.       
-00028bf0: 2069 6e64 6578 203d 206e 702e 756e 6971   index = np.uniq
-00028c00: 7565 2873 656c 662e 6461 7461 5b73 656c  ue(self.data[sel
-00028c10: 662e 7365 7475 702e 4d4f 4445 4c5f 434f  f.setup.MODEL_CO
-00028c20: 4c55 4d4e 5f4e 414d 455d 2e76 616c 7565  LUMN_NAME].value
-00028c30: 7329 0a0a 2020 2020 2020 2020 7365 6c66  s)..        self
-00028c40: 2e61 7661 696c 6162 6c65 5365 7269 6573  .availableSeries
-00028c50: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
-00028c60: 696e 6465 783d 696e 6465 7829 0a20 2020  index=index).   
-00028c70: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
-00028c80: 6720 3d20 7064 2e44 6174 6146 7261 6d65  g = pd.DataFrame
-00028c90: 2869 6e64 6578 3d69 6e64 6578 2c20 636f  (index=index, co
-00028ca0: 6c75 6d6e 733d 5b73 656c 662e 7365 7475  lumns=[self.setu
-00028cb0: 702e 4d4f 4445 4c5f 434f 4c55 4d4e 5f4e  p.MODEL_COLUMN_N
-00028cc0: 414d 455d 290a 2020 2020 2020 2020 7365  AME]).        se
-00028cd0: 6c66 2e6d 6170 7069 6e67 203d 2070 642e  lf.mapping = pd.
-00028ce0: 636f 6e63 6174 285b 7365 6c66 2e6d 6170  concat([self.map
-00028cf0: 7069 6e67 2c20 7365 6c66 2e61 7661 696c  ping, self.avail
-00028d00: 6162 6c65 5365 7269 6573 5d2c 2061 7869  ableSeries], axi
-00028d10: 733d 3129 0a20 2020 2020 2020 2073 656c  s=1).        sel
-00028d20: 662e 6d61 7070 696e 6720 3d20 7365 6c66  f.mapping = self
-00028d30: 2e6d 6170 7069 6e67 2e73 6f72 745f 696e  .mapping.sort_in
-00028d40: 6465 7828 290a 0a20 2020 2020 2020 2073  dex()..        s
-00028d50: 656c 662e 6d61 7070 696e 672e 746f 5f65  elf.mapping.to_e
-00028d60: 7863 656c 2877 7269 7465 722c 2065 6e67  xcel(writer, eng
-00028d70: 696e 653d 276f 7065 6e70 7978 6c27 2c20  ine='openpyxl', 
-00028d80: 7368 6565 745f 6e61 6d65 3d27 6d6f 6465  sheet_name='mode
-00028d90: 6c5f 6d61 7070 696e 6727 290a 0a20 2020  l_mapping')..   
-00028da0: 2020 2020 2023 2073 6365 6e61 7269 6f73       # scenarios
-00028db0: 0a20 2020 2020 2020 2069 6e64 6578 203d  .        index =
-00028dc0: 206e 702e 756e 6971 7565 2873 656c 662e   np.unique(self.
-00028dd0: 6461 7461 5b73 656c 662e 7365 7475 702e  data[self.setup.
-00028de0: 5343 454e 4152 494f 5f43 4f4c 554d 4e5f  SCENARIO_COLUMN_
-00028df0: 4e41 4d45 5d2e 7661 6c75 6573 290a 0a20  NAME].values).. 
-00028e00: 2020 2020 2020 2073 656c 662e 6176 6169         self.avai
-00028e10: 6c61 626c 6553 6572 6965 7320 3d20 7064  lableSeries = pd
-00028e20: 2e44 6174 6146 7261 6d65 2869 6e64 6578  .DataFrame(index
-00028e30: 3d69 6e64 6578 290a 2020 2020 2020 2020  =index).        
-00028e40: 7365 6c66 2e6d 6170 7069 6e67 203d 2070  self.mapping = p
-00028e50: 642e 4461 7461 4672 616d 6528 0a20 2020  d.DataFrame(.   
-00028e60: 2020 2020 2020 2020 2069 6e64 6578 3d69           index=i
-00028e70: 6e64 6578 2c20 636f 6c75 6d6e 733d 5b73  ndex, columns=[s
-00028e80: 656c 662e 7365 7475 702e 5343 454e 4152  elf.setup.SCENAR
-00028e90: 494f 5f43 4f4c 554d 4e5f 4e41 4d45 5d0a  IO_COLUMN_NAME].
-00028ea0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00028eb0: 2020 7365 6c66 2e6d 6170 7069 6e67 203d    self.mapping =
-00028ec0: 2070 642e 636f 6e63 6174 285b 7365 6c66   pd.concat([self
-00028ed0: 2e6d 6170 7069 6e67 2c20 7365 6c66 2e61  .mapping, self.a
-00028ee0: 7661 696c 6162 6c65 5365 7269 6573 5d2c  vailableSeries],
-00028ef0: 2061 7869 733d 3129 0a20 2020 2020 2020   axis=1).       
-00028f00: 2073 656c 662e 6d61 7070 696e 6720 3d20   self.mapping = 
-00028f10: 7365 6c66 2e6d 6170 7069 6e67 2e73 6f72  self.mapping.sor
-00028f20: 745f 696e 6465 7828 290a 2020 2020 2020  t_index().      
-00028f30: 2020 7365 6c66 2e6d 6170 7069 6e67 2e74    self.mapping.t
-00028f40: 6f5f 6578 6365 6c28 7772 6974 6572 2c20  o_excel(writer, 
-00028f50: 656e 6769 6e65 3d27 6f70 656e 7079 786c  engine='openpyxl
-00028f60: 272c 2073 6865 6574 5f6e 616d 653d 2773  ', sheet_name='s
-00028f70: 6365 6e61 7269 6f5f 6d61 7070 696e 6727  cenario_mapping'
-00028f80: 290a 0a20 2020 2020 2020 2023 2072 6567  )..        # reg
-00028f90: 696f 6e0a 2020 2020 2020 2020 696e 6465  ion.        inde
-00028fa0: 7820 3d20 6e70 2e75 6e69 7175 6528 7365  x = np.unique(se
-00028fb0: 6c66 2e64 6174 615b 7365 6c66 2e73 6574  lf.data[self.set
-00028fc0: 7570 2e72 6567 696f 6e5f 434f 4c55 4d4e  up.region_COLUMN
-00028fd0: 5f4e 414d 455d 2e76 616c 7565 7329 0a0a  _NAME].values)..
-00028fe0: 2020 2020 2020 2020 7365 6c66 2e61 7661          self.ava
-00028ff0: 696c 6162 6c65 5365 7269 6573 203d 2070  ilableSeries = p
-00029000: 642e 4461 7461 4672 616d 6528 696e 6465  d.DataFrame(inde
-00029010: 783d 696e 6465 7829 0a20 2020 2020 2020  x=index).       
-00029020: 2073 656c 662e 6d61 7070 696e 6720 3d20   self.mapping = 
-00029030: 7064 2e44 6174 6146 7261 6d65 280a 2020  pd.DataFrame(.  
-00029040: 2020 2020 2020 2020 2020 696e 6465 783d            index=
-00029050: 696e 6465 782c 2063 6f6c 756d 6e73 3d5b  index, columns=[
-00029060: 7365 6c66 2e73 6574 7570 2e52 4547 494f  self.setup.REGIO
-00029070: 4e5f 434f 4c55 4d4e 5f4e 414d 455d 0a20  N_COLUMN_NAME]. 
-00029080: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00029090: 2073 656c 662e 6d61 7070 696e 6720 3d20   self.mapping = 
-000290a0: 7064 2e63 6f6e 6361 7428 5b73 656c 662e  pd.concat([self.
-000290b0: 6d61 7070 696e 672c 2073 656c 662e 6176  mapping, self.av
-000290c0: 6169 6c61 626c 6553 6572 6965 735d 2c20  ailableSeries], 
-000290d0: 6178 6973 3d31 290a 2020 2020 2020 2020  axis=1).        
-000290e0: 7365 6c66 2e6d 6170 7069 6e67 203d 2073  self.mapping = s
-000290f0: 656c 662e 6d61 7070 696e 672e 736f 7274  elf.mapping.sort
-00029100: 5f69 6e64 6578 2829 0a0a 2020 2020 2020  _index()..      
-00029110: 2020 666f 7220 6964 7820 696e 2073 656c    for idx in sel
-00029120: 662e 6d61 7070 696e 672e 696e 6465 783a  f.mapping.index:
-00029130: 0a20 2020 2020 2020 2020 2020 2069 736f  .            iso
-00029140: 203d 2064 742e 7574 696c 2e69 6465 6e74   = dt.util.ident
-00029150: 6966 7943 6f75 6e74 7279 2869 6478 290a  ifyCountry(idx).
-00029160: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00029170: 736f 2069 7320 6e6f 7420 4e6f 6e65 3a0a  so is not None:.
-00029180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029190: 7365 6c66 2e6d 6170 7069 6e67 2e6c 6f63  self.mapping.loc
-000291a0: 5b69 6478 2c20 2772 6567 696f 6e27 5d20  [idx, 'region'] 
-000291b0: 3d20 6973 6f0a 0a20 2020 2020 2020 2073  = iso..        s
-000291c0: 656c 662e 6d61 7070 696e 672e 746f 5f65  elf.mapping.to_e
-000291d0: 7863 656c 2877 7269 7465 722c 2065 6e67  xcel(writer, eng
-000291e0: 696e 653d 276f 7065 6e70 7978 6c27 2c20  ine='openpyxl', 
-000291f0: 7368 6565 745f 6e61 6d65 3d27 7265 6769  sheet_name='regi
-00029200: 6f6e 5f6d 6170 7069 6e67 2729 0a20 2020  on_mapping').   
-00029210: 2020 2020 2077 7269 7465 722e 636c 6f73       writer.clos
-00029220: 6528 290a 0a20 2020 2064 6566 2067 6174  e()..    def gat
-00029230: 6865 724d 6170 7065 6444 6174 6128 7365  herMappedData(se
-00029240: 6c66 2c20 7370 6174 6961 6c53 7562 5365  lf, spatialSubSe
-00029250: 743d 4e6f 6e65 2c20 7570 6461 7465 5461  t=None, updateTa
-00029260: 626c 6573 3d46 616c 7365 293a 0a0a 2020  bles=False):..  
-00029270: 2020 2020 2020 696d 706f 7274 2074 7164        import tqd
-00029280: 6d0a 0a20 2020 2020 2020 2023 206c 6f61  m..        # loa
-00029290: 6469 6e67 2064 6174 6120 6966 206e 6563  ding data if nec
-000292a0: 6573 7361 7279 0a20 2020 2020 2020 2069  essary.        i
-000292b0: 6620 6e6f 7420 6861 7361 7474 7228 7365  f not hasattr(se
-000292c0: 6c66 2c20 2764 6174 6127 293a 0a20 2020  lf, 'data'):.   
-000292d0: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-000292e0: 6164 4461 7461 2829 0a0a 2020 2020 2020  adData()..      
-000292f0: 2020 7461 626c 6573 546f 436f 6d6d 6974    tablesToCommit
-00029300: 203d 205b 5d0a 2020 2020 2020 2020 6d65   = [].        me
-00029310: 7461 4469 6374 203d 2064 6963 7428 290a  taDict = dict().
-00029320: 2020 2020 2020 2020 6d65 7461 4469 6374          metaDict
-00029330: 5b27 736f 7572 6365 275d 203d 2073 656c  ['source'] = sel
-00029340: 662e 7365 7475 702e 534f 5552 4345 5f49  f.setup.SOURCE_I
-00029350: 440a 2020 2020 2020 2020 6578 636c 7564  D.        exclud
-00029360: 6564 5461 626c 6573 203d 2064 6963 7428  edTables = dict(
-00029370: 290a 2020 2020 2020 2020 6578 636c 7564  ).        exclud
-00029380: 6564 5461 626c 6573 5b27 656d 7074 7927  edTables['empty'
-00029390: 5d20 3d20 6c69 7374 2829 0a20 2020 2020  ] = list().     
-000293a0: 2020 2065 7863 6c75 6465 6454 6162 6c65     excludedTable
-000293b0: 735b 2765 7272 6f72 275d 203d 206c 6973  s['error'] = lis
-000293c0: 7428 290a 2020 2020 2020 2020 6578 636c  t().        excl
-000293d0: 7564 6564 5461 626c 6573 5b27 6578 6973  udedTables['exis
-000293e0: 7473 275d 203d 206c 6973 7428 290a 0a20  ts'] = list().. 
-000293f0: 2020 2020 2020 2066 6f72 206d 6f64 656c         for model
-00029400: 2069 6e20 7365 6c66 2e6d 6170 7069 6e67   in self.mapping
-00029410: 5b27 6d6f 6465 6c27 5d2e 6b65 7973 2829  ['model'].keys()
-00029420: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
-00029430: 6d70 4d6f 203d 2073 656c 662e 6461 7461  mpMo = self.data
-00029440: 2e6c 6f63 5b73 656c 662e 6461 7461 2e6d  .loc[self.data.m
-00029450: 6f64 656c 203d 3d20 6d6f 6465 6c5d 0a20  odel == model]. 
-00029460: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-00029470: 6365 6e61 7269 6f20 696e 2073 656c 662e  cenario in self.
-00029480: 6d61 7070 696e 675b 2773 6365 6e61 7269  mapping['scenari
-00029490: 6f27 5d2e 6b65 7973 2829 3a0a 2020 2020  o'].keys():.    
-000294a0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-000294b0: 4d6f 5363 203d 2074 656d 704d 6f2e 6c6f  MoSc = tempMo.lo
-000294c0: 635b 7365 6c66 2e64 6174 612e 7363 656e  c[self.data.scen
-000294d0: 6172 696f 203d 3d20 7363 656e 6172 696f  ario == scenario
-000294e0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-000294f0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-00029500: 2020 2066 6f72 2076 6172 6961 626c 6520     for variable 
-00029510: 696e 2073 656c 662e 6d61 7070 696e 675b  in self.mapping[
-00029520: 2776 6172 6961 626c 6527 5d2e 6b65 7973  'variable'].keys
-00029530: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00029540: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-00029550: 2020 2020 2020 2020 2074 656d 704d 6f53           tempMoS
-00029560: 6356 6120 3d20 7465 6d70 4d6f 5363 2e6c  cVa = tempMoSc.l
-00029570: 6f63 5b73 656c 662e 6461 7461 2e76 6172  oc[self.data.var
-00029580: 6961 626c 6520 3d3d 2076 6172 6961 626c  iable == variabl
-00029590: 655d 0a0a 2020 2020 2020 2020 2020 2020  e]..            
-000295a0: 2020 2020 7461 626c 6573 203d 2064 742e      tables = dt.
-000295b0: 696e 7465 7266 6163 6573 2e72 6561 645f  interfaces.read_
-000295c0: 6c6f 6e67 5f74 6162 6c65 280a 2020 2020  long_table(.    
-000295d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000295e0: 7465 6d70 4d6f 5363 2c20 6c69 7374 2873  tempMoSc, list(s
-000295f0: 656c 662e 6d61 7070 696e 675b 2776 6172  elf.mapping['var
-00029600: 6961 626c 6527 5d2e 6b65 7973 2829 290a  iable'].keys()).
-00029610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029620: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00029630: 2020 666f 7220 7461 626c 6520 696e 2074    for table in t
-00029640: 6162 6c65 733a 0a20 2020 2020 2020 2020  ables:.         
-00029650: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-00029660: 2e6d 6574 615b 2763 6174 6567 6f72 7927  .meta['category'
-00029670: 5d20 3d20 2222 0a20 2020 2020 2020 2020  ] = "".         
-00029680: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-00029690: 2e6d 6574 615b 2773 6f75 7263 6527 5d20  .meta['source'] 
-000296a0: 3d20 7365 6c66 2e73 6574 7570 2e53 4f55  = self.setup.SOU
-000296b0: 5243 455f 4944 0a20 2020 2020 2020 2020  RCE_ID.         
-000296c0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-000296d0: 2e69 6e64 6578 203d 2074 6162 6c65 2e69  .index = table.i
-000296e0: 6e64 6578 2e6d 6170 2873 656c 662e 6d61  ndex.map(self.ma
-000296f0: 7070 696e 675b 2772 6567 696f 6e27 5d29  pping['region'])
-00029700: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00029710: 2020 2020 2020 7461 626c 6549 4420 3d20        tableID = 
-00029720: 6474 2e63 6f72 652e 5f63 7265 6174 6544  dt.core._createD
-00029730: 6174 6162 6173 6549 4428 7461 626c 652e  atabaseID(table.
-00029740: 6d65 7461 290a 2020 2020 2020 2020 2020  meta).          
-00029750: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00029760: 2075 7064 6174 6554 6162 6c65 733a 0a20   updateTables:. 
-00029770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029780: 2020 2020 2020 2069 6620 6474 2e63 6f72         if dt.cor
-00029790: 652e 4442 2e74 6162 6c65 4578 6973 7428  e.DB.tableExist(
-000297a0: 7461 626c 6549 4429 3a0a 2020 2020 2020  tableID):.      
+00026960: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00026970: 2020 2020 2069 6d70 6f72 7420 636f 7079       import copy
+00026980: 0a0a 2020 2020 2020 2020 666f 7220 6761  ..        for ga
+00026990: 7320 696e 2073 656c 662e 6d61 7070 696e  s in self.mappin
+000269a0: 6744 6963 745b 2767 6173 6573 275d 3a0a  gDict['gases']:.
+000269b0: 2020 2020 2020 2020 2020 2020 6966 2027              if '
+000269c0: 456d 6973 7369 6f6e 737c 2720 2b20 6761  Emissions|' + ga
+000269d0: 7320 2b20 277c 4c55 4c55 4346 2720 696e  s + '|LULUCF' in
+000269e0: 2064 6174 6154 6162 6c65 732e 6b65 7973   dataTables.keys
+000269f0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00026a00: 2020 2020 6461 7461 5461 626c 6573 5b27      dataTables['
+00026a10: 456d 6973 7369 6f6e 737c 2720 2b20 6761  Emissions|' + ga
+00026a20: 7320 2b20 277c 4950 434d 3045 4c27 5d20  s + '|IPCM0EL'] 
+00026a30: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00026a40: 2020 2020 2020 2020 6461 7461 5461 626c          dataTabl
+00026a50: 6573 5b27 456d 6973 7369 6f6e 737c 2720  es['Emissions|' 
+00026a60: 2b20 6761 7320 2b20 277c 4950 4330 275d  + gas + '|IPC0']
+00026a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00026a80: 2020 2020 202d 2064 6174 6154 6162 6c65       - dataTable
+00026a90: 735b 2745 6d69 7373 696f 6e73 7c27 202b  s['Emissions|' +
+00026aa0: 2067 6173 202b 2027 7c4c 554c 5543 4627   gas + '|LULUCF'
+00026ab0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00026ac0: 2020 2920 2023 206e 6174 696f 6e61 6c20    )  # national 
+00026ad0: 746f 7461 6c20 6578 636c 7564 696e 6720  total excluding 
+00026ae0: 6c75 6c75 6366 0a20 2020 2020 2020 2020  lulucf.         
+00026af0: 2020 2020 2020 2064 6174 6154 6162 6c65         dataTable
+00026b00: 735b 2745 6d69 7373 696f 6e73 7c27 202b  s['Emissions|' +
+00026b10: 2067 6173 202b 2027 7c49 5043 4d30 454c   gas + '|IPCM0EL
+00026b20: 275d 2e6d 6574 6120 3d20 636f 7079 2e63  '].meta = copy.c
+00026b30: 6f70 7928 0a20 2020 2020 2020 2020 2020  opy(.           
+00026b40: 2020 2020 2020 2020 2064 6174 6154 6162           dataTab
+00026b50: 6c65 735b 2745 6d69 7373 696f 6e73 7c27  les['Emissions|'
+00026b60: 202b 2067 6173 202b 2027 7c49 5043 3027   + gas + '|IPC0'
+00026b70: 5d2e 6d65 7461 0a20 2020 2020 2020 2020  ].meta.         
+00026b80: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00026b90: 2020 2020 2020 2020 2064 6174 6154 6162           dataTab
+00026ba0: 6c65 735b 2745 6d69 7373 696f 6e73 7c27  les['Emissions|'
+00026bb0: 202b 2067 6173 202b 2027 7c49 5043 4d30   + gas + '|IPCM0
+00026bc0: 454c 275d 2e6d 6574 615b 2763 6174 6567  EL'].meta['categ
+00026bd0: 6f72 7927 5d20 3d20 2249 5043 4d30 454c  ory'] = "IPCM0EL
+00026be0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00026bf0: 2020 6461 7461 5461 626c 6573 5b27 456d    dataTables['Em
+00026c00: 6973 7369 6f6e 737c 2720 2b20 6761 7320  issions|' + gas 
+00026c10: 2b20 277c 4950 4333 275d 203d 2028 0a20  + '|IPC3'] = (. 
+00026c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026c30: 2020 2064 6174 6154 6162 6c65 735b 2745     dataTables['E
+00026c40: 6d69 7373 696f 6e73 7c27 202b 2067 6173  missions|' + gas
+00026c50: 202b 2027 7c49 5043 4d41 4727 5d0a 2020   + '|IPCMAG'].  
+00026c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026c70: 2020 2b20 6461 7461 5461 626c 6573 5b27    + dataTables['
+00026c80: 456d 6973 7369 6f6e 737c 2720 2b20 6761  Emissions|' + ga
+00026c90: 7320 2b20 277c 4c55 4c55 4346 275d 0a20  s + '|LULUCF']. 
+00026ca0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00026cb0: 2020 2320 4146 4f4c 550a 2020 2020 2020    # AFOLU.      
+00026cc0: 2020 2020 2020 2020 2020 6461 7461 5461            dataTa
+00026cd0: 626c 6573 5b27 456d 6973 7369 6f6e 737c  bles['Emissions|
+00026ce0: 2720 2b20 6761 7320 2b20 277c 4950 4333  ' + gas + '|IPC3
+00026cf0: 275d 2e6d 6574 6120 3d20 636f 7079 2e63  '].meta = copy.c
+00026d00: 6f70 7928 0a20 2020 2020 2020 2020 2020  opy(.           
+00026d10: 2020 2020 2020 2020 2064 6174 6154 6162           dataTab
+00026d20: 6c65 735b 2745 6d69 7373 696f 6e73 7c27  les['Emissions|'
+00026d30: 202b 2067 6173 202b 2027 7c49 5043 3027   + gas + '|IPC0'
+00026d40: 5d2e 6d65 7461 0a20 2020 2020 2020 2020  ].meta.         
+00026d50: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00026d60: 2020 2020 2020 2020 2064 6174 6154 6162           dataTab
+00026d70: 6c65 735b 2745 6d69 7373 696f 6e73 7c27  les['Emissions|'
+00026d80: 202b 2067 6173 202b 2027 7c49 5043 3327   + gas + '|IPC3'
+00026d90: 5d2e 6d65 7461 5b27 6361 7465 676f 7279  ].meta['category
+00026da0: 275d 203d 2022 4950 434d 3322 0a0a 2020  '] = "IPCM3"..  
+00026db0: 2020 2020 2020 7461 626c 6573 546f 436f        tablesToCo
+00026dc0: 6d6d 6974 203d 206c 6973 7428 290a 2020  mmit = list().  
+00026dd0: 2020 2020 2020 666f 7220 6b65 7920 696e        for key in
+00026de0: 2064 6174 6154 6162 6c65 732e 6b65 7973   dataTables.keys
+00026df0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00026e00: 6461 7461 5461 626c 6573 5b6b 6579 5d20  dataTables[key] 
+00026e10: 3d20 6461 7461 5461 626c 6573 5b6b 6579  = dataTables[key
+00026e20: 5d2e 6173 7479 7065 2866 6c6f 6174 290a  ].astype(float).
+00026e30: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00026e40: 5461 626c 6573 5b6b 6579 5d2e 6765 6e65  Tables[key].gene
+00026e50: 7261 7465 5461 626c 6549 4428 290a 2020  rateTableID().  
+00026e60: 2020 2020 2020 2020 2020 7461 626c 6573            tables
+00026e70: 546f 436f 6d6d 6974 2e61 7070 656e 6428  ToCommit.append(
+00026e80: 6461 7461 5461 626c 6573 5b6b 6579 5d29  dataTables[key])
+00026e90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00026ea0: 7461 626c 6573 546f 436f 6d6d 6974 0a0a  tablesToCommit..
+00026eb0: 0a63 6c61 7373 2053 4447 5f44 4154 415f  .class SDG_DATA_
+00026ec0: 3230 3139 2842 6173 6549 6d70 6f72 7454  2019(BaseImportT
+00026ed0: 6f6f 6c29 3a0a 2020 2020 6465 6620 5f5f  ool):.    def __
+00026ee0: 696e 6974 5f5f 2873 656c 6629 3a0a 0a20  init__(self):.. 
+00026ef0: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
+00026f00: 7020 3d20 7365 7475 7053 7472 7563 7428  p = setupStruct(
+00026f10: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00026f20: 7365 7475 702e 534f 5552 4345 5f49 4420  setup.SOURCE_ID 
+00026f30: 3d20 2253 4447 5f44 425f 3230 3139 220a  = "SDG_DB_2019".
+00026f40: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00026f50: 7570 2e53 4f55 5243 455f 5041 5448 203d  up.SOURCE_PATH =
+00026f60: 206f 732e 7061 7468 2e6a 6f69 6e28 0a20   os.path.join(. 
+00026f70: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+00026f80: 672e 5041 5448 5f54 4f5f 4441 5441 5348  g.PATH_TO_DATASH
+00026f90: 454c 462c 2027 7261 7764 6174 612f 5344  ELF, 'rawdata/SD
+00026fa0: 475f 4442 5f32 3031 3927 0a20 2020 2020  G_DB_2019'.     
+00026fb0: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+00026fc0: 662e 7365 7475 702e 4441 5441 5f46 494c  f.setup.DATA_FIL
+00026fd0: 4520 3d20 6f73 2e70 6174 682e 6a6f 696e  E = os.path.join
+00026fe0: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+00026ff0: 6c66 2e73 6574 7570 2e53 4f55 5243 455f  lf.setup.SOURCE_
+00027000: 5041 5448 2c20 2765 7874 7261 6374 5f30  PATH, 'extract_0
+00027010: 355f 3230 3139 2e63 7376 270a 2020 2020  5_2019.csv'.    
+00027020: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+00027030: 6c66 2e73 6574 7570 2e4d 4150 5049 4e47  lf.setup.MAPPING
+00027040: 5f46 494c 4520 3d20 6f73 2e70 6174 682e  _FILE = os.path.
+00027050: 6a6f 696e 2873 656c 662e 7365 7475 702e  join(self.setup.
+00027060: 534f 5552 4345 5f50 4154 482c 2027 6d61  SOURCE_PATH, 'ma
+00027070: 7070 696e 672e 786c 7378 2729 0a20 2020  pping.xlsx').   
+00027080: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
+00027090: 4c49 4345 4e43 4520 3d20 276f 7065 6e20  LICENCE = 'open 
+000270a0: 6163 6365 7373 2028 554e 2927 0a20 2020  access (UN)'.   
+000270b0: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
+000270c0: 5552 4c20 3d20 2768 7474 7073 3a2f 2f75  URL = 'https://u
+000270d0: 6e73 7461 7473 2e75 6e2e 6f72 672f 7364  nstats.un.org/sd
+000270e0: 6773 2f69 6e64 6963 6174 6f72 732f 6461  gs/indicators/da
+000270f0: 7461 6261 7365 2f27 0a0a 2020 2020 2020  tabase/'..      
+00027100: 2020 7365 6c66 2e73 6574 7570 2e49 4e44    self.setup.IND
+00027110: 4558 5f43 4f4c 554d 4e5f 4e41 4d45 203d  EX_COLUMN_NAME =
+00027120: 2027 5365 7269 6573 436f 6465 270a 2020   'SeriesCode'.  
+00027130: 2020 2020 2020 7365 6c66 2e73 6574 7570        self.setup
+00027140: 2e53 5041 5449 414c 5f43 4f4c 554d 5f4e  .SPATIAL_COLUM_N
+00027150: 414d 4520 3d20 2747 656f 4172 6561 436f  AME = 'GeoAreaCo
+00027160: 6465 270a 0a20 2020 2020 2020 2073 656c  de'..        sel
+00027170: 662e 7365 7475 702e 434f 4c55 4d4e 535f  f.setup.COLUMNS_
+00027180: 544f 5f44 524f 5020 3d20 5b27 436f 756e  TO_DROP = ['Coun
+00027190: 7472 7920 4e61 6d65 272c 2027 496e 6469  try Name', 'Indi
+000271a0: 6361 746f 7220 4e61 6d65 275d 0a0a 2020  cator Name']..  
+000271b0: 2020 2020 2020 7365 6c66 2e63 7265 6174        self.creat
+000271c0: 6553 6f75 7263 654d 6574 6128 290a 0a20  eSourceMeta().. 
+000271d0: 2020 2020 2020 2069 6620 6e6f 7420 286f         if not (o
+000271e0: 732e 7061 7468 2e65 7869 7374 7328 7365  s.path.exists(se
+000271f0: 6c66 2e73 6574 7570 2e4d 4150 5049 4e47  lf.setup.MAPPING
+00027200: 5f46 494c 4529 293a 0a20 2020 2020 2020  _FILE)):.       
+00027210: 2020 2020 2073 656c 662e 6372 6561 7465       self.create
+00027220: 5661 7269 6162 6c65 4d61 7070 696e 6728  VariableMapping(
+00027230: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00027240: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00027250: 2e6d 6170 7069 6e67 203d 2070 642e 7265  .mapping = pd.re
+00027260: 6164 5f65 7863 656c 280a 2020 2020 2020  ad_excel(.      
+00027270: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00027280: 6574 7570 2e4d 4150 5049 4e47 5f46 494c  etup.MAPPING_FIL
+00027290: 452c 2073 6865 6574 5f6e 616d 653d 5641  E, sheet_name=VA
+000272a0: 525f 4d41 5050 494e 475f 5348 4545 542c  R_MAPPING_SHEET,
+000272b0: 2069 6e64 6578 5f63 6f6c 3d30 0a20 2020   index_col=0.   
+000272c0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+000272d0: 6465 6620 6c6f 6164 4461 7461 2873 656c  def loadData(sel
+000272e0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+000272f0: 2e64 6174 6120 3d20 7064 2e72 6561 645f  .data = pd.read_
+00027300: 6373 7628 7365 6c66 2e73 6574 7570 2e44  csv(self.setup.D
+00027310: 4154 415f 4649 4c45 2c20 6865 6164 6572  ATA_FILE, header
+00027320: 3d30 290a 2020 2020 2020 2020 7365 6c66  =0).        self
+00027330: 2e64 6174 615b 2770 7269 6d61 7279 5f63  .data['primary_c
+00027340: 6f64 6527 5d20 3d20 7365 6c66 2e64 6174  ode'] = self.dat
+00027350: 612e 696e 6465 780a 2020 2020 2020 2020  a.index.        
+00027360: 6d6f 6469 6669 6572 436f 6c75 6d6e 7320  modifierColumns 
+00027370: 3d20 5b73 656c 662e 7365 7475 702e 494e  = [self.setup.IN
+00027380: 4445 585f 434f 4c55 4d4e 5f4e 414d 455d  DEX_COLUMN_NAME]
+00027390: 202b 206c 6973 7428 0a20 2020 2020 2020   + list(.       
+000273a0: 2020 2020 2073 656c 662e 6461 7461 2e63       self.data.c
+000273b0: 6f6c 756d 6e73 5b31 343a 2d31 5d0a 2020  olumns[14:-1].  
+000273c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000273d0: 6d6f 6469 6669 6572 436f 6c75 6d6e 732e  modifierColumns.
+000273e0: 7265 6d6f 7665 2827 5b52 6570 6f72 7469  remove('[Reporti
+000273f0: 6e67 2054 7970 655d 2729 0a20 2020 2020  ng Type]').     
+00027400: 2020 2023 2073 656c 662e 6461 7461 5b6d     # self.data[m
+00027410: 6f64 6966 6965 7243 6f6c 756d 6e73 5d20  odifierColumns] 
+00027420: 3d20 7365 6c66 2e64 6174 615b 6d6f 6469  = self.data[modi
+00027430: 6669 6572 436f 6c75 6d6e 735d 2e66 696c  fierColumns].fil
+00027440: 6c6e 6128 274e 614e 2729 0a20 2020 2020  lna('NaN').     
+00027450: 2020 2023 2073 656c 662e 6461 7461 5b6d     # self.data[m
+00027460: 6f64 6966 6965 7243 6f6c 756d 6e73 5d2e  odifierColumns].
+00027470: 6170 706c 7928 6c61 6d62 6461 2078 3a20  apply(lambda x: 
+00027480: 275f 272e 6a6f 696e 2878 292c 2061 7869  '_'.join(x), axi
+00027490: 733d 3129 0a20 2020 2020 2020 2023 2073  s=1).        # s
+000274a0: 656c 662e 6461 7461 5b6d 6f64 6966 6965  elf.data[modifie
+000274b0: 7243 6f6c 756d 6e73 5d2e 6173 7479 7065  rColumns].astype
+000274c0: 2873 7472 292e 6170 706c 7928 6c61 6d62  (str).apply(lamb
+000274d0: 6461 2078 3a20 782e 7374 722e 6361 7428  da x: x.str.cat(
+000274e0: 7365 703d 275f 2729 2c20 6178 6973 3d31  sep='_'), axis=1
+000274f0: 290a 2020 2020 2020 2020 7365 6c66 2e64  ).        self.d
+00027500: 6174 612e 696e 6465 7820 3d20 280a 2020  ata.index = (.  
+00027510: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00027520: 6174 615b 6d6f 6469 6669 6572 436f 6c75  ata[modifierColu
+00027530: 6d6e 735d 0a20 2020 2020 2020 2020 2020  mns].           
+00027540: 202e 6669 6c6c 6e61 2827 2729 0a20 2020   .fillna('').   
+00027550: 2020 2020 2020 2020 202e 6173 7479 7065           .astype
+00027560: 2873 7472 290a 2020 2020 2020 2020 2020  (str).          
+00027570: 2020 2e61 7070 6c79 286c 616d 6264 6120    .apply(lambda 
+00027580: 783a 2027 5f27 2e6a 6f69 6e28 6669 6c74  x: '_'.join(filt
+00027590: 6572 284e 6f6e 652c 2078 2929 2c20 6178  er(None, x)), ax
+000275a0: 6973 3d31 290a 2020 2020 2020 2020 290a  is=1).        ).
+000275b0: 0a20 2020 2064 6566 2063 7265 6174 6556  .    def createV
+000275c0: 6172 6961 626c 654d 6170 7069 6e67 2873  ariableMapping(s
+000275d0: 656c 6629 3a0a 2020 2020 2020 2020 7772  elf):.        wr
+000275e0: 6974 6572 203d 2070 642e 4578 6365 6c57  iter = pd.ExcelW
+000275f0: 7269 7465 7228 0a20 2020 2020 2020 2020  riter(.         
+00027600: 2020 2073 656c 662e 7365 7475 702e 4d41     self.setup.MA
+00027610: 5050 494e 475f 4649 4c45 2c0a 2020 2020  PPING_FILE,.    
+00027620: 2020 2020 2020 2020 656e 6769 6e65 3d27          engine='
+00027630: 786c 7378 7772 6974 6572 272c 0a20 2020  xlsxwriter',.   
+00027640: 2020 2020 2020 2020 2064 6174 6574 696d           datetim
+00027650: 655f 666f 726d 6174 3d27 6d6d 6d20 6420  e_format='mmm d 
+00027660: 7979 7979 2068 683a 6d6d 3a73 7327 2c0a  yyyy hh:mm:ss',.
+00027670: 2020 2020 2020 2020 2020 2020 6461 7465              date
+00027680: 5f66 6f72 6d61 743d 276d 6d6d 6d20 6464  _format='mmmm dd
+00027690: 2079 7979 7927 2c0a 2020 2020 2020 2020   yyyy',.        
+000276a0: 290a 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
+000276b0: 7420 6861 7361 7474 7228 7365 6c66 2c20  t hasattr(self, 
+000276c0: 2764 6174 6127 293a 0a20 2020 2020 2020  'data'):.       
+000276d0: 2020 2020 2023 2020 2020 2020 2020 2020       #          
+000276e0: 2020 7365 6c66 2e64 6174 6120 3d20 7064    self.data = pd
+000276f0: 2e72 6561 645f 6373 7628 7365 6c66 2e73  .read_csv(self.s
+00027700: 6574 7570 2e44 4154 415f 4649 4c45 2c20  etup.DATA_FILE, 
+00027710: 656e 636f 6469 6e67 3d27 7574 6638 272c  encoding='utf8',
+00027720: 2065 6e67 696e 653d 2770 7974 686f 6e27   engine='python'
+00027730: 2c20 696e 6465 785f 636f 6c20 3d20 4e6f  , index_col = No
+00027740: 6e65 2c20 6865 6164 6572 203d 302c 206e  ne, header =0, n
+00027750: 615f 7661 6c75 6573 3d27 2e2e 2729 0a20  a_values='..'). 
+00027760: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+00027770: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
+00027780: 615b 2763 6f6d 6269 6e65 6427 5d20 3d20  a['combined'] = 
+00027790: 7365 6c66 2e64 6174 615b 7365 6c66 2e73  self.data[self.s
+000277a0: 6574 7570 2e49 4e44 4558 5f43 4f4c 554d  etup.INDEX_COLUM
+000277b0: 4e5f 4e41 4d45 5d2e 6170 706c 7928 6c61  N_NAME].apply(la
+000277c0: 6d62 6461 2078 3a20 275f 272e 6a6f 696e  mbda x: '_'.join
+000277d0: 2878 292c 2061 7869 733d 3129 0a20 2020  (x), axis=1).   
+000277e0: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
+000277f0: 6164 4461 7461 2829 0a0a 2020 2020 2020  adData()..      
+00027800: 2020 2320 7365 6c66 2e64 6174 615b 7365    # self.data[se
+00027810: 6c66 2e73 6574 7570 2e49 4e44 4558 5f43  lf.setup.INDEX_C
+00027820: 4f4c 554d 4e5f 4e41 4d45 5d2e 6170 706c  OLUMN_NAME].appl
+00027830: 7928 6c61 6d62 6461 2078 3a20 275f 272e  y(lambda x: '_'.
+00027840: 6a6f 696e 2878 292c 2061 7869 733d 3129  join(x), axis=1)
+00027850: 0a20 2020 2020 2020 2061 7661 696c 6162  .        availab
+00027860: 6c65 5365 7269 6573 203d 2073 656c 662e  leSeries = self.
+00027870: 6461 7461 2e69 6e64 6578 2e75 6e69 7175  data.index.uniqu
+00027880: 6528 290a 2020 2020 2020 2020 6465 7363  e().        desc
+00027890: 7244 6620 3d20 7365 6c66 2e64 6174 615b  rDf = self.data[
+000278a0: 2753 6572 6965 7344 6573 6372 6970 7469  'SeriesDescripti
+000278b0: 6f6e 275d 2e64 726f 705f 6475 706c 6963  on'].drop_duplic
+000278c0: 6174 6573 2829 0a0a 2020 2020 2020 2020  ates()..        
+000278d0: 7365 6c66 2e6d 6170 7069 6e67 203d 2070  self.mapping = p
+000278e0: 642e 4461 7461 4672 616d 6528 0a20 2020  d.DataFrame(.   
+000278f0: 2020 2020 2020 2020 2069 6e64 6578 3d61           index=a
+00027900: 7661 696c 6162 6c65 5365 7269 6573 2c20  vailableSeries, 
+00027910: 636f 6c75 6d6e 733d 4d41 5050 494e 475f  columns=MAPPING_
+00027920: 434f 4c55 4d4e 5320 2b20 5b27 6465 7363  COLUMNS + ['desc
+00027930: 7269 7074 696f 6e27 5d0a 2020 2020 2020  ription'].      
+00027940: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+00027950: 2e6d 6170 7069 6e67 2e73 6f75 7263 6520  .mapping.source 
+00027960: 3d20 7365 6c66 2e73 6574 7570 2e53 4f55  = self.setup.SOU
+00027970: 5243 455f 4944 0a20 2020 2020 2020 2073  RCE_ID.        s
+00027980: 656c 662e 6d61 7070 696e 672e 7363 656e  elf.mapping.scen
+00027990: 6172 696f 203d 2027 6869 7374 6f72 6963  ario = 'historic
+000279a0: 270a 2020 2020 2020 2020 7365 6c66 2e6d  '.        self.m
+000279b0: 6170 7069 6e67 2e64 6573 6372 6970 7469  apping.descripti
+000279c0: 6f6e 203d 2064 6573 6372 4466 0a20 2020  on = descrDf.   
+000279d0: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
+000279e0: 672e 6465 7363 7269 7074 696f 6e20 3d20  g.description = 
+000279f0: 7365 6c66 2e6d 6170 7069 6e67 2e64 6573  self.mapping.des
+00027a00: 6372 6970 7469 6f6e 2e66 696c 6c6e 6128  cription.fillna(
+00027a10: 6d65 7468 6f64 3d27 6666 696c 6c27 290a  method='ffill').
+00027a20: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
+00027a30: 7069 6e67 2e74 6f5f 6578 6365 6c28 7772  ping.to_excel(wr
+00027a40: 6974 6572 2c20 7368 6565 745f 6e61 6d65  iter, sheet_name
+00027a50: 3d56 4152 5f4d 4150 5049 4e47 5f53 4845  =VAR_MAPPING_SHE
+00027a60: 4554 290a 2020 2020 2020 2020 7772 6974  ET).        writ
+00027a70: 6572 2e63 6c6f 7365 2829 0a0a 2020 2020  er.close()..    
+00027a80: 6465 6620 6761 7468 6572 4d61 7070 6564  def gatherMapped
+00027a90: 4461 7461 2873 656c 662c 2073 7061 7469  Data(self, spati
+00027aa0: 616c 5375 6253 6574 3d4e 6f6e 6529 3a0a  alSubSet=None):.
+00027ab0: 2020 2020 2020 2020 2320 6c6f 6164 696e          # loadin
+00027ac0: 6720 6461 7461 2069 6620 6e65 6365 7373  g data if necess
+00027ad0: 6172 790a 2020 2020 2020 2020 6966 206e  ary.        if n
+00027ae0: 6f74 2068 6173 6174 7472 2873 656c 662c  ot hasattr(self,
+00027af0: 2027 6461 7461 2729 3a0a 2020 2020 2020   'data'):.      
+00027b00: 2020 2020 2020 7365 6c66 2e6c 6f61 6444        self.loadD
+00027b10: 6174 6128 290a 0a20 2020 2020 2020 2069  ata()..        i
+00027b20: 6e64 6578 4461 7461 546f 436f 6c6c 6563  ndexDataToCollec
+00027b30: 7420 3d20 7365 6c66 2e6d 6170 7069 6e67  t = self.mapping
+00027b40: 2e69 6e64 6578 5b7e 7064 2e69 736e 756c  .index[~pd.isnul
+00027b50: 6c28 7365 6c66 2e6d 6170 7069 6e67 5b27  l(self.mapping['
+00027b60: 656e 7469 7479 275d 295d 0a0a 2020 2020  entity'])]..    
+00027b70: 2020 2020 7461 626c 6573 546f 436f 6d6d      tablesToComm
+00027b80: 6974 203d 205b 5d0a 2020 2020 2020 2020  it = [].        
+00027b90: 666f 7220 6964 7820 696e 2069 6e64 6578  for idx in index
+00027ba0: 4461 7461 546f 436f 6c6c 6563 743a 0a20  DataToCollect:. 
+00027bb0: 2020 2020 2020 2020 2020 206d 6574 6144             metaD
+00027bc0: 6620 3d20 7365 6c66 2e6d 6170 7069 6e67  f = self.mapping
+00027bd0: 2e6c 6f63 5b69 6478 5d0a 2020 2020 2020  .loc[idx].      
+00027be0: 2020 2020 2020 7072 696e 7428 6964 7829        print(idx)
+00027bf0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00027c00: 7072 696e 7428 6d65 7461 4466 5b63 6f6e  print(metaDf[con
+00027c10: 6669 672e 5245 5155 4952 4544 5f4d 4554  fig.REQUIRED_MET
+00027c20: 415f 4649 454c 4453 5d2e 6973 6e75 6c6c  A_FIELDS].isnull
+00027c30: 2829 2e61 6c6c 2829 203d 3d20 4661 6c73  ().all() == Fals
+00027c40: 6529 0a20 2020 2020 2020 2020 2020 2023  e).            #
+00027c50: 2070 7269 6e74 286d 6574 6144 6174 615b   print(metaData[
+00027c60: 7365 6c66 2e73 6574 7570 2e49 4e44 4558  self.setup.INDEX
+00027c70: 5f43 4f4c 554d 4e5f 4e41 4d45 5d29 0a0a  _COLUMN_NAME])..
+00027c80: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+00027c90: 4469 6374 203d 207b 0a20 2020 2020 2020  Dict = {.       
+00027ca0: 2020 2020 2020 2020 206b 6579 3a20 6d65           key: me
+00027cb0: 7461 4466 5b6b 6579 5d0a 2020 2020 2020  taDf[key].      
+00027cc0: 2020 2020 2020 2020 2020 666f 7220 6b65            for ke
+00027cd0: 7920 696e 2063 6f6e 6669 672e 5245 5155  y in config.REQU
+00027ce0: 4952 4544 5f4d 4554 415f 4649 454c 4453  IRED_META_FIELDS
+00027cf0: 2e75 6e69 6f6e 287b 2775 6e69 7454 6f27  .union({'unitTo'
+00027d00: 7d29 0a20 2020 2020 2020 2020 2020 207d  }).            }
+00027d10: 0a0a 2020 2020 2020 2020 2020 2020 6d65  ..            me
+00027d20: 7461 4469 6374 5b27 6f72 6967 696e 616c  taDict['original
+00027d30: 2063 6f64 6527 5d20 3d20 6964 780a 2020   code'] = idx.  
+00027d40: 2020 2020 2020 2020 2020 2320 6d65 7461            # meta
+00027d50: 4469 6374 5b27 6f72 6967 696e 616c 206e  Dict['original n
+00027d60: 616d 6527 5d20 3d20 6d65 7461 4466 5b27  ame'] = metaDf['
+00027d70: 496e 6469 6361 746f 7220 4e61 6d65 275d  Indicator Name']
+00027d80: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00027d90: 7269 6573 4964 7820 3d20 6964 780a 0a20  riesIdx = idx.. 
+00027da0: 2020 2020 2020 2020 2020 2064 6174 6166             dataf
+00027db0: 7261 6d65 203d 2073 656c 662e 6461 7461  rame = self.data
+00027dc0: 2e6c 6f63 5b73 6572 6965 7349 6478 2c20  .loc[seriesIdx, 
+00027dd0: 5b27 4765 6f41 7265 6143 6f64 6527 2c20  ['GeoAreaCode', 
+00027de0: 2754 696d 6550 6572 696f 6427 2c20 2756  'TimePeriod', 'V
+00027df0: 616c 7565 275d 5d0a 2020 2020 2020 2020  alue']].        
+00027e00: 2020 2020 6461 7461 6672 616d 6520 3d20      dataframe = 
+00027e10: 6461 7461 6672 616d 652e 7069 766f 7428  dataframe.pivot(
+00027e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00027e30: 2069 6e64 6578 3d27 4765 6f41 7265 6143   index='GeoAreaC
+00027e40: 6f64 6527 2c20 636f 6c75 6d6e 733d 2754  ode', columns='T
+00027e50: 696d 6550 6572 696f 6427 2c20 7661 6c75  imePeriod', valu
+00027e60: 6573 3d27 5661 6c75 6527 0a20 2020 2020  es='Value'.     
+00027e70: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00027e80: 2020 2020 2020 6461 7461 6672 616d 6520        dataframe 
+00027e90: 3d20 6461 7461 6672 616d 652e 6173 7479  = dataframe.asty
+00027ea0: 7065 2866 6c6f 6174 290a 0a20 2020 2020  pe(float)..     
+00027eb0: 2020 2020 2020 206e 6577 4461 7461 203d         newData =
+00027ec0: 206c 6973 7428 290a 2020 2020 2020 2020   list().        
+00027ed0: 2020 2020 666f 7220 6952 6f77 2069 6e20      for iRow in 
+00027ee0: 7261 6e67 6528 6c65 6e28 6461 7461 6672  range(len(datafr
+00027ef0: 616d 6529 293a 0a20 2020 2020 2020 2020  ame)):.         
+00027f00: 2020 2020 2020 2049 534f 5f49 4420 3d20         ISO_ID = 
+00027f10: 6474 2e6d 6170 702e 6765 7453 7061 7469  dt.mapp.getSpati
+00027f20: 616c 4944 2864 6174 6166 7261 6d65 2e69  alID(dataframe.i
+00027f30: 6e64 6578 5b69 526f 775d 290a 2020 2020  ndex[iRow]).    
+00027f40: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+00027f50: 6174 6166 7261 6d65 2e69 6e64 6578 5b69  ataframe.index[i
+00027f60: 526f 775d 203d 3d20 313a 0a20 2020 2020  Row] == 1:.     
+00027f70: 2020 2020 2020 2020 2020 2020 2020 2049                 I
+00027f80: 534f 5f49 4420 3d20 2257 6f72 6c64 220a  SO_ID = "World".
+00027f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027fa0: 6966 2049 534f 5f49 443a 0a20 2020 2020  if ISO_ID:.     
+00027fb0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00027fc0: 6577 4461 7461 2e61 7070 656e 6428 4953  ewData.append(IS
+00027fd0: 4f5f 4944 290a 2020 2020 2020 2020 2020  O_ID).          
+00027fe0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00027ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028000: 6e65 7744 6174 612e 6170 7065 6e64 2870  newData.append(p
+00028010: 642e 6e70 2e6e 616e 290a 2020 2020 2020  d.np.nan).      
+00028020: 2020 2020 2020 6461 7461 6672 616d 652e        dataframe.
+00028030: 696e 6465 7820 3d20 6e65 7744 6174 610a  index = newData.
+00028040: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00028050: 7370 6174 6961 6c53 7562 5365 743a 0a20  spatialSubSet:. 
+00028060: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00028070: 7061 7449 6478 203d 2064 6174 6166 7261  patIdx = datafra
+00028080: 6d65 2e69 6e64 6578 2e69 7369 6e28 7370  me.index.isin(sp
+00028090: 6174 6961 6c53 7562 5365 7429 0a20 2020  atialSubSet).   
+000280a0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+000280b0: 6166 7261 6d65 203d 2064 6174 6166 7261  aframe = datafra
+000280c0: 6d65 2e6c 6f63 5b73 7061 7449 6478 5d0a  me.loc[spatIdx].
+000280d0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+000280e0: 6166 7261 6d65 203d 2064 6174 6166 7261  aframe = datafra
+000280f0: 6d65 2e64 726f 706e 6128 6178 6973 3d31  me.dropna(axis=1
+00028100: 2c20 686f 773d 2761 6c6c 2729 0a20 2020  , how='all').   
+00028110: 2020 2020 2020 2020 2064 6174 6166 7261           datafra
+00028120: 6d65 203d 2064 6174 6166 7261 6d65 2e6c  me = dataframe.l
+00028130: 6f63 5b7e 7064 2e69 736e 6128 6461 7461  oc[~pd.isna(data
+00028140: 6672 616d 652e 696e 6465 7829 5d0a 2020  frame.index)].  
+00028150: 2020 2020 2020 2020 2020 6461 7461 5461            dataTa
+00028160: 626c 6520 3d20 4461 7461 7461 626c 6528  ble = Datatable(
+00028170: 6461 7461 6672 616d 652c 206d 6574 613d  dataframe, meta=
+00028180: 6d65 7461 4469 6374 290a 2020 2020 2020  metaDict).      
+00028190: 2020 2020 2020 2320 706f 7373 6962 6c65        # possible
+000281a0: 2072 6571 7569 7265 6420 756e 6974 2063   required unit c
+000281b0: 6f6e 7665 7273 696f 6e0a 2020 2020 2020  onversion.      
+000281c0: 2020 2020 2020 6966 206e 6f74 2070 642e        if not pd.
+000281d0: 6973 6e61 286d 6574 6144 6963 745b 2775  isna(metaDict['u
+000281e0: 6e69 7454 6f27 5d29 3a0a 2020 2020 2020  nitTo']):.      
+000281f0: 2020 2020 2020 2020 2020 6461 7461 5461            dataTa
+00028200: 626c 6520 3d20 6461 7461 5461 626c 652e  ble = dataTable.
+00028210: 636f 6e76 6572 7428 6d65 7461 4469 6374  convert(metaDict
+00028220: 5b27 756e 6974 546f 275d 290a 2020 2020  ['unitTo']).    
+00028230: 2020 2020 2020 2020 7461 626c 6573 546f          tablesTo
+00028240: 436f 6d6d 6974 2e61 7070 656e 6428 6461  Commit.append(da
+00028250: 7461 5461 626c 6529 0a0a 2020 2020 2020  taTable)..      
+00028260: 2020 7265 7475 726e 2074 6162 6c65 7354    return tablesT
+00028270: 6f43 6f6d 6d69 740a 0a0a 636c 6173 7320  oCommit...class 
+00028280: 484f 4553 4c59 3230 3138 2842 6173 6549  HOESLY2018(BaseI
+00028290: 6d70 6f72 7454 6f6f 6c29 3a0a 2020 2020  mportTool):.    
+000282a0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+000282b0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+000282c0: 2e73 6574 7570 203d 2073 6574 7570 5374  .setup = setupSt
+000282d0: 7275 6374 2829 0a20 2020 2020 2020 2073  ruct().        s
+000282e0: 656c 662e 7365 7475 702e 534f 5552 4345  elf.setup.SOURCE
+000282f0: 5f49 4420 3d20 2248 4f45 534c 5932 3031  _ID = "HOESLY201
+00028300: 3822 0a20 2020 2020 2020 2073 656c 662e  8".        self.
+00028310: 7365 7475 702e 534f 5552 4345 5f50 4154  setup.SOURCE_PAT
+00028320: 4820 3d20 6f73 2e70 6174 682e 6a6f 696e  H = os.path.join
+00028330: 280a 2020 2020 2020 2020 2020 2020 636f  (.            co
+00028340: 6e66 6967 2e50 4154 485f 544f 5f44 4154  nfig.PATH_TO_DAT
+00028350: 4153 4845 4c46 2c20 2772 6177 6461 7461  ASHELF, 'rawdata
+00028360: 2f48 4f45 534c 5932 3031 3827 0a20 2020  /HOESLY2018'.   
+00028370: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+00028380: 656c 662e 7365 7475 702e 4441 5441 5f46  elf.setup.DATA_F
+00028390: 494c 4520 3d20 6f73 2e70 6174 682e 6a6f  ILE = os.path.jo
+000283a0: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
+000283b0: 7365 6c66 2e73 6574 7570 2e53 4f55 5243  self.setup.SOURC
+000283c0: 455f 5041 5448 2c20 2763 6f6d 7069 6c65  E_PATH, 'compile
+000283d0: 645f 7261 775f 686f 6573 6c79 2e63 7376  d_raw_hoesly.csv
+000283e0: 270a 2020 2020 2020 2020 290a 2020 2020  '.        ).    
+000283f0: 2020 2020 7365 6c66 2e73 6574 7570 2e4d      self.setup.M
+00028400: 4150 5049 4e47 5f46 494c 4520 3d20 6f73  APPING_FILE = os
+00028410: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
+00028420: 7365 7475 702e 534f 5552 4345 5f50 4154  setup.SOURCE_PAT
+00028430: 482c 2027 6d61 7070 696e 672e 786c 7378  H, 'mapping.xlsx
+00028440: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+00028450: 7365 7475 702e 4c49 4345 4e43 4520 3d20  setup.LICENCE = 
+00028460: 2720 4372 6561 7469 7665 2043 6f6d 6d6f  ' Creative Commo
+00028470: 6e73 2041 7474 7269 6275 7469 6f6e 2033  ns Attribution 3
+00028480: 2e30 204c 6963 656e 7365 270a 2020 2020  .0 License'.    
+00028490: 2020 2020 7365 6c66 2e73 6574 7570 2e55      self.setup.U
+000284a0: 524c 203d 2027 6874 7470 733a 2f2f 7777  RL = 'https://ww
+000284b0: 772e 6765 6f73 6369 2d6d 6f64 656c 2d64  w.geosci-model-d
+000284c0: 6576 2e6e 6574 2f31 312f 3336 392f 3230  ev.net/11/369/20
+000284d0: 3138 2f27 0a0a 2020 2020 2020 2020 7365  18/'..        se
+000284e0: 6c66 2e73 6574 7570 2e4d 4f44 454c 5f43  lf.setup.MODEL_C
+000284f0: 4f4c 554d 4e5f 4e41 4d45 203d 2027 6d6f  OLUMN_NAME = 'mo
+00028500: 6465 6c27 0a20 2020 2020 2020 2073 656c  del'.        sel
+00028510: 662e 7365 7475 702e 5343 454e 4152 494f  f.setup.SCENARIO
+00028520: 5f43 4f4c 554d 4e5f 4e41 4d45 203d 2027  _COLUMN_NAME = '
+00028530: 7363 656e 6172 696f 270a 2020 2020 2020  scenario'.      
+00028540: 2020 7365 6c66 2e73 6574 7570 2e52 4547    self.setup.REG
+00028550: 494f 4e5f 434f 4c55 4d4e 5f4e 414d 4520  ION_COLUMN_NAME 
+00028560: 3d20 2772 6567 696f 6e27 0a20 2020 2020  = 'region'.     
+00028570: 2020 2073 656c 662e 7365 7475 702e 5641     self.setup.VA
+00028580: 5249 4142 4c45 5f43 4f4c 554d 4e5f 4e41  RIABLE_COLUMN_NA
+00028590: 4d45 203d 2027 7661 7269 6162 6c65 270a  ME = 'variable'.
+000285a0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000285b0: 286f 732e 7061 7468 2e65 7869 7374 7328  (os.path.exists(
+000285c0: 7365 6c66 2e73 6574 7570 2e4d 4150 5049  self.setup.MAPPI
+000285d0: 4e47 5f46 494c 4529 293a 0a20 2020 2020  NG_FILE)):.     
+000285e0: 2020 2020 2020 2073 656c 662e 6372 6561         self.crea
+000285f0: 7465 5661 7269 6162 6c65 4d61 7070 696e  teVariableMappin
+00028600: 6728 290a 2020 2020 2020 2020 2020 2020  g().            
+00028610: 7072 696e 7428 226e 6f20 6d61 7070 696e  print("no mappin
+00028620: 6720 6669 6c65 2066 6f75 6e64 2229 0a20  g file found"). 
+00028630: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00028640: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+00028650: 7070 696e 6720 3d20 6469 6374 2829 0a0a  pping = dict()..
+00028660: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00028670: 7661 7220 696e 205b 2776 6172 6961 626c  var in ['variabl
+00028680: 6527 2c20 2773 6365 6e61 7269 6f27 2c20  e', 'scenario', 
+00028690: 276d 6f64 656c 272c 2027 7265 6769 6f6e  'model', 'region
+000286a0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+000286b0: 2020 2020 6466 203d 2070 642e 7265 6164      df = pd.read
+000286c0: 5f65 7863 656c 280a 2020 2020 2020 2020  _excel(.        
+000286d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000286e0: 2e73 6574 7570 2e4d 4150 5049 4e47 5f46  .setup.MAPPING_F
+000286f0: 494c 452c 2073 6865 6574 5f6e 616d 653d  ILE, sheet_name=
+00028700: 7661 7220 2b20 275f 6d61 7070 696e 6727  var + '_mapping'
+00028710: 2c20 696e 6465 785f 636f 6c3d 300a 2020  , index_col=0.  
+00028720: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00028730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028740: 6466 203d 2064 662e 6c6f 635b 7e64 662e  df = df.loc[~df.
+00028750: 6c6f 635b 3a2c 2076 6172 5d2e 6973 6e61  loc[:, var].isna
+00028760: 2829 5d0a 2020 2020 2020 2020 2020 2020  ()].            
+00028770: 2020 2020 7365 6c66 2e6d 6170 7069 6e67      self.mapping
+00028780: 2e75 7064 6174 6528 6466 2e74 6f5f 6469  .update(df.to_di
+00028790: 6374 2829 290a 0a20 2020 2020 2020 2073  ct())..        s
+000287a0: 656c 662e 6372 6561 7465 536f 7572 6365  elf.createSource
+000287b0: 4d65 7461 2829 0a0a 2020 2020 6465 6620  Meta()..    def 
+000287c0: 6c6f 6164 4461 7461 2873 656c 6629 3a0a  loadData(self):.
+000287d0: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
+000287e0: 6120 3d20 7064 2e72 6561 645f 6373 7628  a = pd.read_csv(
+000287f0: 7365 6c66 2e73 6574 7570 2e44 4154 415f  self.setup.DATA_
+00028800: 4649 4c45 2c20 696e 6465 785f 636f 6c3d  FILE, index_col=
+00028810: 4e6f 6e65 2c20 6865 6164 6572 3d30 290a  None, header=0).
+00028820: 0a20 2020 2064 6566 2063 7265 6174 6556  .    def createV
+00028830: 6172 6961 626c 654d 6170 7069 6e67 2873  ariableMapping(s
+00028840: 656c 6629 3a0a 0a20 2020 2020 2020 2023  elf):..        #
+00028850: 206c 6f61 6469 6e67 2064 6174 6120 6966   loading data if
+00028860: 206e 6563 6573 7361 7279 0a20 2020 2020   necessary.     
+00028870: 2020 2069 6620 6e6f 7420 6861 7361 7474     if not hasatt
+00028880: 7228 7365 6c66 2c20 2764 6174 6127 293a  r(self, 'data'):
+00028890: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000288a0: 662e 6c6f 6164 4461 7461 2829 0a0a 2020  f.loadData()..  
+000288b0: 2020 2020 2020 696d 706f 7274 206e 756d        import num
+000288c0: 7079 2061 7320 6e70 0a0a 2020 2020 2020  py as np..      
+000288d0: 2020 7772 6974 6572 203d 2070 642e 4578    writer = pd.Ex
+000288e0: 6365 6c57 7269 7465 7228 0a20 2020 2020  celWriter(.     
+000288f0: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
+00028900: 702e 4d41 5050 494e 475f 4649 4c45 2c0a  p.MAPPING_FILE,.
+00028910: 2020 2020 2020 2020 2020 2020 656e 6769              engi
+00028920: 6e65 3d27 786c 7378 7772 6974 6572 272c  ne='xlsxwriter',
+00028930: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00028940: 6574 696d 655f 666f 726d 6174 3d27 6d6d  etime_format='mm
+00028950: 6d20 6420 7979 7979 2068 683a 6d6d 3a73  m d yyyy hh:mm:s
+00028960: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
+00028970: 6461 7465 5f66 6f72 6d61 743d 276d 6d6d  date_format='mmm
+00028980: 6d20 6464 2079 7979 7927 2c0a 2020 2020  m dd yyyy',.    
+00028990: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
+000289a0: 2076 6172 6961 626c 6573 0a20 2020 2020   variables.     
+000289b0: 2020 2023 2069 6e64 6578 203d 2073 656c     # index = sel
+000289c0: 662e 6461 7461 5b73 656c 662e 7365 7475  f.data[self.setu
+000289d0: 702e 5641 5249 4142 4c45 5f43 4f4c 554d  p.VARIABLE_COLUM
+000289e0: 4e5f 4e41 4d45 5d2e 756e 6971 7565 2829  N_NAME].unique()
+000289f0: 0a20 2020 2020 2020 2073 656c 662e 6176  .        self.av
+00028a00: 6169 6c61 626c 6553 6572 6965 7320 3d20  ailableSeries = 
+00028a10: 7365 6c66 2e64 6174 612e 6472 6f70 5f64  self.data.drop_d
+00028a20: 7570 6c69 6361 7465 7328 2776 6172 6961  uplicates('varia
+00028a30: 626c 6527 292e 7365 745f 696e 6465 7828  ble').set_index(
+00028a40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00028a50: 662e 7365 7475 702e 5641 5249 4142 4c45  f.setup.VARIABLE
+00028a60: 5f43 4f4c 554d 4e5f 4e41 4d45 0a20 2020  _COLUMN_NAME.   
+00028a70: 2020 2020 2029 5b27 756e 6974 275d 0a20       )['unit']. 
+00028a80: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
+00028a90: 696e 6720 3d20 7064 2e44 6174 6146 7261  ing = pd.DataFra
+00028aa0: 6d65 280a 2020 2020 2020 2020 2020 2020  me(.            
+00028ab0: 696e 6465 783d 7365 6c66 2e61 7661 696c  index=self.avail
+00028ac0: 6162 6c65 5365 7269 6573 2e69 6e64 6578  ableSeries.index
+00028ad0: 2c20 636f 6c75 6d6e 733d 5b73 656c 662e  , columns=[self.
+00028ae0: 7365 7475 702e 5641 5249 4142 4c45 5f43  setup.VARIABLE_C
+00028af0: 4f4c 554d 4e5f 4e41 4d45 5d0a 2020 2020  OLUMN_NAME].    
+00028b00: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+00028b10: 6c66 2e6d 6170 7069 6e67 203d 2070 642e  lf.mapping = pd.
+00028b20: 636f 6e63 6174 285b 7365 6c66 2e6d 6170  concat([self.map
+00028b30: 7069 6e67 2c20 7365 6c66 2e61 7661 696c  ping, self.avail
+00028b40: 6162 6c65 5365 7269 6573 5d2c 2061 7869  ableSeries], axi
+00028b50: 733d 3129 0a20 2020 2020 2020 2073 656c  s=1).        sel
+00028b60: 662e 6d61 7070 696e 6720 3d20 7365 6c66  f.mapping = self
+00028b70: 2e6d 6170 7069 6e67 2e73 6f72 745f 696e  .mapping.sort_in
+00028b80: 6465 7828 290a 2020 2020 2020 2020 7365  dex().        se
+00028b90: 6c66 2e6d 6170 7069 6e67 2e74 6f5f 6578  lf.mapping.to_ex
+00028ba0: 6365 6c28 7772 6974 6572 2c20 656e 6769  cel(writer, engi
+00028bb0: 6e65 3d27 6f70 656e 7079 786c 272c 2073  ne='openpyxl', s
+00028bc0: 6865 6574 5f6e 616d 653d 5641 525f 4d41  heet_name=VAR_MA
+00028bd0: 5050 494e 475f 5348 4545 5429 0a0a 2020  PPING_SHEET)..  
+00028be0: 2020 2020 2020 2320 6d6f 6465 6c73 0a20        # models. 
+00028bf0: 2020 2020 2020 2069 6e64 6578 203d 206e         index = n
+00028c00: 702e 756e 6971 7565 2873 656c 662e 6461  p.unique(self.da
+00028c10: 7461 5b73 656c 662e 7365 7475 702e 4d4f  ta[self.setup.MO
+00028c20: 4445 4c5f 434f 4c55 4d4e 5f4e 414d 455d  DEL_COLUMN_NAME]
+00028c30: 2e76 616c 7565 7329 0a0a 2020 2020 2020  .values)..      
+00028c40: 2020 7365 6c66 2e61 7661 696c 6162 6c65    self.available
+00028c50: 5365 7269 6573 203d 2070 642e 4461 7461  Series = pd.Data
+00028c60: 4672 616d 6528 696e 6465 783d 696e 6465  Frame(index=inde
+00028c70: 7829 0a20 2020 2020 2020 2073 656c 662e  x).        self.
+00028c80: 6d61 7070 696e 6720 3d20 7064 2e44 6174  mapping = pd.Dat
+00028c90: 6146 7261 6d65 2869 6e64 6578 3d69 6e64  aFrame(index=ind
+00028ca0: 6578 2c20 636f 6c75 6d6e 733d 5b73 656c  ex, columns=[sel
+00028cb0: 662e 7365 7475 702e 4d4f 4445 4c5f 434f  f.setup.MODEL_CO
+00028cc0: 4c55 4d4e 5f4e 414d 455d 290a 2020 2020  LUMN_NAME]).    
+00028cd0: 2020 2020 7365 6c66 2e6d 6170 7069 6e67      self.mapping
+00028ce0: 203d 2070 642e 636f 6e63 6174 285b 7365   = pd.concat([se
+00028cf0: 6c66 2e6d 6170 7069 6e67 2c20 7365 6c66  lf.mapping, self
+00028d00: 2e61 7661 696c 6162 6c65 5365 7269 6573  .availableSeries
+00028d10: 5d2c 2061 7869 733d 3129 0a20 2020 2020  ], axis=1).     
+00028d20: 2020 2073 656c 662e 6d61 7070 696e 6720     self.mapping 
+00028d30: 3d20 7365 6c66 2e6d 6170 7069 6e67 2e73  = self.mapping.s
+00028d40: 6f72 745f 696e 6465 7828 290a 0a20 2020  ort_index()..   
+00028d50: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
+00028d60: 672e 746f 5f65 7863 656c 2877 7269 7465  g.to_excel(write
+00028d70: 722c 2065 6e67 696e 653d 276f 7065 6e70  r, engine='openp
+00028d80: 7978 6c27 2c20 7368 6565 745f 6e61 6d65  yxl', sheet_name
+00028d90: 3d27 6d6f 6465 6c5f 6d61 7070 696e 6727  ='model_mapping'
+00028da0: 290a 0a20 2020 2020 2020 2023 2073 6365  )..        # sce
+00028db0: 6e61 7269 6f73 0a20 2020 2020 2020 2069  narios.        i
+00028dc0: 6e64 6578 203d 206e 702e 756e 6971 7565  ndex = np.unique
+00028dd0: 2873 656c 662e 6461 7461 5b73 656c 662e  (self.data[self.
+00028de0: 7365 7475 702e 5343 454e 4152 494f 5f43  setup.SCENARIO_C
+00028df0: 4f4c 554d 4e5f 4e41 4d45 5d2e 7661 6c75  OLUMN_NAME].valu
+00028e00: 6573 290a 0a20 2020 2020 2020 2073 656c  es)..        sel
+00028e10: 662e 6176 6169 6c61 626c 6553 6572 6965  f.availableSerie
+00028e20: 7320 3d20 7064 2e44 6174 6146 7261 6d65  s = pd.DataFrame
+00028e30: 2869 6e64 6578 3d69 6e64 6578 290a 2020  (index=index).  
+00028e40: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
+00028e50: 6e67 203d 2070 642e 4461 7461 4672 616d  ng = pd.DataFram
+00028e60: 6528 0a20 2020 2020 2020 2020 2020 2069  e(.            i
+00028e70: 6e64 6578 3d69 6e64 6578 2c20 636f 6c75  ndex=index, colu
+00028e80: 6d6e 733d 5b73 656c 662e 7365 7475 702e  mns=[self.setup.
+00028e90: 5343 454e 4152 494f 5f43 4f4c 554d 4e5f  SCENARIO_COLUMN_
+00028ea0: 4e41 4d45 5d0a 2020 2020 2020 2020 290a  NAME].        ).
+00028eb0: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
+00028ec0: 7069 6e67 203d 2070 642e 636f 6e63 6174  ping = pd.concat
+00028ed0: 285b 7365 6c66 2e6d 6170 7069 6e67 2c20  ([self.mapping, 
+00028ee0: 7365 6c66 2e61 7661 696c 6162 6c65 5365  self.availableSe
+00028ef0: 7269 6573 5d2c 2061 7869 733d 3129 0a20  ries], axis=1). 
+00028f00: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
+00028f10: 696e 6720 3d20 7365 6c66 2e6d 6170 7069  ing = self.mappi
+00028f20: 6e67 2e73 6f72 745f 696e 6465 7828 290a  ng.sort_index().
+00028f30: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
+00028f40: 7069 6e67 2e74 6f5f 6578 6365 6c28 7772  ping.to_excel(wr
+00028f50: 6974 6572 2c20 656e 6769 6e65 3d27 6f70  iter, engine='op
+00028f60: 656e 7079 786c 272c 2073 6865 6574 5f6e  enpyxl', sheet_n
+00028f70: 616d 653d 2773 6365 6e61 7269 6f5f 6d61  ame='scenario_ma
+00028f80: 7070 696e 6727 290a 0a20 2020 2020 2020  pping')..       
+00028f90: 2023 2072 6567 696f 6e0a 2020 2020 2020   # region.      
+00028fa0: 2020 696e 6465 7820 3d20 6e70 2e75 6e69    index = np.uni
+00028fb0: 7175 6528 7365 6c66 2e64 6174 615b 7365  que(self.data[se
+00028fc0: 6c66 2e73 6574 7570 2e72 6567 696f 6e5f  lf.setup.region_
+00028fd0: 434f 4c55 4d4e 5f4e 414d 455d 2e76 616c  COLUMN_NAME].val
+00028fe0: 7565 7329 0a0a 2020 2020 2020 2020 7365  ues)..        se
+00028ff0: 6c66 2e61 7661 696c 6162 6c65 5365 7269  lf.availableSeri
+00029000: 6573 203d 2070 642e 4461 7461 4672 616d  es = pd.DataFram
+00029010: 6528 696e 6465 783d 696e 6465 7829 0a20  e(index=index). 
+00029020: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
+00029030: 696e 6720 3d20 7064 2e44 6174 6146 7261  ing = pd.DataFra
+00029040: 6d65 280a 2020 2020 2020 2020 2020 2020  me(.            
+00029050: 696e 6465 783d 696e 6465 782c 2063 6f6c  index=index, col
+00029060: 756d 6e73 3d5b 7365 6c66 2e73 6574 7570  umns=[self.setup
+00029070: 2e52 4547 494f 4e5f 434f 4c55 4d4e 5f4e  .REGION_COLUMN_N
+00029080: 414d 455d 0a20 2020 2020 2020 2029 0a20  AME].        ). 
+00029090: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
+000290a0: 696e 6720 3d20 7064 2e63 6f6e 6361 7428  ing = pd.concat(
+000290b0: 5b73 656c 662e 6d61 7070 696e 672c 2073  [self.mapping, s
+000290c0: 656c 662e 6176 6169 6c61 626c 6553 6572  elf.availableSer
+000290d0: 6965 735d 2c20 6178 6973 3d31 290a 2020  ies], axis=1).  
+000290e0: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
+000290f0: 6e67 203d 2073 656c 662e 6d61 7070 696e  ng = self.mappin
+00029100: 672e 736f 7274 5f69 6e64 6578 2829 0a0a  g.sort_index()..
+00029110: 2020 2020 2020 2020 666f 7220 6964 7820          for idx 
+00029120: 696e 2073 656c 662e 6d61 7070 696e 672e  in self.mapping.
+00029130: 696e 6465 783a 0a20 2020 2020 2020 2020  index:.         
+00029140: 2020 2069 736f 203d 2064 742e 7574 696c     iso = dt.util
+00029150: 2e69 6465 6e74 6966 7943 6f75 6e74 7279  .identifyCountry
+00029160: 2869 6478 290a 2020 2020 2020 2020 2020  (idx).          
+00029170: 2020 6966 2069 736f 2069 7320 6e6f 7420    if iso is not 
+00029180: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00029190: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
+000291a0: 6e67 2e6c 6f63 5b69 6478 2c20 2772 6567  ng.loc[idx, 'reg
+000291b0: 696f 6e27 5d20 3d20 6973 6f0a 0a20 2020  ion'] = iso..   
+000291c0: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
+000291d0: 672e 746f 5f65 7863 656c 2877 7269 7465  g.to_excel(write
+000291e0: 722c 2065 6e67 696e 653d 276f 7065 6e70  r, engine='openp
+000291f0: 7978 6c27 2c20 7368 6565 745f 6e61 6d65  yxl', sheet_name
+00029200: 3d27 7265 6769 6f6e 5f6d 6170 7069 6e67  ='region_mapping
+00029210: 2729 0a20 2020 2020 2020 2077 7269 7465  ').        write
+00029220: 722e 636c 6f73 6528 290a 0a20 2020 2064  r.close()..    d
+00029230: 6566 2067 6174 6865 724d 6170 7065 6444  ef gatherMappedD
+00029240: 6174 6128 7365 6c66 2c20 7370 6174 6961  ata(self, spatia
+00029250: 6c53 7562 5365 743d 4e6f 6e65 2c20 7570  lSubSet=None, up
+00029260: 6461 7465 5461 626c 6573 3d46 616c 7365  dateTables=False
+00029270: 293a 0a0a 2020 2020 2020 2020 696d 706f  ):..        impo
+00029280: 7274 2074 7164 6d0a 0a20 2020 2020 2020  rt tqdm..       
+00029290: 2023 206c 6f61 6469 6e67 2064 6174 6120   # loading data 
+000292a0: 6966 206e 6563 6573 7361 7279 0a20 2020  if necessary.   
+000292b0: 2020 2020 2069 6620 6e6f 7420 6861 7361       if not hasa
+000292c0: 7474 7228 7365 6c66 2c20 2764 6174 6127  ttr(self, 'data'
+000292d0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+000292e0: 656c 662e 6c6f 6164 4461 7461 2829 0a0a  elf.loadData()..
+000292f0: 2020 2020 2020 2020 7461 626c 6573 546f          tablesTo
+00029300: 436f 6d6d 6974 203d 205b 5d0a 2020 2020  Commit = [].    
+00029310: 2020 2020 6d65 7461 4469 6374 203d 2064      metaDict = d
+00029320: 6963 7428 290a 2020 2020 2020 2020 6d65  ict().        me
+00029330: 7461 4469 6374 5b27 736f 7572 6365 275d  taDict['source']
+00029340: 203d 2073 656c 662e 7365 7475 702e 534f   = self.setup.SO
+00029350: 5552 4345 5f49 440a 2020 2020 2020 2020  URCE_ID.        
+00029360: 6578 636c 7564 6564 5461 626c 6573 203d  excludedTables =
+00029370: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00029380: 6578 636c 7564 6564 5461 626c 6573 5b27  excludedTables['
+00029390: 656d 7074 7927 5d20 3d20 6c69 7374 2829  empty'] = list()
+000293a0: 0a20 2020 2020 2020 2065 7863 6c75 6465  .        exclude
+000293b0: 6454 6162 6c65 735b 2765 7272 6f72 275d  dTables['error']
+000293c0: 203d 206c 6973 7428 290a 2020 2020 2020   = list().      
+000293d0: 2020 6578 636c 7564 6564 5461 626c 6573    excludedTables
+000293e0: 5b27 6578 6973 7473 275d 203d 206c 6973  ['exists'] = lis
+000293f0: 7428 290a 0a20 2020 2020 2020 2066 6f72  t()..        for
+00029400: 206d 6f64 656c 2069 6e20 7365 6c66 2e6d   model in self.m
+00029410: 6170 7069 6e67 5b27 6d6f 6465 6c27 5d2e  apping['model'].
+00029420: 6b65 7973 2829 3a0a 2020 2020 2020 2020  keys():.        
+00029430: 2020 2020 7465 6d70 4d6f 203d 2073 656c      tempMo = sel
+00029440: 662e 6461 7461 2e6c 6f63 5b73 656c 662e  f.data.loc[self.
+00029450: 6461 7461 2e6d 6f64 656c 203d 3d20 6d6f  data.model == mo
+00029460: 6465 6c5d 0a20 2020 2020 2020 2020 2020  del].           
+00029470: 2066 6f72 2073 6365 6e61 7269 6f20 696e   for scenario in
+00029480: 2073 656c 662e 6d61 7070 696e 675b 2773   self.mapping['s
+00029490: 6365 6e61 7269 6f27 5d2e 6b65 7973 2829  cenario'].keys()
+000294a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000294b0: 2020 7465 6d70 4d6f 5363 203d 2074 656d    tempMoSc = tem
+000294c0: 704d 6f2e 6c6f 635b 7365 6c66 2e64 6174  pMo.loc[self.dat
+000294d0: 612e 7363 656e 6172 696f 203d 3d20 7363  a.scenario == sc
+000294e0: 656e 6172 696f 5d0a 2020 2020 2020 2020  enario].        
+000294f0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+00029500: 2020 2020 2020 2020 2066 6f72 2076 6172           for var
+00029510: 6961 626c 6520 696e 2073 656c 662e 6d61  iable in self.ma
+00029520: 7070 696e 675b 2776 6172 6961 626c 6527  pping['variable'
+00029530: 5d2e 6b65 7973 2829 3a0a 2020 2020 2020  ].keys():.      
+00029540: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+00029550: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00029560: 656d 704d 6f53 6356 6120 3d20 7465 6d70  empMoScVa = temp
+00029570: 4d6f 5363 2e6c 6f63 5b73 656c 662e 6461  MoSc.loc[self.da
+00029580: 7461 2e76 6172 6961 626c 6520 3d3d 2076  ta.variable == v
+00029590: 6172 6961 626c 655d 0a0a 2020 2020 2020  ariable]..      
+000295a0: 2020 2020 2020 2020 2020 7461 626c 6573            tables
+000295b0: 203d 2064 742e 696e 7465 7266 6163 6573   = dt.interfaces
+000295c0: 2e72 6561 645f 6c6f 6e67 5f74 6162 6c65  .read_long_table
+000295d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000295e0: 2020 2020 2020 7465 6d70 4d6f 5363 2c20        tempMoSc, 
+000295f0: 6c69 7374 2873 656c 662e 6d61 7070 696e  list(self.mappin
+00029600: 675b 2776 6172 6961 626c 6527 5d2e 6b65  g['variable'].ke
+00029610: 7973 2829 290a 2020 2020 2020 2020 2020  ys()).          
+00029620: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00029630: 2020 2020 2020 2020 666f 7220 7461 626c          for tabl
+00029640: 6520 696e 2074 6162 6c65 733a 0a20 2020  e in tables:.   
+00029650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029660: 2074 6162 6c65 2e6d 6574 615b 2763 6174   table.meta['cat
+00029670: 6567 6f72 7927 5d20 3d20 2222 0a20 2020  egory'] = "".   
+00029680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029690: 2074 6162 6c65 2e6d 6574 615b 2773 6f75   table.meta['sou
+000296a0: 7263 6527 5d20 3d20 7365 6c66 2e73 6574  rce'] = self.set
+000296b0: 7570 2e53 4f55 5243 455f 4944 0a20 2020  up.SOURCE_ID.   
+000296c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000296d0: 2074 6162 6c65 2e69 6e64 6578 203d 2074   table.index = t
+000296e0: 6162 6c65 2e69 6e64 6578 2e6d 6170 2873  able.index.map(s
+000296f0: 656c 662e 6d61 7070 696e 675b 2772 6567  elf.mapping['reg
+00029700: 696f 6e27 5d29 0a0a 2020 2020 2020 2020  ion'])..        
+00029710: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
+00029720: 6549 4420 3d20 6474 2e63 6f72 652e 5f63  eID = dt.core._c
+00029730: 7265 6174 6544 6174 6162 6173 6549 4428  reateDatabaseID(
+00029740: 7461 626c 652e 6d65 7461 290a 2020 2020  table.meta).    
+00029750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029760: 6966 206e 6f74 2075 7064 6174 6554 6162  if not updateTab
+00029770: 6c65 733a 0a20 2020 2020 2020 2020 2020  les:.           
+00029780: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00029790: 6474 2e63 6f72 652e 4442 2e74 6162 6c65  dt.core.DB.table
+000297a0: 4578 6973 7428 7461 626c 6549 4429 3a0a  Exist(tableID):.
 000297b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000297c0: 2020 2020 2020 6578 636c 7564 6564 5461        excludedTa
-000297d0: 626c 6573 5b27 6578 6973 7473 275d 2e61  bles['exists'].a
-000297e0: 7070 656e 6428 7461 626c 6549 4429 0a20  ppend(tableID). 
-000297f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029800: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00029810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029820: 2020 2020 2020 2020 2074 6162 6c65 7354           tablesT
-00029830: 6f43 6f6d 6d69 742e 6170 7065 6e64 2874  oCommit.append(t
-00029840: 6162 6c65 290a 2020 2020 2020 2020 7265  able).        re
-00029850: 7475 726e 2074 6162 6c65 7354 6f43 6f6d  turn tablesToCom
-00029860: 6d69 742c 2065 7863 6c75 6465 6454 6162  mit, excludedTab
-00029870: 6c65 730a 0a0a 636c 6173 7320 5641 4e4d  les...class VANM
-00029880: 4152 4c45 3230 3137 2842 6173 6549 6d70  ARLE2017(BaseImp
-00029890: 6f72 7454 6f6f 6c29 3a0a 2020 2020 6465  ortTool):.    de
-000298a0: 6620 5f5f 696e 6974 5f5f 2873 656c 6629  f __init__(self)
-000298b0: 3a0a 2020 2020 2020 2020 7365 6c66 2e73  :.        self.s
-000298c0: 6574 7570 203d 2073 6574 7570 5374 7275  etup = setupStru
-000298d0: 6374 2829 0a20 2020 2020 2020 2073 656c  ct().        sel
-000298e0: 662e 7365 7475 702e 534f 5552 4345 5f49  f.setup.SOURCE_I
-000298f0: 4420 3d20 2256 414e 4d41 524c 4532 3031  D = "VANMARLE201
-00029900: 3722 0a20 2020 2020 2020 2073 656c 662e  7".        self.
-00029910: 7365 7475 702e 534f 5552 4345 5f50 4154  setup.SOURCE_PAT
-00029920: 4820 3d20 6f73 2e70 6174 682e 6a6f 696e  H = os.path.join
-00029930: 280a 2020 2020 2020 2020 2020 2020 636f  (.            co
-00029940: 6e66 6967 2e50 4154 485f 544f 5f44 4154  nfig.PATH_TO_DAT
-00029950: 4153 4845 4c46 2c20 2772 6177 6461 7461  ASHELF, 'rawdata
-00029960: 2f56 414e 4d41 524c 4532 3031 3727 0a20  /VANMARLE2017'. 
-00029970: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00029980: 2073 656c 662e 7365 7475 702e 4441 5441   self.setup.DATA
-00029990: 5f46 494c 4520 3d20 6f73 2e70 6174 682e  _FILE = os.path.
-000299a0: 6a6f 696e 280a 2020 2020 2020 2020 2020  join(.          
-000299b0: 2020 7365 6c66 2e73 6574 7570 2e53 4f55    self.setup.SOU
-000299c0: 5243 455f 5041 5448 2c20 2763 6f6d 7069  RCE_PATH, 'compi
-000299d0: 6c65 645f 7261 775f 7661 6e6d 6172 6c65  led_raw_vanmarle
-000299e0: 2e63 7376 270a 2020 2020 2020 2020 290a  .csv'.        ).
-000299f0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00029a00: 7570 2e4d 4150 5049 4e47 5f46 494c 4520  up.MAPPING_FILE 
-00029a10: 3d20 6f73 2e70 6174 682e 6a6f 696e 2873  = os.path.join(s
-00029a20: 656c 662e 7365 7475 702e 534f 5552 4345  elf.setup.SOURCE
-00029a30: 5f50 4154 482c 2027 6d61 7070 696e 672e  _PATH, 'mapping.
-00029a40: 786c 7378 2729 0a20 2020 2020 2020 2073  xlsx').        s
-00029a50: 656c 662e 7365 7475 702e 4c49 4345 4e43  elf.setup.LICENC
-00029a60: 4520 3d20 2720 4372 6561 7469 7665 2043  E = ' Creative C
-00029a70: 6f6d 6d6f 6e73 2041 7474 7269 6275 7469  ommons Attributi
-00029a80: 6f6e 2033 2e30 204c 6963 656e 7365 270a  on 3.0 License'.
-00029a90: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00029aa0: 7570 2e55 524c 203d 2027 6874 7470 733a  up.URL = 'https:
-00029ab0: 2f2f 7777 772e 6765 6f73 6369 2d6d 6f64  //www.geosci-mod
-00029ac0: 656c 2d64 6576 2e6e 6574 2f31 302f 3333  el-dev.net/10/33
-00029ad0: 3239 2f32 3031 372f 270a 0a20 2020 2020  29/2017/'..     
-00029ae0: 2020 2073 656c 662e 7365 7475 702e 4d4f     self.setup.MO
-00029af0: 4445 4c5f 434f 4c55 4d4e 5f4e 414d 4520  DEL_COLUMN_NAME 
-00029b00: 3d20 276d 6f64 656c 270a 2020 2020 2020  = 'model'.      
-00029b10: 2020 7365 6c66 2e73 6574 7570 2e53 4345    self.setup.SCE
-00029b20: 4e41 5249 4f5f 434f 4c55 4d4e 5f4e 414d  NARIO_COLUMN_NAM
-00029b30: 4520 3d20 2773 6365 6e61 7269 6f27 0a20  E = 'scenario'. 
-00029b40: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
-00029b50: 702e 5245 4749 4f4e 5f43 4f4c 554d 4e5f  p.REGION_COLUMN_
-00029b60: 4e41 4d45 203d 2027 7265 6769 6f6e 270a  NAME = 'region'.
-00029b70: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00029b80: 7570 2e56 4152 4941 424c 455f 434f 4c55  up.VARIABLE_COLU
-00029b90: 4d4e 5f4e 414d 4520 3d20 2776 6172 6961  MN_NAME = 'varia
-00029ba0: 626c 6527 0a0a 2020 2020 2020 2020 6966  ble'..        if
-00029bb0: 206e 6f74 2028 6f73 2e70 6174 682e 6578   not (os.path.ex
-00029bc0: 6973 7473 2873 656c 662e 7365 7475 702e  ists(self.setup.
-00029bd0: 4d41 5050 494e 475f 4649 4c45 2929 3a0a  MAPPING_FILE)):.
-00029be0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00029bf0: 2e63 7265 6174 6556 6172 6961 626c 654d  .createVariableM
-00029c00: 6170 7069 6e67 2829 0a20 2020 2020 2020  apping().       
-00029c10: 2020 2020 2070 7269 6e74 2822 6e6f 206d       print("no m
-00029c20: 6170 7069 6e67 2066 696c 6520 666f 756e  apping file foun
-00029c30: 6422 290a 2020 2020 2020 2020 656c 7365  d").        else
-00029c40: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00029c50: 6c66 2e6d 6170 7069 6e67 203d 2064 6963  lf.mapping = dic
-00029c60: 7428 290a 0a20 2020 2020 2020 2020 2020  t()..           
-00029c70: 2066 6f72 2076 6172 2069 6e20 5b27 7661   for var in ['va
-00029c80: 7269 6162 6c65 272c 2027 7363 656e 6172  riable', 'scenar
-00029c90: 696f 272c 2027 6d6f 6465 6c27 2c20 2772  io', 'model', 'r
-00029ca0: 6567 696f 6e27 5d3a 0a20 2020 2020 2020  egion']:.       
-00029cb0: 2020 2020 2020 2020 2064 6620 3d20 7064           df = pd
-00029cc0: 2e72 6561 645f 6578 6365 6c28 0a20 2020  .read_excel(.   
-00029cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029ce0: 2073 656c 662e 7365 7475 702e 4d41 5050   self.setup.MAPP
-00029cf0: 494e 475f 4649 4c45 2c20 7368 6565 745f  ING_FILE, sheet_
-00029d00: 6e61 6d65 3d76 6172 202b 2027 5f6d 6170  name=var + '_map
-00029d10: 7069 6e67 272c 2069 6e64 6578 5f63 6f6c  ping', index_col
-00029d20: 3d30 0a20 2020 2020 2020 2020 2020 2020  =0.             
-00029d30: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00029d40: 2020 2020 2064 6620 3d20 6466 2e6c 6f63       df = df.loc
-00029d50: 5b7e 6466 2e6c 6f63 5b3a 2c20 7661 725d  [~df.loc[:, var]
-00029d60: 2e69 736e 6128 295d 0a20 2020 2020 2020  .isna()].       
-00029d70: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-00029d80: 7070 696e 672e 7570 6461 7465 2864 662e  pping.update(df.
-00029d90: 746f 5f64 6963 7428 2929 0a0a 2020 2020  to_dict())..    
-00029da0: 2020 2020 7365 6c66 2e63 7265 6174 6553      self.createS
-00029db0: 6f75 7263 654d 6574 6128 290a 0a20 2020  ourceMeta()..   
-00029dc0: 2064 6566 206c 6f61 6444 6174 6128 7365   def loadData(se
-00029dd0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-00029de0: 662e 6461 7461 203d 2070 642e 7265 6164  f.data = pd.read
-00029df0: 5f63 7376 2873 656c 662e 7365 7475 702e  _csv(self.setup.
-00029e00: 4441 5441 5f46 494c 452c 2069 6e64 6578  DATA_FILE, index
-00029e10: 5f63 6f6c 3d4e 6f6e 652c 2068 6561 6465  _col=None, heade
-00029e20: 723d 3029 0a0a 2020 2020 6465 6620 6372  r=0)..    def cr
-00029e30: 6561 7465 5661 7269 6162 6c65 4d61 7070  eateVariableMapp
-00029e40: 696e 6728 7365 6c66 293a 0a0a 2020 2020  ing(self):..    
-00029e50: 2020 2020 2320 6c6f 6164 696e 6720 6461      # loading da
-00029e60: 7461 2069 6620 6e65 6365 7373 6172 790a  ta if necessary.
-00029e70: 2020 2020 2020 2020 6966 206e 6f74 2068          if not h
-00029e80: 6173 6174 7472 2873 656c 662c 2027 6461  asattr(self, 'da
-00029e90: 7461 2729 3a0a 2020 2020 2020 2020 2020  ta'):.          
-00029ea0: 2020 7365 6c66 2e6c 6f61 6444 6174 6128    self.loadData(
-00029eb0: 290a 0a20 2020 2020 2020 2069 6d70 6f72  )..        impor
-00029ec0: 7420 6e75 6d70 7920 6173 206e 700a 0a20  t numpy as np.. 
-00029ed0: 2020 2020 2020 2077 7269 7465 7220 3d20         writer = 
-00029ee0: 7064 2e45 7863 656c 5772 6974 6572 280a  pd.ExcelWriter(.
-00029ef0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00029f00: 2e73 6574 7570 2e4d 4150 5049 4e47 5f46  .setup.MAPPING_F
-00029f10: 494c 452c 0a20 2020 2020 2020 2020 2020  ILE,.           
-00029f20: 2065 6e67 696e 653d 2778 6c73 7877 7269   engine='xlsxwri
-00029f30: 7465 7227 2c0a 2020 2020 2020 2020 2020  ter',.          
-00029f40: 2020 6461 7465 7469 6d65 5f66 6f72 6d61    datetime_forma
-00029f50: 743d 276d 6d6d 2064 2079 7979 7920 6868  t='mmm d yyyy hh
-00029f60: 3a6d 6d3a 7373 272c 0a20 2020 2020 2020  :mm:ss',.       
-00029f70: 2020 2020 2064 6174 655f 666f 726d 6174       date_format
-00029f80: 3d27 6d6d 6d6d 2064 6420 7979 7979 272c  ='mmmm dd yyyy',
-00029f90: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00029fa0: 2020 2020 2320 7661 7269 6162 6c65 730a      # variables.
-00029fb0: 2020 2020 2020 2020 2320 696e 6465 7820          # index 
-00029fc0: 3d20 7365 6c66 2e64 6174 615b 7365 6c66  = self.data[self
-00029fd0: 2e73 6574 7570 2e56 4152 4941 424c 455f  .setup.VARIABLE_
-00029fe0: 434f 4c55 4d4e 5f4e 414d 455d 2e75 6e69  COLUMN_NAME].uni
-00029ff0: 7175 6528 290a 2020 2020 2020 2020 7365  que().        se
-0002a000: 6c66 2e61 7661 696c 6162 6c65 5365 7269  lf.availableSeri
-0002a010: 6573 203d 2073 656c 662e 6461 7461 2e64  es = self.data.d
-0002a020: 726f 705f 6475 706c 6963 6174 6573 2827  rop_duplicates('
-0002a030: 7661 7269 6162 6c65 2729 2e73 6574 5f69  variable').set_i
-0002a040: 6e64 6578 280a 2020 2020 2020 2020 2020  ndex(.          
-0002a050: 2020 7365 6c66 2e73 6574 7570 2e56 4152    self.setup.VAR
-0002a060: 4941 424c 455f 434f 4c55 4d4e 5f4e 414d  IABLE_COLUMN_NAM
-0002a070: 450a 2020 2020 2020 2020 295b 2775 6e69  E.        )['uni
-0002a080: 7427 5d0a 2020 2020 2020 2020 7365 6c66  t'].        self
-0002a090: 2e6d 6170 7069 6e67 203d 2070 642e 4461  .mapping = pd.Da
-0002a0a0: 7461 4672 616d 6528 0a20 2020 2020 2020  taFrame(.       
-0002a0b0: 2020 2020 2069 6e64 6578 3d73 656c 662e       index=self.
-0002a0c0: 6176 6169 6c61 626c 6553 6572 6965 732e  availableSeries.
-0002a0d0: 696e 6465 782c 2063 6f6c 756d 6e73 3d5b  index, columns=[
-0002a0e0: 7365 6c66 2e73 6574 7570 2e56 4152 4941  self.setup.VARIA
-0002a0f0: 424c 455f 434f 4c55 4d4e 5f4e 414d 455d  BLE_COLUMN_NAME]
-0002a100: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0002a110: 2020 2073 656c 662e 6d61 7070 696e 6720     self.mapping 
-0002a120: 3d20 7064 2e63 6f6e 6361 7428 5b73 656c  = pd.concat([sel
-0002a130: 662e 6d61 7070 696e 672c 2073 656c 662e  f.mapping, self.
-0002a140: 6176 6169 6c61 626c 6553 6572 6965 735d  availableSeries]
-0002a150: 2c20 6178 6973 3d31 290a 2020 2020 2020  , axis=1).      
-0002a160: 2020 7365 6c66 2e6d 6170 7069 6e67 203d    self.mapping =
-0002a170: 2073 656c 662e 6d61 7070 696e 672e 736f   self.mapping.so
-0002a180: 7274 5f69 6e64 6578 2829 0a20 2020 2020  rt_index().     
-0002a190: 2020 2073 656c 662e 6d61 7070 696e 672e     self.mapping.
-0002a1a0: 696e 6465 782e 6e61 6d65 203d 2027 6f72  index.name = 'or
-0002a1b0: 6967 6e61 6c27 0a20 2020 2020 2020 2073  ignal'.        s
-0002a1c0: 656c 662e 6d61 7070 696e 672e 746f 5f65  elf.mapping.to_e
-0002a1d0: 7863 656c 2877 7269 7465 722c 2065 6e67  xcel(writer, eng
-0002a1e0: 696e 653d 276f 7065 6e70 7978 6c27 2c20  ine='openpyxl', 
-0002a1f0: 7368 6565 745f 6e61 6d65 3d56 4152 5f4d  sheet_name=VAR_M
-0002a200: 4150 5049 4e47 5f53 4845 4554 290a 0a20  APPING_SHEET).. 
-0002a210: 2020 2020 2020 2023 206d 6f64 656c 730a         # models.
-0002a220: 2020 2020 2020 2020 696e 6465 7820 3d20          index = 
-0002a230: 6e70 2e75 6e69 7175 6528 7365 6c66 2e64  np.unique(self.d
-0002a240: 6174 615b 7365 6c66 2e73 6574 7570 2e4d  ata[self.setup.M
-0002a250: 4f44 454c 5f43 4f4c 554d 4e5f 4e41 4d45  ODEL_COLUMN_NAME
-0002a260: 5d2e 7661 6c75 6573 290a 0a20 2020 2020  ].values)..     
-0002a270: 2020 2073 656c 662e 6176 6169 6c61 626c     self.availabl
-0002a280: 6553 6572 6965 7320 3d20 7064 2e44 6174  eSeries = pd.Dat
-0002a290: 6146 7261 6d65 2869 6e64 6578 3d69 6e64  aFrame(index=ind
-0002a2a0: 6578 290a 2020 2020 2020 2020 7365 6c66  ex).        self
-0002a2b0: 2e6d 6170 7069 6e67 203d 2070 642e 4461  .mapping = pd.Da
-0002a2c0: 7461 4672 616d 6528 696e 6465 783d 696e  taFrame(index=in
-0002a2d0: 6465 782c 2063 6f6c 756d 6e73 3d5b 7365  dex, columns=[se
-0002a2e0: 6c66 2e73 6574 7570 2e4d 4f44 454c 5f43  lf.setup.MODEL_C
-0002a2f0: 4f4c 554d 4e5f 4e41 4d45 5d29 0a20 2020  OLUMN_NAME]).   
-0002a300: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
-0002a310: 6720 3d20 7064 2e63 6f6e 6361 7428 5b73  g = pd.concat([s
-0002a320: 656c 662e 6d61 7070 696e 672c 2073 656c  elf.mapping, sel
-0002a330: 662e 6176 6169 6c61 626c 6553 6572 6965  f.availableSerie
-0002a340: 735d 2c20 6178 6973 3d31 290a 2020 2020  s], axis=1).    
-0002a350: 2020 2020 7365 6c66 2e6d 6170 7069 6e67      self.mapping
-0002a360: 203d 2073 656c 662e 6d61 7070 696e 672e   = self.mapping.
-0002a370: 736f 7274 5f69 6e64 6578 2829 0a20 2020  sort_index().   
-0002a380: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
-0002a390: 672e 696e 6465 782e 6e61 6d65 203d 2027  g.index.name = '
-0002a3a0: 6f72 6967 6e61 6c27 0a20 2020 2020 2020  orignal'.       
-0002a3b0: 2073 656c 662e 6d61 7070 696e 672e 746f   self.mapping.to
-0002a3c0: 5f65 7863 656c 2877 7269 7465 722c 2065  _excel(writer, e
-0002a3d0: 6e67 696e 653d 276f 7065 6e70 7978 6c27  ngine='openpyxl'
-0002a3e0: 2c20 7368 6565 745f 6e61 6d65 3d27 6d6f  , sheet_name='mo
-0002a3f0: 6465 6c5f 6d61 7070 696e 6727 290a 0a20  del_mapping').. 
-0002a400: 2020 2020 2020 2023 2073 6365 6e61 7269         # scenari
-0002a410: 6f73 0a20 2020 2020 2020 2069 6e64 6578  os.        index
-0002a420: 203d 206e 702e 756e 6971 7565 2873 656c   = np.unique(sel
-0002a430: 662e 6461 7461 5b73 656c 662e 7365 7475  f.data[self.setu
-0002a440: 702e 5343 454e 4152 494f 5f43 4f4c 554d  p.SCENARIO_COLUM
-0002a450: 4e5f 4e41 4d45 5d2e 7661 6c75 6573 290a  N_NAME].values).
-0002a460: 2020 2020 2020 2020 7365 6c66 2e61 7661          self.ava
-0002a470: 696c 6162 6c65 5365 7269 6573 203d 2070  ilableSeries = p
-0002a480: 642e 4461 7461 4672 616d 6528 696e 6465  d.DataFrame(inde
-0002a490: 783d 696e 6465 7829 0a20 2020 2020 2020  x=index).       
-0002a4a0: 2073 656c 662e 6d61 7070 696e 6720 3d20   self.mapping = 
-0002a4b0: 7064 2e44 6174 6146 7261 6d65 280a 2020  pd.DataFrame(.  
-0002a4c0: 2020 2020 2020 2020 2020 696e 6465 783d            index=
-0002a4d0: 696e 6465 782c 2063 6f6c 756d 6e73 3d5b  index, columns=[
-0002a4e0: 7365 6c66 2e73 6574 7570 2e53 4345 4e41  self.setup.SCENA
-0002a4f0: 5249 4f5f 434f 4c55 4d4e 5f4e 414d 455d  RIO_COLUMN_NAME]
-0002a500: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0002a510: 2020 2073 656c 662e 6d61 7070 696e 6720     self.mapping 
-0002a520: 3d20 7064 2e63 6f6e 6361 7428 5b73 656c  = pd.concat([sel
-0002a530: 662e 6d61 7070 696e 672c 2073 656c 662e  f.mapping, self.
-0002a540: 6176 6169 6c61 626c 6553 6572 6965 735d  availableSeries]
-0002a550: 2c20 6178 6973 3d31 290a 2020 2020 2020  , axis=1).      
-0002a560: 2020 7365 6c66 2e6d 6170 7069 6e67 203d    self.mapping =
-0002a570: 2073 656c 662e 6d61 7070 696e 672e 736f   self.mapping.so
-0002a580: 7274 5f69 6e64 6578 2829 0a20 2020 2020  rt_index().     
-0002a590: 2020 2073 656c 662e 6d61 7070 696e 672e     self.mapping.
-0002a5a0: 696e 6465 782e 6e61 6d65 203d 2027 6f72  index.name = 'or
-0002a5b0: 6967 6e61 6c27 0a20 2020 2020 2020 2073  ignal'.        s
-0002a5c0: 656c 662e 6d61 7070 696e 672e 746f 5f65  elf.mapping.to_e
-0002a5d0: 7863 656c 2877 7269 7465 722c 2065 6e67  xcel(writer, eng
-0002a5e0: 696e 653d 276f 7065 6e70 7978 6c27 2c20  ine='openpyxl', 
-0002a5f0: 7368 6565 745f 6e61 6d65 3d27 7363 656e  sheet_name='scen
-0002a600: 6172 696f 5f6d 6170 7069 6e67 2729 0a0a  ario_mapping')..
-0002a610: 2020 2020 2020 2020 2320 7265 6769 6f6e          # region
-0002a620: 0a20 2020 2020 2020 2069 6e64 6578 203d  .        index =
-0002a630: 206e 702e 756e 6971 7565 2873 656c 662e   np.unique(self.
-0002a640: 6461 7461 5b73 656c 662e 7365 7475 702e  data[self.setup.
-0002a650: 5245 4749 4f4e 5f43 4f4c 554d 4e5f 4e41  REGION_COLUMN_NA
-0002a660: 4d45 5d2e 7661 6c75 6573 290a 2020 2020  ME].values).    
-0002a670: 2020 2020 7365 6c66 2e61 7661 696c 6162      self.availab
-0002a680: 6c65 5365 7269 6573 203d 2070 642e 4461  leSeries = pd.Da
-0002a690: 7461 4672 616d 6528 696e 6465 783d 696e  taFrame(index=in
-0002a6a0: 6465 7829 0a20 2020 2020 2020 2073 656c  dex).        sel
-0002a6b0: 662e 6d61 7070 696e 6720 3d20 7064 2e44  f.mapping = pd.D
-0002a6c0: 6174 6146 7261 6d65 280a 2020 2020 2020  ataFrame(.      
-0002a6d0: 2020 2020 2020 696e 6465 783d 696e 6465        index=inde
-0002a6e0: 782c 2063 6f6c 756d 6e73 3d5b 7365 6c66  x, columns=[self
-0002a6f0: 2e73 6574 7570 2e52 4547 494f 4e5f 434f  .setup.REGION_CO
-0002a700: 4c55 4d4e 5f4e 414d 455d 0a20 2020 2020  LUMN_NAME].     
-0002a710: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-0002a720: 662e 6d61 7070 696e 6720 3d20 7064 2e63  f.mapping = pd.c
-0002a730: 6f6e 6361 7428 5b73 656c 662e 6d61 7070  oncat([self.mapp
-0002a740: 696e 672c 2073 656c 662e 6176 6169 6c61  ing, self.availa
-0002a750: 626c 6553 6572 6965 735d 2c20 6178 6973  bleSeries], axis
-0002a760: 3d31 290a 2020 2020 2020 2020 7365 6c66  =1).        self
-0002a770: 2e6d 6170 7069 6e67 203d 2073 656c 662e  .mapping = self.
-0002a780: 6d61 7070 696e 672e 736f 7274 5f69 6e64  mapping.sort_ind
-0002a790: 6578 2829 0a20 2020 2020 2020 2073 656c  ex().        sel
-0002a7a0: 662e 6d61 7070 696e 672e 696e 6465 782e  f.mapping.index.
-0002a7b0: 6e61 6d65 203d 2027 6f72 6967 6e61 6c27  name = 'orignal'
-0002a7c0: 0a20 2020 2020 2020 2066 6f72 2069 6478  .        for idx
-0002a7d0: 2069 6e20 7365 6c66 2e6d 6170 7069 6e67   in self.mapping
-0002a7e0: 2e69 6e64 6578 3a0a 2020 2020 2020 2020  .index:.        
-0002a7f0: 2020 2020 6973 6f20 3d20 6474 2e75 7469      iso = dt.uti
-0002a800: 6c2e 6964 656e 7469 6679 436f 756e 7472  l.identifyCountr
-0002a810: 7928 6964 7829 0a20 2020 2020 2020 2020  y(idx).         
-0002a820: 2020 2069 6620 6973 6f20 6973 206e 6f74     if iso is not
-0002a830: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002a840: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
-0002a850: 696e 672e 6c6f 635b 6964 782c 2027 7265  ing.loc[idx, 're
-0002a860: 6769 6f6e 275d 203d 2069 736f 0a0a 2020  gion'] = iso..  
-0002a870: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
-0002a880: 6e67 2e74 6f5f 6578 6365 6c28 7772 6974  ng.to_excel(writ
-0002a890: 6572 2c20 656e 6769 6e65 3d27 6f70 656e  er, engine='open
-0002a8a0: 7079 786c 272c 2073 6865 6574 5f6e 616d  pyxl', sheet_nam
-0002a8b0: 653d 2772 6567 696f 6e5f 6d61 7070 696e  e='region_mappin
-0002a8c0: 6727 290a 2020 2020 2020 2020 7772 6974  g').        writ
-0002a8d0: 6572 2e63 6c6f 7365 2829 0a0a 2020 2020  er.close()..    
-0002a8e0: 6465 6620 6761 7468 6572 4d61 7070 6564  def gatherMapped
-0002a8f0: 4461 7461 2873 656c 662c 2073 7061 7469  Data(self, spati
-0002a900: 616c 5375 6253 6574 3d4e 6f6e 652c 2075  alSubSet=None, u
-0002a910: 7064 6174 6554 6162 6c65 733d 4661 6c73  pdateTables=Fals
-0002a920: 6529 3a0a 0a20 2020 2020 2020 2069 6d70  e):..        imp
-0002a930: 6f72 7420 7471 646d 0a0a 2020 2020 2020  ort tqdm..      
-0002a940: 2020 2320 6c6f 6164 696e 6720 6461 7461    # loading data
-0002a950: 2069 6620 6e65 6365 7373 6172 790a 2020   if necessary.  
-0002a960: 2020 2020 2020 6966 206e 6f74 2068 6173        if not has
-0002a970: 6174 7472 2873 656c 662c 2027 6461 7461  attr(self, 'data
-0002a980: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
-0002a990: 7365 6c66 2e6c 6f61 6444 6174 6128 290a  self.loadData().
-0002a9a0: 0a20 2020 2020 2020 2074 6162 6c65 7354  .        tablesT
-0002a9b0: 6f43 6f6d 6d69 7420 3d20 5b5d 0a20 2020  oCommit = [].   
-0002a9c0: 2020 2020 206d 6574 6144 6963 7420 3d20       metaDict = 
-0002a9d0: 6469 6374 2829 0a20 2020 2020 2020 206d  dict().        m
-0002a9e0: 6574 6144 6963 745b 2773 6f75 7263 6527  etaDict['source'
-0002a9f0: 5d20 3d20 7365 6c66 2e73 6574 7570 2e53  ] = self.setup.S
-0002aa00: 4f55 5243 455f 4944 0a20 2020 2020 2020  OURCE_ID.       
-0002aa10: 2065 7863 6c75 6465 6454 6162 6c65 7320   excludedTables 
-0002aa20: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0002aa30: 2065 7863 6c75 6465 6454 6162 6c65 735b   excludedTables[
-0002aa40: 2765 6d70 7479 275d 203d 206c 6973 7428  'empty'] = list(
-0002aa50: 290a 2020 2020 2020 2020 6578 636c 7564  ).        exclud
-0002aa60: 6564 5461 626c 6573 5b27 6572 726f 7227  edTables['error'
-0002aa70: 5d20 3d20 6c69 7374 2829 0a20 2020 2020  ] = list().     
-0002aa80: 2020 2065 7863 6c75 6465 6454 6162 6c65     excludedTable
-0002aa90: 735b 2765 7869 7374 7327 5d20 3d20 6c69  s['exists'] = li
-0002aaa0: 7374 2829 0a0a 2020 2020 2020 2020 666f  st()..        fo
-0002aab0: 7220 6d6f 6465 6c20 696e 2073 656c 662e  r model in self.
-0002aac0: 6d61 7070 696e 675b 276d 6f64 656c 275d  mapping['model']
-0002aad0: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
-0002aae0: 2020 2020 2074 656d 704d 6f20 3d20 7365       tempMo = se
-0002aaf0: 6c66 2e64 6174 612e 6c6f 635b 7365 6c66  lf.data.loc[self
-0002ab00: 2e64 6174 612e 6d6f 6465 6c20 3d3d 206d  .data.model == m
-0002ab10: 6f64 656c 5d0a 2020 2020 2020 2020 2020  odel].          
-0002ab20: 2020 666f 7220 7363 656e 6172 696f 2069    for scenario i
-0002ab30: 6e20 7365 6c66 2e6d 6170 7069 6e67 5b27  n self.mapping['
-0002ab40: 7363 656e 6172 696f 275d 2e6b 6579 7328  scenario'].keys(
-0002ab50: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0002ab60: 2020 2074 656d 704d 6f53 6320 3d20 7465     tempMoSc = te
-0002ab70: 6d70 4d6f 2e6c 6f63 5b74 656d 704d 6f2e  mpMo.loc[tempMo.
-0002ab80: 7363 656e 6172 696f 203d 3d20 7363 656e  scenario == scen
-0002ab90: 6172 696f 5d0a 2020 2020 2020 2020 2020  ario].          
-0002aba0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0002abb0: 2020 2020 2020 2066 6f72 2076 6172 6961         for varia
-0002abc0: 626c 6520 696e 2073 656c 662e 6d61 7070  ble in self.mapp
-0002abd0: 696e 675b 2776 6172 6961 626c 6527 5d2e  ing['variable'].
-0002abe0: 6b65 7973 2829 3a0a 2020 2020 2020 2020  keys():.        
-0002abf0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0002ac00: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-0002ac10: 704d 6f53 6356 6120 3d20 7465 6d70 4d6f  pMoScVa = tempMo
-0002ac20: 5363 2e6c 6f63 5b73 656c 662e 6461 7461  Sc.loc[self.data
-0002ac30: 2e76 6172 6961 626c 6520 3d3d 2076 6172  .variable == var
-0002ac40: 6961 626c 655d 0a0a 2020 2020 2020 2020  iable]..        
-0002ac50: 2020 2020 2020 2020 666f 7220 7661 7269          for vari
-0002ac60: 6162 6c65 2069 6e20 6c69 7374 2873 656c  able in list(sel
-0002ac70: 662e 6d61 7070 696e 675b 2776 6172 6961  f.mapping['varia
-0002ac80: 626c 6527 5d2e 6b65 7973 2829 293a 0a20  ble'].keys()):. 
-0002ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002aca0: 2020 2074 656d 704d 6f53 6356 6172 203d     tempMoScVar =
-0002acb0: 2074 656d 704d 6f53 632e 6c6f 635b 7465   tempMoSc.loc[te
-0002acc0: 6d70 4d6f 5363 2e76 6172 6961 626c 6520  mpMoSc.variable 
-0002acd0: 3d3d 2076 6172 6961 626c 655d 0a20 2020  == variable].   
-0002ace0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002acf0: 2074 656d 704d 6f53 6356 6172 2e75 6e69   tempMoScVar.uni
-0002ad00: 7420 3d20 7365 6c66 2e6d 6170 7069 6e67  t = self.mapping
-0002ad10: 5b27 756e 6974 275d 5b76 6172 6961 626c  ['unit'][variabl
-0002ad20: 655d 0a20 2020 2020 2020 2020 2020 2020  e].             
-0002ad30: 2020 2020 2020 2074 6162 6c65 7320 3d20         tables = 
-0002ad40: 6474 2e69 6e74 6572 6661 6365 732e 7265  dt.interfaces.re
-0002ad50: 6164 5f6c 6f6e 675f 7461 626c 6528 7465  ad_long_table(te
-0002ad60: 6d70 4d6f 5363 5661 722c 205b 7661 7269  mpMoScVar, [vari
-0002ad70: 6162 6c65 5d29 0a20 2020 2020 2020 2020  able]).         
-0002ad80: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
-0002ad90: 6162 6c65 2069 6e20 7461 626c 6573 3a0a  able in tables:.
-0002ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002adb0: 2020 2020 2020 2020 7461 626c 652e 6d65          table.me
-0002adc0: 7461 5b27 6361 7465 676f 7279 275d 203d  ta['category'] =
-0002add0: 2022 220a 2020 2020 2020 2020 2020 2020   "".            
-0002ade0: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
-0002adf0: 652e 6d65 7461 5b27 736f 7572 6365 275d  e.meta['source']
-0002ae00: 203d 2073 656c 662e 7365 7475 702e 534f   = self.setup.SO
-0002ae10: 5552 4345 5f49 440a 2020 2020 2020 2020  URCE_ID.        
+000297c0: 2020 2020 2020 2020 2020 2020 6578 636c              excl
+000297d0: 7564 6564 5461 626c 6573 5b27 6578 6973  udedTables['exis
+000297e0: 7473 275d 2e61 7070 656e 6428 7461 626c  ts'].append(tabl
+000297f0: 6549 4429 0a20 2020 2020 2020 2020 2020  eID).           
+00029800: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00029810: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00029820: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00029830: 6162 6c65 7354 6f43 6f6d 6d69 742e 6170  ablesToCommit.ap
+00029840: 7065 6e64 2874 6162 6c65 290a 2020 2020  pend(table).    
+00029850: 2020 2020 7265 7475 726e 2074 6162 6c65      return table
+00029860: 7354 6f43 6f6d 6d69 742c 2065 7863 6c75  sToCommit, exclu
+00029870: 6465 6454 6162 6c65 730a 0a0a 636c 6173  dedTables...clas
+00029880: 7320 5641 4e4d 4152 4c45 3230 3137 2842  s VANMARLE2017(B
+00029890: 6173 6549 6d70 6f72 7454 6f6f 6c29 3a0a  aseImportTool):.
+000298a0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000298b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000298c0: 7365 6c66 2e73 6574 7570 203d 2073 6574  self.setup = set
+000298d0: 7570 5374 7275 6374 2829 0a20 2020 2020  upStruct().     
+000298e0: 2020 2073 656c 662e 7365 7475 702e 534f     self.setup.SO
+000298f0: 5552 4345 5f49 4420 3d20 2256 414e 4d41  URCE_ID = "VANMA
+00029900: 524c 4532 3031 3722 0a20 2020 2020 2020  RLE2017".       
+00029910: 2073 656c 662e 7365 7475 702e 534f 5552   self.setup.SOUR
+00029920: 4345 5f50 4154 4820 3d20 6f73 2e70 6174  CE_PATH = os.pat
+00029930: 682e 6a6f 696e 280a 2020 2020 2020 2020  h.join(.        
+00029940: 2020 2020 636f 6e66 6967 2e50 4154 485f      config.PATH_
+00029950: 544f 5f44 4154 4153 4845 4c46 2c20 2772  TO_DATASHELF, 'r
+00029960: 6177 6461 7461 2f56 414e 4d41 524c 4532  awdata/VANMARLE2
+00029970: 3031 3727 0a20 2020 2020 2020 2029 0a20  017'.        ). 
+00029980: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
+00029990: 702e 4441 5441 5f46 494c 4520 3d20 6f73  p.DATA_FILE = os
+000299a0: 2e70 6174 682e 6a6f 696e 280a 2020 2020  .path.join(.    
+000299b0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+000299c0: 7570 2e53 4f55 5243 455f 5041 5448 2c20  up.SOURCE_PATH, 
+000299d0: 2763 6f6d 7069 6c65 645f 7261 775f 7661  'compiled_raw_va
+000299e0: 6e6d 6172 6c65 2e63 7376 270a 2020 2020  nmarle.csv'.    
+000299f0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+00029a00: 6c66 2e73 6574 7570 2e4d 4150 5049 4e47  lf.setup.MAPPING
+00029a10: 5f46 494c 4520 3d20 6f73 2e70 6174 682e  _FILE = os.path.
+00029a20: 6a6f 696e 2873 656c 662e 7365 7475 702e  join(self.setup.
+00029a30: 534f 5552 4345 5f50 4154 482c 2027 6d61  SOURCE_PATH, 'ma
+00029a40: 7070 696e 672e 786c 7378 2729 0a20 2020  pping.xlsx').   
+00029a50: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
+00029a60: 4c49 4345 4e43 4520 3d20 2720 4372 6561  LICENCE = ' Crea
+00029a70: 7469 7665 2043 6f6d 6d6f 6e73 2041 7474  tive Commons Att
+00029a80: 7269 6275 7469 6f6e 2033 2e30 204c 6963  ribution 3.0 Lic
+00029a90: 656e 7365 270a 2020 2020 2020 2020 7365  ense'.        se
+00029aa0: 6c66 2e73 6574 7570 2e55 524c 203d 2027  lf.setup.URL = '
+00029ab0: 6874 7470 733a 2f2f 7777 772e 6765 6f73  https://www.geos
+00029ac0: 6369 2d6d 6f64 656c 2d64 6576 2e6e 6574  ci-model-dev.net
+00029ad0: 2f31 302f 3333 3239 2f32 3031 372f 270a  /10/3329/2017/'.
+00029ae0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00029af0: 7475 702e 4d4f 4445 4c5f 434f 4c55 4d4e  tup.MODEL_COLUMN
+00029b00: 5f4e 414d 4520 3d20 276d 6f64 656c 270a  _NAME = 'model'.
+00029b10: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00029b20: 7570 2e53 4345 4e41 5249 4f5f 434f 4c55  up.SCENARIO_COLU
+00029b30: 4d4e 5f4e 414d 4520 3d20 2773 6365 6e61  MN_NAME = 'scena
+00029b40: 7269 6f27 0a20 2020 2020 2020 2073 656c  rio'.        sel
+00029b50: 662e 7365 7475 702e 5245 4749 4f4e 5f43  f.setup.REGION_C
+00029b60: 4f4c 554d 4e5f 4e41 4d45 203d 2027 7265  OLUMN_NAME = 're
+00029b70: 6769 6f6e 270a 2020 2020 2020 2020 7365  gion'.        se
+00029b80: 6c66 2e73 6574 7570 2e56 4152 4941 424c  lf.setup.VARIABL
+00029b90: 455f 434f 4c55 4d4e 5f4e 414d 4520 3d20  E_COLUMN_NAME = 
+00029ba0: 2776 6172 6961 626c 6527 0a0a 2020 2020  'variable'..    
+00029bb0: 2020 2020 6966 206e 6f74 2028 6f73 2e70      if not (os.p
+00029bc0: 6174 682e 6578 6973 7473 2873 656c 662e  ath.exists(self.
+00029bd0: 7365 7475 702e 4d41 5050 494e 475f 4649  setup.MAPPING_FI
+00029be0: 4c45 2929 3a0a 2020 2020 2020 2020 2020  LE)):.          
+00029bf0: 2020 7365 6c66 2e63 7265 6174 6556 6172    self.createVar
+00029c00: 6961 626c 654d 6170 7069 6e67 2829 0a20  iableMapping(). 
+00029c10: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00029c20: 2822 6e6f 206d 6170 7069 6e67 2066 696c  ("no mapping fil
+00029c30: 6520 666f 756e 6422 290a 2020 2020 2020  e found").      
+00029c40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00029c50: 2020 2020 7365 6c66 2e6d 6170 7069 6e67      self.mapping
+00029c60: 203d 2064 6963 7428 290a 0a20 2020 2020   = dict()..     
+00029c70: 2020 2020 2020 2066 6f72 2076 6172 2069         for var i
+00029c80: 6e20 5b27 7661 7269 6162 6c65 272c 2027  n ['variable', '
+00029c90: 7363 656e 6172 696f 272c 2027 6d6f 6465  scenario', 'mode
+00029ca0: 6c27 2c20 2772 6567 696f 6e27 5d3a 0a20  l', 'region']:. 
+00029cb0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00029cc0: 6620 3d20 7064 2e72 6561 645f 6578 6365  f = pd.read_exce
+00029cd0: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+00029ce0: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
+00029cf0: 702e 4d41 5050 494e 475f 4649 4c45 2c20  p.MAPPING_FILE, 
+00029d00: 7368 6565 745f 6e61 6d65 3d76 6172 202b  sheet_name=var +
+00029d10: 2027 5f6d 6170 7069 6e67 272c 2069 6e64   '_mapping', ind
+00029d20: 6578 5f63 6f6c 3d30 0a20 2020 2020 2020  ex_col=0.       
+00029d30: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00029d40: 2020 2020 2020 2020 2020 2064 6620 3d20             df = 
+00029d50: 6466 2e6c 6f63 5b7e 6466 2e6c 6f63 5b3a  df.loc[~df.loc[:
+00029d60: 2c20 7661 725d 2e69 736e 6128 295d 0a20  , var].isna()]. 
+00029d70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00029d80: 656c 662e 6d61 7070 696e 672e 7570 6461  elf.mapping.upda
+00029d90: 7465 2864 662e 746f 5f64 6963 7428 2929  te(df.to_dict())
+00029da0: 0a0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
+00029db0: 7265 6174 6553 6f75 7263 654d 6574 6128  reateSourceMeta(
+00029dc0: 290a 0a20 2020 2064 6566 206c 6f61 6444  )..    def loadD
+00029dd0: 6174 6128 7365 6c66 293a 0a20 2020 2020  ata(self):.     
+00029de0: 2020 2073 656c 662e 6461 7461 203d 2070     self.data = p
+00029df0: 642e 7265 6164 5f63 7376 2873 656c 662e  d.read_csv(self.
+00029e00: 7365 7475 702e 4441 5441 5f46 494c 452c  setup.DATA_FILE,
+00029e10: 2069 6e64 6578 5f63 6f6c 3d4e 6f6e 652c   index_col=None,
+00029e20: 2068 6561 6465 723d 3029 0a0a 2020 2020   header=0)..    
+00029e30: 6465 6620 6372 6561 7465 5661 7269 6162  def createVariab
+00029e40: 6c65 4d61 7070 696e 6728 7365 6c66 293a  leMapping(self):
+00029e50: 0a0a 2020 2020 2020 2020 2320 6c6f 6164  ..        # load
+00029e60: 696e 6720 6461 7461 2069 6620 6e65 6365  ing data if nece
+00029e70: 7373 6172 790a 2020 2020 2020 2020 6966  ssary.        if
+00029e80: 206e 6f74 2068 6173 6174 7472 2873 656c   not hasattr(sel
+00029e90: 662c 2027 6461 7461 2729 3a0a 2020 2020  f, 'data'):.    
+00029ea0: 2020 2020 2020 2020 7365 6c66 2e6c 6f61          self.loa
+00029eb0: 6444 6174 6128 290a 0a20 2020 2020 2020  dData()..       
+00029ec0: 2069 6d70 6f72 7420 6e75 6d70 7920 6173   import numpy as
+00029ed0: 206e 700a 0a20 2020 2020 2020 2077 7269   np..        wri
+00029ee0: 7465 7220 3d20 7064 2e45 7863 656c 5772  ter = pd.ExcelWr
+00029ef0: 6974 6572 280a 2020 2020 2020 2020 2020  iter(.          
+00029f00: 2020 7365 6c66 2e73 6574 7570 2e4d 4150    self.setup.MAP
+00029f10: 5049 4e47 5f46 494c 452c 0a20 2020 2020  PING_FILE,.     
+00029f20: 2020 2020 2020 2065 6e67 696e 653d 2778         engine='x
+00029f30: 6c73 7877 7269 7465 7227 2c0a 2020 2020  lsxwriter',.    
+00029f40: 2020 2020 2020 2020 6461 7465 7469 6d65          datetime
+00029f50: 5f66 6f72 6d61 743d 276d 6d6d 2064 2079  _format='mmm d y
+00029f60: 7979 7920 6868 3a6d 6d3a 7373 272c 0a20  yyy hh:mm:ss',. 
+00029f70: 2020 2020 2020 2020 2020 2064 6174 655f             date_
+00029f80: 666f 726d 6174 3d27 6d6d 6d6d 2064 6420  format='mmmm dd 
+00029f90: 7979 7979 272c 0a20 2020 2020 2020 2029  yyyy',.        )
+00029fa0: 0a0a 2020 2020 2020 2020 2320 7661 7269  ..        # vari
+00029fb0: 6162 6c65 730a 2020 2020 2020 2020 2320  ables.        # 
+00029fc0: 696e 6465 7820 3d20 7365 6c66 2e64 6174  index = self.dat
+00029fd0: 615b 7365 6c66 2e73 6574 7570 2e56 4152  a[self.setup.VAR
+00029fe0: 4941 424c 455f 434f 4c55 4d4e 5f4e 414d  IABLE_COLUMN_NAM
+00029ff0: 455d 2e75 6e69 7175 6528 290a 2020 2020  E].unique().    
+0002a000: 2020 2020 7365 6c66 2e61 7661 696c 6162      self.availab
+0002a010: 6c65 5365 7269 6573 203d 2073 656c 662e  leSeries = self.
+0002a020: 6461 7461 2e64 726f 705f 6475 706c 6963  data.drop_duplic
+0002a030: 6174 6573 2827 7661 7269 6162 6c65 2729  ates('variable')
+0002a040: 2e73 6574 5f69 6e64 6578 280a 2020 2020  .set_index(.    
+0002a050: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0002a060: 7570 2e56 4152 4941 424c 455f 434f 4c55  up.VARIABLE_COLU
+0002a070: 4d4e 5f4e 414d 450a 2020 2020 2020 2020  MN_NAME.        
+0002a080: 295b 2775 6e69 7427 5d0a 2020 2020 2020  )['unit'].      
+0002a090: 2020 7365 6c66 2e6d 6170 7069 6e67 203d    self.mapping =
+0002a0a0: 2070 642e 4461 7461 4672 616d 6528 0a20   pd.DataFrame(. 
+0002a0b0: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+0002a0c0: 3d73 656c 662e 6176 6169 6c61 626c 6553  =self.availableS
+0002a0d0: 6572 6965 732e 696e 6465 782c 2063 6f6c  eries.index, col
+0002a0e0: 756d 6e73 3d5b 7365 6c66 2e73 6574 7570  umns=[self.setup
+0002a0f0: 2e56 4152 4941 424c 455f 434f 4c55 4d4e  .VARIABLE_COLUMN
+0002a100: 5f4e 414d 455d 0a20 2020 2020 2020 2029  _NAME].        )
+0002a110: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
+0002a120: 7070 696e 6720 3d20 7064 2e63 6f6e 6361  pping = pd.conca
+0002a130: 7428 5b73 656c 662e 6d61 7070 696e 672c  t([self.mapping,
+0002a140: 2073 656c 662e 6176 6169 6c61 626c 6553   self.availableS
+0002a150: 6572 6965 735d 2c20 6178 6973 3d31 290a  eries], axis=1).
+0002a160: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
+0002a170: 7069 6e67 203d 2073 656c 662e 6d61 7070  ping = self.mapp
+0002a180: 696e 672e 736f 7274 5f69 6e64 6578 2829  ing.sort_index()
+0002a190: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
+0002a1a0: 7070 696e 672e 696e 6465 782e 6e61 6d65  pping.index.name
+0002a1b0: 203d 2027 6f72 6967 6e61 6c27 0a20 2020   = 'orignal'.   
+0002a1c0: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
+0002a1d0: 672e 746f 5f65 7863 656c 2877 7269 7465  g.to_excel(write
+0002a1e0: 722c 2065 6e67 696e 653d 276f 7065 6e70  r, engine='openp
+0002a1f0: 7978 6c27 2c20 7368 6565 745f 6e61 6d65  yxl', sheet_name
+0002a200: 3d56 4152 5f4d 4150 5049 4e47 5f53 4845  =VAR_MAPPING_SHE
+0002a210: 4554 290a 0a20 2020 2020 2020 2023 206d  ET)..        # m
+0002a220: 6f64 656c 730a 2020 2020 2020 2020 696e  odels.        in
+0002a230: 6465 7820 3d20 6e70 2e75 6e69 7175 6528  dex = np.unique(
+0002a240: 7365 6c66 2e64 6174 615b 7365 6c66 2e73  self.data[self.s
+0002a250: 6574 7570 2e4d 4f44 454c 5f43 4f4c 554d  etup.MODEL_COLUM
+0002a260: 4e5f 4e41 4d45 5d2e 7661 6c75 6573 290a  N_NAME].values).
+0002a270: 0a20 2020 2020 2020 2073 656c 662e 6176  .        self.av
+0002a280: 6169 6c61 626c 6553 6572 6965 7320 3d20  ailableSeries = 
+0002a290: 7064 2e44 6174 6146 7261 6d65 2869 6e64  pd.DataFrame(ind
+0002a2a0: 6578 3d69 6e64 6578 290a 2020 2020 2020  ex=index).      
+0002a2b0: 2020 7365 6c66 2e6d 6170 7069 6e67 203d    self.mapping =
+0002a2c0: 2070 642e 4461 7461 4672 616d 6528 696e   pd.DataFrame(in
+0002a2d0: 6465 783d 696e 6465 782c 2063 6f6c 756d  dex=index, colum
+0002a2e0: 6e73 3d5b 7365 6c66 2e73 6574 7570 2e4d  ns=[self.setup.M
+0002a2f0: 4f44 454c 5f43 4f4c 554d 4e5f 4e41 4d45  ODEL_COLUMN_NAME
+0002a300: 5d29 0a20 2020 2020 2020 2073 656c 662e  ]).        self.
+0002a310: 6d61 7070 696e 6720 3d20 7064 2e63 6f6e  mapping = pd.con
+0002a320: 6361 7428 5b73 656c 662e 6d61 7070 696e  cat([self.mappin
+0002a330: 672c 2073 656c 662e 6176 6169 6c61 626c  g, self.availabl
+0002a340: 6553 6572 6965 735d 2c20 6178 6973 3d31  eSeries], axis=1
+0002a350: 290a 2020 2020 2020 2020 7365 6c66 2e6d  ).        self.m
+0002a360: 6170 7069 6e67 203d 2073 656c 662e 6d61  apping = self.ma
+0002a370: 7070 696e 672e 736f 7274 5f69 6e64 6578  pping.sort_index
+0002a380: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0002a390: 6d61 7070 696e 672e 696e 6465 782e 6e61  mapping.index.na
+0002a3a0: 6d65 203d 2027 6f72 6967 6e61 6c27 0a20  me = 'orignal'. 
+0002a3b0: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
+0002a3c0: 696e 672e 746f 5f65 7863 656c 2877 7269  ing.to_excel(wri
+0002a3d0: 7465 722c 2065 6e67 696e 653d 276f 7065  ter, engine='ope
+0002a3e0: 6e70 7978 6c27 2c20 7368 6565 745f 6e61  npyxl', sheet_na
+0002a3f0: 6d65 3d27 6d6f 6465 6c5f 6d61 7070 696e  me='model_mappin
+0002a400: 6727 290a 0a20 2020 2020 2020 2023 2073  g')..        # s
+0002a410: 6365 6e61 7269 6f73 0a20 2020 2020 2020  cenarios.       
+0002a420: 2069 6e64 6578 203d 206e 702e 756e 6971   index = np.uniq
+0002a430: 7565 2873 656c 662e 6461 7461 5b73 656c  ue(self.data[sel
+0002a440: 662e 7365 7475 702e 5343 454e 4152 494f  f.setup.SCENARIO
+0002a450: 5f43 4f4c 554d 4e5f 4e41 4d45 5d2e 7661  _COLUMN_NAME].va
+0002a460: 6c75 6573 290a 2020 2020 2020 2020 7365  lues).        se
+0002a470: 6c66 2e61 7661 696c 6162 6c65 5365 7269  lf.availableSeri
+0002a480: 6573 203d 2070 642e 4461 7461 4672 616d  es = pd.DataFram
+0002a490: 6528 696e 6465 783d 696e 6465 7829 0a20  e(index=index). 
+0002a4a0: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
+0002a4b0: 696e 6720 3d20 7064 2e44 6174 6146 7261  ing = pd.DataFra
+0002a4c0: 6d65 280a 2020 2020 2020 2020 2020 2020  me(.            
+0002a4d0: 696e 6465 783d 696e 6465 782c 2063 6f6c  index=index, col
+0002a4e0: 756d 6e73 3d5b 7365 6c66 2e73 6574 7570  umns=[self.setup
+0002a4f0: 2e53 4345 4e41 5249 4f5f 434f 4c55 4d4e  .SCENARIO_COLUMN
+0002a500: 5f4e 414d 455d 0a20 2020 2020 2020 2029  _NAME].        )
+0002a510: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
+0002a520: 7070 696e 6720 3d20 7064 2e63 6f6e 6361  pping = pd.conca
+0002a530: 7428 5b73 656c 662e 6d61 7070 696e 672c  t([self.mapping,
+0002a540: 2073 656c 662e 6176 6169 6c61 626c 6553   self.availableS
+0002a550: 6572 6965 735d 2c20 6178 6973 3d31 290a  eries], axis=1).
+0002a560: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
+0002a570: 7069 6e67 203d 2073 656c 662e 6d61 7070  ping = self.mapp
+0002a580: 696e 672e 736f 7274 5f69 6e64 6578 2829  ing.sort_index()
+0002a590: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
+0002a5a0: 7070 696e 672e 696e 6465 782e 6e61 6d65  pping.index.name
+0002a5b0: 203d 2027 6f72 6967 6e61 6c27 0a20 2020   = 'orignal'.   
+0002a5c0: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
+0002a5d0: 672e 746f 5f65 7863 656c 2877 7269 7465  g.to_excel(write
+0002a5e0: 722c 2065 6e67 696e 653d 276f 7065 6e70  r, engine='openp
+0002a5f0: 7978 6c27 2c20 7368 6565 745f 6e61 6d65  yxl', sheet_name
+0002a600: 3d27 7363 656e 6172 696f 5f6d 6170 7069  ='scenario_mappi
+0002a610: 6e67 2729 0a0a 2020 2020 2020 2020 2320  ng')..        # 
+0002a620: 7265 6769 6f6e 0a20 2020 2020 2020 2069  region.        i
+0002a630: 6e64 6578 203d 206e 702e 756e 6971 7565  ndex = np.unique
+0002a640: 2873 656c 662e 6461 7461 5b73 656c 662e  (self.data[self.
+0002a650: 7365 7475 702e 5245 4749 4f4e 5f43 4f4c  setup.REGION_COL
+0002a660: 554d 4e5f 4e41 4d45 5d2e 7661 6c75 6573  UMN_NAME].values
+0002a670: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0002a680: 7661 696c 6162 6c65 5365 7269 6573 203d  vailableSeries =
+0002a690: 2070 642e 4461 7461 4672 616d 6528 696e   pd.DataFrame(in
+0002a6a0: 6465 783d 696e 6465 7829 0a20 2020 2020  dex=index).     
+0002a6b0: 2020 2073 656c 662e 6d61 7070 696e 6720     self.mapping 
+0002a6c0: 3d20 7064 2e44 6174 6146 7261 6d65 280a  = pd.DataFrame(.
+0002a6d0: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+0002a6e0: 783d 696e 6465 782c 2063 6f6c 756d 6e73  x=index, columns
+0002a6f0: 3d5b 7365 6c66 2e73 6574 7570 2e52 4547  =[self.setup.REG
+0002a700: 494f 4e5f 434f 4c55 4d4e 5f4e 414d 455d  ION_COLUMN_NAME]
+0002a710: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0002a720: 2020 2073 656c 662e 6d61 7070 696e 6720     self.mapping 
+0002a730: 3d20 7064 2e63 6f6e 6361 7428 5b73 656c  = pd.concat([sel
+0002a740: 662e 6d61 7070 696e 672c 2073 656c 662e  f.mapping, self.
+0002a750: 6176 6169 6c61 626c 6553 6572 6965 735d  availableSeries]
+0002a760: 2c20 6178 6973 3d31 290a 2020 2020 2020  , axis=1).      
+0002a770: 2020 7365 6c66 2e6d 6170 7069 6e67 203d    self.mapping =
+0002a780: 2073 656c 662e 6d61 7070 696e 672e 736f   self.mapping.so
+0002a790: 7274 5f69 6e64 6578 2829 0a20 2020 2020  rt_index().     
+0002a7a0: 2020 2073 656c 662e 6d61 7070 696e 672e     self.mapping.
+0002a7b0: 696e 6465 782e 6e61 6d65 203d 2027 6f72  index.name = 'or
+0002a7c0: 6967 6e61 6c27 0a20 2020 2020 2020 2066  ignal'.        f
+0002a7d0: 6f72 2069 6478 2069 6e20 7365 6c66 2e6d  or idx in self.m
+0002a7e0: 6170 7069 6e67 2e69 6e64 6578 3a0a 2020  apping.index:.  
+0002a7f0: 2020 2020 2020 2020 2020 6973 6f20 3d20            iso = 
+0002a800: 6474 2e75 7469 6c2e 6964 656e 7469 6679  dt.util.identify
+0002a810: 436f 756e 7472 7928 6964 7829 0a20 2020  Country(idx).   
+0002a820: 2020 2020 2020 2020 2069 6620 6973 6f20           if iso 
+0002a830: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002a840: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0002a850: 662e 6d61 7070 696e 672e 6c6f 635b 6964  f.mapping.loc[id
+0002a860: 782c 2027 7265 6769 6f6e 275d 203d 2069  x, 'region'] = i
+0002a870: 736f 0a0a 2020 2020 2020 2020 7365 6c66  so..        self
+0002a880: 2e6d 6170 7069 6e67 2e74 6f5f 6578 6365  .mapping.to_exce
+0002a890: 6c28 7772 6974 6572 2c20 656e 6769 6e65  l(writer, engine
+0002a8a0: 3d27 6f70 656e 7079 786c 272c 2073 6865  ='openpyxl', she
+0002a8b0: 6574 5f6e 616d 653d 2772 6567 696f 6e5f  et_name='region_
+0002a8c0: 6d61 7070 696e 6727 290a 2020 2020 2020  mapping').      
+0002a8d0: 2020 7772 6974 6572 2e63 6c6f 7365 2829    writer.close()
+0002a8e0: 0a0a 2020 2020 6465 6620 6761 7468 6572  ..    def gather
+0002a8f0: 4d61 7070 6564 4461 7461 2873 656c 662c  MappedData(self,
+0002a900: 2073 7061 7469 616c 5375 6253 6574 3d4e   spatialSubSet=N
+0002a910: 6f6e 652c 2075 7064 6174 6554 6162 6c65  one, updateTable
+0002a920: 733d 4661 6c73 6529 3a0a 0a20 2020 2020  s=False):..     
+0002a930: 2020 2069 6d70 6f72 7420 7471 646d 0a0a     import tqdm..
+0002a940: 2020 2020 2020 2020 2320 6c6f 6164 696e          # loadin
+0002a950: 6720 6461 7461 2069 6620 6e65 6365 7373  g data if necess
+0002a960: 6172 790a 2020 2020 2020 2020 6966 206e  ary.        if n
+0002a970: 6f74 2068 6173 6174 7472 2873 656c 662c  ot hasattr(self,
+0002a980: 2027 6461 7461 2729 3a0a 2020 2020 2020   'data'):.      
+0002a990: 2020 2020 2020 7365 6c66 2e6c 6f61 6444        self.loadD
+0002a9a0: 6174 6128 290a 0a20 2020 2020 2020 2074  ata()..        t
+0002a9b0: 6162 6c65 7354 6f43 6f6d 6d69 7420 3d20  ablesToCommit = 
+0002a9c0: 5b5d 0a20 2020 2020 2020 206d 6574 6144  [].        metaD
+0002a9d0: 6963 7420 3d20 6469 6374 2829 0a20 2020  ict = dict().   
+0002a9e0: 2020 2020 206d 6574 6144 6963 745b 2773       metaDict['s
+0002a9f0: 6f75 7263 6527 5d20 3d20 7365 6c66 2e73  ource'] = self.s
+0002aa00: 6574 7570 2e53 4f55 5243 455f 4944 0a20  etup.SOURCE_ID. 
+0002aa10: 2020 2020 2020 2065 7863 6c75 6465 6454         excludedT
+0002aa20: 6162 6c65 7320 3d20 6469 6374 2829 0a20  ables = dict(). 
+0002aa30: 2020 2020 2020 2065 7863 6c75 6465 6454         excludedT
+0002aa40: 6162 6c65 735b 2765 6d70 7479 275d 203d  ables['empty'] =
+0002aa50: 206c 6973 7428 290a 2020 2020 2020 2020   list().        
+0002aa60: 6578 636c 7564 6564 5461 626c 6573 5b27  excludedTables['
+0002aa70: 6572 726f 7227 5d20 3d20 6c69 7374 2829  error'] = list()
+0002aa80: 0a20 2020 2020 2020 2065 7863 6c75 6465  .        exclude
+0002aa90: 6454 6162 6c65 735b 2765 7869 7374 7327  dTables['exists'
+0002aaa0: 5d20 3d20 6c69 7374 2829 0a0a 2020 2020  ] = list()..    
+0002aab0: 2020 2020 666f 7220 6d6f 6465 6c20 696e      for model in
+0002aac0: 2073 656c 662e 6d61 7070 696e 675b 276d   self.mapping['m
+0002aad0: 6f64 656c 275d 2e6b 6579 7328 293a 0a20  odel'].keys():. 
+0002aae0: 2020 2020 2020 2020 2020 2074 656d 704d             tempM
+0002aaf0: 6f20 3d20 7365 6c66 2e64 6174 612e 6c6f  o = self.data.lo
+0002ab00: 635b 7365 6c66 2e64 6174 612e 6d6f 6465  c[self.data.mode
+0002ab10: 6c20 3d3d 206d 6f64 656c 5d0a 2020 2020  l == model].    
+0002ab20: 2020 2020 2020 2020 666f 7220 7363 656e          for scen
+0002ab30: 6172 696f 2069 6e20 7365 6c66 2e6d 6170  ario in self.map
+0002ab40: 7069 6e67 5b27 7363 656e 6172 696f 275d  ping['scenario']
+0002ab50: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
+0002ab60: 2020 2020 2020 2020 2074 656d 704d 6f53           tempMoS
+0002ab70: 6320 3d20 7465 6d70 4d6f 2e6c 6f63 5b74  c = tempMo.loc[t
+0002ab80: 656d 704d 6f2e 7363 656e 6172 696f 203d  empMo.scenario =
+0002ab90: 3d20 7363 656e 6172 696f 5d0a 2020 2020  = scenario].    
+0002aba0: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+0002abb0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0002abc0: 2076 6172 6961 626c 6520 696e 2073 656c   variable in sel
+0002abd0: 662e 6d61 7070 696e 675b 2776 6172 6961  f.mapping['varia
+0002abe0: 626c 6527 5d2e 6b65 7973 2829 3a0a 2020  ble'].keys():.  
+0002abf0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0002ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ac10: 2020 2074 656d 704d 6f53 6356 6120 3d20     tempMoScVa = 
+0002ac20: 7465 6d70 4d6f 5363 2e6c 6f63 5b73 656c  tempMoSc.loc[sel
+0002ac30: 662e 6461 7461 2e76 6172 6961 626c 6520  f.data.variable 
+0002ac40: 3d3d 2076 6172 6961 626c 655d 0a0a 2020  == variable]..  
+0002ac50: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0002ac60: 7220 7661 7269 6162 6c65 2069 6e20 6c69  r variable in li
+0002ac70: 7374 2873 656c 662e 6d61 7070 696e 675b  st(self.mapping[
+0002ac80: 2776 6172 6961 626c 6527 5d2e 6b65 7973  'variable'].keys
+0002ac90: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
+0002aca0: 2020 2020 2020 2020 2074 656d 704d 6f53           tempMoS
+0002acb0: 6356 6172 203d 2074 656d 704d 6f53 632e  cVar = tempMoSc.
+0002acc0: 6c6f 635b 7465 6d70 4d6f 5363 2e76 6172  loc[tempMoSc.var
+0002acd0: 6961 626c 6520 3d3d 2076 6172 6961 626c  iable == variabl
+0002ace0: 655d 0a20 2020 2020 2020 2020 2020 2020  e].             
+0002acf0: 2020 2020 2020 2074 656d 704d 6f53 6356         tempMoScV
+0002ad00: 6172 2e75 6e69 7420 3d20 7365 6c66 2e6d  ar.unit = self.m
+0002ad10: 6170 7069 6e67 5b27 756e 6974 275d 5b76  apping['unit'][v
+0002ad20: 6172 6961 626c 655d 0a20 2020 2020 2020  ariable].       
+0002ad30: 2020 2020 2020 2020 2020 2020 2074 6162               tab
+0002ad40: 6c65 7320 3d20 6474 2e69 6e74 6572 6661  les = dt.interfa
+0002ad50: 6365 732e 7265 6164 5f6c 6f6e 675f 7461  ces.read_long_ta
+0002ad60: 626c 6528 7465 6d70 4d6f 5363 5661 722c  ble(tempMoScVar,
+0002ad70: 205b 7661 7269 6162 6c65 5d29 0a20 2020   [variable]).   
+0002ad80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ad90: 2066 6f72 2074 6162 6c65 2069 6e20 7461   for table in ta
+0002ada0: 626c 6573 3a0a 2020 2020 2020 2020 2020  bles:.          
+0002adb0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+0002adc0: 626c 652e 6d65 7461 5b27 6361 7465 676f  ble.meta['catego
+0002add0: 7279 275d 203d 2022 220a 2020 2020 2020  ry'] = "".      
+0002ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002adf0: 2020 7461 626c 652e 6d65 7461 5b27 736f    table.meta['so
+0002ae00: 7572 6365 275d 203d 2073 656c 662e 7365  urce'] = self.se
+0002ae10: 7475 702e 534f 5552 4345 5f49 440a 2020  tup.SOURCE_ID.  
 0002ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ae30: 7461 626c 652e 696e 6465 7820 3d20 7461  table.index = ta
-0002ae40: 626c 652e 696e 6465 782e 6d61 7028 7365  ble.index.map(se
-0002ae50: 6c66 2e6d 6170 7069 6e67 5b27 7265 6769  lf.mapping['regi
-0002ae60: 6f6e 275d 290a 0a20 2020 2020 2020 2020  on'])..         
-0002ae70: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0002ae80: 6162 6c65 4944 203d 2064 742e 636f 7265  ableID = dt.core
-0002ae90: 2e5f 6372 6561 7465 4461 7461 6261 7365  ._createDatabase
-0002aea0: 4944 2874 6162 6c65 2e6d 6574 6129 0a20  ID(table.meta). 
-0002aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002aec0: 2020 2020 2020 2069 6620 6e6f 7420 7570         if not up
-0002aed0: 6461 7465 5461 626c 6573 3a0a 2020 2020  dateTables:.    
-0002aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002aef0: 2020 2020 2020 2020 6966 2064 742e 636f          if dt.co
-0002af00: 7265 2e44 422e 7461 626c 6545 7869 7374  re.DB.tableExist
-0002af10: 2874 6162 6c65 4944 293a 0a20 2020 2020  (tableID):.     
-0002af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002af30: 2020 2020 2020 2020 2020 2065 7863 6c75             exclu
-0002af40: 6465 6454 6162 6c65 735b 2765 7869 7374  dedTables['exist
-0002af50: 7327 5d2e 6170 7065 6e64 2874 6162 6c65  s'].append(table
-0002af60: 4944 290a 2020 2020 2020 2020 2020 2020  ID).            
+0002ae30: 2020 2020 2020 7461 626c 652e 696e 6465        table.inde
+0002ae40: 7820 3d20 7461 626c 652e 696e 6465 782e  x = table.index.
+0002ae50: 6d61 7028 7365 6c66 2e6d 6170 7069 6e67  map(self.mapping
+0002ae60: 5b27 7265 6769 6f6e 275d 290a 0a20 2020  ['region'])..   
+0002ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ae80: 2020 2020 2074 6162 6c65 4944 203d 2064       tableID = d
+0002ae90: 742e 636f 7265 2e5f 6372 6561 7465 4461  t.core._createDa
+0002aea0: 7461 6261 7365 4944 2874 6162 6c65 2e6d  tabaseID(table.m
+0002aeb0: 6574 6129 0a20 2020 2020 2020 2020 2020  eta).           
+0002aec0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0002aed0: 6e6f 7420 7570 6461 7465 5461 626c 6573  not updateTables
+0002aee0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002aef0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0002af00: 2064 742e 636f 7265 2e44 422e 7461 626c   dt.core.DB.tabl
+0002af10: 6545 7869 7374 2874 6162 6c65 4944 293a  eExist(tableID):
+0002af20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002af30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002af40: 2065 7863 6c75 6465 6454 6162 6c65 735b   excludedTables[
+0002af50: 2765 7869 7374 7327 5d2e 6170 7065 6e64  'exists'].append
+0002af60: 2874 6162 6c65 4944 290a 2020 2020 2020  (tableID).      
 0002af70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002af80: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0002af80: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
 0002af90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002afa0: 2020 2020 2020 7461 626c 6573 546f 436f        tablesToCo
-0002afb0: 6d6d 6974 2e61 7070 656e 6428 7461 626c  mmit.append(tabl
-0002afc0: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
-0002afd0: 6e20 7461 626c 6573 546f 436f 6d6d 6974  n tablesToCommit
-0002afe0: 2c20 6578 636c 7564 6564 5461 626c 6573  , excludedTables
-0002aff0: 0a0a 0a63 6c61 7373 2041 5045 4328 4261  ...class APEC(Ba
-0002b000: 7365 496d 706f 7274 546f 6f6c 293a 0a0a  seImportTool):..
-0002b010: 2020 2020 2222 220a 2020 2020 4952 454e      """.    IREN
-0002b020: 4120 6461 7461 2069 6d70 6f72 7420 746f  A data import to
-0002b030: 6f6c 0a20 2020 2022 2222 0a0a 2020 2020  ol.    """..    
-0002b040: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0002b050: 662c 2079 6561 7229 3a0a 2020 2020 2020  f, year):.      
-0002b060: 2020 7365 6c66 2e73 6574 7570 203d 2073    self.setup = s
-0002b070: 6574 7570 5374 7275 6374 2829 0a20 2020  etupStruct().   
-0002b080: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
-0002b090: 534f 5552 4345 5f49 4420 3d20 2241 5045  SOURCE_ID = "APE
-0002b0a0: 435f 2220 2b20 7374 7228 7965 6172 290a  C_" + str(year).
-0002b0b0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0002b0c0: 7570 2e53 4f55 5243 455f 5041 5448 203d  up.SOURCE_PATH =
-0002b0d0: 206f 732e 7061 7468 2e6a 6f69 6e28 0a20   os.path.join(. 
-0002b0e0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-0002b0f0: 672e 5041 5448 5f54 4f5f 4441 5441 5348  g.PATH_TO_DATASH
-0002b100: 454c 462c 2027 7261 7764 6174 612f 4150  ELF, 'rawdata/AP
-0002b110: 4543 2f27 202b 2073 7472 2879 6561 7229  EC/' + str(year)
-0002b120: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0002b130: 2020 2073 656c 662e 7365 7475 702e 4441     self.setup.DA
-0002b140: 5441 5f46 494c 4520 3d20 6f73 2e70 6174  TA_FILE = os.pat
-0002b150: 682e 6a6f 696e 280a 2020 2020 2020 2020  h.join(.        
-0002b160: 2020 2020 7365 6c66 2e73 6574 7570 2e53      self.setup.S
-0002b170: 4f55 5243 455f 5041 5448 2c20 2763 6f6d  OURCE_PATH, 'com
-0002b180: 7069 6c65 645f 7261 775f 686f 6573 6c79  piled_raw_hoesly
-0002b190: 2e63 7376 270a 2020 2020 2020 2020 290a  .csv'.        ).
-0002b1a0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0002b1b0: 7570 2e4d 4150 5049 4e47 5f46 494c 4520  up.MAPPING_FILE 
-0002b1c0: 3d20 6f73 2e70 6174 682e 6a6f 696e 2873  = os.path.join(s
-0002b1d0: 656c 662e 7365 7475 702e 534f 5552 4345  elf.setup.SOURCE
-0002b1e0: 5f50 4154 482c 2027 6d61 7070 696e 672e  _PATH, 'mapping.
-0002b1f0: 786c 7378 2729 0a20 2020 2020 2020 2073  xlsx').        s
-0002b200: 656c 662e 7365 7475 702e 4c49 4345 4e43  elf.setup.LICENC
-0002b210: 4520 3d20 2728 6329 2032 3031 3920 4173  E = '(c) 2019 As
-0002b220: 6961 2050 6163 6966 6963 2045 636f 6e6f  ia Pacific Econo
-0002b230: 6d69 6320 436f 6f70 6572 6174 696f 6e20  mic Cooperation 
-0002b240: 2841 5045 5243 2927 0a20 2020 2020 2020  (APERC)'.       
-0002b250: 2073 656c 662e 7365 7475 702e 5552 4c20   self.setup.URL 
-0002b260: 3d20 2768 7474 7073 3a2f 2f77 7777 2e61  = 'https://www.a
-0002b270: 7065 632e 6f72 672f 5075 626c 6963 6174  pec.org/Publicat
-0002b280: 696f 6e73 2f32 3031 392f 3035 2f41 5045  ions/2019/05/APE
-0002b290: 432d 456e 6572 6779 2d44 656d 616e 642d  C-Energy-Demand-
-0002b2a0: 616e 642d 5375 7070 6c79 2d4f 7574 6c6f  and-Supply-Outlo
-0002b2b0: 6f6b 2d37 7468 2d45 6469 7469 6f6e 2d2d  ok-7th-Edition--
-0002b2c0: 2d56 6f6c 756d 652d 4927 0a0a 2020 2020  -Volume-I'..    
-0002b2d0: 2020 2020 2320 2020 2020 2020 2073 656c      #        sel
-0002b2e0: 662e 7365 7475 702e 494e 4445 585f 434f  f.setup.INDEX_CO
-0002b2f0: 4c55 4d4e 5f4e 414d 4520 3d20 5b27 464c  LUMN_NAME = ['FL
-0002b300: 4f57 272c 2027 5052 4f44 5543 5427 5d0a  OW', 'PRODUCT'].
-0002b310: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0002b320: 2073 656c 662e 7365 7475 702e 5350 4154   self.setup.SPAT
-0002b330: 4941 4c5f 434f 4c55 4d5f 4e41 4d45 203d  IAL_COLUM_NAME =
-0002b340: 2027 434f 554e 5452 5927 0a20 2020 2020   'COUNTRY'.     
-0002b350: 2020 2023 2020 2020 2020 2020 7365 6c66     #        self
-0002b360: 2e73 6574 7570 2e43 4f4c 554d 4e53 5f54  .setup.COLUMNS_T
-0002b370: 4f5f 4452 4f50 203d 205b 2027 5052 4f44  O_DROP = [ 'PROD
-0002b380: 5543 5427 2c27 464c 4f57 272c 2763 6f6d  UCT','FLOW','com
-0002b390: 6269 6e65 6427 5d0a 0a20 2020 2020 2020  bined']..       
-0002b3a0: 2069 6620 6e6f 7420 286f 732e 7061 7468   if not (os.path
-0002b3b0: 2e65 7869 7374 7328 7365 6c66 2e73 6574  .exists(self.set
-0002b3c0: 7570 2e4d 4150 5049 4e47 5f46 494c 4529  up.MAPPING_FILE)
-0002b3d0: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
-0002b3e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002b3f0: 2e63 7265 6174 6556 6172 6961 626c 654d  .createVariableM
-0002b400: 6170 7069 6e67 2829 0a20 2020 2020 2020  apping().       
-0002b410: 2020 2020 2070 7269 6e74 2822 6e6f 206d       print("no m
-0002b420: 6170 7069 6e67 2066 696c 6520 666f 756e  apping file foun
-0002b430: 6422 290a 2020 2020 2020 2020 656c 7365  d").        else
-0002b440: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002b450: 6c66 2e6d 6170 7069 6e67 203d 2070 642e  lf.mapping = pd.
-0002b460: 7265 6164 5f65 7863 656c 2873 656c 662e  read_excel(self.
-0002b470: 7365 7475 702e 4d41 5050 494e 475f 4649  setup.MAPPING_FI
-0002b480: 4c45 2c20 7368 6565 745f 6e61 6d65 3d27  LE, sheet_name='
-0002b490: 4150 4543 2729 0a0a 2020 2020 2020 2020  APEC')..        
-0002b4a0: 2020 2020 7365 6c66 2e73 7061 7469 616c      self.spatial
-0002b4b0: 4d61 7070 696e 6720 3d20 7064 2e72 6561  Mapping = pd.rea
-0002b4c0: 645f 6578 6365 6c28 0a20 2020 2020 2020  d_excel(.       
-0002b4d0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-0002b4e0: 7475 702e 4d41 5050 494e 475f 4649 4c45  tup.MAPPING_FILE
-0002b4f0: 2c20 7368 6565 745f 6e61 6d65 3d27 7370  , sheet_name='sp
-0002b500: 6174 6961 6c27 2c20 696e 6465 785f 636f  atial', index_co
-0002b510: 6c3d 300a 2020 2020 2020 2020 2020 2020  l=0.            
-0002b520: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0002b530: 6c66 2e73 7061 7469 616c 4d61 7070 696e  lf.spatialMappin
-0002b540: 6720 3d20 7365 6c66 2e73 7061 7469 616c  g = self.spatial
-0002b550: 4d61 7070 696e 672e 6c6f 635b 0a20 2020  Mapping.loc[.   
-0002b560: 2020 2020 2020 2020 2020 2020 207e 7064               ~pd
-0002b570: 2e69 736e 756c 6c28 7365 6c66 2e73 7061  .isnull(self.spa
-0002b580: 7469 616c 4d61 7070 696e 672e 6d61 7070  tialMapping.mapp
-0002b590: 696e 6729 0a20 2020 2020 2020 2020 2020  ing).           
-0002b5a0: 205d 0a0a 2020 2020 2020 2020 7365 6c66   ]..        self
-0002b5b0: 2e63 7265 6174 6553 6f75 7263 654d 6574  .createSourceMet
-0002b5c0: 6128 290a 0a20 2020 2064 6566 2061 6464  a()..    def add
-0002b5d0: 5370 6174 6961 6c4d 6170 7069 6e67 2873  SpatialMapping(s
-0002b5e0: 656c 6629 3a0a 2020 2020 2020 2020 2320  elf):.        # 
-0002b5f0: 4555 0a20 2020 2020 2020 206d 6170 7069  EU.        mappi
-0002b600: 6e67 546f 436f 756e 7472 6965 7320 3d20  ngToCountries = 
-0002b610: 6469 6374 2829 0a20 2020 2020 2020 2023  dict().        #
-0002b620: 2073 656c 662e 7370 6174 6961 6c4d 6170   self.spatialMap
-0002b630: 7069 6e67 2e6c 6f63 5b27 4d65 6d6f 3a20  ping.loc['Memo: 
-0002b640: 4575 726f 7065 616e 2055 6e69 6f6e 2d32  European Union-2
-0002b650: 3827 5d20 3d20 2745 5532 3827 0a0a 2020  8'] = 'EU28'..  
-0002b660: 2020 2320 2020 2020 2020 206d 6170 7069    #        mappi
-0002b670: 6e67 546f 436f 756e 7472 6965 735b 2741  ngToCountries['A
-0002b680: 5345 414e 275d 203d 2020 5b27 564e 4d27  SEAN'] =  ['VNM'
-0002b690: 2c20 2750 484c 272c 2027 5448 4127 2c20  , 'PHL', 'THA', 
-0002b6a0: 2753 4750 272c 2027 4d4d 5227 2c20 2749  'SGP', 'MMR', 'I
-0002b6b0: 444e 272c 2027 4b48 4d27 2c20 2742 524e  DN', 'KHM', 'BRN
-0002b6c0: 272c 2027 4d59 5327 2c20 274c 414f 275d  ', 'MYS', 'LAO']
-0002b6d0: 0a20 2020 2023 2020 2020 2020 2020 6474  .    #        dt
-0002b6e0: 2e6d 6170 702e 7265 6769 6f6e 732e 6164  .mapp.regions.ad
-0002b6f0: 6452 6567 696f 6e54 6f43 6f6e 7465 7874  dRegionToContext
-0002b700: 2827 5745 4f27 2c6d 6170 7069 6e67 546f  ('WEO',mappingTo
-0002b710: 436f 756e 7472 6965 7329 0a0a 2020 2020  Countries)..    
-0002b720: 6465 6620 6761 7468 6572 4d61 7070 6564  def gatherMapped
-0002b730: 4461 7461 2873 656c 662c 2073 7061 7469  Data(self, spati
-0002b740: 616c 5375 6253 6574 3d4e 6f6e 6529 3a0a  alSubSet=None):.
-0002b750: 0a20 2020 2020 2020 2074 6162 6c65 7354  .        tablesT
-0002b760: 6f43 6f6d 6d69 7420 3d20 6474 2e54 6162  oCommit = dt.Tab
-0002b770: 6c65 5365 7428 290a 2020 2020 2020 2020  leSet().        
-0002b780: 7365 7475 7020 3d20 6469 6374 2829 0a20  setup = dict(). 
-0002b790: 2020 2020 2020 2073 6574 7570 5b27 6669         setup['fi
-0002b7a0: 6c65 5061 7468 275d 203d 2073 656c 662e  lePath'] = self.
-0002b7b0: 7365 7475 702e 534f 5552 4345 5f50 4154  setup.SOURCE_PAT
-0002b7c0: 480a 2020 2020 2020 2020 7365 7475 705b  H.        setup[
-0002b7d0: 2766 696c 654e 616d 6527 5d20 3d20 2741  'fileName'] = 'A
-0002b7e0: 5045 435f 456e 6572 6779 5f4f 7574 6c6f  PEC_Energy_Outlo
-0002b7f0: 6f6b 5f37 7468 5f45 6469 7469 6f6e 5f54  ok_7th_Edition_T
-0002b800: 6162 6c65 732e 786c 7378 270a 0a20 2020  ables.xlsx'..   
-0002b810: 2020 2020 2023 206c 6f6f 7020 6f76 6572       # loop over
-0002b820: 2065 6e65 7267 7920 6d61 7070 696e 670a   energy mapping.
-0002b830: 2020 2020 2020 2020 666f 7220 7265 6769          for regi
-0002b840: 6f6e 2069 6e20 7365 6c66 2e73 7061 7469  on in self.spati
-0002b850: 616c 4d61 7070 696e 672e 696e 6465 783a  alMapping.index:
-0002b860: 0a20 2020 2020 2020 2020 2020 2073 6574  .            set
-0002b870: 7570 5b27 7368 6565 744e 616d 6527 5d20  up['sheetName'] 
-0002b880: 3d20 7265 6769 6f6e 0a20 2020 2020 2020  = region.       
-0002b890: 2020 2020 2073 6574 7570 5b27 7469 6d65       setup['time
-0002b8a0: 436f 6c49 6478 275d 203d 205b 2741 4f3a  ColIdx'] = ['AO:
-0002b8b0: 4130 275d 0a20 2020 2020 2020 2020 2020  A0'].           
-0002b8c0: 2073 6574 7570 5b27 7370 6163 6552 6f77   setup['spaceRow
-0002b8d0: 4964 7827 5d20 3d20 5b27 414f 3a41 3027  Idx'] = ['AO:A0'
-0002b8e0: 5d0a 0a20 2020 2020 2020 2020 2020 2065  ]..            e
-0002b8f0: 7820 3d20 6474 2e69 6f2e 4578 6365 6c52  x = dt.io.ExcelR
-0002b900: 6561 6465 7228 7365 7475 7029 0a20 2020  eader(setup).   
-0002b910: 2020 2020 2020 2020 2063 6f49 534f 203d           coISO =
-0002b920: 2073 656c 662e 7370 6174 6961 6c4d 6170   self.spatialMap
-0002b930: 7069 6e67 2e6c 6f63 5b72 6567 696f 6e2c  ping.loc[region,
-0002b940: 2027 6d61 7070 696e 6727 5d0a 2020 2020   'mapping'].    
-0002b950: 2020 2020 2020 2020 7072 696e 7428 7265          print(re
-0002b960: 6769 6f6e 2c20 6578 2e67 6174 6865 7256  gion, ex.gatherV
-0002b970: 616c 7565 2827 4231 2729 202b 2027 2d3e  alue('B1') + '->
-0002b980: 2720 2b20 636f 4953 4f29 0a20 2020 2020  ' + coISO).     
-0002b990: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-0002b9a0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0002b9b0: 2069 2c20 6964 7820 696e 2065 6e75 6d65   i, idx in enume
-0002b9c0: 7261 7465 286c 6973 7428 7365 6c66 2e6d  rate(list(self.m
-0002b9d0: 6170 7069 6e67 2e69 6e64 6578 2929 3a0a  apping.index)):.
-0002b9e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b9f0: 206d 6574 6144 6620 3d20 7365 6c66 2e6d   metaDf = self.m
-0002ba00: 6170 7069 6e67 2e6c 6f63 5b69 6478 2c20  apping.loc[idx, 
-0002ba10: 3a5d 0a20 2020 2020 2020 2020 2020 2020  :].             
-0002ba20: 2020 2023 2070 7269 6e74 286d 6574 6144     # print(metaD
-0002ba30: 665b 2757 6861 7427 5d29 0a0a 2020 2020  f['What'])..    
-0002ba40: 2020 2020 2020 2020 2020 2020 2320 4361              # Ca
-0002ba50: 7061 6369 7479 0a20 2020 2020 2020 2020  pacity.         
-0002ba60: 2020 2020 2020 2073 6574 7570 5b27 7469         setup['ti
-0002ba70: 6d65 436f 6c49 6478 275d 203d 2074 7570  meColIdx'] = tup
-0002ba80: 6c65 286d 6574 6144 665b 2754 696d 6527  le(metaDf['Time'
-0002ba90: 5d2e 7370 6c69 7428 273a 2729 290a 2020  ].split(':')).  
-0002baa0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0002bab0: 7475 705b 2773 7061 6365 526f 7749 6478  tup['spaceRowIdx
-0002bac0: 275d 203d 2074 7570 6c65 285b 6d65 7461  '] = tuple([meta
-0002bad0: 4466 5b27 5768 6174 275d 5d29 0a20 2020  Df['What']]).   
-0002bae0: 2020 2020 2020 2020 2020 2020 2023 2070               # p
-0002baf0: 7269 6e74 286d 6574 6144 665b 636f 6e66  rint(metaDf[conf
-0002bb00: 6967 2e52 4551 5549 5245 445f 4d45 5441  ig.REQUIRED_META
-0002bb10: 5f46 4945 4c44 535d 2e69 736e 756c 6c28  _FIELDS].isnull(
-0002bb20: 292e 616c 6c28 2920 3d3d 2046 616c 7365  ).all() == False
-0002bb30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0002bb40: 2020 2320 7072 696e 7428 6d65 7461 4461    # print(metaDa
-0002bb50: 7461 5b73 656c 662e 7365 7475 702e 494e  ta[self.setup.IN
-0002bb60: 4445 585f 434f 4c55 4d4e 5f4e 414d 455d  DEX_COLUMN_NAME]
-0002bb70: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-0002bb80: 2020 2065 782e 7469 6d65 436f 6c49 6478     ex.timeColIdx
-0002bb90: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-0002bba0: 2020 2020 2020 2020 2064 742e 696f 2e65           dt.io.e
-0002bbb0: 7863 656c 4964 7832 5061 6e64 6173 4964  xcelIdx2PandasId
-0002bbc0: 7828 7829 2066 6f72 2078 2069 6e20 7365  x(x) for x in se
-0002bbd0: 7475 705b 2774 696d 6543 6f6c 4964 7827  tup['timeColIdx'
-0002bbe0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0002bbf0: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
-0002bc00: 2020 2020 6578 2e73 7061 6365 526f 7749      ex.spaceRowI
-0002bc10: 6478 203d 205b 0a20 2020 2020 2020 2020  dx = [.         
-0002bc20: 2020 2020 2020 2020 2020 2064 742e 696f             dt.io
-0002bc30: 2e65 7863 656c 4964 7832 5061 6e64 6173  .excelIdx2Pandas
-0002bc40: 4964 7828 7829 2066 6f72 2078 2069 6e20  Idx(x) for x in 
-0002bc50: 7365 7475 705b 2773 7061 6365 526f 7749  setup['spaceRowI
-0002bc60: 6478 275d 0a20 2020 2020 2020 2020 2020  dx'].           
-0002bc70: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
-0002bc80: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0002bc90: 2020 2020 2020 2020 6966 2022 496e 7465          if "Inte
-0002bca0: 726e 6174 696f 6e61 6c22 2069 6e20 6d65  rnational" in me
-0002bcb0: 7461 4466 5b27 4e61 6d65 275d 3a0a 2020  taDf['Name']:.  
-0002bcc0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0002bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bce0: 2020 2073 6466 0a20 2020 2020 2020 2020     sdf.         
-0002bcf0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0002bd00: 2020 2020 2020 2020 6966 2065 782e 7370          if ex.sp
-0002bd10: 6163 6552 6f77 4964 785b 305d 5b30 5d3e  aceRowIdx[0][0]>
-0002bd20: 3431 2061 6e64 2072 6567 696f 6e20 213d  41 and region !=
-0002bd30: 2027 576f 726c 6427 3a0a 2020 2020 2020   'World':.      
-0002bd40: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-0002bd50: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0002bd60: 782e 7370 6163 6552 6f77 4964 7820 3d20  x.spaceRowIdx = 
-0002bd70: 5b28 6578 2e73 7061 6365 526f 7749 6478  [(ex.spaceRowIdx
-0002bd80: 5b30 5d5b 305d 2d31 2c30 295d 0a0a 2020  [0][0]-1,0)]..  
-0002bd90: 2020 2020 2020 2020 2020 2020 2020 6466                df
-0002bda0: 203d 2065 782e 6761 7468 6572 4461 7461   = ex.gatherData
-0002bdb0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-0002bdc0: 2020 2064 662e 636f 6c75 6d6e 7320 3d20     df.columns = 
-0002bdd0: 6466 2e63 6f6c 756d 6e73 2e61 7374 7970  df.columns.astyp
-0002bde0: 6528 696e 7429 0a20 2020 2020 2020 2020  e(int).         
-0002bdf0: 2020 2020 2020 206d 6574 6144 6963 7420         metaDict 
-0002be00: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0002be10: 2020 2020 2020 2020 206d 6574 6144 6963           metaDic
-0002be20: 745b 2765 6e74 6974 7927 5d20 3d20 6d65  t['entity'] = me
-0002be30: 7461 4466 5b27 4e61 6d65 275d 2e73 7472  taDf['Name'].str
-0002be40: 6970 2829 2e72 6570 6c61 6365 2827 7c20  ip().replace('| 
-0002be50: 272c 2027 7c27 290a 2020 2020 2020 2020  ', '|').        
-0002be60: 2020 2020 2020 2020 6d65 7461 4469 6374          metaDict
-0002be70: 5b27 6361 7465 676f 7279 275d 203d 2027  ['category'] = '
-0002be80: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-0002be90: 2020 6d65 7461 4469 6374 5b27 756e 6974    metaDict['unit
-0002bea0: 275d 203d 206d 6574 6144 665b 2775 6e69  '] = metaDf['uni
-0002beb0: 7427 5d0a 2020 2020 2020 2020 2020 2020  t'].            
-0002bec0: 2020 2020 6d65 7461 4469 6374 5b27 7363      metaDict['sc
-0002bed0: 656e 6172 696f 275d 203d 206d 6574 6144  enario'] = metaD
-0002bee0: 665b 2753 6365 6e61 7269 6f27 5d0a 2020  f['Scenario'].  
-0002bef0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-0002bf00: 7461 4469 6374 5b27 736f 7572 6365 275d  taDict['source']
-0002bf10: 203d 2073 656c 662e 7365 7475 702e 534f   = self.setup.SO
-0002bf20: 5552 4345 5f49 440a 2020 2020 2020 2020  URCE_ID.        
-0002bf30: 2020 2020 2020 2020 6d65 7461 4469 6374          metaDict
-0002bf40: 5b27 756e 6974 546f 275d 203d 206d 6574  ['unitTo'] = met
-0002bf50: 6144 665b 2775 6e69 7454 6f27 5d0a 2020  aDf['unitTo'].  
-0002bf60: 2020 2020 2020 2020 2020 2020 2020 4944                ID
-0002bf70: 203d 2064 742e 636f 7265 2e5f 6372 6561   = dt.core._crea
-0002bf80: 7465 4461 7461 6261 7365 4944 286d 6574  teDatabaseID(met
-0002bf90: 6144 6963 7429 0a0a 2020 2020 2020 2020  aDict)..        
-0002bfa0: 2020 2020 2020 2020 6966 2049 4420 6e6f          if ID no
-0002bfb0: 7420 696e 2074 6162 6c65 7354 6f43 6f6d  t in tablesToCom
-0002bfc0: 6d69 742e 6b65 7973 2829 3a0a 2020 2020  mit.keys():.    
-0002bfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bfe0: 7461 626c 6520 3d20 6474 2e44 6174 6174  table = dt.Datat
-0002bff0: 6162 6c65 2863 6f6c 756d 6e73 3d72 616e  able(columns=ran
-0002c000: 6765 2832 3030 302c 2032 3130 3029 2c20  ge(2000, 2100), 
-0002c010: 6d65 7461 3d6d 6574 6144 6963 7429 0a0a  meta=metaDict)..
-0002c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c030: 2020 2020 7461 626c 652e 6c6f 635b 636f      table.loc[co
-0002c040: 4953 4f2c 2064 662e 636f 6c75 6d6e 735d  ISO, df.columns]
-0002c050: 203d 2064 662e 7661 6c75 6573 0a20 2020   = df.values.   
-0002c060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c070: 2074 6162 6c65 7354 6f43 6f6d 6d69 742e   tablesToCommit.
-0002c080: 6164 6428 7461 626c 6529 0a20 2020 2020  add(table).     
-0002c090: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0002c0a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002c0b0: 2020 2020 2074 6162 6c65 203d 2074 6162       table = tab
-0002c0c0: 6c65 7354 6f43 6f6d 6d69 745b 4944 5d0a  lesToCommit[ID].
-0002c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c0e0: 2020 2020 7461 626c 652e 6c6f 635b 636f      table.loc[co
-0002c0f0: 4953 4f2c 2064 662e 636f 6c75 6d6e 735d  ISO, df.columns]
-0002c100: 203d 2064 662e 7661 6c75 6573 0a0a 2020   = df.values..  
-0002c110: 2020 2020 2020 7461 626c 6573 4c69 7374        tablesList
-0002c120: 203d 206c 6973 7428 290a 2020 2020 2020   = list().      
-0002c130: 2020 666f 7220 4944 2069 6e20 7461 626c    for ID in tabl
-0002c140: 6573 546f 436f 6d6d 6974 2e6b 6579 7328  esToCommit.keys(
-0002c150: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
-0002c160: 6174 6154 6162 6c65 203d 2074 6162 6c65  ataTable = table
-0002c170: 7354 6f43 6f6d 6d69 745b 4944 5d0a 2020  sToCommit[ID].  
-0002c180: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0002c190: 6461 7461 5461 626c 652e 6d65 7461 290a  dataTable.meta).
-0002c1a0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0002c1b0: 6f74 2070 642e 6973 6e61 2864 6174 6154  ot pd.isna(dataT
-0002c1c0: 6162 6c65 2e6d 6574 615b 2775 6e69 7454  able.meta['unitT
-0002c1d0: 6f27 5d29 3a0a 2020 2020 2020 2020 2020  o']):.          
-0002c1e0: 2020 2020 2020 6461 7461 5461 626c 6520        dataTable 
-0002c1f0: 3d20 6461 7461 5461 626c 652e 636f 6e76  = dataTable.conv
-0002c200: 6572 7428 6461 7461 5461 626c 652e 6d65  ert(dataTable.me
-0002c210: 7461 5b27 756e 6974 546f 275d 290a 2020  ta['unitTo']).  
-0002c220: 2020 2020 2020 2020 2020 2020 2020 6465                de
-0002c230: 6c20 6461 7461 5461 626c 652e 6d65 7461  l dataTable.meta
-0002c240: 5b27 756e 6974 546f 275d 0a20 2020 2020  ['unitTo'].     
-0002c250: 2020 2020 2020 2074 6162 6c65 734c 6973         tablesLis
-0002c260: 742e 6170 7065 6e64 2864 6174 6154 6162  t.append(dataTab
-0002c270: 6c65 2e61 7374 7970 6528 666c 6f61 7429  le.astype(float)
-0002c280: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-0002c290: 6e20 7461 626c 6573 4c69 7374 2c20 5b5d  n tablesList, []
-0002c2a0: 0a0a 0a63 6c61 7373 2046 414f 2842 6173  ...class FAO(Bas
-0002c2b0: 6549 6d70 6f72 7454 6f6f 6c29 3a0a 2020  eImportTool):.  
-0002c2c0: 2020 2222 220a 2020 2020 4641 4f20 6461    """.    FAO da
-0002c2d0: 7461 2069 6d70 6f72 7420 746f 6f6c 0a20  ta import tool. 
-0002c2e0: 2020 2022 2222 0a0a 2020 2020 6465 6620     """..    def 
-0002c2f0: 5f5f 696e 6974 5f5f 2873 656c 662c 2079  __init__(self, y
-0002c300: 6561 723d 3230 3139 2c20 6461 7461 5f70  ear=2019, data_p
-0002c310: 6174 683d 4e6f 6e65 293a 0a0a 2020 2020  ath=None):..    
-0002c320: 2020 2020 6966 2064 6174 615f 7061 7468      if data_path
-0002c330: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0002c340: 2020 2020 2020 6461 7461 5f70 6174 6820        data_path 
-0002c350: 3d20 6f73 2e70 6174 682e 6a6f 696e 2863  = os.path.join(c
-0002c360: 6f6e 6669 672e 5041 5448 5f54 4f5f 4441  onfig.PATH_TO_DA
-0002c370: 5441 5348 454c 462c 2027 7261 7764 6174  TASHELF, 'rawdat
-0002c380: 6127 290a 0a20 2020 2020 2020 2073 656c  a')..        sel
-0002c390: 662e 7365 7475 7020 3d20 7365 7475 7053  f.setup = setupS
-0002c3a0: 7472 7563 7428 290a 2020 2020 2020 2020  truct().        
-0002c3b0: 7365 6c66 2e73 6574 7570 2e53 4f55 5243  self.setup.SOURC
-0002c3c0: 455f 4944 203d 2022 4641 4f5f 2220 2b20  E_ID = "FAO_" + 
-0002c3d0: 7374 7228 7965 6172 290a 2020 2020 2020  str(year).      
-0002c3e0: 2020 7365 6c66 2e73 6574 7570 2e53 4f55    self.setup.SOU
-0002c3f0: 5243 455f 5041 5448 203d 206f 732e 7061  RCE_PATH = os.pa
-0002c400: 7468 2e6a 6f69 6e28 6461 7461 5f70 6174  th.join(data_pat
-0002c410: 682c 2027 4641 4f5f 2720 2b20 7374 7228  h, 'FAO_' + str(
-0002c420: 7965 6172 2929 0a20 2020 2020 2020 2073  year)).        s
-0002c430: 656c 662e 7365 7475 702e 4441 5441 5f46  elf.setup.DATA_F
-0002c440: 494c 4520 3d20 7b0a 2020 2020 2020 2020  ILE = {.        
-0002c450: 2020 2020 2745 6d69 7373 696f 6e73 5f4c      'Emissions_L
-0002c460: 616e 645f 5573 655f 273a 206f 732e 7061  and_Use_': os.pa
-0002c470: 7468 2e6a 6f69 6e28 0a20 2020 2020 2020  th.join(.       
-0002c480: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-0002c490: 7475 702e 534f 5552 4345 5f50 4154 482c  tup.SOURCE_PATH,
-0002c4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002c4b0: 2027 456d 6973 7369 6f6e 735f 4c61 6e64   'Emissions_Land
-0002c4c0: 5f55 7365 5f4c 616e 645f 5573 655f 546f  _Use_Land_Use_To
-0002c4d0: 7461 6c5f 455f 416c 6c5f 4461 7461 2e63  tal_E_All_Data.c
-0002c4e0: 7376 272c 0a20 2020 2020 2020 2020 2020  sv',.           
-0002c4f0: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-0002c500: 2745 6d69 7373 696f 6e73 5f41 6772 6963  'Emissions_Agric
-0002c510: 756c 7475 7265 5f27 3a20 6f73 2e70 6174  ulture_': os.pat
-0002c520: 682e 6a6f 696e 280a 2020 2020 2020 2020  h.join(.        
-0002c530: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0002c540: 7570 2e53 4f55 5243 455f 5041 5448 2c0a  up.SOURCE_PATH,.
-0002c550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c560: 2745 6d69 7373 696f 6e73 5f41 6772 6963  'Emissions_Agric
-0002c570: 756c 7475 7265 5f41 6772 6963 756c 7475  ulture_Agricultu
-0002c580: 7265 5f74 6f74 616c 5f45 5f41 6c6c 5f44  re_total_E_All_D
-0002c590: 6174 612e 6373 7627 2c0a 2020 2020 2020  ata.csv',.      
-0002c5a0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-0002c5b0: 2020 2020 2027 456e 7669 726f 6e6d 656e       'Environmen
-0002c5c0: 745f 456d 6973 7369 6f6e 735f 6279 5f53  t_Emissions_by_S
-0002c5d0: 6563 746f 725f 273a 206f 732e 7061 7468  ector_': os.path
-0002c5e0: 2e6a 6f69 6e28 0a20 2020 2020 2020 2020  .join(.         
-0002c5f0: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
-0002c600: 702e 534f 5552 4345 5f50 4154 482c 2027  p.SOURCE_PATH, '
-0002c610: 456e 7669 726f 6e6d 656e 745f 456d 6973  Environment_Emis
-0002c620: 7369 6f6e 735f 6279 5f53 6563 746f 725f  sions_by_Sector_
-0002c630: 455f 416c 6c5f 4461 7461 2e63 7376 270a  E_All_Data.csv'.
-0002c640: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-0002c650: 2020 2020 2020 2020 2020 2027 456e 7669             'Envi
-0002c660: 726f 6e6d 656e 745f 456d 6973 7369 6f6e  ronment_Emission
-0002c670: 735f 696e 7465 6e73 6974 6965 735f 273a  s_intensities_':
-0002c680: 206f 732e 7061 7468 2e6a 6f69 6e28 0a20   os.path.join(. 
-0002c690: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0002c6a0: 656c 662e 7365 7475 702e 534f 5552 4345  elf.setup.SOURCE
-0002c6b0: 5f50 4154 482c 0a20 2020 2020 2020 2020  _PATH,.         
-0002c6c0: 2020 2020 2020 2027 456e 7669 726f 6e6d         'Environm
-0002c6d0: 656e 745f 456d 6973 7369 6f6e 735f 696e  ent_Emissions_in
-0002c6e0: 7465 6e73 6974 6965 735f 455f 416c 6c5f  tensities_E_All_
-0002c6f0: 4461 7461 2e63 7376 272c 0a20 2020 2020  Data.csv',.     
-0002c700: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-0002c710: 2020 2020 2020 2745 6e76 6972 6f6e 6d65        'Environme
-0002c720: 6e74 5f4c 616e 6443 6f76 6572 5f27 3a20  nt_LandCover_': 
-0002c730: 6f73 2e70 6174 682e 6a6f 696e 280a 2020  os.path.join(.  
-0002c740: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0002c750: 6c66 2e73 6574 7570 2e53 4f55 5243 455f  lf.setup.SOURCE_
-0002c760: 5041 5448 2c20 2745 6e76 6972 6f6e 6d65  PATH, 'Environme
-0002c770: 6e74 5f4c 616e 6443 6f76 6572 5f45 5f41  nt_LandCover_E_A
-0002c780: 6c6c 5f44 6174 612e 6373 7627 0a20 2020  ll_Data.csv'.   
-0002c790: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-0002c7a0: 2020 2020 2020 2020 2745 6e76 6972 6f6e          'Environ
-0002c7b0: 6d65 6e74 5f4c 616e 6455 7365 5f27 3a20  ment_LandUse_': 
-0002c7c0: 6f73 2e70 6174 682e 6a6f 696e 280a 2020  os.path.join(.  
-0002c7d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0002c7e0: 6c66 2e73 6574 7570 2e53 4f55 5243 455f  lf.setup.SOURCE_
-0002c7f0: 5041 5448 2c20 2745 6e76 6972 6f6e 6d65  PATH, 'Environme
-0002c800: 6e74 5f4c 616e 6455 7365 5f45 5f41 6c6c  nt_LandUse_E_All
-0002c810: 5f44 6174 612e 6373 7627 0a20 2020 2020  _Data.csv'.     
-0002c820: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-0002c830: 2020 2020 2020 2749 6e70 7574 735f 4c61        'Inputs_La
-0002c840: 6e64 5573 655f 273a 206f 732e 7061 7468  ndUse_': os.path
-0002c850: 2e6a 6f69 6e28 0a20 2020 2020 2020 2020  .join(.         
-0002c860: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
-0002c870: 702e 534f 5552 4345 5f50 4154 482c 2027  p.SOURCE_PATH, '
-0002c880: 496e 7075 7473 5f4c 616e 6455 7365 5f45  Inputs_LandUse_E
-0002c890: 5f41 6c6c 5f44 6174 612e 6373 7627 0a20  _All_Data.csv'. 
-0002c8a0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-0002c8b0: 2020 2020 2020 2020 2020 2745 6d69 7373            'Emiss
-0002c8c0: 696f 6e73 5f54 6f74 616c 273a 206f 732e  ions_Total': os.
-0002c8d0: 7061 7468 2e6a 6f69 6e28 0a20 2020 2020  path.join(.     
-0002c8e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002c8f0: 7365 7475 702e 534f 5552 4345 5f50 4154  setup.SOURCE_PAT
-0002c900: 482c 2027 456d 6973 7369 6f6e 735f 546f  H, 'Emissions_To
-0002c910: 7461 6c73 5f45 5f41 6c6c 5f44 6174 612e  tals_E_All_Data.
-0002c920: 6373 7627 0a20 2020 2020 2020 2020 2020  csv'.           
-0002c930: 2029 2c0a 2020 2020 2020 2020 7d0a 0a20   ),.        }.. 
-0002c940: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
-0002c950: 702e 4d41 5050 494e 475f 4649 4c45 203d  p.MAPPING_FILE =
-0002c960: 206f 732e 7061 7468 2e6a 6f69 6e28 0a20   os.path.join(. 
-0002c970: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002c980: 7365 7475 702e 534f 5552 4345 5f50 4154  setup.SOURCE_PAT
-0002c990: 482c 2027 6d61 7070 696e 675f 3230 3232  H, 'mapping_2022
-0002c9a0: 2e78 6c73 7827 0a20 2020 2020 2020 2029  .xlsx'.        )
-0002c9b0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0002c9c0: 7475 702e 4c49 4345 4e43 4520 3d20 280a  tup.LICENCE = (.
-0002c9d0: 2020 2020 2020 2020 2020 2020 2746 6f6f              'Foo
-0002c9e0: 6420 616e 6420 4167 7269 6375 6c74 7572  d and Agricultur
-0002c9f0: 6520 4f72 6761 6e69 7a61 7469 6f6e 206f  e Organization o
-0002ca00: 6620 7468 6520 556e 6974 6564 204e 6174  f the United Nat
-0002ca10: 696f 6e73 2028 4641 4f29 270a 2020 2020  ions (FAO)'.    
-0002ca20: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-0002ca30: 6c66 2e73 6574 7570 2e55 524c 203d 2027  lf.setup.URL = '
-0002ca40: 6874 7470 3a2f 2f77 7777 2e66 616f 2e6f  http://www.fao.o
-0002ca50: 7267 2f66 616f 7374 6174 2f65 6e2f 2364  rg/faostat/en/#d
-0002ca60: 6174 612f 474c 270a 2020 2020 2020 2020  ata/GL'.        
-0002ca70: 2320 2020 2020 2020 2073 656c 662e 7365  #        self.se
-0002ca80: 7475 702e 4d4f 4445 4c5f 434f 4c55 4d4e  tup.MODEL_COLUMN
-0002ca90: 5f4e 414d 4520 3d20 276d 6f64 656c 270a  _NAME = 'model'.
-0002caa0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0002cab0: 7570 2e53 4345 4e41 5249 4f5f 434f 4c55  up.SCENARIO_COLU
-0002cac0: 4d4e 5f4e 414d 4520 3d20 2773 6365 6e61  MN_NAME = 'scena
-0002cad0: 7269 6f27 0a20 2020 2020 2020 2073 656c  rio'.        sel
-0002cae0: 662e 7365 7475 702e 5245 4749 4f4e 5f43  f.setup.REGION_C
-0002caf0: 4f4c 554d 4e5f 4e41 4d45 203d 2027 7265  OLUMN_NAME = 're
-0002cb00: 6769 6f6e 270a 2020 2020 2020 2020 7365  gion'.        se
-0002cb10: 6c66 2e73 6574 7570 2e56 4152 4941 424c  lf.setup.VARIABL
-0002cb20: 455f 434f 4c55 4d4e 5f4e 414d 4520 3d20  E_COLUMN_NAME = 
-0002cb30: 2765 6e74 6974 7927 0a20 2020 2020 2020  'entity'.       
-0002cb40: 2023 2020 2020 2020 2020 7365 6c66 2e73   #        self.s
-0002cb50: 6574 7570 2e49 4e44 4558 5f43 4f4c 554d  etup.INDEX_COLUM
-0002cb60: 4e5f 4e41 4d45 203d 205b 2746 4c4f 5727  N_NAME = ['FLOW'
-0002cb70: 2c20 2750 524f 4455 4354 275d 0a20 2020  , 'PRODUCT'].   
-0002cb80: 2020 2020 2023 2020 2020 2020 2020 7365       #        se
-0002cb90: 6c66 2e73 6574 7570 2e53 5041 5449 414c  lf.setup.SPATIAL
-0002cba0: 5f43 4f4c 554d 5f4e 414d 4520 3d20 2743  _COLUM_NAME = 'C
-0002cbb0: 4f55 4e54 5259 270a 2020 2020 2020 2020  OUNTRY'.        
-0002cbc0: 2320 2020 2020 2020 2073 656c 662e 7365  #        self.se
-0002cbd0: 7475 702e 434f 4c55 4d4e 535f 544f 5f44  tup.COLUMNS_TO_D
-0002cbe0: 524f 5020 3d20 5b20 2750 524f 4455 4354  ROP = [ 'PRODUCT
-0002cbf0: 272c 2746 4c4f 5727 2c27 636f 6d62 696e  ','FLOW','combin
-0002cc00: 6564 275d 0a0a 2020 2020 2020 2020 6966  ed']..        if
-0002cc10: 206e 6f74 2028 6f73 2e70 6174 682e 6578   not (os.path.ex
-0002cc20: 6973 7473 2873 656c 662e 7365 7475 702e  ists(self.setup.
-0002cc30: 4d41 5050 494e 475f 4649 4c45 2929 3a0a  MAPPING_FILE)):.
-0002cc40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002cc50: 2e63 7265 6174 6556 6172 6961 626c 654d  .createVariableM
-0002cc60: 6170 7069 6e67 2829 0a20 2020 2020 2020  apping().       
-0002cc70: 2020 2020 2070 7269 6e74 2822 6e6f 206d       print("no m
-0002cc80: 6170 7069 6e67 2066 696c 6520 666f 756e  apping file foun
-0002cc90: 6422 290a 2020 2020 2020 2020 656c 7365  d").        else
-0002cca0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002ccb0: 6c66 2e6d 6170 7069 6e67 203d 2064 6963  lf.mapping = dic
-0002ccc0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-0002ccd0: 666f 7220 7661 7220 696e 205b 2765 6e74  for var in ['ent
-0002cce0: 6974 7927 2c20 2773 6365 6e61 7269 6f27  ity', 'scenario'
-0002ccf0: 2c20 2772 6567 696f 6e27 5d3a 0a20 2020  , 'region']:.   
-0002cd00: 2020 2020 2020 2020 2020 2020 2064 6620               df 
-0002cd10: 3d20 7064 2e72 6561 645f 6578 6365 6c28  = pd.read_excel(
-0002cd20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002cd30: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
-0002cd40: 4d41 5050 494e 475f 4649 4c45 2c20 7368  MAPPING_FILE, sh
-0002cd50: 6565 745f 6e61 6d65 3d76 6172 202b 2027  eet_name=var + '
-0002cd60: 5f6d 6170 7069 6e67 272c 2069 6e64 6578  _mapping', index
-0002cd70: 5f63 6f6c 3d30 0a20 2020 2020 2020 2020  _col=0.         
-0002cd80: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0002cd90: 2020 2020 2020 2020 2064 6620 3d20 6466           df = df
-0002cda0: 2e6c 6f63 5b7e 6466 2e6c 6f63 5b3a 2c20  .loc[~df.loc[:, 
-0002cdb0: 7661 725d 2e69 736e 6128 295d 0a20 2020  var].isna()].   
-0002cdc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0002cdd0: 662e 6d61 7070 696e 672e 7570 6461 7465  f.mapping.update
-0002cde0: 2864 662e 746f 5f64 6963 7428 2929 0a20  (df.to_dict()). 
-0002cdf0: 2020 2020 2020 2073 656c 662e 6372 6561         self.crea
-0002ce00: 7465 536f 7572 6365 4d65 7461 2829 0a0a  teSourceMeta()..
-0002ce10: 2020 2020 6465 6620 6c6f 6164 4461 7461      def loadData
-0002ce20: 2873 656c 6629 3a0a 0a20 2020 2020 2020  (self):..       
-0002ce30: 2066 6f72 2069 2c20 6669 6c65 4b65 7920   for i, fileKey 
-0002ce40: 696e 2065 6e75 6d65 7261 7465 2873 656c  in enumerate(sel
-0002ce50: 662e 7365 7475 702e 4441 5441 5f46 494c  f.setup.DATA_FIL
-0002ce60: 452e 6b65 7973 2829 293a 0a0a 2020 2020  E.keys()):..    
-0002ce70: 2020 2020 2020 2020 6669 6c65 203d 2073          file = s
-0002ce80: 656c 662e 7365 7475 702e 4441 5441 5f46  elf.setup.DATA_F
-0002ce90: 494c 455b 6669 6c65 4b65 795d 0a20 2020  ILE[fileKey].   
-0002cea0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-0002ceb0: 696c 6529 0a20 2020 2020 2020 2020 2020  ile).           
-0002cec0: 2069 6620 6e6f 7420 6f73 2e70 6174 682e   if not os.path.
-0002ced0: 6578 6973 7473 2866 696c 6529 3a0a 2020  exists(file):.  
-0002cee0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0002cef0: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
-0002cf00: 2020 2074 656d 7020 3d20 7064 2e72 6561     temp = pd.rea
-0002cf10: 645f 6373 7628 0a20 2020 2020 2020 2020  d_csv(.         
-0002cf20: 2020 2020 2020 2066 696c 652c 2065 6e67         file, eng
-0002cf30: 696e 653d 2770 7974 686f 6e27 2c20 696e  ine='python', in
-0002cf40: 6465 785f 636f 6c3d 4e6f 6e65 2c20 6865  dex_col=None, he
-0002cf50: 6164 6572 3d30 2c20 656e 636f 6469 6e67  ader=0, encoding
-0002cf60: 3d22 4953 4f2d 3838 3539 2d31 220a 2020  ="ISO-8859-1".  
-0002cf70: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0002cf80: 2020 2020 2020 2020 7465 6d70 2e45 6c65          temp.Ele
-0002cf90: 6d65 6e74 203d 2074 656d 702e 456c 656d  ment = temp.Elem
-0002cfa0: 656e 742e 6170 706c 7928 6c61 6d62 6461  ent.apply(lambda
-0002cfb0: 2078 3a20 6669 6c65 4b65 7920 2b20 7829   x: fileKey + x)
-0002cfc0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0002cfd0: 6e6f 7420 6861 7361 7474 7228 7365 6c66  not hasattr(self
-0002cfe0: 2c20 2764 6174 6127 293a 0a20 2020 2020  , 'data'):.     
-0002cff0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002d000: 6461 7461 203d 2074 656d 700a 2020 2020  data = temp.    
-0002d010: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0002d020: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0002d030: 6c66 2e64 6174 6120 3d20 7365 6c66 2e64  lf.data = self.d
-0002d040: 6174 612e 6170 7065 6e64 2874 656d 7029  ata.append(temp)
-0002d050: 0a0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
-0002d060: 6174 612e 6c6f 635b 3a2c 2027 7265 6769  ata.loc[:, 'regi
-0002d070: 6f6e 275d 203d 2073 656c 662e 6461 7461  on'] = self.data
-0002d080: 2e41 7265 610a 2020 2020 2020 2020 7365  .Area.        se
-0002d090: 6c66 2e64 6174 612e 6c6f 635b 3a2c 2027  lf.data.loc[:, '
-0002d0a0: 656e 7469 7479 275d 203d 2073 656c 662e  entity'] = self.
-0002d0b0: 6461 7461 2e45 6c65 6d65 6e74 202b 2027  data.Element + '
-0002d0c0: 5f27 202b 2073 656c 662e 6461 7461 2e49  _' + self.data.I
-0002d0d0: 7465 6d0a 2020 2020 2020 2020 7365 6c66  tem.        self
-0002d0e0: 2e64 6174 612e 6c6f 635b 3a2c 2027 7363  .data.loc[:, 'sc
-0002d0f0: 656e 6172 696f 275d 203d 2027 4869 7374  enario'] = 'Hist
-0002d100: 6f72 6963 270a 2020 2020 2020 2020 7365  oric'.        se
-0002d110: 6c66 2e64 6174 612e 6c6f 635b 3a2c 2027  lf.data.loc[:, '
-0002d120: 6d6f 6465 6c27 5d20 3d20 2727 0a20 2020  model'] = ''.   
-0002d130: 2020 2020 2069 6e64 6578 5f6b 6565 7020       index_keep 
-0002d140: 3d20 7365 6c66 2e64 6174 612e 696e 6465  = self.data.inde
-0002d150: 785b 7365 6c66 2e64 6174 615b 2753 6f75  x[self.data['Sou
-0002d160: 7263 6527 5d20 3d3d 2027 4641 4f20 5449  rce'] == 'FAO TI
-0002d170: 4552 2031 275d 0a20 2020 2020 2020 2073  ER 1'].        s
-0002d180: 656c 662e 6461 7461 203d 2073 656c 662e  elf.data = self.
-0002d190: 6461 7461 2e6c 6f63 5b69 6e64 6578 5f6b  data.loc[index_k
-0002d1a0: 6565 705d 0a0a 2020 2020 2020 2020 6e65  eep]..        ne
-0002d1b0: 7743 6f6c 756d 6e73 203d 205b 2772 6567  wColumns = ['reg
-0002d1c0: 696f 6e27 2c20 2765 6e74 6974 7927 2c20  ion', 'entity', 
-0002d1d0: 2773 6365 6e61 7269 6f27 2c20 276d 6f64  'scenario', 'mod
-0002d1e0: 656c 272c 2027 556e 6974 275d 0a20 2020  el', 'Unit'].   
-0002d1f0: 2020 2020 2073 656c 662e 7469 6d65 436f       self.timeCo
-0002d200: 6c75 6d6e 7320 3d20 6c69 7374 2829 0a20  lumns = list(). 
-0002d210: 2020 2020 2020 2066 6f72 2063 6f6c 756d         for colum
-0002d220: 6e20 696e 2073 656c 662e 6461 7461 2e63  n in self.data.c
-0002d230: 6f6c 756d 6e73 3a0a 2020 2020 2020 2020  olumns:.        
-0002d240: 2020 2020 6966 2063 6f6c 756d 6e2e 7374      if column.st
-0002d250: 6172 7473 7769 7468 2827 5927 2920 616e  artswith('Y') an
-0002d260: 6420 6c65 6e28 636f 6c75 6d6e 2920 3d3d  d len(column) ==
-0002d270: 2035 3a0a 2020 2020 2020 2020 2020 2020   5:.            
-0002d280: 2020 2020 7365 6c66 2e64 6174 612e 6c6f      self.data.lo
-0002d290: 635b 3a2c 2069 6e74 2863 6f6c 756d 6e5b  c[:, int(column[
-0002d2a0: 313a 5d29 5d20 3d20 7365 6c66 2e64 6174  1:])] = self.dat
-0002d2b0: 612e 6c6f 635b 3a2c 2063 6f6c 756d 6e5d  a.loc[:, column]
-0002d2c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002d2d0: 206e 6577 436f 6c75 6d6e 732e 6170 7065   newColumns.appe
-0002d2e0: 6e64 2869 6e74 2863 6f6c 756d 6e5b 313a  nd(int(column[1:
-0002d2f0: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-0002d300: 2020 2020 7365 6c66 2e74 696d 6543 6f6c      self.timeCol
-0002d310: 756d 6e73 2e61 7070 656e 6428 696e 7428  umns.append(int(
-0002d320: 636f 6c75 6d6e 5b31 3a5d 2929 0a0a 2020  column[1:]))..  
-0002d330: 2020 2020 2020 7365 6c66 2e64 6174 6120        self.data 
-0002d340: 3d20 7365 6c66 2e64 6174 612e 6c6f 635b  = self.data.loc[
-0002d350: 3a2c 206e 6577 436f 6c75 6d6e 735d 0a0a  :, newColumns]..
-0002d360: 2020 2020 6465 6620 6372 6561 7465 5661      def createVa
-0002d370: 7269 6162 6c65 4d61 7070 696e 6728 7365  riableMapping(se
-0002d380: 6c66 293a 0a0a 2020 2020 2020 2020 2320  lf):..        # 
-0002d390: 6c6f 6164 696e 6720 6461 7461 2069 6620  loading data if 
-0002d3a0: 6e65 6365 7373 6172 790a 2020 2020 2020  necessary.      
-0002d3b0: 2020 6966 206e 6f74 2068 6173 6174 7472    if not hasattr
-0002d3c0: 2873 656c 662c 2027 6461 7461 2729 3a0a  (self, 'data'):.
-0002d3d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002d3e0: 2e6c 6f61 6444 6174 6128 290a 2020 2020  .loadData().    
-0002d3f0: 2020 2020 2320 2020 2020 2020 2072 6574      #        ret
-0002d400: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
-0002d410: 2020 696d 706f 7274 206e 756d 7079 2061    import numpy a
-0002d420: 7320 6e70 0a0a 2020 2020 2020 2020 7772  s np..        wr
-0002d430: 6974 6572 203d 2070 642e 4578 6365 6c57  iter = pd.ExcelW
-0002d440: 7269 7465 7228 0a20 2020 2020 2020 2020  riter(.         
-0002d450: 2020 2073 656c 662e 7365 7475 702e 4d41     self.setup.MA
-0002d460: 5050 494e 475f 4649 4c45 2c0a 2020 2020  PPING_FILE,.    
-0002d470: 2020 2020 2020 2020 656e 6769 6e65 3d27          engine='
-0002d480: 786c 7378 7772 6974 6572 272c 0a20 2020  xlsxwriter',.   
-0002d490: 2020 2020 2020 2020 2064 6174 6574 696d           datetim
-0002d4a0: 655f 666f 726d 6174 3d27 6d6d 6d20 6420  e_format='mmm d 
-0002d4b0: 7979 7979 2068 683a 6d6d 3a73 7327 2c0a  yyyy hh:mm:ss',.
-0002d4c0: 2020 2020 2020 2020 2020 2020 6461 7465              date
-0002d4d0: 5f66 6f72 6d61 743d 276d 6d6d 6d20 6464  _format='mmmm dd
-0002d4e0: 2079 7979 7927 2c0a 2020 2020 2020 2020   yyyy',.        
-0002d4f0: 290a 0a20 2020 2020 2020 2023 2076 6172  )..        # var
-0002d500: 6961 626c 6573 0a20 2020 2020 2020 2023  iables.        #
-0002d510: 2069 6e64 6578 203d 2073 656c 662e 6461   index = self.da
-0002d520: 7461 5b73 656c 662e 7365 7475 702e 5641  ta[self.setup.VA
-0002d530: 5249 4142 4c45 5f43 4f4c 554d 4e5f 4e41  RIABLE_COLUMN_NA
-0002d540: 4d45 5d2e 756e 6971 7565 2829 0a20 2020  ME].unique().   
-0002d550: 2020 2020 2073 656c 662e 6176 6169 6c61       self.availa
-0002d560: 626c 6553 6572 6965 7320 3d20 7365 6c66  bleSeries = self
-0002d570: 2e64 6174 612e 6472 6f70 5f64 7570 6c69  .data.drop_dupli
-0002d580: 6361 7465 7328 2765 6e74 6974 7927 292e  cates('entity').
-0002d590: 7365 745f 696e 6465 7828 0a20 2020 2020  set_index(.     
-0002d5a0: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
-0002d5b0: 702e 5641 5249 4142 4c45 5f43 4f4c 554d  p.VARIABLE_COLUM
-0002d5c0: 4e5f 4e41 4d45 0a20 2020 2020 2020 2029  N_NAME.        )
-0002d5d0: 5b27 556e 6974 275d 0a20 2020 2020 2020  ['Unit'].       
-0002d5e0: 2073 656c 662e 6d61 7070 696e 6720 3d20   self.mapping = 
-0002d5f0: 7064 2e44 6174 6146 7261 6d65 280a 2020  pd.DataFrame(.  
-0002d600: 2020 2020 2020 2020 2020 696e 6465 783d            index=
-0002d610: 7365 6c66 2e61 7661 696c 6162 6c65 5365  self.availableSe
-0002d620: 7269 6573 2e69 6e64 6578 2c20 636f 6c75  ries.index, colu
-0002d630: 6d6e 733d 5b73 656c 662e 7365 7475 702e  mns=[self.setup.
-0002d640: 5641 5249 4142 4c45 5f43 4f4c 554d 4e5f  VARIABLE_COLUMN_
-0002d650: 4e41 4d45 5d0a 2020 2020 2020 2020 290a  NAME].        ).
-0002d660: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
-0002d670: 7069 6e67 203d 2070 642e 636f 6e63 6174  ping = pd.concat
-0002d680: 285b 7365 6c66 2e6d 6170 7069 6e67 2c20  ([self.mapping, 
-0002d690: 7365 6c66 2e61 7661 696c 6162 6c65 5365  self.availableSe
-0002d6a0: 7269 6573 5d2c 2061 7869 733d 3129 0a20  ries], axis=1). 
-0002d6b0: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
-0002d6c0: 696e 6720 3d20 7365 6c66 2e6d 6170 7069  ing = self.mappi
-0002d6d0: 6e67 2e73 6f72 745f 696e 6465 7828 290a  ng.sort_index().
-0002d6e0: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
-0002d6f0: 7069 6e67 2e69 6e64 6578 2e6e 616d 6520  ping.index.name 
-0002d700: 3d20 276f 7269 676e 616c 270a 2020 2020  = 'orignal'.    
-0002d710: 2020 2020 7365 6c66 2e6d 6170 7069 6e67      self.mapping
-0002d720: 2e74 6f5f 6578 6365 6c28 7772 6974 6572  .to_excel(writer
-0002d730: 2c20 656e 6769 6e65 3d27 6f70 656e 7079  , engine='openpy
-0002d740: 786c 272c 2073 6865 6574 5f6e 616d 653d  xl', sheet_name=
-0002d750: 5641 525f 4d41 5050 494e 475f 5348 4545  VAR_MAPPING_SHEE
-0002d760: 5429 0a0a 2020 2020 2020 2020 2320 6d6f  T)..        # mo
-0002d770: 6465 6c73 0a20 2020 2020 2020 2023 2020  dels.        #  
-0002d780: 2020 2020 2020 696e 6465 7820 3d20 6e70        index = np
-0002d790: 2e75 6e69 7175 6528 7365 6c66 2e64 6174  .unique(self.dat
-0002d7a0: 615b 7365 6c66 2e73 6574 7570 2e4d 4f44  a[self.setup.MOD
-0002d7b0: 454c 5f43 4f4c 554d 4e5f 4e41 4d45 5d2e  EL_COLUMN_NAME].
-0002d7c0: 7661 6c75 6573 290a 2020 2020 2020 2020  values).        
-0002d7d0: 230a 2020 2020 2020 2020 2320 2020 2020  #.        #     
-0002d7e0: 2020 2073 656c 662e 6176 6169 6c61 626c     self.availabl
-0002d7f0: 6553 6572 6965 7320 3d20 7064 2e44 6174  eSeries = pd.Dat
-0002d800: 6146 7261 6d65 2869 6e64 6578 3d69 6e64  aFrame(index=ind
-0002d810: 6578 290a 2020 2020 2020 2020 2320 2020  ex).        #   
-0002d820: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
-0002d830: 6720 3d20 7064 2e44 6174 6146 7261 6d65  g = pd.DataFrame
-0002d840: 2869 6e64 6578 3d69 6e64 6578 2c20 636f  (index=index, co
-0002d850: 6c75 6d6e 7320 3d20 5b73 656c 662e 7365  lumns = [self.se
-0002d860: 7475 702e 4d4f 4445 4c5f 434f 4c55 4d4e  tup.MODEL_COLUMN
-0002d870: 5f4e 414d 455d 290a 2020 2020 2020 2020  _NAME]).        
-0002d880: 2320 2020 2020 2020 2073 656c 662e 6d61  #        self.ma
-0002d890: 7070 696e 6720 3d20 7064 2e63 6f6e 6361  pping = pd.conca
-0002d8a0: 7428 5b73 656c 662e 6d61 7070 696e 672c  t([self.mapping,
-0002d8b0: 2073 656c 662e 6176 6169 6c61 626c 6553   self.availableS
-0002d8c0: 6572 6965 735d 2c20 6178 6973 3d31 290a  eries], axis=1).
-0002d8d0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0002d8e0: 2073 656c 662e 6d61 7070 696e 6720 3d20   self.mapping = 
-0002d8f0: 7365 6c66 2e6d 6170 7069 6e67 2e73 6f72  self.mapping.sor
-0002d900: 745f 696e 6465 7828 290a 2020 2020 2020  t_index().      
-0002d910: 2020 2320 2020 2020 2020 2073 656c 662e    #        self.
-0002d920: 6d61 7070 696e 672e 696e 6465 782e 6e61  mapping.index.na
-0002d930: 6d65 203d 2027 6f72 6967 6e61 6c27 0a20  me = 'orignal'. 
-0002d940: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0002d950: 7365 6c66 2e6d 6170 7069 6e67 2e74 6f5f  self.mapping.to_
-0002d960: 6578 6365 6c28 7772 6974 6572 2c20 656e  excel(writer, en
-0002d970: 6769 6e65 3d27 6f70 656e 7079 786c 272c  gine='openpyxl',
-0002d980: 2073 6865 6574 5f6e 616d 653d 276d 6f64   sheet_name='mod
-0002d990: 656c 5f6d 6170 7069 6e67 2729 0a0a 2020  el_mapping')..  
-0002d9a0: 2020 2020 2020 2320 7363 656e 6172 696f        # scenario
-0002d9b0: 730a 2020 2020 2020 2020 696e 6465 7820  s.        index 
-0002d9c0: 3d20 6e70 2e75 6e69 7175 6528 7365 6c66  = np.unique(self
-0002d9d0: 2e64 6174 615b 7365 6c66 2e73 6574 7570  .data[self.setup
-0002d9e0: 2e53 4345 4e41 5249 4f5f 434f 4c55 4d4e  .SCENARIO_COLUMN
-0002d9f0: 5f4e 414d 455d 2e76 616c 7565 7329 0a20  _NAME].values). 
-0002da00: 2020 2020 2020 2073 656c 662e 6176 6169         self.avai
-0002da10: 6c61 626c 6553 6572 6965 7320 3d20 7064  lableSeries = pd
-0002da20: 2e44 6174 6146 7261 6d65 2869 6e64 6578  .DataFrame(index
-0002da30: 3d69 6e64 6578 290a 2020 2020 2020 2020  =index).        
-0002da40: 7365 6c66 2e6d 6170 7069 6e67 203d 2070  self.mapping = p
-0002da50: 642e 4461 7461 4672 616d 6528 0a20 2020  d.DataFrame(.   
-0002da60: 2020 2020 2020 2020 2069 6e64 6578 3d69           index=i
-0002da70: 6e64 6578 2c20 636f 6c75 6d6e 733d 5b73  ndex, columns=[s
-0002da80: 656c 662e 7365 7475 702e 5343 454e 4152  elf.setup.SCENAR
-0002da90: 494f 5f43 4f4c 554d 4e5f 4e41 4d45 5d0a  IO_COLUMN_NAME].
-0002daa0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0002dab0: 2020 7365 6c66 2e6d 6170 7069 6e67 203d    self.mapping =
-0002dac0: 2070 642e 636f 6e63 6174 285b 7365 6c66   pd.concat([self
-0002dad0: 2e6d 6170 7069 6e67 2c20 7365 6c66 2e61  .mapping, self.a
-0002dae0: 7661 696c 6162 6c65 5365 7269 6573 5d2c  vailableSeries],
-0002daf0: 2061 7869 733d 3129 0a20 2020 2020 2020   axis=1).       
-0002db00: 2073 656c 662e 6d61 7070 696e 6720 3d20   self.mapping = 
-0002db10: 7365 6c66 2e6d 6170 7069 6e67 2e73 6f72  self.mapping.sor
-0002db20: 745f 696e 6465 7828 290a 2020 2020 2020  t_index().      
-0002db30: 2020 7365 6c66 2e6d 6170 7069 6e67 2e69    self.mapping.i
-0002db40: 6e64 6578 2e6e 616d 6520 3d20 276f 7269  ndex.name = 'ori
-0002db50: 676e 616c 270a 2020 2020 2020 2020 7365  gnal'.        se
-0002db60: 6c66 2e6d 6170 7069 6e67 2e74 6f5f 6578  lf.mapping.to_ex
-0002db70: 6365 6c28 7772 6974 6572 2c20 656e 6769  cel(writer, engi
-0002db80: 6e65 3d27 6f70 656e 7079 786c 272c 2073  ne='openpyxl', s
-0002db90: 6865 6574 5f6e 616d 653d 2773 6365 6e61  heet_name='scena
-0002dba0: 7269 6f5f 6d61 7070 696e 6727 290a 0a20  rio_mapping').. 
-0002dbb0: 2020 2020 2020 2023 2072 6567 696f 6e0a         # region.
-0002dbc0: 2020 2020 2020 2020 696e 6465 7820 3d20          index = 
-0002dbd0: 6e70 2e75 6e69 7175 6528 7365 6c66 2e64  np.unique(self.d
-0002dbe0: 6174 615b 7365 6c66 2e73 6574 7570 2e52  ata[self.setup.R
-0002dbf0: 4547 494f 4e5f 434f 4c55 4d4e 5f4e 414d  EGION_COLUMN_NAM
-0002dc00: 455d 2e76 616c 7565 7329 0a20 2020 2020  E].values).     
-0002dc10: 2020 2073 656c 662e 6176 6169 6c61 626c     self.availabl
-0002dc20: 6553 6572 6965 7320 3d20 7064 2e44 6174  eSeries = pd.Dat
-0002dc30: 6146 7261 6d65 2869 6e64 6578 3d69 6e64  aFrame(index=ind
-0002dc40: 6578 290a 2020 2020 2020 2020 7365 6c66  ex).        self
-0002dc50: 2e6d 6170 7069 6e67 203d 2070 642e 4461  .mapping = pd.Da
-0002dc60: 7461 4672 616d 6528 0a20 2020 2020 2020  taFrame(.       
-0002dc70: 2020 2020 2069 6e64 6578 3d69 6e64 6578       index=index
-0002dc80: 2c20 636f 6c75 6d6e 733d 5b73 656c 662e  , columns=[self.
-0002dc90: 7365 7475 702e 5245 4749 4f4e 5f43 4f4c  setup.REGION_COL
-0002dca0: 554d 4e5f 4e41 4d45 5d0a 2020 2020 2020  UMN_NAME].      
-0002dcb0: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
-0002dcc0: 2e6d 6170 7069 6e67 203d 2070 642e 636f  .mapping = pd.co
-0002dcd0: 6e63 6174 285b 7365 6c66 2e6d 6170 7069  ncat([self.mappi
-0002dce0: 6e67 2c20 7365 6c66 2e61 7661 696c 6162  ng, self.availab
-0002dcf0: 6c65 5365 7269 6573 5d2c 2061 7869 733d  leSeries], axis=
-0002dd00: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
-0002dd10: 6d61 7070 696e 6720 3d20 7365 6c66 2e6d  mapping = self.m
-0002dd20: 6170 7069 6e67 2e73 6f72 745f 696e 6465  apping.sort_inde
-0002dd30: 7828 290a 2020 2020 2020 2020 7365 6c66  x().        self
-0002dd40: 2e6d 6170 7069 6e67 2e69 6e64 6578 2e6e  .mapping.index.n
-0002dd50: 616d 6520 3d20 276f 7269 676e 616c 270a  ame = 'orignal'.
-0002dd60: 2020 2020 2020 2020 666f 7220 6964 7820          for idx 
-0002dd70: 696e 2073 656c 662e 6d61 7070 696e 672e  in self.mapping.
-0002dd80: 696e 6465 783a 0a20 2020 2020 2020 2020  index:.         
-0002dd90: 2020 2069 736f 203d 2064 742e 7574 696c     iso = dt.util
-0002dda0: 2e69 6465 6e74 6966 7943 6f75 6e74 7279  .identifyCountry
-0002ddb0: 2869 6478 290a 2020 2020 2020 2020 2020  (idx).          
-0002ddc0: 2020 6966 2069 736f 2069 7320 6e6f 7420    if iso is not 
-0002ddd0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002dde0: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
-0002ddf0: 6e67 2e6c 6f63 5b69 6478 2c20 2772 6567  ng.loc[idx, 'reg
-0002de00: 696f 6e27 5d20 3d20 6973 6f0a 0a20 2020  ion'] = iso..   
-0002de10: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
-0002de20: 672e 746f 5f65 7863 656c 2877 7269 7465  g.to_excel(write
-0002de30: 722c 2065 6e67 696e 653d 276f 7065 6e70  r, engine='openp
-0002de40: 7978 6c27 2c20 7368 6565 745f 6e61 6d65  yxl', sheet_name
-0002de50: 3d27 7265 6769 6f6e 5f6d 6170 7069 6e67  ='region_mapping
-0002de60: 2729 0a20 2020 2020 2020 2077 7269 7465  ').        write
-0002de70: 722e 636c 6f73 6528 290a 0a20 2020 2064  r.close()..    d
-0002de80: 6566 2067 6174 6865 724d 6170 7065 6444  ef gatherMappedD
-0002de90: 6174 6128 7365 6c66 2c20 7370 6174 6961  ata(self, spatia
-0002dea0: 6c53 7562 5365 743d 4e6f 6e65 293a 0a0a  lSubSet=None):..
-0002deb0: 2020 2020 2020 2020 696d 706f 7274 2074          import t
-0002dec0: 7164 6d0a 0a20 2020 2020 2020 2023 206c  qdm..        # l
-0002ded0: 6f61 6469 6e67 2064 6174 6120 6966 206e  oading data if n
-0002dee0: 6563 6573 7361 7279 0a20 2020 2020 2020  ecessary.       
-0002def0: 2069 6620 6e6f 7420 6861 7361 7474 7228   if not hasattr(
-0002df00: 7365 6c66 2c20 2764 6174 6127 293a 0a20  self, 'data'):. 
-0002df10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002df20: 6c6f 6164 4461 7461 2829 0a0a 2020 2020  loadData()..    
-0002df30: 2020 2020 7461 626c 6573 546f 436f 6d6d      tablesToComm
-0002df40: 6974 203d 205b 5d0a 2020 2020 2020 2020  it = [].        
-0002df50: 6d65 7461 4469 6374 203d 2064 6963 7428  metaDict = dict(
-0002df60: 290a 2020 2020 2020 2020 6d65 7461 4469  ).        metaDi
-0002df70: 6374 5b27 736f 7572 6365 275d 203d 2073  ct['source'] = s
-0002df80: 656c 662e 7365 7475 702e 534f 5552 4345  elf.setup.SOURCE
-0002df90: 5f49 440a 2020 2020 2020 2020 6578 636c  _ID.        excl
-0002dfa0: 7564 6564 5461 626c 6573 203d 2064 6963  udedTables = dic
-0002dfb0: 7428 290a 2020 2020 2020 2020 6578 636c  t().        excl
-0002dfc0: 7564 6564 5461 626c 6573 5b27 656d 7074  udedTables['empt
-0002dfd0: 7927 5d20 3d20 6c69 7374 2829 0a20 2020  y'] = list().   
-0002dfe0: 2020 2020 2065 7863 6c75 6465 6454 6162       excludedTab
-0002dff0: 6c65 735b 2765 7272 6f72 275d 203d 206c  les['error'] = l
-0002e000: 6973 7428 290a 2020 2020 2020 2020 6578  ist().        ex
-0002e010: 636c 7564 6564 5461 626c 6573 5b27 6578  cludedTables['ex
-0002e020: 6973 7473 275d 203d 206c 6973 7428 290a  ists'] = list().
-0002e030: 0a20 2020 2020 2020 2066 6f72 206d 6f64  .        for mod
-0002e040: 656c 2069 6e20 5b27 275d 3a0a 2020 2020  el in ['']:.    
-0002e050: 2020 2020 2020 2020 7465 6d70 4d6f 203d          tempMo =
-0002e060: 2073 656c 662e 6461 7461 0a0a 2020 2020   self.data..    
-0002e070: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0002e080: 2020 2020 2074 656d 704d 6f20 3d20 7365       tempMo = se
-0002e090: 6c66 2e64 6174 612e 6c6f 635b 7365 6c66  lf.data.loc[self
-0002e0a0: 2e64 6174 612e 6d6f 6465 6c20 3d3d 206d  .data.model == m
-0002e0b0: 6f64 656c 5d0a 2020 2020 2020 2020 2020  odel].          
-0002e0c0: 2020 666f 7220 7363 656e 6172 696f 2069    for scenario i
-0002e0d0: 6e20 7365 6c66 2e6d 6170 7069 6e67 5b27  n self.mapping['
-0002e0e0: 7363 656e 6172 696f 275d 2e6b 6579 7328  scenario'].keys(
-0002e0f0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0002e100: 2020 2074 656d 704d 6f53 6320 3d20 7465     tempMoSc = te
-0002e110: 6d70 4d6f 2e6c 6f63 5b74 656d 704d 6f2e  mpMo.loc[tempMo.
-0002e120: 7363 656e 6172 696f 203d 3d20 7363 656e  scenario == scen
-0002e130: 6172 696f 5d0a 2020 2020 2020 2020 2020  ario].          
-0002e140: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0002e150: 2020 2020 2020 2066 6f72 2076 6172 6961         for varia
-0002e160: 626c 6520 696e 2073 656c 662e 6d61 7070  ble in self.mapp
-0002e170: 696e 675b 2776 6172 6961 626c 6527 5d2e  ing['variable'].
-0002e180: 6b65 7973 2829 3a0a 2020 2020 2020 2020  keys():.        
-0002e190: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0002e1a0: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-0002e1b0: 704d 6f53 6356 6120 3d20 7465 6d70 4d6f  pMoScVa = tempMo
-0002e1c0: 5363 2e6c 6f63 5b73 656c 662e 6461 7461  Sc.loc[self.data
-0002e1d0: 2e76 6172 6961 626c 6520 3d3d 2076 6172  .variable == var
-0002e1e0: 6961 626c 655d 0a0a 2020 2020 2020 2020  iable]..        
-0002e1f0: 2020 2020 2020 2020 666f 7220 7661 7269          for vari
-0002e200: 6162 6c65 2069 6e20 6c69 7374 2873 656c  able in list(sel
-0002e210: 662e 6d61 7070 696e 675b 2765 6e74 6974  f.mapping['entit
-0002e220: 7927 5d2e 6b65 7973 2829 293a 0a20 2020  y'].keys()):.   
-0002e230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e240: 2074 656d 704d 6f53 6356 6172 203d 2074   tempMoScVar = t
-0002e250: 656d 704d 6f53 632e 6c6f 635b 7465 6d70  empMoSc.loc[temp
-0002e260: 4d6f 5363 2e65 6e74 6974 7920 3d3d 2076  MoSc.entity == v
-0002e270: 6172 6961 626c 655d 0a20 2020 2020 2020  ariable].       
-0002e280: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-0002e290: 704d 6f53 6356 6172 2e75 6e69 7420 3d20  pMoScVar.unit = 
-0002e2a0: 7365 6c66 2e6d 6170 7069 6e67 5b27 756e  self.mapping['un
-0002e2b0: 6974 275d 5b76 6172 6961 626c 655d 0a20  it'][variable]. 
-0002e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e2d0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0002e2e0: 2020 2020 2020 2020 7461 626c 6573 203d          tables =
-0002e2f0: 2064 742e 696e 7465 7266 6163 6573 2e72   dt.interfaces.r
-0002e300: 6561 645f 6c6f 6e67 5f74 6162 6c65 2874  ead_long_table(t
-0002e310: 656d 704d 6f53 6356 6172 2c20 5b76 6172  empMoScVar, [var
-0002e320: 6961 626c 655d 290a 0a20 2020 2020 2020  iable])..       
-0002e330: 2020 2020 2020 2020 2020 2020 2074 6162               tab
-0002e340: 6c65 203d 2074 656d 704d 6f53 6356 6172  le = tempMoScVar
-0002e350: 2e6c 6f63 5b3a 2c20 7365 6c66 2e74 696d  .loc[:, self.tim
-0002e360: 6543 6f6c 756d 6e73 5d0a 0a20 2020 2020  eColumns]..     
-0002e370: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0002e380: 6162 6c65 203d 2044 6174 6174 6162 6c65  able = Datatable
-0002e390: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0002e3a0: 2020 2020 2020 2020 2020 7461 626c 652c            table,
-0002e3b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002e3c0: 2020 2020 2020 2020 206d 6574 613d 7b0a           meta={.
-0002e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e3e0: 2020 2020 2020 2020 2020 2020 2765 6e74              'ent
-0002e3f0: 6974 7927 3a20 7365 6c66 2e6d 6170 7069  ity': self.mappi
-0002e400: 6e67 5b27 656e 7469 7479 275d 5b76 6172  ng['entity'][var
-0002e410: 6961 626c 655d 2c0a 2020 2020 2020 2020  iable],.        
+0002afa0: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
+0002afb0: 6573 546f 436f 6d6d 6974 2e61 7070 656e  esToCommit.appen
+0002afc0: 6428 7461 626c 6529 0a20 2020 2020 2020  d(table).       
+0002afd0: 2072 6574 7572 6e20 7461 626c 6573 546f   return tablesTo
+0002afe0: 436f 6d6d 6974 2c20 6578 636c 7564 6564  Commit, excluded
+0002aff0: 5461 626c 6573 0a0a 0a63 6c61 7373 2041  Tables...class A
+0002b000: 5045 4328 4261 7365 496d 706f 7274 546f  PEC(BaseImportTo
+0002b010: 6f6c 293a 0a0a 2020 2020 2222 220a 2020  ol):..    """.  
+0002b020: 2020 4952 454e 4120 6461 7461 2069 6d70    IRENA data imp
+0002b030: 6f72 7420 746f 6f6c 0a20 2020 2022 2222  ort tool.    """
+0002b040: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+0002b050: 5f5f 2873 656c 662c 2079 6561 7229 3a0a  __(self, year):.
+0002b060: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0002b070: 7570 203d 2073 6574 7570 5374 7275 6374  up = setupStruct
+0002b080: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0002b090: 7365 7475 702e 534f 5552 4345 5f49 4420  setup.SOURCE_ID 
+0002b0a0: 3d20 2241 5045 435f 2220 2b20 7374 7228  = "APEC_" + str(
+0002b0b0: 7965 6172 290a 2020 2020 2020 2020 7365  year).        se
+0002b0c0: 6c66 2e73 6574 7570 2e53 4f55 5243 455f  lf.setup.SOURCE_
+0002b0d0: 5041 5448 203d 206f 732e 7061 7468 2e6a  PATH = os.path.j
+0002b0e0: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
+0002b0f0: 2063 6f6e 6669 672e 5041 5448 5f54 4f5f   config.PATH_TO_
+0002b100: 4441 5441 5348 454c 462c 2027 7261 7764  DATASHELF, 'rawd
+0002b110: 6174 612f 4150 4543 2f27 202b 2073 7472  ata/APEC/' + str
+0002b120: 2879 6561 7229 0a20 2020 2020 2020 2029  (year).        )
+0002b130: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0002b140: 7475 702e 4441 5441 5f46 494c 4520 3d20  tup.DATA_FILE = 
+0002b150: 6f73 2e70 6174 682e 6a6f 696e 280a 2020  os.path.join(.  
+0002b160: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0002b170: 6574 7570 2e53 4f55 5243 455f 5041 5448  etup.SOURCE_PATH
+0002b180: 2c20 2763 6f6d 7069 6c65 645f 7261 775f  , 'compiled_raw_
+0002b190: 686f 6573 6c79 2e63 7376 270a 2020 2020  hoesly.csv'.    
+0002b1a0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+0002b1b0: 6c66 2e73 6574 7570 2e4d 4150 5049 4e47  lf.setup.MAPPING
+0002b1c0: 5f46 494c 4520 3d20 6f73 2e70 6174 682e  _FILE = os.path.
+0002b1d0: 6a6f 696e 2873 656c 662e 7365 7475 702e  join(self.setup.
+0002b1e0: 534f 5552 4345 5f50 4154 482c 2027 6d61  SOURCE_PATH, 'ma
+0002b1f0: 7070 696e 672e 786c 7378 2729 0a20 2020  pping.xlsx').   
+0002b200: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
+0002b210: 4c49 4345 4e43 4520 3d20 2728 6329 2032  LICENCE = '(c) 2
+0002b220: 3031 3920 4173 6961 2050 6163 6966 6963  019 Asia Pacific
+0002b230: 2045 636f 6e6f 6d69 6320 436f 6f70 6572   Economic Cooper
+0002b240: 6174 696f 6e20 2841 5045 5243 2927 0a20  ation (APERC)'. 
+0002b250: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
+0002b260: 702e 5552 4c20 3d20 2768 7474 7073 3a2f  p.URL = 'https:/
+0002b270: 2f77 7777 2e61 7065 632e 6f72 672f 5075  /www.apec.org/Pu
+0002b280: 626c 6963 6174 696f 6e73 2f32 3031 392f  blications/2019/
+0002b290: 3035 2f41 5045 432d 456e 6572 6779 2d44  05/APEC-Energy-D
+0002b2a0: 656d 616e 642d 616e 642d 5375 7070 6c79  emand-and-Supply
+0002b2b0: 2d4f 7574 6c6f 6f6b 2d37 7468 2d45 6469  -Outlook-7th-Edi
+0002b2c0: 7469 6f6e 2d2d 2d56 6f6c 756d 652d 4927  tion---Volume-I'
+0002b2d0: 0a0a 2020 2020 2020 2020 2320 2020 2020  ..        #     
+0002b2e0: 2020 2073 656c 662e 7365 7475 702e 494e     self.setup.IN
+0002b2f0: 4445 585f 434f 4c55 4d4e 5f4e 414d 4520  DEX_COLUMN_NAME 
+0002b300: 3d20 5b27 464c 4f57 272c 2027 5052 4f44  = ['FLOW', 'PROD
+0002b310: 5543 5427 5d0a 2020 2020 2020 2020 2320  UCT'].        # 
+0002b320: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
+0002b330: 702e 5350 4154 4941 4c5f 434f 4c55 4d5f  p.SPATIAL_COLUM_
+0002b340: 4e41 4d45 203d 2027 434f 554e 5452 5927  NAME = 'COUNTRY'
+0002b350: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0002b360: 2020 7365 6c66 2e73 6574 7570 2e43 4f4c    self.setup.COL
+0002b370: 554d 4e53 5f54 4f5f 4452 4f50 203d 205b  UMNS_TO_DROP = [
+0002b380: 2027 5052 4f44 5543 5427 2c27 464c 4f57   'PRODUCT','FLOW
+0002b390: 272c 2763 6f6d 6269 6e65 6427 5d0a 0a20  ','combined'].. 
+0002b3a0: 2020 2020 2020 2069 6620 6e6f 7420 286f         if not (o
+0002b3b0: 732e 7061 7468 2e65 7869 7374 7328 7365  s.path.exists(se
+0002b3c0: 6c66 2e73 6574 7570 2e4d 4150 5049 4e47  lf.setup.MAPPING
+0002b3d0: 5f46 494c 4529 293a 0a20 2020 2020 2020  _FILE)):.       
+0002b3e0: 2020 2020 2023 2020 2020 2020 2020 2020       #          
+0002b3f0: 2020 7365 6c66 2e63 7265 6174 6556 6172    self.createVar
+0002b400: 6961 626c 654d 6170 7069 6e67 2829 0a20  iableMapping(). 
+0002b410: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0002b420: 2822 6e6f 206d 6170 7069 6e67 2066 696c  ("no mapping fil
+0002b430: 6520 666f 756e 6422 290a 2020 2020 2020  e found").      
+0002b440: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0002b450: 2020 2020 7365 6c66 2e6d 6170 7069 6e67      self.mapping
+0002b460: 203d 2070 642e 7265 6164 5f65 7863 656c   = pd.read_excel
+0002b470: 2873 656c 662e 7365 7475 702e 4d41 5050  (self.setup.MAPP
+0002b480: 494e 475f 4649 4c45 2c20 7368 6565 745f  ING_FILE, sheet_
+0002b490: 6e61 6d65 3d27 4150 4543 2729 0a0a 2020  name='APEC')..  
+0002b4a0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0002b4b0: 7061 7469 616c 4d61 7070 696e 6720 3d20  patialMapping = 
+0002b4c0: 7064 2e72 6561 645f 6578 6365 6c28 0a20  pd.read_excel(. 
+0002b4d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0002b4e0: 656c 662e 7365 7475 702e 4d41 5050 494e  elf.setup.MAPPIN
+0002b4f0: 475f 4649 4c45 2c20 7368 6565 745f 6e61  G_FILE, sheet_na
+0002b500: 6d65 3d27 7370 6174 6961 6c27 2c20 696e  me='spatial', in
+0002b510: 6465 785f 636f 6c3d 300a 2020 2020 2020  dex_col=0.      
+0002b520: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0002b530: 2020 2020 7365 6c66 2e73 7061 7469 616c      self.spatial
+0002b540: 4d61 7070 696e 6720 3d20 7365 6c66 2e73  Mapping = self.s
+0002b550: 7061 7469 616c 4d61 7070 696e 672e 6c6f  patialMapping.lo
+0002b560: 635b 0a20 2020 2020 2020 2020 2020 2020  c[.             
+0002b570: 2020 207e 7064 2e69 736e 756c 6c28 7365     ~pd.isnull(se
+0002b580: 6c66 2e73 7061 7469 616c 4d61 7070 696e  lf.spatialMappin
+0002b590: 672e 6d61 7070 696e 6729 0a20 2020 2020  g.mapping).     
+0002b5a0: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
+0002b5b0: 2020 7365 6c66 2e63 7265 6174 6553 6f75    self.createSou
+0002b5c0: 7263 654d 6574 6128 290a 0a20 2020 2064  rceMeta()..    d
+0002b5d0: 6566 2061 6464 5370 6174 6961 6c4d 6170  ef addSpatialMap
+0002b5e0: 7069 6e67 2873 656c 6629 3a0a 2020 2020  ping(self):.    
+0002b5f0: 2020 2020 2320 4555 0a20 2020 2020 2020      # EU.       
+0002b600: 206d 6170 7069 6e67 546f 436f 756e 7472   mappingToCountr
+0002b610: 6965 7320 3d20 6469 6374 2829 0a20 2020  ies = dict().   
+0002b620: 2020 2020 2023 2073 656c 662e 7370 6174       # self.spat
+0002b630: 6961 6c4d 6170 7069 6e67 2e6c 6f63 5b27  ialMapping.loc['
+0002b640: 4d65 6d6f 3a20 4575 726f 7065 616e 2055  Memo: European U
+0002b650: 6e69 6f6e 2d32 3827 5d20 3d20 2745 5532  nion-28'] = 'EU2
+0002b660: 3827 0a0a 2020 2020 2320 2020 2020 2020  8'..    #       
+0002b670: 206d 6170 7069 6e67 546f 436f 756e 7472   mappingToCountr
+0002b680: 6965 735b 2741 5345 414e 275d 203d 2020  ies['ASEAN'] =  
+0002b690: 5b27 564e 4d27 2c20 2750 484c 272c 2027  ['VNM', 'PHL', '
+0002b6a0: 5448 4127 2c20 2753 4750 272c 2027 4d4d  THA', 'SGP', 'MM
+0002b6b0: 5227 2c20 2749 444e 272c 2027 4b48 4d27  R', 'IDN', 'KHM'
+0002b6c0: 2c20 2742 524e 272c 2027 4d59 5327 2c20  , 'BRN', 'MYS', 
+0002b6d0: 274c 414f 275d 0a20 2020 2023 2020 2020  'LAO'].    #    
+0002b6e0: 2020 2020 6474 2e6d 6170 702e 7265 6769      dt.mapp.regi
+0002b6f0: 6f6e 732e 6164 6452 6567 696f 6e54 6f43  ons.addRegionToC
+0002b700: 6f6e 7465 7874 2827 5745 4f27 2c6d 6170  ontext('WEO',map
+0002b710: 7069 6e67 546f 436f 756e 7472 6965 7329  pingToCountries)
+0002b720: 0a0a 2020 2020 6465 6620 6761 7468 6572  ..    def gather
+0002b730: 4d61 7070 6564 4461 7461 2873 656c 662c  MappedData(self,
+0002b740: 2073 7061 7469 616c 5375 6253 6574 3d4e   spatialSubSet=N
+0002b750: 6f6e 6529 3a0a 0a20 2020 2020 2020 2074  one):..        t
+0002b760: 6162 6c65 7354 6f43 6f6d 6d69 7420 3d20  ablesToCommit = 
+0002b770: 6474 2e54 6162 6c65 5365 7428 290a 2020  dt.TableSet().  
+0002b780: 2020 2020 2020 7365 7475 7020 3d20 6469        setup = di
+0002b790: 6374 2829 0a20 2020 2020 2020 2073 6574  ct().        set
+0002b7a0: 7570 5b27 6669 6c65 5061 7468 275d 203d  up['filePath'] =
+0002b7b0: 2073 656c 662e 7365 7475 702e 534f 5552   self.setup.SOUR
+0002b7c0: 4345 5f50 4154 480a 2020 2020 2020 2020  CE_PATH.        
+0002b7d0: 7365 7475 705b 2766 696c 654e 616d 6527  setup['fileName'
+0002b7e0: 5d20 3d20 2741 5045 435f 456e 6572 6779  ] = 'APEC_Energy
+0002b7f0: 5f4f 7574 6c6f 6f6b 5f37 7468 5f45 6469  _Outlook_7th_Edi
+0002b800: 7469 6f6e 5f54 6162 6c65 732e 786c 7378  tion_Tables.xlsx
+0002b810: 270a 0a20 2020 2020 2020 2023 206c 6f6f  '..        # loo
+0002b820: 7020 6f76 6572 2065 6e65 7267 7920 6d61  p over energy ma
+0002b830: 7070 696e 670a 2020 2020 2020 2020 666f  pping.        fo
+0002b840: 7220 7265 6769 6f6e 2069 6e20 7365 6c66  r region in self
+0002b850: 2e73 7061 7469 616c 4d61 7070 696e 672e  .spatialMapping.
+0002b860: 696e 6465 783a 0a20 2020 2020 2020 2020  index:.         
+0002b870: 2020 2073 6574 7570 5b27 7368 6565 744e     setup['sheetN
+0002b880: 616d 6527 5d20 3d20 7265 6769 6f6e 0a20  ame'] = region. 
+0002b890: 2020 2020 2020 2020 2020 2073 6574 7570             setup
+0002b8a0: 5b27 7469 6d65 436f 6c49 6478 275d 203d  ['timeColIdx'] =
+0002b8b0: 205b 2741 4f3a 4130 275d 0a20 2020 2020   ['AO:A0'].     
+0002b8c0: 2020 2020 2020 2073 6574 7570 5b27 7370         setup['sp
+0002b8d0: 6163 6552 6f77 4964 7827 5d20 3d20 5b27  aceRowIdx'] = ['
+0002b8e0: 414f 3a41 3027 5d0a 0a20 2020 2020 2020  AO:A0']..       
+0002b8f0: 2020 2020 2065 7820 3d20 6474 2e69 6f2e       ex = dt.io.
+0002b900: 4578 6365 6c52 6561 6465 7228 7365 7475  ExcelReader(setu
+0002b910: 7029 0a20 2020 2020 2020 2020 2020 2063  p).            c
+0002b920: 6f49 534f 203d 2073 656c 662e 7370 6174  oISO = self.spat
+0002b930: 6961 6c4d 6170 7069 6e67 2e6c 6f63 5b72  ialMapping.loc[r
+0002b940: 6567 696f 6e2c 2027 6d61 7070 696e 6727  egion, 'mapping'
+0002b950: 5d0a 2020 2020 2020 2020 2020 2020 7072  ].            pr
+0002b960: 696e 7428 7265 6769 6f6e 2c20 6578 2e67  int(region, ex.g
+0002b970: 6174 6865 7256 616c 7565 2827 4231 2729  atherValue('B1')
+0002b980: 202b 2027 2d3e 2720 2b20 636f 4953 4f29   + '->' + coISO)
+0002b990: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+0002b9a0: 7469 6e75 650a 0a20 2020 2020 2020 2020  tinue..         
+0002b9b0: 2020 2066 6f72 2069 2c20 6964 7820 696e     for i, idx in
+0002b9c0: 2065 6e75 6d65 7261 7465 286c 6973 7428   enumerate(list(
+0002b9d0: 7365 6c66 2e6d 6170 7069 6e67 2e69 6e64  self.mapping.ind
+0002b9e0: 6578 2929 3a0a 0a20 2020 2020 2020 2020  ex)):..         
+0002b9f0: 2020 2020 2020 206d 6574 6144 6620 3d20         metaDf = 
+0002ba00: 7365 6c66 2e6d 6170 7069 6e67 2e6c 6f63  self.mapping.loc
+0002ba10: 5b69 6478 2c20 3a5d 0a20 2020 2020 2020  [idx, :].       
+0002ba20: 2020 2020 2020 2020 2023 2070 7269 6e74           # print
+0002ba30: 286d 6574 6144 665b 2757 6861 7427 5d29  (metaDf['What'])
+0002ba40: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0002ba50: 2020 2320 4361 7061 6369 7479 0a20 2020    # Capacity.   
+0002ba60: 2020 2020 2020 2020 2020 2020 2073 6574               set
+0002ba70: 7570 5b27 7469 6d65 436f 6c49 6478 275d  up['timeColIdx']
+0002ba80: 203d 2074 7570 6c65 286d 6574 6144 665b   = tuple(metaDf[
+0002ba90: 2754 696d 6527 5d2e 7370 6c69 7428 273a  'Time'].split(':
+0002baa0: 2729 290a 2020 2020 2020 2020 2020 2020  ')).            
+0002bab0: 2020 2020 7365 7475 705b 2773 7061 6365      setup['space
+0002bac0: 526f 7749 6478 275d 203d 2074 7570 6c65  RowIdx'] = tuple
+0002bad0: 285b 6d65 7461 4466 5b27 5768 6174 275d  ([metaDf['What']
+0002bae0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0002baf0: 2020 2023 2070 7269 6e74 286d 6574 6144     # print(metaD
+0002bb00: 665b 636f 6e66 6967 2e52 4551 5549 5245  f[config.REQUIRE
+0002bb10: 445f 4d45 5441 5f46 4945 4c44 535d 2e69  D_META_FIELDS].i
+0002bb20: 736e 756c 6c28 292e 616c 6c28 2920 3d3d  snull().all() ==
+0002bb30: 2046 616c 7365 290a 2020 2020 2020 2020   False).        
+0002bb40: 2020 2020 2020 2020 2320 7072 696e 7428          # print(
+0002bb50: 6d65 7461 4461 7461 5b73 656c 662e 7365  metaData[self.se
+0002bb60: 7475 702e 494e 4445 585f 434f 4c55 4d4e  tup.INDEX_COLUMN
+0002bb70: 5f4e 414d 455d 290a 0a20 2020 2020 2020  _NAME])..       
+0002bb80: 2020 2020 2020 2020 2065 782e 7469 6d65           ex.time
+0002bb90: 436f 6c49 6478 203d 205b 0a20 2020 2020  ColIdx = [.     
+0002bba0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0002bbb0: 742e 696f 2e65 7863 656c 4964 7832 5061  t.io.excelIdx2Pa
+0002bbc0: 6e64 6173 4964 7828 7829 2066 6f72 2078  ndasIdx(x) for x
+0002bbd0: 2069 6e20 7365 7475 705b 2774 696d 6543   in setup['timeC
+0002bbe0: 6f6c 4964 7827 5d0a 2020 2020 2020 2020  olIdx'].        
+0002bbf0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+0002bc00: 2020 2020 2020 2020 2020 6578 2e73 7061            ex.spa
+0002bc10: 6365 526f 7749 6478 203d 205b 0a20 2020  ceRowIdx = [.   
+0002bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bc30: 2064 742e 696f 2e65 7863 656c 4964 7832   dt.io.excelIdx2
+0002bc40: 5061 6e64 6173 4964 7828 7829 2066 6f72  PandasIdx(x) for
+0002bc50: 2078 2069 6e20 7365 7475 705b 2773 7061   x in setup['spa
+0002bc60: 6365 526f 7749 6478 275d 0a20 2020 2020  ceRowIdx'].     
+0002bc70: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+0002bc80: 2020 2020 2020 2020 2020 2020 2023 2020               #  
+0002bc90: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0002bca0: 2022 496e 7465 726e 6174 696f 6e61 6c22   "International"
+0002bcb0: 2069 6e20 6d65 7461 4466 5b27 4e61 6d65   in metaDf['Name
+0002bcc0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+0002bcd0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0002bce0: 2020 2020 2020 2020 2073 6466 0a20 2020           sdf.   
+0002bcf0: 2020 2020 2020 2020 2020 2020 2023 2020               #  
+0002bd00: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0002bd10: 2065 782e 7370 6163 6552 6f77 4964 785b   ex.spaceRowIdx[
+0002bd20: 305d 5b30 5d3e 3431 2061 6e64 2072 6567  0][0]>41 and reg
+0002bd30: 696f 6e20 213d 2027 576f 726c 6427 3a0a  ion != 'World':.
+0002bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bd50: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0002bd60: 2020 2020 2065 782e 7370 6163 6552 6f77       ex.spaceRow
+0002bd70: 4964 7820 3d20 5b28 6578 2e73 7061 6365  Idx = [(ex.space
+0002bd80: 526f 7749 6478 5b30 5d5b 305d 2d31 2c30  RowIdx[0][0]-1,0
+0002bd90: 295d 0a0a 2020 2020 2020 2020 2020 2020  )]..            
+0002bda0: 2020 2020 6466 203d 2065 782e 6761 7468      df = ex.gath
+0002bdb0: 6572 4461 7461 2829 0a20 2020 2020 2020  erData().       
+0002bdc0: 2020 2020 2020 2020 2064 662e 636f 6c75           df.colu
+0002bdd0: 6d6e 7320 3d20 6466 2e63 6f6c 756d 6e73  mns = df.columns
+0002bde0: 2e61 7374 7970 6528 696e 7429 0a20 2020  .astype(int).   
+0002bdf0: 2020 2020 2020 2020 2020 2020 206d 6574               met
+0002be00: 6144 6963 7420 3d20 6469 6374 2829 0a20  aDict = dict(). 
+0002be10: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0002be20: 6574 6144 6963 745b 2765 6e74 6974 7927  etaDict['entity'
+0002be30: 5d20 3d20 6d65 7461 4466 5b27 4e61 6d65  ] = metaDf['Name
+0002be40: 275d 2e73 7472 6970 2829 2e72 6570 6c61  '].strip().repla
+0002be50: 6365 2827 7c20 272c 2027 7c27 290a 2020  ce('| ', '|').  
+0002be60: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+0002be70: 7461 4469 6374 5b27 6361 7465 676f 7279  taDict['category
+0002be80: 275d 203d 2027 270a 2020 2020 2020 2020  '] = ''.        
+0002be90: 2020 2020 2020 2020 6d65 7461 4469 6374          metaDict
+0002bea0: 5b27 756e 6974 275d 203d 206d 6574 6144  ['unit'] = metaD
+0002beb0: 665b 2775 6e69 7427 5d0a 2020 2020 2020  f['unit'].      
+0002bec0: 2020 2020 2020 2020 2020 6d65 7461 4469            metaDi
+0002bed0: 6374 5b27 7363 656e 6172 696f 275d 203d  ct['scenario'] =
+0002bee0: 206d 6574 6144 665b 2753 6365 6e61 7269   metaDf['Scenari
+0002bef0: 6f27 5d0a 2020 2020 2020 2020 2020 2020  o'].            
+0002bf00: 2020 2020 6d65 7461 4469 6374 5b27 736f      metaDict['so
+0002bf10: 7572 6365 275d 203d 2073 656c 662e 7365  urce'] = self.se
+0002bf20: 7475 702e 534f 5552 4345 5f49 440a 2020  tup.SOURCE_ID.  
+0002bf30: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+0002bf40: 7461 4469 6374 5b27 756e 6974 546f 275d  taDict['unitTo']
+0002bf50: 203d 206d 6574 6144 665b 2775 6e69 7454   = metaDf['unitT
+0002bf60: 6f27 5d0a 2020 2020 2020 2020 2020 2020  o'].            
+0002bf70: 2020 2020 4944 203d 2064 742e 636f 7265      ID = dt.core
+0002bf80: 2e5f 6372 6561 7465 4461 7461 6261 7365  ._createDatabase
+0002bf90: 4944 286d 6574 6144 6963 7429 0a0a 2020  ID(metaDict)..  
+0002bfa0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0002bfb0: 2049 4420 6e6f 7420 696e 2074 6162 6c65   ID not in table
+0002bfc0: 7354 6f43 6f6d 6d69 742e 6b65 7973 2829  sToCommit.keys()
+0002bfd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002bfe0: 2020 2020 2020 7461 626c 6520 3d20 6474        table = dt
+0002bff0: 2e44 6174 6174 6162 6c65 2863 6f6c 756d  .Datatable(colum
+0002c000: 6e73 3d72 616e 6765 2832 3030 302c 2032  ns=range(2000, 2
+0002c010: 3130 3029 2c20 6d65 7461 3d6d 6574 6144  100), meta=metaD
+0002c020: 6963 7429 0a0a 2020 2020 2020 2020 2020  ict)..          
+0002c030: 2020 2020 2020 2020 2020 7461 626c 652e            table.
+0002c040: 6c6f 635b 636f 4953 4f2c 2064 662e 636f  loc[coISO, df.co
+0002c050: 6c75 6d6e 735d 203d 2064 662e 7661 6c75  lumns] = df.valu
+0002c060: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+0002c070: 2020 2020 2020 2074 6162 6c65 7354 6f43         tablesToC
+0002c080: 6f6d 6d69 742e 6164 6428 7461 626c 6529  ommit.add(table)
+0002c090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c0a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0002c0b0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+0002c0c0: 203d 2074 6162 6c65 7354 6f43 6f6d 6d69   = tablesToCommi
+0002c0d0: 745b 4944 5d0a 2020 2020 2020 2020 2020  t[ID].          
+0002c0e0: 2020 2020 2020 2020 2020 7461 626c 652e            table.
+0002c0f0: 6c6f 635b 636f 4953 4f2c 2064 662e 636f  loc[coISO, df.co
+0002c100: 6c75 6d6e 735d 203d 2064 662e 7661 6c75  lumns] = df.valu
+0002c110: 6573 0a0a 2020 2020 2020 2020 7461 626c  es..        tabl
+0002c120: 6573 4c69 7374 203d 206c 6973 7428 290a  esList = list().
+0002c130: 2020 2020 2020 2020 666f 7220 4944 2069          for ID i
+0002c140: 6e20 7461 626c 6573 546f 436f 6d6d 6974  n tablesToCommit
+0002c150: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
+0002c160: 2020 2020 2064 6174 6154 6162 6c65 203d       dataTable =
+0002c170: 2074 6162 6c65 7354 6f43 6f6d 6d69 745b   tablesToCommit[
+0002c180: 4944 5d0a 2020 2020 2020 2020 2020 2020  ID].            
+0002c190: 7072 696e 7428 6461 7461 5461 626c 652e  print(dataTable.
+0002c1a0: 6d65 7461 290a 2020 2020 2020 2020 2020  meta).          
+0002c1b0: 2020 6966 206e 6f74 2070 642e 6973 6e61    if not pd.isna
+0002c1c0: 2864 6174 6154 6162 6c65 2e6d 6574 615b  (dataTable.meta[
+0002c1d0: 2775 6e69 7454 6f27 5d29 3a0a 2020 2020  'unitTo']):.    
+0002c1e0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0002c1f0: 5461 626c 6520 3d20 6461 7461 5461 626c  Table = dataTabl
+0002c200: 652e 636f 6e76 6572 7428 6461 7461 5461  e.convert(dataTa
+0002c210: 626c 652e 6d65 7461 5b27 756e 6974 546f  ble.meta['unitTo
+0002c220: 275d 290a 2020 2020 2020 2020 2020 2020  ']).            
+0002c230: 2020 2020 6465 6c20 6461 7461 5461 626c      del dataTabl
+0002c240: 652e 6d65 7461 5b27 756e 6974 546f 275d  e.meta['unitTo']
+0002c250: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
+0002c260: 6c65 734c 6973 742e 6170 7065 6e64 2864  lesList.append(d
+0002c270: 6174 6154 6162 6c65 2e61 7374 7970 6528  ataTable.astype(
+0002c280: 666c 6f61 7429 290a 0a20 2020 2020 2020  float))..       
+0002c290: 2072 6574 7572 6e20 7461 626c 6573 4c69   return tablesLi
+0002c2a0: 7374 2c20 5b5d 0a0a 0a63 6c61 7373 2046  st, []...class F
+0002c2b0: 414f 2842 6173 6549 6d70 6f72 7454 6f6f  AO(BaseImportToo
+0002c2c0: 6c29 3a0a 2020 2020 2222 220a 2020 2020  l):.    """.    
+0002c2d0: 4641 4f20 6461 7461 2069 6d70 6f72 7420  FAO data import 
+0002c2e0: 746f 6f6c 0a20 2020 2022 2222 0a0a 2020  tool.    """..  
+0002c2f0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0002c300: 656c 662c 2079 6561 723d 3230 3139 2c20  elf, year=2019, 
+0002c310: 6461 7461 5f70 6174 683d 4e6f 6e65 293a  data_path=None):
+0002c320: 0a0a 2020 2020 2020 2020 6966 2064 6174  ..        if dat
+0002c330: 615f 7061 7468 2069 7320 4e6f 6e65 3a0a  a_path is None:.
+0002c340: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0002c350: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
+0002c360: 6a6f 696e 2863 6f6e 6669 672e 5041 5448  join(config.PATH
+0002c370: 5f54 4f5f 4441 5441 5348 454c 462c 2027  _TO_DATASHELF, '
+0002c380: 7261 7764 6174 6127 290a 0a20 2020 2020  rawdata')..     
+0002c390: 2020 2073 656c 662e 7365 7475 7020 3d20     self.setup = 
+0002c3a0: 7365 7475 7053 7472 7563 7428 290a 2020  setupStruct().  
+0002c3b0: 2020 2020 2020 7365 6c66 2e73 6574 7570        self.setup
+0002c3c0: 2e53 4f55 5243 455f 4944 203d 2022 4641  .SOURCE_ID = "FA
+0002c3d0: 4f5f 2220 2b20 7374 7228 7965 6172 290a  O_" + str(year).
+0002c3e0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0002c3f0: 7570 2e53 4f55 5243 455f 5041 5448 203d  up.SOURCE_PATH =
+0002c400: 206f 732e 7061 7468 2e6a 6f69 6e28 6461   os.path.join(da
+0002c410: 7461 5f70 6174 682c 2027 4641 4f5f 2720  ta_path, 'FAO_' 
+0002c420: 2b20 7374 7228 7965 6172 2929 0a20 2020  + str(year)).   
+0002c430: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
+0002c440: 4441 5441 5f46 494c 4520 3d20 7b0a 2020  DATA_FILE = {.  
+0002c450: 2020 2020 2020 2020 2020 2745 6d69 7373            'Emiss
+0002c460: 696f 6e73 5f4c 616e 645f 5573 655f 273a  ions_Land_Use_':
+0002c470: 206f 732e 7061 7468 2e6a 6f69 6e28 0a20   os.path.join(. 
+0002c480: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0002c490: 656c 662e 7365 7475 702e 534f 5552 4345  elf.setup.SOURCE
+0002c4a0: 5f50 4154 482c 0a20 2020 2020 2020 2020  _PATH,.         
+0002c4b0: 2020 2020 2020 2027 456d 6973 7369 6f6e         'Emission
+0002c4c0: 735f 4c61 6e64 5f55 7365 5f4c 616e 645f  s_Land_Use_Land_
+0002c4d0: 5573 655f 546f 7461 6c5f 455f 416c 6c5f  Use_Total_E_All_
+0002c4e0: 4461 7461 2e63 7376 272c 0a20 2020 2020  Data.csv',.     
+0002c4f0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+0002c500: 2020 2020 2020 2745 6d69 7373 696f 6e73        'Emissions
+0002c510: 5f41 6772 6963 756c 7475 7265 5f27 3a20  _Agriculture_': 
+0002c520: 6f73 2e70 6174 682e 6a6f 696e 280a 2020  os.path.join(.  
+0002c530: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0002c540: 6c66 2e73 6574 7570 2e53 4f55 5243 455f  lf.setup.SOURCE_
+0002c550: 5041 5448 2c0a 2020 2020 2020 2020 2020  PATH,.          
+0002c560: 2020 2020 2020 2745 6d69 7373 696f 6e73        'Emissions
+0002c570: 5f41 6772 6963 756c 7475 7265 5f41 6772  _Agriculture_Agr
+0002c580: 6963 756c 7475 7265 5f74 6f74 616c 5f45  iculture_total_E
+0002c590: 5f41 6c6c 5f44 6174 612e 6373 7627 2c0a  _All_Data.csv',.
+0002c5a0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+0002c5b0: 2020 2020 2020 2020 2020 2027 456e 7669             'Envi
+0002c5c0: 726f 6e6d 656e 745f 456d 6973 7369 6f6e  ronment_Emission
+0002c5d0: 735f 6279 5f53 6563 746f 725f 273a 206f  s_by_Sector_': o
+0002c5e0: 732e 7061 7468 2e6a 6f69 6e28 0a20 2020  s.path.join(.   
+0002c5f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0002c600: 662e 7365 7475 702e 534f 5552 4345 5f50  f.setup.SOURCE_P
+0002c610: 4154 482c 2027 456e 7669 726f 6e6d 656e  ATH, 'Environmen
+0002c620: 745f 456d 6973 7369 6f6e 735f 6279 5f53  t_Emissions_by_S
+0002c630: 6563 746f 725f 455f 416c 6c5f 4461 7461  ector_E_All_Data
+0002c640: 2e63 7376 270a 2020 2020 2020 2020 2020  .csv'.          
+0002c650: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+0002c660: 2027 456e 7669 726f 6e6d 656e 745f 456d   'Environment_Em
+0002c670: 6973 7369 6f6e 735f 696e 7465 6e73 6974  issions_intensit
+0002c680: 6965 735f 273a 206f 732e 7061 7468 2e6a  ies_': os.path.j
+0002c690: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
+0002c6a0: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
+0002c6b0: 534f 5552 4345 5f50 4154 482c 0a20 2020  SOURCE_PATH,.   
+0002c6c0: 2020 2020 2020 2020 2020 2020 2027 456e               'En
+0002c6d0: 7669 726f 6e6d 656e 745f 456d 6973 7369  vironment_Emissi
+0002c6e0: 6f6e 735f 696e 7465 6e73 6974 6965 735f  ons_intensities_
+0002c6f0: 455f 416c 6c5f 4461 7461 2e63 7376 272c  E_All_Data.csv',
+0002c700: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
+0002c710: 2020 2020 2020 2020 2020 2020 2745 6e76              'Env
+0002c720: 6972 6f6e 6d65 6e74 5f4c 616e 6443 6f76  ironment_LandCov
+0002c730: 6572 5f27 3a20 6f73 2e70 6174 682e 6a6f  er_': os.path.jo
+0002c740: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
+0002c750: 2020 2020 7365 6c66 2e73 6574 7570 2e53      self.setup.S
+0002c760: 4f55 5243 455f 5041 5448 2c20 2745 6e76  OURCE_PATH, 'Env
+0002c770: 6972 6f6e 6d65 6e74 5f4c 616e 6443 6f76  ironment_LandCov
+0002c780: 6572 5f45 5f41 6c6c 5f44 6174 612e 6373  er_E_All_Data.cs
+0002c790: 7627 0a20 2020 2020 2020 2020 2020 2029  v'.            )
+0002c7a0: 2c0a 2020 2020 2020 2020 2020 2020 2745  ,.            'E
+0002c7b0: 6e76 6972 6f6e 6d65 6e74 5f4c 616e 6455  nvironment_LandU
+0002c7c0: 7365 5f27 3a20 6f73 2e70 6174 682e 6a6f  se_': os.path.jo
+0002c7d0: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
+0002c7e0: 2020 2020 7365 6c66 2e73 6574 7570 2e53      self.setup.S
+0002c7f0: 4f55 5243 455f 5041 5448 2c20 2745 6e76  OURCE_PATH, 'Env
+0002c800: 6972 6f6e 6d65 6e74 5f4c 616e 6455 7365  ironment_LandUse
+0002c810: 5f45 5f41 6c6c 5f44 6174 612e 6373 7627  _E_All_Data.csv'
+0002c820: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
+0002c830: 2020 2020 2020 2020 2020 2020 2749 6e70              'Inp
+0002c840: 7574 735f 4c61 6e64 5573 655f 273a 206f  uts_LandUse_': o
+0002c850: 732e 7061 7468 2e6a 6f69 6e28 0a20 2020  s.path.join(.   
+0002c860: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0002c870: 662e 7365 7475 702e 534f 5552 4345 5f50  f.setup.SOURCE_P
+0002c880: 4154 482c 2027 496e 7075 7473 5f4c 616e  ATH, 'Inputs_Lan
+0002c890: 6455 7365 5f45 5f41 6c6c 5f44 6174 612e  dUse_E_All_Data.
+0002c8a0: 6373 7627 0a20 2020 2020 2020 2020 2020  csv'.           
+0002c8b0: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+0002c8c0: 2745 6d69 7373 696f 6e73 5f54 6f74 616c  'Emissions_Total
+0002c8d0: 273a 206f 732e 7061 7468 2e6a 6f69 6e28  ': os.path.join(
+0002c8e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c8f0: 2073 656c 662e 7365 7475 702e 534f 5552   self.setup.SOUR
+0002c900: 4345 5f50 4154 482c 2027 456d 6973 7369  CE_PATH, 'Emissi
+0002c910: 6f6e 735f 546f 7461 6c73 5f45 5f41 6c6c  ons_Totals_E_All
+0002c920: 5f44 6174 612e 6373 7627 0a20 2020 2020  _Data.csv'.     
+0002c930: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+0002c940: 2020 7d0a 0a20 2020 2020 2020 2073 656c    }..        sel
+0002c950: 662e 7365 7475 702e 4d41 5050 494e 475f  f.setup.MAPPING_
+0002c960: 4649 4c45 203d 206f 732e 7061 7468 2e6a  FILE = os.path.j
+0002c970: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
+0002c980: 2073 656c 662e 7365 7475 702e 534f 5552   self.setup.SOUR
+0002c990: 4345 5f50 4154 482c 2027 6d61 7070 696e  CE_PATH, 'mappin
+0002c9a0: 675f 3230 3232 2e78 6c73 7827 0a20 2020  g_2022.xlsx'.   
+0002c9b0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+0002c9c0: 656c 662e 7365 7475 702e 4c49 4345 4e43  elf.setup.LICENC
+0002c9d0: 4520 3d20 280a 2020 2020 2020 2020 2020  E = (.          
+0002c9e0: 2020 2746 6f6f 6420 616e 6420 4167 7269    'Food and Agri
+0002c9f0: 6375 6c74 7572 6520 4f72 6761 6e69 7a61  culture Organiza
+0002ca00: 7469 6f6e 206f 6620 7468 6520 556e 6974  tion of the Unit
+0002ca10: 6564 204e 6174 696f 6e73 2028 4641 4f29  ed Nations (FAO)
+0002ca20: 270a 2020 2020 2020 2020 290a 2020 2020  '.        ).    
+0002ca30: 2020 2020 7365 6c66 2e73 6574 7570 2e55      self.setup.U
+0002ca40: 524c 203d 2027 6874 7470 3a2f 2f77 7777  RL = 'http://www
+0002ca50: 2e66 616f 2e6f 7267 2f66 616f 7374 6174  .fao.org/faostat
+0002ca60: 2f65 6e2f 2364 6174 612f 474c 270a 2020  /en/#data/GL'.  
+0002ca70: 2020 2020 2020 2320 2020 2020 2020 2073        #        s
+0002ca80: 656c 662e 7365 7475 702e 4d4f 4445 4c5f  elf.setup.MODEL_
+0002ca90: 434f 4c55 4d4e 5f4e 414d 4520 3d20 276d  COLUMN_NAME = 'm
+0002caa0: 6f64 656c 270a 2020 2020 2020 2020 7365  odel'.        se
+0002cab0: 6c66 2e73 6574 7570 2e53 4345 4e41 5249  lf.setup.SCENARI
+0002cac0: 4f5f 434f 4c55 4d4e 5f4e 414d 4520 3d20  O_COLUMN_NAME = 
+0002cad0: 2773 6365 6e61 7269 6f27 0a20 2020 2020  'scenario'.     
+0002cae0: 2020 2073 656c 662e 7365 7475 702e 5245     self.setup.RE
+0002caf0: 4749 4f4e 5f43 4f4c 554d 4e5f 4e41 4d45  GION_COLUMN_NAME
+0002cb00: 203d 2027 7265 6769 6f6e 270a 2020 2020   = 'region'.    
+0002cb10: 2020 2020 7365 6c66 2e73 6574 7570 2e56      self.setup.V
+0002cb20: 4152 4941 424c 455f 434f 4c55 4d4e 5f4e  ARIABLE_COLUMN_N
+0002cb30: 414d 4520 3d20 2765 6e74 6974 7927 0a20  AME = 'entity'. 
+0002cb40: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0002cb50: 7365 6c66 2e73 6574 7570 2e49 4e44 4558  self.setup.INDEX
+0002cb60: 5f43 4f4c 554d 4e5f 4e41 4d45 203d 205b  _COLUMN_NAME = [
+0002cb70: 2746 4c4f 5727 2c20 2750 524f 4455 4354  'FLOW', 'PRODUCT
+0002cb80: 275d 0a20 2020 2020 2020 2023 2020 2020  '].        #    
+0002cb90: 2020 2020 7365 6c66 2e73 6574 7570 2e53      self.setup.S
+0002cba0: 5041 5449 414c 5f43 4f4c 554d 5f4e 414d  PATIAL_COLUM_NAM
+0002cbb0: 4520 3d20 2743 4f55 4e54 5259 270a 2020  E = 'COUNTRY'.  
+0002cbc0: 2020 2020 2020 2320 2020 2020 2020 2073        #        s
+0002cbd0: 656c 662e 7365 7475 702e 434f 4c55 4d4e  elf.setup.COLUMN
+0002cbe0: 535f 544f 5f44 524f 5020 3d20 5b20 2750  S_TO_DROP = [ 'P
+0002cbf0: 524f 4455 4354 272c 2746 4c4f 5727 2c27  RODUCT','FLOW','
+0002cc00: 636f 6d62 696e 6564 275d 0a0a 2020 2020  combined']..    
+0002cc10: 2020 2020 6966 206e 6f74 2028 6f73 2e70      if not (os.p
+0002cc20: 6174 682e 6578 6973 7473 2873 656c 662e  ath.exists(self.
+0002cc30: 7365 7475 702e 4d41 5050 494e 475f 4649  setup.MAPPING_FI
+0002cc40: 4c45 2929 3a0a 2020 2020 2020 2020 2020  LE)):.          
+0002cc50: 2020 7365 6c66 2e63 7265 6174 6556 6172    self.createVar
+0002cc60: 6961 626c 654d 6170 7069 6e67 2829 0a20  iableMapping(). 
+0002cc70: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0002cc80: 2822 6e6f 206d 6170 7069 6e67 2066 696c  ("no mapping fil
+0002cc90: 6520 666f 756e 6422 290a 2020 2020 2020  e found").      
+0002cca0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0002ccb0: 2020 2020 7365 6c66 2e6d 6170 7069 6e67      self.mapping
+0002ccc0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+0002ccd0: 2020 2020 2020 666f 7220 7661 7220 696e        for var in
+0002cce0: 205b 2765 6e74 6974 7927 2c20 2773 6365   ['entity', 'sce
+0002ccf0: 6e61 7269 6f27 2c20 2772 6567 696f 6e27  nario', 'region'
+0002cd00: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+0002cd10: 2020 2064 6620 3d20 7064 2e72 6561 645f     df = pd.read_
+0002cd20: 6578 6365 6c28 0a20 2020 2020 2020 2020  excel(.         
+0002cd30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002cd40: 7365 7475 702e 4d41 5050 494e 475f 4649  setup.MAPPING_FI
+0002cd50: 4c45 2c20 7368 6565 745f 6e61 6d65 3d76  LE, sheet_name=v
+0002cd60: 6172 202b 2027 5f6d 6170 7069 6e67 272c  ar + '_mapping',
+0002cd70: 2069 6e64 6578 5f63 6f6c 3d30 0a20 2020   index_col=0.   
+0002cd80: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0002cd90: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0002cda0: 6620 3d20 6466 2e6c 6f63 5b7e 6466 2e6c  f = df.loc[~df.l
+0002cdb0: 6f63 5b3a 2c20 7661 725d 2e69 736e 6128  oc[:, var].isna(
+0002cdc0: 295d 0a20 2020 2020 2020 2020 2020 2020  )].             
+0002cdd0: 2020 2073 656c 662e 6d61 7070 696e 672e     self.mapping.
+0002cde0: 7570 6461 7465 2864 662e 746f 5f64 6963  update(df.to_dic
+0002cdf0: 7428 2929 0a20 2020 2020 2020 2073 656c  t()).        sel
+0002ce00: 662e 6372 6561 7465 536f 7572 6365 4d65  f.createSourceMe
+0002ce10: 7461 2829 0a0a 2020 2020 6465 6620 6c6f  ta()..    def lo
+0002ce20: 6164 4461 7461 2873 656c 6629 3a0a 0a20  adData(self):.. 
+0002ce30: 2020 2020 2020 2066 6f72 2069 2c20 6669         for i, fi
+0002ce40: 6c65 4b65 7920 696e 2065 6e75 6d65 7261  leKey in enumera
+0002ce50: 7465 2873 656c 662e 7365 7475 702e 4441  te(self.setup.DA
+0002ce60: 5441 5f46 494c 452e 6b65 7973 2829 293a  TA_FILE.keys()):
+0002ce70: 0a0a 2020 2020 2020 2020 2020 2020 6669  ..            fi
+0002ce80: 6c65 203d 2073 656c 662e 7365 7475 702e  le = self.setup.
+0002ce90: 4441 5441 5f46 494c 455b 6669 6c65 4b65  DATA_FILE[fileKe
+0002cea0: 795d 0a20 2020 2020 2020 2020 2020 2070  y].            p
+0002ceb0: 7269 6e74 2866 696c 6529 0a20 2020 2020  rint(file).     
+0002cec0: 2020 2020 2020 2069 6620 6e6f 7420 6f73         if not os
+0002ced0: 2e70 6174 682e 6578 6973 7473 2866 696c  .path.exists(fil
+0002cee0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+0002cef0: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+0002cf00: 2020 2020 2020 2020 2074 656d 7020 3d20           temp = 
+0002cf10: 7064 2e72 6561 645f 6373 7628 0a20 2020  pd.read_csv(.   
+0002cf20: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+0002cf30: 652c 2065 6e67 696e 653d 2770 7974 686f  e, engine='pytho
+0002cf40: 6e27 2c20 696e 6465 785f 636f 6c3d 4e6f  n', index_col=No
+0002cf50: 6e65 2c20 6865 6164 6572 3d30 2c20 656e  ne, header=0, en
+0002cf60: 636f 6469 6e67 3d22 4953 4f2d 3838 3539  coding="ISO-8859
+0002cf70: 2d31 220a 2020 2020 2020 2020 2020 2020  -1".            
+0002cf80: 290a 2020 2020 2020 2020 2020 2020 7465  ).            te
+0002cf90: 6d70 2e45 6c65 6d65 6e74 203d 2074 656d  mp.Element = tem
+0002cfa0: 702e 456c 656d 656e 742e 6170 706c 7928  p.Element.apply(
+0002cfb0: 6c61 6d62 6461 2078 3a20 6669 6c65 4b65  lambda x: fileKe
+0002cfc0: 7920 2b20 7829 0a20 2020 2020 2020 2020  y + x).         
+0002cfd0: 2020 2069 6620 6e6f 7420 6861 7361 7474     if not hasatt
+0002cfe0: 7228 7365 6c66 2c20 2764 6174 6127 293a  r(self, 'data'):
+0002cff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002d000: 2073 656c 662e 6461 7461 203d 2074 656d   self.data = tem
+0002d010: 700a 2020 2020 2020 2020 2020 2020 656c  p.            el
+0002d020: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0002d030: 2020 2020 7365 6c66 2e64 6174 6120 3d20      self.data = 
+0002d040: 7365 6c66 2e64 6174 612e 6170 7065 6e64  self.data.append
+0002d050: 2874 656d 7029 0a0a 2020 2020 2020 2020  (temp)..        
+0002d060: 7365 6c66 2e64 6174 612e 6c6f 635b 3a2c  self.data.loc[:,
+0002d070: 2027 7265 6769 6f6e 275d 203d 2073 656c   'region'] = sel
+0002d080: 662e 6461 7461 2e41 7265 610a 2020 2020  f.data.Area.    
+0002d090: 2020 2020 7365 6c66 2e64 6174 612e 6c6f      self.data.lo
+0002d0a0: 635b 3a2c 2027 656e 7469 7479 275d 203d  c[:, 'entity'] =
+0002d0b0: 2073 656c 662e 6461 7461 2e45 6c65 6d65   self.data.Eleme
+0002d0c0: 6e74 202b 2027 5f27 202b 2073 656c 662e  nt + '_' + self.
+0002d0d0: 6461 7461 2e49 7465 6d0a 2020 2020 2020  data.Item.      
+0002d0e0: 2020 7365 6c66 2e64 6174 612e 6c6f 635b    self.data.loc[
+0002d0f0: 3a2c 2027 7363 656e 6172 696f 275d 203d  :, 'scenario'] =
+0002d100: 2027 4869 7374 6f72 6963 270a 2020 2020   'Historic'.    
+0002d110: 2020 2020 7365 6c66 2e64 6174 612e 6c6f      self.data.lo
+0002d120: 635b 3a2c 2027 6d6f 6465 6c27 5d20 3d20  c[:, 'model'] = 
+0002d130: 2727 0a20 2020 2020 2020 2069 6e64 6578  ''.        index
+0002d140: 5f6b 6565 7020 3d20 7365 6c66 2e64 6174  _keep = self.dat
+0002d150: 612e 696e 6465 785b 7365 6c66 2e64 6174  a.index[self.dat
+0002d160: 615b 2753 6f75 7263 6527 5d20 3d3d 2027  a['Source'] == '
+0002d170: 4641 4f20 5449 4552 2031 275d 0a20 2020  FAO TIER 1'].   
+0002d180: 2020 2020 2073 656c 662e 6461 7461 203d       self.data =
+0002d190: 2073 656c 662e 6461 7461 2e6c 6f63 5b69   self.data.loc[i
+0002d1a0: 6e64 6578 5f6b 6565 705d 0a0a 2020 2020  ndex_keep]..    
+0002d1b0: 2020 2020 6e65 7743 6f6c 756d 6e73 203d      newColumns =
+0002d1c0: 205b 2772 6567 696f 6e27 2c20 2765 6e74   ['region', 'ent
+0002d1d0: 6974 7927 2c20 2773 6365 6e61 7269 6f27  ity', 'scenario'
+0002d1e0: 2c20 276d 6f64 656c 272c 2027 556e 6974  , 'model', 'Unit
+0002d1f0: 275d 0a20 2020 2020 2020 2073 656c 662e  '].        self.
+0002d200: 7469 6d65 436f 6c75 6d6e 7320 3d20 6c69  timeColumns = li
+0002d210: 7374 2829 0a20 2020 2020 2020 2066 6f72  st().        for
+0002d220: 2063 6f6c 756d 6e20 696e 2073 656c 662e   column in self.
+0002d230: 6461 7461 2e63 6f6c 756d 6e73 3a0a 2020  data.columns:.  
+0002d240: 2020 2020 2020 2020 2020 6966 2063 6f6c            if col
+0002d250: 756d 6e2e 7374 6172 7473 7769 7468 2827  umn.startswith('
+0002d260: 5927 2920 616e 6420 6c65 6e28 636f 6c75  Y') and len(colu
+0002d270: 6d6e 2920 3d3d 2035 3a0a 2020 2020 2020  mn) == 5:.      
+0002d280: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+0002d290: 6174 612e 6c6f 635b 3a2c 2069 6e74 2863  ata.loc[:, int(c
+0002d2a0: 6f6c 756d 6e5b 313a 5d29 5d20 3d20 7365  olumn[1:])] = se
+0002d2b0: 6c66 2e64 6174 612e 6c6f 635b 3a2c 2063  lf.data.loc[:, c
+0002d2c0: 6f6c 756d 6e5d 0a20 2020 2020 2020 2020  olumn].         
+0002d2d0: 2020 2020 2020 206e 6577 436f 6c75 6d6e         newColumn
+0002d2e0: 732e 6170 7065 6e64 2869 6e74 2863 6f6c  s.append(int(col
+0002d2f0: 756d 6e5b 313a 5d29 290a 2020 2020 2020  umn[1:])).      
+0002d300: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0002d310: 696d 6543 6f6c 756d 6e73 2e61 7070 656e  imeColumns.appen
+0002d320: 6428 696e 7428 636f 6c75 6d6e 5b31 3a5d  d(int(column[1:]
+0002d330: 2929 0a0a 2020 2020 2020 2020 7365 6c66  ))..        self
+0002d340: 2e64 6174 6120 3d20 7365 6c66 2e64 6174  .data = self.dat
+0002d350: 612e 6c6f 635b 3a2c 206e 6577 436f 6c75  a.loc[:, newColu
+0002d360: 6d6e 735d 0a0a 2020 2020 6465 6620 6372  mns]..    def cr
+0002d370: 6561 7465 5661 7269 6162 6c65 4d61 7070  eateVariableMapp
+0002d380: 696e 6728 7365 6c66 293a 0a0a 2020 2020  ing(self):..    
+0002d390: 2020 2020 2320 6c6f 6164 696e 6720 6461      # loading da
+0002d3a0: 7461 2069 6620 6e65 6365 7373 6172 790a  ta if necessary.
+0002d3b0: 2020 2020 2020 2020 6966 206e 6f74 2068          if not h
+0002d3c0: 6173 6174 7472 2873 656c 662c 2027 6461  asattr(self, 'da
+0002d3d0: 7461 2729 3a0a 2020 2020 2020 2020 2020  ta'):.          
+0002d3e0: 2020 7365 6c66 2e6c 6f61 6444 6174 6128    self.loadData(
+0002d3f0: 290a 2020 2020 2020 2020 2320 2020 2020  ).        #     
+0002d400: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+0002d410: 2020 2020 2020 2020 696d 706f 7274 206e          import n
+0002d420: 756d 7079 2061 7320 6e70 0a0a 2020 2020  umpy as np..    
+0002d430: 2020 2020 7772 6974 6572 203d 2070 642e      writer = pd.
+0002d440: 4578 6365 6c57 7269 7465 7228 0a20 2020  ExcelWriter(.   
+0002d450: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0002d460: 7475 702e 4d41 5050 494e 475f 4649 4c45  tup.MAPPING_FILE
+0002d470: 2c0a 2020 2020 2020 2020 2020 2020 656e  ,.            en
+0002d480: 6769 6e65 3d27 786c 7378 7772 6974 6572  gine='xlsxwriter
+0002d490: 272c 0a20 2020 2020 2020 2020 2020 2064  ',.            d
+0002d4a0: 6174 6574 696d 655f 666f 726d 6174 3d27  atetime_format='
+0002d4b0: 6d6d 6d20 6420 7979 7979 2068 683a 6d6d  mmm d yyyy hh:mm
+0002d4c0: 3a73 7327 2c0a 2020 2020 2020 2020 2020  :ss',.          
+0002d4d0: 2020 6461 7465 5f66 6f72 6d61 743d 276d    date_format='m
+0002d4e0: 6d6d 6d20 6464 2079 7979 7927 2c0a 2020  mmm dd yyyy',.  
+0002d4f0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0002d500: 2023 2076 6172 6961 626c 6573 0a20 2020   # variables.   
+0002d510: 2020 2020 2023 2069 6e64 6578 203d 2073       # index = s
+0002d520: 656c 662e 6461 7461 5b73 656c 662e 7365  elf.data[self.se
+0002d530: 7475 702e 5641 5249 4142 4c45 5f43 4f4c  tup.VARIABLE_COL
+0002d540: 554d 4e5f 4e41 4d45 5d2e 756e 6971 7565  UMN_NAME].unique
+0002d550: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0002d560: 6176 6169 6c61 626c 6553 6572 6965 7320  availableSeries 
+0002d570: 3d20 7365 6c66 2e64 6174 612e 6472 6f70  = self.data.drop
+0002d580: 5f64 7570 6c69 6361 7465 7328 2765 6e74  _duplicates('ent
+0002d590: 6974 7927 292e 7365 745f 696e 6465 7828  ity').set_index(
+0002d5a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002d5b0: 662e 7365 7475 702e 5641 5249 4142 4c45  f.setup.VARIABLE
+0002d5c0: 5f43 4f4c 554d 4e5f 4e41 4d45 0a20 2020  _COLUMN_NAME.   
+0002d5d0: 2020 2020 2029 5b27 556e 6974 275d 0a20       )['Unit']. 
+0002d5e0: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
+0002d5f0: 696e 6720 3d20 7064 2e44 6174 6146 7261  ing = pd.DataFra
+0002d600: 6d65 280a 2020 2020 2020 2020 2020 2020  me(.            
+0002d610: 696e 6465 783d 7365 6c66 2e61 7661 696c  index=self.avail
+0002d620: 6162 6c65 5365 7269 6573 2e69 6e64 6578  ableSeries.index
+0002d630: 2c20 636f 6c75 6d6e 733d 5b73 656c 662e  , columns=[self.
+0002d640: 7365 7475 702e 5641 5249 4142 4c45 5f43  setup.VARIABLE_C
+0002d650: 4f4c 554d 4e5f 4e41 4d45 5d0a 2020 2020  OLUMN_NAME].    
+0002d660: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+0002d670: 6c66 2e6d 6170 7069 6e67 203d 2070 642e  lf.mapping = pd.
+0002d680: 636f 6e63 6174 285b 7365 6c66 2e6d 6170  concat([self.map
+0002d690: 7069 6e67 2c20 7365 6c66 2e61 7661 696c  ping, self.avail
+0002d6a0: 6162 6c65 5365 7269 6573 5d2c 2061 7869  ableSeries], axi
+0002d6b0: 733d 3129 0a20 2020 2020 2020 2073 656c  s=1).        sel
+0002d6c0: 662e 6d61 7070 696e 6720 3d20 7365 6c66  f.mapping = self
+0002d6d0: 2e6d 6170 7069 6e67 2e73 6f72 745f 696e  .mapping.sort_in
+0002d6e0: 6465 7828 290a 2020 2020 2020 2020 7365  dex().        se
+0002d6f0: 6c66 2e6d 6170 7069 6e67 2e69 6e64 6578  lf.mapping.index
+0002d700: 2e6e 616d 6520 3d20 276f 7269 676e 616c  .name = 'orignal
+0002d710: 270a 2020 2020 2020 2020 7365 6c66 2e6d  '.        self.m
+0002d720: 6170 7069 6e67 2e74 6f5f 6578 6365 6c28  apping.to_excel(
+0002d730: 7772 6974 6572 2c20 656e 6769 6e65 3d27  writer, engine='
+0002d740: 6f70 656e 7079 786c 272c 2073 6865 6574  openpyxl', sheet
+0002d750: 5f6e 616d 653d 5641 525f 4d41 5050 494e  _name=VAR_MAPPIN
+0002d760: 475f 5348 4545 5429 0a0a 2020 2020 2020  G_SHEET)..      
+0002d770: 2020 2320 6d6f 6465 6c73 0a20 2020 2020    # models.     
+0002d780: 2020 2023 2020 2020 2020 2020 696e 6465     #        inde
+0002d790: 7820 3d20 6e70 2e75 6e69 7175 6528 7365  x = np.unique(se
+0002d7a0: 6c66 2e64 6174 615b 7365 6c66 2e73 6574  lf.data[self.set
+0002d7b0: 7570 2e4d 4f44 454c 5f43 4f4c 554d 4e5f  up.MODEL_COLUMN_
+0002d7c0: 4e41 4d45 5d2e 7661 6c75 6573 290a 2020  NAME].values).  
+0002d7d0: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
+0002d7e0: 2320 2020 2020 2020 2073 656c 662e 6176  #        self.av
+0002d7f0: 6169 6c61 626c 6553 6572 6965 7320 3d20  ailableSeries = 
+0002d800: 7064 2e44 6174 6146 7261 6d65 2869 6e64  pd.DataFrame(ind
+0002d810: 6578 3d69 6e64 6578 290a 2020 2020 2020  ex=index).      
+0002d820: 2020 2320 2020 2020 2020 2073 656c 662e    #        self.
+0002d830: 6d61 7070 696e 6720 3d20 7064 2e44 6174  mapping = pd.Dat
+0002d840: 6146 7261 6d65 2869 6e64 6578 3d69 6e64  aFrame(index=ind
+0002d850: 6578 2c20 636f 6c75 6d6e 7320 3d20 5b73  ex, columns = [s
+0002d860: 656c 662e 7365 7475 702e 4d4f 4445 4c5f  elf.setup.MODEL_
+0002d870: 434f 4c55 4d4e 5f4e 414d 455d 290a 2020  COLUMN_NAME]).  
+0002d880: 2020 2020 2020 2320 2020 2020 2020 2073        #        s
+0002d890: 656c 662e 6d61 7070 696e 6720 3d20 7064  elf.mapping = pd
+0002d8a0: 2e63 6f6e 6361 7428 5b73 656c 662e 6d61  .concat([self.ma
+0002d8b0: 7070 696e 672c 2073 656c 662e 6176 6169  pping, self.avai
+0002d8c0: 6c61 626c 6553 6572 6965 735d 2c20 6178  lableSeries], ax
+0002d8d0: 6973 3d31 290a 2020 2020 2020 2020 2320  is=1).        # 
+0002d8e0: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
+0002d8f0: 696e 6720 3d20 7365 6c66 2e6d 6170 7069  ing = self.mappi
+0002d900: 6e67 2e73 6f72 745f 696e 6465 7828 290a  ng.sort_index().
+0002d910: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0002d920: 2073 656c 662e 6d61 7070 696e 672e 696e   self.mapping.in
+0002d930: 6465 782e 6e61 6d65 203d 2027 6f72 6967  dex.name = 'orig
+0002d940: 6e61 6c27 0a20 2020 2020 2020 2023 2020  nal'.        #  
+0002d950: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
+0002d960: 6e67 2e74 6f5f 6578 6365 6c28 7772 6974  ng.to_excel(writ
+0002d970: 6572 2c20 656e 6769 6e65 3d27 6f70 656e  er, engine='open
+0002d980: 7079 786c 272c 2073 6865 6574 5f6e 616d  pyxl', sheet_nam
+0002d990: 653d 276d 6f64 656c 5f6d 6170 7069 6e67  e='model_mapping
+0002d9a0: 2729 0a0a 2020 2020 2020 2020 2320 7363  ')..        # sc
+0002d9b0: 656e 6172 696f 730a 2020 2020 2020 2020  enarios.        
+0002d9c0: 696e 6465 7820 3d20 6e70 2e75 6e69 7175  index = np.uniqu
+0002d9d0: 6528 7365 6c66 2e64 6174 615b 7365 6c66  e(self.data[self
+0002d9e0: 2e73 6574 7570 2e53 4345 4e41 5249 4f5f  .setup.SCENARIO_
+0002d9f0: 434f 4c55 4d4e 5f4e 414d 455d 2e76 616c  COLUMN_NAME].val
+0002da00: 7565 7329 0a20 2020 2020 2020 2073 656c  ues).        sel
+0002da10: 662e 6176 6169 6c61 626c 6553 6572 6965  f.availableSerie
+0002da20: 7320 3d20 7064 2e44 6174 6146 7261 6d65  s = pd.DataFrame
+0002da30: 2869 6e64 6578 3d69 6e64 6578 290a 2020  (index=index).  
+0002da40: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
+0002da50: 6e67 203d 2070 642e 4461 7461 4672 616d  ng = pd.DataFram
+0002da60: 6528 0a20 2020 2020 2020 2020 2020 2069  e(.            i
+0002da70: 6e64 6578 3d69 6e64 6578 2c20 636f 6c75  ndex=index, colu
+0002da80: 6d6e 733d 5b73 656c 662e 7365 7475 702e  mns=[self.setup.
+0002da90: 5343 454e 4152 494f 5f43 4f4c 554d 4e5f  SCENARIO_COLUMN_
+0002daa0: 4e41 4d45 5d0a 2020 2020 2020 2020 290a  NAME].        ).
+0002dab0: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
+0002dac0: 7069 6e67 203d 2070 642e 636f 6e63 6174  ping = pd.concat
+0002dad0: 285b 7365 6c66 2e6d 6170 7069 6e67 2c20  ([self.mapping, 
+0002dae0: 7365 6c66 2e61 7661 696c 6162 6c65 5365  self.availableSe
+0002daf0: 7269 6573 5d2c 2061 7869 733d 3129 0a20  ries], axis=1). 
+0002db00: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
+0002db10: 696e 6720 3d20 7365 6c66 2e6d 6170 7069  ing = self.mappi
+0002db20: 6e67 2e73 6f72 745f 696e 6465 7828 290a  ng.sort_index().
+0002db30: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
+0002db40: 7069 6e67 2e69 6e64 6578 2e6e 616d 6520  ping.index.name 
+0002db50: 3d20 276f 7269 676e 616c 270a 2020 2020  = 'orignal'.    
+0002db60: 2020 2020 7365 6c66 2e6d 6170 7069 6e67      self.mapping
+0002db70: 2e74 6f5f 6578 6365 6c28 7772 6974 6572  .to_excel(writer
+0002db80: 2c20 656e 6769 6e65 3d27 6f70 656e 7079  , engine='openpy
+0002db90: 786c 272c 2073 6865 6574 5f6e 616d 653d  xl', sheet_name=
+0002dba0: 2773 6365 6e61 7269 6f5f 6d61 7070 696e  'scenario_mappin
+0002dbb0: 6727 290a 0a20 2020 2020 2020 2023 2072  g')..        # r
+0002dbc0: 6567 696f 6e0a 2020 2020 2020 2020 696e  egion.        in
+0002dbd0: 6465 7820 3d20 6e70 2e75 6e69 7175 6528  dex = np.unique(
+0002dbe0: 7365 6c66 2e64 6174 615b 7365 6c66 2e73  self.data[self.s
+0002dbf0: 6574 7570 2e52 4547 494f 4e5f 434f 4c55  etup.REGION_COLU
+0002dc00: 4d4e 5f4e 414d 455d 2e76 616c 7565 7329  MN_NAME].values)
+0002dc10: 0a20 2020 2020 2020 2073 656c 662e 6176  .        self.av
+0002dc20: 6169 6c61 626c 6553 6572 6965 7320 3d20  ailableSeries = 
+0002dc30: 7064 2e44 6174 6146 7261 6d65 2869 6e64  pd.DataFrame(ind
+0002dc40: 6578 3d69 6e64 6578 290a 2020 2020 2020  ex=index).      
+0002dc50: 2020 7365 6c66 2e6d 6170 7069 6e67 203d    self.mapping =
+0002dc60: 2070 642e 4461 7461 4672 616d 6528 0a20   pd.DataFrame(. 
+0002dc70: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+0002dc80: 3d69 6e64 6578 2c20 636f 6c75 6d6e 733d  =index, columns=
+0002dc90: 5b73 656c 662e 7365 7475 702e 5245 4749  [self.setup.REGI
+0002dca0: 4f4e 5f43 4f4c 554d 4e5f 4e41 4d45 5d0a  ON_COLUMN_NAME].
+0002dcb0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0002dcc0: 2020 7365 6c66 2e6d 6170 7069 6e67 203d    self.mapping =
+0002dcd0: 2070 642e 636f 6e63 6174 285b 7365 6c66   pd.concat([self
+0002dce0: 2e6d 6170 7069 6e67 2c20 7365 6c66 2e61  .mapping, self.a
+0002dcf0: 7661 696c 6162 6c65 5365 7269 6573 5d2c  vailableSeries],
+0002dd00: 2061 7869 733d 3129 0a20 2020 2020 2020   axis=1).       
+0002dd10: 2073 656c 662e 6d61 7070 696e 6720 3d20   self.mapping = 
+0002dd20: 7365 6c66 2e6d 6170 7069 6e67 2e73 6f72  self.mapping.sor
+0002dd30: 745f 696e 6465 7828 290a 2020 2020 2020  t_index().      
+0002dd40: 2020 7365 6c66 2e6d 6170 7069 6e67 2e69    self.mapping.i
+0002dd50: 6e64 6578 2e6e 616d 6520 3d20 276f 7269  ndex.name = 'ori
+0002dd60: 676e 616c 270a 2020 2020 2020 2020 666f  gnal'.        fo
+0002dd70: 7220 6964 7820 696e 2073 656c 662e 6d61  r idx in self.ma
+0002dd80: 7070 696e 672e 696e 6465 783a 0a20 2020  pping.index:.   
+0002dd90: 2020 2020 2020 2020 2069 736f 203d 2064           iso = d
+0002dda0: 742e 7574 696c 2e69 6465 6e74 6966 7943  t.util.identifyC
+0002ddb0: 6f75 6e74 7279 2869 6478 290a 2020 2020  ountry(idx).    
+0002ddc0: 2020 2020 2020 2020 6966 2069 736f 2069          if iso i
+0002ddd0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002dde0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002ddf0: 2e6d 6170 7069 6e67 2e6c 6f63 5b69 6478  .mapping.loc[idx
+0002de00: 2c20 2772 6567 696f 6e27 5d20 3d20 6973  , 'region'] = is
+0002de10: 6f0a 0a20 2020 2020 2020 2073 656c 662e  o..        self.
+0002de20: 6d61 7070 696e 672e 746f 5f65 7863 656c  mapping.to_excel
+0002de30: 2877 7269 7465 722c 2065 6e67 696e 653d  (writer, engine=
+0002de40: 276f 7065 6e70 7978 6c27 2c20 7368 6565  'openpyxl', shee
+0002de50: 745f 6e61 6d65 3d27 7265 6769 6f6e 5f6d  t_name='region_m
+0002de60: 6170 7069 6e67 2729 0a20 2020 2020 2020  apping').       
+0002de70: 2077 7269 7465 722e 636c 6f73 6528 290a   writer.close().
+0002de80: 0a20 2020 2064 6566 2067 6174 6865 724d  .    def gatherM
+0002de90: 6170 7065 6444 6174 6128 7365 6c66 2c20  appedData(self, 
+0002dea0: 7370 6174 6961 6c53 7562 5365 743d 4e6f  spatialSubSet=No
+0002deb0: 6e65 293a 0a0a 2020 2020 2020 2020 696d  ne):..        im
+0002dec0: 706f 7274 2074 7164 6d0a 0a20 2020 2020  port tqdm..     
+0002ded0: 2020 2023 206c 6f61 6469 6e67 2064 6174     # loading dat
+0002dee0: 6120 6966 206e 6563 6573 7361 7279 0a20  a if necessary. 
+0002def0: 2020 2020 2020 2069 6620 6e6f 7420 6861         if not ha
+0002df00: 7361 7474 7228 7365 6c66 2c20 2764 6174  sattr(self, 'dat
+0002df10: 6127 293a 0a20 2020 2020 2020 2020 2020  a'):.           
+0002df20: 2073 656c 662e 6c6f 6164 4461 7461 2829   self.loadData()
+0002df30: 0a0a 2020 2020 2020 2020 7461 626c 6573  ..        tables
+0002df40: 546f 436f 6d6d 6974 203d 205b 5d0a 2020  ToCommit = [].  
+0002df50: 2020 2020 2020 6d65 7461 4469 6374 203d        metaDict =
+0002df60: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0002df70: 6d65 7461 4469 6374 5b27 736f 7572 6365  metaDict['source
+0002df80: 275d 203d 2073 656c 662e 7365 7475 702e  '] = self.setup.
+0002df90: 534f 5552 4345 5f49 440a 2020 2020 2020  SOURCE_ID.      
+0002dfa0: 2020 6578 636c 7564 6564 5461 626c 6573    excludedTables
+0002dfb0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+0002dfc0: 2020 6578 636c 7564 6564 5461 626c 6573    excludedTables
+0002dfd0: 5b27 656d 7074 7927 5d20 3d20 6c69 7374  ['empty'] = list
+0002dfe0: 2829 0a20 2020 2020 2020 2065 7863 6c75  ().        exclu
+0002dff0: 6465 6454 6162 6c65 735b 2765 7272 6f72  dedTables['error
+0002e000: 275d 203d 206c 6973 7428 290a 2020 2020  '] = list().    
+0002e010: 2020 2020 6578 636c 7564 6564 5461 626c      excludedTabl
+0002e020: 6573 5b27 6578 6973 7473 275d 203d 206c  es['exists'] = l
+0002e030: 6973 7428 290a 0a20 2020 2020 2020 2066  ist()..        f
+0002e040: 6f72 206d 6f64 656c 2069 6e20 5b27 275d  or model in ['']
+0002e050: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+0002e060: 6d70 4d6f 203d 2073 656c 662e 6461 7461  mpMo = self.data
+0002e070: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0002e080: 2020 2020 2020 2020 2020 2074 656d 704d             tempM
+0002e090: 6f20 3d20 7365 6c66 2e64 6174 612e 6c6f  o = self.data.lo
+0002e0a0: 635b 7365 6c66 2e64 6174 612e 6d6f 6465  c[self.data.mode
+0002e0b0: 6c20 3d3d 206d 6f64 656c 5d0a 2020 2020  l == model].    
+0002e0c0: 2020 2020 2020 2020 666f 7220 7363 656e          for scen
+0002e0d0: 6172 696f 2069 6e20 7365 6c66 2e6d 6170  ario in self.map
+0002e0e0: 7069 6e67 5b27 7363 656e 6172 696f 275d  ping['scenario']
+0002e0f0: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
+0002e100: 2020 2020 2020 2020 2074 656d 704d 6f53           tempMoS
+0002e110: 6320 3d20 7465 6d70 4d6f 2e6c 6f63 5b74  c = tempMo.loc[t
+0002e120: 656d 704d 6f2e 7363 656e 6172 696f 203d  empMo.scenario =
+0002e130: 3d20 7363 656e 6172 696f 5d0a 2020 2020  = scenario].    
+0002e140: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+0002e150: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0002e160: 2076 6172 6961 626c 6520 696e 2073 656c   variable in sel
+0002e170: 662e 6d61 7070 696e 675b 2776 6172 6961  f.mapping['varia
+0002e180: 626c 6527 5d2e 6b65 7973 2829 3a0a 2020  ble'].keys():.  
+0002e190: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0002e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e1b0: 2020 2074 656d 704d 6f53 6356 6120 3d20     tempMoScVa = 
+0002e1c0: 7465 6d70 4d6f 5363 2e6c 6f63 5b73 656c  tempMoSc.loc[sel
+0002e1d0: 662e 6461 7461 2e76 6172 6961 626c 6520  f.data.variable 
+0002e1e0: 3d3d 2076 6172 6961 626c 655d 0a0a 2020  == variable]..  
+0002e1f0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0002e200: 7220 7661 7269 6162 6c65 2069 6e20 6c69  r variable in li
+0002e210: 7374 2873 656c 662e 6d61 7070 696e 675b  st(self.mapping[
+0002e220: 2765 6e74 6974 7927 5d2e 6b65 7973 2829  'entity'].keys()
+0002e230: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0002e240: 2020 2020 2020 2074 656d 704d 6f53 6356         tempMoScV
+0002e250: 6172 203d 2074 656d 704d 6f53 632e 6c6f  ar = tempMoSc.lo
+0002e260: 635b 7465 6d70 4d6f 5363 2e65 6e74 6974  c[tempMoSc.entit
+0002e270: 7920 3d3d 2076 6172 6961 626c 655d 0a20  y == variable]. 
+0002e280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e290: 2020 2074 656d 704d 6f53 6356 6172 2e75     tempMoScVar.u
+0002e2a0: 6e69 7420 3d20 7365 6c66 2e6d 6170 7069  nit = self.mappi
+0002e2b0: 6e67 5b27 756e 6974 275d 5b76 6172 6961  ng['unit'][varia
+0002e2c0: 626c 655d 0a20 2020 2020 2020 2020 2020  ble].           
+0002e2d0: 2020 2020 2020 2020 2023 2020 2020 2020           #      
+0002e2e0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+0002e2f0: 626c 6573 203d 2064 742e 696e 7465 7266  bles = dt.interf
+0002e300: 6163 6573 2e72 6561 645f 6c6f 6e67 5f74  aces.read_long_t
+0002e310: 6162 6c65 2874 656d 704d 6f53 6356 6172  able(tempMoScVar
+0002e320: 2c20 5b76 6172 6961 626c 655d 290a 0a20  , [variable]).. 
+0002e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e340: 2020 2074 6162 6c65 203d 2074 656d 704d     table = tempM
+0002e350: 6f53 6356 6172 2e6c 6f63 5b3a 2c20 7365  oScVar.loc[:, se
+0002e360: 6c66 2e74 696d 6543 6f6c 756d 6e73 5d0a  lf.timeColumns].
+0002e370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002e380: 2020 2020 2074 6162 6c65 203d 2044 6174       table = Dat
+0002e390: 6174 6162 6c65 280a 2020 2020 2020 2020  atable(.        
+0002e3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e3b0: 7461 626c 652c 0a20 2020 2020 2020 2020  table,.         
+0002e3c0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0002e3d0: 6574 613d 7b0a 2020 2020 2020 2020 2020  eta={.          
+0002e3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e3f0: 2020 2765 6e74 6974 7927 3a20 7365 6c66    'entity': self
+0002e400: 2e6d 6170 7069 6e67 5b27 656e 7469 7479  .mapping['entity
+0002e410: 275d 5b76 6172 6961 626c 655d 2c0a 2020  '][variable],.  
 0002e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e430: 2020 2020 2763 6174 6567 6f72 7927 3a20      'category': 
-0002e440: 7365 6c66 2e6d 6170 7069 6e67 5b27 6361  self.mapping['ca
-0002e450: 7465 676f 7279 275d 5b76 6172 6961 626c  tegory'][variabl
-0002e460: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
+0002e430: 2020 2020 2020 2020 2020 2763 6174 6567            'categ
+0002e440: 6f72 7927 3a20 7365 6c66 2e6d 6170 7069  ory': self.mappi
+0002e450: 6e67 5b27 6361 7465 676f 7279 275d 5b76  ng['category'][v
+0002e460: 6172 6961 626c 655d 2c0a 2020 2020 2020  ariable],.      
 0002e470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e480: 2773 6365 6e61 7269 6f27 3a20 7363 656e  'scenario': scen
-0002e490: 6172 696f 2c0a 2020 2020 2020 2020 2020  ario,.          
+0002e480: 2020 2020 2020 2773 6365 6e61 7269 6f27        'scenario'
+0002e490: 3a20 7363 656e 6172 696f 2c0a 2020 2020  : scenario,.    
 0002e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e4b0: 2020 2773 6f75 7263 6527 3a20 7365 6c66    'source': self
-0002e4c0: 2e73 6574 7570 2e53 4f55 5243 455f 4944  .setup.SOURCE_ID
-0002e4d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002e4e0: 2020 2020 2020 2020 2020 2020 2020 2775                'u
-0002e4f0: 6e69 7427 3a20 7365 6c66 2e6d 6170 7069  nit': self.mappi
-0002e500: 6e67 5b27 756e 6974 275d 5b76 6172 6961  ng['unit'][varia
-0002e510: 626c 655d 2c0a 2020 2020 2020 2020 2020  ble],.          
-0002e520: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-0002e530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002e540: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0002e550: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-0002e560: 2e69 6e64 6578 203d 2074 656d 704d 6f53  .index = tempMoS
-0002e570: 6356 6172 2e72 6567 696f 6e0a 2020 2020  cVar.region.    
-0002e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e590: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-0002e5a0: 2020 2020 2074 6162 6c65 2e6d 6574 615b       table.meta[
-0002e5b0: 2763 6174 6567 6f72 7927 5d20 3d20 2222  'category'] = ""
-0002e5c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002e5d0: 2020 2020 2023 2020 2020 2020 2020 2020       #          
-0002e5e0: 2020 2020 2020 2020 2020 7461 626c 652e            table.
-0002e5f0: 6d65 7461 5b27 736f 7572 6365 275d 203d  meta['source'] =
-0002e600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002e610: 2020 2020 2074 6162 6c65 2e69 6e64 6578       table.index
-0002e620: 203d 2074 6162 6c65 2e69 6e64 6578 2e6d   = table.index.m
-0002e630: 6170 2873 656c 662e 6d61 7070 696e 675b  ap(self.mapping[
-0002e640: 2772 6567 696f 6e27 5d29 0a0a 2020 2020  'region'])..    
-0002e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e660: 7461 626c 6520 3d20 7461 626c 652e 6c6f  table = table.lo
-0002e670: 635b 7e70 642e 6973 6e61 2874 6162 6c65  c[~pd.isna(table
-0002e680: 2e69 6e64 6578 292c 203a 5d0a 0a20 2020  .index), :]..   
-0002e690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e6a0: 2069 6620 6e6f 7420 7064 2e69 736e 6128   if not pd.isna(
-0002e6b0: 7365 6c66 2e6d 6170 7069 6e67 5b27 756e  self.mapping['un
-0002e6c0: 6974 546f 275d 5b76 6172 6961 626c 655d  itTo'][variable]
-0002e6d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0002e6e0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0002e6f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0002e700: 2020 2020 2020 2020 2020 2020 2020 2763                'c
-0002e710: 6f6e 7665 7273 696f 6e20 746f 203a 2027  onversion to : '
-0002e720: 202b 2073 7472 2873 656c 662e 6d61 7070   + str(self.mapp
-0002e730: 696e 675b 2775 6e69 7454 6f27 5d5b 7661  ing['unitTo'][va
-0002e740: 7269 6162 6c65 5d29 0a20 2020 2020 2020  riable]).       
+0002e4b0: 2020 2020 2020 2020 2773 6f75 7263 6527          'source'
+0002e4c0: 3a20 7365 6c66 2e73 6574 7570 2e53 4f55  : self.setup.SOU
+0002e4d0: 5243 455f 4944 2c0a 2020 2020 2020 2020  RCE_ID,.        
+0002e4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e4f0: 2020 2020 2775 6e69 7427 3a20 7365 6c66      'unit': self
+0002e500: 2e6d 6170 7069 6e67 5b27 756e 6974 275d  .mapping['unit']
+0002e510: 5b76 6172 6961 626c 655d 2c0a 2020 2020  [variable],.    
+0002e520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e530: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+0002e540: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0002e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e560: 2074 6162 6c65 2e69 6e64 6578 203d 2074   table.index = t
+0002e570: 656d 704d 6f53 6356 6172 2e72 6567 696f  empMoScVar.regio
+0002e580: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+0002e590: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0002e5a0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+0002e5b0: 2e6d 6574 615b 2763 6174 6567 6f72 7927  .meta['category'
+0002e5c0: 5d20 3d20 2222 0a20 2020 2020 2020 2020  ] = "".         
+0002e5d0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+0002e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e5f0: 7461 626c 652e 6d65 7461 5b27 736f 7572  table.meta['sour
+0002e600: 6365 275d 203d 0a20 2020 2020 2020 2020  ce'] =.         
+0002e610: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+0002e620: 2e69 6e64 6578 203d 2074 6162 6c65 2e69  .index = table.i
+0002e630: 6e64 6578 2e6d 6170 2873 656c 662e 6d61  ndex.map(self.ma
+0002e640: 7070 696e 675b 2772 6567 696f 6e27 5d29  pping['region'])
+0002e650: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0002e660: 2020 2020 2020 7461 626c 6520 3d20 7461        table = ta
+0002e670: 626c 652e 6c6f 635b 7e70 642e 6973 6e61  ble.loc[~pd.isna
+0002e680: 2874 6162 6c65 2e69 6e64 6578 292c 203a  (table.index), :
+0002e690: 5d0a 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0002e6a0: 2020 2020 2020 2069 6620 6e6f 7420 7064         if not pd
+0002e6b0: 2e69 736e 6128 7365 6c66 2e6d 6170 7069  .isna(self.mappi
+0002e6c0: 6e67 5b27 756e 6974 546f 275d 5b76 6172  ng['unitTo'][var
+0002e6d0: 6961 626c 655d 293a 0a20 2020 2020 2020  iable]):.       
+0002e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e6f0: 2070 7269 6e74 280a 2020 2020 2020 2020   print(.        
+0002e700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e710: 2020 2020 2763 6f6e 7665 7273 696f 6e20      'conversion 
+0002e720: 746f 203a 2027 202b 2073 7472 2873 656c  to : ' + str(sel
+0002e730: 662e 6d61 7070 696e 675b 2775 6e69 7454  f.mapping['unitT
+0002e740: 6f27 5d5b 7661 7269 6162 6c65 5d29 0a20  o'][variable]). 
 0002e750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e760: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0002e770: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-0002e780: 203d 2074 6162 6c65 2e63 6f6e 7665 7274   = table.convert
-0002e790: 2873 656c 662e 6d61 7070 696e 675b 2775  (self.mapping['u
-0002e7a0: 6e69 7454 6f27 5d5b 7661 7269 6162 6c65  nitTo'][variable
-0002e7b0: 5d29 0a0a 2020 2020 2020 2020 2020 2020  ])..            
-0002e7c0: 2020 2020 2020 2020 7461 626c 6549 4420          tableID 
-0002e7d0: 3d20 6474 2e63 6f72 652e 5f63 7265 6174  = dt.core._creat
-0002e7e0: 6544 6174 6162 6173 6549 4428 7461 626c  eDatabaseID(tabl
-0002e7f0: 652e 6d65 7461 290a 2020 2020 2020 2020  e.meta).        
-0002e800: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
-0002e810: 6573 546f 436f 6d6d 6974 2e61 7070 656e  esToCommit.appen
-0002e820: 6428 7461 626c 6529 0a0a 2020 2020 2020  d(table)..      
-0002e830: 2020 7265 7475 726e 2074 6162 6c65 7354    return tablesT
-0002e840: 6f43 6f6d 6d69 742c 2065 7863 6c75 6465  oCommit, exclude
-0002e850: 6454 6162 6c65 730a 0a0a 636c 6173 7320  dTables...class 
-0002e860: 5745 4f28 4261 7365 496d 706f 7274 546f  WEO(BaseImportTo
-0002e870: 6f6c 293a 0a20 2020 2022 2222 0a20 2020  ol):.    """.   
-0002e880: 2057 454f 2064 6174 6120 696d 706f 7274   WEO data import
-0002e890: 2074 6f6f 6c0a 2020 2020 2222 220a 0a20   tool.    """.. 
-0002e8a0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0002e8b0: 7365 6c66 2c20 7965 6172 293a 0a20 2020  self, year):.   
-0002e8c0: 2020 2020 2073 656c 662e 7365 7475 7020       self.setup 
-0002e8d0: 3d20 7365 7475 7053 7472 7563 7428 290a  = setupStruct().
-0002e8e0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0002e8f0: 7570 2e53 4f55 5243 455f 4944 203d 2022  up.SOURCE_ID = "
-0002e900: 5745 4f5f 2220 2b20 7374 7228 7965 6172  WEO_" + str(year
-0002e910: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0002e920: 6574 7570 2e53 4f55 5243 455f 5041 5448  etup.SOURCE_PATH
-0002e930: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-0002e940: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-0002e950: 6669 672e 5041 5448 5f54 4f5f 4441 5441  fig.PATH_TO_DATA
-0002e960: 5348 454c 462c 2066 2772 6177 6461 7461  SHELF, f'rawdata
-0002e970: 2f57 454f 2f7b 7965 6172 7d27 0a20 2020  /WEO/{year}'.   
-0002e980: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-0002e990: 656c 662e 7365 7475 702e 4441 5441 5f46  elf.setup.DATA_F
-0002e9a0: 494c 4520 3d20 6627 5745 4f7b 7965 6172  ILE = f'WEO{year
-0002e9b0: 7d5f 416e 6e65 7841 2e78 6c73 7827 0a20  }_AnnexA.xlsx'. 
-0002e9c0: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
-0002e9d0: 702e 4d41 5050 494e 475f 4649 4c45 203d  p.MAPPING_FILE =
-0002e9e0: 206f 732e 7061 7468 2e6a 6f69 6e28 0a20   os.path.join(. 
-0002e9f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002ea00: 7365 7475 702e 534f 5552 4345 5f50 4154  setup.SOURCE_PAT
-0002ea10: 482c 2066 276d 6170 7069 6e67 5f57 454f  H, f'mapping_WEO
-0002ea20: 5f7b 7965 6172 7d2e 786c 7378 270a 2020  _{year}.xlsx'.  
-0002ea30: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0002ea40: 7365 6c66 2e73 6574 7570 2e4c 4943 454e  self.setup.LICEN
-0002ea50: 4345 203d 2027 4945 4120 616c 6c20 7269  CE = 'IEA all ri
-0002ea60: 6768 7473 2072 6573 6572 7665 6427 0a20  ghts reserved'. 
-0002ea70: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
-0002ea80: 702e 5552 4c20 3d20 2768 7474 7073 3a2f  p.URL = 'https:/
-0002ea90: 2f77 7777 2e69 6561 2e6f 7267 2f77 656f  /www.iea.org/weo
-0002eaa0: 2f27 0a0a 2020 2020 2020 2020 2320 2020  /'..        #   
-0002eab0: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
-0002eac0: 494e 4445 585f 434f 4c55 4d4e 5f4e 414d  INDEX_COLUMN_NAM
-0002ead0: 4520 3d20 5b27 464c 4f57 272c 2027 5052  E = ['FLOW', 'PR
-0002eae0: 4f44 5543 5427 5d0a 2020 2020 2020 2020  ODUCT'].        
-0002eaf0: 2320 2020 2020 2020 2073 656c 662e 7365  #        self.se
-0002eb00: 7475 702e 5350 4154 4941 4c5f 434f 4c55  tup.SPATIAL_COLU
-0002eb10: 4d5f 4e41 4d45 203d 2027 434f 554e 5452  M_NAME = 'COUNTR
-0002eb20: 5927 0a20 2020 2020 2020 2023 2020 2020  Y'.        #    
-0002eb30: 2020 2020 7365 6c66 2e73 6574 7570 2e43      self.setup.C
-0002eb40: 4f4c 554d 4e53 5f54 4f5f 4452 4f50 203d  OLUMNS_TO_DROP =
-0002eb50: 205b 2027 5052 4f44 5543 5427 2c27 464c   [ 'PRODUCT','FL
-0002eb60: 4f57 272c 2763 6f6d 6269 6e65 6427 5d0a  OW','combined'].
-0002eb70: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0002eb80: 286f 732e 7061 7468 2e65 7869 7374 7328  (os.path.exists(
-0002eb90: 7365 6c66 2e73 6574 7570 2e4d 4150 5049  self.setup.MAPPI
-0002eba0: 4e47 5f46 494c 4529 293a 0a20 2020 2020  NG_FILE)):.     
-0002ebb0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0002ebc0: 2020 2020 7365 6c66 2e63 7265 6174 6556      self.createV
-0002ebd0: 6172 6961 626c 654d 6170 7069 6e67 2829  ariableMapping()
-0002ebe0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-0002ebf0: 6e74 2822 6e6f 206d 6170 7069 6e67 2066  nt("no mapping f
-0002ec00: 696c 6520 666f 756e 6422 290a 2020 2020  ile found").    
-0002ec10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0002ec20: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
-0002ec30: 6e67 456e 6572 6779 203d 2070 642e 7265  ngEnergy = pd.re
-0002ec40: 6164 5f65 7863 656c 280a 2020 2020 2020  ad_excel(.      
-0002ec50: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0002ec60: 6574 7570 2e4d 4150 5049 4e47 5f46 494c  etup.MAPPING_FIL
-0002ec70: 452c 2073 6865 6574 5f6e 616d 653d 2745  E, sheet_name='E
-0002ec80: 6e65 7267 795f 4261 6c61 6e63 6527 0a20  nergy_Balance'. 
-0002ec90: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0002eca0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-0002ecb0: 7070 696e 6745 6d69 7373 696f 6e73 203d  ppingEmissions =
-0002ecc0: 2070 642e 7265 6164 5f65 7863 656c 280a   pd.read_excel(.
-0002ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ece0: 7365 6c66 2e73 6574 7570 2e4d 4150 5049  self.setup.MAPPI
-0002ecf0: 4e47 5f46 494c 452c 2073 6865 6574 5f6e  NG_FILE, sheet_n
-0002ed00: 616d 653d 2753 495f 434f 325f 496e 6427  ame='SI_CO2_Ind'
-0002ed10: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-0002ed20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002ed30: 2e73 7061 7469 616c 4d61 7070 696e 6720  .spatialMapping 
-0002ed40: 3d20 7064 2e72 6561 645f 6578 6365 6c28  = pd.read_excel(
-0002ed50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002ed60: 2073 656c 662e 7365 7475 702e 4d41 5050   self.setup.MAPP
-0002ed70: 494e 475f 4649 4c45 2c20 7368 6565 745f  ING_FILE, sheet_
-0002ed80: 6e61 6d65 3d27 7370 6174 6961 6c27 0a20  name='spatial'. 
-0002ed90: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-0002eda0: 2020 2020 2020 7365 6c66 2e63 7265 6174        self.creat
-0002edb0: 6553 6f75 7263 654d 6574 6128 290a 0a20  eSourceMeta().. 
-0002edc0: 2020 2064 6566 2061 6464 5370 6174 6961     def addSpatia
-0002edd0: 6c4d 6170 7069 6e67 2873 656c 6629 3a0a  lMapping(self):.
-0002ede0: 2020 2020 2020 2020 2320 4555 0a20 2020          # EU.   
-0002edf0: 2020 2020 206d 6170 7069 6e67 546f 436f       mappingToCo
-0002ee00: 756e 7472 6965 7320 3d20 6469 6374 2829  untries = dict()
-0002ee10: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
-0002ee20: 7370 6174 6961 6c4d 6170 7069 6e67 2e6c  spatialMapping.l
-0002ee30: 6f63 5b27 4d65 6d6f 3a20 4575 726f 7065  oc['Memo: Europe
-0002ee40: 616e 2055 6e69 6f6e 2d32 3827 5d20 3d20  an Union-28'] = 
-0002ee50: 2745 5532 3827 0a20 2020 2020 2020 206d  'EU28'.        m
-0002ee60: 6170 7069 6e67 546f 436f 756e 7472 6965  appingToCountrie
-0002ee70: 735b 2741 5345 414e 275d 203d 205b 0a20  s['ASEAN'] = [. 
-0002ee80: 2020 2020 2020 2020 2020 2027 564e 4d27             'VNM'
-0002ee90: 2c0a 2020 2020 2020 2020 2020 2020 2750  ,.            'P
-0002eea0: 484c 272c 0a20 2020 2020 2020 2020 2020  HL',.           
-0002eeb0: 2027 5448 4127 2c0a 2020 2020 2020 2020   'THA',.        
-0002eec0: 2020 2020 2753 4750 272c 0a20 2020 2020      'SGP',.     
-0002eed0: 2020 2020 2020 2027 4d4d 5227 2c0a 2020         'MMR',.  
-0002eee0: 2020 2020 2020 2020 2020 2749 444e 272c            'IDN',
-0002eef0: 0a20 2020 2020 2020 2020 2020 2027 4b48  .            'KH
-0002ef00: 4d27 2c0a 2020 2020 2020 2020 2020 2020  M',.            
-0002ef10: 2742 524e 272c 0a20 2020 2020 2020 2020  'BRN',.         
-0002ef20: 2020 2027 4d59 5327 2c0a 2020 2020 2020     'MYS',.      
-0002ef30: 2020 2020 2020 274c 414f 272c 0a20 2020        'LAO',.   
-0002ef40: 2020 2020 205d 0a20 2020 2020 2020 2064       ].        d
-0002ef50: 742e 6d61 7070 2e72 6567 696f 6e73 2e61  t.mapp.regions.a
-0002ef60: 6464 5265 6769 6f6e 546f 436f 6e74 6578  ddRegionToContex
-0002ef70: 7428 2757 454f 272c 206d 6170 7069 6e67  t('WEO', mapping
-0002ef80: 546f 436f 756e 7472 6965 7329 0a0a 2020  ToCountries)..  
-0002ef90: 2020 6465 6620 6761 7468 6572 4d61 7070    def gatherMapp
-0002efa0: 6564 4461 7461 2873 656c 662c 2073 7061  edData(self, spa
-0002efb0: 7469 616c 5375 6253 6574 3d4e 6f6e 6529  tialSubSet=None)
-0002efc0: 3a0a 0a20 2020 2020 2020 2074 6162 6c65  :..        table
-0002efd0: 7354 6f43 6f6d 6d69 7420 3d20 6474 2e54  sToCommit = dt.T
-0002efe0: 6162 6c65 5365 7428 290a 2020 2020 2020  ableSet().      
-0002eff0: 2020 7365 7475 7020 3d20 6469 6374 2829    setup = dict()
-0002f000: 0a20 2020 2020 2020 2073 6574 7570 5b27  .        setup['
-0002f010: 6669 6c65 5061 7468 275d 203d 2073 656c  filePath'] = sel
-0002f020: 662e 7365 7475 702e 534f 5552 4345 5f50  f.setup.SOURCE_P
-0002f030: 4154 480a 2020 2020 2020 2020 7365 7475  ATH.        setu
-0002f040: 705b 2766 696c 654e 616d 6527 5d20 3d20  p['fileName'] = 
-0002f050: 7365 6c66 2e73 6574 7570 2e44 4154 415f  self.setup.DATA_
-0002f060: 4649 4c45 0a0a 2020 2020 2020 2020 2320  FILE..        # 
-0002f070: 6c6f 6f70 206f 7665 7220 656e 6572 6779  loop over energy
-0002f080: 206d 6170 7069 6e67 0a20 2020 2020 2020   mapping.       
-0002f090: 2066 6f72 2072 6567 696f 6e20 696e 2073   for region in s
-0002f0a0: 656c 662e 7370 6174 6961 6c4d 6170 7069  elf.spatialMappi
-0002f0b0: 6e67 2e69 6e64 6578 3a0a 2020 2020 2020  ng.index:.      
-0002f0c0: 2020 2020 2020 7365 7475 705b 2773 6865        setup['she
-0002f0d0: 6574 4e61 6d65 275d 203d 2072 6567 696f  etName'] = regio
-0002f0e0: 6e20 2b20 275f 4261 6c61 6e63 6527 0a20  n + '_Balance'. 
-0002f0f0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-0002f100: 2c20 6964 7820 696e 2065 6e75 6d65 7261  , idx in enumera
-0002f110: 7465 286c 6973 7428 7365 6c66 2e6d 6170  te(list(self.map
-0002f120: 7069 6e67 456e 6572 6779 2e69 6e64 6578  pingEnergy.index
-0002f130: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-0002f140: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0002f150: 2020 2020 2070 7269 6e74 2869 290a 2020       print(i).  
-0002f160: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-0002f170: 7461 4466 203d 2073 656c 662e 6d61 7070  taDf = self.mapp
-0002f180: 696e 6745 6e65 7267 792e 6c6f 635b 6964  ingEnergy.loc[id
-0002f190: 782c 203a 5d0a 2020 2020 2020 2020 2020  x, :].          
-0002f1a0: 2020 2020 2020 7072 696e 7428 6d65 7461        print(meta
-0002f1b0: 4466 5b27 5768 6174 275d 290a 0a20 2020  Df['What'])..   
-0002f1c0: 2020 2020 2020 2020 2020 2020 2023 2043               # C
-0002f1d0: 6170 6163 6974 790a 2020 2020 2020 2020  apacity.        
-0002f1e0: 2020 2020 2020 2020 7365 7475 705b 2774          setup['t
-0002f1f0: 696d 6549 6478 4c69 7374 275d 203d 2074  imeIdxList'] = t
-0002f200: 7570 6c65 286d 6574 6144 665b 2754 696d  uple(metaDf['Tim
-0002f210: 6527 5d2e 7370 6c69 7428 273a 2729 290a  e'].split(':')).
-0002f220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f230: 7365 7475 705b 2773 7061 6365 4964 784c  setup['spaceIdxL
-0002f240: 6973 7427 5d20 3d20 7475 706c 6528 5b6d  ist'] = tuple([m
-0002f250: 6574 6144 665b 2757 6861 7427 5d5d 290a  etaDf['What']]).
-0002f260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f270: 2320 7072 696e 7428 6d65 7461 4466 5b63  # print(metaDf[c
-0002f280: 6f6e 6669 672e 5245 5155 4952 4544 5f4d  onfig.REQUIRED_M
-0002f290: 4554 415f 4649 454c 4453 5d2e 6973 6e75  ETA_FIELDS].isnu
-0002f2a0: 6c6c 2829 2e61 6c6c 2829 203d 3d20 4661  ll().all() == Fa
-0002f2b0: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
-0002f2c0: 2020 2020 2023 2070 7269 6e74 286d 6574       # print(met
-0002f2d0: 6144 6174 615b 7365 6c66 2e73 6574 7570  aData[self.setup
-0002f2e0: 2e49 4e44 4558 5f43 4f4c 554d 4e5f 4e41  .INDEX_COLUMN_NA
-0002f2f0: 4d45 5d29 0a0a 2020 2020 2020 2020 2020  ME])..          
-0002f300: 2020 2020 2020 6966 2069 203d 3d20 303a        if i == 0:
-0002f310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002f320: 2020 2020 2065 7820 3d20 6474 2e69 6f2e       ex = dt.io.
-0002f330: 4578 6365 6c52 6561 6465 7228 7365 7475  ExcelReader(setu
-0002f340: 7029 0a20 2020 2020 2020 2020 2020 2020  p).             
-0002f350: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0002f360: 2020 2020 2020 2020 2020 2020 2065 782e               ex.
-0002f370: 7469 6d65 4964 784c 6973 7420 3d20 5b0a  timeIdxList = [.
-0002f380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f390: 2020 2020 2020 2020 6474 2e69 6f2e 6578          dt.io.ex
-0002f3a0: 6365 6c49 6478 3250 616e 6461 7349 6478  celIdx2PandasIdx
-0002f3b0: 2878 2920 666f 7220 7820 696e 2073 6574  (x) for x in set
-0002f3c0: 7570 5b27 7469 6d65 4964 784c 6973 7427  up['timeIdxList'
-0002f3d0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0002f3e0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-0002f3f0: 2020 2020 2020 2020 2020 2020 6578 2e73              ex.s
-0002f400: 7061 6365 4964 784c 6973 7420 3d20 5b0a  paceIdxList = [.
-0002f410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f420: 2020 2020 2020 2020 6474 2e69 6f2e 6578          dt.io.ex
-0002f430: 6365 6c49 6478 3250 616e 6461 7349 6478  celIdx2PandasIdx
-0002f440: 2878 2920 666f 7220 7820 696e 2073 6574  (x) for x in set
-0002f450: 7570 5b27 7370 6163 6549 6478 4c69 7374  up['spaceIdxList
-0002f460: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
-0002f470: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-0002f480: 2020 2020 2020 2020 2020 2020 2023 2070               # p
-0002f490: 7269 6e74 2865 782e 6466 290a 2020 2020  rint(ex.df).    
-0002f4a0: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-0002f4b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0002f4c0: 2249 6e74 6572 6e61 7469 6f6e 616c 2220  "International" 
-0002f4d0: 696e 206d 6574 6144 665b 274e 616d 6527  in metaDf['Name'
-0002f4e0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-0002f4f0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0002f500: 2020 2020 2020 2020 7364 660a 2020 2020          sdf.    
-0002f510: 2020 2020 2020 2020 2020 2020 6966 2065              if e
-0002f520: 782e 7370 6163 6549 6478 4c69 7374 5b30  x.spaceIdxList[0
-0002f530: 5d5b 305d 203e 2034 3120 616e 6420 7265  ][0] > 41 and re
-0002f540: 6769 6f6e 2021 3d20 2757 6f72 6c64 273a  gion != 'World':
-0002f550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002f560: 2020 2020 2065 782e 7370 6163 6549 6478       ex.spaceIdx
-0002f570: 4c69 7374 203d 205b 2865 782e 7370 6163  List = [(ex.spac
-0002f580: 6549 6478 4c69 7374 5b30 5d5b 305d 202d  eIdxList[0][0] -
-0002f590: 2031 2c20 3029 5d0a 0a20 2020 2020 2020   1, 0)]..       
-0002f5a0: 2020 2020 2020 2020 2023 2020 2020 2020           #      
-0002f5b0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0002f5c0: 6578 2e73 6574 7570 2829 290a 2020 2020  ex.setup()).    
-0002f5d0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0002f5e0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-0002f5f0: 2020 2020 2020 2020 2020 2064 6620 3d20             df = 
-0002f600: 6578 2e67 6174 6865 7244 6174 6128 290a  ex.gatherData().
-0002f610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f620: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0002f630: 2020 2020 2020 2020 2020 6466 203d 2065            df = e
-0002f640: 782e 6761 7468 6572 4461 7461 286c 6f61  x.gatherData(loa
-0002f650: 643d 4661 6c73 6529 0a20 2020 2020 2020  d=False).       
-0002f660: 2020 2020 2020 2020 2070 7269 6e74 2864           print(d
-0002f670: 6629 0a20 2020 2020 2020 2020 2020 2020  f).             
-0002f680: 2020 2064 6620 3d20 6466 2e6c 6f63 5b3a     df = df.loc[:
-0002f690: 2c20 7965 6172 7343 6f6c 756d 6e73 4f6e  , yearsColumnsOn
-0002f6a0: 6c79 2864 6629 5d0a 2020 2020 2020 2020  ly(df)].        
-0002f6b0: 2020 2020 2020 2020 6466 2e63 6f6c 756d          df.colum
-0002f6c0: 6e73 203d 2064 662e 636f 6c75 6d6e 732e  ns = df.columns.
-0002f6d0: 6173 7479 7065 2869 6e74 290a 2020 2020  astype(int).    
-0002f6e0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-0002f6f0: 4469 6374 203d 2064 6963 7428 290a 2020  Dict = dict().  
-0002f700: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-0002f710: 7461 4469 6374 5b27 656e 7469 7479 275d  taDict['entity']
-0002f720: 203d 206d 6574 6144 665b 274e 616d 6527   = metaDf['Name'
-0002f730: 5d2e 7374 7269 7028 292e 7265 706c 6163  ].strip().replac
-0002f740: 6528 277c 2027 2c20 277c 2729 0a20 2020  e('| ', '|').   
-0002f750: 2020 2020 2020 2020 2020 2020 206d 6574               met
-0002f760: 6144 6963 745b 2763 6174 6567 6f72 7927  aDict['category'
-0002f770: 5d20 3d20 2727 0a20 2020 2020 2020 2020  ] = ''.         
-0002f780: 2020 2020 2020 206d 6574 6144 6963 745b         metaDict[
-0002f790: 2775 6e69 7427 5d20 3d20 6d65 7461 4466  'unit'] = metaDf
-0002f7a0: 5b27 756e 6974 275d 0a20 2020 2020 2020  ['unit'].       
-0002f7b0: 2020 2020 2020 2020 206d 6574 6144 6963           metaDic
-0002f7c0: 745b 2773 6365 6e61 7269 6f27 5d20 3d20  t['scenario'] = 
-0002f7d0: 6d65 7461 4466 5b27 5363 656e 6172 696f  metaDf['Scenario
-0002f7e0: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
-0002f7f0: 2020 206d 6574 6144 6963 745b 2773 6f75     metaDict['sou
-0002f800: 7263 6527 5d20 3d20 7365 6c66 2e73 6574  rce'] = self.set
-0002f810: 7570 2e53 4f55 5243 455f 4944 0a20 2020  up.SOURCE_ID.   
-0002f820: 2020 2020 2020 2020 2020 2020 206d 6574               met
-0002f830: 6144 6963 745b 2775 6e69 7454 6f27 5d20  aDict['unitTo'] 
-0002f840: 3d20 6d65 7461 4466 5b27 756e 6974 546f  = metaDf['unitTo
-0002f850: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
-0002f860: 2020 206d 6574 6144 6963 7420 3d20 6474     metaDict = dt
-0002f870: 2e63 6f72 652e 5f75 7064 6174 655f 6d65  .core._update_me
-0002f880: 7461 286d 6574 6144 6963 7429 0a20 2020  ta(metaDict).   
-0002f890: 2020 2020 2020 2020 2020 2020 2049 4420               ID 
-0002f8a0: 3d20 6474 2e63 6f72 652e 5f63 7265 6174  = dt.core._creat
-0002f8b0: 6544 6174 6162 6173 6549 4428 6d65 7461  eDatabaseID(meta
-0002f8c0: 4469 6374 290a 2020 2020 2020 2020 2020  Dict).          
-0002f8d0: 2020 2020 2020 636f 4953 4f20 3d20 7365        coISO = se
-0002f8e0: 6c66 2e73 7061 7469 616c 4d61 7070 696e  lf.spatialMappin
-0002f8f0: 672e 6c6f 635b 7265 6769 6f6e 2c20 276d  g.loc[region, 'm
-0002f900: 6170 7069 6e67 275d 0a20 2020 2020 2020  apping'].       
-0002f910: 2020 2020 2020 2020 2069 6620 4944 206e           if ID n
-0002f920: 6f74 2069 6e20 7461 626c 6573 546f 436f  ot in tablesToCo
-0002f930: 6d6d 6974 2e6b 6579 7328 293a 0a20 2020  mmit.keys():.   
-0002f940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f950: 2074 6162 6c65 203d 2064 742e 4461 7461   table = dt.Data
-0002f960: 7461 626c 6528 636f 6c75 6d6e 733d 7261  table(columns=ra
-0002f970: 6e67 6528 3230 3030 2c20 3231 3030 292c  nge(2000, 2100),
-0002f980: 206d 6574 613d 6d65 7461 4469 6374 290a   meta=metaDict).
-0002f990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002f9a0: 2020 2020 2074 6162 6c65 2e6c 6f63 5b63       table.loc[c
-0002f9b0: 6f49 534f 2c20 6466 2e63 6f6c 756d 6e73  oISO, df.columns
-0002f9c0: 5d20 3d20 6466 2e76 616c 7565 730a 2020  ] = df.values.  
-0002f9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f9e0: 2020 7461 626c 6573 546f 436f 6d6d 6974    tablesToCommit
-0002f9f0: 2e61 6464 2874 6162 6c65 290a 2020 2020  .add(table).    
-0002fa00: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0002fa10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0002fa20: 2020 2020 2020 7461 626c 6520 3d20 7461        table = ta
-0002fa30: 626c 6573 546f 436f 6d6d 6974 5b49 445d  blesToCommit[ID]
-0002fa40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002fa50: 2020 2020 2074 6162 6c65 2e6c 6f63 5b63       table.loc[c
-0002fa60: 6f49 534f 2c20 6466 2e63 6f6c 756d 6e73  oISO, df.columns
-0002fa70: 5d20 3d20 6466 2e76 616c 7565 730a 0a20  ] = df.values.. 
-0002fa80: 2020 2020 2020 2020 2020 2023 2043 4f32             # CO2
-0002fa90: 2061 6e64 2065 6d69 7373 696f 6e20 696e   and emission in
-0002faa0: 6469 6361 746f 7273 0a0a 2020 2020 2020  dicators..      
-0002fab0: 2020 2020 2020 7365 7475 705b 2773 6865        setup['she
-0002fac0: 6574 4e61 6d65 275d 203d 2072 6567 696f  etName'] = regio
-0002fad0: 6e20 2b20 275f 456c 5f43 4f32 5f49 6e64  n + '_El_CO2_Ind
-0002fae0: 270a 2020 2020 2020 2020 2020 2020 666f  '.            fo
-0002faf0: 7220 692c 2069 6478 2069 6e20 656e 756d  r i, idx in enum
-0002fb00: 6572 6174 6528 6c69 7374 2873 656c 662e  erate(list(self.
-0002fb10: 6d61 7070 696e 6745 6d69 7373 696f 6e73  mappingEmissions
-0002fb20: 2e69 6e64 6578 2929 3a0a 2020 2020 2020  .index)):.      
-0002fb30: 2020 2020 2020 2020 2020 6d65 7461 4466            metaDf
-0002fb40: 203d 2073 656c 662e 6d61 7070 696e 6745   = self.mappingE
-0002fb50: 6d69 7373 696f 6e73 2e6c 6f63 5b69 6478  missions.loc[idx
-0002fb60: 2c20 3a5d 0a20 2020 2020 2020 2020 2020  , :].           
-0002fb70: 2020 2020 2070 7269 6e74 286d 6574 6144       print(metaD
-0002fb80: 665b 2757 6861 7427 5d29 0a0a 2020 2020  f['What'])..    
-0002fb90: 2020 2020 2020 2020 2020 2020 2320 4361              # Ca
-0002fba0: 7061 6369 7479 0a20 2020 2020 2020 2020  pacity.         
-0002fbb0: 2020 2020 2020 2073 6574 7570 5b27 7469         setup['ti
-0002fbc0: 6d65 4964 784c 6973 7427 5d20 3d20 7475  meIdxList'] = tu
-0002fbd0: 706c 6528 6d65 7461 4466 5b27 5469 6d65  ple(metaDf['Time
-0002fbe0: 275d 2e73 706c 6974 2827 3a27 2929 0a20  '].split(':')). 
-0002fbf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0002fc00: 6574 7570 5b27 7370 6163 6549 6478 4c69  etup['spaceIdxLi
-0002fc10: 7374 275d 203d 2074 7570 6c65 285b 6d65  st'] = tuple([me
-0002fc20: 7461 4466 5b27 5768 6174 275d 5d29 0a20  taDf['What']]). 
-0002fc30: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0002fc40: 2070 7269 6e74 286d 6574 6144 665b 636f   print(metaDf[co
-0002fc50: 6e66 6967 2e52 4551 5549 5245 445f 4d45  nfig.REQUIRED_ME
-0002fc60: 5441 5f46 4945 4c44 535d 2e69 736e 756c  TA_FIELDS].isnul
-0002fc70: 6c28 292e 616c 6c28 2920 3d3d 2046 616c  l().all() == Fal
-0002fc80: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
-0002fc90: 2020 2020 2320 7072 696e 7428 6d65 7461      # print(meta
-0002fca0: 4461 7461 5b73 656c 662e 7365 7475 702e  Data[self.setup.
-0002fcb0: 494e 4445 585f 434f 4c55 4d4e 5f4e 414d  INDEX_COLUMN_NAM
-0002fcc0: 455d 290a 0a20 2020 2020 2020 2020 2020  E])..           
-0002fcd0: 2020 2020 2069 6620 6920 3d3d 2030 3a0a       if i == 0:.
-0002fce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002fcf0: 2020 2020 6578 203d 2064 742e 696f 2e45      ex = dt.io.E
-0002fd00: 7863 656c 5265 6164 6572 2873 6574 7570  xcelReader(setup
-0002fd10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0002fd20: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0002fd30: 2020 2020 2020 2061 7364 0a20 2020 2020         asd.     
-0002fd40: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0002fd50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002fd60: 2020 2020 2065 782e 7469 6d65 4964 784c       ex.timeIdxL
-0002fd70: 6973 7420 3d20 5b0a 2020 2020 2020 2020  ist = [.        
+0002e760: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0002e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e780: 2074 6162 6c65 203d 2074 6162 6c65 2e63   table = table.c
+0002e790: 6f6e 7665 7274 2873 656c 662e 6d61 7070  onvert(self.mapp
+0002e7a0: 696e 675b 2775 6e69 7454 6f27 5d5b 7661  ing['unitTo'][va
+0002e7b0: 7269 6162 6c65 5d29 0a0a 2020 2020 2020  riable])..      
+0002e7c0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+0002e7d0: 626c 6549 4420 3d20 6474 2e63 6f72 652e  bleID = dt.core.
+0002e7e0: 5f63 7265 6174 6544 6174 6162 6173 6549  _createDatabaseI
+0002e7f0: 4428 7461 626c 652e 6d65 7461 290a 2020  D(table.meta).  
+0002e800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e810: 2020 7461 626c 6573 546f 436f 6d6d 6974    tablesToCommit
+0002e820: 2e61 7070 656e 6428 7461 626c 6529 0a0a  .append(table)..
+0002e830: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+0002e840: 6162 6c65 7354 6f43 6f6d 6d69 742c 2065  ablesToCommit, e
+0002e850: 7863 6c75 6465 6454 6162 6c65 730a 0a0a  xcludedTables...
+0002e860: 636c 6173 7320 5745 4f28 4261 7365 496d  class WEO(BaseIm
+0002e870: 706f 7274 546f 6f6c 293a 0a20 2020 2022  portTool):.    "
+0002e880: 2222 0a20 2020 2057 454f 2064 6174 6120  "".    WEO data 
+0002e890: 696d 706f 7274 2074 6f6f 6c0a 2020 2020  import tool.    
+0002e8a0: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
+0002e8b0: 6e69 745f 5f28 7365 6c66 2c20 7965 6172  nit__(self, year
+0002e8c0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0002e8d0: 7365 7475 7020 3d20 7365 7475 7053 7472  setup = setupStr
+0002e8e0: 7563 7428 290a 2020 2020 2020 2020 7365  uct().        se
+0002e8f0: 6c66 2e73 6574 7570 2e53 4f55 5243 455f  lf.setup.SOURCE_
+0002e900: 4944 203d 2022 5745 4f5f 2220 2b20 7374  ID = "WEO_" + st
+0002e910: 7228 7965 6172 290a 2020 2020 2020 2020  r(year).        
+0002e920: 7365 6c66 2e73 6574 7570 2e53 4f55 5243  self.setup.SOURC
+0002e930: 455f 5041 5448 203d 206f 732e 7061 7468  E_PATH = os.path
+0002e940: 2e6a 6f69 6e28 0a20 2020 2020 2020 2020  .join(.         
+0002e950: 2020 2063 6f6e 6669 672e 5041 5448 5f54     config.PATH_T
+0002e960: 4f5f 4441 5441 5348 454c 462c 2066 2772  O_DATASHELF, f'r
+0002e970: 6177 6461 7461 2f57 454f 2f7b 7965 6172  awdata/WEO/{year
+0002e980: 7d27 0a20 2020 2020 2020 2029 0a20 2020  }'.        ).   
+0002e990: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
+0002e9a0: 4441 5441 5f46 494c 4520 3d20 6627 5745  DATA_FILE = f'WE
+0002e9b0: 4f7b 7965 6172 7d5f 416e 6e65 7841 2e78  O{year}_AnnexA.x
+0002e9c0: 6c73 7827 0a20 2020 2020 2020 2073 656c  lsx'.        sel
+0002e9d0: 662e 7365 7475 702e 4d41 5050 494e 475f  f.setup.MAPPING_
+0002e9e0: 4649 4c45 203d 206f 732e 7061 7468 2e6a  FILE = os.path.j
+0002e9f0: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
+0002ea00: 2073 656c 662e 7365 7475 702e 534f 5552   self.setup.SOUR
+0002ea10: 4345 5f50 4154 482c 2066 276d 6170 7069  CE_PATH, f'mappi
+0002ea20: 6e67 5f57 454f 5f7b 7965 6172 7d2e 786c  ng_WEO_{year}.xl
+0002ea30: 7378 270a 2020 2020 2020 2020 290a 2020  sx'.        ).  
+0002ea40: 2020 2020 2020 7365 6c66 2e73 6574 7570        self.setup
+0002ea50: 2e4c 4943 454e 4345 203d 2027 4945 4120  .LICENCE = 'IEA 
+0002ea60: 616c 6c20 7269 6768 7473 2072 6573 6572  all rights reser
+0002ea70: 7665 6427 0a20 2020 2020 2020 2073 656c  ved'.        sel
+0002ea80: 662e 7365 7475 702e 5552 4c20 3d20 2768  f.setup.URL = 'h
+0002ea90: 7474 7073 3a2f 2f77 7777 2e69 6561 2e6f  ttps://www.iea.o
+0002eaa0: 7267 2f77 656f 2f27 0a0a 2020 2020 2020  rg/weo/'..      
+0002eab0: 2020 2320 2020 2020 2020 2073 656c 662e    #        self.
+0002eac0: 7365 7475 702e 494e 4445 585f 434f 4c55  setup.INDEX_COLU
+0002ead0: 4d4e 5f4e 414d 4520 3d20 5b27 464c 4f57  MN_NAME = ['FLOW
+0002eae0: 272c 2027 5052 4f44 5543 5427 5d0a 2020  ', 'PRODUCT'].  
+0002eaf0: 2020 2020 2020 2320 2020 2020 2020 2073        #        s
+0002eb00: 656c 662e 7365 7475 702e 5350 4154 4941  elf.setup.SPATIA
+0002eb10: 4c5f 434f 4c55 4d5f 4e41 4d45 203d 2027  L_COLUM_NAME = '
+0002eb20: 434f 554e 5452 5927 0a20 2020 2020 2020  COUNTRY'.       
+0002eb30: 2023 2020 2020 2020 2020 7365 6c66 2e73   #        self.s
+0002eb40: 6574 7570 2e43 4f4c 554d 4e53 5f54 4f5f  etup.COLUMNS_TO_
+0002eb50: 4452 4f50 203d 205b 2027 5052 4f44 5543  DROP = [ 'PRODUC
+0002eb60: 5427 2c27 464c 4f57 272c 2763 6f6d 6269  T','FLOW','combi
+0002eb70: 6e65 6427 5d0a 0a20 2020 2020 2020 2069  ned']..        i
+0002eb80: 6620 6e6f 7420 286f 732e 7061 7468 2e65  f not (os.path.e
+0002eb90: 7869 7374 7328 7365 6c66 2e73 6574 7570  xists(self.setup
+0002eba0: 2e4d 4150 5049 4e47 5f46 494c 4529 293a  .MAPPING_FILE)):
+0002ebb0: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+0002ebc0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0002ebd0: 7265 6174 6556 6172 6961 626c 654d 6170  reateVariableMap
+0002ebe0: 7069 6e67 2829 0a20 2020 2020 2020 2020  ping().         
+0002ebf0: 2020 2070 7269 6e74 2822 6e6f 206d 6170     print("no map
+0002ec00: 7069 6e67 2066 696c 6520 666f 756e 6422  ping file found"
+0002ec10: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0002ec20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002ec30: 2e6d 6170 7069 6e67 456e 6572 6779 203d  .mappingEnergy =
+0002ec40: 2070 642e 7265 6164 5f65 7863 656c 280a   pd.read_excel(.
+0002ec50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ec60: 7365 6c66 2e73 6574 7570 2e4d 4150 5049  self.setup.MAPPI
+0002ec70: 4e47 5f46 494c 452c 2073 6865 6574 5f6e  NG_FILE, sheet_n
+0002ec80: 616d 653d 2745 6e65 7267 795f 4261 6c61  ame='Energy_Bala
+0002ec90: 6e63 6527 0a20 2020 2020 2020 2020 2020  nce'.           
+0002eca0: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
+0002ecb0: 656c 662e 6d61 7070 696e 6745 6d69 7373  elf.mappingEmiss
+0002ecc0: 696f 6e73 203d 2070 642e 7265 6164 5f65  ions = pd.read_e
+0002ecd0: 7863 656c 280a 2020 2020 2020 2020 2020  xcel(.          
+0002ece0: 2020 2020 2020 7365 6c66 2e73 6574 7570        self.setup
+0002ecf0: 2e4d 4150 5049 4e47 5f46 494c 452c 2073  .MAPPING_FILE, s
+0002ed00: 6865 6574 5f6e 616d 653d 2753 495f 434f  heet_name='SI_CO
+0002ed10: 325f 496e 6427 0a20 2020 2020 2020 2020  2_Ind'.         
+0002ed20: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+0002ed30: 2020 7365 6c66 2e73 7061 7469 616c 4d61    self.spatialMa
+0002ed40: 7070 696e 6720 3d20 7064 2e72 6561 645f  pping = pd.read_
+0002ed50: 6578 6365 6c28 0a20 2020 2020 2020 2020  excel(.         
+0002ed60: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
+0002ed70: 702e 4d41 5050 494e 475f 4649 4c45 2c20  p.MAPPING_FILE, 
+0002ed80: 7368 6565 745f 6e61 6d65 3d27 7370 6174  sheet_name='spat
+0002ed90: 6961 6c27 0a20 2020 2020 2020 2020 2020  ial'.           
+0002eda0: 2029 0a0a 2020 2020 2020 2020 7365 6c66   )..        self
+0002edb0: 2e63 7265 6174 6553 6f75 7263 654d 6574  .createSourceMet
+0002edc0: 6128 290a 0a20 2020 2064 6566 2061 6464  a()..    def add
+0002edd0: 5370 6174 6961 6c4d 6170 7069 6e67 2873  SpatialMapping(s
+0002ede0: 656c 6629 3a0a 2020 2020 2020 2020 2320  elf):.        # 
+0002edf0: 4555 0a20 2020 2020 2020 206d 6170 7069  EU.        mappi
+0002ee00: 6e67 546f 436f 756e 7472 6965 7320 3d20  ngToCountries = 
+0002ee10: 6469 6374 2829 0a20 2020 2020 2020 2023  dict().        #
+0002ee20: 2073 656c 662e 7370 6174 6961 6c4d 6170   self.spatialMap
+0002ee30: 7069 6e67 2e6c 6f63 5b27 4d65 6d6f 3a20  ping.loc['Memo: 
+0002ee40: 4575 726f 7065 616e 2055 6e69 6f6e 2d32  European Union-2
+0002ee50: 3827 5d20 3d20 2745 5532 3827 0a20 2020  8'] = 'EU28'.   
+0002ee60: 2020 2020 206d 6170 7069 6e67 546f 436f       mappingToCo
+0002ee70: 756e 7472 6965 735b 2741 5345 414e 275d  untries['ASEAN']
+0002ee80: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+0002ee90: 2027 564e 4d27 2c0a 2020 2020 2020 2020   'VNM',.        
+0002eea0: 2020 2020 2750 484c 272c 0a20 2020 2020      'PHL',.     
+0002eeb0: 2020 2020 2020 2027 5448 4127 2c0a 2020         'THA',.  
+0002eec0: 2020 2020 2020 2020 2020 2753 4750 272c            'SGP',
+0002eed0: 0a20 2020 2020 2020 2020 2020 2027 4d4d  .            'MM
+0002eee0: 5227 2c0a 2020 2020 2020 2020 2020 2020  R',.            
+0002eef0: 2749 444e 272c 0a20 2020 2020 2020 2020  'IDN',.         
+0002ef00: 2020 2027 4b48 4d27 2c0a 2020 2020 2020     'KHM',.      
+0002ef10: 2020 2020 2020 2742 524e 272c 0a20 2020        'BRN',.   
+0002ef20: 2020 2020 2020 2020 2027 4d59 5327 2c0a           'MYS',.
+0002ef30: 2020 2020 2020 2020 2020 2020 274c 414f              'LAO
+0002ef40: 272c 0a20 2020 2020 2020 205d 0a20 2020  ',.        ].   
+0002ef50: 2020 2020 2064 742e 6d61 7070 2e72 6567       dt.mapp.reg
+0002ef60: 696f 6e73 2e61 6464 5265 6769 6f6e 546f  ions.addRegionTo
+0002ef70: 436f 6e74 6578 7428 2757 454f 272c 206d  Context('WEO', m
+0002ef80: 6170 7069 6e67 546f 436f 756e 7472 6965  appingToCountrie
+0002ef90: 7329 0a0a 2020 2020 6465 6620 6761 7468  s)..    def gath
+0002efa0: 6572 4d61 7070 6564 4461 7461 2873 656c  erMappedData(sel
+0002efb0: 662c 2073 7061 7469 616c 5375 6253 6574  f, spatialSubSet
+0002efc0: 3d4e 6f6e 6529 3a0a 0a20 2020 2020 2020  =None):..       
+0002efd0: 2074 6162 6c65 7354 6f43 6f6d 6d69 7420   tablesToCommit 
+0002efe0: 3d20 6474 2e54 6162 6c65 5365 7428 290a  = dt.TableSet().
+0002eff0: 2020 2020 2020 2020 7365 7475 7020 3d20          setup = 
+0002f000: 6469 6374 2829 0a20 2020 2020 2020 2073  dict().        s
+0002f010: 6574 7570 5b27 6669 6c65 5061 7468 275d  etup['filePath']
+0002f020: 203d 2073 656c 662e 7365 7475 702e 534f   = self.setup.SO
+0002f030: 5552 4345 5f50 4154 480a 2020 2020 2020  URCE_PATH.      
+0002f040: 2020 7365 7475 705b 2766 696c 654e 616d    setup['fileNam
+0002f050: 6527 5d20 3d20 7365 6c66 2e73 6574 7570  e'] = self.setup
+0002f060: 2e44 4154 415f 4649 4c45 0a0a 2020 2020  .DATA_FILE..    
+0002f070: 2020 2020 2320 6c6f 6f70 206f 7665 7220      # loop over 
+0002f080: 656e 6572 6779 206d 6170 7069 6e67 0a20  energy mapping. 
+0002f090: 2020 2020 2020 2066 6f72 2072 6567 696f         for regio
+0002f0a0: 6e20 696e 2073 656c 662e 7370 6174 6961  n in self.spatia
+0002f0b0: 6c4d 6170 7069 6e67 2e69 6e64 6578 3a0a  lMapping.index:.
+0002f0c0: 2020 2020 2020 2020 2020 2020 7365 7475              setu
+0002f0d0: 705b 2773 6865 6574 4e61 6d65 275d 203d  p['sheetName'] =
+0002f0e0: 2072 6567 696f 6e20 2b20 275f 4261 6c61   region + '_Bala
+0002f0f0: 6e63 6527 0a20 2020 2020 2020 2020 2020  nce'.           
+0002f100: 2066 6f72 2069 2c20 6964 7820 696e 2065   for i, idx in e
+0002f110: 6e75 6d65 7261 7465 286c 6973 7428 7365  numerate(list(se
+0002f120: 6c66 2e6d 6170 7069 6e67 456e 6572 6779  lf.mappingEnergy
+0002f130: 2e69 6e64 6578 2929 3a0a 2020 2020 2020  .index)):.      
+0002f140: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+0002f150: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0002f160: 2869 290a 2020 2020 2020 2020 2020 2020  (i).            
+0002f170: 2020 2020 6d65 7461 4466 203d 2073 656c      metaDf = sel
+0002f180: 662e 6d61 7070 696e 6745 6e65 7267 792e  f.mappingEnergy.
+0002f190: 6c6f 635b 6964 782c 203a 5d0a 2020 2020  loc[idx, :].    
+0002f1a0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0002f1b0: 7428 6d65 7461 4466 5b27 5768 6174 275d  t(metaDf['What']
+0002f1c0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+0002f1d0: 2020 2023 2043 6170 6163 6974 790a 2020     # Capacity.  
+0002f1e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0002f1f0: 7475 705b 2774 696d 6549 6478 4c69 7374  tup['timeIdxList
+0002f200: 275d 203d 2074 7570 6c65 286d 6574 6144  '] = tuple(metaD
+0002f210: 665b 2754 696d 6527 5d2e 7370 6c69 7428  f['Time'].split(
+0002f220: 273a 2729 290a 2020 2020 2020 2020 2020  ':')).          
+0002f230: 2020 2020 2020 7365 7475 705b 2773 7061        setup['spa
+0002f240: 6365 4964 784c 6973 7427 5d20 3d20 7475  ceIdxList'] = tu
+0002f250: 706c 6528 5b6d 6574 6144 665b 2757 6861  ple([metaDf['Wha
+0002f260: 7427 5d5d 290a 2020 2020 2020 2020 2020  t']]).          
+0002f270: 2020 2020 2020 2320 7072 696e 7428 6d65        # print(me
+0002f280: 7461 4466 5b63 6f6e 6669 672e 5245 5155  taDf[config.REQU
+0002f290: 4952 4544 5f4d 4554 415f 4649 454c 4453  IRED_META_FIELDS
+0002f2a0: 5d2e 6973 6e75 6c6c 2829 2e61 6c6c 2829  ].isnull().all()
+0002f2b0: 203d 3d20 4661 6c73 6529 0a20 2020 2020   == False).     
+0002f2c0: 2020 2020 2020 2020 2020 2023 2070 7269             # pri
+0002f2d0: 6e74 286d 6574 6144 6174 615b 7365 6c66  nt(metaData[self
+0002f2e0: 2e73 6574 7570 2e49 4e44 4558 5f43 4f4c  .setup.INDEX_COL
+0002f2f0: 554d 4e5f 4e41 4d45 5d29 0a0a 2020 2020  UMN_NAME])..    
+0002f300: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0002f310: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+0002f320: 2020 2020 2020 2020 2020 2065 7820 3d20             ex = 
+0002f330: 6474 2e69 6f2e 4578 6365 6c52 6561 6465  dt.io.ExcelReade
+0002f340: 7228 7365 7475 7029 0a20 2020 2020 2020  r(setup).       
+0002f350: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0002f360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f370: 2020 2065 782e 7469 6d65 4964 784c 6973     ex.timeIdxLis
+0002f380: 7420 3d20 5b0a 2020 2020 2020 2020 2020  t = [.          
+0002f390: 2020 2020 2020 2020 2020 2020 2020 6474                dt
+0002f3a0: 2e69 6f2e 6578 6365 6c49 6478 3250 616e  .io.excelIdx2Pan
+0002f3b0: 6461 7349 6478 2878 2920 666f 7220 7820  dasIdx(x) for x 
+0002f3c0: 696e 2073 6574 7570 5b27 7469 6d65 4964  in setup['timeId
+0002f3d0: 784c 6973 7427 5d0a 2020 2020 2020 2020  xList'].        
+0002f3e0: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+0002f3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f400: 2020 6578 2e73 7061 6365 4964 784c 6973    ex.spaceIdxLis
+0002f410: 7420 3d20 5b0a 2020 2020 2020 2020 2020  t = [.          
+0002f420: 2020 2020 2020 2020 2020 2020 2020 6474                dt
+0002f430: 2e69 6f2e 6578 6365 6c49 6478 3250 616e  .io.excelIdx2Pan
+0002f440: 6461 7349 6478 2878 2920 666f 7220 7820  dasIdx(x) for x 
+0002f450: 696e 2073 6574 7570 5b27 7370 6163 6549  in setup['spaceI
+0002f460: 6478 4c69 7374 275d 0a20 2020 2020 2020  dxList'].       
+0002f470: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
+0002f480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f490: 2020 2023 2070 7269 6e74 2865 782e 6466     # print(ex.df
+0002f4a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0002f4b0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0002f4c0: 2020 2069 6620 2249 6e74 6572 6e61 7469     if "Internati
+0002f4d0: 6f6e 616c 2220 696e 206d 6574 6144 665b  onal" in metaDf[
+0002f4e0: 274e 616d 6527 5d3a 0a20 2020 2020 2020  'Name']:.       
+0002f4f0: 2020 2020 2020 2020 2023 2020 2020 2020           #      
+0002f500: 2020 2020 2020 2020 2020 2020 2020 7364                sd
+0002f510: 660a 2020 2020 2020 2020 2020 2020 2020  f.              
+0002f520: 2020 6966 2065 782e 7370 6163 6549 6478    if ex.spaceIdx
+0002f530: 4c69 7374 5b30 5d5b 305d 203e 2034 3120  List[0][0] > 41 
+0002f540: 616e 6420 7265 6769 6f6e 2021 3d20 2757  and region != 'W
+0002f550: 6f72 6c64 273a 0a20 2020 2020 2020 2020  orld':.         
+0002f560: 2020 2020 2020 2020 2020 2065 782e 7370             ex.sp
+0002f570: 6163 6549 6478 4c69 7374 203d 205b 2865  aceIdxList = [(e
+0002f580: 782e 7370 6163 6549 6478 4c69 7374 5b30  x.spaceIdxList[0
+0002f590: 5d5b 305d 202d 2031 2c20 3029 5d0a 0a20  ][0] - 1, 0)].. 
+0002f5a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0002f5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f5c0: 7072 696e 7428 6578 2e73 6574 7570 2829  print(ex.setup()
+0002f5d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0002f5e0: 2020 6966 2069 203d 3d20 303a 0a20 2020    if i == 0:.   
+0002f5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f600: 2064 6620 3d20 6578 2e67 6174 6865 7244   df = ex.gatherD
+0002f610: 6174 6128 290a 2020 2020 2020 2020 2020  ata().          
+0002f620: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0002f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f640: 6466 203d 2065 782e 6761 7468 6572 4461  df = ex.gatherDa
+0002f650: 7461 286c 6f61 643d 4661 6c73 6529 0a20  ta(load=False). 
+0002f660: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0002f670: 7269 6e74 2864 6629 0a20 2020 2020 2020  rint(df).       
+0002f680: 2020 2020 2020 2020 2064 6620 3d20 6466           df = df
+0002f690: 2e6c 6f63 5b3a 2c20 7965 6172 7343 6f6c  .loc[:, yearsCol
+0002f6a0: 756d 6e73 4f6e 6c79 2864 6629 5d0a 2020  umnsOnly(df)].  
+0002f6b0: 2020 2020 2020 2020 2020 2020 2020 6466                df
+0002f6c0: 2e63 6f6c 756d 6e73 203d 2064 662e 636f  .columns = df.co
+0002f6d0: 6c75 6d6e 732e 6173 7479 7065 2869 6e74  lumns.astype(int
+0002f6e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0002f6f0: 2020 6d65 7461 4469 6374 203d 2064 6963    metaDict = dic
+0002f700: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+0002f710: 2020 2020 6d65 7461 4469 6374 5b27 656e      metaDict['en
+0002f720: 7469 7479 275d 203d 206d 6574 6144 665b  tity'] = metaDf[
+0002f730: 274e 616d 6527 5d2e 7374 7269 7028 292e  'Name'].strip().
+0002f740: 7265 706c 6163 6528 277c 2027 2c20 277c  replace('| ', '|
+0002f750: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+0002f760: 2020 206d 6574 6144 6963 745b 2763 6174     metaDict['cat
+0002f770: 6567 6f72 7927 5d20 3d20 2727 0a20 2020  egory'] = ''.   
+0002f780: 2020 2020 2020 2020 2020 2020 206d 6574               met
+0002f790: 6144 6963 745b 2775 6e69 7427 5d20 3d20  aDict['unit'] = 
+0002f7a0: 6d65 7461 4466 5b27 756e 6974 275d 0a20  metaDf['unit']. 
+0002f7b0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0002f7c0: 6574 6144 6963 745b 2773 6365 6e61 7269  etaDict['scenari
+0002f7d0: 6f27 5d20 3d20 6d65 7461 4466 5b27 5363  o'] = metaDf['Sc
+0002f7e0: 656e 6172 696f 275d 0a20 2020 2020 2020  enario'].       
+0002f7f0: 2020 2020 2020 2020 206d 6574 6144 6963           metaDic
+0002f800: 745b 2773 6f75 7263 6527 5d20 3d20 7365  t['source'] = se
+0002f810: 6c66 2e73 6574 7570 2e53 4f55 5243 455f  lf.setup.SOURCE_
+0002f820: 4944 0a20 2020 2020 2020 2020 2020 2020  ID.             
+0002f830: 2020 206d 6574 6144 6963 745b 2775 6e69     metaDict['uni
+0002f840: 7454 6f27 5d20 3d20 6d65 7461 4466 5b27  tTo'] = metaDf['
+0002f850: 756e 6974 546f 275d 0a20 2020 2020 2020  unitTo'].       
+0002f860: 2020 2020 2020 2020 206d 6574 6144 6963           metaDic
+0002f870: 7420 3d20 6474 2e63 6f72 652e 5f75 7064  t = dt.core._upd
+0002f880: 6174 655f 6d65 7461 286d 6574 6144 6963  ate_meta(metaDic
+0002f890: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+0002f8a0: 2020 2049 4420 3d20 6474 2e63 6f72 652e     ID = dt.core.
+0002f8b0: 5f63 7265 6174 6544 6174 6162 6173 6549  _createDatabaseI
+0002f8c0: 4428 6d65 7461 4469 6374 290a 2020 2020  D(metaDict).    
+0002f8d0: 2020 2020 2020 2020 2020 2020 636f 4953              coIS
+0002f8e0: 4f20 3d20 7365 6c66 2e73 7061 7469 616c  O = self.spatial
+0002f8f0: 4d61 7070 696e 672e 6c6f 635b 7265 6769  Mapping.loc[regi
+0002f900: 6f6e 2c20 276d 6170 7069 6e67 275d 0a20  on, 'mapping']. 
+0002f910: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0002f920: 6620 4944 206e 6f74 2069 6e20 7461 626c  f ID not in tabl
+0002f930: 6573 546f 436f 6d6d 6974 2e6b 6579 7328  esToCommit.keys(
+0002f940: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0002f950: 2020 2020 2020 2074 6162 6c65 203d 2064         table = d
+0002f960: 742e 4461 7461 7461 626c 6528 636f 6c75  t.Datatable(colu
+0002f970: 6d6e 733d 7261 6e67 6528 3230 3030 2c20  mns=range(2000, 
+0002f980: 3231 3030 292c 206d 6574 613d 6d65 7461  2100), meta=meta
+0002f990: 4469 6374 290a 0a20 2020 2020 2020 2020  Dict)..         
+0002f9a0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+0002f9b0: 2e6c 6f63 5b63 6f49 534f 2c20 6466 2e63  .loc[coISO, df.c
+0002f9c0: 6f6c 756d 6e73 5d20 3d20 6466 2e76 616c  olumns] = df.val
+0002f9d0: 7565 730a 2020 2020 2020 2020 2020 2020  ues.            
+0002f9e0: 2020 2020 2020 2020 7461 626c 6573 546f          tablesTo
+0002f9f0: 436f 6d6d 6974 2e61 6464 2874 6162 6c65  Commit.add(table
+0002fa00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0002fa10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0002fa20: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
+0002fa30: 6520 3d20 7461 626c 6573 546f 436f 6d6d  e = tablesToComm
+0002fa40: 6974 5b49 445d 0a20 2020 2020 2020 2020  it[ID].         
+0002fa50: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+0002fa60: 2e6c 6f63 5b63 6f49 534f 2c20 6466 2e63  .loc[coISO, df.c
+0002fa70: 6f6c 756d 6e73 5d20 3d20 6466 2e76 616c  olumns] = df.val
+0002fa80: 7565 730a 0a20 2020 2020 2020 2020 2020  ues..           
+0002fa90: 2023 2043 4f32 2061 6e64 2065 6d69 7373   # CO2 and emiss
+0002faa0: 696f 6e20 696e 6469 6361 746f 7273 0a0a  ion indicators..
+0002fab0: 2020 2020 2020 2020 2020 2020 7365 7475              setu
+0002fac0: 705b 2773 6865 6574 4e61 6d65 275d 203d  p['sheetName'] =
+0002fad0: 2072 6567 696f 6e20 2b20 275f 456c 5f43   region + '_El_C
+0002fae0: 4f32 5f49 6e64 270a 2020 2020 2020 2020  O2_Ind'.        
+0002faf0: 2020 2020 666f 7220 692c 2069 6478 2069      for i, idx i
+0002fb00: 6e20 656e 756d 6572 6174 6528 6c69 7374  n enumerate(list
+0002fb10: 2873 656c 662e 6d61 7070 696e 6745 6d69  (self.mappingEmi
+0002fb20: 7373 696f 6e73 2e69 6e64 6578 2929 3a0a  ssions.index)):.
+0002fb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002fb40: 6d65 7461 4466 203d 2073 656c 662e 6d61  metaDf = self.ma
+0002fb50: 7070 696e 6745 6d69 7373 696f 6e73 2e6c  ppingEmissions.l
+0002fb60: 6f63 5b69 6478 2c20 3a5d 0a20 2020 2020  oc[idx, :].     
+0002fb70: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0002fb80: 286d 6574 6144 665b 2757 6861 7427 5d29  (metaDf['What'])
+0002fb90: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0002fba0: 2020 2320 4361 7061 6369 7479 0a20 2020    # Capacity.   
+0002fbb0: 2020 2020 2020 2020 2020 2020 2073 6574               set
+0002fbc0: 7570 5b27 7469 6d65 4964 784c 6973 7427  up['timeIdxList'
+0002fbd0: 5d20 3d20 7475 706c 6528 6d65 7461 4466  ] = tuple(metaDf
+0002fbe0: 5b27 5469 6d65 275d 2e73 706c 6974 2827  ['Time'].split('
+0002fbf0: 3a27 2929 0a20 2020 2020 2020 2020 2020  :')).           
+0002fc00: 2020 2020 2073 6574 7570 5b27 7370 6163       setup['spac
+0002fc10: 6549 6478 4c69 7374 275d 203d 2074 7570  eIdxList'] = tup
+0002fc20: 6c65 285b 6d65 7461 4466 5b27 5768 6174  le([metaDf['What
+0002fc30: 275d 5d29 0a20 2020 2020 2020 2020 2020  ']]).           
+0002fc40: 2020 2020 2023 2070 7269 6e74 286d 6574       # print(met
+0002fc50: 6144 665b 636f 6e66 6967 2e52 4551 5549  aDf[config.REQUI
+0002fc60: 5245 445f 4d45 5441 5f46 4945 4c44 535d  RED_META_FIELDS]
+0002fc70: 2e69 736e 756c 6c28 292e 616c 6c28 2920  .isnull().all() 
+0002fc80: 3d3d 2046 616c 7365 290a 2020 2020 2020  == False).      
+0002fc90: 2020 2020 2020 2020 2020 2320 7072 696e            # prin
+0002fca0: 7428 6d65 7461 4461 7461 5b73 656c 662e  t(metaData[self.
+0002fcb0: 7365 7475 702e 494e 4445 585f 434f 4c55  setup.INDEX_COLU
+0002fcc0: 4d4e 5f4e 414d 455d 290a 0a20 2020 2020  MN_NAME])..     
+0002fcd0: 2020 2020 2020 2020 2020 2069 6620 6920             if i 
+0002fce0: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+0002fcf0: 2020 2020 2020 2020 2020 6578 203d 2064            ex = d
+0002fd00: 742e 696f 2e45 7863 656c 5265 6164 6572  t.io.ExcelReader
+0002fd10: 2873 6574 7570 290a 2020 2020 2020 2020  (setup).        
+0002fd20: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0002fd30: 2020 2020 2020 2020 2020 2020 2061 7364               asd
+0002fd40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002fd50: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0002fd60: 2020 2020 2020 2020 2020 2065 782e 7469             ex.ti
+0002fd70: 6d65 4964 784c 6973 7420 3d20 5b0a 2020  meIdxList = [.  
 0002fd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002fd90: 6474 2e69 6f2e 6578 6365 6c49 6478 3250  dt.io.excelIdx2P
-0002fda0: 616e 6461 7349 6478 2878 2920 666f 7220  andasIdx(x) for 
-0002fdb0: 7820 696e 2073 6574 7570 5b27 7469 6d65  x in setup['time
-0002fdc0: 4964 784c 6973 7427 5d0a 2020 2020 2020  IdxList'].      
-0002fdd0: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
-0002fde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002fdf0: 2020 2020 6578 2e73 7061 6365 4964 784c      ex.spaceIdxL
-0002fe00: 6973 7420 3d20 5b0a 2020 2020 2020 2020  ist = [.        
+0002fd90: 2020 2020 2020 6474 2e69 6f2e 6578 6365        dt.io.exce
+0002fda0: 6c49 6478 3250 616e 6461 7349 6478 2878  lIdx2PandasIdx(x
+0002fdb0: 2920 666f 7220 7820 696e 2073 6574 7570  ) for x in setup
+0002fdc0: 5b27 7469 6d65 4964 784c 6973 7427 5d0a  ['timeIdxList'].
+0002fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002fde0: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+0002fdf0: 2020 2020 2020 2020 2020 6578 2e73 7061            ex.spa
+0002fe00: 6365 4964 784c 6973 7420 3d20 5b0a 2020  ceIdxList = [.  
 0002fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002fe20: 6474 2e69 6f2e 6578 6365 6c49 6478 3250  dt.io.excelIdx2P
-0002fe30: 616e 6461 7349 6478 2878 2920 666f 7220  andasIdx(x) for 
-0002fe40: 7820 696e 2073 6574 7570 5b27 7370 6163  x in setup['spac
-0002fe50: 6549 6478 4c69 7374 275d 0a20 2020 2020  eIdxList'].     
-0002fe60: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-0002fe70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002fe80: 2023 2020 2020 2020 2020 2020 2020 2020   #              
-0002fe90: 2020 6966 2022 496e 7465 726e 6174 696f    if "Internatio
-0002fea0: 6e61 6c22 2069 6e20 6d65 7461 4466 5b27  nal" in metaDf['
-0002feb0: 4e61 6d65 275d 3a0a 2020 2020 2020 2020  Name']:.        
-0002fec0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0002fed0: 2020 2020 2020 2020 2020 2020 2073 6466               sdf
-0002fee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002fef0: 2069 6620 6578 2e73 7061 6365 4964 784c   if ex.spaceIdxL
-0002ff00: 6973 745b 305d 5b30 5d20 3e20 3531 2061  ist[0][0] > 51 a
-0002ff10: 6e64 2072 6567 696f 6e20 213d 2027 576f  nd region != 'Wo
-0002ff20: 726c 6427 3a0a 2020 2020 2020 2020 2020  rld':.          
-0002ff30: 2020 2020 2020 2020 2020 6578 2e73 7061            ex.spa
-0002ff40: 6365 4964 784c 6973 7420 3d20 5b28 6578  ceIdxList = [(ex
-0002ff50: 2e73 7061 6365 4964 784c 6973 745b 305d  .spaceIdxList[0]
-0002ff60: 5b30 5d20 2d20 312c 2030 295d 0a0a 2020  [0] - 1, 0)]..  
-0002ff70: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0002ff80: 2069 203d 3d20 303a 0a20 2020 2020 2020   i == 0:.       
-0002ff90: 2020 2020 2020 2020 2020 2020 2064 6620               df 
-0002ffa0: 3d20 6578 2e67 6174 6865 7244 6174 6128  = ex.gatherData(
-0002ffb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0002ffc0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0002ffd0: 2020 2020 2020 2020 2020 2020 6466 203d              df =
-0002ffe0: 2065 782e 6761 7468 6572 4461 7461 286c   ex.gatherData(l
-0002fff0: 6f61 643d 4661 6c73 6529 0a20 2020 2020  oad=False).     
-00030000: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00030010: 2864 6629 0a20 2020 2020 2020 2020 2020  (df).           
-00030020: 2020 2020 2064 6620 3d20 6466 2e6c 6f63       df = df.loc
-00030030: 5b3a 2c20 7965 6172 7343 6f6c 756d 6e73  [:, yearsColumns
-00030040: 4f6e 6c79 2864 6629 5d0a 2020 2020 2020  Only(df)].      
-00030050: 2020 2020 2020 2020 2020 6466 2e63 6f6c            df.col
-00030060: 756d 6e73 203d 2064 662e 636f 6c75 6d6e  umns = df.column
-00030070: 732e 6173 7479 7065 2869 6e74 290a 2020  s.astype(int).  
-00030080: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00030090: 7461 4469 6374 203d 2064 6963 7428 290a  taDict = dict().
-000300a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000300b0: 6d65 7461 4469 6374 5b27 656e 7469 7479  metaDict['entity
-000300c0: 275d 203d 206d 6574 6144 665b 274e 616d  '] = metaDf['Nam
-000300d0: 6527 5d2e 7374 7269 7028 292e 7265 706c  e'].strip().repl
-000300e0: 6163 6528 277c 2027 2c20 277c 2729 0a20  ace('| ', '|'). 
-000300f0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00030100: 6574 6144 6963 745b 2763 6174 6567 6f72  etaDict['categor
-00030110: 7927 5d20 3d20 2727 0a20 2020 2020 2020  y'] = ''.       
-00030120: 2020 2020 2020 2020 206d 6574 6144 6963           metaDic
-00030130: 745b 2775 6e69 7427 5d20 3d20 6d65 7461  t['unit'] = meta
-00030140: 4466 5b27 756e 6974 275d 0a20 2020 2020  Df['unit'].     
-00030150: 2020 2020 2020 2020 2020 206d 6574 6144             metaD
-00030160: 6963 745b 2773 6365 6e61 7269 6f27 5d20  ict['scenario'] 
-00030170: 3d20 6d65 7461 4466 5b27 5363 656e 6172  = metaDf['Scenar
-00030180: 696f 275d 0a20 2020 2020 2020 2020 2020  io'].           
-00030190: 2020 2020 206d 6574 6144 6963 745b 2773       metaDict['s
-000301a0: 6f75 7263 6527 5d20 3d20 7365 6c66 2e73  ource'] = self.s
-000301b0: 6574 7570 2e53 4f55 5243 455f 4944 0a20  etup.SOURCE_ID. 
-000301c0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000301d0: 6574 6144 6963 745b 2775 6e69 7454 6f27  etaDict['unitTo'
-000301e0: 5d20 3d20 6d65 7461 4466 5b27 756e 6974  ] = metaDf['unit
-000301f0: 546f 275d 0a0a 2020 2020 2020 2020 2020  To']..          
-00030200: 2020 2020 2020 6d65 7461 4469 6374 203d        metaDict =
-00030210: 2064 742e 636f 7265 2e5f 7570 6461 7465   dt.core._update
-00030220: 5f6d 6574 6128 6d65 7461 4469 6374 290a  _meta(metaDict).
-00030230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030240: 4944 203d 2064 742e 636f 7265 2e5f 6372  ID = dt.core._cr
-00030250: 6561 7465 4461 7461 6261 7365 4944 286d  eateDatabaseID(m
-00030260: 6574 6144 6963 7429 0a20 2020 2020 2020  etaDict).       
-00030270: 2020 2020 2020 2020 2063 6f49 534f 203d           coISO =
-00030280: 2073 656c 662e 7370 6174 6961 6c4d 6170   self.spatialMap
-00030290: 7069 6e67 2e6c 6f63 5b72 6567 696f 6e2c  ping.loc[region,
-000302a0: 2027 6d61 7070 696e 6727 5d0a 2020 2020   'mapping'].    
-000302b0: 2020 2020 2020 2020 2020 2020 6966 2049              if I
-000302c0: 4420 6e6f 7420 696e 2074 6162 6c65 7354  D not in tablesT
-000302d0: 6f43 6f6d 6d69 742e 6b65 7973 2829 3a0a  oCommit.keys():.
-000302e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000302f0: 2020 2020 7461 626c 6520 3d20 6474 2e44      table = dt.D
-00030300: 6174 6174 6162 6c65 2863 6f6c 756d 6e73  atatable(columns
-00030310: 3d72 616e 6765 2832 3030 302c 2032 3130  =range(2000, 210
-00030320: 3029 2c20 6d65 7461 3d6d 6574 6144 6963  0), meta=metaDic
-00030330: 7429 0a0a 2020 2020 2020 2020 2020 2020  t)..            
-00030340: 2020 2020 2020 2020 7461 626c 652e 6c6f          table.lo
-00030350: 635b 636f 4953 4f2c 2064 662e 636f 6c75  c[coISO, df.colu
-00030360: 6d6e 735d 203d 2064 662e 7661 6c75 6573  mns] = df.values
-00030370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00030380: 2020 2020 2074 6162 6c65 7354 6f43 6f6d       tablesToCom
-00030390: 6d69 742e 6164 6428 7461 626c 6529 0a20  mit.add(table). 
-000303a0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000303b0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000303c0: 2020 2020 2020 2020 2074 6162 6c65 203d           table =
-000303d0: 2074 6162 6c65 7354 6f43 6f6d 6d69 745b   tablesToCommit[
-000303e0: 4944 5d0a 2020 2020 2020 2020 2020 2020  ID].            
-000303f0: 2020 2020 2020 2020 7461 626c 652e 6c6f          table.lo
-00030400: 635b 636f 4953 4f2c 2064 662e 636f 6c75  c[coISO, df.colu
-00030410: 6d6e 735d 203d 2064 662e 7661 6c75 6573  mns] = df.values
-00030420: 0a0a 2020 2020 2020 2020 7461 626c 6573  ..        tables
-00030430: 4c69 7374 203d 206c 6973 7428 290a 2020  List = list().  
-00030440: 2020 2020 2020 666f 7220 4944 2069 6e20        for ID in 
-00030450: 7461 626c 6573 546f 436f 6d6d 6974 2e6b  tablesToCommit.k
-00030460: 6579 7328 293a 0a20 2020 2020 2020 2020  eys():.         
-00030470: 2020 2064 6174 6154 6162 6c65 203d 2074     dataTable = t
-00030480: 6162 6c65 7354 6f43 6f6d 6d69 745b 4944  ablesToCommit[ID
-00030490: 5d0a 2020 2020 2020 2020 2020 2020 7072  ].            pr
-000304a0: 696e 7428 6461 7461 5461 626c 652e 6d65  int(dataTable.me
-000304b0: 7461 290a 2020 2020 2020 2020 2020 2020  ta).            
-000304c0: 6966 206e 6f74 2070 642e 6973 6e61 2864  if not pd.isna(d
-000304d0: 6174 6154 6162 6c65 2e6d 6574 615b 2775  ataTable.meta['u
-000304e0: 6e69 7454 6f27 5d29 3a0a 2020 2020 2020  nitTo']):.      
-000304f0: 2020 2020 2020 2020 2020 6461 7461 5461            dataTa
-00030500: 626c 6520 3d20 6461 7461 5461 626c 652e  ble = dataTable.
-00030510: 636f 6e76 6572 7428 6461 7461 5461 626c  convert(dataTabl
-00030520: 652e 6d65 7461 5b27 756e 6974 546f 275d  e.meta['unitTo']
-00030530: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00030540: 2020 6465 6c20 6461 7461 5461 626c 652e    del dataTable.
-00030550: 6d65 7461 5b27 756e 6974 546f 275d 0a20  meta['unitTo']. 
-00030560: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-00030570: 734c 6973 742e 6170 7065 6e64 2864 6174  sList.append(dat
-00030580: 6154 6162 6c65 2e61 7374 7970 6528 666c  aTable.astype(fl
-00030590: 6f61 7429 290a 0a20 2020 2020 2020 2072  oat))..        r
-000305a0: 6574 7572 6e20 7461 626c 6573 4c69 7374  eturn tablesList
-000305b0: 2c20 5b5d 0a0a 0a63 6c61 7373 2045 4e45  , []...class ENE
-000305c0: 5244 4154 4128 4261 7365 496d 706f 7274  RDATA(BaseImport
-000305d0: 546f 6f6c 293a 0a20 2020 2064 6566 205f  Tool):.    def _
-000305e0: 5f69 6e69 745f 5f28 7365 6c66 2c20 7965  _init__(self, ye
-000305f0: 6172 3d32 3031 392c 2064 6174 615f 7061  ar=2019, data_pa
-00030600: 7468 3d4e 6f6e 652c 2066 696c 656e 616d  th=None, filenam
-00030610: 653d 4e6f 6e65 293a 0a0a 2020 2020 2020  e=None):..      
-00030620: 2020 6966 2064 6174 615f 7061 7468 2069    if data_path i
-00030630: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00030640: 2020 2020 6461 7461 5f70 6174 6820 3d20      data_path = 
-00030650: 6f73 2e70 6174 682e 6a6f 696e 2863 6f6e  os.path.join(con
-00030660: 6669 672e 5041 5448 5f54 4f5f 4441 5441  fig.PATH_TO_DATA
-00030670: 5348 454c 462c 2027 7261 7764 6174 6127  SHELF, 'rawdata'
-00030680: 290a 0a20 2020 2020 2020 2069 6620 6669  )..        if fi
-00030690: 6c65 6e61 6d65 2069 7320 4e6f 6e65 3a0a  lename is None:.
-000306a0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-000306b0: 6e61 6d65 203d 2066 2765 6e65 7264 6174  name = f'enerdat
-000306c0: 615f 7b79 6561 727d 2e78 6c73 7827 0a20  a_{year}.xlsx'. 
-000306d0: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
-000306e0: 7020 3d20 7365 7475 7053 7472 7563 7428  p = setupStruct(
-000306f0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00030700: 6574 7570 2e53 4f55 5243 455f 4944 203d  etup.SOURCE_ID =
-00030710: 2022 454e 4552 4441 5441 5f22 202b 2073   "ENERDATA_" + s
-00030720: 7472 2879 6561 7229 0a20 2020 2020 2020  tr(year).       
-00030730: 2073 656c 662e 7365 7475 702e 534f 5552   self.setup.SOUR
-00030740: 4345 5f50 4154 4820 3d20 6f73 2e70 6174  CE_PATH = os.pat
-00030750: 682e 6a6f 696e 2864 6174 615f 7061 7468  h.join(data_path
-00030760: 2c20 7365 6c66 2e73 6574 7570 2e53 4f55  , self.setup.SOU
-00030770: 5243 455f 4944 290a 0a20 2020 2020 2020  RCE_ID)..       
-00030780: 2073 656c 662e 7365 7475 702e 4441 5441   self.setup.DATA
-00030790: 5f46 494c 4520 3d20 6f73 2e70 6174 682e  _FILE = os.path.
-000307a0: 6a6f 696e 2873 656c 662e 7365 7475 702e  join(self.setup.
-000307b0: 534f 5552 4345 5f50 4154 482c 2066 696c  SOURCE_PATH, fil
-000307c0: 656e 616d 6529 0a20 2020 2020 2020 2073  ename).        s
-000307d0: 656c 662e 7365 7475 702e 4d41 5050 494e  elf.setup.MAPPIN
-000307e0: 475f 4649 4c45 203d 206f 732e 7061 7468  G_FILE = os.path
-000307f0: 2e6a 6f69 6e28 0a20 2020 2020 2020 2020  .join(.         
-00030800: 2020 2073 656c 662e 7365 7475 702e 534f     self.setup.SO
-00030810: 5552 4345 5f50 4154 482c 2027 6d61 7070  URCE_PATH, 'mapp
-00030820: 696e 675f 2720 2b20 7374 7228 7965 6172  ing_' + str(year
-00030830: 2920 2b20 272e 786c 7378 270a 2020 2020  ) + '.xlsx'.    
-00030840: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-00030850: 6c66 2e73 6574 7570 2e4c 4943 454e 4345  lf.setup.LICENCE
-00030860: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00030870: 2027 2052 6573 7472 6963 7465 6420 7573   ' Restricted us
-00030880: 6520 696e 2074 6865 2043 6c69 6d61 7465  e in the Climate
-00030890: 2054 7261 6e73 7061 7265 6e63 7920 5265   Transparency Re
-000308a0: 706f 7274 2070 726f 6a65 6374 206f 6e6c  port project onl
-000308b0: 7927 0a20 2020 2020 2020 2029 0a20 2020  y'.        ).   
-000308c0: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
-000308d0: 5552 4c20 3d20 2768 7474 7073 3a2f 2f77  URL = 'https://w
-000308e0: 7777 2e65 6e65 7264 6174 612e 6e65 742f  ww.enerdata.net/
-000308f0: 7573 6572 2f3f 6465 7374 696e 6174 696f  user/?destinatio
-00030900: 6e3d 7365 7276 6963 6573 2e68 746d 6c27  n=services.html'
-00030910: 0a0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-00030920: 6574 7570 2e52 4547 494f 4e5f 434f 4c55  etup.REGION_COLU
-00030930: 4d4e 5f4e 414d 4520 3d20 2749 534f 2063  MN_NAME = 'ISO c
-00030940: 6f64 6527 0a20 2020 2020 2020 2073 656c  ode'.        sel
-00030950: 662e 7365 7475 702e 5641 5249 4142 4c45  f.setup.VARIABLE
-00030960: 5f43 4f4c 554d 4e5f 4e41 4d45 203d 2027  _COLUMN_NAME = '
-00030970: 4974 656d 2063 6f64 6527 0a0a 2020 2020  Item code'..    
-00030980: 2020 2020 6966 206e 6f74 2028 6f73 2e70      if not (os.p
-00030990: 6174 682e 6578 6973 7473 2873 656c 662e  ath.exists(self.
-000309a0: 7365 7475 702e 4d41 5050 494e 475f 4649  setup.MAPPING_FI
-000309b0: 4c45 2929 3a0a 2020 2020 2020 2020 2020  LE)):.          
-000309c0: 2020 7365 6c66 2e63 7265 6174 6556 6172    self.createVar
-000309d0: 6961 626c 654d 6170 7069 6e67 2829 0a20  iableMapping(). 
-000309e0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-000309f0: 2822 6e6f 206d 6170 7069 6e67 2066 696c  ("no mapping fil
-00030a00: 6520 666f 756e 6422 290a 2020 2020 2020  e found").      
-00030a10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00030a20: 2020 2020 7365 6c66 2e6d 6170 7069 6e67      self.mapping
-00030a30: 203d 2064 6963 7428 290a 0a20 2020 2020   = dict()..     
-00030a40: 2020 2020 2020 2066 6f72 2076 6172 2069         for var i
-00030a50: 6e20 5b27 656e 7469 7479 272c 2027 7265  n ['entity', 're
-00030a60: 6769 6f6e 275d 3a0a 2020 2020 2020 2020  gion']:.        
-00030a70: 2020 2020 2020 2020 6466 203d 2070 642e          df = pd.
-00030a80: 7265 6164 5f65 7863 656c 280a 2020 2020  read_excel(.    
-00030a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030aa0: 7365 6c66 2e73 6574 7570 2e4d 4150 5049  self.setup.MAPPI
-00030ab0: 4e47 5f46 494c 452c 2073 6865 6574 5f6e  NG_FILE, sheet_n
-00030ac0: 616d 653d 7661 7220 2b20 275f 6d61 7070  ame=var + '_mapp
-00030ad0: 696e 6727 2c20 696e 6465 785f 636f 6c3d  ing', index_col=
-00030ae0: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-00030af0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00030b00: 2020 2020 6466 203d 2064 662e 6c6f 635b      df = df.loc[
-00030b10: 7e64 662e 6c6f 635b 3a2c 2076 6172 5d2e  ~df.loc[:, var].
-00030b20: 6973 6e61 2829 5d0a 2020 2020 2020 2020  isna()].        
-00030b30: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
-00030b40: 7069 6e67 2e75 7064 6174 6528 6466 2e74  ping.update(df.t
-00030b50: 6f5f 6469 6374 2829 290a 0a20 2020 2020  o_dict())..     
-00030b60: 2020 2073 656c 662e 6372 6561 7465 536f     self.createSo
-00030b70: 7572 6365 4d65 7461 2829 0a0a 2020 2020  urceMeta()..    
-00030b80: 6465 6620 6c6f 6164 4461 7461 2873 656c  def loadData(sel
-00030b90: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00030ba0: 2e64 6174 6120 3d20 7064 2e72 6561 645f  .data = pd.read_
-00030bb0: 6578 6365 6c28 0a20 2020 2020 2020 2020  excel(.         
-00030bc0: 2020 2073 656c 662e 7365 7475 702e 4441     self.setup.DA
-00030bd0: 5441 5f46 494c 452c 2069 6e64 6578 5f63  TA_FILE, index_c
-00030be0: 6f6c 3d4e 6f6e 652c 2068 6561 6465 723d  ol=None, header=
-00030bf0: 302c 206e 615f 7661 6c75 6573 3d27 6e2e  0, na_values='n.
-00030c00: 612e 270a 2020 2020 2020 2020 290a 0a20  a.'.        ).. 
-00030c10: 2020 2020 2020 2023 2066 6978 2064 6f6f         # fix doo
-00030c20: 7562 6c65 2065 6e74 7279 206f 6620 736f  uble entry of so
-00030c30: 6c61 720a 2020 2020 2020 2020 6d61 736b  lar.        mask
-00030c40: 203d 2028 7365 6c66 2e64 6174 612e 6c6f   = (self.data.lo
-00030c50: 635b 3a2c 2027 4974 656d 2063 6f64 6527  c[:, 'Item code'
-00030c60: 5d20 3d3d 2027 6564 7670 6427 2920 2620  ] == 'edvpd') & 
-00030c70: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-00030c80: 6c66 2e64 6174 612e 6c6f 635b 3a2c 2027  lf.data.loc[:, '
-00030c90: 556e 6974 275d 203d 3d20 274d 746f 6527  Unit'] == 'Mtoe'
-00030ca0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00030cb0: 2020 2069 6e64 5f74 6f5f 6472 6f70 7020     ind_to_dropp 
-00030cc0: 3d20 7365 6c66 2e64 6174 612e 696e 6465  = self.data.inde
-00030cd0: 785b 6d61 736b 5d0a 2020 2020 2020 2020  x[mask].        
-00030ce0: 7365 6c66 2e64 6174 6120 3d20 7365 6c66  self.data = self
-00030cf0: 2e64 6174 612e 6472 6f70 2869 6e64 5f74  .data.drop(ind_t
-00030d00: 6f5f 6472 6f70 7029 0a0a 2020 2020 2020  o_dropp)..      
-00030d10: 2020 7365 6c66 2e64 6174 612e 6c6f 635b    self.data.loc[
-00030d20: 3a2c 2027 7265 6769 6f6e 275d 203d 2073  :, 'region'] = s
-00030d30: 656c 662e 6461 7461 2e6c 6f63 5b3a 2c20  elf.data.loc[:, 
-00030d40: 7365 6c66 2e73 6574 7570 2e52 4547 494f  self.setup.REGIO
-00030d50: 4e5f 434f 4c55 4d4e 5f4e 414d 455d 0a20  N_COLUMN_NAME]. 
-00030d60: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
-00030d70: 2e6c 6f63 5b3a 2c20 2765 6e74 6974 7927  .loc[:, 'entity'
-00030d80: 5d20 3d20 7365 6c66 2e64 6174 612e 6c6f  ] = self.data.lo
-00030d90: 635b 3a2c 2073 656c 662e 7365 7475 702e  c[:, self.setup.
-00030da0: 5641 5249 4142 4c45 5f43 4f4c 554d 4e5f  VARIABLE_COLUMN_
-00030db0: 4e41 4d45 5d0a 2020 2020 2020 2020 7365  NAME].        se
-00030dc0: 6c66 2e64 6174 612e 6c6f 635b 3a2c 2027  lf.data.loc[:, '
-00030dd0: 7363 656e 6172 696f 275d 203d 2027 4869  scenario'] = 'Hi
-00030de0: 7374 6f72 6963 270a 0a20 2020 2020 2020  storic'..       
-00030df0: 2073 656c 662e 7469 6d65 436f 6c75 6d6e   self.timeColumn
-00030e00: 7320 3d20 6c69 7374 2829 0a20 2020 2020  s = list().     
-00030e10: 2020 2066 6f72 2063 6f6c 2069 6e20 7365     for col in se
-00030e20: 6c66 2e64 6174 612e 636f 6c75 6d6e 733a  lf.data.columns:
-00030e30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00030e40: 6973 696e 7374 616e 6365 2863 6f6c 2c20  isinstance(col, 
-00030e50: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-00030e60: 2020 2020 2020 7365 6c66 2e74 696d 6543        self.timeC
-00030e70: 6f6c 756d 6e73 2e61 7070 656e 6428 636f  olumns.append(co
-00030e80: 6c29 0a0a 2020 2020 2320 2020 2020 2020  l)..    #       
-00030e90: 2073 656c 662e 6461 7461 2e6c 6f63 5b3a   self.data.loc[:
-00030ea0: 2c27 6d6f 6465 6c27 5d20 3d20 2727 0a20  ,'model'] = ''. 
-00030eb0: 2020 2064 6566 2063 7265 6174 6556 6172     def createVar
-00030ec0: 6961 626c 654d 6170 7069 6e67 2873 656c  iableMapping(sel
-00030ed0: 6629 3a0a 0a20 2020 2020 2020 2023 206c  f):..        # l
-00030ee0: 6f61 6469 6e67 2064 6174 6120 6966 206e  oading data if n
-00030ef0: 6563 6573 7361 7279 0a20 2020 2020 2020  ecessary.       
-00030f00: 2069 6620 6e6f 7420 6861 7361 7474 7228   if not hasattr(
-00030f10: 7365 6c66 2c20 2764 6174 6127 293a 0a20  self, 'data'):. 
-00030f20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00030f30: 6c6f 6164 4461 7461 2829 0a0a 2020 2020  loadData()..    
-00030f40: 2020 2020 696d 706f 7274 206e 756d 7079      import numpy
-00030f50: 2061 7320 6e70 0a0a 2020 2020 2020 2020   as np..        
-00030f60: 7772 6974 6572 203d 2070 642e 4578 6365  writer = pd.Exce
-00030f70: 6c57 7269 7465 7228 0a20 2020 2020 2020  lWriter(.       
-00030f80: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
-00030f90: 4d41 5050 494e 475f 4649 4c45 2c0a 2020  MAPPING_FILE,.  
-00030fa0: 2020 2020 2020 2020 2020 656e 6769 6e65            engine
-00030fb0: 3d27 786c 7378 7772 6974 6572 272c 0a20  ='xlsxwriter',. 
-00030fc0: 2020 2020 2020 2020 2020 2064 6174 6574             datet
-00030fd0: 696d 655f 666f 726d 6174 3d27 6d6d 6d20  ime_format='mmm 
-00030fe0: 6420 7979 7979 2068 683a 6d6d 3a73 7327  d yyyy hh:mm:ss'
-00030ff0: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
-00031000: 7465 5f66 6f72 6d61 743d 276d 6d6d 6d20  te_format='mmmm 
-00031010: 6464 2079 7979 7927 2c0a 2020 2020 2020  dd yyyy',.      
-00031020: 2020 290a 0a20 2020 2020 2020 2023 2076    )..        # v
-00031030: 6172 6961 626c 6573 0a20 2020 2020 2020  ariables.       
-00031040: 2023 2069 6e64 6578 203d 2073 656c 662e   # index = self.
-00031050: 6461 7461 5b73 656c 662e 7365 7475 702e  data[self.setup.
-00031060: 5641 5249 4142 4c45 5f43 4f4c 554d 4e5f  VARIABLE_COLUMN_
-00031070: 4e41 4d45 5d2e 756e 6971 7565 2829 0a20  NAME].unique(). 
-00031080: 2020 2020 2020 2073 656c 662e 6176 6169         self.avai
-00031090: 6c61 626c 6553 6572 6965 7320 3d20 7365  lableSeries = se
-000310a0: 6c66 2e64 6174 612e 6472 6f70 5f64 7570  lf.data.drop_dup
-000310b0: 6c69 6361 7465 7328 0a20 2020 2020 2020  licates(.       
-000310c0: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
-000310d0: 5641 5249 4142 4c45 5f43 4f4c 554d 4e5f  VARIABLE_COLUMN_
-000310e0: 4e41 4d45 0a20 2020 2020 2020 2029 2e73  NAME.        ).s
-000310f0: 6574 5f69 6e64 6578 2873 656c 662e 7365  et_index(self.se
-00031100: 7475 702e 5641 5249 4142 4c45 5f43 4f4c  tup.VARIABLE_COL
-00031110: 554d 4e5f 4e41 4d45 295b 5b27 556e 6974  UMN_NAME)[['Unit
-00031120: 272c 2027 5469 746c 6527 5d5d 0a20 2020  ', 'Title']].   
-00031130: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
-00031140: 6720 3d20 7064 2e44 6174 6146 7261 6d65  g = pd.DataFrame
-00031150: 280a 2020 2020 2020 2020 2020 2020 696e  (.            in
-00031160: 6465 783d 7365 6c66 2e61 7661 696c 6162  dex=self.availab
-00031170: 6c65 5365 7269 6573 2e69 6e64 6578 2c20  leSeries.index, 
-00031180: 636f 6c75 6d6e 733d 5b27 656e 7469 7479  columns=['entity
-00031190: 272c 2027 6361 7465 676f 7279 272c 2027  ', 'category', '
-000311a0: 756e 6974 546f 275d 0a20 2020 2020 2020  unitTo'].       
-000311b0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-000311c0: 6d61 7070 696e 6720 3d20 7064 2e63 6f6e  mapping = pd.con
-000311d0: 6361 7428 5b73 656c 662e 6d61 7070 696e  cat([self.mappin
-000311e0: 672c 2073 656c 662e 6176 6169 6c61 626c  g, self.availabl
-000311f0: 6553 6572 6965 735d 2c20 6178 6973 3d31  eSeries], axis=1
-00031200: 290a 2020 2020 2020 2020 7365 6c66 2e6d  ).        self.m
-00031210: 6170 7069 6e67 203d 2073 656c 662e 6d61  apping = self.ma
-00031220: 7070 696e 672e 736f 7274 5f69 6e64 6578  pping.sort_index
-00031230: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00031240: 6d61 7070 696e 672e 746f 5f65 7863 656c  mapping.to_excel
-00031250: 2877 7269 7465 722c 2065 6e67 696e 653d  (writer, engine=
-00031260: 276f 7065 6e70 7978 6c27 2c20 7368 6565  'openpyxl', shee
-00031270: 745f 6e61 6d65 3d56 4152 5f4d 4150 5049  t_name=VAR_MAPPI
-00031280: 4e47 5f53 4845 4554 290a 0a20 2020 2020  NG_SHEET)..     
-00031290: 2020 2023 206d 6f64 656c 730a 2020 2020     # models.    
-000312a0: 2020 2020 2320 2020 2020 2020 2069 6e64      #        ind
-000312b0: 6578 203d 206e 702e 756e 6971 7565 2873  ex = np.unique(s
-000312c0: 656c 662e 6461 7461 5b73 656c 662e 7365  elf.data[self.se
-000312d0: 7475 702e 4d4f 4445 4c5f 434f 4c55 4d4e  tup.MODEL_COLUMN
-000312e0: 5f4e 414d 455d 2e76 616c 7565 7329 0a20  _NAME].values). 
-000312f0: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
-00031300: 2023 2020 2020 2020 2020 7365 6c66 2e61   #        self.a
-00031310: 7661 696c 6162 6c65 5365 7269 6573 203d  vailableSeries =
-00031320: 2070 642e 4461 7461 4672 616d 6528 696e   pd.DataFrame(in
-00031330: 6465 783d 696e 6465 7829 0a20 2020 2020  dex=index).     
-00031340: 2020 2023 2020 2020 2020 2020 7365 6c66     #        self
-00031350: 2e6d 6170 7069 6e67 203d 2070 642e 4461  .mapping = pd.Da
-00031360: 7461 4672 616d 6528 696e 6465 783d 696e  taFrame(index=in
-00031370: 6465 782c 2063 6f6c 756d 6e73 203d 205b  dex, columns = [
-00031380: 7365 6c66 2e73 6574 7570 2e4d 4f44 454c  self.setup.MODEL
-00031390: 5f43 4f4c 554d 4e5f 4e41 4d45 5d29 0a20  _COLUMN_NAME]). 
-000313a0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-000313b0: 7365 6c66 2e6d 6170 7069 6e67 203d 2070  self.mapping = p
-000313c0: 642e 636f 6e63 6174 285b 7365 6c66 2e6d  d.concat([self.m
-000313d0: 6170 7069 6e67 2c20 7365 6c66 2e61 7661  apping, self.ava
-000313e0: 696c 6162 6c65 5365 7269 6573 5d2c 2061  ilableSeries], a
-000313f0: 7869 733d 3129 0a20 2020 2020 2020 2023  xis=1).        #
-00031400: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
-00031410: 7069 6e67 203d 2073 656c 662e 6d61 7070  ping = self.mapp
-00031420: 696e 672e 736f 7274 5f69 6e64 6578 2829  ing.sort_index()
-00031430: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-00031440: 2020 2023 2020 2020 2020 2020 7365 6c66     #        self
-00031450: 2e6d 6170 7069 6e67 2e74 6f5f 6578 6365  .mapping.to_exce
-00031460: 6c28 7772 6974 6572 2c20 656e 6769 6e65  l(writer, engine
-00031470: 3d27 6f70 656e 7079 786c 272c 2073 6865  ='openpyxl', she
-00031480: 6574 5f6e 616d 653d 276d 6f64 656c 5f6d  et_name='model_m
-00031490: 6170 7069 6e67 2729 0a0a 2020 2020 2020  apping')..      
-000314a0: 2020 2320 7363 656e 6172 696f 730a 2020    # scenarios.  
-000314b0: 2020 2020 2020 2320 2020 2020 2020 2069        #        i
-000314c0: 6e64 6578 203d 206e 702e 756e 6971 7565  ndex = np.unique
-000314d0: 2873 656c 662e 6461 7461 5b73 656c 662e  (self.data[self.
-000314e0: 7365 7475 702e 5343 454e 4152 494f 5f43  setup.SCENARIO_C
-000314f0: 4f4c 554d 4e5f 4e41 4d45 5d2e 7661 6c75  OLUMN_NAME].valu
-00031500: 6573 290a 2020 2020 2020 2020 230a 2020  es).        #.  
-00031510: 2020 2020 2020 2320 2020 2020 2020 2073        #        s
-00031520: 656c 662e 6176 6169 6c61 626c 6553 6572  elf.availableSer
-00031530: 6965 7320 3d20 7064 2e44 6174 6146 7261  ies = pd.DataFra
-00031540: 6d65 2869 6e64 6578 3d69 6e64 6578 290a  me(index=index).
-00031550: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-00031560: 2073 656c 662e 6d61 7070 696e 6720 3d20   self.mapping = 
-00031570: 7064 2e44 6174 6146 7261 6d65 2869 6e64  pd.DataFrame(ind
-00031580: 6578 3d69 6e64 6578 2c20 636f 6c75 6d6e  ex=index, column
-00031590: 7320 3d20 5b73 656c 662e 7365 7475 702e  s = [self.setup.
-000315a0: 5343 454e 4152 494f 5f43 4f4c 554d 4e5f  SCENARIO_COLUMN_
-000315b0: 4e41 4d45 5d29 0a20 2020 2020 2020 2023  NAME]).        #
-000315c0: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
-000315d0: 7069 6e67 203d 2070 642e 636f 6e63 6174  ping = pd.concat
-000315e0: 285b 7365 6c66 2e6d 6170 7069 6e67 2c20  ([self.mapping, 
-000315f0: 7365 6c66 2e61 7661 696c 6162 6c65 5365  self.availableSe
-00031600: 7269 6573 5d2c 2061 7869 733d 3129 0a20  ries], axis=1). 
-00031610: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-00031620: 7365 6c66 2e6d 6170 7069 6e67 203d 2073  self.mapping = s
-00031630: 656c 662e 6d61 7070 696e 672e 736f 7274  elf.mapping.sort
-00031640: 5f69 6e64 6578 2829 0a20 2020 2020 2020  _index().       
-00031650: 2023 2020 2020 2020 2020 7365 6c66 2e6d   #        self.m
-00031660: 6170 7069 6e67 2e74 6f5f 6578 6365 6c28  apping.to_excel(
-00031670: 7772 6974 6572 2c20 656e 6769 6e65 3d27  writer, engine='
-00031680: 6f70 656e 7079 786c 272c 2073 6865 6574  openpyxl', sheet
-00031690: 5f6e 616d 653d 2773 6365 6e61 7269 6f5f  _name='scenario_
-000316a0: 6d61 7070 696e 6727 290a 0a20 2020 2020  mapping')..     
-000316b0: 2020 2023 2072 6567 696f 6e0a 2020 2020     # region.    
-000316c0: 2020 2020 696e 6465 7820 3d20 7365 6c66      index = self
-000316d0: 2e64 6174 615b 7365 6c66 2e73 6574 7570  .data[self.setup
-000316e0: 2e52 4547 494f 4e5f 434f 4c55 4d4e 5f4e  .REGION_COLUMN_N
-000316f0: 414d 455d 2e75 6e69 7175 6528 290a 0a20  AME].unique().. 
-00031700: 2020 2020 2020 2073 656c 662e 6176 6169         self.avai
-00031710: 6c61 626c 6553 6572 6965 7320 3d20 7064  lableSeries = pd
-00031720: 2e44 6174 6146 7261 6d65 2869 6e64 6578  .DataFrame(index
-00031730: 3d69 6e64 6578 290a 2020 2020 2020 2020  =index).        
-00031740: 7365 6c66 2e6d 6170 7069 6e67 203d 2070  self.mapping = p
-00031750: 642e 4461 7461 4672 616d 6528 696e 6465  d.DataFrame(inde
-00031760: 783d 696e 6465 782c 2063 6f6c 756d 6e73  x=index, columns
-00031770: 3d5b 2772 6567 696f 6e27 5d29 0a20 2020  =['region']).   
-00031780: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
-00031790: 6720 3d20 7064 2e63 6f6e 6361 7428 5b73  g = pd.concat([s
-000317a0: 656c 662e 6d61 7070 696e 672c 2073 656c  elf.mapping, sel
-000317b0: 662e 6176 6169 6c61 626c 6553 6572 6965  f.availableSerie
-000317c0: 735d 2c20 6178 6973 3d31 290a 2020 2020  s], axis=1).    
-000317d0: 2020 2020 7365 6c66 2e6d 6170 7069 6e67      self.mapping
-000317e0: 203d 2073 656c 662e 6d61 7070 696e 672e   = self.mapping.
-000317f0: 736f 7274 5f69 6e64 6578 2829 0a0a 2020  sort_index()..  
-00031800: 2020 2020 2020 666f 7220 6964 7820 696e        for idx in
-00031810: 2073 656c 662e 6d61 7070 696e 672e 696e   self.mapping.in
-00031820: 6465 783a 0a20 2020 2020 2020 2020 2020  dex:.           
-00031830: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-00031840: 6365 2869 6478 2c20 2873 7472 2c20 696e  ce(idx, (str, in
-00031850: 7429 293a 0a20 2020 2020 2020 2020 2020  t)):.           
-00031860: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-00031870: 2020 2020 2020 2020 2020 6973 6f20 3d20            iso = 
-00031880: 6474 2e75 7469 6c2e 6964 656e 7469 6679  dt.util.identify
-00031890: 436f 756e 7472 7928 6964 7829 0a20 2020  Country(idx).   
-000318a0: 2020 2020 2020 2020 2069 6620 6973 6f20           if iso 
-000318b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000318c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000318d0: 662e 6d61 7070 696e 672e 6c6f 635b 6964  f.mapping.loc[id
-000318e0: 782c 2027 7265 6769 6f6e 275d 203d 2069  x, 'region'] = i
-000318f0: 736f 0a0a 2020 2020 2020 2020 7365 6c66  so..        self
-00031900: 2e6d 6170 7069 6e67 2e74 6f5f 6578 6365  .mapping.to_exce
-00031910: 6c28 7772 6974 6572 2c20 656e 6769 6e65  l(writer, engine
-00031920: 3d27 6f70 656e 7079 786c 272c 2073 6865  ='openpyxl', she
-00031930: 6574 5f6e 616d 653d 2772 6567 696f 6e5f  et_name='region_
-00031940: 6d61 7070 696e 6727 290a 2020 2020 2020  mapping').      
-00031950: 2020 7772 6974 6572 2e63 6c6f 7365 2829    writer.close()
-00031960: 0a0a 2020 2020 6465 6620 6761 7468 6572  ..    def gather
-00031970: 4d61 7070 6564 4461 7461 2873 656c 662c  MappedData(self,
-00031980: 2073 7061 7469 616c 5375 6253 6574 3d4e   spatialSubSet=N
-00031990: 6f6e 6529 3a0a 0a20 2020 2020 2020 2069  one):..        i
-000319a0: 6d70 6f72 7420 7471 646d 0a0a 2020 2020  mport tqdm..    
-000319b0: 2020 2020 2320 6c6f 6164 696e 6720 6461      # loading da
-000319c0: 7461 2069 6620 6e65 6365 7373 6172 790a  ta if necessary.
-000319d0: 2020 2020 2020 2020 6966 206e 6f74 2068          if not h
-000319e0: 6173 6174 7472 2873 656c 662c 2027 6461  asattr(self, 'da
-000319f0: 7461 2729 3a0a 2020 2020 2020 2020 2020  ta'):.          
-00031a00: 2020 7365 6c66 2e6c 6f61 6444 6174 6128    self.loadData(
-00031a10: 290a 0a20 2020 2020 2020 2074 6162 6c65  )..        table
-00031a20: 7354 6f43 6f6d 6d69 7420 3d20 5b5d 0a20  sToCommit = []. 
-00031a30: 2020 2020 2020 206d 6574 6144 6963 7420         metaDict 
-00031a40: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00031a50: 206d 6574 6144 6963 745b 2773 6f75 7263   metaDict['sourc
-00031a60: 6527 5d20 3d20 7365 6c66 2e73 6574 7570  e'] = self.setup
-00031a70: 2e53 4f55 5243 455f 4944 0a20 2020 2020  .SOURCE_ID.     
-00031a80: 2020 2065 7863 6c75 6465 6454 6162 6c65     excludedTable
-00031a90: 7320 3d20 6469 6374 2829 0a20 2020 2020  s = dict().     
-00031aa0: 2020 2065 7863 6c75 6465 6454 6162 6c65     excludedTable
-00031ab0: 735b 2765 6d70 7479 275d 203d 206c 6973  s['empty'] = lis
-00031ac0: 7428 290a 2020 2020 2020 2020 6578 636c  t().        excl
-00031ad0: 7564 6564 5461 626c 6573 5b27 6572 726f  udedTables['erro
-00031ae0: 7227 5d20 3d20 6c69 7374 2829 0a20 2020  r'] = list().   
-00031af0: 2020 2020 2065 7863 6c75 6465 6454 6162       excludedTab
-00031b00: 6c65 735b 2765 7869 7374 7327 5d20 3d20  les['exists'] = 
-00031b10: 6c69 7374 2829 0a0a 2020 2020 2020 2020  list()..        
-00031b20: 2320 6669 7820 646f 7562 6c65 2065 6e74  # fix double ent
-00031b30: 7269 6573 2066 6f72 2070 6f77 6572 2067  ries for power g
-00031b40: 656e 6572 6174 696f 6e20 7769 6e64 0a20  eneration wind. 
-00031b50: 2020 2020 2020 2077 696e 645f 6d61 736b         wind_mask
-00031b60: 203d 2073 656c 662e 6461 7461 2e65 6e74   = self.data.ent
-00031b70: 6974 7920 3d3d 2027 6565 6f70 6427 0a20  ity == 'eeopd'. 
-00031b80: 2020 2020 2020 204d 746f 655f 6d61 736b         Mtoe_mask
-00031b90: 203d 2073 656c 662e 6461 7461 2e55 6e69   = self.data.Uni
-00031ba0: 7420 3d3d 2027 4d74 6f65 270a 2020 2020  t == 'Mtoe'.    
-00031bb0: 2020 2020 6d61 736b 203d 2077 696e 645f      mask = wind_
-00031bc0: 6d61 736b 2026 204d 746f 655f 6d61 736b  mask & Mtoe_mask
-00031bd0: 0a20 2020 2020 2020 2073 656c 662e 6461  .        self.da
-00031be0: 7461 203d 2073 656c 662e 6461 7461 2e64  ta = self.data.d
-00031bf0: 726f 7028 7365 6c66 2e64 6174 612e 696e  rop(self.data.in
-00031c00: 6465 785b 6d61 736b 5d29 0a0a 2020 2020  dex[mask])..    
-00031c10: 2020 2020 666f 7220 7661 7269 6162 6c65      for variable
-00031c20: 2069 6e20 6c69 7374 2873 656c 662e 6d61   in list(self.ma
-00031c30: 7070 696e 675b 2765 6e74 6974 7927 5d2e  pping['entity'].
-00031c40: 6b65 7973 2829 293a 0a20 2020 2020 2020  keys()):.       
-00031c50: 2020 2020 2023 2020 2020 2020 2020 2020       #          
-00031c60: 2020 6d65 7461 4466 203d 2073 656c 662e    metaDf = self.
-00031c70: 6d61 7070 696e 672e 6c6f 635b 7661 7269  mapping.loc[vari
-00031c80: 6162 6c65 5d0a 2020 2020 2020 2020 2020  able].          
-00031c90: 2020 7465 6d70 4d6f 5363 5661 7220 3d20    tempMoScVar = 
-00031ca0: 7365 6c66 2e64 6174 612e 6c6f 635b 7365  self.data.loc[se
-00031cb0: 6c66 2e64 6174 612e 656e 7469 7479 203d  lf.data.entity =
-00031cc0: 3d20 7661 7269 6162 6c65 5d0a 2020 2020  = variable].    
-00031cd0: 2020 2020 2020 2020 7465 6d70 4d6f 5363          tempMoSc
-00031ce0: 5661 722e 756e 6974 203d 2073 656c 662e  Var.unit = self.
-00031cf0: 6d61 7070 696e 675b 2775 6e69 7427 5d5b  mapping['unit'][
-00031d00: 7661 7269 6162 6c65 5d0a 2020 2020 2020  variable].      
-00031d10: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-00031d20: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-00031d30: 7320 3d20 6474 2e69 6e74 6572 6661 6365  s = dt.interface
-00031d40: 732e 7265 6164 5f6c 6f6e 675f 7461 626c  s.read_long_tabl
-00031d50: 6528 7465 6d70 4d6f 5363 5661 722c 205b  e(tempMoScVar, [
-00031d60: 7661 7269 6162 6c65 5d29 0a0a 2020 2020  variable])..    
-00031d70: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
-00031d80: 7465 6d70 4d6f 5363 5661 722e 6c6f 635b  tempMoScVar.loc[
-00031d90: 3a2c 2073 656c 662e 7469 6d65 436f 6c75  :, self.timeColu
-00031da0: 6d6e 735d 0a0a 2020 2020 2020 2020 2020  mns]..          
-00031db0: 2020 7461 626c 6520 3d20 4461 7461 7461    table = Datata
-00031dc0: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
-00031dd0: 2020 2020 2074 6162 6c65 2c0a 2020 2020       table,.    
-00031de0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-00031df0: 3d7b 0a20 2020 2020 2020 2020 2020 2020  ={.             
-00031e00: 2020 2020 2020 2027 656e 7469 7479 273a         'entity':
-00031e10: 2073 656c 662e 6d61 7070 696e 675b 2765   self.mapping['e
-00031e20: 6e74 6974 7927 5d5b 7661 7269 6162 6c65  ntity'][variable
-00031e30: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00031e40: 2020 2020 2020 2027 6361 7465 676f 7279         'category
-00031e50: 273a 2073 656c 662e 6d61 7070 696e 675b  ': self.mapping[
-00031e60: 2763 6174 6567 6f72 7927 5d5b 7661 7269  'category'][vari
-00031e70: 6162 6c65 5d2c 0a20 2020 2020 2020 2020  able],.         
-00031e80: 2020 2020 2020 2020 2020 2027 7363 656e             'scen
-00031e90: 6172 696f 273a 2027 4869 7374 6f72 6963  ario': 'Historic
-00031ea0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00031eb0: 2020 2020 2020 2027 736f 7572 6365 273a         'source':
-00031ec0: 2073 656c 662e 7365 7475 702e 534f 5552   self.setup.SOUR
-00031ed0: 4345 5f49 442c 0a20 2020 2020 2020 2020  CE_ID,.         
-00031ee0: 2020 2020 2020 2020 2020 2027 756e 6974             'unit
-00031ef0: 273a 2073 656c 662e 6d61 7070 696e 675b  ': self.mapping[
-00031f00: 2775 6e69 7427 5d5b 7661 7269 6162 6c65  'unit'][variable
-00031f10: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00031f20: 2020 2020 2020 2027 6f72 6967 696e 616c         'original
-00031f30: 2063 6f64 6527 3a20 7661 7269 6162 6c65   code': variable
-00031f40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00031f50: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00031f60: 2029 0a20 2020 2020 2020 2020 2020 2074   ).            t
-00031f70: 6162 6c65 2e69 6e64 6578 203d 2074 656d  able.index = tem
-00031f80: 704d 6f53 6356 6172 2e72 6567 696f 6e0a  pMoScVar.region.
-00031f90: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-00031fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031fb0: 2074 6162 6c65 2e6d 6574 615b 2763 6174   table.meta['cat
-00031fc0: 6567 6f72 7927 5d20 3d20 2222 0a20 2020  egory'] = "".   
-00031fd0: 2020 2020 2020 2020 2023 2020 2020 2020           #      
-00031fe0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-00031ff0: 626c 652e 6d65 7461 5b27 736f 7572 6365  ble.meta['source
-00032000: 275d 203d 0a20 2020 2020 2020 2020 2020  '] =.           
-00032010: 2074 6162 6c65 2e69 6e64 6578 203d 2074   table.index = t
-00032020: 6162 6c65 2e69 6e64 6578 2e6d 6170 2873  able.index.map(s
-00032030: 656c 662e 6d61 7070 696e 675b 2772 6567  elf.mapping['reg
-00032040: 696f 6e27 5d29 0a0a 2020 2020 2020 2020  ion'])..        
-00032050: 2020 2020 7461 626c 6520 3d20 7461 626c      table = tabl
-00032060: 652e 6c6f 635b 7e70 642e 6973 6e61 2874  e.loc[~pd.isna(t
-00032070: 6162 6c65 2e69 6e64 6578 292c 203a 5d0a  able.index), :].
-00032080: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00032090: 6f74 2070 642e 6973 6e61 2873 656c 662e  ot pd.isna(self.
-000320a0: 6d61 7070 696e 675b 2775 6e69 7454 6f27  mapping['unitTo'
-000320b0: 5d5b 7661 7269 6162 6c65 5d29 3a0a 2020  ][variable]):.  
-000320c0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000320d0: 696e 7428 2763 6f6e 7665 7273 696f 6e20  int('conversion 
-000320e0: 746f 203a 2027 202b 2073 7472 2873 656c  to : ' + str(sel
-000320f0: 662e 6d61 7070 696e 675b 2775 6e69 7454  f.mapping['unitT
-00032100: 6f27 5d5b 7661 7269 6162 6c65 5d29 290a  o'][variable])).
-00032110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032120: 7461 626c 6520 3d20 7461 626c 652e 636f  table = table.co
-00032130: 6e76 6572 7428 7365 6c66 2e6d 6170 7069  nvert(self.mappi
-00032140: 6e67 5b27 756e 6974 546f 275d 5b76 6172  ng['unitTo'][var
-00032150: 6961 626c 655d 290a 2020 2020 2020 2020  iable]).        
-00032160: 2020 2020 7461 626c 6549 4420 3d20 6474      tableID = dt
-00032170: 2e63 6f72 652e 5f63 7265 6174 6544 6174  .core._createDat
-00032180: 6162 6173 6549 4428 7461 626c 652e 6d65  abaseID(table.me
-00032190: 7461 290a 2020 2020 2020 2020 2020 2020  ta).            
-000321a0: 7461 626c 6573 546f 436f 6d6d 6974 2e61  tablesToCommit.a
-000321b0: 7070 656e 6428 7461 626c 6529 0a0a 2020  ppend(table)..  
-000321c0: 2020 2020 2020 7265 7475 726e 2074 6162        return tab
-000321d0: 6c65 7354 6f43 6f6d 6d69 742c 2065 7863  lesToCommit, exc
-000321e0: 6c75 6465 6454 6162 6c65 730a 0a0a 636c  ludedTables...cl
-000321f0: 6173 7320 5049 4b5f 4e44 4328 4261 7365  ass PIK_NDC(Base
-00032200: 496d 706f 7274 546f 6f6c 293a 0a20 2020  ImportTool):.   
-00032210: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00032220: 6c66 2c20 7965 6172 2c20 7665 7273 696f  lf, year, versio
-00032230: 6e29 3a0a 2020 2020 2020 2020 7365 6c66  n):.        self
-00032240: 2e73 6574 7570 203d 2073 6574 7570 5374  .setup = setupSt
-00032250: 7275 6374 2829 0a0a 2020 2020 2020 2020  ruct()..        
-00032260: 7365 6c66 2e73 6574 7570 2e53 4f55 5243  self.setup.SOURC
-00032270: 455f 4944 203d 2022 5049 4b5f 4e44 435f  E_ID = "PIK_NDC_
-00032280: 2220 2b20 7374 7228 7965 6172 290a 2020  " + str(year).  
-00032290: 2020 2020 2020 7365 6c66 2e73 6574 7570        self.setup
-000322a0: 2e53 4f55 5243 455f 4e41 4d45 203d 2022  .SOURCE_NAME = "
-000322b0: 5049 4b5f 4e44 4322 0a20 2020 2020 2020  PIK_NDC".       
-000322c0: 2073 656c 662e 7365 7475 702e 534f 5552   self.setup.SOUR
-000322d0: 4345 5f59 4541 5220 3d20 7374 7228 7965  CE_YEAR = str(ye
-000322e0: 6172 290a 0a20 2020 2020 2020 2073 656c  ar)..        sel
-000322f0: 662e 7365 7475 702e 534f 5552 4345 5f50  f.setup.SOURCE_P
-00032300: 4154 4820 3d20 6f73 2e70 6174 682e 6a6f  ATH = os.path.jo
-00032310: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
-00032320: 636f 6e66 6967 2e50 4154 485f 544f 5f44  config.PATH_TO_D
-00032330: 4154 4153 4845 4c46 2c20 6627 7261 7764  ATASHELF, f'rawd
-00032340: 6174 612f 5049 4b5f 4e44 435f 7b79 6561  ata/PIK_NDC_{yea
-00032350: 727d 270a 2020 2020 2020 2020 290a 2020  r}'.        ).  
-00032360: 2020 2020 2020 7365 6c66 2e73 6574 7570        self.setup
-00032370: 2e44 4154 415f 4649 4c45 203d 206f 732e  .DATA_FILE = os.
-00032380: 7061 7468 2e6a 6f69 6e28 0a20 2020 2020  path.join(.     
-00032390: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
-000323a0: 702e 534f 5552 4345 5f50 4154 482c 0a20  p.SOURCE_PATH,. 
-000323b0: 2020 2020 2020 2020 2020 2066 276e 6463             f'ndc
-000323c0: 5f74 6172 6765 7473 5f70 6174 6877 6179  _targets_pathway
-000323d0: 735f 7065 725f 636f 756e 7472 795f 7573  s_per_country_us
-000323e0: 6564 5f66 6f72 5f67 726f 7570 5f70 6174  ed_for_group_pat
-000323f0: 6877 6179 735f 7b76 6572 7369 6f6e 7d2e  hways_{version}.
-00032400: 6373 7627 2c0a 2020 2020 2020 2020 290a  csv',.        ).
-00032410: 2020 2020 2020 2020 2320 7365 6c66 2e73          # self.s
-00032420: 6574 7570 2e4d 4150 5049 4e47 5f46 494c  etup.MAPPING_FIL
-00032430: 4520 3d20 6f73 2e70 6174 682e 6a6f 696e  E = os.path.join
-00032440: 2873 656c 662e 7365 7475 702e 534f 5552  (self.setup.SOUR
-00032450: 4345 5f50 4154 482c 2027 6d61 7070 696e  CE_PATH, 'mappin
-00032460: 672e 786c 7378 2729 0a20 2020 2020 2020  g.xlsx').       
-00032470: 2073 656c 662e 7365 7475 702e 4c49 4345   self.setup.LICE
-00032480: 4e43 4520 3d20 2743 4320 4259 2d34 2e30  NCE = 'CC BY-4.0
-00032490: 270a 2020 2020 2020 2020 7365 6c66 2e73  '.        self.s
-000324a0: 6574 7570 2e55 524c 203d 2027 6874 7470  etup.URL = 'http
-000324b0: 733a 2f2f 7a65 6e6f 646f 2e6f 7267 2f72  s://zenodo.org/r
-000324c0: 6563 6f72 642f 3531 3133 3938 3727 0a20  ecord/5113987'. 
-000324d0: 2020 2020 2020 2073 656c 662e 7665 7273         self.vers
-000324e0: 696f 6e20 3d20 7665 7273 696f 6e0a 0a20  ion = version.. 
-000324f0: 2020 2064 6566 2067 6174 6865 724d 6170     def gatherMap
-00032500: 7065 6444 6174 6128 7365 6c66 293a 0a0a  pedData(self):..
-00032510: 2020 2020 2020 2020 7069 6b5f 6461 7461          pik_data
-00032520: 203d 2070 642e 7265 6164 5f63 7376 280a   = pd.read_csv(.
-00032530: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00032540: 2e73 6574 7570 2e44 4154 415f 4649 4c45  .setup.DATA_FILE
-00032550: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00032560: 2020 2020 7072 696e 7428 7069 6b5f 6461      print(pik_da
-00032570: 7461 2e68 6561 6428 2929 0a0a 2020 2020  ta.head())..    
-00032580: 2020 2020 2320 7265 6d6f 7665 2063 6f75      # remove cou
-00032590: 6e74 7269 6573 2074 6861 7420 646f 206e  ntries that do n
-000325a0: 6f74 2068 6176 6520 6120 6361 6c63 7561  ot have a calcua
-000325b0: 6c74 6564 2074 6172 6765 740a 2020 2020  lted target.    
-000325c0: 2020 2020 6d61 736b 203d 2070 696b 5f64      mask = pik_d
-000325d0: 6174 612e 6164 645f 696e 666f 2e73 7472  ata.add_info.str
-000325e0: 2e73 7461 7274 7377 6974 6828 274e 6f20  .startswith('No 
-000325f0: 7461 7267 6574 7320 6361 6c63 756c 6174  targets calculat
-00032600: 6564 2729 0a20 2020 2020 2020 2069 6478  ed').        idx
-00032610: 5f74 6f5f 6472 6f70 203d 2070 696b 5f64  _to_drop = pik_d
-00032620: 6174 612e 696e 6465 785b 6d61 736b 203d  ata.index[mask =
-00032630: 3d20 5472 7565 5d0a 0a20 2020 2020 2020  = True]..       
-00032640: 2070 696b 5f64 6174 6120 3d20 7069 6b5f   pik_data = pik_
-00032650: 6461 7461 2e64 726f 7028 6964 785f 746f  data.drop(idx_to
-00032660: 5f64 726f 7029 0a0a 2020 2020 2020 2020  _drop)..        
-00032670: 7069 6b5f 6461 7461 203d 2070 696b 5f64  pik_data = pik_d
-00032680: 6174 612e 7365 745f 696e 6465 7828 5b27  ata.set_index(['
-00032690: 636f 6e64 6927 2c20 2772 6765 275d 290a  condi', 'rge']).
-000326a0: 0a20 2020 2020 2020 2070 6c65 6467 655f  .        pledge_
-000326b0: 6c6f 7720 3d20 7069 6b5f 6461 7461 5b0a  low = pik_data[.
-000326c0: 2020 2020 2020 2020 2020 2020 2870 696b              (pik
-000326d0: 5f64 6174 612e 696e 6465 782e 6765 745f  _data.index.get_
-000326e0: 6c65 7665 6c5f 7661 6c75 6573 2827 636f  level_values('co
-000326f0: 6e64 6927 2920 3d3d 2027 636f 6e64 6974  ndi') == 'condit
-00032700: 696f 6e61 6c27 290a 2020 2020 2020 2020  ional').        
-00032710: 2020 2020 2620 2870 696b 5f64 6174 612e      & (pik_data.
-00032720: 696e 6465 782e 6765 745f 6c65 7665 6c5f  index.get_level_
-00032730: 7661 6c75 6573 2827 7267 6527 2920 3d3d  values('rge') ==
-00032740: 2027 6265 7374 2729 0a20 2020 2020 2020   'best').       
-00032750: 205d 0a20 2020 2020 2020 2070 6c65 6467   ].        pledg
-00032760: 655f 6c6f 7720 3d20 706c 6564 6765 5f6c  e_low = pledge_l
-00032770: 6f77 2e73 6574 5f69 6e64 6578 2870 6c65  ow.set_index(ple
-00032780: 6467 655f 6c6f 772e 6c6f 635b 3a2c 2027  dge_low.loc[:, '
-00032790: 6973 6f33 275d 292e 6c6f 635b 0a20 2020  iso3']).loc[.   
-000327a0: 2020 2020 2020 2020 203a 2c20 5b73 7472           :, [str
-000327b0: 2878 2920 666f 7220 7820 696e 2072 616e  (x) for x in ran
-000327c0: 6765 2831 3939 302c 2032 3033 3129 5d0a  ge(1990, 2031)].
-000327d0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-000327e0: 2020 706c 6564 6765 5f6c 6f77 203d 2064    pledge_low = d
-000327f0: 742e 4461 7461 7461 626c 6528 0a20 2020  t.Datatable(.   
-00032800: 2020 2020 2020 2020 2070 6c65 6467 655f           pledge_
-00032810: 6c6f 772c 0a20 2020 2020 2020 2020 2020  low,.           
-00032820: 206d 6574 613d 7b0a 2020 2020 2020 2020   meta={.        
-00032830: 2020 2020 2020 2020 2765 6e74 6974 7927          'entity'
-00032840: 3a20 2745 6d69 7373 696f 6e73 7c4b 594f  : 'Emissions|KYO
-00032850: 544f 4748 475f 4152 3427 2c0a 2020 2020  TOGHG_AR4',.    
-00032860: 2020 2020 2020 2020 2020 2020 2763 6174              'cat
-00032870: 6567 6f72 7927 3a20 274e 6174 696f 6e61  egory': 'Nationa
-00032880: 6c5f 746f 7461 6c5f 6578 636c 5f4c 554c  l_total_excl_LUL
-00032890: 5543 4627 2c0a 2020 2020 2020 2020 2020  UCF',.          
-000328a0: 2020 2020 2020 276d 6f64 656c 273a 2066        'model': f
-000328b0: 2750 494b 5f4e 4443 6d69 7469 517c 7b73  'PIK_NDCmitiQ|{s
-000328c0: 656c 662e 7665 7273 696f 6e7d 272c 0a20  elf.version}',. 
-000328d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000328e0: 7363 656e 6172 696f 273a 2027 506c 6564  scenario': 'Pled
-000328f0: 6765 5f6c 6f77 272c 0a20 2020 2020 2020  ge_low',.       
-00032900: 2020 2020 2020 2020 2027 736f 7572 6365           'source
-00032910: 273a 2073 656c 662e 7365 7475 702e 534f  ': self.setup.SO
-00032920: 5552 4345 5f49 442c 0a20 2020 2020 2020  URCE_ID,.       
-00032930: 2020 2020 2020 2020 2027 756e 6974 273a           'unit':
-00032940: 2027 4d74 2043 4f32 6571 272c 0a20 2020   'Mt CO2eq',.   
-00032950: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00032960: 2020 2020 290a 0a20 2020 2020 2020 2070      )..        p
-00032970: 6c65 6467 655f 6869 6768 203d 2070 696b  ledge_high = pik
-00032980: 5f64 6174 615b 0a20 2020 2020 2020 2020  _data[.         
-00032990: 2020 2028 7069 6b5f 6461 7461 2e69 6e64     (pik_data.ind
-000329a0: 6578 2e67 6574 5f6c 6576 656c 5f76 616c  ex.get_level_val
-000329b0: 7565 7328 2763 6f6e 6469 2729 203d 3d20  ues('condi') == 
-000329c0: 2775 6e63 6f6e 6469 7469 6f6e 616c 2729  'unconditional')
-000329d0: 0a20 2020 2020 2020 2020 2020 2026 2028  .            & (
-000329e0: 7069 6b5f 6461 7461 2e69 6e64 6578 2e67  pik_data.index.g
-000329f0: 6574 5f6c 6576 656c 5f76 616c 7565 7328  et_level_values(
-00032a00: 2772 6765 2729 203d 3d20 2777 6f72 7374  'rge') == 'worst
-00032a10: 2729 0a20 2020 2020 2020 205d 0a20 2020  ').        ].   
-00032a20: 2020 2020 2070 6c65 6467 655f 6869 6768       pledge_high
-00032a30: 203d 2070 6c65 6467 655f 6869 6768 2e73   = pledge_high.s
-00032a40: 6574 5f69 6e64 6578 2870 6c65 6467 655f  et_index(pledge_
-00032a50: 6869 6768 2e6c 6f63 5b3a 2c20 2769 736f  high.loc[:, 'iso
-00032a60: 3327 5d29 2e6c 6f63 5b0a 2020 2020 2020  3']).loc[.      
-00032a70: 2020 2020 2020 3a2c 205b 7374 7228 7829        :, [str(x)
-00032a80: 2066 6f72 2078 2069 6e20 7261 6e67 6528   for x in range(
-00032a90: 3139 3930 2c20 3230 3331 295d 0a20 2020  1990, 2031)].   
-00032aa0: 2020 2020 205d 0a20 2020 2020 2020 2070       ].        p
-00032ab0: 6c65 6467 655f 6869 6768 203d 2064 742e  ledge_high = dt.
-00032ac0: 4461 7461 7461 626c 6528 0a20 2020 2020  Datatable(.     
-00032ad0: 2020 2020 2020 2070 6c65 6467 655f 6869         pledge_hi
-00032ae0: 6768 2c0a 2020 2020 2020 2020 2020 2020  gh,.            
-00032af0: 6d65 7461 3d7b 0a20 2020 2020 2020 2020  meta={.         
-00032b00: 2020 2020 2020 2027 656e 7469 7479 273a         'entity':
-00032b10: 2027 456d 6973 7369 6f6e 737c 4b59 4f54   'Emissions|KYOT
-00032b20: 4f47 4847 5f41 5234 272c 0a20 2020 2020  OGHG_AR4',.     
-00032b30: 2020 2020 2020 2020 2020 2027 6361 7465             'cate
-00032b40: 676f 7279 273a 2027 4e61 7469 6f6e 616c  gory': 'National
-00032b50: 5f74 6f74 616c 5f65 7863 6c5f 4c55 4c55  _total_excl_LULU
-00032b60: 4346 272c 0a20 2020 2020 2020 2020 2020  CF',.           
-00032b70: 2020 2020 2027 6d6f 6465 6c27 3a20 6627       'model': f'
-00032b80: 5049 4b5f 4e44 436d 6974 6951 7c7b 7365  PIK_NDCmitiQ|{se
-00032b90: 6c66 2e76 6572 7369 6f6e 7d27 2c0a 2020  lf.version}',.  
-00032ba0: 2020 2020 2020 2020 2020 2020 2020 2773                's
-00032bb0: 6365 6e61 7269 6f27 3a20 2750 6c65 6467  cenario': 'Pledg
-00032bc0: 655f 6869 6768 272c 0a20 2020 2020 2020  e_high',.       
-00032bd0: 2020 2020 2020 2020 2027 736f 7572 6365           'source
-00032be0: 273a 2073 656c 662e 7365 7475 702e 534f  ': self.setup.SO
-00032bf0: 5552 4345 5f49 442c 0a20 2020 2020 2020  URCE_ID,.       
-00032c00: 2020 2020 2020 2020 2027 756e 6974 273a           'unit':
-00032c10: 2027 4d74 2043 4f32 6571 272c 0a20 2020   'Mt CO2eq',.   
-00032c20: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00032c30: 2020 2020 290a 0a20 2020 2020 2020 2072      )..        r
-00032c40: 6574 7572 6e20 5b70 6c65 6467 655f 6869  eturn [pledge_hi
-00032c50: 6768 2c20 706c 6564 6765 5f6c 6f77 5d2c  gh, pledge_low],
-00032c60: 204e 6f6e 650a 0a0a 696d 706f 7274 2070   None...import p
-00032c70: 7961 6d0a 6672 6f6d 2074 7164 6d20 696d  yam.from tqdm im
-00032c80: 706f 7274 2074 7164 6d0a 0a0a 636c 6173  port tqdm...clas
-00032c90: 7320 4949 4153 4128 4261 7365 496d 706f  s IIASA(BaseImpo
-00032ca0: 7274 546f 6f6c 293a 0a20 2020 2064 6566  rtTool):.    def
-00032cb0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00032cc0: 736f 7572 6365 5f49 442c 2069 6961 7361  source_ID, iiasa
-00032cd0: 5f73 6f75 7263 653d 4e6f 6e65 2c20 6461  _source=None, da
-00032ce0: 7461 5f66 696c 653d 4e6f 6e65 2c20 6d65  ta_file=None, me
-00032cf0: 7461 5f66 696c 653d 4e6f 6e65 293a 0a20  ta_file=None):. 
-00032d00: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
-00032d10: 7020 3d20 7365 7475 7053 7472 7563 7428  p = setupStruct(
-00032d20: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00032d30: 7365 7475 702e 534f 5552 4345 5f49 4420  setup.SOURCE_ID 
-00032d40: 3d20 736f 7572 6365 5f49 440a 0a20 2020  = source_ID..   
-00032d50: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
-00032d60: 4441 5441 5f46 494c 4520 3d20 2727 0a20  DATA_FILE = ''. 
-00032d70: 2020 2020 2020 2023 2073 656c 662e 7365         # self.se
-00032d80: 7475 702e 4d41 5050 494e 475f 4649 4c45  tup.MAPPING_FILE
-00032d90: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-00032da0: 7365 6c66 2e73 6574 7570 2e53 4f55 5243  self.setup.SOURC
-00032db0: 455f 5041 5448 2c20 276d 6170 7069 6e67  E_PATH, 'mapping
-00032dc0: 2e78 6c73 7827 290a 2020 2020 2020 2020  .xlsx').        
-00032dd0: 7365 6c66 2e73 6574 7570 2e4c 4943 454e  self.setup.LICEN
-00032de0: 4345 203d 2027 3f27 2020 2320 544f 444f  CE = '?'  # TODO
-00032df0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00032e00: 7475 702e 5552 4c20 3d20 2764 6174 612e  tup.URL = 'data.
-00032e10: 656e 652e 6969 6173 612e 6163 2e61 7427  ene.iiasa.ac.at'
-00032e20: 0a0a 2020 2020 2020 2020 7365 6c66 2e53  ..        self.S
-00032e30: 4f55 5243 455f 4944 203d 2073 6f75 7263  OURCE_ID = sourc
-00032e40: 655f 4944 0a0a 2020 2020 2020 2020 6966  e_ID..        if
-00032e50: 2069 6961 7361 5f73 6f75 7263 6520 6973   iiasa_source is
-00032e60: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00032e70: 2020 2020 2020 2073 656c 662e 636f 6e6e         self.conn
-00032e80: 203d 2070 7961 6d2e 6969 6173 612e 436f   = pyam.iiasa.Co
-00032e90: 6e6e 6563 7469 6f6e 2869 6961 7361 5f73  nnection(iiasa_s
-00032ea0: 6f75 7263 6529 0a20 2020 2020 2020 2020  ource).         
-00032eb0: 2020 2073 656c 662e 6969 6173 615f 736f     self.iiasa_so
-00032ec0: 7572 6365 203d 2069 6961 7361 5f73 6f75  urce = iiasa_sou
-00032ed0: 7263 650a 2020 2020 2020 2020 2020 2020  rce.            
-00032ee0: 7365 6c66 2e6d 6574 6120 3d20 7365 6c66  self.meta = self
-00032ef0: 2e63 6f6e 6e2e 6d65 7461 2829 0a20 2020  .conn.meta().   
-00032f00: 2020 2020 2020 2020 2073 656c 662e 6170           self.ap
-00032f10: 6920 3d20 5472 7565 0a20 2020 2020 2020  i = True.       
-00032f20: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
-00032f30: 675f 6b65 7920 3d20 6969 6173 615f 736f  g_key = iiasa_so
-00032f40: 7572 6365 0a0a 2020 2020 2020 2020 656c  urce..        el
-00032f50: 6966 2064 6174 615f 6669 6c65 2069 7320  if data_file is 
-00032f60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00032f70: 2020 2020 2020 7365 6c66 2e64 6174 615f        self.data_
-00032f80: 6669 6c65 203d 2064 6174 615f 6669 6c65  file = data_file
-00032f90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00032fa0: 662e 6d65 7461 5f66 696c 6520 3d20 6d65  f.meta_file = me
-00032fb0: 7461 5f66 696c 650a 2020 2020 2020 2020  ta_file.        
-00032fc0: 2020 2020 7365 6c66 2e6d 6574 6120 3d20      self.meta = 
-00032fd0: 7064 2e44 6174 6146 7261 6d65 2829 0a20  pd.DataFrame(). 
-00032fe0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00032ff0: 6170 6920 3d20 4661 6c73 650a 2020 2020  api = False.    
-00033000: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
-00033010: 7069 6e67 5f6b 6579 203d 2073 6f75 7263  ping_key = sourc
-00033020: 655f 4944 0a0a 2020 2020 2020 2020 7365  e_ID..        se
-00033030: 6c66 2e72 6567 696f 6e5f 6d61 7070 696e  lf.region_mappin
-00033040: 6720 3d20 6469 6374 2829 0a0a 2020 2020  g = dict()..    
-00033050: 2020 2020 0a20 2020 2020 2020 200a 2020      .        .  
-00033060: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
-00033070: 6e5f 6d61 7070 696e 675b 2769 616d 6331  n_mapping['iamc1
-00033080: 3527 5d20 3d6d 6170 7069 6e67 2e49 5043  5'] =mapping.IPC
-00033090: 435f 5352 3135 2829 2e72 6567 696f 6e5f  C_SR15().region_
-000330a0: 6d61 7070 696e 6728 290a 2020 2020 2020  mapping().      
-000330b0: 2020 7365 6c66 2e72 6567 696f 6e5f 6d61    self.region_ma
-000330c0: 7070 696e 675b 2749 5043 435f 5352 3135  pping['IPCC_SR15
-000330d0: 275d 203d 2073 656c 662e 7265 6769 6f6e  '] = self.region
-000330e0: 5f6d 6170 7069 6e67 5b27 6961 6d63 3135  _mapping['iamc15
-000330f0: 275d 0a20 2020 2020 2020 2073 656c 662e  '].        self.
-00033100: 7265 6769 6f6e 5f6d 6170 7069 6e67 5b22  region_mapping["
-00033110: 4941 4d43 3135 5f32 3031 395f 5232 225d  IAMC15_2019_R2"]
-00033120: 203d 2073 656c 662e 7265 6769 6f6e 5f6d   = self.region_m
-00033130: 6170 7069 6e67 5b22 6961 6d63 3135 225d  apping["iamc15"]
-00033140: 2020 0a20 2020 2020 2020 200a 2020 2020    .        .    
-00033150: 2020 2020 7365 6c66 2e72 6567 696f 6e5f      self.region_
-00033160: 6d61 7070 696e 675b 2743 445f 4c49 4e4b  mapping['CD_LINK
-00033170: 5327 5d20 3d6d 6170 7069 6e67 2e43 445f  S'] =mapping.CD_
-00033180: 4c49 4e4b 5328 292e 7265 6769 6f6e 5f6d  LINKS().region_m
-00033190: 6170 7069 6e67 2829 0a20 2020 2020 2020  apping().       
-000331a0: 200a 2020 2020 2020 2020 7365 6c66 2e72   .        self.r
-000331b0: 6567 696f 6e5f 6d61 7070 696e 675b 2765  egion_mapping['e
-000331c0: 6e67 6167 6527 5d20 3d6d 6170 7069 6e67  ngage'] =mapping
-000331d0: 2e45 4e47 4147 4528 292e 7265 6769 6f6e  .ENGAGE().region
-000331e0: 5f6d 6170 7069 6e67 2829 0a20 2020 2020  _mapping().     
-000331f0: 2020 200a 2020 2020 2020 2020 7365 6c66     .        self
-00033200: 2e72 6567 696f 6e5f 6d61 7070 696e 675b  .region_mapping[
-00033210: 2749 5043 435f 4152 3527 5d20 3d20 6d61  'IPCC_AR5'] = ma
-00033220: 7070 696e 672e 4950 4343 5f41 5235 2829  pping.IPCC_AR5()
-00033230: 2e72 6567 696f 6e5f 6d61 7070 696e 6728  .region_mapping(
-00033240: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00033250: 7265 6769 6f6e 5f6d 6170 7069 6e67 5b27  region_mapping['
-00033260: 4950 4343 5f41 5236 275d 203d 206d 6170  IPCC_AR6'] = map
-00033270: 7069 6e67 2e49 5043 435f 4152 3628 292e  ping.IPCC_AR6().
-00033280: 7265 6769 6f6e 5f6d 6170 7069 6e67 2829  region_mapping()
-00033290: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-000332a0: 6769 6f6e 5f6d 6170 7069 6e67 5b27 4950  gion_mapping['IP
-000332b0: 4343 5f41 5236 5f72 6177 275d 203d 206d  CC_AR6_raw'] = m
-000332c0: 6170 7069 6e67 2e49 5043 435f 4152 3628  apping.IPCC_AR6(
-000332d0: 292e 7265 6769 6f6e 5f6d 6170 7069 6e67  ).region_mapping
-000332e0: 2829 0a0a 2020 2020 2020 2020 7365 6c66  ()..        self
-000332f0: 2e72 6567 696f 6e5f 6d61 7070 696e 675b  .region_mapping[
-00033300: 276e 6766 735f 3227 5d20 3d20 6d61 7070  'ngfs_2'] = mapp
-00033310: 696e 672e 4e47 4653 2829 2e72 6567 696f  ing.NGFS().regio
-00033320: 6e5f 6d61 7070 696e 6728 290a 0a20 2020  n_mapping()..   
-00033330: 2020 2020 2073 656c 662e 7265 6769 6f6e       self.region
-00033340: 5f6d 6170 7069 6e67 5b27 4144 5641 4e43  _mapping['ADVANC
-00033350: 4527 5d20 3d20 6d61 7070 696e 672e 4144  E'] = mapping.AD
-00033360: 5641 4e43 4528 292e 7265 6769 6f6e 5f6d  VANCE().region_m
-00033370: 6170 7069 6e67 2829 0a0a 2020 2020 6465  apping()..    de
-00033380: 6620 6164 6170 745f 756e 6974 7328 7365  f adapt_units(se
-00033390: 6c66 2c20 6d65 7461 293a 0a20 2020 2020  lf, meta):.     
-000333a0: 2020 206d 6574 615b 2775 6e69 7427 5d20     meta['unit'] 
-000333b0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-000333c0: 6d65 7461 5b27 756e 6974 275d 0a20 2020  meta['unit'].   
-000333d0: 2020 2020 2020 2020 202e 7265 706c 6163           .replac
-000333e0: 6528 276b 7455 272c 2027 6b74 2055 2729  e('ktU', 'kt U')
-000333f0: 0a20 2020 2020 2020 2020 2020 202e 7265  .            .re
-00033400: 706c 6163 6528 274d 7420 434f 322d 6571  place('Mt CO2-eq
-00033410: 7569 762f 7972 272c 2027 4d74 2043 4f32  uiv/yr', 'Mt CO2
-00033420: 6571 2f79 7227 290a 2020 2020 2020 2020  eq/yr').        
-00033430: 2020 2020 2e72 6570 6c61 6365 2827 6b74      .replace('kt
-00033440: 2043 4634 2d65 7175 6976 2f79 272c 2027   CF4-equiv/y', '
-00033450: 6b74 2043 4634 6571 2f79 2729 0a20 2020  kt CF4eq/y').   
-00033460: 2020 2020 2020 2020 202e 7265 706c 6163           .replac
-00033470: 6528 276b 7420 4846 4331 3334 612d 6571  e('kt HFC134a-eq
-00033480: 7569 762f 7972 272c 2027 6b74 2048 4643  uiv/yr', 'kt HFC
-00033490: 3133 3461 6571 2f79 7227 290a 2020 2020  134aeq/yr').    
-000334a0: 2020 2020 2020 2020 2e72 6570 6c61 6365          .replace
-000334b0: 2827 496e 6465 7820 2832 3030 3520 3d20  ('Index (2005 = 
-000334c0: 3129 272c 2027 6469 6d65 6e73 696f 6e6c  1)', 'dimensionl
-000334d0: 6573 7327 2920 2023 203f 3f20 544f 444f  ess')  # ?? TODO
-000334e0: 0a20 2020 2020 2020 2020 2020 202e 7265  .            .re
-000334f0: 706c 6163 6528 2755 5324 272c 2027 5553  place('US$', 'US
-00033500: 4427 290a 2020 2020 2020 2020 2020 2020  D').            
-00033510: 2e72 6570 6c61 6365 2827 6b74 2048 4643  .replace('kt HFC
-00033520: 3433 2d31 302f 7972 272c 2027 6b74 2048  43-10/yr', 'kt H
-00033530: 4643 3433 5f31 302f 7972 2729 0a20 2020  FC43_10/yr').   
-00033540: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
-00033550: 6574 7572 6e20 6d65 7461 0a0a 2020 2020  eturn meta..    
-00033560: 6465 6620 6761 7468 6572 4d61 7070 6564  def gatherMapped
-00033570: 4461 7461 2873 656c 662c 206d 6f64 656c  Data(self, model
-00033580: 733d 4e6f 6e65 2c20 6961 6d63 5f66 696c  s=None, iamc_fil
-00033590: 7465 723d 5b5d 293a 0a0a 2020 2020 2020  ter=[]):..      
-000335a0: 2020 7461 626c 6573 203d 206c 6973 7428    tables = list(
-000335b0: 290a 2020 2020 2020 2020 7461 626c 6573  ).        tables
-000335c0: 5f65 7863 6c75 6465 6420 3d20 6c69 7374  _excluded = list
-000335d0: 2829 0a0a 2020 2020 2020 2020 6966 206e  ()..        if n
-000335e0: 6f74 2068 6173 6174 7472 2873 656c 662c  ot hasattr(self,
-000335f0: 2027 6461 7461 2729 3a0a 2020 2020 2020   'data'):.      
-00033600: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00033610: 662e 6170 693a 0a20 2020 2020 2020 2020  f.api:.         
-00033620: 2020 2020 2020 2023 206c 6f61 6420 6461         # load da
-00033630: 7461 0a20 2020 2020 2020 2020 2020 2020  ta.             
-00033640: 2020 2073 656c 662e 6c6f 6164 4461 7461     self.loadData
-00033650: 2829 0a20 2020 2020 2020 200a 2020 2020  ().        .    
-00033660: 2020 2020 6966 2027 6d6f 6465 6c27 206e      if 'model' n
-00033670: 6f74 2069 6e20 6961 6d63 5f66 696c 7465  ot in iamc_filte
-00033680: 722e 6b65 7973 2829 3a0a 2020 2020 2020  r.keys():.      
-00033690: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-000336a0: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-000336b0: 6966 206d 6f64 656c 7320 6973 204e 6f6e  if models is Non
-000336c0: 653a 0a20 2020 200a 2020 2020 2020 2020  e:.    .        
-000336d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000336e0: 6170 693a 0a20 2020 2020 2020 2020 2020  api:.           
-000336f0: 2020 2020 2020 2020 206d 6f64 656c 7320           models 
-00033700: 3d20 7365 6c66 2e6d 6574 612e 696e 6465  = self.meta.inde
-00033710: 782e 6765 745f 6c65 7665 6c5f 7661 6c75  x.get_level_valu
-00033720: 6573 2830 292e 756e 6971 7565 2829 0a20  es(0).unique(). 
-00033730: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00033740: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00033750: 2020 2020 2020 2020 206d 6f64 656c 7320           models 
-00033760: 3d20 7365 6c66 2e64 6174 612e 6d6f 6465  = self.data.mode
-00033770: 6c0a 2020 2020 0a20 2020 2020 2020 2020  l.    .         
-00033780: 2020 2066 6f72 206d 6f64 656c 2069 6e20     for model in 
-00033790: 7471 646d 286d 6f64 656c 732c 2064 6573  tqdm(models, des
-000337a0: 633d 274c 6f6f 7020 6f76 6572 206d 6f64  c='Loop over mod
-000337b0: 656c 7327 293a 0a20 2020 200a 2020 2020  els'):.    .    
-000337c0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000337d0: 656c 662e 6170 693a 0a20 2020 2020 2020  elf.api:.       
-000337e0: 2020 2020 2020 2020 2020 2020 2069 6466               idf
-000337f0: 203d 2073 656c 662e 636f 6e6e 2e71 7565   = self.conn.que
-00033800: 7279 282a 2a69 616d 635f 6669 6c74 6572  ry(**iamc_filter
-00033810: 2c20 6d6f 6465 6c3d 6d6f 6465 6c29 0a20  , model=model). 
-00033820: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00033830: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00033840: 2020 2020 2020 2020 2069 6466 203d 2073           idf = s
-00033850: 656c 662e 6461 7461 2e66 696c 7465 7228  elf.data.filter(
-00033860: 2a2a 6961 6d63 5f66 696c 7465 722c 206d  **iamc_filter, m
-00033870: 6f64 656c 3d6d 6f64 656c 290a 2020 2020  odel=model).    
-00033880: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00033890: 2e69 6466 203d 2069 6466 0a20 2020 2020  .idf = idf.     
-000338a0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-000338b0: 6e28 6964 6629 203d 3d20 303a 0a20 2020  n(idf) == 0:.   
-000338c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000338d0: 2063 6f6e 7469 6e75 650a 2020 2020 0a20   continue.    . 
-000338e0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000338f0: 6162 6c65 732c 2074 6162 6c65 735f 6578  ables, tables_ex
-00033900: 636c 7564 6564 203d 2073 656c 662e 5f72  cluded = self._r
-00033910: 6561 645f 6964 665f 6461 7461 280a 2020  ead_idf_data(.  
-00033920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033930: 2020 6964 662c 206d 6f64 656c 2c20 7461    idf, model, ta
-00033940: 626c 6573 2c20 7461 626c 6573 5f65 7863  bles, tables_exc
-00033950: 6c75 6465 640a 2020 2020 2020 2020 2020  luded.          
-00033960: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00033970: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00033980: 2069 6620 7365 6c66 2e61 7069 3a0a 2020   if self.api:.  
-00033990: 2020 2020 2020 2020 2020 2020 2069 6466               idf
-000339a0: 203d 2073 656c 662e 636f 6e6e 2e71 7565   = self.conn.que
-000339b0: 7279 282a 2a69 616d 635f 6669 6c74 6572  ry(**iamc_filter
-000339c0: 290a 2020 2020 2020 2020 2020 2065 6c73  ).           els
-000339d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000339e0: 2020 6964 6620 3d20 7365 6c66 2e64 6174    idf = self.dat
-000339f0: 612e 6669 6c74 6572 282a 2a69 616d 635f  a.filter(**iamc_
-00033a00: 6669 6c74 6572 290a 2020 2020 2020 2020  filter).        
-00033a10: 2020 2073 656c 662e 6964 6620 3d20 6964     self.idf = id
-00033a20: 660a 2020 2020 2020 2020 2020 200a 2020  f.           .  
-00033a30: 200a 2020 2020 2020 2020 2020 2066 6f72   .           for
-00033a40: 206d 6f64 656c 2069 6e20 6964 662e 6d6f   model in idf.mo
-00033a50: 6465 6c3a 200a 2020 2020 2020 2020 2020  del: .          
-00033a60: 2020 2020 2069 6466 5f73 656c 203d 2069       idf_sel = i
-00033a70: 6466 2e66 696c 7465 7228 6d6f 6465 6c3d  df.filter(model=
-00033a80: 6d6f 6465 6c29 0a20 2020 2020 2020 2020  model).         
-00033a90: 2020 2020 2020 6966 206c 656e 2869 6466        if len(idf
-00033aa0: 5f73 656c 2920 3d3d 2030 3a0a 2020 2020  _sel) == 0:.    
-00033ab0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00033ac0: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-00033ad0: 2020 2020 2020 2074 6162 6c65 732c 2074         tables, t
-00033ae0: 6162 6c65 735f 6578 636c 7564 6564 203d  ables_excluded =
-00033af0: 2073 656c 662e 5f72 6561 645f 6964 665f   self._read_idf_
-00033b00: 6461 7461 280a 2020 2020 2020 2020 2020  data(.          
-00033b10: 2020 2020 2020 2020 2069 6466 5f73 656c           idf_sel
-00033b20: 2c20 6d6f 6465 6c2c 2074 6162 6c65 732c  , model, tables,
-00033b30: 2074 6162 6c65 735f 6578 636c 7564 6564   tables_excluded
-00033b40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00033b50: 2020 0a0a 2020 2020 2020 2020 7265 7475    ..        retu
-00033b60: 726e 2074 6162 6c65 732c 2074 6162 6c65  rn tables, table
-00033b70: 735f 6578 636c 7564 6564 0a0a 2020 2020  s_excluded..    
-00033b80: 6465 6620 5f72 6561 645f 6461 7461 2873  def _read_data(s
-00033b90: 656c 662c 2064 6174 615f 6669 6c65 2c20  elf, data_file, 
-00033ba0: 6d65 7461 5f66 696c 653d 4e6f 6e65 2c20  meta_file=None, 
-00033bb0: 2a2a 6669 6c74 6572 7329 3a0a 2020 2020  **filters):.    
-00033bc0: 2020 2020 7072 696e 7428 6627 7265 6164      print(f'read
-00033bd0: 696e 6720 696e 3a20 207b 6461 7461 5f66  ing in:  {data_f
-00033be0: 696c 657d 2729 0a20 2020 2020 2020 2064  ile}').        d
-00033bf0: 6174 6120 3d20 7079 616d 2e49 616d 4461  ata = pyam.IamDa
-00033c00: 7461 4672 616d 6528 6474 2e74 6f6f 6c73  taFrame(dt.tools
-00033c10: 2e70 7961 6d2e 7265 6164 5f70 6172 7469  .pyam.read_parti
-00033c20: 616c 2864 6174 615f 6669 6c65 2c20 2a2a  al(data_file, **
-00033c30: 6669 6c74 6572 7329 290a 2020 2020 2020  filters)).      
-00033c40: 2020 6966 206d 6574 615f 6669 6c65 2069    if meta_file i
-00033c50: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00033c60: 2020 2020 2020 2020 6461 7461 2e6c 6f61          data.loa
-00033c70: 645f 6d65 7461 286d 6574 615f 6669 6c65  d_meta(meta_file
-00033c80: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00033c90: 6e20 6461 7461 0a0a 2020 2020 6465 6620  n data..    def 
-00033ca0: 6c6f 6164 4461 7461 2873 656c 662c 202a  loadData(self, *
-00033cb0: 2a66 696c 7465 7273 293a 0a0a 2020 2020  *filters):..    
-00033cc0: 2020 2020 2320 7365 6c66 2e64 6174 6120      # self.data 
-00033cd0: 3d20 7064 2e72 6561 645f 6373 7628 7365  = pd.read_csv(se
-00033ce0: 6c66 2e64 6174 615f 6669 6c65 290a 2020  lf.data_file).  
-00033cf0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00033d00: 6e63 6528 7365 6c66 2e64 6174 615f 6669  nce(self.data_fi
-00033d10: 6c65 2c20 6c69 7374 2920 616e 6420 6973  le, list) and is
-00033d20: 696e 7374 616e 6365 2873 656c 662e 6461  instance(self.da
-00033d30: 7461 5f66 696c 652c 206c 6973 7429 3a0a  ta_file, list):.
-00033d40: 2020 2020 2020 2020 2020 2020 2320 6d75              # mu
-00033d50: 6c74 6970 6c65 2066 696c 6573 0a20 2020  ltiple files.   
-00033d60: 2020 2020 2020 2020 2064 6174 615f 6c69           data_li
-00033d70: 7374 203d 206c 6973 7428 290a 2020 2020  st = list().    
-00033d80: 2020 2020 2020 2020 666f 7220 6461 7461          for data
-00033d90: 5f66 696c 652c 206d 6574 615f 6669 6c65  _file, meta_file
-00033da0: 2069 6e20 7a69 7028 7365 6c66 2e64 6174   in zip(self.dat
-00033db0: 615f 6669 6c65 2c20 7365 6c66 2e6d 6574  a_file, self.met
-00033dc0: 615f 6669 6c65 293a 0a0a 2020 2020 2020  a_file):..      
-00033dd0: 2020 2020 2020 2020 2020 6461 7461 5f6c            data_l
-00033de0: 6973 742e 6170 7065 6e64 2873 656c 662e  ist.append(self.
-00033df0: 5f72 6561 645f 6461 7461 2864 6174 615f  _read_data(data_
-00033e00: 6669 6c65 2c20 6d65 7461 5f66 696c 652c  file, meta_file,
-00033e10: 202a 2a66 696c 7465 7273 2929 0a0a 2020   **filters))..  
-00033e20: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00033e30: 6174 6120 3d20 7079 616d 2e63 6f6e 6361  ata = pyam.conca
-00033e40: 7428 6461 7461 5f6c 6973 7429 0a20 2020  t(data_list).   
-00033e50: 2020 2020 2020 2020 2073 656c 662e 6d65           self.me
-00033e60: 7461 203d 2073 656c 662e 6461 7461 2e6d  ta = self.data.m
-00033e70: 6574 610a 2020 2020 2020 2020 2020 2020  eta.            
-00033e80: 6465 6c20 6461 7461 5f6c 6973 740a 2020  del data_list.  
-00033e90: 2020 2020 2020 2020 2020 2320 6465 6c20            # del 
-00033ea0: 6461 7461 0a0a 2020 2020 2020 2020 656c  data..        el
-00033eb0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00033ec0: 2320 7369 6e67 6c65 2066 696c 650a 2020  # single file.  
-00033ed0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00033ee0: 6174 6120 3d20 7365 6c66 2e5f 7265 6164  ata = self._read
-00033ef0: 5f64 6174 6128 7365 6c66 2e64 6174 615f  _data(self.data_
-00033f00: 6669 6c65 2c20 7365 6c66 2e6d 6574 615f  file, self.meta_
-00033f10: 6669 6c65 2c20 2a2a 6669 6c74 6572 7329  file, **filters)
-00033f20: 0a20 2020 2020 2020 2023 2073 6574 7469  .        # setti
-00033f30: 6e67 206d 6574 610a 2020 2020 2020 2020  ng meta.        
-00033f40: 7365 6c66 2e6d 6574 6120 3d20 7365 6c66  self.meta = self
-00033f50: 2e64 6174 612e 6d65 7461 0a0a 2020 2020  .data.meta..    
-00033f60: 6465 6620 5f72 6561 645f 6964 665f 6461  def _read_idf_da
-00033f70: 7461 2873 656c 662c 2069 6466 2c20 6d6f  ta(self, idf, mo
-00033f80: 6465 6c2c 2074 6162 6c65 732c 2074 6162  del, tables, tab
-00033f90: 6c65 735f 6578 636c 7564 6564 293a 0a0a  les_excluded):..
-00033fa0: 2020 2020 2020 2020 7764 6620 3d20 6964          wdf = id
-00033fb0: 662e 7469 6d65 7365 7269 6573 2829 0a20  f.timeseries(). 
-00033fc0: 2020 2020 2020 2066 6f72 2073 6365 6e61         for scena
-00033fd0: 7269 6f20 696e 2077 6466 2e69 6e64 6578  rio in wdf.index
-00033fe0: 2e67 6574 5f6c 6576 656c 5f76 616c 7565  .get_level_value
-00033ff0: 7328 3129 2e75 6e69 7175 6528 293a 0a20  s(1).unique():. 
-00034000: 2020 2020 2020 2020 2020 2073 7562 5f73             sub_s
-00034010: 6365 6e61 7269 6f20 3d20 7764 662e 6c6f  cenario = wdf.lo
-00034020: 635b 736c 6963 6528 4e6f 6e65 292c 205b  c[slice(None), [
-00034030: 7363 656e 6172 696f 5d2c 2073 6c69 6365  scenario], slice
-00034040: 284e 6f6e 6529 2c20 736c 6963 6528 4e6f  (None), slice(No
-00034050: 6e65 295d 0a0a 2020 2020 2020 2020 2020  ne)]..          
-00034060: 2020 666f 7220 7661 7220 696e 2073 7562    for var in sub
-00034070: 5f73 6365 6e61 7269 6f2e 696e 6465 782e  _scenario.index.
-00034080: 6765 745f 6c65 7665 6c5f 7661 6c75 6573  get_level_values
-00034090: 2833 292e 756e 6971 7565 2829 3a0a 2020  (3).unique():.  
-000340a0: 2020 2020 2020 2020 2020 2020 2020 7375                su
-000340b0: 6273 6574 203d 2028 0a20 2020 2020 2020  bset = (.       
-000340c0: 2020 2020 2020 2020 2020 2020 2073 7562               sub
-000340d0: 5f73 6365 6e61 7269 6f2e 6c6f 635b 736c  _scenario.loc[sl
-000340e0: 6963 6528 4e6f 6e65 292c 2073 6c69 6365  ice(None), slice
-000340f0: 284e 6f6e 6529 2c20 736c 6963 6528 4e6f  (None), slice(No
-00034100: 6e65 292c 205b 7661 725d 5d0a 2020 2020  ne), [var]].    
-00034110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00034120: 2e72 6573 6574 5f69 6e64 6578 2829 0a20  .reset_index(). 
-00034130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00034140: 2020 202e 7365 745f 696e 6465 7828 2772     .set_index('r
-00034150: 6567 696f 6e27 290a 2020 2020 2020 2020  egion').        
-00034160: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00034170: 2020 2020 2020 2020 2020 2074 696d 655f             time_
-00034180: 636f 6c73 203d 2064 742e 7574 696c 2e79  cols = dt.util.y
-00034190: 6561 7273 436f 6c75 6d6e 734f 6e6c 7928  earsColumnsOnly(
-000341a0: 7375 6273 6574 2e63 6f6c 756d 6e73 290a  subset.columns).
+0002fe20: 2020 2020 2020 6474 2e69 6f2e 6578 6365        dt.io.exce
+0002fe30: 6c49 6478 3250 616e 6461 7349 6478 2878  lIdx2PandasIdx(x
+0002fe40: 2920 666f 7220 7820 696e 2073 6574 7570  ) for x in setup
+0002fe50: 5b27 7370 6163 6549 6478 4c69 7374 275d  ['spaceIdxList']
+0002fe60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002fe70: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
+0002fe80: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0002fe90: 2020 2020 2020 2020 6966 2022 496e 7465          if "Inte
+0002fea0: 726e 6174 696f 6e61 6c22 2069 6e20 6d65  rnational" in me
+0002feb0: 7461 4466 5b27 4e61 6d65 275d 3a0a 2020  taDf['Name']:.  
+0002fec0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0002fed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002fee0: 2020 2073 6466 0a20 2020 2020 2020 2020     sdf.         
+0002fef0: 2020 2020 2020 2069 6620 6578 2e73 7061         if ex.spa
+0002ff00: 6365 4964 784c 6973 745b 305d 5b30 5d20  ceIdxList[0][0] 
+0002ff10: 3e20 3531 2061 6e64 2072 6567 696f 6e20  > 51 and region 
+0002ff20: 213d 2027 576f 726c 6427 3a0a 2020 2020  != 'World':.    
+0002ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ff40: 6578 2e73 7061 6365 4964 784c 6973 7420  ex.spaceIdxList 
+0002ff50: 3d20 5b28 6578 2e73 7061 6365 4964 784c  = [(ex.spaceIdxL
+0002ff60: 6973 745b 305d 5b30 5d20 2d20 312c 2030  ist[0][0] - 1, 0
+0002ff70: 295d 0a0a 2020 2020 2020 2020 2020 2020  )]..            
+0002ff80: 2020 2020 6966 2069 203d 3d20 303a 0a20      if i == 0:. 
+0002ff90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ffa0: 2020 2064 6620 3d20 6578 2e67 6174 6865     df = ex.gathe
+0002ffb0: 7244 6174 6128 290a 2020 2020 2020 2020  rData().        
+0002ffc0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0002ffd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ffe0: 2020 6466 203d 2065 782e 6761 7468 6572    df = ex.gather
+0002fff0: 4461 7461 286c 6f61 643d 4661 6c73 6529  Data(load=False)
+00030000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00030010: 2070 7269 6e74 2864 6629 0a20 2020 2020   print(df).     
+00030020: 2020 2020 2020 2020 2020 2064 6620 3d20             df = 
+00030030: 6466 2e6c 6f63 5b3a 2c20 7965 6172 7343  df.loc[:, yearsC
+00030040: 6f6c 756d 6e73 4f6e 6c79 2864 6629 5d0a  olumnsOnly(df)].
+00030050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030060: 6466 2e63 6f6c 756d 6e73 203d 2064 662e  df.columns = df.
+00030070: 636f 6c75 6d6e 732e 6173 7479 7065 2869  columns.astype(i
+00030080: 6e74 290a 2020 2020 2020 2020 2020 2020  nt).            
+00030090: 2020 2020 6d65 7461 4469 6374 203d 2064      metaDict = d
+000300a0: 6963 7428 290a 2020 2020 2020 2020 2020  ict().          
+000300b0: 2020 2020 2020 6d65 7461 4469 6374 5b27        metaDict['
+000300c0: 656e 7469 7479 275d 203d 206d 6574 6144  entity'] = metaD
+000300d0: 665b 274e 616d 6527 5d2e 7374 7269 7028  f['Name'].strip(
+000300e0: 292e 7265 706c 6163 6528 277c 2027 2c20  ).replace('| ', 
+000300f0: 277c 2729 0a20 2020 2020 2020 2020 2020  '|').           
+00030100: 2020 2020 206d 6574 6144 6963 745b 2763       metaDict['c
+00030110: 6174 6567 6f72 7927 5d20 3d20 2727 0a20  ategory'] = ''. 
+00030120: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00030130: 6574 6144 6963 745b 2775 6e69 7427 5d20  etaDict['unit'] 
+00030140: 3d20 6d65 7461 4466 5b27 756e 6974 275d  = metaDf['unit']
+00030150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00030160: 206d 6574 6144 6963 745b 2773 6365 6e61   metaDict['scena
+00030170: 7269 6f27 5d20 3d20 6d65 7461 4466 5b27  rio'] = metaDf['
+00030180: 5363 656e 6172 696f 275d 0a20 2020 2020  Scenario'].     
+00030190: 2020 2020 2020 2020 2020 206d 6574 6144             metaD
+000301a0: 6963 745b 2773 6f75 7263 6527 5d20 3d20  ict['source'] = 
+000301b0: 7365 6c66 2e73 6574 7570 2e53 4f55 5243  self.setup.SOURC
+000301c0: 455f 4944 0a20 2020 2020 2020 2020 2020  E_ID.           
+000301d0: 2020 2020 206d 6574 6144 6963 745b 2775       metaDict['u
+000301e0: 6e69 7454 6f27 5d20 3d20 6d65 7461 4466  nitTo'] = metaDf
+000301f0: 5b27 756e 6974 546f 275d 0a0a 2020 2020  ['unitTo']..    
+00030200: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+00030210: 4469 6374 203d 2064 742e 636f 7265 2e5f  Dict = dt.core._
+00030220: 7570 6461 7465 5f6d 6574 6128 6d65 7461  update_meta(meta
+00030230: 4469 6374 290a 2020 2020 2020 2020 2020  Dict).          
+00030240: 2020 2020 2020 4944 203d 2064 742e 636f        ID = dt.co
+00030250: 7265 2e5f 6372 6561 7465 4461 7461 6261  re._createDataba
+00030260: 7365 4944 286d 6574 6144 6963 7429 0a20  seID(metaDict). 
+00030270: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00030280: 6f49 534f 203d 2073 656c 662e 7370 6174  oISO = self.spat
+00030290: 6961 6c4d 6170 7069 6e67 2e6c 6f63 5b72  ialMapping.loc[r
+000302a0: 6567 696f 6e2c 2027 6d61 7070 696e 6727  egion, 'mapping'
+000302b0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000302c0: 2020 6966 2049 4420 6e6f 7420 696e 2074    if ID not in t
+000302d0: 6162 6c65 7354 6f43 6f6d 6d69 742e 6b65  ablesToCommit.ke
+000302e0: 7973 2829 3a0a 2020 2020 2020 2020 2020  ys():.          
+000302f0: 2020 2020 2020 2020 2020 7461 626c 6520            table 
+00030300: 3d20 6474 2e44 6174 6174 6162 6c65 2863  = dt.Datatable(c
+00030310: 6f6c 756d 6e73 3d72 616e 6765 2832 3030  olumns=range(200
+00030320: 302c 2032 3130 3029 2c20 6d65 7461 3d6d  0, 2100), meta=m
+00030330: 6574 6144 6963 7429 0a0a 2020 2020 2020  etaDict)..      
+00030340: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+00030350: 626c 652e 6c6f 635b 636f 4953 4f2c 2064  ble.loc[coISO, d
+00030360: 662e 636f 6c75 6d6e 735d 203d 2064 662e  f.columns] = df.
+00030370: 7661 6c75 6573 0a20 2020 2020 2020 2020  values.         
+00030380: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+00030390: 7354 6f43 6f6d 6d69 742e 6164 6428 7461  sToCommit.add(ta
+000303a0: 626c 6529 0a20 2020 2020 2020 2020 2020  ble).           
+000303b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000303c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000303d0: 6162 6c65 203d 2074 6162 6c65 7354 6f43  able = tablesToC
+000303e0: 6f6d 6d69 745b 4944 5d0a 2020 2020 2020  ommit[ID].      
+000303f0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+00030400: 626c 652e 6c6f 635b 636f 4953 4f2c 2064  ble.loc[coISO, d
+00030410: 662e 636f 6c75 6d6e 735d 203d 2064 662e  f.columns] = df.
+00030420: 7661 6c75 6573 0a0a 2020 2020 2020 2020  values..        
+00030430: 7461 626c 6573 4c69 7374 203d 206c 6973  tablesList = lis
+00030440: 7428 290a 2020 2020 2020 2020 666f 7220  t().        for 
+00030450: 4944 2069 6e20 7461 626c 6573 546f 436f  ID in tablesToCo
+00030460: 6d6d 6974 2e6b 6579 7328 293a 0a20 2020  mmit.keys():.   
+00030470: 2020 2020 2020 2020 2064 6174 6154 6162           dataTab
+00030480: 6c65 203d 2074 6162 6c65 7354 6f43 6f6d  le = tablesToCom
+00030490: 6d69 745b 4944 5d0a 2020 2020 2020 2020  mit[ID].        
+000304a0: 2020 2020 7072 696e 7428 6461 7461 5461      print(dataTa
+000304b0: 626c 652e 6d65 7461 290a 2020 2020 2020  ble.meta).      
+000304c0: 2020 2020 2020 6966 206e 6f74 2070 642e        if not pd.
+000304d0: 6973 6e61 2864 6174 6154 6162 6c65 2e6d  isna(dataTable.m
+000304e0: 6574 615b 2775 6e69 7454 6f27 5d29 3a0a  eta['unitTo']):.
+000304f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030500: 6461 7461 5461 626c 6520 3d20 6461 7461  dataTable = data
+00030510: 5461 626c 652e 636f 6e76 6572 7428 6461  Table.convert(da
+00030520: 7461 5461 626c 652e 6d65 7461 5b27 756e  taTable.meta['un
+00030530: 6974 546f 275d 290a 2020 2020 2020 2020  itTo']).        
+00030540: 2020 2020 2020 2020 6465 6c20 6461 7461          del data
+00030550: 5461 626c 652e 6d65 7461 5b27 756e 6974  Table.meta['unit
+00030560: 546f 275d 0a20 2020 2020 2020 2020 2020  To'].           
+00030570: 2074 6162 6c65 734c 6973 742e 6170 7065   tablesList.appe
+00030580: 6e64 2864 6174 6154 6162 6c65 2e61 7374  nd(dataTable.ast
+00030590: 7970 6528 666c 6f61 7429 290a 0a20 2020  ype(float))..   
+000305a0: 2020 2020 2072 6574 7572 6e20 7461 626c       return tabl
+000305b0: 6573 4c69 7374 2c20 5b5d 0a0a 0a63 6c61  esList, []...cla
+000305c0: 7373 2045 4e45 5244 4154 4128 4261 7365  ss ENERDATA(Base
+000305d0: 496d 706f 7274 546f 6f6c 293a 0a20 2020  ImportTool):.   
+000305e0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+000305f0: 6c66 2c20 7965 6172 3d32 3031 392c 2064  lf, year=2019, d
+00030600: 6174 615f 7061 7468 3d4e 6f6e 652c 2066  ata_path=None, f
+00030610: 696c 656e 616d 653d 4e6f 6e65 293a 0a0a  ilename=None):..
+00030620: 2020 2020 2020 2020 6966 2064 6174 615f          if data_
+00030630: 7061 7468 2069 7320 4e6f 6e65 3a0a 2020  path is None:.  
+00030640: 2020 2020 2020 2020 2020 6461 7461 5f70            data_p
+00030650: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
+00030660: 696e 2863 6f6e 6669 672e 5041 5448 5f54  in(config.PATH_T
+00030670: 4f5f 4441 5441 5348 454c 462c 2027 7261  O_DATASHELF, 'ra
+00030680: 7764 6174 6127 290a 0a20 2020 2020 2020  wdata')..       
+00030690: 2069 6620 6669 6c65 6e61 6d65 2069 7320   if filename is 
+000306a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000306b0: 2020 6669 6c65 6e61 6d65 203d 2066 2765    filename = f'e
+000306c0: 6e65 7264 6174 615f 7b79 6561 727d 2e78  nerdata_{year}.x
+000306d0: 6c73 7827 0a20 2020 2020 2020 2073 656c  lsx'.        sel
+000306e0: 662e 7365 7475 7020 3d20 7365 7475 7053  f.setup = setupS
+000306f0: 7472 7563 7428 290a 2020 2020 2020 2020  truct().        
+00030700: 7365 6c66 2e73 6574 7570 2e53 4f55 5243  self.setup.SOURC
+00030710: 455f 4944 203d 2022 454e 4552 4441 5441  E_ID = "ENERDATA
+00030720: 5f22 202b 2073 7472 2879 6561 7229 0a20  _" + str(year). 
+00030730: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
+00030740: 702e 534f 5552 4345 5f50 4154 4820 3d20  p.SOURCE_PATH = 
+00030750: 6f73 2e70 6174 682e 6a6f 696e 2864 6174  os.path.join(dat
+00030760: 615f 7061 7468 2c20 7365 6c66 2e73 6574  a_path, self.set
+00030770: 7570 2e53 4f55 5243 455f 4944 290a 0a20  up.SOURCE_ID).. 
+00030780: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
+00030790: 702e 4441 5441 5f46 494c 4520 3d20 6f73  p.DATA_FILE = os
+000307a0: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
+000307b0: 7365 7475 702e 534f 5552 4345 5f50 4154  setup.SOURCE_PAT
+000307c0: 482c 2066 696c 656e 616d 6529 0a20 2020  H, filename).   
+000307d0: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
+000307e0: 4d41 5050 494e 475f 4649 4c45 203d 206f  MAPPING_FILE = o
+000307f0: 732e 7061 7468 2e6a 6f69 6e28 0a20 2020  s.path.join(.   
+00030800: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00030810: 7475 702e 534f 5552 4345 5f50 4154 482c  tup.SOURCE_PATH,
+00030820: 2027 6d61 7070 696e 675f 2720 2b20 7374   'mapping_' + st
+00030830: 7228 7965 6172 2920 2b20 272e 786c 7378  r(year) + '.xlsx
+00030840: 270a 2020 2020 2020 2020 290a 2020 2020  '.        ).    
+00030850: 2020 2020 7365 6c66 2e73 6574 7570 2e4c      self.setup.L
+00030860: 4943 454e 4345 203d 2028 0a20 2020 2020  ICENCE = (.     
+00030870: 2020 2020 2020 2027 2052 6573 7472 6963         ' Restric
+00030880: 7465 6420 7573 6520 696e 2074 6865 2043  ted use in the C
+00030890: 6c69 6d61 7465 2054 7261 6e73 7061 7265  limate Transpare
+000308a0: 6e63 7920 5265 706f 7274 2070 726f 6a65  ncy Report proje
+000308b0: 6374 206f 6e6c 7927 0a20 2020 2020 2020  ct only'.       
+000308c0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+000308d0: 7365 7475 702e 5552 4c20 3d20 2768 7474  setup.URL = 'htt
+000308e0: 7073 3a2f 2f77 7777 2e65 6e65 7264 6174  ps://www.enerdat
+000308f0: 612e 6e65 742f 7573 6572 2f3f 6465 7374  a.net/user/?dest
+00030900: 696e 6174 696f 6e3d 7365 7276 6963 6573  ination=services
+00030910: 2e68 746d 6c27 0a0a 2020 2020 2020 2020  .html'..        
+00030920: 7365 6c66 2e73 6574 7570 2e52 4547 494f  self.setup.REGIO
+00030930: 4e5f 434f 4c55 4d4e 5f4e 414d 4520 3d20  N_COLUMN_NAME = 
+00030940: 2749 534f 2063 6f64 6527 0a20 2020 2020  'ISO code'.     
+00030950: 2020 2073 656c 662e 7365 7475 702e 5641     self.setup.VA
+00030960: 5249 4142 4c45 5f43 4f4c 554d 4e5f 4e41  RIABLE_COLUMN_NA
+00030970: 4d45 203d 2027 4974 656d 2063 6f64 6527  ME = 'Item code'
+00030980: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00030990: 2028 6f73 2e70 6174 682e 6578 6973 7473   (os.path.exists
+000309a0: 2873 656c 662e 7365 7475 702e 4d41 5050  (self.setup.MAPP
+000309b0: 494e 475f 4649 4c45 2929 3a0a 2020 2020  ING_FILE)):.    
+000309c0: 2020 2020 2020 2020 7365 6c66 2e63 7265          self.cre
+000309d0: 6174 6556 6172 6961 626c 654d 6170 7069  ateVariableMappi
+000309e0: 6e67 2829 0a20 2020 2020 2020 2020 2020  ng().           
+000309f0: 2070 7269 6e74 2822 6e6f 206d 6170 7069   print("no mappi
+00030a00: 6e67 2066 696c 6520 666f 756e 6422 290a  ng file found").
+00030a10: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00030a20: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00030a30: 6170 7069 6e67 203d 2064 6963 7428 290a  apping = dict().
+00030a40: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00030a50: 2076 6172 2069 6e20 5b27 656e 7469 7479   var in ['entity
+00030a60: 272c 2027 7265 6769 6f6e 275d 3a0a 2020  ', 'region']:.  
+00030a70: 2020 2020 2020 2020 2020 2020 2020 6466                df
+00030a80: 203d 2070 642e 7265 6164 5f65 7863 656c   = pd.read_excel
+00030a90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00030aa0: 2020 2020 2020 7365 6c66 2e73 6574 7570        self.setup
+00030ab0: 2e4d 4150 5049 4e47 5f46 494c 452c 2073  .MAPPING_FILE, s
+00030ac0: 6865 6574 5f6e 616d 653d 7661 7220 2b20  heet_name=var + 
+00030ad0: 275f 6d61 7070 696e 6727 2c20 696e 6465  '_mapping', inde
+00030ae0: 785f 636f 6c3d 300a 2020 2020 2020 2020  x_col=0.        
+00030af0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00030b00: 2020 2020 2020 2020 2020 6466 203d 2064            df = d
+00030b10: 662e 6c6f 635b 7e64 662e 6c6f 635b 3a2c  f.loc[~df.loc[:,
+00030b20: 2076 6172 5d2e 6973 6e61 2829 5d0a 2020   var].isna()].  
+00030b30: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00030b40: 6c66 2e6d 6170 7069 6e67 2e75 7064 6174  lf.mapping.updat
+00030b50: 6528 6466 2e74 6f5f 6469 6374 2829 290a  e(df.to_dict()).
+00030b60: 0a20 2020 2020 2020 2073 656c 662e 6372  .        self.cr
+00030b70: 6561 7465 536f 7572 6365 4d65 7461 2829  eateSourceMeta()
+00030b80: 0a0a 2020 2020 6465 6620 6c6f 6164 4461  ..    def loadDa
+00030b90: 7461 2873 656c 6629 3a0a 2020 2020 2020  ta(self):.      
+00030ba0: 2020 7365 6c66 2e64 6174 6120 3d20 7064    self.data = pd
+00030bb0: 2e72 6561 645f 6578 6365 6c28 0a20 2020  .read_excel(.   
+00030bc0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00030bd0: 7475 702e 4441 5441 5f46 494c 452c 2069  tup.DATA_FILE, i
+00030be0: 6e64 6578 5f63 6f6c 3d4e 6f6e 652c 2068  ndex_col=None, h
+00030bf0: 6561 6465 723d 302c 206e 615f 7661 6c75  eader=0, na_valu
+00030c00: 6573 3d27 6e2e 612e 270a 2020 2020 2020  es='n.a.'.      
+00030c10: 2020 290a 0a20 2020 2020 2020 2023 2066    )..        # f
+00030c20: 6978 2064 6f6f 7562 6c65 2065 6e74 7279  ix doouble entry
+00030c30: 206f 6620 736f 6c61 720a 2020 2020 2020   of solar.      
+00030c40: 2020 6d61 736b 203d 2028 7365 6c66 2e64    mask = (self.d
+00030c50: 6174 612e 6c6f 635b 3a2c 2027 4974 656d  ata.loc[:, 'Item
+00030c60: 2063 6f64 6527 5d20 3d3d 2027 6564 7670   code'] == 'edvp
+00030c70: 6427 2920 2620 280a 2020 2020 2020 2020  d') & (.        
+00030c80: 2020 2020 7365 6c66 2e64 6174 612e 6c6f      self.data.lo
+00030c90: 635b 3a2c 2027 556e 6974 275d 203d 3d20  c[:, 'Unit'] == 
+00030ca0: 274d 746f 6527 0a20 2020 2020 2020 2029  'Mtoe'.        )
+00030cb0: 0a20 2020 2020 2020 2069 6e64 5f74 6f5f  .        ind_to_
+00030cc0: 6472 6f70 7020 3d20 7365 6c66 2e64 6174  dropp = self.dat
+00030cd0: 612e 696e 6465 785b 6d61 736b 5d0a 2020  a.index[mask].  
+00030ce0: 2020 2020 2020 7365 6c66 2e64 6174 6120        self.data 
+00030cf0: 3d20 7365 6c66 2e64 6174 612e 6472 6f70  = self.data.drop
+00030d00: 2869 6e64 5f74 6f5f 6472 6f70 7029 0a0a  (ind_to_dropp)..
+00030d10: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
+00030d20: 612e 6c6f 635b 3a2c 2027 7265 6769 6f6e  a.loc[:, 'region
+00030d30: 275d 203d 2073 656c 662e 6461 7461 2e6c  '] = self.data.l
+00030d40: 6f63 5b3a 2c20 7365 6c66 2e73 6574 7570  oc[:, self.setup
+00030d50: 2e52 4547 494f 4e5f 434f 4c55 4d4e 5f4e  .REGION_COLUMN_N
+00030d60: 414d 455d 0a20 2020 2020 2020 2073 656c  AME].        sel
+00030d70: 662e 6461 7461 2e6c 6f63 5b3a 2c20 2765  f.data.loc[:, 'e
+00030d80: 6e74 6974 7927 5d20 3d20 7365 6c66 2e64  ntity'] = self.d
+00030d90: 6174 612e 6c6f 635b 3a2c 2073 656c 662e  ata.loc[:, self.
+00030da0: 7365 7475 702e 5641 5249 4142 4c45 5f43  setup.VARIABLE_C
+00030db0: 4f4c 554d 4e5f 4e41 4d45 5d0a 2020 2020  OLUMN_NAME].    
+00030dc0: 2020 2020 7365 6c66 2e64 6174 612e 6c6f      self.data.lo
+00030dd0: 635b 3a2c 2027 7363 656e 6172 696f 275d  c[:, 'scenario']
+00030de0: 203d 2027 4869 7374 6f72 6963 270a 0a20   = 'Historic'.. 
+00030df0: 2020 2020 2020 2073 656c 662e 7469 6d65         self.time
+00030e00: 436f 6c75 6d6e 7320 3d20 6c69 7374 2829  Columns = list()
+00030e10: 0a20 2020 2020 2020 2066 6f72 2063 6f6c  .        for col
+00030e20: 2069 6e20 7365 6c66 2e64 6174 612e 636f   in self.data.co
+00030e30: 6c75 6d6e 733a 0a20 2020 2020 2020 2020  lumns:.         
+00030e40: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00030e50: 2863 6f6c 2c20 696e 7429 3a0a 2020 2020  (col, int):.    
+00030e60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00030e70: 2e74 696d 6543 6f6c 756d 6e73 2e61 7070  .timeColumns.app
+00030e80: 656e 6428 636f 6c29 0a0a 2020 2020 2320  end(col)..    # 
+00030e90: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
+00030ea0: 2e6c 6f63 5b3a 2c27 6d6f 6465 6c27 5d20  .loc[:,'model'] 
+00030eb0: 3d20 2727 0a20 2020 2064 6566 2063 7265  = ''.    def cre
+00030ec0: 6174 6556 6172 6961 626c 654d 6170 7069  ateVariableMappi
+00030ed0: 6e67 2873 656c 6629 3a0a 0a20 2020 2020  ng(self):..     
+00030ee0: 2020 2023 206c 6f61 6469 6e67 2064 6174     # loading dat
+00030ef0: 6120 6966 206e 6563 6573 7361 7279 0a20  a if necessary. 
+00030f00: 2020 2020 2020 2069 6620 6e6f 7420 6861         if not ha
+00030f10: 7361 7474 7228 7365 6c66 2c20 2764 6174  sattr(self, 'dat
+00030f20: 6127 293a 0a20 2020 2020 2020 2020 2020  a'):.           
+00030f30: 2073 656c 662e 6c6f 6164 4461 7461 2829   self.loadData()
+00030f40: 0a0a 2020 2020 2020 2020 696d 706f 7274  ..        import
+00030f50: 206e 756d 7079 2061 7320 6e70 0a0a 2020   numpy as np..  
+00030f60: 2020 2020 2020 7772 6974 6572 203d 2070        writer = p
+00030f70: 642e 4578 6365 6c57 7269 7465 7228 0a20  d.ExcelWriter(. 
+00030f80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00030f90: 7365 7475 702e 4d41 5050 494e 475f 4649  setup.MAPPING_FI
+00030fa0: 4c45 2c0a 2020 2020 2020 2020 2020 2020  LE,.            
+00030fb0: 656e 6769 6e65 3d27 786c 7378 7772 6974  engine='xlsxwrit
+00030fc0: 6572 272c 0a20 2020 2020 2020 2020 2020  er',.           
+00030fd0: 2064 6174 6574 696d 655f 666f 726d 6174   datetime_format
+00030fe0: 3d27 6d6d 6d20 6420 7979 7979 2068 683a  ='mmm d yyyy hh:
+00030ff0: 6d6d 3a73 7327 2c0a 2020 2020 2020 2020  mm:ss',.        
+00031000: 2020 2020 6461 7465 5f66 6f72 6d61 743d      date_format=
+00031010: 276d 6d6d 6d20 6464 2079 7979 7927 2c0a  'mmmm dd yyyy',.
+00031020: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00031030: 2020 2023 2076 6172 6961 626c 6573 0a20     # variables. 
+00031040: 2020 2020 2020 2023 2069 6e64 6578 203d         # index =
+00031050: 2073 656c 662e 6461 7461 5b73 656c 662e   self.data[self.
+00031060: 7365 7475 702e 5641 5249 4142 4c45 5f43  setup.VARIABLE_C
+00031070: 4f4c 554d 4e5f 4e41 4d45 5d2e 756e 6971  OLUMN_NAME].uniq
+00031080: 7565 2829 0a20 2020 2020 2020 2073 656c  ue().        sel
+00031090: 662e 6176 6169 6c61 626c 6553 6572 6965  f.availableSerie
+000310a0: 7320 3d20 7365 6c66 2e64 6174 612e 6472  s = self.data.dr
+000310b0: 6f70 5f64 7570 6c69 6361 7465 7328 0a20  op_duplicates(. 
+000310c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000310d0: 7365 7475 702e 5641 5249 4142 4c45 5f43  setup.VARIABLE_C
+000310e0: 4f4c 554d 4e5f 4e41 4d45 0a20 2020 2020  OLUMN_NAME.     
+000310f0: 2020 2029 2e73 6574 5f69 6e64 6578 2873     ).set_index(s
+00031100: 656c 662e 7365 7475 702e 5641 5249 4142  elf.setup.VARIAB
+00031110: 4c45 5f43 4f4c 554d 4e5f 4e41 4d45 295b  LE_COLUMN_NAME)[
+00031120: 5b27 556e 6974 272c 2027 5469 746c 6527  ['Unit', 'Title'
+00031130: 5d5d 0a20 2020 2020 2020 2073 656c 662e  ]].        self.
+00031140: 6d61 7070 696e 6720 3d20 7064 2e44 6174  mapping = pd.Dat
+00031150: 6146 7261 6d65 280a 2020 2020 2020 2020  aFrame(.        
+00031160: 2020 2020 696e 6465 783d 7365 6c66 2e61      index=self.a
+00031170: 7661 696c 6162 6c65 5365 7269 6573 2e69  vailableSeries.i
+00031180: 6e64 6578 2c20 636f 6c75 6d6e 733d 5b27  ndex, columns=['
+00031190: 656e 7469 7479 272c 2027 6361 7465 676f  entity', 'catego
+000311a0: 7279 272c 2027 756e 6974 546f 275d 0a20  ry', 'unitTo']. 
+000311b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000311c0: 2073 656c 662e 6d61 7070 696e 6720 3d20   self.mapping = 
+000311d0: 7064 2e63 6f6e 6361 7428 5b73 656c 662e  pd.concat([self.
+000311e0: 6d61 7070 696e 672c 2073 656c 662e 6176  mapping, self.av
+000311f0: 6169 6c61 626c 6553 6572 6965 735d 2c20  ailableSeries], 
+00031200: 6178 6973 3d31 290a 2020 2020 2020 2020  axis=1).        
+00031210: 7365 6c66 2e6d 6170 7069 6e67 203d 2073  self.mapping = s
+00031220: 656c 662e 6d61 7070 696e 672e 736f 7274  elf.mapping.sort
+00031230: 5f69 6e64 6578 2829 0a20 2020 2020 2020  _index().       
+00031240: 2073 656c 662e 6d61 7070 696e 672e 746f   self.mapping.to
+00031250: 5f65 7863 656c 2877 7269 7465 722c 2065  _excel(writer, e
+00031260: 6e67 696e 653d 276f 7065 6e70 7978 6c27  ngine='openpyxl'
+00031270: 2c20 7368 6565 745f 6e61 6d65 3d56 4152  , sheet_name=VAR
+00031280: 5f4d 4150 5049 4e47 5f53 4845 4554 290a  _MAPPING_SHEET).
+00031290: 0a20 2020 2020 2020 2023 206d 6f64 656c  .        # model
+000312a0: 730a 2020 2020 2020 2020 2320 2020 2020  s.        #     
+000312b0: 2020 2069 6e64 6578 203d 206e 702e 756e     index = np.un
+000312c0: 6971 7565 2873 656c 662e 6461 7461 5b73  ique(self.data[s
+000312d0: 656c 662e 7365 7475 702e 4d4f 4445 4c5f  elf.setup.MODEL_
+000312e0: 434f 4c55 4d4e 5f4e 414d 455d 2e76 616c  COLUMN_NAME].val
+000312f0: 7565 7329 0a20 2020 2020 2020 2023 0a20  ues).        #. 
+00031300: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+00031310: 7365 6c66 2e61 7661 696c 6162 6c65 5365  self.availableSe
+00031320: 7269 6573 203d 2070 642e 4461 7461 4672  ries = pd.DataFr
+00031330: 616d 6528 696e 6465 783d 696e 6465 7829  ame(index=index)
+00031340: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+00031350: 2020 7365 6c66 2e6d 6170 7069 6e67 203d    self.mapping =
+00031360: 2070 642e 4461 7461 4672 616d 6528 696e   pd.DataFrame(in
+00031370: 6465 783d 696e 6465 782c 2063 6f6c 756d  dex=index, colum
+00031380: 6e73 203d 205b 7365 6c66 2e73 6574 7570  ns = [self.setup
+00031390: 2e4d 4f44 454c 5f43 4f4c 554d 4e5f 4e41  .MODEL_COLUMN_NA
+000313a0: 4d45 5d29 0a20 2020 2020 2020 2023 2020  ME]).        #  
+000313b0: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
+000313c0: 6e67 203d 2070 642e 636f 6e63 6174 285b  ng = pd.concat([
+000313d0: 7365 6c66 2e6d 6170 7069 6e67 2c20 7365  self.mapping, se
+000313e0: 6c66 2e61 7661 696c 6162 6c65 5365 7269  lf.availableSeri
+000313f0: 6573 5d2c 2061 7869 733d 3129 0a20 2020  es], axis=1).   
+00031400: 2020 2020 2023 2020 2020 2020 2020 7365       #        se
+00031410: 6c66 2e6d 6170 7069 6e67 203d 2073 656c  lf.mapping = sel
+00031420: 662e 6d61 7070 696e 672e 736f 7274 5f69  f.mapping.sort_i
+00031430: 6e64 6578 2829 0a20 2020 2020 2020 2023  ndex().        #
+00031440: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+00031450: 2020 7365 6c66 2e6d 6170 7069 6e67 2e74    self.mapping.t
+00031460: 6f5f 6578 6365 6c28 7772 6974 6572 2c20  o_excel(writer, 
+00031470: 656e 6769 6e65 3d27 6f70 656e 7079 786c  engine='openpyxl
+00031480: 272c 2073 6865 6574 5f6e 616d 653d 276d  ', sheet_name='m
+00031490: 6f64 656c 5f6d 6170 7069 6e67 2729 0a0a  odel_mapping')..
+000314a0: 2020 2020 2020 2020 2320 7363 656e 6172          # scenar
+000314b0: 696f 730a 2020 2020 2020 2020 2320 2020  ios.        #   
+000314c0: 2020 2020 2069 6e64 6578 203d 206e 702e       index = np.
+000314d0: 756e 6971 7565 2873 656c 662e 6461 7461  unique(self.data
+000314e0: 5b73 656c 662e 7365 7475 702e 5343 454e  [self.setup.SCEN
+000314f0: 4152 494f 5f43 4f4c 554d 4e5f 4e41 4d45  ARIO_COLUMN_NAME
+00031500: 5d2e 7661 6c75 6573 290a 2020 2020 2020  ].values).      
+00031510: 2020 230a 2020 2020 2020 2020 2320 2020    #.        #   
+00031520: 2020 2020 2073 656c 662e 6176 6169 6c61       self.availa
+00031530: 626c 6553 6572 6965 7320 3d20 7064 2e44  bleSeries = pd.D
+00031540: 6174 6146 7261 6d65 2869 6e64 6578 3d69  ataFrame(index=i
+00031550: 6e64 6578 290a 2020 2020 2020 2020 2320  ndex).        # 
+00031560: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
+00031570: 696e 6720 3d20 7064 2e44 6174 6146 7261  ing = pd.DataFra
+00031580: 6d65 2869 6e64 6578 3d69 6e64 6578 2c20  me(index=index, 
+00031590: 636f 6c75 6d6e 7320 3d20 5b73 656c 662e  columns = [self.
+000315a0: 7365 7475 702e 5343 454e 4152 494f 5f43  setup.SCENARIO_C
+000315b0: 4f4c 554d 4e5f 4e41 4d45 5d29 0a20 2020  OLUMN_NAME]).   
+000315c0: 2020 2020 2023 2020 2020 2020 2020 7365       #        se
+000315d0: 6c66 2e6d 6170 7069 6e67 203d 2070 642e  lf.mapping = pd.
+000315e0: 636f 6e63 6174 285b 7365 6c66 2e6d 6170  concat([self.map
+000315f0: 7069 6e67 2c20 7365 6c66 2e61 7661 696c  ping, self.avail
+00031600: 6162 6c65 5365 7269 6573 5d2c 2061 7869  ableSeries], axi
+00031610: 733d 3129 0a20 2020 2020 2020 2023 2020  s=1).        #  
+00031620: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
+00031630: 6e67 203d 2073 656c 662e 6d61 7070 696e  ng = self.mappin
+00031640: 672e 736f 7274 5f69 6e64 6578 2829 0a20  g.sort_index(). 
+00031650: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+00031660: 7365 6c66 2e6d 6170 7069 6e67 2e74 6f5f  self.mapping.to_
+00031670: 6578 6365 6c28 7772 6974 6572 2c20 656e  excel(writer, en
+00031680: 6769 6e65 3d27 6f70 656e 7079 786c 272c  gine='openpyxl',
+00031690: 2073 6865 6574 5f6e 616d 653d 2773 6365   sheet_name='sce
+000316a0: 6e61 7269 6f5f 6d61 7070 696e 6727 290a  nario_mapping').
+000316b0: 0a20 2020 2020 2020 2023 2072 6567 696f  .        # regio
+000316c0: 6e0a 2020 2020 2020 2020 696e 6465 7820  n.        index 
+000316d0: 3d20 7365 6c66 2e64 6174 615b 7365 6c66  = self.data[self
+000316e0: 2e73 6574 7570 2e52 4547 494f 4e5f 434f  .setup.REGION_CO
+000316f0: 4c55 4d4e 5f4e 414d 455d 2e75 6e69 7175  LUMN_NAME].uniqu
+00031700: 6528 290a 0a20 2020 2020 2020 2073 656c  e()..        sel
+00031710: 662e 6176 6169 6c61 626c 6553 6572 6965  f.availableSerie
+00031720: 7320 3d20 7064 2e44 6174 6146 7261 6d65  s = pd.DataFrame
+00031730: 2869 6e64 6578 3d69 6e64 6578 290a 2020  (index=index).  
+00031740: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
+00031750: 6e67 203d 2070 642e 4461 7461 4672 616d  ng = pd.DataFram
+00031760: 6528 696e 6465 783d 696e 6465 782c 2063  e(index=index, c
+00031770: 6f6c 756d 6e73 3d5b 2772 6567 696f 6e27  olumns=['region'
+00031780: 5d29 0a20 2020 2020 2020 2073 656c 662e  ]).        self.
+00031790: 6d61 7070 696e 6720 3d20 7064 2e63 6f6e  mapping = pd.con
+000317a0: 6361 7428 5b73 656c 662e 6d61 7070 696e  cat([self.mappin
+000317b0: 672c 2073 656c 662e 6176 6169 6c61 626c  g, self.availabl
+000317c0: 6553 6572 6965 735d 2c20 6178 6973 3d31  eSeries], axis=1
+000317d0: 290a 2020 2020 2020 2020 7365 6c66 2e6d  ).        self.m
+000317e0: 6170 7069 6e67 203d 2073 656c 662e 6d61  apping = self.ma
+000317f0: 7070 696e 672e 736f 7274 5f69 6e64 6578  pping.sort_index
+00031800: 2829 0a0a 2020 2020 2020 2020 666f 7220  ()..        for 
+00031810: 6964 7820 696e 2073 656c 662e 6d61 7070  idx in self.mapp
+00031820: 696e 672e 696e 6465 783a 0a20 2020 2020  ing.index:.     
+00031830: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+00031840: 696e 7374 616e 6365 2869 6478 2c20 2873  instance(idx, (s
+00031850: 7472 2c20 696e 7429 293a 0a20 2020 2020  tr, int)):.     
+00031860: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+00031870: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
+00031880: 6973 6f20 3d20 6474 2e75 7469 6c2e 6964  iso = dt.util.id
+00031890: 656e 7469 6679 436f 756e 7472 7928 6964  entifyCountry(id
+000318a0: 7829 0a20 2020 2020 2020 2020 2020 2069  x).            i
+000318b0: 6620 6973 6f20 6973 206e 6f74 204e 6f6e  f iso is not Non
+000318c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000318d0: 2020 2073 656c 662e 6d61 7070 696e 672e     self.mapping.
+000318e0: 6c6f 635b 6964 782c 2027 7265 6769 6f6e  loc[idx, 'region
+000318f0: 275d 203d 2069 736f 0a0a 2020 2020 2020  '] = iso..      
+00031900: 2020 7365 6c66 2e6d 6170 7069 6e67 2e74    self.mapping.t
+00031910: 6f5f 6578 6365 6c28 7772 6974 6572 2c20  o_excel(writer, 
+00031920: 656e 6769 6e65 3d27 6f70 656e 7079 786c  engine='openpyxl
+00031930: 272c 2073 6865 6574 5f6e 616d 653d 2772  ', sheet_name='r
+00031940: 6567 696f 6e5f 6d61 7070 696e 6727 290a  egion_mapping').
+00031950: 2020 2020 2020 2020 7772 6974 6572 2e63          writer.c
+00031960: 6c6f 7365 2829 0a0a 2020 2020 6465 6620  lose()..    def 
+00031970: 6761 7468 6572 4d61 7070 6564 4461 7461  gatherMappedData
+00031980: 2873 656c 662c 2073 7061 7469 616c 5375  (self, spatialSu
+00031990: 6253 6574 3d4e 6f6e 6529 3a0a 0a20 2020  bSet=None):..   
+000319a0: 2020 2020 2069 6d70 6f72 7420 7471 646d       import tqdm
+000319b0: 0a0a 2020 2020 2020 2020 2320 6c6f 6164  ..        # load
+000319c0: 696e 6720 6461 7461 2069 6620 6e65 6365  ing data if nece
+000319d0: 7373 6172 790a 2020 2020 2020 2020 6966  ssary.        if
+000319e0: 206e 6f74 2068 6173 6174 7472 2873 656c   not hasattr(sel
+000319f0: 662c 2027 6461 7461 2729 3a0a 2020 2020  f, 'data'):.    
+00031a00: 2020 2020 2020 2020 7365 6c66 2e6c 6f61          self.loa
+00031a10: 6444 6174 6128 290a 0a20 2020 2020 2020  dData()..       
+00031a20: 2074 6162 6c65 7354 6f43 6f6d 6d69 7420   tablesToCommit 
+00031a30: 3d20 5b5d 0a20 2020 2020 2020 206d 6574  = [].        met
+00031a40: 6144 6963 7420 3d20 6469 6374 2829 0a20  aDict = dict(). 
+00031a50: 2020 2020 2020 206d 6574 6144 6963 745b         metaDict[
+00031a60: 2773 6f75 7263 6527 5d20 3d20 7365 6c66  'source'] = self
+00031a70: 2e73 6574 7570 2e53 4f55 5243 455f 4944  .setup.SOURCE_ID
+00031a80: 0a20 2020 2020 2020 2065 7863 6c75 6465  .        exclude
+00031a90: 6454 6162 6c65 7320 3d20 6469 6374 2829  dTables = dict()
+00031aa0: 0a20 2020 2020 2020 2065 7863 6c75 6465  .        exclude
+00031ab0: 6454 6162 6c65 735b 2765 6d70 7479 275d  dTables['empty']
+00031ac0: 203d 206c 6973 7428 290a 2020 2020 2020   = list().      
+00031ad0: 2020 6578 636c 7564 6564 5461 626c 6573    excludedTables
+00031ae0: 5b27 6572 726f 7227 5d20 3d20 6c69 7374  ['error'] = list
+00031af0: 2829 0a20 2020 2020 2020 2065 7863 6c75  ().        exclu
+00031b00: 6465 6454 6162 6c65 735b 2765 7869 7374  dedTables['exist
+00031b10: 7327 5d20 3d20 6c69 7374 2829 0a0a 2020  s'] = list()..  
+00031b20: 2020 2020 2020 2320 6669 7820 646f 7562        # fix doub
+00031b30: 6c65 2065 6e74 7269 6573 2066 6f72 2070  le entries for p
+00031b40: 6f77 6572 2067 656e 6572 6174 696f 6e20  ower generation 
+00031b50: 7769 6e64 0a20 2020 2020 2020 2077 696e  wind.        win
+00031b60: 645f 6d61 736b 203d 2073 656c 662e 6461  d_mask = self.da
+00031b70: 7461 2e65 6e74 6974 7920 3d3d 2027 6565  ta.entity == 'ee
+00031b80: 6f70 6427 0a20 2020 2020 2020 204d 746f  opd'.        Mto
+00031b90: 655f 6d61 736b 203d 2073 656c 662e 6461  e_mask = self.da
+00031ba0: 7461 2e55 6e69 7420 3d3d 2027 4d74 6f65  ta.Unit == 'Mtoe
+00031bb0: 270a 2020 2020 2020 2020 6d61 736b 203d  '.        mask =
+00031bc0: 2077 696e 645f 6d61 736b 2026 204d 746f   wind_mask & Mto
+00031bd0: 655f 6d61 736b 0a20 2020 2020 2020 2073  e_mask.        s
+00031be0: 656c 662e 6461 7461 203d 2073 656c 662e  elf.data = self.
+00031bf0: 6461 7461 2e64 726f 7028 7365 6c66 2e64  data.drop(self.d
+00031c00: 6174 612e 696e 6465 785b 6d61 736b 5d29  ata.index[mask])
+00031c10: 0a0a 2020 2020 2020 2020 666f 7220 7661  ..        for va
+00031c20: 7269 6162 6c65 2069 6e20 6c69 7374 2873  riable in list(s
+00031c30: 656c 662e 6d61 7070 696e 675b 2765 6e74  elf.mapping['ent
+00031c40: 6974 7927 5d2e 6b65 7973 2829 293a 0a20  ity'].keys()):. 
+00031c50: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+00031c60: 2020 2020 2020 2020 6d65 7461 4466 203d          metaDf =
+00031c70: 2073 656c 662e 6d61 7070 696e 672e 6c6f   self.mapping.lo
+00031c80: 635b 7661 7269 6162 6c65 5d0a 2020 2020  c[variable].    
+00031c90: 2020 2020 2020 2020 7465 6d70 4d6f 5363          tempMoSc
+00031ca0: 5661 7220 3d20 7365 6c66 2e64 6174 612e  Var = self.data.
+00031cb0: 6c6f 635b 7365 6c66 2e64 6174 612e 656e  loc[self.data.en
+00031cc0: 7469 7479 203d 3d20 7661 7269 6162 6c65  tity == variable
+00031cd0: 5d0a 2020 2020 2020 2020 2020 2020 7465  ].            te
+00031ce0: 6d70 4d6f 5363 5661 722e 756e 6974 203d  mpMoScVar.unit =
+00031cf0: 2073 656c 662e 6d61 7070 696e 675b 2775   self.mapping['u
+00031d00: 6e69 7427 5d5b 7661 7269 6162 6c65 5d0a  nit'][variable].
+00031d10: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+00031d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031d30: 2074 6162 6c65 7320 3d20 6474 2e69 6e74   tables = dt.int
+00031d40: 6572 6661 6365 732e 7265 6164 5f6c 6f6e  erfaces.read_lon
+00031d50: 675f 7461 626c 6528 7465 6d70 4d6f 5363  g_table(tempMoSc
+00031d60: 5661 722c 205b 7661 7269 6162 6c65 5d29  Var, [variable])
+00031d70: 0a0a 2020 2020 2020 2020 2020 2020 7461  ..            ta
+00031d80: 626c 6520 3d20 7465 6d70 4d6f 5363 5661  ble = tempMoScVa
+00031d90: 722e 6c6f 635b 3a2c 2073 656c 662e 7469  r.loc[:, self.ti
+00031da0: 6d65 436f 6c75 6d6e 735d 0a0a 2020 2020  meColumns]..    
+00031db0: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
+00031dc0: 4461 7461 7461 626c 6528 0a20 2020 2020  Datatable(.     
+00031dd0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+00031de0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00031df0: 2020 6d65 7461 3d7b 0a20 2020 2020 2020    meta={.       
+00031e00: 2020 2020 2020 2020 2020 2020 2027 656e               'en
+00031e10: 7469 7479 273a 2073 656c 662e 6d61 7070  tity': self.mapp
+00031e20: 696e 675b 2765 6e74 6974 7927 5d5b 7661  ing['entity'][va
+00031e30: 7269 6162 6c65 5d2c 0a20 2020 2020 2020  riable],.       
+00031e40: 2020 2020 2020 2020 2020 2020 2027 6361               'ca
+00031e50: 7465 676f 7279 273a 2073 656c 662e 6d61  tegory': self.ma
+00031e60: 7070 696e 675b 2763 6174 6567 6f72 7927  pping['category'
+00031e70: 5d5b 7661 7269 6162 6c65 5d2c 0a20 2020  ][variable],.   
+00031e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031e90: 2027 7363 656e 6172 696f 273a 2027 4869   'scenario': 'Hi
+00031ea0: 7374 6f72 6963 272c 0a20 2020 2020 2020  storic',.       
+00031eb0: 2020 2020 2020 2020 2020 2020 2027 736f               'so
+00031ec0: 7572 6365 273a 2073 656c 662e 7365 7475  urce': self.setu
+00031ed0: 702e 534f 5552 4345 5f49 442c 0a20 2020  p.SOURCE_ID,.   
+00031ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031ef0: 2027 756e 6974 273a 2073 656c 662e 6d61   'unit': self.ma
+00031f00: 7070 696e 675b 2775 6e69 7427 5d5b 7661  pping['unit'][va
+00031f10: 7269 6162 6c65 5d2c 0a20 2020 2020 2020  riable],.       
+00031f20: 2020 2020 2020 2020 2020 2020 2027 6f72               'or
+00031f30: 6967 696e 616c 2063 6f64 6527 3a20 7661  iginal code': va
+00031f40: 7269 6162 6c65 2c0a 2020 2020 2020 2020  riable,.        
+00031f50: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00031f60: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00031f70: 2020 2020 2074 6162 6c65 2e69 6e64 6578       table.index
+00031f80: 203d 2074 656d 704d 6f53 6356 6172 2e72   = tempMoScVar.r
+00031f90: 6567 696f 6e0a 2020 2020 2020 2020 2020  egion.          
+00031fa0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+00031fb0: 2020 2020 2020 2074 6162 6c65 2e6d 6574         table.met
+00031fc0: 615b 2763 6174 6567 6f72 7927 5d20 3d20  a['category'] = 
+00031fd0: 2222 0a20 2020 2020 2020 2020 2020 2023  "".            #
+00031fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031ff0: 2020 2020 7461 626c 652e 6d65 7461 5b27      table.meta['
+00032000: 736f 7572 6365 275d 203d 0a20 2020 2020  source'] =.     
+00032010: 2020 2020 2020 2074 6162 6c65 2e69 6e64         table.ind
+00032020: 6578 203d 2074 6162 6c65 2e69 6e64 6578  ex = table.index
+00032030: 2e6d 6170 2873 656c 662e 6d61 7070 696e  .map(self.mappin
+00032040: 675b 2772 6567 696f 6e27 5d29 0a0a 2020  g['region'])..  
+00032050: 2020 2020 2020 2020 2020 7461 626c 6520            table 
+00032060: 3d20 7461 626c 652e 6c6f 635b 7e70 642e  = table.loc[~pd.
+00032070: 6973 6e61 2874 6162 6c65 2e69 6e64 6578  isna(table.index
+00032080: 292c 203a 5d0a 2020 2020 2020 2020 2020  ), :].          
+00032090: 2020 6966 206e 6f74 2070 642e 6973 6e61    if not pd.isna
+000320a0: 2873 656c 662e 6d61 7070 696e 675b 2775  (self.mapping['u
+000320b0: 6e69 7454 6f27 5d5b 7661 7269 6162 6c65  nitTo'][variable
+000320c0: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
+000320d0: 2020 2020 7072 696e 7428 2763 6f6e 7665      print('conve
+000320e0: 7273 696f 6e20 746f 203a 2027 202b 2073  rsion to : ' + s
+000320f0: 7472 2873 656c 662e 6d61 7070 696e 675b  tr(self.mapping[
+00032100: 2775 6e69 7454 6f27 5d5b 7661 7269 6162  'unitTo'][variab
+00032110: 6c65 5d29 290a 2020 2020 2020 2020 2020  le])).          
+00032120: 2020 2020 2020 7461 626c 6520 3d20 7461        table = ta
+00032130: 626c 652e 636f 6e76 6572 7428 7365 6c66  ble.convert(self
+00032140: 2e6d 6170 7069 6e67 5b27 756e 6974 546f  .mapping['unitTo
+00032150: 275d 5b76 6172 6961 626c 655d 290a 2020  '][variable]).  
+00032160: 2020 2020 2020 2020 2020 7461 626c 6549            tableI
+00032170: 4420 3d20 6474 2e63 6f72 652e 5f63 7265  D = dt.core._cre
+00032180: 6174 6544 6174 6162 6173 6549 4428 7461  ateDatabaseID(ta
+00032190: 626c 652e 6d65 7461 290a 2020 2020 2020  ble.meta).      
+000321a0: 2020 2020 2020 7461 626c 6573 546f 436f        tablesToCo
+000321b0: 6d6d 6974 2e61 7070 656e 6428 7461 626c  mmit.append(tabl
+000321c0: 6529 0a0a 2020 2020 2020 2020 7265 7475  e)..        retu
+000321d0: 726e 2074 6162 6c65 7354 6f43 6f6d 6d69  rn tablesToCommi
+000321e0: 742c 2065 7863 6c75 6465 6454 6162 6c65  t, excludedTable
+000321f0: 730a 0a0a 636c 6173 7320 5049 4b5f 4e44  s...class PIK_ND
+00032200: 4328 4261 7365 496d 706f 7274 546f 6f6c  C(BaseImportTool
+00032210: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00032220: 745f 5f28 7365 6c66 2c20 7965 6172 2c20  t__(self, year, 
+00032230: 7665 7273 696f 6e29 3a0a 2020 2020 2020  version):.      
+00032240: 2020 7365 6c66 2e73 6574 7570 203d 2073    self.setup = s
+00032250: 6574 7570 5374 7275 6374 2829 0a0a 2020  etupStruct()..  
+00032260: 2020 2020 2020 7365 6c66 2e73 6574 7570        self.setup
+00032270: 2e53 4f55 5243 455f 4944 203d 2022 5049  .SOURCE_ID = "PI
+00032280: 4b5f 4e44 435f 2220 2b20 7374 7228 7965  K_NDC_" + str(ye
+00032290: 6172 290a 2020 2020 2020 2020 7365 6c66  ar).        self
+000322a0: 2e73 6574 7570 2e53 4f55 5243 455f 4e41  .setup.SOURCE_NA
+000322b0: 4d45 203d 2022 5049 4b5f 4e44 4322 0a20  ME = "PIK_NDC". 
+000322c0: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
+000322d0: 702e 534f 5552 4345 5f59 4541 5220 3d20  p.SOURCE_YEAR = 
+000322e0: 7374 7228 7965 6172 290a 0a20 2020 2020  str(year)..     
+000322f0: 2020 2073 656c 662e 7365 7475 702e 534f     self.setup.SO
+00032300: 5552 4345 5f50 4154 4820 3d20 6f73 2e70  URCE_PATH = os.p
+00032310: 6174 682e 6a6f 696e 280a 2020 2020 2020  ath.join(.      
+00032320: 2020 2020 2020 636f 6e66 6967 2e50 4154        config.PAT
+00032330: 485f 544f 5f44 4154 4153 4845 4c46 2c20  H_TO_DATASHELF, 
+00032340: 6627 7261 7764 6174 612f 5049 4b5f 4e44  f'rawdata/PIK_ND
+00032350: 435f 7b79 6561 727d 270a 2020 2020 2020  C_{year}'.      
+00032360: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+00032370: 2e73 6574 7570 2e44 4154 415f 4649 4c45  .setup.DATA_FILE
+00032380: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00032390: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000323a0: 662e 7365 7475 702e 534f 5552 4345 5f50  f.setup.SOURCE_P
+000323b0: 4154 482c 0a20 2020 2020 2020 2020 2020  ATH,.           
+000323c0: 2066 276e 6463 5f74 6172 6765 7473 5f70   f'ndc_targets_p
+000323d0: 6174 6877 6179 735f 7065 725f 636f 756e  athways_per_coun
+000323e0: 7472 795f 7573 6564 5f66 6f72 5f67 726f  try_used_for_gro
+000323f0: 7570 5f70 6174 6877 6179 735f 7b76 6572  up_pathways_{ver
+00032400: 7369 6f6e 7d2e 6373 7627 2c0a 2020 2020  sion}.csv',.    
+00032410: 2020 2020 290a 2020 2020 2020 2020 2320      ).        # 
+00032420: 7365 6c66 2e73 6574 7570 2e4d 4150 5049  self.setup.MAPPI
+00032430: 4e47 5f46 494c 4520 3d20 6f73 2e70 6174  NG_FILE = os.pat
+00032440: 682e 6a6f 696e 2873 656c 662e 7365 7475  h.join(self.setu
+00032450: 702e 534f 5552 4345 5f50 4154 482c 2027  p.SOURCE_PATH, '
+00032460: 6d61 7070 696e 672e 786c 7378 2729 0a20  mapping.xlsx'). 
+00032470: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
+00032480: 702e 4c49 4345 4e43 4520 3d20 2743 4320  p.LICENCE = 'CC 
+00032490: 4259 2d34 2e30 270a 2020 2020 2020 2020  BY-4.0'.        
+000324a0: 7365 6c66 2e73 6574 7570 2e55 524c 203d  self.setup.URL =
+000324b0: 2027 6874 7470 733a 2f2f 7a65 6e6f 646f   'https://zenodo
+000324c0: 2e6f 7267 2f72 6563 6f72 642f 3531 3133  .org/record/5113
+000324d0: 3938 3727 0a20 2020 2020 2020 2073 656c  987'.        sel
+000324e0: 662e 7665 7273 696f 6e20 3d20 7665 7273  f.version = vers
+000324f0: 696f 6e0a 0a20 2020 2064 6566 2067 6174  ion..    def gat
+00032500: 6865 724d 6170 7065 6444 6174 6128 7365  herMappedData(se
+00032510: 6c66 293a 0a0a 2020 2020 2020 2020 7069  lf):..        pi
+00032520: 6b5f 6461 7461 203d 2070 642e 7265 6164  k_data = pd.read
+00032530: 5f63 7376 280a 2020 2020 2020 2020 2020  _csv(.          
+00032540: 2020 7365 6c66 2e73 6574 7570 2e44 4154    self.setup.DAT
+00032550: 415f 4649 4c45 2c0a 2020 2020 2020 2020  A_FILE,.        
+00032560: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+00032570: 7069 6b5f 6461 7461 2e68 6561 6428 2929  pik_data.head())
+00032580: 0a0a 2020 2020 2020 2020 2320 7265 6d6f  ..        # remo
+00032590: 7665 2063 6f75 6e74 7269 6573 2074 6861  ve countries tha
+000325a0: 7420 646f 206e 6f74 2068 6176 6520 6120  t do not have a 
+000325b0: 6361 6c63 7561 6c74 6564 2074 6172 6765  calcualted targe
+000325c0: 740a 2020 2020 2020 2020 6d61 736b 203d  t.        mask =
+000325d0: 2070 696b 5f64 6174 612e 6164 645f 696e   pik_data.add_in
+000325e0: 666f 2e73 7472 2e73 7461 7274 7377 6974  fo.str.startswit
+000325f0: 6828 274e 6f20 7461 7267 6574 7320 6361  h('No targets ca
+00032600: 6c63 756c 6174 6564 2729 0a20 2020 2020  lculated').     
+00032610: 2020 2069 6478 5f74 6f5f 6472 6f70 203d     idx_to_drop =
+00032620: 2070 696b 5f64 6174 612e 696e 6465 785b   pik_data.index[
+00032630: 6d61 736b 203d 3d20 5472 7565 5d0a 0a20  mask == True].. 
+00032640: 2020 2020 2020 2070 696b 5f64 6174 6120         pik_data 
+00032650: 3d20 7069 6b5f 6461 7461 2e64 726f 7028  = pik_data.drop(
+00032660: 6964 785f 746f 5f64 726f 7029 0a0a 2020  idx_to_drop)..  
+00032670: 2020 2020 2020 7069 6b5f 6461 7461 203d        pik_data =
+00032680: 2070 696b 5f64 6174 612e 7365 745f 696e   pik_data.set_in
+00032690: 6465 7828 5b27 636f 6e64 6927 2c20 2772  dex(['condi', 'r
+000326a0: 6765 275d 290a 0a20 2020 2020 2020 2070  ge'])..        p
+000326b0: 6c65 6467 655f 6c6f 7720 3d20 7069 6b5f  ledge_low = pik_
+000326c0: 6461 7461 5b0a 2020 2020 2020 2020 2020  data[.          
+000326d0: 2020 2870 696b 5f64 6174 612e 696e 6465    (pik_data.inde
+000326e0: 782e 6765 745f 6c65 7665 6c5f 7661 6c75  x.get_level_valu
+000326f0: 6573 2827 636f 6e64 6927 2920 3d3d 2027  es('condi') == '
+00032700: 636f 6e64 6974 696f 6e61 6c27 290a 2020  conditional').  
+00032710: 2020 2020 2020 2020 2020 2620 2870 696b            & (pik
+00032720: 5f64 6174 612e 696e 6465 782e 6765 745f  _data.index.get_
+00032730: 6c65 7665 6c5f 7661 6c75 6573 2827 7267  level_values('rg
+00032740: 6527 2920 3d3d 2027 6265 7374 2729 0a20  e') == 'best'). 
+00032750: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00032760: 2070 6c65 6467 655f 6c6f 7720 3d20 706c   pledge_low = pl
+00032770: 6564 6765 5f6c 6f77 2e73 6574 5f69 6e64  edge_low.set_ind
+00032780: 6578 2870 6c65 6467 655f 6c6f 772e 6c6f  ex(pledge_low.lo
+00032790: 635b 3a2c 2027 6973 6f33 275d 292e 6c6f  c[:, 'iso3']).lo
+000327a0: 635b 0a20 2020 2020 2020 2020 2020 203a  c[.            :
+000327b0: 2c20 5b73 7472 2878 2920 666f 7220 7820  , [str(x) for x 
+000327c0: 696e 2072 616e 6765 2831 3939 302c 2032  in range(1990, 2
+000327d0: 3033 3129 5d0a 2020 2020 2020 2020 5d0a  031)].        ].
+000327e0: 2020 2020 2020 2020 706c 6564 6765 5f6c          pledge_l
+000327f0: 6f77 203d 2064 742e 4461 7461 7461 626c  ow = dt.Datatabl
+00032800: 6528 0a20 2020 2020 2020 2020 2020 2070  e(.            p
+00032810: 6c65 6467 655f 6c6f 772c 0a20 2020 2020  ledge_low,.     
+00032820: 2020 2020 2020 206d 6574 613d 7b0a 2020         meta={.  
+00032830: 2020 2020 2020 2020 2020 2020 2020 2765                'e
+00032840: 6e74 6974 7927 3a20 2745 6d69 7373 696f  ntity': 'Emissio
+00032850: 6e73 7c4b 594f 544f 4748 475f 4152 3427  ns|KYOTOGHG_AR4'
+00032860: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00032870: 2020 2763 6174 6567 6f72 7927 3a20 274e    'category': 'N
+00032880: 6174 696f 6e61 6c5f 746f 7461 6c5f 6578  ational_total_ex
+00032890: 636c 5f4c 554c 5543 4627 2c0a 2020 2020  cl_LULUCF',.    
+000328a0: 2020 2020 2020 2020 2020 2020 276d 6f64              'mod
+000328b0: 656c 273a 2066 2750 494b 5f4e 4443 6d69  el': f'PIK_NDCmi
+000328c0: 7469 517c 7b73 656c 662e 7665 7273 696f  tiQ|{self.versio
+000328d0: 6e7d 272c 0a20 2020 2020 2020 2020 2020  n}',.           
+000328e0: 2020 2020 2027 7363 656e 6172 696f 273a       'scenario':
+000328f0: 2027 506c 6564 6765 5f6c 6f77 272c 0a20   'Pledge_low',. 
+00032900: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00032910: 736f 7572 6365 273a 2073 656c 662e 7365  source': self.se
+00032920: 7475 702e 534f 5552 4345 5f49 442c 0a20  tup.SOURCE_ID,. 
+00032930: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00032940: 756e 6974 273a 2027 4d74 2043 4f32 6571  unit': 'Mt CO2eq
+00032950: 272c 0a20 2020 2020 2020 2020 2020 207d  ',.            }
+00032960: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00032970: 2020 2020 2070 6c65 6467 655f 6869 6768       pledge_high
+00032980: 203d 2070 696b 5f64 6174 615b 0a20 2020   = pik_data[.   
+00032990: 2020 2020 2020 2020 2028 7069 6b5f 6461           (pik_da
+000329a0: 7461 2e69 6e64 6578 2e67 6574 5f6c 6576  ta.index.get_lev
+000329b0: 656c 5f76 616c 7565 7328 2763 6f6e 6469  el_values('condi
+000329c0: 2729 203d 3d20 2775 6e63 6f6e 6469 7469  ') == 'unconditi
+000329d0: 6f6e 616c 2729 0a20 2020 2020 2020 2020  onal').         
+000329e0: 2020 2026 2028 7069 6b5f 6461 7461 2e69     & (pik_data.i
+000329f0: 6e64 6578 2e67 6574 5f6c 6576 656c 5f76  ndex.get_level_v
+00032a00: 616c 7565 7328 2772 6765 2729 203d 3d20  alues('rge') == 
+00032a10: 2777 6f72 7374 2729 0a20 2020 2020 2020  'worst').       
+00032a20: 205d 0a20 2020 2020 2020 2070 6c65 6467   ].        pledg
+00032a30: 655f 6869 6768 203d 2070 6c65 6467 655f  e_high = pledge_
+00032a40: 6869 6768 2e73 6574 5f69 6e64 6578 2870  high.set_index(p
+00032a50: 6c65 6467 655f 6869 6768 2e6c 6f63 5b3a  ledge_high.loc[:
+00032a60: 2c20 2769 736f 3327 5d29 2e6c 6f63 5b0a  , 'iso3']).loc[.
+00032a70: 2020 2020 2020 2020 2020 2020 3a2c 205b              :, [
+00032a80: 7374 7228 7829 2066 6f72 2078 2069 6e20  str(x) for x in 
+00032a90: 7261 6e67 6528 3139 3930 2c20 3230 3331  range(1990, 2031
+00032aa0: 295d 0a20 2020 2020 2020 205d 0a20 2020  )].        ].   
+00032ab0: 2020 2020 2070 6c65 6467 655f 6869 6768       pledge_high
+00032ac0: 203d 2064 742e 4461 7461 7461 626c 6528   = dt.Datatable(
+00032ad0: 0a20 2020 2020 2020 2020 2020 2070 6c65  .            ple
+00032ae0: 6467 655f 6869 6768 2c0a 2020 2020 2020  dge_high,.      
+00032af0: 2020 2020 2020 6d65 7461 3d7b 0a20 2020        meta={.   
+00032b00: 2020 2020 2020 2020 2020 2020 2027 656e               'en
+00032b10: 7469 7479 273a 2027 456d 6973 7369 6f6e  tity': 'Emission
+00032b20: 737c 4b59 4f54 4f47 4847 5f41 5234 272c  s|KYOTOGHG_AR4',
+00032b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00032b40: 2027 6361 7465 676f 7279 273a 2027 4e61   'category': 'Na
+00032b50: 7469 6f6e 616c 5f74 6f74 616c 5f65 7863  tional_total_exc
+00032b60: 6c5f 4c55 4c55 4346 272c 0a20 2020 2020  l_LULUCF',.     
+00032b70: 2020 2020 2020 2020 2020 2027 6d6f 6465             'mode
+00032b80: 6c27 3a20 6627 5049 4b5f 4e44 436d 6974  l': f'PIK_NDCmit
+00032b90: 6951 7c7b 7365 6c66 2e76 6572 7369 6f6e  iQ|{self.version
+00032ba0: 7d27 2c0a 2020 2020 2020 2020 2020 2020  }',.            
+00032bb0: 2020 2020 2773 6365 6e61 7269 6f27 3a20      'scenario': 
+00032bc0: 2750 6c65 6467 655f 6869 6768 272c 0a20  'Pledge_high',. 
+00032bd0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00032be0: 736f 7572 6365 273a 2073 656c 662e 7365  source': self.se
+00032bf0: 7475 702e 534f 5552 4345 5f49 442c 0a20  tup.SOURCE_ID,. 
+00032c00: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00032c10: 756e 6974 273a 2027 4d74 2043 4f32 6571  unit': 'Mt CO2eq
+00032c20: 272c 0a20 2020 2020 2020 2020 2020 207d  ',.            }
+00032c30: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00032c40: 2020 2020 2072 6574 7572 6e20 5b70 6c65       return [ple
+00032c50: 6467 655f 6869 6768 2c20 706c 6564 6765  dge_high, pledge
+00032c60: 5f6c 6f77 5d2c 204e 6f6e 650a 0a0a 696d  _low], None...im
+00032c70: 706f 7274 2070 7961 6d0a 6672 6f6d 2074  port pyam.from t
+00032c80: 7164 6d20 696d 706f 7274 2074 7164 6d0a  qdm import tqdm.
+00032c90: 0a0a 636c 6173 7320 4949 4153 4128 4261  ..class IIASA(Ba
+00032ca0: 7365 496d 706f 7274 546f 6f6c 293a 0a20  seImportTool):. 
+00032cb0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00032cc0: 7365 6c66 2c20 736f 7572 6365 5f49 442c  self, source_ID,
+00032cd0: 2069 6961 7361 5f73 6f75 7263 653d 4e6f   iiasa_source=No
+00032ce0: 6e65 2c20 6461 7461 5f66 696c 653d 4e6f  ne, data_file=No
+00032cf0: 6e65 2c20 6d65 7461 5f66 696c 653d 4e6f  ne, meta_file=No
+00032d00: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
+00032d10: 662e 7365 7475 7020 3d20 7365 7475 7053  f.setup = setupS
+00032d20: 7472 7563 7428 290a 0a20 2020 2020 2020  truct()..       
+00032d30: 2073 656c 662e 7365 7475 702e 534f 5552   self.setup.SOUR
+00032d40: 4345 5f49 4420 3d20 736f 7572 6365 5f49  CE_ID = source_I
+00032d50: 440a 0a20 2020 2020 2020 2073 656c 662e  D..        self.
+00032d60: 7365 7475 702e 4441 5441 5f46 494c 4520  setup.DATA_FILE 
+00032d70: 3d20 2727 0a20 2020 2020 2020 2023 2073  = ''.        # s
+00032d80: 656c 662e 7365 7475 702e 4d41 5050 494e  elf.setup.MAPPIN
+00032d90: 475f 4649 4c45 203d 206f 732e 7061 7468  G_FILE = os.path
+00032da0: 2e6a 6f69 6e28 7365 6c66 2e73 6574 7570  .join(self.setup
+00032db0: 2e53 4f55 5243 455f 5041 5448 2c20 276d  .SOURCE_PATH, 'm
+00032dc0: 6170 7069 6e67 2e78 6c73 7827 290a 2020  apping.xlsx').  
+00032dd0: 2020 2020 2020 7365 6c66 2e73 6574 7570        self.setup
+00032de0: 2e4c 4943 454e 4345 203d 2027 3f27 2020  .LICENCE = '?'  
+00032df0: 2320 544f 444f 0a20 2020 2020 2020 2073  # TODO.        s
+00032e00: 656c 662e 7365 7475 702e 5552 4c20 3d20  elf.setup.URL = 
+00032e10: 2764 6174 612e 656e 652e 6969 6173 612e  'data.ene.iiasa.
+00032e20: 6163 2e61 7427 0a0a 2020 2020 2020 2020  ac.at'..        
+00032e30: 7365 6c66 2e53 4f55 5243 455f 4944 203d  self.SOURCE_ID =
+00032e40: 2073 6f75 7263 655f 4944 0a0a 2020 2020   source_ID..    
+00032e50: 2020 2020 6966 2069 6961 7361 5f73 6f75      if iiasa_sou
+00032e60: 7263 6520 6973 206e 6f74 204e 6f6e 653a  rce is not None:
+00032e70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00032e80: 662e 636f 6e6e 203d 2070 7961 6d2e 6969  f.conn = pyam.ii
+00032e90: 6173 612e 436f 6e6e 6563 7469 6f6e 2869  asa.Connection(i
+00032ea0: 6961 7361 5f73 6f75 7263 6529 0a20 2020  iasa_source).   
+00032eb0: 2020 2020 2020 2020 2073 656c 662e 6969           self.ii
+00032ec0: 6173 615f 736f 7572 6365 203d 2069 6961  asa_source = iia
+00032ed0: 7361 5f73 6f75 7263 650a 2020 2020 2020  sa_source.      
+00032ee0: 2020 2020 2020 7365 6c66 2e6d 6574 6120        self.meta 
+00032ef0: 3d20 7365 6c66 2e63 6f6e 6e2e 6d65 7461  = self.conn.meta
+00032f00: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00032f10: 656c 662e 6170 6920 3d20 5472 7565 0a20  elf.api = True. 
+00032f20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00032f30: 6d61 7070 696e 675f 6b65 7920 3d20 6969  mapping_key = ii
+00032f40: 6173 615f 736f 7572 6365 0a0a 2020 2020  asa_source..    
+00032f50: 2020 2020 656c 6966 2064 6174 615f 6669      elif data_fi
+00032f60: 6c65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  le is not None:.
+00032f70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00032f80: 2e64 6174 615f 6669 6c65 203d 2064 6174  .data_file = dat
+00032f90: 615f 6669 6c65 0a20 2020 2020 2020 2020  a_file.         
+00032fa0: 2020 2073 656c 662e 6d65 7461 5f66 696c     self.meta_fil
+00032fb0: 6520 3d20 6d65 7461 5f66 696c 650a 2020  e = meta_file.  
+00032fc0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00032fd0: 6574 6120 3d20 7064 2e44 6174 6146 7261  eta = pd.DataFra
+00032fe0: 6d65 2829 0a20 2020 2020 2020 2020 2020  me().           
+00032ff0: 2073 656c 662e 6170 6920 3d20 4661 6c73   self.api = Fals
+00033000: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
+00033010: 6c66 2e6d 6170 7069 6e67 5f6b 6579 203d  lf.mapping_key =
+00033020: 2073 6f75 7263 655f 4944 0a0a 2020 2020   source_ID..    
+00033030: 2020 2020 7365 6c66 2e72 6567 696f 6e5f      self.region_
+00033040: 6d61 7070 696e 6720 3d20 6469 6374 2829  mapping = dict()
+00033050: 0a0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00033060: 2020 200a 2020 2020 2020 2020 7365 6c66     .        self
+00033070: 2e72 6567 696f 6e5f 6d61 7070 696e 675b  .region_mapping[
+00033080: 2769 616d 6331 3527 5d20 3d6d 6170 7069  'iamc15'] =mappi
+00033090: 6e67 2e49 5043 435f 5352 3135 2829 2e72  ng.IPCC_SR15().r
+000330a0: 6567 696f 6e5f 6d61 7070 696e 6728 290a  egion_mapping().
+000330b0: 2020 2020 2020 2020 7365 6c66 2e72 6567          self.reg
+000330c0: 696f 6e5f 6d61 7070 696e 675b 2749 5043  ion_mapping['IPC
+000330d0: 435f 5352 3135 275d 203d 2073 656c 662e  C_SR15'] = self.
+000330e0: 7265 6769 6f6e 5f6d 6170 7069 6e67 5b27  region_mapping['
+000330f0: 6961 6d63 3135 275d 0a20 2020 2020 2020  iamc15'].       
+00033100: 2073 656c 662e 7265 6769 6f6e 5f6d 6170   self.region_map
+00033110: 7069 6e67 5b22 4941 4d43 3135 5f32 3031  ping["IAMC15_201
+00033120: 395f 5232 225d 203d 2073 656c 662e 7265  9_R2"] = self.re
+00033130: 6769 6f6e 5f6d 6170 7069 6e67 5b22 6961  gion_mapping["ia
+00033140: 6d63 3135 225d 2020 0a20 2020 2020 2020  mc15"]  .       
+00033150: 200a 2020 2020 2020 2020 7365 6c66 2e72   .        self.r
+00033160: 6567 696f 6e5f 6d61 7070 696e 675b 2743  egion_mapping['C
+00033170: 445f 4c49 4e4b 5327 5d20 3d6d 6170 7069  D_LINKS'] =mappi
+00033180: 6e67 2e43 445f 4c49 4e4b 5328 292e 7265  ng.CD_LINKS().re
+00033190: 6769 6f6e 5f6d 6170 7069 6e67 2829 0a20  gion_mapping(). 
+000331a0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000331b0: 7365 6c66 2e72 6567 696f 6e5f 6d61 7070  self.region_mapp
+000331c0: 696e 675b 2765 6e67 6167 6527 5d20 3d6d  ing['engage'] =m
+000331d0: 6170 7069 6e67 2e45 4e47 4147 4528 292e  apping.ENGAGE().
+000331e0: 7265 6769 6f6e 5f6d 6170 7069 6e67 2829  region_mapping()
+000331f0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00033200: 2020 7365 6c66 2e72 6567 696f 6e5f 6d61    self.region_ma
+00033210: 7070 696e 675b 2749 5043 435f 4152 3527  pping['IPCC_AR5'
+00033220: 5d20 3d20 6d61 7070 696e 672e 4950 4343  ] = mapping.IPCC
+00033230: 5f41 5235 2829 2e72 6567 696f 6e5f 6d61  _AR5().region_ma
+00033240: 7070 696e 6728 290a 0a20 2020 2020 2020  pping()..       
+00033250: 2073 656c 662e 7265 6769 6f6e 5f6d 6170   self.region_map
+00033260: 7069 6e67 5b27 4950 4343 5f41 5236 275d  ping['IPCC_AR6']
+00033270: 203d 206d 6170 7069 6e67 2e49 5043 435f   = mapping.IPCC_
+00033280: 4152 3628 292e 7265 6769 6f6e 5f6d 6170  AR6().region_map
+00033290: 7069 6e67 2829 0a20 2020 2020 2020 2073  ping().        s
+000332a0: 656c 662e 7265 6769 6f6e 5f6d 6170 7069  elf.region_mappi
+000332b0: 6e67 5b27 4950 4343 5f41 5236 5f72 6177  ng['IPCC_AR6_raw
+000332c0: 275d 203d 206d 6170 7069 6e67 2e49 5043  '] = mapping.IPC
+000332d0: 435f 4152 3628 292e 7265 6769 6f6e 5f6d  C_AR6().region_m
+000332e0: 6170 7069 6e67 2829 0a20 2020 2020 2020  apping().       
+000332f0: 2073 656c 662e 7265 6769 6f6e 5f6d 6170   self.region_map
+00033300: 7069 6e67 5b27 4950 4343 5f53 5350 5f32  ping['IPCC_SSP_2
+00033310: 3031 3827 5d20 3d20 6d61 7070 696e 672e  018'] = mapping.
+00033320: 4950 4343 5f41 5236 2829 2e72 6567 696f  IPCC_AR6().regio
+00033330: 6e5f 6d61 7070 696e 6728 290a 2020 2020  n_mapping().    
+00033340: 2020 2020 7365 6c66 2e72 6567 696f 6e5f      self.region_
+00033350: 6d61 7070 696e 675b 276e 6766 735f 3227  mapping['ngfs_2'
+00033360: 5d20 3d20 6d61 7070 696e 672e 4e47 4653  ] = mapping.NGFS
+00033370: 2829 2e72 6567 696f 6e5f 6d61 7070 696e  ().region_mappin
+00033380: 6728 290a 0a20 2020 2020 2020 2073 656c  g()..        sel
+00033390: 662e 7265 6769 6f6e 5f6d 6170 7069 6e67  f.region_mapping
+000333a0: 5b27 4144 5641 4e43 4527 5d20 3d20 6d61  ['ADVANCE'] = ma
+000333b0: 7070 696e 672e 4144 5641 4e43 4528 292e  pping.ADVANCE().
+000333c0: 7265 6769 6f6e 5f6d 6170 7069 6e67 2829  region_mapping()
+000333d0: 0a0a 2020 2020 6465 6620 6164 6170 745f  ..    def adapt_
+000333e0: 756e 6974 7328 7365 6c66 2c20 6d65 7461  units(self, meta
+000333f0: 293a 0a20 2020 2020 2020 206d 6574 615b  ):.        meta[
+00033400: 2775 6e69 7427 5d20 3d20 280a 2020 2020  'unit'] = (.    
+00033410: 2020 2020 2020 2020 6d65 7461 5b27 756e          meta['un
+00033420: 6974 275d 0a20 2020 2020 2020 2020 2020  it'].           
+00033430: 202e 7265 706c 6163 6528 276b 7455 272c   .replace('ktU',
+00033440: 2027 6b74 2055 2729 0a20 2020 2020 2020   'kt U').       
+00033450: 2020 2020 202e 7265 706c 6163 6528 274d       .replace('M
+00033460: 7420 434f 322d 6571 7569 762f 7972 272c  t CO2-equiv/yr',
+00033470: 2027 4d74 2043 4f32 6571 2f79 7227 290a   'Mt CO2eq/yr').
+00033480: 2020 2020 2020 2020 2020 2020 2e72 6570              .rep
+00033490: 6c61 6365 2827 6b74 2043 4634 2d65 7175  lace('kt CF4-equ
+000334a0: 6976 2f79 272c 2027 6b74 2043 4634 6571  iv/y', 'kt CF4eq
+000334b0: 2f79 2729 0a20 2020 2020 2020 2020 2020  /y').           
+000334c0: 202e 7265 706c 6163 6528 276b 7420 4846   .replace('kt HF
+000334d0: 4331 3334 612d 6571 7569 762f 7972 272c  C134a-equiv/yr',
+000334e0: 2027 6b74 2048 4643 3133 3461 6571 2f79   'kt HFC134aeq/y
+000334f0: 7227 290a 2020 2020 2020 2020 2020 2020  r').            
+00033500: 2e72 6570 6c61 6365 2827 496e 6465 7820  .replace('Index 
+00033510: 2832 3030 3520 3d20 3129 272c 2027 6469  (2005 = 1)', 'di
+00033520: 6d65 6e73 696f 6e6c 6573 7327 2920 2023  mensionless')  #
+00033530: 203f 3f20 544f 444f 0a20 2020 2020 2020   ?? TODO.       
+00033540: 2020 2020 202e 7265 706c 6163 6528 2755       .replace('U
+00033550: 5324 272c 2027 5553 4427 290a 2020 2020  S$', 'USD').    
+00033560: 2020 2020 2020 2020 2e72 6570 6c61 6365          .replace
+00033570: 2827 6b74 2048 4643 3433 2d31 302f 7972  ('kt HFC43-10/yr
+00033580: 272c 2027 6b74 2048 4643 3433 5f31 302f  ', 'kt HFC43_10/
+00033590: 7972 2729 0a20 2020 2020 2020 2029 0a20  yr').        ). 
+000335a0: 2020 2020 2020 2072 6574 7572 6e20 6d65         return me
+000335b0: 7461 0a0a 2020 2020 6465 6620 6761 7468  ta..    def gath
+000335c0: 6572 4d61 7070 6564 4461 7461 2873 656c  erMappedData(sel
+000335d0: 662c 206d 6f64 656c 733d 4e6f 6e65 2c20  f, models=None, 
+000335e0: 6961 6d63 5f66 696c 7465 723d 5b5d 293a  iamc_filter=[]):
+000335f0: 0a0a 2020 2020 2020 2020 7461 626c 6573  ..        tables
+00033600: 203d 206c 6973 7428 290a 2020 2020 2020   = list().      
+00033610: 2020 7461 626c 6573 5f65 7863 6c75 6465    tables_exclude
+00033620: 6420 3d20 6c69 7374 2829 0a0a 2020 2020  d = list()..    
+00033630: 2020 2020 6966 206e 6f74 2068 6173 6174      if not hasat
+00033640: 7472 2873 656c 662c 2027 6461 7461 2729  tr(self, 'data')
+00033650: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00033660: 206e 6f74 2073 656c 662e 6170 693a 0a20   not self.api:. 
+00033670: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00033680: 206c 6f61 6420 6461 7461 0a20 2020 2020   load data.     
+00033690: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000336a0: 6c6f 6164 4461 7461 2829 0a20 2020 2020  loadData().     
+000336b0: 2020 200a 2020 2020 2020 2020 6966 2027     .        if '
+000336c0: 6d6f 6465 6c27 206e 6f74 2069 6e20 6961  model' not in ia
+000336d0: 6d63 5f66 696c 7465 722e 6b65 7973 2829  mc_filter.keys()
+000336e0: 3a0a 2020 2020 2020 2020 2020 2020 0a20  :.            . 
+000336f0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00033700: 2020 2020 2020 2020 6966 206d 6f64 656c          if model
+00033710: 7320 6973 204e 6f6e 653a 0a20 2020 200a  s is None:.    .
+00033720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00033730: 6966 2073 656c 662e 6170 693a 0a20 2020  if self.api:.   
+00033740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00033750: 206d 6f64 656c 7320 3d20 7365 6c66 2e6d   models = self.m
+00033760: 6574 612e 696e 6465 782e 6765 745f 6c65  eta.index.get_le
+00033770: 7665 6c5f 7661 6c75 6573 2830 292e 756e  vel_values(0).un
+00033780: 6971 7565 2829 0a20 2020 2020 2020 2020  ique().         
+00033790: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000337a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000337b0: 206d 6f64 656c 7320 3d20 7365 6c66 2e64   models = self.d
+000337c0: 6174 612e 6d6f 6465 6c0a 2020 2020 0a20  ata.model.    . 
+000337d0: 2020 2020 2020 2020 2020 2066 6f72 206d             for m
+000337e0: 6f64 656c 2069 6e20 7471 646d 286d 6f64  odel in tqdm(mod
+000337f0: 656c 732c 2064 6573 633d 274c 6f6f 7020  els, desc='Loop 
+00033800: 6f76 6572 206d 6f64 656c 7327 293a 0a20  over models'):. 
+00033810: 2020 200a 2020 2020 2020 2020 2020 2020     .            
+00033820: 2020 2020 6966 2073 656c 662e 6170 693a      if self.api:
+00033830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00033840: 2020 2020 2069 6466 203d 2073 656c 662e       idf = self.
+00033850: 636f 6e6e 2e71 7565 7279 282a 2a69 616d  conn.query(**iam
+00033860: 635f 6669 6c74 6572 2c20 6d6f 6465 6c3d  c_filter, model=
+00033870: 6d6f 6465 6c29 0a20 2020 2020 2020 2020  model).         
+00033880: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00033890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000338a0: 2069 6466 203d 2073 656c 662e 6461 7461   idf = self.data
+000338b0: 2e66 696c 7465 7228 2a2a 6961 6d63 5f66  .filter(**iamc_f
+000338c0: 696c 7465 722c 206d 6f64 656c 3d6d 6f64  ilter, model=mod
+000338d0: 656c 290a 2020 2020 2020 2020 2020 2020  el).            
+000338e0: 2020 2020 7365 6c66 2e69 6466 203d 2069      self.idf = i
+000338f0: 6466 0a20 2020 2020 2020 2020 2020 2020  df.             
+00033900: 2020 2069 6620 6c65 6e28 6964 6629 203d     if len(idf) =
+00033910: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00033920: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00033930: 650a 2020 2020 0a20 2020 2020 2020 2020  e.    .         
+00033940: 2020 2020 2020 2074 6162 6c65 732c 2074         tables, t
+00033950: 6162 6c65 735f 6578 636c 7564 6564 203d  ables_excluded =
+00033960: 2073 656c 662e 5f72 6561 645f 6964 665f   self._read_idf_
+00033970: 6461 7461 280a 2020 2020 2020 2020 2020  data(.          
+00033980: 2020 2020 2020 2020 2020 6964 662c 206d            idf, m
+00033990: 6f64 656c 2c20 7461 626c 6573 2c20 7461  odel, tables, ta
+000339a0: 626c 6573 5f65 7863 6c75 6465 640a 2020  bles_excluded.  
+000339b0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000339c0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000339d0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000339e0: 2e61 7069 3a0a 2020 2020 2020 2020 2020  .api:.          
+000339f0: 2020 2020 2069 6466 203d 2073 656c 662e       idf = self.
+00033a00: 636f 6e6e 2e71 7565 7279 282a 2a69 616d  conn.query(**iam
+00033a10: 635f 6669 6c74 6572 290a 2020 2020 2020  c_filter).      
+00033a20: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00033a30: 2020 2020 2020 2020 2020 6964 6620 3d20            idf = 
+00033a40: 7365 6c66 2e64 6174 612e 6669 6c74 6572  self.data.filter
+00033a50: 282a 2a69 616d 635f 6669 6c74 6572 290a  (**iamc_filter).
+00033a60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00033a70: 6964 6620 3d20 6964 660a 2020 2020 2020  idf = idf.      
+00033a80: 2020 2020 200a 2020 200a 2020 2020 2020       .   .      
+00033a90: 2020 2020 2066 6f72 206d 6f64 656c 2069       for model i
+00033aa0: 6e20 6964 662e 6d6f 6465 6c3a 200a 2020  n idf.model: .  
+00033ab0: 2020 2020 2020 2020 2020 2020 2069 6466               idf
+00033ac0: 5f73 656c 203d 2069 6466 2e66 696c 7465  _sel = idf.filte
+00033ad0: 7228 6d6f 6465 6c3d 6d6f 6465 6c29 0a20  r(model=model). 
+00033ae0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00033af0: 206c 656e 2869 6466 5f73 656c 2920 3d3d   len(idf_sel) ==
+00033b00: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00033b10: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00033b20: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00033b30: 6162 6c65 732c 2074 6162 6c65 735f 6578  ables, tables_ex
+00033b40: 636c 7564 6564 203d 2073 656c 662e 5f72  cluded = self._r
+00033b50: 6561 645f 6964 665f 6461 7461 280a 2020  ead_idf_data(.  
+00033b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00033b70: 2069 6466 5f73 656c 2c20 6d6f 6465 6c2c   idf_sel, model,
+00033b80: 2074 6162 6c65 732c 2074 6162 6c65 735f   tables, tables_
+00033b90: 6578 636c 7564 6564 290a 2020 2020 2020  excluded).      
+00033ba0: 2020 2020 2020 2020 2020 0a0a 2020 2020            ..    
+00033bb0: 2020 2020 7265 7475 726e 2074 6162 6c65      return table
+00033bc0: 732c 2074 6162 6c65 735f 6578 636c 7564  s, tables_exclud
+00033bd0: 6564 0a0a 2020 2020 6465 6620 5f72 6561  ed..    def _rea
+00033be0: 645f 6461 7461 2873 656c 662c 2064 6174  d_data(self, dat
+00033bf0: 615f 6669 6c65 2c20 6d65 7461 5f66 696c  a_file, meta_fil
+00033c00: 653d 4e6f 6e65 2c20 2a2a 6669 6c74 6572  e=None, **filter
+00033c10: 7329 3a0a 2020 2020 2020 2020 7072 696e  s):.        prin
+00033c20: 7428 6627 7265 6164 696e 6720 696e 3a20  t(f'reading in: 
+00033c30: 207b 6461 7461 5f66 696c 657d 2729 0a20   {data_file}'). 
+00033c40: 2020 2020 2020 2064 6174 6120 3d20 7079         data = py
+00033c50: 616d 2e49 616d 4461 7461 4672 616d 6528  am.IamDataFrame(
+00033c60: 6474 2e74 6f6f 6c73 2e70 7961 6d2e 7265  dt.tools.pyam.re
+00033c70: 6164 5f70 6172 7469 616c 2864 6174 615f  ad_partial(data_
+00033c80: 6669 6c65 2c20 2a2a 6669 6c74 6572 7329  file, **filters)
+00033c90: 290a 2020 2020 2020 2020 6966 206d 6574  ).        if met
+00033ca0: 615f 6669 6c65 2069 7320 6e6f 7420 4e6f  a_file is not No
+00033cb0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00033cc0: 6461 7461 2e6c 6f61 645f 6d65 7461 286d  data.load_meta(m
+00033cd0: 6574 615f 6669 6c65 290a 0a20 2020 2020  eta_file)..     
+00033ce0: 2020 2072 6574 7572 6e20 6461 7461 0a0a     return data..
+00033cf0: 2020 2020 6465 6620 6c6f 6164 4461 7461      def loadData
+00033d00: 2873 656c 662c 202a 2a66 696c 7465 7273  (self, **filters
+00033d10: 293a 0a0a 2020 2020 2020 2020 2320 7365  ):..        # se
+00033d20: 6c66 2e64 6174 6120 3d20 7064 2e72 6561  lf.data = pd.rea
+00033d30: 645f 6373 7628 7365 6c66 2e64 6174 615f  d_csv(self.data_
+00033d40: 6669 6c65 290a 2020 2020 2020 2020 6966  file).        if
+00033d50: 2069 7369 6e73 7461 6e63 6528 7365 6c66   isinstance(self
+00033d60: 2e64 6174 615f 6669 6c65 2c20 6c69 7374  .data_file, list
+00033d70: 2920 616e 6420 6973 696e 7374 616e 6365  ) and isinstance
+00033d80: 2873 656c 662e 6461 7461 5f66 696c 652c  (self.data_file,
+00033d90: 206c 6973 7429 3a0a 2020 2020 2020 2020   list):.        
+00033da0: 2020 2020 2320 6d75 6c74 6970 6c65 2066      # multiple f
+00033db0: 696c 6573 0a20 2020 2020 2020 2020 2020  iles.           
+00033dc0: 2064 6174 615f 6c69 7374 203d 206c 6973   data_list = lis
+00033dd0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00033de0: 666f 7220 6461 7461 5f66 696c 652c 206d  for data_file, m
+00033df0: 6574 615f 6669 6c65 2069 6e20 7a69 7028  eta_file in zip(
+00033e00: 7365 6c66 2e64 6174 615f 6669 6c65 2c20  self.data_file, 
+00033e10: 7365 6c66 2e6d 6574 615f 6669 6c65 293a  self.meta_file):
+00033e20: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00033e30: 2020 6461 7461 5f6c 6973 742e 6170 7065    data_list.appe
+00033e40: 6e64 2873 656c 662e 5f72 6561 645f 6461  nd(self._read_da
+00033e50: 7461 2864 6174 615f 6669 6c65 2c20 6d65  ta(data_file, me
+00033e60: 7461 5f66 696c 652c 202a 2a66 696c 7465  ta_file, **filte
+00033e70: 7273 2929 0a0a 2020 2020 2020 2020 2020  rs))..          
+00033e80: 2020 7365 6c66 2e64 6174 6120 3d20 7079    self.data = py
+00033e90: 616d 2e63 6f6e 6361 7428 6461 7461 5f6c  am.concat(data_l
+00033ea0: 6973 7429 0a20 2020 2020 2020 2020 2020  ist).           
+00033eb0: 2073 656c 662e 6d65 7461 203d 2073 656c   self.meta = sel
+00033ec0: 662e 6461 7461 2e6d 6574 610a 2020 2020  f.data.meta.    
+00033ed0: 2020 2020 2020 2020 6465 6c20 6461 7461          del data
+00033ee0: 5f6c 6973 740a 2020 2020 2020 2020 2020  _list.          
+00033ef0: 2020 2320 6465 6c20 6461 7461 0a0a 2020    # del data..  
+00033f00: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00033f10: 2020 2020 2020 2020 2320 7369 6e67 6c65          # single
+00033f20: 2066 696c 650a 2020 2020 2020 2020 2020   file.          
+00033f30: 2020 7365 6c66 2e64 6174 6120 3d20 7365    self.data = se
+00033f40: 6c66 2e5f 7265 6164 5f64 6174 6128 7365  lf._read_data(se
+00033f50: 6c66 2e64 6174 615f 6669 6c65 2c20 7365  lf.data_file, se
+00033f60: 6c66 2e6d 6574 615f 6669 6c65 2c20 2a2a  lf.meta_file, **
+00033f70: 6669 6c74 6572 7329 0a20 2020 2020 2020  filters).       
+00033f80: 2023 2073 6574 7469 6e67 206d 6574 610a   # setting meta.
+00033f90: 2020 2020 2020 2020 7365 6c66 2e6d 6574          self.met
+00033fa0: 6120 3d20 7365 6c66 2e64 6174 612e 6d65  a = self.data.me
+00033fb0: 7461 0a0a 2020 2020 6465 6620 5f72 6561  ta..    def _rea
+00033fc0: 645f 6964 665f 6461 7461 2873 656c 662c  d_idf_data(self,
+00033fd0: 2069 6466 2c20 6d6f 6465 6c2c 2074 6162   idf, model, tab
+00033fe0: 6c65 732c 2074 6162 6c65 735f 6578 636c  les, tables_excl
+00033ff0: 7564 6564 293a 0a0a 2020 2020 2020 2020  uded):..        
+00034000: 7764 6620 3d20 6964 662e 7469 6d65 7365  wdf = idf.timese
+00034010: 7269 6573 2829 0a20 2020 2020 2020 2066  ries().        f
+00034020: 6f72 2073 6365 6e61 7269 6f20 696e 2077  or scenario in w
+00034030: 6466 2e69 6e64 6578 2e67 6574 5f6c 6576  df.index.get_lev
+00034040: 656c 5f76 616c 7565 7328 3129 2e75 6e69  el_values(1).uni
+00034050: 7175 6528 293a 0a20 2020 2020 2020 2020  que():.         
+00034060: 2020 2073 7562 5f73 6365 6e61 7269 6f20     sub_scenario 
+00034070: 3d20 7764 662e 6c6f 635b 736c 6963 6528  = wdf.loc[slice(
+00034080: 4e6f 6e65 292c 205b 7363 656e 6172 696f  None), [scenario
+00034090: 5d2c 2073 6c69 6365 284e 6f6e 6529 2c20  ], slice(None), 
+000340a0: 736c 6963 6528 4e6f 6e65 295d 0a0a 2020  slice(None)]..  
+000340b0: 2020 2020 2020 2020 2020 666f 7220 7661            for va
+000340c0: 7220 696e 2073 7562 5f73 6365 6e61 7269  r in sub_scenari
+000340d0: 6f2e 696e 6465 782e 6765 745f 6c65 7665  o.index.get_leve
+000340e0: 6c5f 7661 6c75 6573 2833 292e 756e 6971  l_values(3).uniq
+000340f0: 7565 2829 3a0a 2020 2020 2020 2020 2020  ue():.          
+00034100: 2020 2020 2020 7375 6273 6574 203d 2028        subset = (
+00034110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00034120: 2020 2020 2073 7562 5f73 6365 6e61 7269       sub_scenari
+00034130: 6f2e 6c6f 635b 736c 6963 6528 4e6f 6e65  o.loc[slice(None
+00034140: 292c 2073 6c69 6365 284e 6f6e 6529 2c20  ), slice(None), 
+00034150: 736c 6963 6528 4e6f 6e65 292c 205b 7661  slice(None), [va
+00034160: 725d 5d0a 2020 2020 2020 2020 2020 2020  r]].            
+00034170: 2020 2020 2020 2020 2e72 6573 6574 5f69          .reset_i
+00034180: 6e64 6578 2829 0a20 2020 2020 2020 2020  ndex().         
+00034190: 2020 2020 2020 2020 2020 202e 7365 745f             .set_
+000341a0: 696e 6465 7828 2772 6567 696f 6e27 290a  index('region').
 000341b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000341c0: 6d65 7461 5f63 6f6c 7320 3d20 7375 6273  meta_cols = subs
-000341d0: 6574 2e63 6f6c 756d 6e73 2e64 6966 6665  et.columns.diffe
-000341e0: 7265 6e63 6528 7469 6d65 5f63 6f6c 7329  rence(time_cols)
-000341f0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00034200: 2020 7461 626c 6520 3d20 6474 2e44 6174    table = dt.Dat
-00034210: 6174 6162 6c65 2873 7562 7365 742e 6c6f  atable(subset.lo
-00034220: 635b 3a2c 2074 696d 655f 636f 6c73 5d29  c[:, time_cols])
-00034230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00034240: 2066 6f72 206d 6574 615f 6b65 7920 696e   for meta_key in
-00034250: 206d 6574 615f 636f 6c73 3a0a 2020 2020   meta_cols:.    
-00034260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00034270: 7461 626c 652e 6d65 7461 5b6d 6574 615f  table.meta[meta_
-00034280: 6b65 795d 203d 206c 6973 7428 7375 6273  key] = list(subs
-00034290: 6574 5b6d 6574 615f 6b65 795d 2e75 6e69  et[meta_key].uni
-000342a0: 7175 6528 2929 5b30 5d0a 2020 2020 2020  que())[0].      
-000342b0: 2020 2020 2020 2020 2020 6966 2028 6d6f            if (mo
-000342c0: 6465 6c2c 2073 6365 6e61 7269 6f29 2069  del, scenario) i
-000342d0: 6e20 7365 6c66 2e6d 6574 612e 696e 6465  n self.meta.inde
-000342e0: 783a 0a20 2020 2020 2020 2020 2020 2020  x:.             
-000342f0: 2020 2020 2020 2066 6f72 206d 6574 615f         for meta_
-00034300: 636f 6c2c 2076 616c 7565 2069 6e20 7365  col, value in se
-00034310: 6c66 2e6d 6574 612e 6c6f 635b 286d 6f64  lf.meta.loc[(mod
-00034320: 656c 2c20 7363 656e 6172 696f 292c 203a  el, scenario), :
-00034330: 5d2e 6974 656d 7328 293a 0a0a 2020 2020  ].items():..    
-00034340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00034350: 2020 2020 2320 6d61 6e75 616c 6c79 2063      # manually c
-00034360: 6861 6e67 6520 6d65 7461 2063 6174 6567  hange meta categ
-00034370: 6f72 7920 746f 2061 766f 6964 206f 7665  ory to avoid ove
-00034380: 7277 7269 7465 206f 6620 6461 7461 746f  rwrite of datato
-00034390: 6f6c 626f 7820 6361 7465 676f 7279 0a20  olbox category. 
-000343a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000343b0: 2020 2020 2020 2069 6620 6d65 7461 5f63         if meta_c
-000343c0: 6f6c 203d 3d20 2763 6174 6567 6f72 7927  ol == 'category'
-000343d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000343e0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-000343f0: 7461 5f63 6f6c 203d 2027 636c 696d 6174  ta_col = 'climat
-00034400: 655f 6361 7465 676f 7279 270a 2020 2020  e_category'.    
-00034410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00034420: 2020 2020 6966 206d 6574 615f 636f 6c20      if meta_col 
-00034430: 6e6f 7420 696e 2063 6f6e 6669 672e 4944  not in config.ID
-00034440: 5f46 4945 4c44 533a 0a20 2020 2020 2020  _FIELDS:.       
-00034450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00034460: 2020 2020 2074 6162 6c65 2e6d 6574 615b       table.meta[
-00034470: 6d65 7461 5f63 6f6c 5d20 3d20 7661 6c75  meta_col] = valu
-00034480: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00034490: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-000344a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000344b0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000344c0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-000344d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000344e0: 2020 2027 5761 726d 696e 673a 2063 6f75     'Warming: cou
-000344f0: 6c64 206e 6f74 2073 6574 206d 6574 6120  ld not set meta 
-00034500: 6b65 7920 7b6d 6574 615f 636f 6c7d 2073  key {meta_col} s
-00034510: 696e 6365 2069 7420 6973 2070 6172 7420  ince it is part 
-00034520: 6f66 2049 4420 6669 656c 6473 270a 2020  of ID fields'.  
-00034530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00034540: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00034550: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
-00034560: 652e 6d65 7461 5b27 736f 7572 6365 275d  e.meta['source']
-00034570: 203d 2073 656c 662e 534f 5552 4345 5f49   = self.SOURCE_I
-00034580: 440a 0a20 2020 2020 2020 2020 2020 2020  D..             
-00034590: 2020 2074 6162 6c65 203d 2073 656c 662e     table = self.
-000345a0: 6164 645f 7374 616e 6461 7264 5f72 6567  add_standard_reg
-000345b0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-000345c0: 2020 2020 2020 2020 2074 6162 6c65 2c20           table, 
-000345d0: 7365 6c66 2e72 6567 696f 6e5f 6d61 7070  self.region_mapp
-000345e0: 696e 675b 7365 6c66 2e6d 6170 7069 6e67  ing[self.mapping
-000345f0: 5f6b 6579 5d0a 2020 2020 2020 2020 2020  _key].          
-00034600: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00034610: 2020 2020 2020 2020 7461 626c 652e 6d65          table.me
-00034620: 7461 203d 2073 656c 662e 6164 6170 745f  ta = self.adapt_
-00034630: 756e 6974 7328 7461 626c 652e 6d65 7461  units(table.meta
-00034640: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00034650: 2020 2074 6162 6c65 2e67 656e 6572 6174     table.generat
-00034660: 6554 6162 6c65 4944 2829 0a20 2020 2020  eTableID().     
-00034670: 2020 2020 2020 2020 2020 2069 6620 6474             if dt
-00034680: 2e63 6f72 652e 5f76 616c 6964 6174 655f  .core._validate_
-00034690: 756e 6974 2874 6162 6c65 293a 0a20 2020  unit(table):.   
-000346a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000346b0: 2074 6162 6c65 732e 6170 7065 6e64 2874   tables.append(t
-000346c0: 6162 6c65 290a 2020 2020 2020 2020 2020  able).          
-000346d0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000346e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000346f0: 7461 626c 6573 5f65 7863 6c75 6465 642e  tables_excluded.
-00034700: 6170 7065 6e64 2874 6162 6c65 290a 2020  append(table).  
-00034710: 2020 2020 2020 7265 7475 726e 2074 6162        return tab
-00034720: 6c65 732c 2074 6162 6c65 735f 6578 636c  les, tables_excl
-00034730: 7564 6564 0a0a 2020 2020 6465 6620 6765  uded..    def ge
-00034740: 745f 7265 6769 6f6e 5f6d 6170 7069 6e67  t_region_mapping
-00034750: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00034760: 7265 7475 726e 2073 656c 662e 7265 6769  return self.regi
-00034770: 6f6e 5f6d 6170 7069 7265 0a0a 0a63 6c61  on_mappire...cla
-00034780: 7373 2043 4154 5f50 6172 6973 5f53 6563  ss CAT_Paris_Sec
-00034790: 746f 725f 526f 6c6c 6f75 7428 4261 7365  tor_Rollout(Base
-000347a0: 496d 706f 7274 546f 6f6c 293a 0a20 2020  ImportTool):.   
-000347b0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-000347c0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-000347d0: 662e 7365 7475 7020 3d20 7365 7475 7053  f.setup = setupS
-000347e0: 7472 7563 7428 290a 2020 2020 2020 2020  truct().        
-000347f0: 7365 6c66 2e73 6574 7570 2e53 4f55 5243  self.setup.SOURC
-00034800: 455f 4944 203d 2022 4341 545f 5053 525f  E_ID = "CAT_PSR_
-00034810: 3230 3139 220a 2020 2020 2020 2020 7365  2019".        se
-00034820: 6c66 2e73 6574 7570 2e53 4f55 5243 455f  lf.setup.SOURCE_
-00034830: 5041 5448 203d 206f 732e 7061 7468 2e6a  PATH = os.path.j
-00034840: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
-00034850: 2063 6f6e 6669 672e 5041 5448 5f54 4f5f   config.PATH_TO_
-00034860: 4441 5441 5348 454c 462c 2027 7261 7764  DATASHELF, 'rawd
-00034870: 6174 612f 4341 545f 5053 525f 3230 3139  ata/CAT_PSR_2019
-00034880: 270a 2020 2020 2020 2020 290a 2020 2020  '.        ).    
-00034890: 2020 2020 7365 6c66 2e73 6574 7570 2e44      self.setup.D
-000348a0: 4154 415f 4649 4c45 203d 206f 732e 7061  ATA_FILE = os.pa
-000348b0: 7468 2e6a 6f69 6e28 0a20 2020 2020 2020  th.join(.       
-000348c0: 2020 2020 2073 656c 662e 7365 7475 702e       self.setup.
-000348d0: 534f 5552 4345 5f50 4154 482c 2027 706f  SOURCE_PATH, 'po
-000348e0: 7274 616c 5f64 6174 615f 616c 6c5f 3136  rtal_data_all_16
-000348f0: 3036 3230 2e63 7376 270a 2020 2020 2020  0620.csv'.      
-00034900: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
-00034910: 2e73 6574 7570 2e4d 4150 5049 4e47 5f46  .setup.MAPPING_F
-00034920: 494c 4520 3d20 6f73 2e70 6174 682e 6a6f  ILE = os.path.jo
-00034930: 696e 2873 656c 662e 7365 7475 702e 534f  in(self.setup.SO
-00034940: 5552 4345 5f50 4154 482c 2027 6d61 7070  URCE_PATH, 'mapp
-00034950: 696e 672e 786c 7378 2729 0a20 2020 2020  ing.xlsx').     
-00034960: 2020 2073 656c 662e 7365 7475 702e 4c49     self.setup.LI
-00034970: 4345 4e43 4520 3d20 2720 4372 6561 7469  CENCE = ' Creati
-00034980: 7665 2043 6f6d 6d6f 6e73 2041 7474 7269  ve Commons Attri
-00034990: 6275 7469 6f6e 2033 2e30 204c 6963 656e  bution 3.0 Licen
-000349a0: 7365 270a 2020 2020 2020 2020 7365 6c66  se'.        self
-000349b0: 2e73 6574 7570 2e55 524c 203d 2027 6874  .setup.URL = 'ht
-000349c0: 7470 733a 2f2f 636c 696d 6174 6561 6374  tps://climateact
-000349d0: 696f 6e74 7261 636b 6572 2e6f 7267 2f64  iontracker.org/d
-000349e0: 6174 612d 706f 7274 616c 2f27 0a0a 2020  ata-portal/'..  
-000349f0: 2020 2020 2020 7365 6c66 2e63 6f6c 756d        self.colum
-00034a00: 735f 746f 5f70 726f 6365 7373 203d 205b  s_to_process = [
-00034a10: 2776 6172 6961 626c 6527 2c20 2773 6365  'variable', 'sce
-00034a20: 6e61 7269 6f27 2c20 2772 6567 696f 6e27  nario', 'region'
-00034a30: 5d0a 0a20 2020 2020 2020 2023 2020 2020  ]..        #    
-00034a40: 2020 2020 7365 6c66 2e73 6574 7570 2e4d      self.setup.M
-00034a50: 4f44 454c 5f43 4f4c 554d 4e5f 4e41 4d45  ODEL_COLUMN_NAME
-00034a60: 203d 2027 6d6f 6465 6c27 0a20 2020 2020   = 'model'.     
-00034a70: 2020 2073 656c 662e 7365 7475 702e 5343     self.setup.SC
-00034a80: 454e 4152 494f 5f43 4f4c 554d 4e5f 4e41  ENARIO_COLUMN_NA
-00034a90: 4d45 203d 2027 7661 7269 6162 6c65 270a  ME = 'variable'.
-00034aa0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00034ab0: 7570 2e52 4547 494f 4e5f 434f 4c55 4d4e  up.REGION_COLUMN
-00034ac0: 5f4e 414d 4520 3d20 2763 6f75 6e74 7279  _NAME = 'country
-00034ad0: 270a 2020 2020 2020 2020 7365 6c66 2e73  '.        self.s
-00034ae0: 6574 7570 2e56 4152 4941 424c 455f 434f  etup.VARIABLE_CO
-00034af0: 4c55 4d4e 5f4e 414d 4520 3d20 276f 6c64  LUMN_NAME = 'old
-00034b00: 5f76 6172 270a 0a20 2020 2020 2020 2073  _var'..        s
-00034b10: 656c 662e 7365 7475 702e 636f 6c75 6d6e  elf.setup.column
-00034b20: 4d61 7070 696e 6720 3d20 7b0a 2020 2020  Mapping = {.    
-00034b30: 2020 2020 2020 2020 2776 6172 6961 626c          'variabl
-00034b40: 6527 3a20 2765 6e74 6974 7927 2c0a 2020  e': 'entity',.  
-00034b50: 2020 2020 2020 2020 2020 2772 6567 696f            'regio
-00034b60: 6e27 3a20 2772 6567 696f 6e27 2c0a 2020  n': 'region',.  
-00034b70: 2020 2020 2020 2020 2020 2773 6365 6e61            'scena
-00034b80: 7269 6f27 3a20 2773 6365 6e61 7269 6f27  rio': 'scenario'
-00034b90: 2c0a 2020 2020 2020 2020 7d0a 0a20 2020  ,.        }..   
-00034ba0: 2020 2020 2069 6620 6e6f 7420 286f 732e       if not (os.
-00034bb0: 7061 7468 2e65 7869 7374 7328 7365 6c66  path.exists(self
-00034bc0: 2e73 6574 7570 2e4d 4150 5049 4e47 5f46  .setup.MAPPING_F
-00034bd0: 494c 4529 293a 0a20 2020 2020 2020 2020  ILE)):.         
-00034be0: 2020 2073 656c 662e 6372 6561 7465 5661     self.createVa
-00034bf0: 7269 6162 6c65 4d61 7070 696e 6728 290a  riableMapping().
-00034c00: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00034c10: 7428 226e 6f20 6d61 7070 696e 6720 6669  t("no mapping fi
-00034c20: 6c65 2066 6f75 6e64 2229 0a20 2020 2020  le found").     
-00034c30: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00034c40: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
-00034c50: 6720 3d20 6469 6374 2829 0a0a 2020 2020  g = dict()..    
-00034c60: 2020 2020 2020 2020 666f 7220 7661 7220          for var 
-00034c70: 696e 2073 656c 662e 636f 6c75 6d73 5f74  in self.colums_t
-00034c80: 6f5f 7072 6f63 6573 733a 0a20 2020 2020  o_process:.     
-00034c90: 2020 2020 2020 2020 2020 2064 6620 3d20             df = 
-00034ca0: 7064 2e72 6561 645f 6578 6365 6c28 0a20  pd.read_excel(. 
-00034cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00034cc0: 2020 2073 656c 662e 7365 7475 702e 4d41     self.setup.MA
-00034cd0: 5050 494e 475f 4649 4c45 2c20 7368 6565  PPING_FILE, shee
-00034ce0: 745f 6e61 6d65 3d76 6172 202b 2027 5f6d  t_name=var + '_m
-00034cf0: 6170 7069 6e67 272c 2069 6e64 6578 5f63  apping', index_c
-00034d00: 6f6c 3d30 0a20 2020 2020 2020 2020 2020  ol=0.           
-00034d10: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00034d20: 2020 2020 2020 2064 6620 3d20 6466 2e6c         df = df.l
-00034d30: 6f63 5b7e 6466 2e6c 6f63 5b3a 2c20 7365  oc[~df.loc[:, se
-00034d40: 6c66 2e73 6574 7570 2e63 6f6c 756d 6e4d  lf.setup.columnM
-00034d50: 6170 7069 6e67 5b76 6172 5d5d 2e69 736e  apping[var]].isn
-00034d60: 6128 295d 0a20 2020 2020 2020 2020 2020  a()].           
-00034d70: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
-00034d80: 672e 7570 6461 7465 2864 662e 746f 5f64  g.update(df.to_d
-00034d90: 6963 7428 2929 0a0a 2020 2020 2020 2020  ict())..        
-00034da0: 7365 6c66 2e63 7265 6174 6553 6f75 7263  self.createSourc
-00034db0: 654d 6574 6128 290a 0a20 2020 2064 6566  eMeta()..    def
-00034dc0: 206c 6f61 6444 6174 6128 7365 6c66 293a   loadData(self):
-00034dd0: 0a20 2020 2020 2020 2073 656c 662e 6461  .        self.da
-00034de0: 7461 203d 2070 642e 7265 6164 5f63 7376  ta = pd.read_csv
-00034df0: 2873 656c 662e 7365 7475 702e 4441 5441  (self.setup.DATA
-00034e00: 5f46 494c 452c 2069 6e64 6578 5f63 6f6c  _FILE, index_col
-00034e10: 3d4e 6f6e 652c 2068 6561 6465 723d 3029  =None, header=0)
-00034e20: 0a20 2020 2020 2020 2073 656c 662e 6461  .        self.da
-00034e30: 7461 2e6c 6f63 5b3a 2c20 276f 6c64 5f76  ta.loc[:, 'old_v
-00034e40: 6172 275d 203d 2073 656c 662e 6461 7461  ar'] = self.data
-00034e50: 2e6c 6f63 5b3a 2c20 5b27 7365 6374 6f72  .loc[:, ['sector
-00034e60: 272c 2027 696e 6469 6361 746f 7227 5d5d  ', 'indicator']]
-00034e70: 2e61 7070 6c79 280a 2020 2020 2020 2020  .apply(.        
-00034e80: 2020 2020 6c61 6d62 6461 2078 3a20 275f      lambda x: '_
-00034e90: 272e 6a6f 696e 286d 6170 2873 7472 2c20  '.join(map(str, 
-00034ea0: 7829 292c 2061 7869 733d 310a 2020 2020  x)), axis=1.    
-00034eb0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-00034ec0: 6c66 2e64 6174 612e 6c6f 635b 3a2c 2027  lf.data.loc[:, '
-00034ed0: 7363 656e 6172 696f 275d 203d 2073 656c  scenario'] = sel
-00034ee0: 662e 6461 7461 2e6c 6f63 5b3a 2c20 2776  f.data.loc[:, 'v
-00034ef0: 6172 6961 626c 6527 5d0a 2020 2020 2020  ariable'].      
-00034f00: 2020 7365 6c66 2e64 6174 612e 6c6f 635b    self.data.loc[
-00034f10: 3a2c 2027 7265 6769 6f6e 275d 203d 2073  :, 'region'] = s
-00034f20: 656c 662e 6461 7461 2e6c 6f63 5b3a 2c20  elf.data.loc[:, 
-00034f30: 2763 6f75 6e74 7279 275d 0a20 2020 2020  'country'].     
-00034f40: 2020 2073 656c 662e 6461 7461 2e6c 6f63     self.data.loc
-00034f50: 5b3a 2c20 276d 6f64 656c 275d 203d 2027  [:, 'model'] = '
-00034f60: 270a 2020 2020 2020 2020 7365 6c66 2e64  '.        self.d
-00034f70: 6174 612e 6c6f 635b 3a2c 2027 7661 7269  ata.loc[:, 'vari
-00034f80: 6162 6c65 275d 203d 2073 656c 662e 6461  able'] = self.da
-00034f90: 7461 2e6c 6f63 5b3a 2c20 276f 6c64 5f76  ta.loc[:, 'old_v
-00034fa0: 6172 275d 0a0a 2020 2020 6465 6620 6372  ar']..    def cr
-00034fb0: 6561 7465 5661 7269 6162 6c65 4d61 7070  eateVariableMapp
-00034fc0: 696e 6728 7365 6c66 293a 0a0a 2020 2020  ing(self):..    
-00034fd0: 2020 2020 2320 6c6f 6164 696e 6720 6461      # loading da
-00034fe0: 7461 2069 6620 6e65 6365 7373 6172 790a  ta if necessary.
-00034ff0: 2020 2020 2020 2020 6966 206e 6f74 2068          if not h
-00035000: 6173 6174 7472 2873 656c 662c 2027 6461  asattr(self, 'da
-00035010: 7461 2729 3a0a 2020 2020 2020 2020 2020  ta'):.          
-00035020: 2020 7365 6c66 2e6c 6f61 6444 6174 6128    self.loadData(
-00035030: 290a 0a20 2020 2020 2020 2069 6d70 6f72  )..        impor
-00035040: 7420 6e75 6d70 7920 6173 206e 700a 0a20  t numpy as np.. 
-00035050: 2020 2020 2020 2077 7269 7465 7220 3d20         writer = 
-00035060: 7064 2e45 7863 656c 5772 6974 6572 280a  pd.ExcelWriter(.
-00035070: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00035080: 2e73 6574 7570 2e4d 4150 5049 4e47 5f46  .setup.MAPPING_F
-00035090: 494c 452c 0a20 2020 2020 2020 2020 2020  ILE,.           
-000350a0: 2065 6e67 696e 653d 2778 6c73 7877 7269   engine='xlsxwri
-000350b0: 7465 7227 2c0a 2020 2020 2020 2020 2020  ter',.          
-000350c0: 2020 6461 7465 7469 6d65 5f66 6f72 6d61    datetime_forma
-000350d0: 743d 276d 6d6d 2064 2079 7979 7920 6868  t='mmm d yyyy hh
-000350e0: 3a6d 6d3a 7373 272c 0a20 2020 2020 2020  :mm:ss',.       
-000350f0: 2020 2020 2064 6174 655f 666f 726d 6174       date_format
-00035100: 3d27 6d6d 6d6d 2064 6420 7979 7979 272c  ='mmmm dd yyyy',
-00035110: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00035120: 2020 2020 2320 7661 7269 6162 6c65 730a      # variables.
-00035130: 2020 2020 2020 2020 2320 696e 6465 7820          # index 
-00035140: 3d20 7365 6c66 2e64 6174 615b 7365 6c66  = self.data[self
-00035150: 2e73 6574 7570 2e56 4152 4941 424c 455f  .setup.VARIABLE_
-00035160: 434f 4c55 4d4e 5f4e 414d 455d 2e75 6e69  COLUMN_NAME].uni
-00035170: 7175 6528 290a 2020 2020 2020 2020 7365  que().        se
-00035180: 6c66 2e61 7661 696c 6162 6c65 5365 7269  lf.availableSeri
-00035190: 6573 203d 2073 656c 662e 6461 7461 2e64  es = self.data.d
-000351a0: 726f 705f 6475 706c 6963 6174 6573 280a  rop_duplicates(.
-000351b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000351c0: 2e73 6574 7570 2e56 4152 4941 424c 455f  .setup.VARIABLE_
-000351d0: 434f 4c55 4d4e 5f4e 414d 450a 2020 2020  COLUMN_NAME.    
-000351e0: 2020 2020 292e 7365 745f 696e 6465 7828      ).set_index(
-000351f0: 7365 6c66 2e73 6574 7570 2e56 4152 4941  self.setup.VARIA
-00035200: 424c 455f 434f 4c55 4d4e 5f4e 414d 4529  BLE_COLUMN_NAME)
-00035210: 5b27 756e 6974 275d 0a20 2020 2020 2020  ['unit'].       
-00035220: 2073 656c 662e 6d61 7070 696e 6720 3d20   self.mapping = 
-00035230: 7064 2e44 6174 6146 7261 6d65 280a 2020  pd.DataFrame(.  
-00035240: 2020 2020 2020 2020 2020 696e 6465 783d            index=
-00035250: 7365 6c66 2e61 7661 696c 6162 6c65 5365  self.availableSe
-00035260: 7269 6573 2e69 6e64 6578 2c20 636f 6c75  ries.index, colu
-00035270: 6d6e 733d 5b27 656e 6974 7479 272c 2027  mns=['enitty', '
-00035280: 6361 7465 676f 7279 275d 0a20 2020 2020  category'].     
-00035290: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-000352a0: 662e 6d61 7070 696e 6720 3d20 7064 2e63  f.mapping = pd.c
-000352b0: 6f6e 6361 7428 5b73 656c 662e 6d61 7070  oncat([self.mapp
-000352c0: 696e 672c 2073 656c 662e 6176 6169 6c61  ing, self.availa
-000352d0: 626c 6553 6572 6965 735d 2c20 6178 6973  bleSeries], axis
-000352e0: 3d31 290a 2020 2020 2020 2020 7365 6c66  =1).        self
-000352f0: 2e6d 6170 7069 6e67 203d 2073 656c 662e  .mapping = self.
-00035300: 6d61 7070 696e 672e 736f 7274 5f69 6e64  mapping.sort_ind
-00035310: 6578 2829 0a20 2020 2020 2020 2073 656c  ex().        sel
-00035320: 662e 6d61 7070 696e 672e 746f 5f65 7863  f.mapping.to_exc
-00035330: 656c 2877 7269 7465 722c 2065 6e67 696e  el(writer, engin
-00035340: 653d 276f 7065 6e70 7978 6c27 2c20 7368  e='openpyxl', sh
-00035350: 6565 745f 6e61 6d65 3d56 4152 5f4d 4150  eet_name=VAR_MAP
-00035360: 5049 4e47 5f53 4845 4554 290a 0a20 2020  PING_SHEET)..   
-00035370: 2020 2020 2023 206d 6f64 656c 730a 2020       # models.  
-00035380: 2020 2020 2020 2320 2020 2020 2020 2069        #        i
-00035390: 6e64 6578 203d 206e 702e 756e 6971 7565  ndex = np.unique
-000353a0: 2873 656c 662e 6461 7461 5b73 656c 662e  (self.data[self.
-000353b0: 7365 7475 702e 4d4f 4445 4c5f 434f 4c55  setup.MODEL_COLU
-000353c0: 4d4e 5f4e 414d 455d 2e76 616c 7565 7329  MN_NAME].values)
-000353d0: 0a0a 2020 2020 2020 2020 2320 2020 2020  ..        #     
-000353e0: 2020 2073 656c 662e 6176 6169 6c61 626c     self.availabl
-000353f0: 6553 6572 6965 7320 3d20 7064 2e44 6174  eSeries = pd.Dat
-00035400: 6146 7261 6d65 2869 6e64 6578 3d69 6e64  aFrame(index=ind
-00035410: 6578 290a 2020 2020 2020 2020 2320 2020  ex).        #   
-00035420: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
-00035430: 6720 3d20 7064 2e44 6174 6146 7261 6d65  g = pd.DataFrame
-00035440: 2869 6e64 6578 3d69 6e64 6578 2c20 636f  (index=index, co
-00035450: 6c75 6d6e 7320 3d20 5b73 656c 662e 7365  lumns = [self.se
-00035460: 7475 702e 4d4f 4445 4c5f 434f 4c55 4d4e  tup.MODEL_COLUMN
-00035470: 5f4e 414d 455d 290a 2020 2020 2020 2020  _NAME]).        
-00035480: 2320 2020 2020 2020 2073 656c 662e 6d61  #        self.ma
-00035490: 7070 696e 6720 3d20 7064 2e63 6f6e 6361  pping = pd.conca
-000354a0: 7428 5b73 656c 662e 6d61 7070 696e 672c  t([self.mapping,
-000354b0: 2073 656c 662e 6176 6169 6c61 626c 6553   self.availableS
-000354c0: 6572 6965 735d 2c20 6178 6973 3d31 290a  eries], axis=1).
+000341c0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+000341d0: 2020 2074 696d 655f 636f 6c73 203d 2064     time_cols = d
+000341e0: 742e 7574 696c 2e79 6561 7273 436f 6c75  t.util.yearsColu
+000341f0: 6d6e 734f 6e6c 7928 7375 6273 6574 2e63  mnsOnly(subset.c
+00034200: 6f6c 756d 6e73 290a 2020 2020 2020 2020  olumns).        
+00034210: 2020 2020 2020 2020 6d65 7461 5f63 6f6c          meta_col
+00034220: 7320 3d20 7375 6273 6574 2e63 6f6c 756d  s = subset.colum
+00034230: 6e73 2e64 6966 6665 7265 6e63 6528 7469  ns.difference(ti
+00034240: 6d65 5f63 6f6c 7329 0a0a 2020 2020 2020  me_cols)..      
+00034250: 2020 2020 2020 2020 2020 7461 626c 6520            table 
+00034260: 3d20 6474 2e44 6174 6174 6162 6c65 2873  = dt.Datatable(s
+00034270: 7562 7365 742e 6c6f 635b 3a2c 2074 696d  ubset.loc[:, tim
+00034280: 655f 636f 6c73 5d29 0a20 2020 2020 2020  e_cols]).       
+00034290: 2020 2020 2020 2020 2066 6f72 206d 6574           for met
+000342a0: 615f 6b65 7920 696e 206d 6574 615f 636f  a_key in meta_co
+000342b0: 6c73 3a0a 2020 2020 2020 2020 2020 2020  ls:.            
+000342c0: 2020 2020 2020 2020 7461 626c 652e 6d65          table.me
+000342d0: 7461 5b6d 6574 615f 6b65 795d 203d 206c  ta[meta_key] = l
+000342e0: 6973 7428 7375 6273 6574 5b6d 6574 615f  ist(subset[meta_
+000342f0: 6b65 795d 2e75 6e69 7175 6528 2929 5b30  key].unique())[0
+00034300: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00034310: 2020 6966 2028 6d6f 6465 6c2c 2073 6365    if (model, sce
+00034320: 6e61 7269 6f29 2069 6e20 7365 6c66 2e6d  nario) in self.m
+00034330: 6574 612e 696e 6465 783a 0a20 2020 2020  eta.index:.     
+00034340: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00034350: 6f72 206d 6574 615f 636f 6c2c 2076 616c  or meta_col, val
+00034360: 7565 2069 6e20 7365 6c66 2e6d 6574 612e  ue in self.meta.
+00034370: 6c6f 635b 286d 6f64 656c 2c20 7363 656e  loc[(model, scen
+00034380: 6172 696f 292c 203a 5d2e 6974 656d 7328  ario), :].items(
+00034390: 293a 0a0a 2020 2020 2020 2020 2020 2020  ):..            
+000343a0: 2020 2020 2020 2020 2020 2020 2320 6d61              # ma
+000343b0: 6e75 616c 6c79 2063 6861 6e67 6520 6d65  nually change me
+000343c0: 7461 2063 6174 6567 6f72 7920 746f 2061  ta category to a
+000343d0: 766f 6964 206f 7665 7277 7269 7465 206f  void overwrite o
+000343e0: 6620 6461 7461 746f 6f6c 626f 7820 6361  f datatoolbox ca
+000343f0: 7465 676f 7279 0a20 2020 2020 2020 2020  tegory.         
+00034400: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00034410: 6620 6d65 7461 5f63 6f6c 203d 3d20 2763  f meta_col == 'c
+00034420: 6174 6567 6f72 7927 3a0a 2020 2020 2020  ategory':.      
+00034430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00034440: 2020 2020 2020 6d65 7461 5f63 6f6c 203d        meta_col =
+00034450: 2027 636c 696d 6174 655f 6361 7465 676f   'climate_catego
+00034460: 7279 270a 2020 2020 2020 2020 2020 2020  ry'.            
+00034470: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+00034480: 6574 615f 636f 6c20 6e6f 7420 696e 2063  eta_col not in c
+00034490: 6f6e 6669 672e 4944 5f46 4945 4c44 533a  onfig.ID_FIELDS:
+000344a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000344b0: 2020 2020 2020 2020 2020 2020 2074 6162               tab
+000344c0: 6c65 2e6d 6574 615b 6d65 7461 5f63 6f6c  le.meta[meta_col
+000344d0: 5d20 3d20 7661 6c75 650a 2020 2020 2020  ] = value.      
+000344e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000344f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00034500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00034510: 2020 2020 7072 696e 7428 0a20 2020 2020      print(.     
+00034520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00034530: 2020 2020 2020 2020 2020 2027 5761 726d             'Warm
+00034540: 696e 673a 2063 6f75 6c64 206e 6f74 2073  ing: could not s
+00034550: 6574 206d 6574 6120 6b65 7920 7b6d 6574  et meta key {met
+00034560: 615f 636f 6c7d 2073 696e 6365 2069 7420  a_col} since it 
+00034570: 6973 2070 6172 7420 6f66 2049 4420 6669  is part of ID fi
+00034580: 656c 6473 270a 2020 2020 2020 2020 2020  elds'.          
+00034590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000345a0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000345b0: 2020 2020 7461 626c 652e 6d65 7461 5b27      table.meta['
+000345c0: 736f 7572 6365 275d 203d 2073 656c 662e  source'] = self.
+000345d0: 534f 5552 4345 5f49 440a 0a20 2020 2020  SOURCE_ID..     
+000345e0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+000345f0: 203d 2073 656c 662e 6164 645f 7374 616e   = self.add_stan
+00034600: 6461 7264 5f72 6567 696f 6e28 0a20 2020  dard_region(.   
+00034610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00034620: 2074 6162 6c65 2c20 7365 6c66 2e72 6567   table, self.reg
+00034630: 696f 6e5f 6d61 7070 696e 675b 7365 6c66  ion_mapping[self
+00034640: 2e6d 6170 7069 6e67 5f6b 6579 5d0a 2020  .mapping_key].  
+00034650: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00034660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00034670: 7461 626c 652e 6d65 7461 203d 2073 656c  table.meta = sel
+00034680: 662e 6164 6170 745f 756e 6974 7328 7461  f.adapt_units(ta
+00034690: 626c 652e 6d65 7461 290a 0a20 2020 2020  ble.meta)..     
+000346a0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+000346b0: 2e67 656e 6572 6174 6554 6162 6c65 4944  .generateTableID
+000346c0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+000346d0: 2020 2069 6620 6474 2e63 6f72 652e 5f76     if dt.core._v
+000346e0: 616c 6964 6174 655f 756e 6974 2874 6162  alidate_unit(tab
+000346f0: 6c65 293a 0a20 2020 2020 2020 2020 2020  le):.           
+00034700: 2020 2020 2020 2020 2074 6162 6c65 732e           tables.
+00034710: 6170 7065 6e64 2874 6162 6c65 290a 2020  append(table).  
+00034720: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00034730: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00034740: 2020 2020 2020 2020 7461 626c 6573 5f65          tables_e
+00034750: 7863 6c75 6465 642e 6170 7065 6e64 2874  xcluded.append(t
+00034760: 6162 6c65 290a 2020 2020 2020 2020 7265  able).        re
+00034770: 7475 726e 2074 6162 6c65 732c 2074 6162  turn tables, tab
+00034780: 6c65 735f 6578 636c 7564 6564 0a0a 2020  les_excluded..  
+00034790: 2020 6465 6620 6765 745f 7265 6769 6f6e    def get_region
+000347a0: 5f6d 6170 7069 6e67 2873 656c 6629 3a0a  _mapping(self):.
+000347b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000347c0: 656c 662e 7265 6769 6f6e 5f6d 6170 7069  elf.region_mappi
+000347d0: 7265 0a0a 0a63 6c61 7373 2043 4154 5f50  re...class CAT_P
+000347e0: 6172 6973 5f53 6563 746f 725f 526f 6c6c  aris_Sector_Roll
+000347f0: 6f75 7428 4261 7365 496d 706f 7274 546f  out(BaseImportTo
+00034800: 6f6c 293a 0a20 2020 2064 6566 205f 5f69  ol):.    def __i
+00034810: 6e69 745f 5f28 7365 6c66 293a 0a20 2020  nit__(self):.   
+00034820: 2020 2020 2073 656c 662e 7365 7475 7020       self.setup 
+00034830: 3d20 7365 7475 7053 7472 7563 7428 290a  = setupStruct().
+00034840: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00034850: 7570 2e53 4f55 5243 455f 4944 203d 2022  up.SOURCE_ID = "
+00034860: 4341 545f 5053 525f 3230 3139 220a 2020  CAT_PSR_2019".  
+00034870: 2020 2020 2020 7365 6c66 2e73 6574 7570        self.setup
+00034880: 2e53 4f55 5243 455f 5041 5448 203d 206f  .SOURCE_PATH = o
+00034890: 732e 7061 7468 2e6a 6f69 6e28 0a20 2020  s.path.join(.   
+000348a0: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
+000348b0: 5041 5448 5f54 4f5f 4441 5441 5348 454c  PATH_TO_DATASHEL
+000348c0: 462c 2027 7261 7764 6174 612f 4341 545f  F, 'rawdata/CAT_
+000348d0: 5053 525f 3230 3139 270a 2020 2020 2020  PSR_2019'.      
+000348e0: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+000348f0: 2e73 6574 7570 2e44 4154 415f 4649 4c45  .setup.DATA_FILE
+00034900: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00034910: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00034920: 662e 7365 7475 702e 534f 5552 4345 5f50  f.setup.SOURCE_P
+00034930: 4154 482c 2027 706f 7274 616c 5f64 6174  ATH, 'portal_dat
+00034940: 615f 616c 6c5f 3136 3036 3230 2e63 7376  a_all_160620.csv
+00034950: 270a 2020 2020 2020 2020 290a 2020 2020  '.        ).    
+00034960: 2020 2020 7365 6c66 2e73 6574 7570 2e4d      self.setup.M
+00034970: 4150 5049 4e47 5f46 494c 4520 3d20 6f73  APPING_FILE = os
+00034980: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
+00034990: 7365 7475 702e 534f 5552 4345 5f50 4154  setup.SOURCE_PAT
+000349a0: 482c 2027 6d61 7070 696e 672e 786c 7378  H, 'mapping.xlsx
+000349b0: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+000349c0: 7365 7475 702e 4c49 4345 4e43 4520 3d20  setup.LICENCE = 
+000349d0: 2720 4372 6561 7469 7665 2043 6f6d 6d6f  ' Creative Commo
+000349e0: 6e73 2041 7474 7269 6275 7469 6f6e 2033  ns Attribution 3
+000349f0: 2e30 204c 6963 656e 7365 270a 2020 2020  .0 License'.    
+00034a00: 2020 2020 7365 6c66 2e73 6574 7570 2e55      self.setup.U
+00034a10: 524c 203d 2027 6874 7470 733a 2f2f 636c  RL = 'https://cl
+00034a20: 696d 6174 6561 6374 696f 6e74 7261 636b  imateactiontrack
+00034a30: 6572 2e6f 7267 2f64 6174 612d 706f 7274  er.org/data-port
+00034a40: 616c 2f27 0a0a 2020 2020 2020 2020 7365  al/'..        se
+00034a50: 6c66 2e63 6f6c 756d 735f 746f 5f70 726f  lf.colums_to_pro
+00034a60: 6365 7373 203d 205b 2776 6172 6961 626c  cess = ['variabl
+00034a70: 6527 2c20 2773 6365 6e61 7269 6f27 2c20  e', 'scenario', 
+00034a80: 2772 6567 696f 6e27 5d0a 0a20 2020 2020  'region']..     
+00034a90: 2020 2023 2020 2020 2020 2020 7365 6c66     #        self
+00034aa0: 2e73 6574 7570 2e4d 4f44 454c 5f43 4f4c  .setup.MODEL_COL
+00034ab0: 554d 4e5f 4e41 4d45 203d 2027 6d6f 6465  UMN_NAME = 'mode
+00034ac0: 6c27 0a20 2020 2020 2020 2073 656c 662e  l'.        self.
+00034ad0: 7365 7475 702e 5343 454e 4152 494f 5f43  setup.SCENARIO_C
+00034ae0: 4f4c 554d 4e5f 4e41 4d45 203d 2027 7661  OLUMN_NAME = 'va
+00034af0: 7269 6162 6c65 270a 2020 2020 2020 2020  riable'.        
+00034b00: 7365 6c66 2e73 6574 7570 2e52 4547 494f  self.setup.REGIO
+00034b10: 4e5f 434f 4c55 4d4e 5f4e 414d 4520 3d20  N_COLUMN_NAME = 
+00034b20: 2763 6f75 6e74 7279 270a 2020 2020 2020  'country'.      
+00034b30: 2020 7365 6c66 2e73 6574 7570 2e56 4152    self.setup.VAR
+00034b40: 4941 424c 455f 434f 4c55 4d4e 5f4e 414d  IABLE_COLUMN_NAM
+00034b50: 4520 3d20 276f 6c64 5f76 6172 270a 0a20  E = 'old_var'.. 
+00034b60: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
+00034b70: 702e 636f 6c75 6d6e 4d61 7070 696e 6720  p.columnMapping 
+00034b80: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00034b90: 2776 6172 6961 626c 6527 3a20 2765 6e74  'variable': 'ent
+00034ba0: 6974 7927 2c0a 2020 2020 2020 2020 2020  ity',.          
+00034bb0: 2020 2772 6567 696f 6e27 3a20 2772 6567    'region': 'reg
+00034bc0: 696f 6e27 2c0a 2020 2020 2020 2020 2020  ion',.          
+00034bd0: 2020 2773 6365 6e61 7269 6f27 3a20 2773    'scenario': 's
+00034be0: 6365 6e61 7269 6f27 2c0a 2020 2020 2020  cenario',.      
+00034bf0: 2020 7d0a 0a20 2020 2020 2020 2069 6620    }..        if 
+00034c00: 6e6f 7420 286f 732e 7061 7468 2e65 7869  not (os.path.exi
+00034c10: 7374 7328 7365 6c66 2e73 6574 7570 2e4d  sts(self.setup.M
+00034c20: 4150 5049 4e47 5f46 494c 4529 293a 0a20  APPING_FILE)):. 
+00034c30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00034c40: 6372 6561 7465 5661 7269 6162 6c65 4d61  createVariableMa
+00034c50: 7070 696e 6728 290a 2020 2020 2020 2020  pping().        
+00034c60: 2020 2020 7072 696e 7428 226e 6f20 6d61      print("no ma
+00034c70: 7070 696e 6720 6669 6c65 2066 6f75 6e64  pping file found
+00034c80: 2229 0a20 2020 2020 2020 2065 6c73 653a  ").        else:
+00034c90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00034ca0: 662e 6d61 7070 696e 6720 3d20 6469 6374  f.mapping = dict
+00034cb0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+00034cc0: 666f 7220 7661 7220 696e 2073 656c 662e  for var in self.
+00034cd0: 636f 6c75 6d73 5f74 6f5f 7072 6f63 6573  colums_to_proces
+00034ce0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00034cf0: 2020 2064 6620 3d20 7064 2e72 6561 645f     df = pd.read_
+00034d00: 6578 6365 6c28 0a20 2020 2020 2020 2020  excel(.         
+00034d10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00034d20: 7365 7475 702e 4d41 5050 494e 475f 4649  setup.MAPPING_FI
+00034d30: 4c45 2c20 7368 6565 745f 6e61 6d65 3d76  LE, sheet_name=v
+00034d40: 6172 202b 2027 5f6d 6170 7069 6e67 272c  ar + '_mapping',
+00034d50: 2069 6e64 6578 5f63 6f6c 3d30 0a20 2020   index_col=0.   
+00034d60: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00034d70: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00034d80: 6620 3d20 6466 2e6c 6f63 5b7e 6466 2e6c  f = df.loc[~df.l
+00034d90: 6f63 5b3a 2c20 7365 6c66 2e73 6574 7570  oc[:, self.setup
+00034da0: 2e63 6f6c 756d 6e4d 6170 7069 6e67 5b76  .columnMapping[v
+00034db0: 6172 5d5d 2e69 736e 6128 295d 0a20 2020  ar]].isna()].   
+00034dc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00034dd0: 662e 6d61 7070 696e 672e 7570 6461 7465  f.mapping.update
+00034de0: 2864 662e 746f 5f64 6963 7428 2929 0a0a  (df.to_dict())..
+00034df0: 2020 2020 2020 2020 7365 6c66 2e63 7265          self.cre
+00034e00: 6174 6553 6f75 7263 654d 6574 6128 290a  ateSourceMeta().
+00034e10: 0a20 2020 2064 6566 206c 6f61 6444 6174  .    def loadDat
+00034e20: 6128 7365 6c66 293a 0a20 2020 2020 2020  a(self):.       
+00034e30: 2073 656c 662e 6461 7461 203d 2070 642e   self.data = pd.
+00034e40: 7265 6164 5f63 7376 2873 656c 662e 7365  read_csv(self.se
+00034e50: 7475 702e 4441 5441 5f46 494c 452c 2069  tup.DATA_FILE, i
+00034e60: 6e64 6578 5f63 6f6c 3d4e 6f6e 652c 2068  ndex_col=None, h
+00034e70: 6561 6465 723d 3029 0a20 2020 2020 2020  eader=0).       
+00034e80: 2073 656c 662e 6461 7461 2e6c 6f63 5b3a   self.data.loc[:
+00034e90: 2c20 276f 6c64 5f76 6172 275d 203d 2073  , 'old_var'] = s
+00034ea0: 656c 662e 6461 7461 2e6c 6f63 5b3a 2c20  elf.data.loc[:, 
+00034eb0: 5b27 7365 6374 6f72 272c 2027 696e 6469  ['sector', 'indi
+00034ec0: 6361 746f 7227 5d5d 2e61 7070 6c79 280a  cator']].apply(.
+00034ed0: 2020 2020 2020 2020 2020 2020 6c61 6d62              lamb
+00034ee0: 6461 2078 3a20 275f 272e 6a6f 696e 286d  da x: '_'.join(m
+00034ef0: 6170 2873 7472 2c20 7829 292c 2061 7869  ap(str, x)), axi
+00034f00: 733d 310a 2020 2020 2020 2020 290a 2020  s=1.        ).  
+00034f10: 2020 2020 2020 7365 6c66 2e64 6174 612e        self.data.
+00034f20: 6c6f 635b 3a2c 2027 7363 656e 6172 696f  loc[:, 'scenario
+00034f30: 275d 203d 2073 656c 662e 6461 7461 2e6c  '] = self.data.l
+00034f40: 6f63 5b3a 2c20 2776 6172 6961 626c 6527  oc[:, 'variable'
+00034f50: 5d0a 2020 2020 2020 2020 7365 6c66 2e64  ].        self.d
+00034f60: 6174 612e 6c6f 635b 3a2c 2027 7265 6769  ata.loc[:, 'regi
+00034f70: 6f6e 275d 203d 2073 656c 662e 6461 7461  on'] = self.data
+00034f80: 2e6c 6f63 5b3a 2c20 2763 6f75 6e74 7279  .loc[:, 'country
+00034f90: 275d 0a20 2020 2020 2020 2073 656c 662e  '].        self.
+00034fa0: 6461 7461 2e6c 6f63 5b3a 2c20 276d 6f64  data.loc[:, 'mod
+00034fb0: 656c 275d 203d 2027 270a 2020 2020 2020  el'] = ''.      
+00034fc0: 2020 7365 6c66 2e64 6174 612e 6c6f 635b    self.data.loc[
+00034fd0: 3a2c 2027 7661 7269 6162 6c65 275d 203d  :, 'variable'] =
+00034fe0: 2073 656c 662e 6461 7461 2e6c 6f63 5b3a   self.data.loc[:
+00034ff0: 2c20 276f 6c64 5f76 6172 275d 0a0a 2020  , 'old_var']..  
+00035000: 2020 6465 6620 6372 6561 7465 5661 7269    def createVari
+00035010: 6162 6c65 4d61 7070 696e 6728 7365 6c66  ableMapping(self
+00035020: 293a 0a0a 2020 2020 2020 2020 2320 6c6f  ):..        # lo
+00035030: 6164 696e 6720 6461 7461 2069 6620 6e65  ading data if ne
+00035040: 6365 7373 6172 790a 2020 2020 2020 2020  cessary.        
+00035050: 6966 206e 6f74 2068 6173 6174 7472 2873  if not hasattr(s
+00035060: 656c 662c 2027 6461 7461 2729 3a0a 2020  elf, 'data'):.  
+00035070: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+00035080: 6f61 6444 6174 6128 290a 0a20 2020 2020  oadData()..     
+00035090: 2020 2069 6d70 6f72 7420 6e75 6d70 7920     import numpy 
+000350a0: 6173 206e 700a 0a20 2020 2020 2020 2077  as np..        w
+000350b0: 7269 7465 7220 3d20 7064 2e45 7863 656c  riter = pd.Excel
+000350c0: 5772 6974 6572 280a 2020 2020 2020 2020  Writer(.        
+000350d0: 2020 2020 7365 6c66 2e73 6574 7570 2e4d      self.setup.M
+000350e0: 4150 5049 4e47 5f46 494c 452c 0a20 2020  APPING_FILE,.   
+000350f0: 2020 2020 2020 2020 2065 6e67 696e 653d           engine=
+00035100: 2778 6c73 7877 7269 7465 7227 2c0a 2020  'xlsxwriter',.  
+00035110: 2020 2020 2020 2020 2020 6461 7465 7469            dateti
+00035120: 6d65 5f66 6f72 6d61 743d 276d 6d6d 2064  me_format='mmm d
+00035130: 2079 7979 7920 6868 3a6d 6d3a 7373 272c   yyyy hh:mm:ss',
+00035140: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00035150: 655f 666f 726d 6174 3d27 6d6d 6d6d 2064  e_format='mmmm d
+00035160: 6420 7979 7979 272c 0a20 2020 2020 2020  d yyyy',.       
+00035170: 2029 0a0a 2020 2020 2020 2020 2320 7661   )..        # va
+00035180: 7269 6162 6c65 730a 2020 2020 2020 2020  riables.        
+00035190: 2320 696e 6465 7820 3d20 7365 6c66 2e64  # index = self.d
+000351a0: 6174 615b 7365 6c66 2e73 6574 7570 2e56  ata[self.setup.V
+000351b0: 4152 4941 424c 455f 434f 4c55 4d4e 5f4e  ARIABLE_COLUMN_N
+000351c0: 414d 455d 2e75 6e69 7175 6528 290a 2020  AME].unique().  
+000351d0: 2020 2020 2020 7365 6c66 2e61 7661 696c        self.avail
+000351e0: 6162 6c65 5365 7269 6573 203d 2073 656c  ableSeries = sel
+000351f0: 662e 6461 7461 2e64 726f 705f 6475 706c  f.data.drop_dupl
+00035200: 6963 6174 6573 280a 2020 2020 2020 2020  icates(.        
+00035210: 2020 2020 7365 6c66 2e73 6574 7570 2e56      self.setup.V
+00035220: 4152 4941 424c 455f 434f 4c55 4d4e 5f4e  ARIABLE_COLUMN_N
+00035230: 414d 450a 2020 2020 2020 2020 292e 7365  AME.        ).se
+00035240: 745f 696e 6465 7828 7365 6c66 2e73 6574  t_index(self.set
+00035250: 7570 2e56 4152 4941 424c 455f 434f 4c55  up.VARIABLE_COLU
+00035260: 4d4e 5f4e 414d 4529 5b27 756e 6974 275d  MN_NAME)['unit']
+00035270: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
+00035280: 7070 696e 6720 3d20 7064 2e44 6174 6146  pping = pd.DataF
+00035290: 7261 6d65 280a 2020 2020 2020 2020 2020  rame(.          
+000352a0: 2020 696e 6465 783d 7365 6c66 2e61 7661    index=self.ava
+000352b0: 696c 6162 6c65 5365 7269 6573 2e69 6e64  ilableSeries.ind
+000352c0: 6578 2c20 636f 6c75 6d6e 733d 5b27 656e  ex, columns=['en
+000352d0: 6974 7479 272c 2027 6361 7465 676f 7279  itty', 'category
+000352e0: 275d 0a20 2020 2020 2020 2029 0a20 2020  '].        ).   
+000352f0: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
+00035300: 6720 3d20 7064 2e63 6f6e 6361 7428 5b73  g = pd.concat([s
+00035310: 656c 662e 6d61 7070 696e 672c 2073 656c  elf.mapping, sel
+00035320: 662e 6176 6169 6c61 626c 6553 6572 6965  f.availableSerie
+00035330: 735d 2c20 6178 6973 3d31 290a 2020 2020  s], axis=1).    
+00035340: 2020 2020 7365 6c66 2e6d 6170 7069 6e67      self.mapping
+00035350: 203d 2073 656c 662e 6d61 7070 696e 672e   = self.mapping.
+00035360: 736f 7274 5f69 6e64 6578 2829 0a20 2020  sort_index().   
+00035370: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
+00035380: 672e 746f 5f65 7863 656c 2877 7269 7465  g.to_excel(write
+00035390: 722c 2065 6e67 696e 653d 276f 7065 6e70  r, engine='openp
+000353a0: 7978 6c27 2c20 7368 6565 745f 6e61 6d65  yxl', sheet_name
+000353b0: 3d56 4152 5f4d 4150 5049 4e47 5f53 4845  =VAR_MAPPING_SHE
+000353c0: 4554 290a 0a20 2020 2020 2020 2023 206d  ET)..        # m
+000353d0: 6f64 656c 730a 2020 2020 2020 2020 2320  odels.        # 
+000353e0: 2020 2020 2020 2069 6e64 6578 203d 206e         index = n
+000353f0: 702e 756e 6971 7565 2873 656c 662e 6461  p.unique(self.da
+00035400: 7461 5b73 656c 662e 7365 7475 702e 4d4f  ta[self.setup.MO
+00035410: 4445 4c5f 434f 4c55 4d4e 5f4e 414d 455d  DEL_COLUMN_NAME]
+00035420: 2e76 616c 7565 7329 0a0a 2020 2020 2020  .values)..      
+00035430: 2020 2320 2020 2020 2020 2073 656c 662e    #        self.
+00035440: 6176 6169 6c61 626c 6553 6572 6965 7320  availableSeries 
+00035450: 3d20 7064 2e44 6174 6146 7261 6d65 2869  = pd.DataFrame(i
+00035460: 6e64 6578 3d69 6e64 6578 290a 2020 2020  ndex=index).    
+00035470: 2020 2020 2320 2020 2020 2020 2073 656c      #        sel
+00035480: 662e 6d61 7070 696e 6720 3d20 7064 2e44  f.mapping = pd.D
+00035490: 6174 6146 7261 6d65 2869 6e64 6578 3d69  ataFrame(index=i
+000354a0: 6e64 6578 2c20 636f 6c75 6d6e 7320 3d20  ndex, columns = 
+000354b0: 5b73 656c 662e 7365 7475 702e 4d4f 4445  [self.setup.MODE
+000354c0: 4c5f 434f 4c55 4d4e 5f4e 414d 455d 290a  L_COLUMN_NAME]).
 000354d0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
 000354e0: 2073 656c 662e 6d61 7070 696e 6720 3d20   self.mapping = 
-000354f0: 7365 6c66 2e6d 6170 7069 6e67 2e73 6f72  self.mapping.sor
-00035500: 745f 696e 6465 7828 290a 2020 2020 2020  t_index().      
-00035510: 2020 230a 2020 2020 2020 2020 2320 2020    #.        #   
-00035520: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
-00035530: 672e 746f 5f65 7863 656c 2877 7269 7465  g.to_excel(write
-00035540: 722c 2065 6e67 696e 653d 276f 7065 6e70  r, engine='openp
-00035550: 7978 6c27 2c20 7368 6565 745f 6e61 6d65  yxl', sheet_name
-00035560: 3d27 6d6f 6465 6c5f 6d61 7070 696e 6727  ='model_mapping'
-00035570: 290a 0a20 2020 2020 2020 2023 2073 6365  )..        # sce
-00035580: 6e61 7269 6f73 0a20 2020 2020 2020 2069  narios.        i
-00035590: 6e64 6578 203d 206e 702e 756e 6971 7565  ndex = np.unique
-000355a0: 2873 656c 662e 6461 7461 5b73 656c 662e  (self.data[self.
-000355b0: 7365 7475 702e 5343 454e 4152 494f 5f43  setup.SCENARIO_C
-000355c0: 4f4c 554d 4e5f 4e41 4d45 5d2e 7661 6c75  OLUMN_NAME].valu
-000355d0: 6573 290a 0a20 2020 2020 2020 2073 656c  es)..        sel
-000355e0: 662e 6176 6169 6c61 626c 6553 6572 6965  f.availableSerie
-000355f0: 7320 3d20 7064 2e44 6174 6146 7261 6d65  s = pd.DataFrame
-00035600: 2869 6e64 6578 3d69 6e64 6578 290a 2020  (index=index).  
-00035610: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
-00035620: 6e67 203d 2070 642e 4461 7461 4672 616d  ng = pd.DataFram
-00035630: 6528 0a20 2020 2020 2020 2020 2020 2069  e(.            i
-00035640: 6e64 6578 3d69 6e64 6578 2c20 636f 6c75  ndex=index, colu
-00035650: 6d6e 733d 5b73 656c 662e 7365 7475 702e  mns=[self.setup.
-00035660: 5343 454e 4152 494f 5f43 4f4c 554d 4e5f  SCENARIO_COLUMN_
-00035670: 4e41 4d45 5d0a 2020 2020 2020 2020 290a  NAME].        ).
-00035680: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
-00035690: 7069 6e67 203d 2070 642e 636f 6e63 6174  ping = pd.concat
-000356a0: 285b 7365 6c66 2e6d 6170 7069 6e67 2c20  ([self.mapping, 
-000356b0: 7365 6c66 2e61 7661 696c 6162 6c65 5365  self.availableSe
-000356c0: 7269 6573 5d2c 2061 7869 733d 3129 0a20  ries], axis=1). 
-000356d0: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
-000356e0: 696e 6720 3d20 7365 6c66 2e6d 6170 7069  ing = self.mappi
-000356f0: 6e67 2e73 6f72 745f 696e 6465 7828 290a  ng.sort_index().
-00035700: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
-00035710: 7069 6e67 2e74 6f5f 6578 6365 6c28 7772  ping.to_excel(wr
-00035720: 6974 6572 2c20 656e 6769 6e65 3d27 6f70  iter, engine='op
-00035730: 656e 7079 786c 272c 2073 6865 6574 5f6e  enpyxl', sheet_n
-00035740: 616d 653d 2773 6365 6e61 7269 6f5f 6d61  ame='scenario_ma
-00035750: 7070 696e 6727 290a 0a20 2020 2020 2020  pping')..       
-00035760: 2023 2072 6567 696f 6e0a 2020 2020 2020   # region.      
-00035770: 2020 696e 6465 7820 3d20 6e70 2e75 6e69    index = np.uni
-00035780: 7175 6528 7365 6c66 2e64 6174 615b 7365  que(self.data[se
-00035790: 6c66 2e73 6574 7570 2e52 4547 494f 4e5f  lf.setup.REGION_
-000357a0: 434f 4c55 4d4e 5f4e 414d 455d 2e76 616c  COLUMN_NAME].val
-000357b0: 7565 7329 0a0a 2020 2020 2020 2020 7365  ues)..        se
-000357c0: 6c66 2e61 7661 696c 6162 6c65 5365 7269  lf.availableSeri
-000357d0: 6573 203d 2070 642e 4461 7461 4672 616d  es = pd.DataFram
-000357e0: 6528 696e 6465 783d 696e 6465 7829 0a20  e(index=index). 
-000357f0: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
-00035800: 696e 6720 3d20 7064 2e44 6174 6146 7261  ing = pd.DataFra
-00035810: 6d65 280a 2020 2020 2020 2020 2020 2020  me(.            
-00035820: 696e 6465 783d 696e 6465 782c 2063 6f6c  index=index, col
-00035830: 756d 6e73 3d5b 7365 6c66 2e73 6574 7570  umns=[self.setup
-00035840: 2e52 4547 494f 4e5f 434f 4c55 4d4e 5f4e  .REGION_COLUMN_N
-00035850: 414d 455d 0a20 2020 2020 2020 2029 0a20  AME].        ). 
-00035860: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
-00035870: 696e 6720 3d20 7064 2e63 6f6e 6361 7428  ing = pd.concat(
-00035880: 5b73 656c 662e 6d61 7070 696e 672c 2073  [self.mapping, s
-00035890: 656c 662e 6176 6169 6c61 626c 6553 6572  elf.availableSer
-000358a0: 6965 735d 2c20 6178 6973 3d31 290a 2020  ies], axis=1).  
-000358b0: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
-000358c0: 6e67 203d 2073 656c 662e 6d61 7070 696e  ng = self.mappin
-000358d0: 672e 736f 7274 5f69 6e64 6578 2829 0a0a  g.sort_index()..
-000358e0: 2020 2020 2020 2020 666f 7220 6964 7820          for idx 
-000358f0: 696e 2073 656c 662e 6d61 7070 696e 672e  in self.mapping.
-00035900: 696e 6465 783a 0a20 2020 2020 2020 2020  index:.         
-00035910: 2020 2069 736f 203d 2064 742e 7574 696c     iso = dt.util
-00035920: 2e69 6465 6e74 6966 7943 6f75 6e74 7279  .identifyCountry
-00035930: 2869 6478 290a 2020 2020 2020 2020 2020  (idx).          
-00035940: 2020 6966 2069 736f 2069 7320 6e6f 7420    if iso is not 
-00035950: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00035960: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
-00035970: 6e67 2e6c 6f63 5b69 6478 2c20 2772 6567  ng.loc[idx, 'reg
-00035980: 696f 6e27 5d20 3d20 6973 6f0a 0a20 2020  ion'] = iso..   
-00035990: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
-000359a0: 672e 746f 5f65 7863 656c 2877 7269 7465  g.to_excel(write
-000359b0: 722c 2065 6e67 696e 653d 276f 7065 6e70  r, engine='openp
-000359c0: 7978 6c27 2c20 7368 6565 745f 6e61 6d65  yxl', sheet_name
-000359d0: 3d27 7265 6769 6f6e 5f6d 6170 7069 6e67  ='region_mapping
-000359e0: 2729 0a20 2020 2020 2020 2077 7269 7465  ').        write
-000359f0: 722e 636c 6f73 6528 290a 0a20 2020 2064  r.close()..    d
-00035a00: 6566 2067 6174 6865 724d 6170 7065 6444  ef gatherMappedD
-00035a10: 6174 6128 7365 6c66 2c20 7370 6174 6961  ata(self, spatia
-00035a20: 6c53 7562 5365 743d 4e6f 6e65 2c20 7570  lSubSet=None, up
-00035a30: 6461 7465 5461 626c 6573 3d46 616c 7365  dateTables=False
-00035a40: 293a 0a0a 2020 2020 2020 2020 696d 706f  ):..        impo
-00035a50: 7274 2074 7164 6d0a 0a20 2020 2020 2020  rt tqdm..       
-00035a60: 2023 206c 6f61 6469 6e67 2064 6174 6120   # loading data 
-00035a70: 6966 206e 6563 6573 7361 7279 0a20 2020  if necessary.   
-00035a80: 2020 2020 2069 6620 6e6f 7420 6861 7361       if not hasa
-00035a90: 7474 7228 7365 6c66 2c20 2764 6174 6127  ttr(self, 'data'
-00035aa0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00035ab0: 656c 662e 6c6f 6164 4461 7461 2829 0a0a  elf.loadData()..
-00035ac0: 2020 2020 2020 2020 7461 626c 6573 546f          tablesTo
-00035ad0: 436f 6d6d 6974 203d 205b 5d0a 2020 2020  Commit = [].    
-00035ae0: 2020 2020 6d65 7461 4469 6374 203d 2064      metaDict = d
-00035af0: 6963 7428 290a 2020 2020 2020 2020 6d65  ict().        me
-00035b00: 7461 4469 6374 5b27 736f 7572 6365 275d  taDict['source']
-00035b10: 203d 2073 656c 662e 7365 7475 702e 534f   = self.setup.SO
-00035b20: 5552 4345 5f49 440a 2020 2020 2020 2020  URCE_ID.        
-00035b30: 6578 636c 7564 6564 5461 626c 6573 203d  excludedTables =
-00035b40: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00035b50: 6578 636c 7564 6564 5461 626c 6573 5b27  excludedTables['
-00035b60: 656d 7074 7927 5d20 3d20 6c69 7374 2829  empty'] = list()
-00035b70: 0a20 2020 2020 2020 2065 7863 6c75 6465  .        exclude
-00035b80: 6454 6162 6c65 735b 2765 7272 6f72 275d  dTables['error']
-00035b90: 203d 206c 6973 7428 290a 2020 2020 2020   = list().      
-00035ba0: 2020 6578 636c 7564 6564 5461 626c 6573    excludedTables
-00035bb0: 5b27 6578 6973 7473 275d 203d 206c 6973  ['exists'] = lis
-00035bc0: 7428 290a 0a20 2020 2020 2020 2023 2020  t()..        #  
-00035bd0: 2020 2020 2020 7365 6c66 2e64 6174 6120        self.data 
-00035be0: 3d20 7365 6c66 2e64 6174 610a 0a20 2020  = self.data..   
-00035bf0: 2020 2020 2066 6f72 2073 6365 6e61 7269       for scenari
-00035c00: 6f20 696e 2073 656c 662e 6d61 7070 696e  o in self.mappin
-00035c10: 675b 2773 6365 6e61 7269 6f27 5d2e 6b65  g['scenario'].ke
-00035c20: 7973 2829 3a0a 2020 2020 2020 2020 2020  ys():.          
-00035c30: 2020 7465 6d70 4d6f 5363 203d 2073 656c    tempMoSc = sel
-00035c40: 662e 6461 7461 2e6c 6f63 5b73 656c 662e  f.data.loc[self.
-00035c50: 6461 7461 2e73 6365 6e61 7269 6f20 3d3d  data.scenario ==
-00035c60: 2073 6365 6e61 7269 6f5d 0a20 2020 2020   scenario].     
-00035c70: 2020 2020 2020 2066 6f72 2076 6172 6961         for varia
-00035c80: 626c 6520 696e 2073 656c 662e 6d61 7070  ble in self.mapp
-00035c90: 696e 675b 2765 6e74 6974 7927 5d2e 6b65  ing['entity'].ke
-00035ca0: 7973 2829 3a0a 2020 2020 2020 2020 2020  ys():.          
-00035cb0: 2020 2020 2020 7465 6d70 4d6f 5363 5661        tempMoScVa
-00035cc0: 203d 2074 656d 704d 6f53 632e 6c6f 635b   = tempMoSc.loc[
-00035cd0: 7465 6d70 4d6f 5363 2e76 6172 6961 626c  tempMoSc.variabl
-00035ce0: 6520 3d3d 2076 6172 6961 626c 655d 0a20  e == variable]. 
-00035cf0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00035d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035d10: 666f 7220 6361 7465 676f 7279 2069 6e20  for category in 
-00035d20: 7365 6c66 2e6d 6170 7069 6e67 5b27 6361  self.mapping['ca
-00035d30: 7465 676f 7279 275d 2e6b 6579 7328 293a  tegory'].keys():
-00035d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00035d50: 2023 2020 2020 2020 2020 2020 2020 2020   #              
-00035d60: 2020 7465 6d70 4d6f 5363 5661 203d 2074    tempMoScVa = t
-00035d70: 656d 704d 6f53 6356 612e 6c6f 635b 7465  empMoScVa.loc[te
-00035d80: 6d70 4d6f 5363 5661 2e76 6172 6961 626c  mpMoScVa.variabl
-00035d90: 6520 3d3d 2063 6174 6567 6f72 795d 0a20  e == category]. 
-00035da0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00035db0: 656d 704d 6f53 6356 6120 3d20 7465 6d70  empMoScVa = temp
-00035dc0: 4d6f 5363 5661 2e6c 6f63 5b0a 2020 2020  MoScVa.loc[.    
-00035dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035de0: 3a2c 0a20 2020 2020 2020 2020 2020 2020  :,.             
-00035df0: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-00035e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035e10: 2027 756e 6974 272c 0a20 2020 2020 2020   'unit',.       
-00035e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035e30: 2027 6d6f 6465 6c27 2c0a 2020 2020 2020   'model',.      
-00035e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035e50: 2020 2773 6365 6e61 7269 6f27 2c0a 2020    'scenario',.  
-00035e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035e70: 2020 2020 2020 2779 6561 7227 2c0a 2020        'year',.  
-00035e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035e90: 2020 2020 2020 2772 6567 696f 6e27 2c0a        'region',.
-00035ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035eb0: 2020 2020 2020 2020 2776 616c 7565 272c          'value',
-00035ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00035ed0: 2020 2020 2020 2020 2027 7661 7269 6162           'variab
-00035ee0: 6c65 272c 0a20 2020 2020 2020 2020 2020  le',.           
-00035ef0: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
-00035f00: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
-00035f10: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00035f20: 6d70 4d6f 5363 5661 2e6c 6f63 5b3a 2c20  mpMoScVa.loc[:, 
-00035f30: 2775 6e69 7427 5d20 3d20 7365 6c66 2e6d  'unit'] = self.m
-00035f40: 6170 7069 6e67 5b27 756e 6974 275d 5b76  apping['unit'][v
-00035f50: 6172 6961 626c 655d 0a20 2020 2020 2020  ariable].       
-00035f60: 2020 2020 2020 2020 2074 656d 704d 6f53           tempMoS
-00035f70: 6356 612e 6c6f 635b 3a2c 2027 7363 656e  cVa.loc[:, 'scen
-00035f80: 6172 696f 275d 203d 2073 656c 662e 6d61  ario'] = self.ma
-00035f90: 7070 696e 675b 2773 6365 6e61 7269 6f27  pping['scenario'
-00035fa0: 5d5b 7363 656e 6172 696f 5d0a 2020 2020  ][scenario].    
-00035fb0: 2020 2020 2020 2020 2020 2020 2323 2020              ##  
-00035fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035fd0: 2020 6466 670a 2020 2020 2020 2020 2020    dfg.          
-00035fe0: 2020 2020 2020 7461 626c 6573 203d 2064        tables = d
-00035ff0: 742e 696e 7465 7266 6163 6573 2e72 6561  t.interfaces.rea
-00036000: 645f 6c6f 6e67 5f74 6162 6c65 2874 656d  d_long_table(tem
-00036010: 704d 6f53 6356 612c 205b 7661 7269 6162  pMoScVa, [variab
-00036020: 6c65 5d29 0a20 2020 2020 2020 2020 2020  le]).           
-00036030: 2020 2020 2066 6f72 2074 6162 6c65 2069       for table i
-00036040: 6e20 7461 626c 6573 3a0a 2020 2020 2020  n tables:.      
-00036050: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-00036060: 626c 652e 6d65 7461 5b27 656e 7469 7479  ble.meta['entity
-00036070: 275d 203d 2073 656c 662e 6d61 7070 696e  '] = self.mappin
-00036080: 675b 2765 6e74 6974 7927 5d5b 7661 7269  g['entity'][vari
-00036090: 6162 6c65 5d0a 2020 2020 2020 2020 2020  able].          
-000360a0: 2020 2020 2020 2020 2020 7461 626c 652e            table.
-000360b0: 6d65 7461 5b27 6361 7465 676f 7279 275d  meta['category']
-000360c0: 203d 2073 656c 662e 6d61 7070 696e 675b   = self.mapping[
-000360d0: 2763 6174 6567 6f72 7927 5d5b 7661 7269  'category'][vari
-000360e0: 6162 6c65 5d0a 2020 2020 2020 2020 2020  able].          
-000360f0: 2020 2020 2020 2020 2020 7461 626c 652e            table.
-00036100: 6d65 7461 5b27 7363 656e 6172 696f 275d  meta['scenario']
-00036110: 203d 2073 656c 662e 6d61 7070 696e 675b   = self.mapping[
-00036120: 2773 6365 6e61 7269 6f27 5d5b 7363 656e  'scenario'][scen
-00036130: 6172 696f 5d0a 2020 2020 2020 2020 2020  ario].          
-00036140: 2020 2020 2020 2020 2020 7461 626c 652e            table.
-00036150: 6d65 7461 5b27 736f 7572 6365 275d 203d  meta['source'] =
-00036160: 2073 656c 662e 7365 7475 702e 534f 5552   self.setup.SOUR
-00036170: 4345 5f49 440a 2020 2020 2020 2020 2020  CE_ID.          
-00036180: 2020 2020 2020 2020 2020 7461 626c 652e            table.
-00036190: 696e 6465 7820 3d20 7461 626c 652e 696e  index = table.in
-000361a0: 6465 782e 6d61 7028 7365 6c66 2e6d 6170  dex.map(self.map
-000361b0: 7069 6e67 5b27 7265 6769 6f6e 275d 290a  ping['region']).
-000361c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000361d0: 2020 2020 2074 6162 6c65 4944 203d 2074       tableID = t
-000361e0: 6162 6c65 2e67 656e 6572 6174 6554 6162  able.generateTab
-000361f0: 6c65 4944 2829 0a20 2020 2020 2020 2020  leID().         
-00036200: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00036210: 7420 7570 6461 7465 5461 626c 6573 3a0a  t updateTables:.
-00036220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00036230: 2020 2020 2020 2020 6966 2064 742e 636f          if dt.co
-00036240: 7265 2e44 422e 7461 626c 6545 7869 7374  re.DB.tableExist
-00036250: 2874 6162 6c65 4944 293a 0a20 2020 2020  (tableID):.     
-00036260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00036270: 2020 2020 2020 2065 7863 6c75 6465 6454         excludedT
-00036280: 6162 6c65 735b 2765 7869 7374 7327 5d2e  ables['exists'].
-00036290: 6170 7065 6e64 2874 6162 6c65 4944 290a  append(tableID).
-000362a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000362b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000362c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000362d0: 2020 2020 2020 2020 2020 7461 626c 6573            tables
-000362e0: 546f 436f 6d6d 6974 2e61 7070 656e 6428  ToCommit.append(
-000362f0: 7461 626c 6529 0a20 2020 2020 2020 2072  table).        r
-00036300: 6574 7572 6e20 7461 626c 6573 546f 436f  eturn tablesToCo
-00036310: 6d6d 6974 2c20 6578 636c 7564 6564 5461  mmit, excludedTa
-00036320: 626c 6573 0a0a 0a23 2525 2049 6d70 6f72  bles...#%% Impor
-00036330: 7420 6675 6e63 7469 6f6e 730a 0a0a 6465  t functions...de
-00036340: 6620 4844 495f 696d 706f 7274 2879 6561  f HDI_import(yea
-00036350: 723d 3230 3230 293a 0a20 2020 2073 6f75  r=2020):.    sou
-00036360: 7263 654d 6574 6120 3d20 7b0a 2020 2020  rceMeta = {.    
-00036370: 2020 2020 2753 4f55 5243 455f 4944 273a      'SOURCE_ID':
-00036380: 2027 4844 495f 2720 2b20 7374 7228 7965   'HDI_' + str(ye
-00036390: 6172 292c 0a20 2020 2020 2020 2027 636f  ar),.        'co
-000363a0: 6c6c 6563 7465 645f 6279 273a 2027 4147  llected_by': 'AG
-000363b0: 272c 0a20 2020 2020 2020 2027 6461 7465  ',.        'date
-000363c0: 273a 2064 742e 636f 7265 2e67 6574 5f64  ': dt.core.get_d
-000363d0: 6174 655f 7374 7269 6e67 2829 2c0a 2020  ate_string(),.  
-000363e0: 2020 2020 2020 2773 6f75 7263 655f 7572        'source_ur
-000363f0: 6c27 3a20 2768 7474 703a 2f2f 6864 722e  l': 'http://hdr.
-00036400: 756e 6470 2e6f 7267 2f65 6e2f 6461 7461  undp.org/en/data
-00036410: 272c 0a20 2020 2020 2020 2027 6c69 6365  ',.        'lice
-00036420: 6e63 6527 3a20 276f 7065 6e20 736f 7572  nce': 'open sour
-00036430: 6365 272c 0a20 2020 207d 0a0a 2020 2020  ce',.    }..    
-00036440: 534f 5552 4345 5f50 4154 4820 3d20 6f73  SOURCE_PATH = os
-00036450: 2e70 6174 682e 6a6f 696e 280a 2020 2020  .path.join(.    
-00036460: 2020 2020 6474 2e63 6f6e 6669 672e 5041      dt.config.PA
-00036470: 5448 5f54 4f5f 4441 5441 5348 454c 462c  TH_TO_DATASHELF,
-00036480: 2027 7261 7764 6174 6127 2c20 736f 7572   'rawdata', sour
-00036490: 6365 4d65 7461 5b27 534f 5552 4345 5f49  ceMeta['SOURCE_I
-000364a0: 4427 5d0a 2020 2020 290a 2020 2020 6461  D'].    ).    da
-000364b0: 7461 203d 2070 642e 7265 6164 5f63 7376  ta = pd.read_csv
-000364c0: 280a 2020 2020 2020 2020 6f73 2e70 6174  (.        os.pat
-000364d0: 682e 6a6f 696e 2853 4f55 5243 455f 5041  h.join(SOURCE_PA
-000364e0: 5448 2c20 2248 756d 616e 2044 6576 656c  TH, "Human Devel
-000364f0: 6f70 6d65 6e74 2049 6e64 6578 2028 4844  opment Index (HD
-00036500: 4929 2e63 7376 2229 2c0a 2020 2020 2020  I).csv"),.      
-00036510: 2020 6e61 5f76 616c 7565 733d 272e 2e27    na_values='..'
-00036520: 2c0a 2020 2020 290a 0a20 2020 2079 6561  ,.    )..    yea
-00036530: 7243 6f6c 756d 6e73 203d 2064 742e 7574  rColumns = dt.ut
-00036540: 696c 2e79 6561 7273 436f 6c75 6d6e 734f  il.yearsColumnsO
-00036550: 6e6c 7928 6461 7461 290a 0a20 2020 2064  nly(data)..    d
-00036560: 6174 6120 3d20 6461 7461 2e6c 6f63 5b3a  ata = data.loc[:
-00036570: 2c20 5b27 436f 756e 7472 7927 5d20 2b20  , ['Country'] + 
-00036580: 7965 6172 436f 6c75 6d6e 735d 0a0a 2020  yearColumns]..  
-00036590: 2020 2320 2020 2072 6567 696f 6e4d 6170    #    regionMap
-000365a0: 7069 6e67 203d 207b 783a 7920 666f 7220  ping = {x:y for 
-000365b0: 782c 7920 696e 207a 6970 286c 6973 7428  x,y in zip(list(
-000365c0: 6461 7461 2e6c 6f63 5b3a 2c27 436f 756e  data.loc[:,'Coun
-000365d0: 7472 7927 5d29 2c20 6c69 7374 2864 6174  try']), list(dat
-000365e0: 612e 6c6f 635b 3a2c 2743 6f75 6e74 7279  a.loc[:,'Country
-000365f0: 275d 2e6d 6170 286c 616d 6264 6120 7820  '].map(lambda x 
-00036600: 3a20 6474 2e67 6574 436f 756e 7472 7949  : dt.getCountryI
-00036610: 534f 2873 7472 2878 2929 2929 297d 0a20  SO(str(x)))))}. 
-00036620: 2020 2072 6567 696f 6e4d 6170 7069 6e67     regionMapping
-00036630: 203d 207b 0a20 2020 2020 2020 2027 2041   = {.        ' A
-00036640: 6667 6861 6e69 7374 616e 273a 2027 4146  fghanistan': 'AF
-00036650: 4727 2c0a 2020 2020 2020 2020 2720 416c  G',.        ' Al
-00036660: 6261 6e69 6127 3a20 2741 4c42 272c 0a20  bania': 'ALB',. 
-00036670: 2020 2020 2020 2027 2041 6c67 6572 6961         ' Algeria
-00036680: 273a 2027 445a 4127 2c0a 2020 2020 2020  ': 'DZA',.      
-00036690: 2020 2720 416e 646f 7272 6127 3a20 2741    ' Andorra': 'A
-000366a0: 4e44 272c 0a20 2020 2020 2020 2027 2041  ND',.        ' A
-000366b0: 6e67 6f6c 6127 3a20 2741 474f 272c 0a20  ngola': 'AGO',. 
-000366c0: 2020 2020 2020 2027 2041 6e74 6967 7561         ' Antigua
-000366d0: 2061 6e64 2042 6172 6275 6461 273a 2027   and Barbuda': '
-000366e0: 4154 4727 2c0a 2020 2020 2020 2020 2720  ATG',.        ' 
-000366f0: 4172 6765 6e74 696e 6127 3a20 2741 5247  Argentina': 'ARG
-00036700: 272c 0a20 2020 2020 2020 2027 2041 726d  ',.        ' Arm
-00036710: 656e 6961 273a 2027 4152 4d27 2c0a 2020  enia': 'ARM',.  
-00036720: 2020 2020 2020 2720 4175 7374 7261 6c69        ' Australi
-00036730: 6127 3a20 2741 5553 272c 0a20 2020 2020  a': 'AUS',.     
-00036740: 2020 2027 2041 7573 7472 6961 273a 2027     ' Austria': '
-00036750: 4155 5427 2c0a 2020 2020 2020 2020 2720  AUT',.        ' 
-00036760: 417a 6572 6261 696a 616e 273a 2027 415a  Azerbaijan': 'AZ
-00036770: 4527 2c0a 2020 2020 2020 2020 2720 4261  E',.        ' Ba
-00036780: 6861 6d61 7327 3a20 2742 4853 272c 0a20  hamas': 'BHS',. 
-00036790: 2020 2020 2020 2027 2042 6168 7261 696e         ' Bahrain
-000367a0: 273a 2027 4248 5227 2c0a 2020 2020 2020  ': 'BHR',.      
-000367b0: 2020 2720 4261 6e67 6c61 6465 7368 273a    ' Bangladesh':
-000367c0: 2027 4247 4427 2c0a 2020 2020 2020 2020   'BGD',.        
-000367d0: 2720 4261 7262 6164 6f73 273a 2027 4252  ' Barbados': 'BR
-000367e0: 4227 2c0a 2020 2020 2020 2020 2720 4265  B',.        ' Be
-000367f0: 6c61 7275 7327 3a20 2742 4c52 272c 0a20  larus': 'BLR',. 
-00036800: 2020 2020 2020 2027 2042 656c 6769 756d         ' Belgium
-00036810: 273a 2027 4245 4c27 2c0a 2020 2020 2020  ': 'BEL',.      
-00036820: 2020 2720 4265 6c69 7a65 273a 2027 424c    ' Belize': 'BL
-00036830: 5a27 2c0a 2020 2020 2020 2020 2720 4265  Z',.        ' Be
-00036840: 6e69 6e27 3a20 2742 454e 272c 0a20 2020  nin': 'BEN',.   
-00036850: 2020 2020 2027 2042 6875 7461 6e27 3a20       ' Bhutan': 
-00036860: 2742 544e 272c 0a20 2020 2020 2020 2027  'BTN',.        '
-00036870: 2042 6f6c 6976 6961 2028 506c 7572 696e   Bolivia (Plurin
-00036880: 6174 696f 6e61 6c20 5374 6174 6520 6f66  ational State of
-00036890: 2927 3a20 2742 4f4c 272c 0a20 2020 2020  )': 'BOL',.     
-000368a0: 2020 2027 2042 6f73 6e69 6120 616e 6420     ' Bosnia and 
-000368b0: 4865 727a 6567 6f76 696e 6127 3a20 2742  Herzegovina': 'B
-000368c0: 4948 272c 0a20 2020 2020 2020 2027 2042  IH',.        ' B
-000368d0: 6f74 7377 616e 6127 3a20 2742 5741 272c  otswana': 'BWA',
-000368e0: 0a20 2020 2020 2020 2027 2042 7261 7a69  .        ' Brazi
-000368f0: 6c27 3a20 2742 5241 272c 0a20 2020 2020  l': 'BRA',.     
-00036900: 2020 2027 2042 7275 6e65 6920 4461 7275     ' Brunei Daru
-00036910: 7373 616c 616d 273a 2027 4252 4e27 2c0a  ssalam': 'BRN',.
-00036920: 2020 2020 2020 2020 2720 4275 6c67 6172          ' Bulgar
-00036930: 6961 273a 2027 4247 5227 2c0a 2020 2020  ia': 'BGR',.    
-00036940: 2020 2020 2720 4275 726b 696e 6120 4661      ' Burkina Fa
-00036950: 736f 273a 2027 4246 4127 2c0a 2020 2020  so': 'BFA',.    
-00036960: 2020 2020 2720 4275 7275 6e64 6927 3a20      ' Burundi': 
-00036970: 2742 4449 272c 0a20 2020 2020 2020 2027  'BDI',.        '
-00036980: 2043 6162 6f20 5665 7264 6527 3a20 2743   Cabo Verde': 'C
-00036990: 5056 272c 0a20 2020 2020 2020 2027 2043  PV',.        ' C
-000369a0: 616d 626f 6469 6127 3a20 274b 484d 272c  ambodia': 'KHM',
-000369b0: 0a20 2020 2020 2020 2027 2043 616d 6572  .        ' Camer
-000369c0: 6f6f 6e27 3a20 2743 4d52 272c 0a20 2020  oon': 'CMR',.   
-000369d0: 2020 2020 2027 2043 616e 6164 6127 3a20       ' Canada': 
-000369e0: 2743 414e 272c 0a20 2020 2020 2020 2027  'CAN',.        '
-000369f0: 2043 656e 7472 616c 2041 6672 6963 616e   Central African
-00036a00: 2052 6570 7562 6c69 6327 3a20 2743 4146   Republic': 'CAF
-00036a10: 272c 0a20 2020 2020 2020 2027 2043 6861  ',.        ' Cha
-00036a20: 6427 3a20 2754 4344 272c 0a20 2020 2020  d': 'TCD',.     
-00036a30: 2020 2027 2043 6869 6c65 273a 2027 4348     ' Chile': 'CH
-00036a40: 4c27 2c0a 2020 2020 2020 2020 2720 4368  L',.        ' Ch
-00036a50: 696e 6127 3a20 2743 484e 272c 0a20 2020  ina': 'CHN',.   
-00036a60: 2020 2020 2027 2043 6f6c 6f6d 6269 6127       ' Colombia'
-00036a70: 3a20 2743 4f4c 272c 0a20 2020 2020 2020  : 'COL',.       
-00036a80: 2027 2043 6f6d 6f72 6f73 273a 2027 434f   ' Comoros': 'CO
-00036a90: 4d27 2c0a 2020 2020 2020 2020 2720 436f  M',.        ' Co
-00036aa0: 6e67 6f27 3a20 2743 4f47 272c 0a20 2020  ngo': 'COG',.   
-00036ab0: 2020 2020 2027 2043 6f6e 676f 2028 4465       ' Congo (De
-00036ac0: 6d6f 6372 6174 6963 2052 6570 7562 6c69  mocratic Republi
-00036ad0: 6320 6f66 2074 6865 2927 3a20 2743 4f44  c of the)': 'COD
-00036ae0: 272c 0a20 2020 2020 2020 2027 2043 6f73  ',.        ' Cos
-00036af0: 7461 2052 6963 6127 3a20 2743 5249 272c  ta Rica': 'CRI',
-00036b00: 0a20 2020 2020 2020 2027 2043 726f 6174  .        ' Croat
-00036b10: 6961 273a 2027 4852 5627 2c0a 2020 2020  ia': 'HRV',.    
-00036b20: 2020 2020 2720 4375 6261 273a 2027 4355      ' Cuba': 'CU
-00036b30: 4227 2c0a 2020 2020 2020 2020 2720 4379  B',.        ' Cy
-00036b40: 7072 7573 273a 2027 4359 5027 2c0a 2020  prus': 'CYP',.  
-00036b50: 2020 2020 2020 2720 437a 6563 6869 6127        ' Czechia'
-00036b60: 3a20 2743 5a45 272c 0a20 2020 2020 2020  : 'CZE',.       
-00036b70: 2022 2043 c3b4 7465 2064 2749 766f 6972   " C..te d'Ivoir
-00036b80: 6522 3a20 2743 4956 272c 0a20 2020 2020  e": 'CIV',.     
-00036b90: 2020 2027 2044 656e 6d61 726b 273a 2027     ' Denmark': '
-00036ba0: 444e 4b27 2c0a 2020 2020 2020 2020 2720  DNK',.        ' 
-00036bb0: 446a 6962 6f75 7469 273a 2027 444a 4927  Djibouti': 'DJI'
-00036bc0: 2c0a 2020 2020 2020 2020 2720 446f 6d69  ,.        ' Domi
-00036bd0: 6e69 6361 273a 2027 444d 4127 2c0a 2020  nica': 'DMA',.  
-00036be0: 2020 2020 2020 2720 446f 6d69 6e69 6361        ' Dominica
-00036bf0: 6e20 5265 7075 626c 6963 273a 2027 444f  n Republic': 'DO
-00036c00: 4d27 2c0a 2020 2020 2020 2020 2720 4563  M',.        ' Ec
-00036c10: 7561 646f 7227 3a20 2745 4355 272c 0a20  uador': 'ECU',. 
-00036c20: 2020 2020 2020 2027 2045 6779 7074 273a         ' Egypt':
-00036c30: 2027 4547 5927 2c0a 2020 2020 2020 2020   'EGY',.        
-00036c40: 2720 456c 2053 616c 7661 646f 7227 3a20  ' El Salvador': 
-00036c50: 2753 4c56 272c 0a20 2020 2020 2020 2027  'SLV',.        '
-00036c60: 2045 7175 6174 6f72 6961 6c20 4775 696e   Equatorial Guin
-00036c70: 6561 273a 2027 474e 5127 2c0a 2020 2020  ea': 'GNQ',.    
-00036c80: 2020 2020 2720 4572 6974 7265 6127 3a20      ' Eritrea': 
-00036c90: 2745 5249 272c 0a20 2020 2020 2020 2027  'ERI',.        '
-00036ca0: 2045 7374 6f6e 6961 273a 2027 4553 5427   Estonia': 'EST'
-00036cb0: 2c0a 2020 2020 2020 2020 2720 4573 7761  ,.        ' Eswa
-00036cc0: 7469 6e69 2028 4b69 6e67 646f 6d20 6f66  tini (Kingdom of
-00036cd0: 2927 3a20 2753 575a 272c 0a20 2020 2020  )': 'SWZ',.     
-00036ce0: 2020 2027 2045 7468 696f 7069 6127 3a20     ' Ethiopia': 
-00036cf0: 2745 5448 272c 0a20 2020 2020 2020 2027  'ETH',.        '
-00036d00: 2046 696a 6927 3a20 2746 4a49 272c 0a20   Fiji': 'FJI',. 
-00036d10: 2020 2020 2020 2027 2046 696e 6c61 6e64         ' Finland
-00036d20: 273a 2027 4649 4e27 2c0a 2020 2020 2020  ': 'FIN',.      
-00036d30: 2020 2720 4672 616e 6365 273a 2027 4652    ' France': 'FR
-00036d40: 4127 2c0a 2020 2020 2020 2020 2720 4761  A',.        ' Ga
-00036d50: 626f 6e27 3a20 2747 4142 272c 0a20 2020  bon': 'GAB',.   
-00036d60: 2020 2020 2027 2047 616d 6269 6127 3a20       ' Gambia': 
-00036d70: 2747 4d42 272c 0a20 2020 2020 2020 2027  'GMB',.        '
-00036d80: 2047 656f 7267 6961 273a 2027 4745 4f27   Georgia': 'GEO'
-00036d90: 2c0a 2020 2020 2020 2020 2720 4765 726d  ,.        ' Germ
-00036da0: 616e 7927 3a20 2744 4555 272c 0a20 2020  any': 'DEU',.   
-00036db0: 2020 2020 2027 2047 6861 6e61 273a 2027       ' Ghana': '
-00036dc0: 4748 4127 2c0a 2020 2020 2020 2020 2720  GHA',.        ' 
-00036dd0: 4772 6565 6365 273a 2027 4752 4327 2c0a  Greece': 'GRC',.
-00036de0: 2020 2020 2020 2020 2720 4772 656e 6164          ' Grenad
-00036df0: 6127 3a20 2747 5244 272c 0a20 2020 2020  a': 'GRD',.     
-00036e00: 2020 2027 2047 7561 7465 6d61 6c61 273a     ' Guatemala':
-00036e10: 2027 4754 4d27 2c0a 2020 2020 2020 2020   'GTM',.        
-00036e20: 2720 4775 696e 6561 273a 2027 4749 4e27  ' Guinea': 'GIN'
-00036e30: 2c0a 2020 2020 2020 2020 2720 4775 696e  ,.        ' Guin
-00036e40: 6561 2d42 6973 7361 7527 3a20 2747 4e42  ea-Bissau': 'GNB
-00036e50: 272c 0a20 2020 2020 2020 2027 2047 7579  ',.        ' Guy
-00036e60: 616e 6127 3a20 2747 5559 272c 0a20 2020  ana': 'GUY',.   
-00036e70: 2020 2020 2027 2048 6169 7469 273a 2027       ' Haiti': '
-00036e80: 4854 4927 2c0a 2020 2020 2020 2020 2720  HTI',.        ' 
-00036e90: 486f 6e64 7572 6173 273a 2027 484e 4427  Honduras': 'HND'
-00036ea0: 2c0a 2020 2020 2020 2020 2720 486f 6e67  ,.        ' Hong
-00036eb0: 204b 6f6e 672c 2043 6869 6e61 2028 5341   Kong, China (SA
-00036ec0: 5229 273a 2027 484b 4727 2c0a 2020 2020  R)': 'HKG',.    
-00036ed0: 2020 2020 2720 4875 6e67 6172 7927 3a20      ' Hungary': 
-00036ee0: 2748 554e 272c 0a20 2020 2020 2020 2027  'HUN',.        '
-00036ef0: 2049 6365 6c61 6e64 273a 2027 4953 4c27   Iceland': 'ISL'
-00036f00: 2c0a 2020 2020 2020 2020 2720 496e 6469  ,.        ' Indi
-00036f10: 6127 3a20 2749 4e44 272c 0a20 2020 2020  a': 'IND',.     
-00036f20: 2020 2027 2049 6e64 6f6e 6573 6961 273a     ' Indonesia':
-00036f30: 2027 4944 4e27 2c0a 2020 2020 2020 2020   'IDN',.        
-00036f40: 2720 4972 616e 2028 4973 6c61 6d69 6320  ' Iran (Islamic 
-00036f50: 5265 7075 626c 6963 206f 6629 273a 2027  Republic of)': '
-00036f60: 4952 4e27 2c0a 2020 2020 2020 2020 2720  IRN',.        ' 
-00036f70: 4972 6171 273a 2027 4952 5127 2c0a 2020  Iraq': 'IRQ',.  
-00036f80: 2020 2020 2020 2720 4972 656c 616e 6427        ' Ireland'
-00036f90: 3a20 2749 524c 272c 0a20 2020 2020 2020  : 'IRL',.       
-00036fa0: 2027 2049 7372 6165 6c27 3a20 2749 5352   ' Israel': 'ISR
-00036fb0: 272c 0a20 2020 2020 2020 2027 2049 7461  ',.        ' Ita
-00036fc0: 6c79 273a 2027 4954 4127 2c0a 2020 2020  ly': 'ITA',.    
-00036fd0: 2020 2020 2720 4a61 6d61 6963 6127 3a20      ' Jamaica': 
-00036fe0: 274a 414d 272c 0a20 2020 2020 2020 2027  'JAM',.        '
-00036ff0: 204a 6170 616e 273a 2027 4a50 4e27 2c0a   Japan': 'JPN',.
-00037000: 2020 2020 2020 2020 2720 4a6f 7264 616e          ' Jordan
-00037010: 273a 2027 4a4f 5227 2c0a 2020 2020 2020  ': 'JOR',.      
-00037020: 2020 2720 4b61 7a61 6b68 7374 616e 273a    ' Kazakhstan':
-00037030: 2027 4b41 5a27 2c0a 2020 2020 2020 2020   'KAZ',.        
-00037040: 2720 4b65 6e79 6127 3a20 274b 454e 272c  ' Kenya': 'KEN',
-00037050: 0a20 2020 2020 2020 2027 204b 6972 6962  .        ' Kirib
-00037060: 6174 6927 3a20 274b 4952 272c 0a20 2020  ati': 'KIR',.   
-00037070: 2020 2020 2027 204b 6f72 6561 2028 5265       ' Korea (Re
-00037080: 7075 626c 6963 206f 6629 273a 2027 4b4f  public of)': 'KO
-00037090: 5227 2c0a 2020 2020 2020 2020 2720 4b75  R',.        ' Ku
-000370a0: 7761 6974 273a 2027 4b57 5427 2c0a 2020  wait': 'KWT',.  
-000370b0: 2020 2020 2020 2720 4b79 7267 797a 7374        ' Kyrgyzst
-000370c0: 616e 273a 2027 4b47 5a27 2c0a 2020 2020  an': 'KGZ',.    
-000370d0: 2020 2020 2220 4c61 6f20 5065 6f70 6c65      " Lao People
-000370e0: 2773 2044 656d 6f63 7261 7469 6320 5265  's Democratic Re
-000370f0: 7075 626c 6963 223a 2027 4c41 4f27 2c0a  public": 'LAO',.
-00037100: 2020 2020 2020 2020 2720 4c61 7476 6961          ' Latvia
-00037110: 273a 2027 4c56 4127 2c0a 2020 2020 2020  ': 'LVA',.      
-00037120: 2020 2720 4c65 6261 6e6f 6e27 3a20 274c    ' Lebanon': 'L
-00037130: 424e 272c 0a20 2020 2020 2020 2027 204c  BN',.        ' L
-00037140: 6573 6f74 686f 273a 2027 4c53 4f27 2c0a  esotho': 'LSO',.
-00037150: 2020 2020 2020 2020 2720 4c69 6265 7269          ' Liberi
-00037160: 6127 3a20 274c 4252 272c 0a20 2020 2020  a': 'LBR',.     
-00037170: 2020 2027 204c 6962 7961 273a 2027 4c42     ' Libya': 'LB
-00037180: 5927 2c0a 2020 2020 2020 2020 2720 4c69  Y',.        ' Li
-00037190: 6563 6874 656e 7374 6569 6e27 3a20 274c  echtenstein': 'L
-000371a0: 4945 272c 0a20 2020 2020 2020 2027 204c  IE',.        ' L
-000371b0: 6974 6875 616e 6961 273a 2027 4c54 5527  ithuania': 'LTU'
-000371c0: 2c0a 2020 2020 2020 2020 2720 4c75 7865  ,.        ' Luxe
-000371d0: 6d62 6f75 7267 273a 2027 4c55 5827 2c0a  mbourg': 'LUX',.
-000371e0: 2020 2020 2020 2020 2720 4d61 6461 6761          ' Madaga
-000371f0: 7363 6172 273a 2027 4d44 4727 2c0a 2020  scar': 'MDG',.  
-00037200: 2020 2020 2020 2720 4d61 6c61 7769 273a        ' Malawi':
-00037210: 2027 4d57 4927 2c0a 2020 2020 2020 2020   'MWI',.        
-00037220: 2720 4d61 6c61 7973 6961 273a 2027 4d59  ' Malaysia': 'MY
-00037230: 5327 2c0a 2020 2020 2020 2020 2720 4d61  S',.        ' Ma
-00037240: 6c64 6976 6573 273a 2027 4d44 5627 2c0a  ldives': 'MDV',.
-00037250: 2020 2020 2020 2020 2720 4d61 6c69 273a          ' Mali':
-00037260: 2027 4d4c 4927 2c0a 2020 2020 2020 2020   'MLI',.        
-00037270: 2720 4d61 6c74 6127 3a20 274d 4c54 272c  ' Malta': 'MLT',
-00037280: 0a20 2020 2020 2020 2027 204d 6172 7368  .        ' Marsh
-00037290: 616c 6c20 4973 6c61 6e64 7327 3a20 274d  all Islands': 'M
-000372a0: 484c 272c 0a20 2020 2020 2020 2027 204d  HL',.        ' M
-000372b0: 6175 7269 7461 6e69 6127 3a20 274d 5254  auritania': 'MRT
-000372c0: 272c 0a20 2020 2020 2020 2027 204d 6175  ',.        ' Mau
-000372d0: 7269 7469 7573 273a 2027 4d55 5327 2c0a  ritius': 'MUS',.
-000372e0: 2020 2020 2020 2020 2720 4d65 7869 636f          ' Mexico
-000372f0: 273a 2027 4d45 5827 2c0a 2020 2020 2020  ': 'MEX',.      
-00037300: 2020 2720 4d69 6372 6f6e 6573 6961 2028    ' Micronesia (
-00037310: 4665 6465 7261 7465 6420 5374 6174 6573  Federated States
-00037320: 206f 6629 273a 2027 4653 4d27 2c0a 2020   of)': 'FSM',.  
-00037330: 2020 2020 2020 2720 4d6f 6c64 6f76 6120        ' Moldova 
-00037340: 2852 6570 7562 6c69 6320 6f66 2927 3a20  (Republic of)': 
-00037350: 274d 4441 272c 0a20 2020 2020 2020 2027  'MDA',.        '
-00037360: 204d 6f6e 676f 6c69 6127 3a20 274d 4e47   Mongolia': 'MNG
-00037370: 272c 0a20 2020 2020 2020 2027 204d 6f6e  ',.        ' Mon
-00037380: 7465 6e65 6772 6f27 3a20 274d 4e45 272c  tenegro': 'MNE',
-00037390: 0a20 2020 2020 2020 2027 204d 6f72 6f63  .        ' Moroc
-000373a0: 636f 273a 2027 4d41 5227 2c0a 2020 2020  co': 'MAR',.    
-000373b0: 2020 2020 2720 4d6f 7a61 6d62 6971 7565      ' Mozambique
-000373c0: 273a 2027 4d4f 5a27 2c0a 2020 2020 2020  ': 'MOZ',.      
-000373d0: 2020 2720 4d79 616e 6d61 7227 3a20 274d    ' Myanmar': 'M
-000373e0: 4d52 272c 0a20 2020 2020 2020 2027 204e  MR',.        ' N
-000373f0: 616d 6962 6961 273a 2027 4e41 4d27 2c0a  amibia': 'NAM',.
-00037400: 2020 2020 2020 2020 2720 4e65 7061 6c27          ' Nepal'
-00037410: 3a20 274e 504c 272c 0a20 2020 2020 2020  : 'NPL',.       
-00037420: 2027 204e 6574 6865 726c 616e 6473 273a   ' Netherlands':
-00037430: 2027 4e4c 4427 2c0a 2020 2020 2020 2020   'NLD',.        
-00037440: 2720 4e65 7720 5a65 616c 616e 6427 3a20  ' New Zealand': 
-00037450: 274e 5a4c 272c 0a20 2020 2020 2020 2027  'NZL',.        '
-00037460: 204e 6963 6172 6167 7561 273a 2027 4e49   Nicaragua': 'NI
-00037470: 4327 2c0a 2020 2020 2020 2020 2720 4e69  C',.        ' Ni
-00037480: 6765 7227 3a20 274e 4552 272c 0a20 2020  ger': 'NER',.   
-00037490: 2020 2020 2027 204e 6967 6572 6961 273a       ' Nigeria':
-000374a0: 2027 4e47 4127 2c0a 2020 2020 2020 2020   'NGA',.        
-000374b0: 2720 4e6f 7274 6820 4d61 6365 646f 6e69  ' North Macedoni
-000374c0: 6127 3a20 274d 4b44 272c 0a20 2020 2020  a': 'MKD',.     
-000374d0: 2020 2027 204e 6f72 7761 7927 3a20 274e     ' Norway': 'N
-000374e0: 4f52 272c 0a20 2020 2020 2020 2027 204f  OR',.        ' O
-000374f0: 6d61 6e27 3a20 274f 4d4e 272c 0a20 2020  man': 'OMN',.   
-00037500: 2020 2020 2027 2050 616b 6973 7461 6e27       ' Pakistan'
-00037510: 3a20 2750 414b 272c 0a20 2020 2020 2020  : 'PAK',.       
-00037520: 2027 2050 616c 6175 273a 2027 504c 5727   ' Palau': 'PLW'
-00037530: 2c0a 2020 2020 2020 2020 2720 5061 6c65  ,.        ' Pale
-00037540: 7374 696e 652c 2053 7461 7465 206f 6627  stine, State of'
-00037550: 3a20 2750 5345 272c 0a20 2020 2020 2020  : 'PSE',.       
-00037560: 2027 2050 616e 616d 6127 3a20 2750 414e   ' Panama': 'PAN
-00037570: 272c 0a20 2020 2020 2020 2027 2050 6170  ',.        ' Pap
-00037580: 7561 204e 6577 2047 7569 6e65 6127 3a20  ua New Guinea': 
-00037590: 2750 4e47 272c 0a20 2020 2020 2020 2027  'PNG',.        '
-000375a0: 2050 6172 6167 7561 7927 3a20 2750 5259   Paraguay': 'PRY
-000375b0: 272c 0a20 2020 2020 2020 2027 2050 6572  ',.        ' Per
-000375c0: 7527 3a20 2750 4552 272c 0a20 2020 2020  u': 'PER',.     
-000375d0: 2020 2027 2050 6869 6c69 7070 696e 6573     ' Philippines
-000375e0: 273a 2027 5048 4c27 2c0a 2020 2020 2020  ': 'PHL',.      
-000375f0: 2020 2720 506f 6c61 6e64 273a 2027 504f    ' Poland': 'PO
-00037600: 4c27 2c0a 2020 2020 2020 2020 2720 506f  L',.        ' Po
-00037610: 7274 7567 616c 273a 2027 5052 5427 2c0a  rtugal': 'PRT',.
-00037620: 2020 2020 2020 2020 2720 5161 7461 7227          ' Qatar'
-00037630: 3a20 2751 4154 272c 0a20 2020 2020 2020  : 'QAT',.       
-00037640: 2027 2052 6f6d 616e 6961 273a 2027 524f   ' Romania': 'RO
-00037650: 5527 2c0a 2020 2020 2020 2020 2720 5275  U',.        ' Ru
-00037660: 7373 6961 6e20 4665 6465 7261 7469 6f6e  ssian Federation
-00037670: 273a 2027 5255 5327 2c0a 2020 2020 2020  ': 'RUS',.      
-00037680: 2020 2720 5277 616e 6461 273a 2027 5257    ' Rwanda': 'RW
-00037690: 4127 2c0a 2020 2020 2020 2020 2720 5361  A',.        ' Sa
-000376a0: 696e 7420 4b69 7474 7320 616e 6420 4e65  int Kitts and Ne
-000376b0: 7669 7327 3a20 274b 4e41 272c 0a20 2020  vis': 'KNA',.   
-000376c0: 2020 2020 2027 2053 6169 6e74 204c 7563       ' Saint Luc
-000376d0: 6961 273a 2027 4c43 4127 2c0a 2020 2020  ia': 'LCA',.    
-000376e0: 2020 2020 2720 5361 696e 7420 5669 6e63      ' Saint Vinc
-000376f0: 656e 7420 616e 6420 7468 6520 4772 656e  ent and the Gren
-00037700: 6164 696e 6573 273a 2027 5643 5427 2c0a  adines': 'VCT',.
-00037710: 2020 2020 2020 2020 2720 5361 6d6f 6127          ' Samoa'
-00037720: 3a20 2757 534d 272c 0a20 2020 2020 2020  : 'WSM',.       
-00037730: 2027 2053 616f 2054 6f6d 6520 616e 6420   ' Sao Tome and 
-00037740: 5072 696e 6369 7065 273a 2027 5354 5027  Principe': 'STP'
-00037750: 2c0a 2020 2020 2020 2020 2720 5361 7564  ,.        ' Saud
-00037760: 6920 4172 6162 6961 273a 2027 5341 5527  i Arabia': 'SAU'
-00037770: 2c0a 2020 2020 2020 2020 2720 5365 6e65  ,.        ' Sene
-00037780: 6761 6c27 3a20 2753 454e 272c 0a20 2020  gal': 'SEN',.   
-00037790: 2020 2020 2027 2053 6572 6269 6127 3a20       ' Serbia': 
-000377a0: 2753 5242 272c 0a20 2020 2020 2020 2027  'SRB',.        '
-000377b0: 2053 6579 6368 656c 6c65 7327 3a20 2753   Seychelles': 'S
-000377c0: 5943 272c 0a20 2020 2020 2020 2027 2053  YC',.        ' S
-000377d0: 6965 7272 6120 4c65 6f6e 6527 3a20 2753  ierra Leone': 'S
-000377e0: 4c45 272c 0a20 2020 2020 2020 2027 2053  LE',.        ' S
-000377f0: 696e 6761 706f 7265 273a 2027 5347 5027  ingapore': 'SGP'
-00037800: 2c0a 2020 2020 2020 2020 2720 536c 6f76  ,.        ' Slov
-00037810: 616b 6961 273a 2027 5356 4b27 2c0a 2020  akia': 'SVK',.  
-00037820: 2020 2020 2020 2720 536c 6f76 656e 6961        ' Slovenia
-00037830: 273a 2027 5356 4e27 2c0a 2020 2020 2020  ': 'SVN',.      
-00037840: 2020 2720 536f 6c6f 6d6f 6e20 4973 6c61    ' Solomon Isla
-00037850: 6e64 7327 3a20 2753 4c42 272c 0a20 2020  nds': 'SLB',.   
-00037860: 2020 2020 2027 2053 6f75 7468 2041 6672       ' South Afr
-00037870: 6963 6127 3a20 275a 4146 272c 0a20 2020  ica': 'ZAF',.   
-00037880: 2020 2020 2027 2053 6f75 7468 2053 7564       ' South Sud
-00037890: 616e 273a 2027 5353 4427 2c0a 2020 2020  an': 'SSD',.    
-000378a0: 2020 2020 2720 5370 6169 6e27 3a20 2745      ' Spain': 'E
-000378b0: 5350 272c 0a20 2020 2020 2020 2027 2053  SP',.        ' S
-000378c0: 7269 204c 616e 6b61 273a 2027 4c4b 4127  ri Lanka': 'LKA'
-000378d0: 2c0a 2020 2020 2020 2020 2720 5375 6461  ,.        ' Suda
-000378e0: 6e27 3a20 2753 444e 272c 0a20 2020 2020  n': 'SDN',.     
-000378f0: 2020 2027 2053 7572 696e 616d 6527 3a20     ' Suriname': 
-00037900: 2753 5552 272c 0a20 2020 2020 2020 2027  'SUR',.        '
-00037910: 2053 7765 6465 6e27 3a20 2753 5745 272c   Sweden': 'SWE',
-00037920: 0a20 2020 2020 2020 2027 2053 7769 747a  .        ' Switz
-00037930: 6572 6c61 6e64 273a 2027 4348 4527 2c0a  erland': 'CHE',.
-00037940: 2020 2020 2020 2020 2720 5379 7269 616e          ' Syrian
-00037950: 2041 7261 6220 5265 7075 626c 6963 273a   Arab Republic':
-00037960: 2027 5359 5227 2c0a 2020 2020 2020 2020   'SYR',.        
-00037970: 2720 5461 6a69 6b69 7374 616e 273a 2027  ' Tajikistan': '
-00037980: 544a 4b27 2c0a 2020 2020 2020 2020 2720  TJK',.        ' 
-00037990: 5461 6e7a 616e 6961 2028 556e 6974 6564  Tanzania (United
-000379a0: 2052 6570 7562 6c69 6320 6f66 2927 3a20   Republic of)': 
-000379b0: 2754 5a41 272c 0a20 2020 2020 2020 2027  'TZA',.        '
-000379c0: 2054 6861 696c 616e 6427 3a20 2754 4841   Thailand': 'THA
-000379d0: 272c 0a20 2020 2020 2020 2027 2054 696d  ',.        ' Tim
-000379e0: 6f72 2d4c 6573 7465 273a 2027 544c 5327  or-Leste': 'TLS'
-000379f0: 2c0a 2020 2020 2020 2020 2720 546f 676f  ,.        ' Togo
-00037a00: 273a 2027 5447 4f27 2c0a 2020 2020 2020  ': 'TGO',.      
-00037a10: 2020 2720 546f 6e67 6127 3a20 2754 4f4e    ' Tonga': 'TON
-00037a20: 272c 0a20 2020 2020 2020 2027 2054 7269  ',.        ' Tri
-00037a30: 6e69 6461 6420 616e 6420 546f 6261 676f  nidad and Tobago
-00037a40: 273a 2027 5454 4f27 2c0a 2020 2020 2020  ': 'TTO',.      
-00037a50: 2020 2720 5475 6e69 7369 6127 3a20 2754    ' Tunisia': 'T
-00037a60: 554e 272c 0a20 2020 2020 2020 2027 2054  UN',.        ' T
-00037a70: 7572 6b65 7927 3a20 2754 5552 272c 0a20  urkey': 'TUR',. 
-00037a80: 2020 2020 2020 2027 2054 7572 6b6d 656e         ' Turkmen
-00037a90: 6973 7461 6e27 3a20 2754 4b4d 272c 0a20  istan': 'TKM',. 
-00037aa0: 2020 2020 2020 2027 2055 6761 6e64 6127         ' Uganda'
-00037ab0: 3a20 2755 4741 272c 0a20 2020 2020 2020  : 'UGA',.       
-00037ac0: 2027 2055 6b72 6169 6e65 273a 2027 554b   ' Ukraine': 'UK
-00037ad0: 5227 2c0a 2020 2020 2020 2020 2720 556e  R',.        ' Un
-00037ae0: 6974 6564 2041 7261 6220 456d 6972 6174  ited Arab Emirat
-00037af0: 6573 273a 2027 4152 4527 2c0a 2020 2020  es': 'ARE',.    
-00037b00: 2020 2020 2720 556e 6974 6564 204b 696e      ' United Kin
-00037b10: 6764 6f6d 273a 2027 4742 5227 2c0a 2020  gdom': 'GBR',.  
-00037b20: 2020 2020 2020 2720 556e 6974 6564 2053        ' United S
-00037b30: 7461 7465 7327 3a20 2755 5341 272c 0a20  tates': 'USA',. 
-00037b40: 2020 2020 2020 2027 2055 7275 6775 6179         ' Uruguay
-00037b50: 273a 2027 5552 5927 2c0a 2020 2020 2020  ': 'URY',.      
-00037b60: 2020 2720 557a 6265 6b69 7374 616e 273a    ' Uzbekistan':
-00037b70: 2027 555a 4227 2c0a 2020 2020 2020 2020   'UZB',.        
-00037b80: 2720 5661 6e75 6174 7527 3a20 2756 5554  ' Vanuatu': 'VUT
-00037b90: 272c 0a20 2020 2020 2020 2027 2056 656e  ',.        ' Ven
-00037ba0: 657a 7565 6c61 2028 426f 6c69 7661 7269  ezuela (Bolivari
-00037bb0: 616e 2052 6570 7562 6c69 6320 6f66 2927  an Republic of)'
-00037bc0: 3a20 2756 454e 272c 0a20 2020 2020 2020  : 'VEN',.       
-00037bd0: 2027 2056 6965 7420 4e61 6d27 3a20 2756   ' Viet Nam': 'V
-00037be0: 4e4d 272c 0a20 2020 2020 2020 2027 2059  NM',.        ' Y
-00037bf0: 656d 656e 273a 2027 5945 4d27 2c0a 2020  emen': 'YEM',.  
-00037c00: 2020 2020 2020 2720 5a61 6d62 6961 273a        ' Zambia':
-00037c10: 2027 5a4d 4227 2c0a 2020 2020 2020 2020   'ZMB',.        
-00037c20: 2720 5a69 6d62 6162 7765 273a 2027 5a57  ' Zimbabwe': 'ZW
-00037c30: 4527 2c0a 2020 2020 2020 2020 2748 756d  E',.        'Hum
-00037c40: 616e 2044 6576 656c 6f70 6d65 6e74 273a  an Development':
-00037c50: 204e 6f6e 652c 0a20 2020 2020 2020 2027   None,.        '
-00037c60: 5665 7279 2068 6967 6820 6875 6d61 6e20  Very high human 
-00037c70: 6465 7665 6c6f 706d 656e 7427 3a20 4e6f  development': No
-00037c80: 6e65 2c0a 2020 2020 2020 2020 2748 6967  ne,.        'Hig
-00037c90: 6820 6875 6d61 6e20 6465 7665 6c6f 706d  h human developm
-00037ca0: 656e 7427 3a20 4e6f 6e65 2c0a 2020 2020  ent': None,.    
-00037cb0: 2020 2020 274d 6564 6975 6d20 6875 6d61      'Medium huma
-00037cc0: 6e20 6465 7665 6c6f 706d 656e 7427 3a20  n development': 
-00037cd0: 4e6f 6e65 2c0a 2020 2020 2020 2020 274c  None,.        'L
-00037ce0: 6f77 2068 756d 616e 2064 6576 656c 6f70  ow human develop
-00037cf0: 6d65 6e74 273a 204e 6f6e 652c 0a20 2020  ment': None,.   
-00037d00: 2020 2020 2027 4465 7665 6c6f 7069 6e67       'Developing
-00037d10: 2043 6f75 6e74 7269 6573 273a 204e 6f6e   Countries': Non
-00037d20: 652c 0a20 2020 2020 2020 2027 5265 6769  e,.        'Regi
-00037d30: 6f6e 7327 3a20 4e6f 6e65 2c0a 2020 2020  ons': None,.    
-00037d40: 2020 2020 2741 7261 6220 5374 6174 6573      'Arab States
-00037d50: 273a 204e 6f6e 652c 0a20 2020 2020 2020  ': None,.       
-00037d60: 2027 4561 7374 2041 7369 6120 616e 6420   'East Asia and 
-00037d70: 7468 6520 5061 6369 6669 6327 3a20 4e6f  the Pacific': No
-00037d80: 6e65 2c0a 2020 2020 2020 2020 2745 7572  ne,.        'Eur
-00037d90: 6f70 6520 616e 6420 4365 6e74 7261 6c20  ope and Central 
-00037da0: 4173 6961 273a 204e 6f6e 652c 0a20 2020  Asia': None,.   
-00037db0: 2020 2020 2027 4c61 7469 6e20 416d 6572       'Latin Amer
-00037dc0: 6963 6120 616e 6420 7468 6520 4361 7269  ica and the Cari
-00037dd0: 6262 6561 6e27 3a20 4e6f 6e65 2c0a 2020  bbean': None,.  
-00037de0: 2020 2020 2020 2753 6f75 7468 2041 7369        'South Asi
-00037df0: 6127 3a20 4e6f 6e65 2c0a 2020 2020 2020  a': None,.      
-00037e00: 2020 2753 7562 2d53 6168 6172 616e 2041    'Sub-Saharan A
-00037e10: 6672 6963 6127 3a20 4e6f 6e65 2c0a 2020  frica': None,.  
-00037e20: 2020 2020 2020 274c 6561 7374 2044 6576        'Least Dev
-00037e30: 656c 6f70 6564 2043 6f75 6e74 7269 6573  eloped Countries
-00037e40: 273a 204e 6f6e 652c 0a20 2020 2020 2020  ': None,.       
-00037e50: 2027 536d 616c 6c20 4973 6c61 6e64 2044   'Small Island D
-00037e60: 6576 656c 6f70 696e 6720 5374 6174 6573  eveloping States
-00037e70: 273a 204e 6f6e 652c 0a20 2020 2020 2020  ': None,.       
-00037e80: 2027 4f72 6761 6e69 7a61 7469 6f6e 2066   'Organization f
-00037e90: 6f72 2045 636f 6e6f 6d69 6320 436f 2d6f  or Economic Co-o
-00037ea0: 7065 7261 7469 6f6e 2061 6e64 2044 6576  peration and Dev
-00037eb0: 656c 6f70 6d65 6e74 273a 204e 6f6e 652c  elopment': None,
-00037ec0: 0a20 2020 2020 2020 2027 576f 726c 6427  .        'World'
-00037ed0: 3a20 2757 6f72 6c64 272c 0a20 2020 207d  : 'World',.    }
-00037ee0: 0a0a 2020 2020 6461 7461 2e69 6e64 6578  ..    data.index
-00037ef0: 203d 2064 6174 612e 6c6f 635b 3a2c 2027   = data.loc[:, '
-00037f00: 436f 756e 7472 7927 5d2e 6d61 7028 7265  Country'].map(re
-00037f10: 6769 6f6e 4d61 7070 696e 6729 0a0a 2020  gionMapping)..  
-00037f20: 2020 6461 7461 2e69 6e64 6578 5b64 6174    data.index[dat
-00037f30: 612e 696e 6465 782e 6475 706c 6963 6174  a.index.duplicat
-00037f40: 6564 2829 5d0a 2020 2020 6461 7461 203d  ed()].    data =
-00037f50: 2064 6174 612e 6c6f 635b 3a2c 2079 6561   data.loc[:, yea
-00037f60: 7243 6f6c 756d 6e73 5d0a 2020 2020 6461  rColumns].    da
-00037f70: 7461 203d 2064 6174 612e 6c6f 635b 7e64  ta = data.loc[~d
-00037f80: 6174 612e 696e 6465 782e 6973 6e75 6c6c  ata.index.isnull
-00037f90: 2829 2c20 3a5d 2e61 7374 7970 6528 666c  (), :].astype(fl
-00037fa0: 6f61 7429 0a0a 2020 2020 6d65 7461 203d  oat)..    meta =
-00037fb0: 207b 0a20 2020 2020 2020 2027 656e 7469   {.        'enti
-00037fc0: 7479 273a 2027 4844 495f 4875 6d61 6e5f  ty': 'HDI_Human_
-00037fd0: 6465 7665 6c6f 706d 656e 745f 696e 6465  development_inde
-00037fe0: 7827 2c0a 2020 2020 2020 2020 2773 6365  x',.        'sce
-00037ff0: 6e61 7269 6f27 3a20 2748 6973 746f 7269  nario': 'Histori
-00038000: 6327 2c0a 2020 2020 2020 2020 2775 6e69  c',.        'uni
-00038010: 7427 3a20 2764 696d 656e 7369 6f6e 6c65  t': 'dimensionle
-00038020: 7373 272c 0a20 2020 2020 2020 2027 736f  ss',.        'so
-00038030: 7572 6365 273a 2073 6f75 7263 654d 6574  urce': sourceMet
-00038040: 615b 2753 4f55 5243 455f 4944 275d 2c0a  a['SOURCE_ID'],.
-00038050: 2020 2020 7d0a 2020 2020 7461 626c 6520      }.    table 
-00038060: 3d20 6474 2e44 6174 6174 6162 6c65 2864  = dt.Datatable(d
-00038070: 6174 612c 206d 6574 613d 6d65 7461 290a  ata, meta=meta).
-00038080: 2020 2020 7461 626c 652e 6765 6e65 7261      table.genera
-00038090: 7465 5461 626c 6549 4428 290a 0a20 2020  teTableID()..   
-000380a0: 2064 742e 636f 6d6d 6974 5461 626c 6573   dt.commitTables
-000380b0: 285b 7461 626c 655d 2c20 2748 4449 2064  ([table], 'HDI d
-000380c0: 6174 6120 7570 6461 7465 272c 2073 6f75  ata update', sou
-000380d0: 7263 654d 6574 612c 2075 7064 6174 653d  rceMeta, update=
-000380e0: 5472 7565 290a 0a0a 6465 6620 554e 5f57  True)...def UN_W
-000380f0: 5050 5f32 3031 395f 696d 706f 7274 2829  PP_2019_import()
-00038100: 3a0a 2020 2020 736f 7572 6365 4d65 7461  :.    sourceMeta
-00038110: 203d 207b 0a20 2020 2020 2020 2027 534f   = {.        'SO
-00038120: 5552 4345 5f49 4427 3a20 2755 4e5f 5750  URCE_ID': 'UN_WP
-00038130: 5032 3031 3927 2c0a 2020 2020 2020 2020  P2019',.        
-00038140: 2763 6f6c 6c65 6374 6564 5f62 7927 3a20  'collected_by': 
-00038150: 2741 4727 2c0a 2020 2020 2020 2020 2764  'AG',.        'd
-00038160: 6174 6527 3a20 6474 2e63 6f72 652e 6765  ate': dt.core.ge
-00038170: 745f 6461 7465 5f73 7472 696e 6728 292c  t_date_string(),
-00038180: 0a20 2020 2020 2020 2027 736f 7572 6365  .        'source
-00038190: 5f75 726c 273a 2027 6874 7470 733a 2f2f  _url': 'https://
-000381a0: 706f 7075 6c61 7469 6f6e 2e75 6e2e 6f72  population.un.or
-000381b0: 672f 7770 702f 446f 776e 6c6f 6164 2f53  g/wpp/Download/S
-000381c0: 7461 6e64 6172 642f 506f 7075 6c61 7469  tandard/Populati
-000381d0: 6f6e 2f27 2c0a 2020 2020 2020 2020 276c  on/',.        'l
-000381e0: 6963 656e 6365 273a 2027 6f70 656e 2073  icence': 'open s
-000381f0: 6f75 7263 6527 2c0a 2020 2020 7d0a 0a20  ource',.    }.. 
-00038200: 2020 206d 6170 7069 6e67 4469 6374 203d     mappingDict =
-00038210: 207b 0a20 2020 2020 2020 2069 6e74 2878   {.        int(x
-00038220: 293a 2079 0a20 2020 2020 2020 2066 6f72  ): y.        for
-00038230: 2078 2c20 7920 696e 207a 6970 2864 742e   x, y in zip(dt.
-00038240: 6d61 7070 2e63 6f75 6e74 7269 6573 2e63  mapp.countries.c
-00038250: 6f64 6573 2e6e 756d 4953 4f2c 2064 742e  odes.numISO, dt.
-00038260: 6d61 7070 2e63 6f75 6e74 7269 6573 2e63  mapp.countries.c
-00038270: 6f64 6573 2e69 6e64 6578 290a 2020 2020  odes.index).    
-00038280: 2020 2020 6966 206e 6f74 2028 7064 2e6e      if not (pd.n
-00038290: 702e 6973 6e61 6e28 7829 290a 2020 2020  p.isnan(x)).    
-000382a0: 7d0a 2020 2020 6d61 7070 696e 6744 6963  }.    mappingDic
-000382b0: 745b 3930 305d 203d 2027 576f 726c 6427  t[900] = 'World'
-000382c0: 0a20 2020 2053 4f55 5243 4520 3d20 2255  .    SOURCE = "U
-000382d0: 4e5f 5750 5032 3031 3922 0a20 2020 2053  N_WPP2019".    S
-000382e0: 4f55 5243 455f 5041 5448 203d 206f 732e  OURCE_PATH = os.
-000382f0: 7061 7468 2e6a 6f69 6e28 6474 2e63 6f6e  path.join(dt.con
-00038300: 6669 672e 5041 5448 5f54 4f5f 4441 5441  fig.PATH_TO_DATA
-00038310: 5348 454c 462c 2027 7261 7764 6174 612f  SHELF, 'rawdata/
-00038320: 554e 5f57 5050 3230 3139 2729 0a20 2020  UN_WPP2019').   
-00038330: 206d 6574 6153 6574 7570 203d 207b 0a20   metaSetup = {. 
-00038340: 2020 2020 2020 2027 736f 7572 6365 273a         'source':
-00038350: 2053 4f55 5243 452c 0a20 2020 2020 2020   SOURCE,.       
-00038360: 2027 656e 7469 7479 273a 2027 706f 7075   'entity': 'popu
-00038370: 6c61 7469 6f6e 272c 0a20 2020 2020 2020  lation',.       
-00038380: 2027 756e 6974 273a 2027 7468 6f75 7361   'unit': 'thousa
-00038390: 6e64 7327 2c0a 2020 2020 2020 2020 2763  nds',.        'c
-000383a0: 6174 6567 6f72 7927 3a20 2774 6f74 616c  ategory': 'total
-000383b0: 272c 0a20 2020 207d 0a0a 2020 2020 2320  ',.    }..    # 
-000383c0: 6368 616e 6765 2073 6574 7570 0a20 2020  change setup.   
-000383d0: 2065 7863 656c 5365 7475 7020 3d20 6469   excelSetup = di
-000383e0: 6374 2829 0a20 2020 2065 7863 656c 5365  ct().    excelSe
-000383f0: 7475 705b 2766 696c 6550 6174 6827 5d20  tup['filePath'] 
-00038400: 3d20 534f 5552 4345 5f50 4154 480a 2020  = SOURCE_PATH.  
-00038410: 2020 6578 6365 6c53 6574 7570 5b27 6669    excelSetup['fi
-00038420: 6c65 4e61 6d65 275d 203d 2027 5750 5032  leName'] = 'WPP2
-00038430: 3031 395f 504f 505f 4630 315f 315f 544f  019_POP_F01_1_TO
-00038440: 5441 4c5f 504f 5055 4c41 5449 4f4e 5f42  TAL_POPULATION_B
-00038450: 4f54 485f 5345 5845 532e 786c 7378 270a  OTH_SEXES.xlsx'.
-00038460: 2020 2020 6578 6365 6c53 6574 7570 5b27      excelSetup['
-00038470: 7368 6565 744e 616d 6527 5d20 3d20 2745  sheetName'] = 'E
-00038480: 5354 494d 4154 4553 270a 2020 2020 6578  STIMATES'.    ex
-00038490: 6365 6c53 6574 7570 5b27 7469 6d65 436f  celSetup['timeCo
-000384a0: 6c49 6478 275d 203d 2028 2748 3137 272c  lIdx'] = ('H17',
-000384b0: 2027 434a 3137 2729 0a20 2020 2065 7863   'CJ17').    exc
-000384c0: 656c 5365 7475 705b 2773 7061 6365 526f  elSetup['spaceRo
-000384d0: 7749 6478 275d 203d 2028 2745 3138 272c  wIdx'] = ('E18',
-000384e0: 2027 4533 3036 2729 0a0a 2020 2020 7461   'E306')..    ta
-000384f0: 626c 6573 203d 206c 6973 7428 290a 0a20  bles = list().. 
-00038500: 2020 2023 2067 6174 6865 7220 6869 7374     # gather hist
-00038510: 6f72 6963 2064 6174 610a 2020 2020 2320  oric data.    # 
-00038520: 2020 2020 2020 2069 746f 6f6c 203d 2055         itool = U
-00038530: 4e5f 5750 5028 6578 6365 6c53 6574 7570  N_WPP(excelSetup
-00038540: 290a 2020 2020 6d65 7461 5365 7475 705b  ).    metaSetup[
-00038550: 2773 6365 6e61 7269 6f27 5d20 3d20 2768  'scenario'] = 'h
-00038560: 6973 746f 7269 6327 0a20 2020 2065 7874  istoric'.    ext
-00038570: 7261 6374 6f72 203d 2064 742e 696f 2e45  ractor = dt.io.E
-00038580: 7863 656c 5265 6164 6572 2865 7863 656c  xcelReader(excel
-00038590: 5365 7475 7029 0a20 2020 2074 6162 6c65  Setup).    table
-000385a0: 203d 2065 7874 7261 6374 6f72 2e67 6174   = extractor.gat
-000385b0: 6865 7244 6174 6128 290a 2020 2020 7461  herData().    ta
-000385c0: 626c 6520 3d20 7461 626c 652e 7265 706c  ble = table.repl
-000385d0: 6163 6528 27e2 80a6 272c 2070 642e 6e70  ace('...', pd.np
-000385e0: 2e6e 616e 290a 2020 2020 7461 626c 655b  .nan).    table[
-000385f0: 276e 6577 496e 6465 7827 5d20 3d20 7461  'newIndex'] = ta
-00038600: 626c 652e 696e 6465 780a 2020 2020 7461  ble.index.    ta
-00038610: 626c 655b 276e 6577 496e 6465 7827 5d20  ble['newIndex'] 
-00038620: 3d20 7461 626c 652e 696e 6465 782e 746f  = table.index.to
-00038630: 5f73 6572 6965 7328 292e 6d61 7028 6d61  _series().map(ma
-00038640: 7070 696e 6744 6963 7429 0a20 2020 2074  ppingDict).    t
-00038650: 6162 6c65 2e6c 6f63 5b70 642e 6973 6e75  able.loc[pd.isnu
-00038660: 6c6c 2874 6162 6c65 5b27 6e65 7749 6e64  ll(table['newInd
-00038670: 6578 275d 292c 2027 6e65 7749 6e64 6578  ex']), 'newIndex
-00038680: 275d 203d 2074 6162 6c65 2e69 6e64 6578  '] = table.index
-00038690: 5b0a 2020 2020 2020 2020 7064 2e69 736e  [.        pd.isn
-000386a0: 756c 6c28 7461 626c 655b 276e 6577 496e  ull(table['newIn
-000386b0: 6465 7827 5d29 0a20 2020 205d 0a20 2020  dex']).    ].   
-000386c0: 2074 6162 6c65 203d 2074 6162 6c65 2e73   table = table.s
-000386d0: 6574 5f69 6e64 6578 2827 6e65 7749 6e64  et_index('newInd
-000386e0: 6578 2729 0a20 2020 206e 6577 4964 7820  ex').    newIdx 
-000386f0: 3d20 5b6d 6170 7069 6e67 4469 6374 5b78  = [mappingDict[x
-00038700: 5d20 666f 7220 7820 696e 2074 6162 6c65  ] for x in table
-00038710: 2e69 6e64 6578 2069 6620 7820 696e 206d  .index if x in m
-00038720: 6170 7069 6e67 4469 6374 2e6b 6579 7328  appingDict.keys(
-00038730: 295d 0a20 2020 2074 6162 6c65 732e 6170  )].    tables.ap
-00038740: 7065 6e64 2864 742e 4461 7461 7461 626c  pend(dt.Datatabl
-00038750: 6528 7461 626c 652c 206d 6574 613d 6d65  e(table, meta=me
-00038760: 7461 5365 7475 7029 290a 0a20 2020 2023  taSetup))..    #
-00038770: 2067 6174 6865 7220 7072 6f6a 6563 7469   gather projecti
-00038780: 6e6f 730a 2020 2020 2320 6578 6365 6c53  nos.    # excelS
-00038790: 6574 7570 5b27 7469 6d65 436f 6c49 6478  etup['timeColIdx
-000387a0: 275d 2020 3d20 2827 4631 3727 2c20 2743  ']  = ('F17', 'C
-000387b0: 5731 3727 290a 0a20 2020 2073 6365 6e44  W17')..    scenD
-000387c0: 6963 7420 3d20 7b0a 2020 2020 2020 2020  ict = {.        
-000387d0: 2750 524f 4a45 4354 494f 4e5f 4c4f 5727  'PROJECTION_LOW'
-000387e0: 3a20 274c 4f57 2056 4152 4941 4e54 272c  : 'LOW VARIANT',
-000387f0: 0a20 2020 2020 2020 2027 5052 4f4a 4543  .        'PROJEC
-00038800: 5449 4f4e 5f4d 4544 273a 2027 4d45 4449  TION_MED': 'MEDI
-00038810: 554d 2056 4152 4941 4e54 272c 0a20 2020  UM VARIANT',.   
-00038820: 2020 2020 2027 5052 4f4a 4543 5449 4f4e       'PROJECTION
-00038830: 5f48 4927 3a20 2748 4947 4820 5641 5249  _HI': 'HIGH VARI
-00038840: 414e 5427 2c0a 2020 2020 7d0a 2020 2020  ANT',.    }.    
-00038850: 2320 6974 6f6f 6c20 3d20 554e 5f57 5050  # itool = UN_WPP
-00038860: 2865 7863 656c 5365 7475 7029 0a0a 2020  (excelSetup)..  
-00038870: 2020 666f 7220 7363 656e 6172 696f 2c20    for scenario, 
-00038880: 7368 6565 744e 616d 6520 696e 2073 6365  sheetName in sce
-00038890: 6e44 6963 742e 6974 656d 7328 293a 0a20  nDict.items():. 
-000388a0: 2020 2020 2020 206d 6574 6153 6574 7570         metaSetup
-000388b0: 5b27 7363 656e 6172 696f 275d 203d 2073  ['scenario'] = s
-000388c0: 6365 6e61 7269 6f0a 2020 2020 2020 2020  cenario.        
-000388d0: 6578 6365 6c53 6574 7570 5b27 7368 6565  excelSetup['shee
-000388e0: 744e 616d 6527 5d20 3d20 7368 6565 744e  tName'] = sheetN
-000388f0: 616d 650a 2020 2020 2020 2020 6578 7472  ame.        extr
-00038900: 6163 746f 7220 3d20 6474 2e69 6f2e 4578  actor = dt.io.Ex
-00038910: 6365 6c52 6561 6465 7228 6578 6365 6c53  celReader(excelS
-00038920: 6574 7570 290a 2020 2020 2020 2020 7461  etup).        ta
-00038930: 626c 6520 3d20 6578 7472 6163 746f 722e  ble = extractor.
-00038940: 6761 7468 6572 4461 7461 2829 0a20 2020  gatherData().   
-00038950: 2020 2020 2074 6162 6c65 203d 2074 6162       table = tab
-00038960: 6c65 2e72 6570 6c61 6365 2827 e280 a627  le.replace('...'
-00038970: 2c20 7064 2e6e 702e 6e61 6e29 0a20 2020  , pd.np.nan).   
-00038980: 2020 2020 2074 6162 6c65 5b27 6e65 7749       table['newI
-00038990: 6e64 6578 275d 203d 2074 6162 6c65 2e69  ndex'] = table.i
-000389a0: 6e64 6578 0a20 2020 2020 2020 2074 6162  ndex.        tab
-000389b0: 6c65 5b27 6e65 7749 6e64 6578 275d 203d  le['newIndex'] =
-000389c0: 2074 6162 6c65 2e69 6e64 6578 2e74 6f5f   table.index.to_
-000389d0: 7365 7269 6573 2829 2e6d 6170 286d 6170  series().map(map
-000389e0: 7069 6e67 4469 6374 290a 2020 2020 2020  pingDict).      
-000389f0: 2020 7461 626c 652e 6c6f 635b 7064 2e69    table.loc[pd.i
-00038a00: 736e 756c 6c28 7461 626c 655b 276e 6577  snull(table['new
-00038a10: 496e 6465 7827 5d29 2c20 276e 6577 496e  Index']), 'newIn
-00038a20: 6465 7827 5d20 3d20 7461 626c 652e 696e  dex'] = table.in
-00038a30: 6465 785b 0a20 2020 2020 2020 2020 2020  dex[.           
-00038a40: 2070 642e 6973 6e75 6c6c 2874 6162 6c65   pd.isnull(table
-00038a50: 5b27 6e65 7749 6e64 6578 275d 290a 2020  ['newIndex']).  
-00038a60: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00038a70: 7461 626c 6520 3d20 7461 626c 652e 7365  table = table.se
-00038a80: 745f 696e 6465 7828 276e 6577 496e 6465  t_index('newInde
-00038a90: 7827 290a 2020 2020 2020 2020 7461 626c  x').        tabl
-00038aa0: 6573 2e61 7070 656e 6428 6474 2e44 6174  es.append(dt.Dat
-00038ab0: 6174 6162 6c65 2874 6162 6c65 2c20 6d65  atable(table, me
-00038ac0: 7461 3d6d 6574 6153 6574 7570 2929 0a20  ta=metaSetup)). 
-00038ad0: 2020 2023 2525 0a20 2020 2064 6566 2061     #%%.    def a
-00038ae0: 6464 5f45 5528 7461 626c 6529 3a0a 2020  dd_EU(table):.  
-00038af0: 2020 2020 2020 4555 5f43 4f55 4e54 5249        EU_COUNTRI
-00038b00: 4553 203d 206c 6973 7428 6474 2e6d 6170  ES = list(dt.map
-00038b10: 702e 7265 6769 6f6e 732e 4555 3238 2e6d  p.regions.EU28.m
-00038b20: 656d 6265 7273 4f66 2827 4555 3238 2729  embersOf('EU28')
-00038b30: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
-00038b40: 6c6f 635b 2745 5532 3827 5d20 3d20 7461  loc['EU28'] = ta
-00038b50: 626c 652e 6c6f 635b 4555 5f43 4f55 4e54  ble.loc[EU_COUNT
-00038b60: 5249 4553 5d2e 7375 6d28 290a 2020 2020  RIES].sum().    
-00038b70: 2020 2020 7265 7475 726e 2074 6162 6c65      return table
-00038b80: 0a0a 2020 2020 7461 626c 6573 203d 205b  ..    tables = [
-00038b90: 6164 645f 4555 2874 6162 6c65 2920 666f  add_EU(table) fo
-00038ba0: 7220 7461 626c 6520 696e 2074 6162 6c65  r table in table
-00038bb0: 735d 0a0a 2020 2020 6474 2e63 6f6d 6d69  s]..    dt.commi
-00038bc0: 7454 6162 6c65 7328 7461 626c 6573 2c20  tTables(tables, 
-00038bd0: 2755 4e57 5050 3230 3137 2064 6174 6127  'UNWPP2017 data'
-00038be0: 2c20 736f 7572 6365 4d65 7461 2c20 6170  , sourceMeta, ap
-00038bf0: 7065 6e64 5f64 6174 613d 5472 7565 2c20  pend_data=True, 
-00038c00: 7570 6461 7465 3d54 7275 6529 0a20 2020  update=True).   
-00038c10: 2072 6574 7572 6e20 7461 626c 6573 0a0a   return tables..
-00038c20: 0a69 6620 636f 6e66 6967 2e44 4542 5547  .if config.DEBUG
-00038c30: 3a0a 2020 2020 7072 696e 7428 2752 6177  :.    print('Raw
-00038c40: 2073 6f75 7263 6573 206c 6f61 6465 6420   sources loaded 
-00038c50: 696e 207b 3a32 2e34 667d 2073 6563 6f6e  in {:2.4f} secon
-00038c60: 6473 272e 666f 726d 6174 2874 696d 652e  ds'.format(time.
-00038c70: 7469 6d65 2829 202d 2074 7429 290a 0a0a  time() - tt))...
-00038c80: 2325 2520 496d 706f 7274 2065 7861 6d70  #%% Import examp
-00038c90: 6c65 0a69 6620 5f5f 6e61 6d65 5f5f 203d  le.if __name__ =
-00038ca0: 3d20 275f 5f6d 6169 6e5f 5f27 3a0a 2020  = '__main__':.  
-00038cb0: 2020 2320 7864 6667 0a20 2020 2022 2222    # xdfg.    """
-00038cc0: 0a20 2020 2043 6f6e 6669 670a 2020 2020  .    Config.    
-00038cd0: 2222 220a 2020 2020 7570 6461 7465 5f63  """.    update_c
-00038ce0: 6f6e 7465 6e74 203d 2054 7275 650a 0a20  ontent = True.. 
-00038cf0: 2020 2022 2222 200a 2020 2020 496e 6974     """ .    Init
-00038d00: 6961 6c69 7a65 2063 6c61 7373 3a0a 2020  ialize class:.  
-00038d10: 2020 5468 6973 2077 696c 6c20 6c6f 6164    This will load
-00038d20: 2074 6865 206d 6170 7069 6e67 2066 696c   the mapping fil
-00038d30: 652c 2072 6561 6420 7468 6520 6461 7461  e, read the data
-00038d40: 2061 6e64 2070 7265 7061 7265 2074 6865   and prepare the
-00038d50: 2061 6464 6974 696f 6e61 6c0a 2020 2020   additional.    
-00038d60: 6d65 7461 2069 6e66 6f72 6d61 7469 6f6e  meta information
-00038d70: 732e 0a20 2020 2022 2222 0a20 2020 2023  s..    """.    #
-00038d80: 2072 6561 6465 7220 3d20 5052 494d 4150   reader = PRIMAP
-00038d90: 5f48 4953 5428 7665 7273 696f 6e3d 2276  _HIST(version="v
-00038da0: 322e 335f 6e6f 5f72 6f75 6e64 696e 675f  2.3_no_rounding_
-00038db0: 3238 5f4a 756c 5f32 3032 3122 2c20 7965  28_Jul_2021", ye
-00038dc0: 6172 3d32 3032 3129 0a20 2020 2023 2072  ar=2021).    # r
-00038dd0: 6561 6465 7220 3d20 5049 4b5f 4e44 4328  eader = PIK_NDC(
-00038de0: 3230 3231 2c20 7665 7273 696f 6e20 3d20  2021, version = 
-00038df0: 2776 312e 302e 3227 290a 2020 2020 2320  'v1.0.2').    # 
-00038e00: 7265 6164 6572 203d 2050 5249 4d41 5028  reader = PRIMAP(
-00038e10: 7965 6172 203d 2032 3032 3129 0a20 2020  year = 2021).   
-00038e20: 2023 2072 6561 6465 7220 3d20 4949 4153   # reader = IIAS
-00038e30: 4128 2745 4e47 4147 455f 3230 3231 272c  A('ENGAGE_2021',
-00038e40: 2027 656e 6761 6765 2729 0a20 2020 2023   'engage').    #
-00038e50: 2072 6561 6465 7220 3d20 4949 4153 4128   reader = IIASA(
-00038e60: 274e 4746 535f 3230 3231 272c 2027 6e67  'NGFS_2021', 'ng
-00038e70: 6673 5f32 2729 0a20 2020 2023 2072 6561  fs_2').    # rea
-00038e80: 6465 7220 3d20 4949 4153 4128 2743 445f  der = IIASA('CD_
-00038e90: 4c49 4e4b 5327 2c20 2763 646c 696e 6b73  LINKS', 'cdlinks
+000354f0: 7064 2e63 6f6e 6361 7428 5b73 656c 662e  pd.concat([self.
+00035500: 6d61 7070 696e 672c 2073 656c 662e 6176  mapping, self.av
+00035510: 6169 6c61 626c 6553 6572 6965 735d 2c20  ailableSeries], 
+00035520: 6178 6973 3d31 290a 2020 2020 2020 2020  axis=1).        
+00035530: 2320 2020 2020 2020 2073 656c 662e 6d61  #        self.ma
+00035540: 7070 696e 6720 3d20 7365 6c66 2e6d 6170  pping = self.map
+00035550: 7069 6e67 2e73 6f72 745f 696e 6465 7828  ping.sort_index(
+00035560: 290a 2020 2020 2020 2020 230a 2020 2020  ).        #.    
+00035570: 2020 2020 2320 2020 2020 2020 2073 656c      #        sel
+00035580: 662e 6d61 7070 696e 672e 746f 5f65 7863  f.mapping.to_exc
+00035590: 656c 2877 7269 7465 722c 2065 6e67 696e  el(writer, engin
+000355a0: 653d 276f 7065 6e70 7978 6c27 2c20 7368  e='openpyxl', sh
+000355b0: 6565 745f 6e61 6d65 3d27 6d6f 6465 6c5f  eet_name='model_
+000355c0: 6d61 7070 696e 6727 290a 0a20 2020 2020  mapping')..     
+000355d0: 2020 2023 2073 6365 6e61 7269 6f73 0a20     # scenarios. 
+000355e0: 2020 2020 2020 2069 6e64 6578 203d 206e         index = n
+000355f0: 702e 756e 6971 7565 2873 656c 662e 6461  p.unique(self.da
+00035600: 7461 5b73 656c 662e 7365 7475 702e 5343  ta[self.setup.SC
+00035610: 454e 4152 494f 5f43 4f4c 554d 4e5f 4e41  ENARIO_COLUMN_NA
+00035620: 4d45 5d2e 7661 6c75 6573 290a 0a20 2020  ME].values)..   
+00035630: 2020 2020 2073 656c 662e 6176 6169 6c61       self.availa
+00035640: 626c 6553 6572 6965 7320 3d20 7064 2e44  bleSeries = pd.D
+00035650: 6174 6146 7261 6d65 2869 6e64 6578 3d69  ataFrame(index=i
+00035660: 6e64 6578 290a 2020 2020 2020 2020 7365  ndex).        se
+00035670: 6c66 2e6d 6170 7069 6e67 203d 2070 642e  lf.mapping = pd.
+00035680: 4461 7461 4672 616d 6528 0a20 2020 2020  DataFrame(.     
+00035690: 2020 2020 2020 2069 6e64 6578 3d69 6e64         index=ind
+000356a0: 6578 2c20 636f 6c75 6d6e 733d 5b73 656c  ex, columns=[sel
+000356b0: 662e 7365 7475 702e 5343 454e 4152 494f  f.setup.SCENARIO
+000356c0: 5f43 4f4c 554d 4e5f 4e41 4d45 5d0a 2020  _COLUMN_NAME].  
+000356d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000356e0: 7365 6c66 2e6d 6170 7069 6e67 203d 2070  self.mapping = p
+000356f0: 642e 636f 6e63 6174 285b 7365 6c66 2e6d  d.concat([self.m
+00035700: 6170 7069 6e67 2c20 7365 6c66 2e61 7661  apping, self.ava
+00035710: 696c 6162 6c65 5365 7269 6573 5d2c 2061  ilableSeries], a
+00035720: 7869 733d 3129 0a20 2020 2020 2020 2073  xis=1).        s
+00035730: 656c 662e 6d61 7070 696e 6720 3d20 7365  elf.mapping = se
+00035740: 6c66 2e6d 6170 7069 6e67 2e73 6f72 745f  lf.mapping.sort_
+00035750: 696e 6465 7828 290a 2020 2020 2020 2020  index().        
+00035760: 7365 6c66 2e6d 6170 7069 6e67 2e74 6f5f  self.mapping.to_
+00035770: 6578 6365 6c28 7772 6974 6572 2c20 656e  excel(writer, en
+00035780: 6769 6e65 3d27 6f70 656e 7079 786c 272c  gine='openpyxl',
+00035790: 2073 6865 6574 5f6e 616d 653d 2773 6365   sheet_name='sce
+000357a0: 6e61 7269 6f5f 6d61 7070 696e 6727 290a  nario_mapping').
+000357b0: 0a20 2020 2020 2020 2023 2072 6567 696f  .        # regio
+000357c0: 6e0a 2020 2020 2020 2020 696e 6465 7820  n.        index 
+000357d0: 3d20 6e70 2e75 6e69 7175 6528 7365 6c66  = np.unique(self
+000357e0: 2e64 6174 615b 7365 6c66 2e73 6574 7570  .data[self.setup
+000357f0: 2e52 4547 494f 4e5f 434f 4c55 4d4e 5f4e  .REGION_COLUMN_N
+00035800: 414d 455d 2e76 616c 7565 7329 0a0a 2020  AME].values)..  
+00035810: 2020 2020 2020 7365 6c66 2e61 7661 696c        self.avail
+00035820: 6162 6c65 5365 7269 6573 203d 2070 642e  ableSeries = pd.
+00035830: 4461 7461 4672 616d 6528 696e 6465 783d  DataFrame(index=
+00035840: 696e 6465 7829 0a20 2020 2020 2020 2073  index).        s
+00035850: 656c 662e 6d61 7070 696e 6720 3d20 7064  elf.mapping = pd
+00035860: 2e44 6174 6146 7261 6d65 280a 2020 2020  .DataFrame(.    
+00035870: 2020 2020 2020 2020 696e 6465 783d 696e          index=in
+00035880: 6465 782c 2063 6f6c 756d 6e73 3d5b 7365  dex, columns=[se
+00035890: 6c66 2e73 6574 7570 2e52 4547 494f 4e5f  lf.setup.REGION_
+000358a0: 434f 4c55 4d4e 5f4e 414d 455d 0a20 2020  COLUMN_NAME].   
+000358b0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+000358c0: 656c 662e 6d61 7070 696e 6720 3d20 7064  elf.mapping = pd
+000358d0: 2e63 6f6e 6361 7428 5b73 656c 662e 6d61  .concat([self.ma
+000358e0: 7070 696e 672c 2073 656c 662e 6176 6169  pping, self.avai
+000358f0: 6c61 626c 6553 6572 6965 735d 2c20 6178  lableSeries], ax
+00035900: 6973 3d31 290a 2020 2020 2020 2020 7365  is=1).        se
+00035910: 6c66 2e6d 6170 7069 6e67 203d 2073 656c  lf.mapping = sel
+00035920: 662e 6d61 7070 696e 672e 736f 7274 5f69  f.mapping.sort_i
+00035930: 6e64 6578 2829 0a0a 2020 2020 2020 2020  ndex()..        
+00035940: 666f 7220 6964 7820 696e 2073 656c 662e  for idx in self.
+00035950: 6d61 7070 696e 672e 696e 6465 783a 0a20  mapping.index:. 
+00035960: 2020 2020 2020 2020 2020 2069 736f 203d             iso =
+00035970: 2064 742e 7574 696c 2e69 6465 6e74 6966   dt.util.identif
+00035980: 7943 6f75 6e74 7279 2869 6478 290a 2020  yCountry(idx).  
+00035990: 2020 2020 2020 2020 2020 6966 2069 736f            if iso
+000359a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000359b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000359c0: 6c66 2e6d 6170 7069 6e67 2e6c 6f63 5b69  lf.mapping.loc[i
+000359d0: 6478 2c20 2772 6567 696f 6e27 5d20 3d20  dx, 'region'] = 
+000359e0: 6973 6f0a 0a20 2020 2020 2020 2073 656c  iso..        sel
+000359f0: 662e 6d61 7070 696e 672e 746f 5f65 7863  f.mapping.to_exc
+00035a00: 656c 2877 7269 7465 722c 2065 6e67 696e  el(writer, engin
+00035a10: 653d 276f 7065 6e70 7978 6c27 2c20 7368  e='openpyxl', sh
+00035a20: 6565 745f 6e61 6d65 3d27 7265 6769 6f6e  eet_name='region
+00035a30: 5f6d 6170 7069 6e67 2729 0a20 2020 2020  _mapping').     
+00035a40: 2020 2077 7269 7465 722e 636c 6f73 6528     writer.close(
+00035a50: 290a 0a20 2020 2064 6566 2067 6174 6865  )..    def gathe
+00035a60: 724d 6170 7065 6444 6174 6128 7365 6c66  rMappedData(self
+00035a70: 2c20 7370 6174 6961 6c53 7562 5365 743d  , spatialSubSet=
+00035a80: 4e6f 6e65 2c20 7570 6461 7465 5461 626c  None, updateTabl
+00035a90: 6573 3d46 616c 7365 293a 0a0a 2020 2020  es=False):..    
+00035aa0: 2020 2020 696d 706f 7274 2074 7164 6d0a      import tqdm.
+00035ab0: 0a20 2020 2020 2020 2023 206c 6f61 6469  .        # loadi
+00035ac0: 6e67 2064 6174 6120 6966 206e 6563 6573  ng data if neces
+00035ad0: 7361 7279 0a20 2020 2020 2020 2069 6620  sary.        if 
+00035ae0: 6e6f 7420 6861 7361 7474 7228 7365 6c66  not hasattr(self
+00035af0: 2c20 2764 6174 6127 293a 0a20 2020 2020  , 'data'):.     
+00035b00: 2020 2020 2020 2073 656c 662e 6c6f 6164         self.load
+00035b10: 4461 7461 2829 0a0a 2020 2020 2020 2020  Data()..        
+00035b20: 7461 626c 6573 546f 436f 6d6d 6974 203d  tablesToCommit =
+00035b30: 205b 5d0a 2020 2020 2020 2020 6d65 7461   [].        meta
+00035b40: 4469 6374 203d 2064 6963 7428 290a 2020  Dict = dict().  
+00035b50: 2020 2020 2020 6d65 7461 4469 6374 5b27        metaDict['
+00035b60: 736f 7572 6365 275d 203d 2073 656c 662e  source'] = self.
+00035b70: 7365 7475 702e 534f 5552 4345 5f49 440a  setup.SOURCE_ID.
+00035b80: 2020 2020 2020 2020 6578 636c 7564 6564          excluded
+00035b90: 5461 626c 6573 203d 2064 6963 7428 290a  Tables = dict().
+00035ba0: 2020 2020 2020 2020 6578 636c 7564 6564          excluded
+00035bb0: 5461 626c 6573 5b27 656d 7074 7927 5d20  Tables['empty'] 
+00035bc0: 3d20 6c69 7374 2829 0a20 2020 2020 2020  = list().       
+00035bd0: 2065 7863 6c75 6465 6454 6162 6c65 735b   excludedTables[
+00035be0: 2765 7272 6f72 275d 203d 206c 6973 7428  'error'] = list(
+00035bf0: 290a 2020 2020 2020 2020 6578 636c 7564  ).        exclud
+00035c00: 6564 5461 626c 6573 5b27 6578 6973 7473  edTables['exists
+00035c10: 275d 203d 206c 6973 7428 290a 0a20 2020  '] = list()..   
+00035c20: 2020 2020 2023 2020 2020 2020 2020 7365       #        se
+00035c30: 6c66 2e64 6174 6120 3d20 7365 6c66 2e64  lf.data = self.d
+00035c40: 6174 610a 0a20 2020 2020 2020 2066 6f72  ata..        for
+00035c50: 2073 6365 6e61 7269 6f20 696e 2073 656c   scenario in sel
+00035c60: 662e 6d61 7070 696e 675b 2773 6365 6e61  f.mapping['scena
+00035c70: 7269 6f27 5d2e 6b65 7973 2829 3a0a 2020  rio'].keys():.  
+00035c80: 2020 2020 2020 2020 2020 7465 6d70 4d6f            tempMo
+00035c90: 5363 203d 2073 656c 662e 6461 7461 2e6c  Sc = self.data.l
+00035ca0: 6f63 5b73 656c 662e 6461 7461 2e73 6365  oc[self.data.sce
+00035cb0: 6e61 7269 6f20 3d3d 2073 6365 6e61 7269  nario == scenari
+00035cc0: 6f5d 0a20 2020 2020 2020 2020 2020 2066  o].            f
+00035cd0: 6f72 2076 6172 6961 626c 6520 696e 2073  or variable in s
+00035ce0: 656c 662e 6d61 7070 696e 675b 2765 6e74  elf.mapping['ent
+00035cf0: 6974 7927 5d2e 6b65 7973 2829 3a0a 2020  ity'].keys():.  
+00035d00: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00035d10: 6d70 4d6f 5363 5661 203d 2074 656d 704d  mpMoScVa = tempM
+00035d20: 6f53 632e 6c6f 635b 7465 6d70 4d6f 5363  oSc.loc[tempMoSc
+00035d30: 2e76 6172 6961 626c 6520 3d3d 2076 6172  .variable == var
+00035d40: 6961 626c 655d 0a20 2020 2020 2020 2020  iable].         
+00035d50: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+00035d60: 2020 2020 2020 2020 666f 7220 6361 7465          for cate
+00035d70: 676f 7279 2069 6e20 7365 6c66 2e6d 6170  gory in self.map
+00035d80: 7069 6e67 5b27 6361 7465 676f 7279 275d  ping['category']
+00035d90: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
+00035da0: 2020 2020 2020 2020 2023 2020 2020 2020           #      
+00035db0: 2020 2020 2020 2020 2020 7465 6d70 4d6f            tempMo
+00035dc0: 5363 5661 203d 2074 656d 704d 6f53 6356  ScVa = tempMoScV
+00035dd0: 612e 6c6f 635b 7465 6d70 4d6f 5363 5661  a.loc[tempMoScVa
+00035de0: 2e76 6172 6961 626c 6520 3d3d 2063 6174  .variable == cat
+00035df0: 6567 6f72 795d 0a20 2020 2020 2020 2020  egory].         
+00035e00: 2020 2020 2020 2074 656d 704d 6f53 6356         tempMoScV
+00035e10: 6120 3d20 7465 6d70 4d6f 5363 5661 2e6c  a = tempMoScVa.l
+00035e20: 6f63 5b0a 2020 2020 2020 2020 2020 2020  oc[.            
+00035e30: 2020 2020 2020 2020 3a2c 0a20 2020 2020          :,.     
+00035e40: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00035e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00035e60: 2020 2020 2020 2020 2027 756e 6974 272c           'unit',
+00035e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00035e80: 2020 2020 2020 2020 2027 6d6f 6465 6c27           'model'
+00035e90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00035ea0: 2020 2020 2020 2020 2020 2773 6365 6e61            'scena
+00035eb0: 7269 6f27 2c0a 2020 2020 2020 2020 2020  rio',.          
+00035ec0: 2020 2020 2020 2020 2020 2020 2020 2779                'y
+00035ed0: 6561 7227 2c0a 2020 2020 2020 2020 2020  ear',.          
+00035ee0: 2020 2020 2020 2020 2020 2020 2020 2772                'r
+00035ef0: 6567 696f 6e27 2c0a 2020 2020 2020 2020  egion',.        
+00035f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035f10: 2776 616c 7565 272c 0a20 2020 2020 2020  'value',.       
+00035f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035f30: 2027 7661 7269 6162 6c65 272c 0a20 2020   'variable',.   
+00035f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035f50: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
+00035f60: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+00035f70: 2020 2020 2020 7465 6d70 4d6f 5363 5661        tempMoScVa
+00035f80: 2e6c 6f63 5b3a 2c20 2775 6e69 7427 5d20  .loc[:, 'unit'] 
+00035f90: 3d20 7365 6c66 2e6d 6170 7069 6e67 5b27  = self.mapping['
+00035fa0: 756e 6974 275d 5b76 6172 6961 626c 655d  unit'][variable]
+00035fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00035fc0: 2074 656d 704d 6f53 6356 612e 6c6f 635b   tempMoScVa.loc[
+00035fd0: 3a2c 2027 7363 656e 6172 696f 275d 203d  :, 'scenario'] =
+00035fe0: 2073 656c 662e 6d61 7070 696e 675b 2773   self.mapping['s
+00035ff0: 6365 6e61 7269 6f27 5d5b 7363 656e 6172  cenario'][scenar
+00036000: 696f 5d0a 2020 2020 2020 2020 2020 2020  io].            
+00036010: 2020 2020 2323 2020 2020 2020 2020 2020      ##          
+00036020: 2020 2020 2020 2020 2020 6466 670a 2020            dfg.  
+00036030: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+00036040: 626c 6573 203d 2064 742e 696e 7465 7266  bles = dt.interf
+00036050: 6163 6573 2e72 6561 645f 6c6f 6e67 5f74  aces.read_long_t
+00036060: 6162 6c65 2874 656d 704d 6f53 6356 612c  able(tempMoScVa,
+00036070: 205b 7661 7269 6162 6c65 5d29 0a20 2020   [variable]).   
+00036080: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00036090: 2074 6162 6c65 2069 6e20 7461 626c 6573   table in tables
+000360a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000360b0: 2020 2020 2020 7461 626c 652e 6d65 7461        table.meta
+000360c0: 5b27 656e 7469 7479 275d 203d 2073 656c  ['entity'] = sel
+000360d0: 662e 6d61 7070 696e 675b 2765 6e74 6974  f.mapping['entit
+000360e0: 7927 5d5b 7661 7269 6162 6c65 5d0a 2020  y'][variable].  
+000360f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00036100: 2020 7461 626c 652e 6d65 7461 5b27 6361    table.meta['ca
+00036110: 7465 676f 7279 275d 203d 2073 656c 662e  tegory'] = self.
+00036120: 6d61 7070 696e 675b 2763 6174 6567 6f72  mapping['categor
+00036130: 7927 5d5b 7661 7269 6162 6c65 5d0a 2020  y'][variable].  
+00036140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00036150: 2020 7461 626c 652e 6d65 7461 5b27 7363    table.meta['sc
+00036160: 656e 6172 696f 275d 203d 2073 656c 662e  enario'] = self.
+00036170: 6d61 7070 696e 675b 2773 6365 6e61 7269  mapping['scenari
+00036180: 6f27 5d5b 7363 656e 6172 696f 5d0a 2020  o'][scenario].  
+00036190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000361a0: 2020 7461 626c 652e 6d65 7461 5b27 736f    table.meta['so
+000361b0: 7572 6365 275d 203d 2073 656c 662e 7365  urce'] = self.se
+000361c0: 7475 702e 534f 5552 4345 5f49 440a 2020  tup.SOURCE_ID.  
+000361d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000361e0: 2020 7461 626c 652e 696e 6465 7820 3d20    table.index = 
+000361f0: 7461 626c 652e 696e 6465 782e 6d61 7028  table.index.map(
+00036200: 7365 6c66 2e6d 6170 7069 6e67 5b27 7265  self.mapping['re
+00036210: 6769 6f6e 275d 290a 0a20 2020 2020 2020  gion'])..       
+00036220: 2020 2020 2020 2020 2020 2020 2074 6162               tab
+00036230: 6c65 4944 203d 2074 6162 6c65 2e67 656e  leID = table.gen
+00036240: 6572 6174 6554 6162 6c65 4944 2829 0a20  erateTableID(). 
+00036250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00036260: 2020 2069 6620 6e6f 7420 7570 6461 7465     if not update
+00036270: 5461 626c 6573 3a0a 2020 2020 2020 2020  Tables:.        
+00036280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00036290: 6966 2064 742e 636f 7265 2e44 422e 7461  if dt.core.DB.ta
+000362a0: 626c 6545 7869 7374 2874 6162 6c65 4944  bleExist(tableID
+000362b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000362c0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000362d0: 7863 6c75 6465 6454 6162 6c65 735b 2765  xcludedTables['e
+000362e0: 7869 7374 7327 5d2e 6170 7065 6e64 2874  xists'].append(t
+000362f0: 6162 6c65 4944 290a 2020 2020 2020 2020  ableID).        
+00036300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00036310: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00036320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00036330: 2020 7461 626c 6573 546f 436f 6d6d 6974    tablesToCommit
+00036340: 2e61 7070 656e 6428 7461 626c 6529 0a20  .append(table). 
+00036350: 2020 2020 2020 2072 6574 7572 6e20 7461         return ta
+00036360: 626c 6573 546f 436f 6d6d 6974 2c20 6578  blesToCommit, ex
+00036370: 636c 7564 6564 5461 626c 6573 0a0a 0a23  cludedTables...#
+00036380: 2525 2049 6d70 6f72 7420 6675 6e63 7469  %% Import functi
+00036390: 6f6e 730a 0a0a 6465 6620 4844 495f 696d  ons...def HDI_im
+000363a0: 706f 7274 2879 6561 723d 3230 3230 293a  port(year=2020):
+000363b0: 0a20 2020 2073 6f75 7263 654d 6574 6120  .    sourceMeta 
+000363c0: 3d20 7b0a 2020 2020 2020 2020 2753 4f55  = {.        'SOU
+000363d0: 5243 455f 4944 273a 2027 4844 495f 2720  RCE_ID': 'HDI_' 
+000363e0: 2b20 7374 7228 7965 6172 292c 0a20 2020  + str(year),.   
+000363f0: 2020 2020 2027 636f 6c6c 6563 7465 645f       'collected_
+00036400: 6279 273a 2027 4147 272c 0a20 2020 2020  by': 'AG',.     
+00036410: 2020 2027 6461 7465 273a 2064 742e 636f     'date': dt.co
+00036420: 7265 2e67 6574 5f64 6174 655f 7374 7269  re.get_date_stri
+00036430: 6e67 2829 2c0a 2020 2020 2020 2020 2773  ng(),.        's
+00036440: 6f75 7263 655f 7572 6c27 3a20 2768 7474  ource_url': 'htt
+00036450: 703a 2f2f 6864 722e 756e 6470 2e6f 7267  p://hdr.undp.org
+00036460: 2f65 6e2f 6461 7461 272c 0a20 2020 2020  /en/data',.     
+00036470: 2020 2027 6c69 6365 6e63 6527 3a20 276f     'licence': 'o
+00036480: 7065 6e20 736f 7572 6365 272c 0a20 2020  pen source',.   
+00036490: 207d 0a0a 2020 2020 534f 5552 4345 5f50   }..    SOURCE_P
+000364a0: 4154 4820 3d20 6f73 2e70 6174 682e 6a6f  ATH = os.path.jo
+000364b0: 696e 280a 2020 2020 2020 2020 6474 2e63  in(.        dt.c
+000364c0: 6f6e 6669 672e 5041 5448 5f54 4f5f 4441  onfig.PATH_TO_DA
+000364d0: 5441 5348 454c 462c 2027 7261 7764 6174  TASHELF, 'rawdat
+000364e0: 6127 2c20 736f 7572 6365 4d65 7461 5b27  a', sourceMeta['
+000364f0: 534f 5552 4345 5f49 4427 5d0a 2020 2020  SOURCE_ID'].    
+00036500: 290a 2020 2020 6461 7461 203d 2070 642e  ).    data = pd.
+00036510: 7265 6164 5f63 7376 280a 2020 2020 2020  read_csv(.      
+00036520: 2020 6f73 2e70 6174 682e 6a6f 696e 2853    os.path.join(S
+00036530: 4f55 5243 455f 5041 5448 2c20 2248 756d  OURCE_PATH, "Hum
+00036540: 616e 2044 6576 656c 6f70 6d65 6e74 2049  an Development I
+00036550: 6e64 6578 2028 4844 4929 2e63 7376 2229  ndex (HDI).csv")
+00036560: 2c0a 2020 2020 2020 2020 6e61 5f76 616c  ,.        na_val
+00036570: 7565 733d 272e 2e27 2c0a 2020 2020 290a  ues='..',.    ).
+00036580: 0a20 2020 2079 6561 7243 6f6c 756d 6e73  .    yearColumns
+00036590: 203d 2064 742e 7574 696c 2e79 6561 7273   = dt.util.years
+000365a0: 436f 6c75 6d6e 734f 6e6c 7928 6461 7461  ColumnsOnly(data
+000365b0: 290a 0a20 2020 2064 6174 6120 3d20 6461  )..    data = da
+000365c0: 7461 2e6c 6f63 5b3a 2c20 5b27 436f 756e  ta.loc[:, ['Coun
+000365d0: 7472 7927 5d20 2b20 7965 6172 436f 6c75  try'] + yearColu
+000365e0: 6d6e 735d 0a0a 2020 2020 2320 2020 2072  mns]..    #    r
+000365f0: 6567 696f 6e4d 6170 7069 6e67 203d 207b  egionMapping = {
+00036600: 783a 7920 666f 7220 782c 7920 696e 207a  x:y for x,y in z
+00036610: 6970 286c 6973 7428 6461 7461 2e6c 6f63  ip(list(data.loc
+00036620: 5b3a 2c27 436f 756e 7472 7927 5d29 2c20  [:,'Country']), 
+00036630: 6c69 7374 2864 6174 612e 6c6f 635b 3a2c  list(data.loc[:,
+00036640: 2743 6f75 6e74 7279 275d 2e6d 6170 286c  'Country'].map(l
+00036650: 616d 6264 6120 7820 3a20 6474 2e67 6574  ambda x : dt.get
+00036660: 436f 756e 7472 7949 534f 2873 7472 2878  CountryISO(str(x
+00036670: 2929 2929 297d 0a20 2020 2072 6567 696f  )))))}.    regio
+00036680: 6e4d 6170 7069 6e67 203d 207b 0a20 2020  nMapping = {.   
+00036690: 2020 2020 2027 2041 6667 6861 6e69 7374       ' Afghanist
+000366a0: 616e 273a 2027 4146 4727 2c0a 2020 2020  an': 'AFG',.    
+000366b0: 2020 2020 2720 416c 6261 6e69 6127 3a20      ' Albania': 
+000366c0: 2741 4c42 272c 0a20 2020 2020 2020 2027  'ALB',.        '
+000366d0: 2041 6c67 6572 6961 273a 2027 445a 4127   Algeria': 'DZA'
+000366e0: 2c0a 2020 2020 2020 2020 2720 416e 646f  ,.        ' Ando
+000366f0: 7272 6127 3a20 2741 4e44 272c 0a20 2020  rra': 'AND',.   
+00036700: 2020 2020 2027 2041 6e67 6f6c 6127 3a20       ' Angola': 
+00036710: 2741 474f 272c 0a20 2020 2020 2020 2027  'AGO',.        '
+00036720: 2041 6e74 6967 7561 2061 6e64 2042 6172   Antigua and Bar
+00036730: 6275 6461 273a 2027 4154 4727 2c0a 2020  buda': 'ATG',.  
+00036740: 2020 2020 2020 2720 4172 6765 6e74 696e        ' Argentin
+00036750: 6127 3a20 2741 5247 272c 0a20 2020 2020  a': 'ARG',.     
+00036760: 2020 2027 2041 726d 656e 6961 273a 2027     ' Armenia': '
+00036770: 4152 4d27 2c0a 2020 2020 2020 2020 2720  ARM',.        ' 
+00036780: 4175 7374 7261 6c69 6127 3a20 2741 5553  Australia': 'AUS
+00036790: 272c 0a20 2020 2020 2020 2027 2041 7573  ',.        ' Aus
+000367a0: 7472 6961 273a 2027 4155 5427 2c0a 2020  tria': 'AUT',.  
+000367b0: 2020 2020 2020 2720 417a 6572 6261 696a        ' Azerbaij
+000367c0: 616e 273a 2027 415a 4527 2c0a 2020 2020  an': 'AZE',.    
+000367d0: 2020 2020 2720 4261 6861 6d61 7327 3a20      ' Bahamas': 
+000367e0: 2742 4853 272c 0a20 2020 2020 2020 2027  'BHS',.        '
+000367f0: 2042 6168 7261 696e 273a 2027 4248 5227   Bahrain': 'BHR'
+00036800: 2c0a 2020 2020 2020 2020 2720 4261 6e67  ,.        ' Bang
+00036810: 6c61 6465 7368 273a 2027 4247 4427 2c0a  ladesh': 'BGD',.
+00036820: 2020 2020 2020 2020 2720 4261 7262 6164          ' Barbad
+00036830: 6f73 273a 2027 4252 4227 2c0a 2020 2020  os': 'BRB',.    
+00036840: 2020 2020 2720 4265 6c61 7275 7327 3a20      ' Belarus': 
+00036850: 2742 4c52 272c 0a20 2020 2020 2020 2027  'BLR',.        '
+00036860: 2042 656c 6769 756d 273a 2027 4245 4c27   Belgium': 'BEL'
+00036870: 2c0a 2020 2020 2020 2020 2720 4265 6c69  ,.        ' Beli
+00036880: 7a65 273a 2027 424c 5a27 2c0a 2020 2020  ze': 'BLZ',.    
+00036890: 2020 2020 2720 4265 6e69 6e27 3a20 2742      ' Benin': 'B
+000368a0: 454e 272c 0a20 2020 2020 2020 2027 2042  EN',.        ' B
+000368b0: 6875 7461 6e27 3a20 2742 544e 272c 0a20  hutan': 'BTN',. 
+000368c0: 2020 2020 2020 2027 2042 6f6c 6976 6961         ' Bolivia
+000368d0: 2028 506c 7572 696e 6174 696f 6e61 6c20   (Plurinational 
+000368e0: 5374 6174 6520 6f66 2927 3a20 2742 4f4c  State of)': 'BOL
+000368f0: 272c 0a20 2020 2020 2020 2027 2042 6f73  ',.        ' Bos
+00036900: 6e69 6120 616e 6420 4865 727a 6567 6f76  nia and Herzegov
+00036910: 696e 6127 3a20 2742 4948 272c 0a20 2020  ina': 'BIH',.   
+00036920: 2020 2020 2027 2042 6f74 7377 616e 6127       ' Botswana'
+00036930: 3a20 2742 5741 272c 0a20 2020 2020 2020  : 'BWA',.       
+00036940: 2027 2042 7261 7a69 6c27 3a20 2742 5241   ' Brazil': 'BRA
+00036950: 272c 0a20 2020 2020 2020 2027 2042 7275  ',.        ' Bru
+00036960: 6e65 6920 4461 7275 7373 616c 616d 273a  nei Darussalam':
+00036970: 2027 4252 4e27 2c0a 2020 2020 2020 2020   'BRN',.        
+00036980: 2720 4275 6c67 6172 6961 273a 2027 4247  ' Bulgaria': 'BG
+00036990: 5227 2c0a 2020 2020 2020 2020 2720 4275  R',.        ' Bu
+000369a0: 726b 696e 6120 4661 736f 273a 2027 4246  rkina Faso': 'BF
+000369b0: 4127 2c0a 2020 2020 2020 2020 2720 4275  A',.        ' Bu
+000369c0: 7275 6e64 6927 3a20 2742 4449 272c 0a20  rundi': 'BDI',. 
+000369d0: 2020 2020 2020 2027 2043 6162 6f20 5665         ' Cabo Ve
+000369e0: 7264 6527 3a20 2743 5056 272c 0a20 2020  rde': 'CPV',.   
+000369f0: 2020 2020 2027 2043 616d 626f 6469 6127       ' Cambodia'
+00036a00: 3a20 274b 484d 272c 0a20 2020 2020 2020  : 'KHM',.       
+00036a10: 2027 2043 616d 6572 6f6f 6e27 3a20 2743   ' Cameroon': 'C
+00036a20: 4d52 272c 0a20 2020 2020 2020 2027 2043  MR',.        ' C
+00036a30: 616e 6164 6127 3a20 2743 414e 272c 0a20  anada': 'CAN',. 
+00036a40: 2020 2020 2020 2027 2043 656e 7472 616c         ' Central
+00036a50: 2041 6672 6963 616e 2052 6570 7562 6c69   African Republi
+00036a60: 6327 3a20 2743 4146 272c 0a20 2020 2020  c': 'CAF',.     
+00036a70: 2020 2027 2043 6861 6427 3a20 2754 4344     ' Chad': 'TCD
+00036a80: 272c 0a20 2020 2020 2020 2027 2043 6869  ',.        ' Chi
+00036a90: 6c65 273a 2027 4348 4c27 2c0a 2020 2020  le': 'CHL',.    
+00036aa0: 2020 2020 2720 4368 696e 6127 3a20 2743      ' China': 'C
+00036ab0: 484e 272c 0a20 2020 2020 2020 2027 2043  HN',.        ' C
+00036ac0: 6f6c 6f6d 6269 6127 3a20 2743 4f4c 272c  olombia': 'COL',
+00036ad0: 0a20 2020 2020 2020 2027 2043 6f6d 6f72  .        ' Comor
+00036ae0: 6f73 273a 2027 434f 4d27 2c0a 2020 2020  os': 'COM',.    
+00036af0: 2020 2020 2720 436f 6e67 6f27 3a20 2743      ' Congo': 'C
+00036b00: 4f47 272c 0a20 2020 2020 2020 2027 2043  OG',.        ' C
+00036b10: 6f6e 676f 2028 4465 6d6f 6372 6174 6963  ongo (Democratic
+00036b20: 2052 6570 7562 6c69 6320 6f66 2074 6865   Republic of the
+00036b30: 2927 3a20 2743 4f44 272c 0a20 2020 2020  )': 'COD',.     
+00036b40: 2020 2027 2043 6f73 7461 2052 6963 6127     ' Costa Rica'
+00036b50: 3a20 2743 5249 272c 0a20 2020 2020 2020  : 'CRI',.       
+00036b60: 2027 2043 726f 6174 6961 273a 2027 4852   ' Croatia': 'HR
+00036b70: 5627 2c0a 2020 2020 2020 2020 2720 4375  V',.        ' Cu
+00036b80: 6261 273a 2027 4355 4227 2c0a 2020 2020  ba': 'CUB',.    
+00036b90: 2020 2020 2720 4379 7072 7573 273a 2027      ' Cyprus': '
+00036ba0: 4359 5027 2c0a 2020 2020 2020 2020 2720  CYP',.        ' 
+00036bb0: 437a 6563 6869 6127 3a20 2743 5a45 272c  Czechia': 'CZE',
+00036bc0: 0a20 2020 2020 2020 2022 2043 c3b4 7465  .        " C..te
+00036bd0: 2064 2749 766f 6972 6522 3a20 2743 4956   d'Ivoire": 'CIV
+00036be0: 272c 0a20 2020 2020 2020 2027 2044 656e  ',.        ' Den
+00036bf0: 6d61 726b 273a 2027 444e 4b27 2c0a 2020  mark': 'DNK',.  
+00036c00: 2020 2020 2020 2720 446a 6962 6f75 7469        ' Djibouti
+00036c10: 273a 2027 444a 4927 2c0a 2020 2020 2020  ': 'DJI',.      
+00036c20: 2020 2720 446f 6d69 6e69 6361 273a 2027    ' Dominica': '
+00036c30: 444d 4127 2c0a 2020 2020 2020 2020 2720  DMA',.        ' 
+00036c40: 446f 6d69 6e69 6361 6e20 5265 7075 626c  Dominican Republ
+00036c50: 6963 273a 2027 444f 4d27 2c0a 2020 2020  ic': 'DOM',.    
+00036c60: 2020 2020 2720 4563 7561 646f 7227 3a20      ' Ecuador': 
+00036c70: 2745 4355 272c 0a20 2020 2020 2020 2027  'ECU',.        '
+00036c80: 2045 6779 7074 273a 2027 4547 5927 2c0a   Egypt': 'EGY',.
+00036c90: 2020 2020 2020 2020 2720 456c 2053 616c          ' El Sal
+00036ca0: 7661 646f 7227 3a20 2753 4c56 272c 0a20  vador': 'SLV',. 
+00036cb0: 2020 2020 2020 2027 2045 7175 6174 6f72         ' Equator
+00036cc0: 6961 6c20 4775 696e 6561 273a 2027 474e  ial Guinea': 'GN
+00036cd0: 5127 2c0a 2020 2020 2020 2020 2720 4572  Q',.        ' Er
+00036ce0: 6974 7265 6127 3a20 2745 5249 272c 0a20  itrea': 'ERI',. 
+00036cf0: 2020 2020 2020 2027 2045 7374 6f6e 6961         ' Estonia
+00036d00: 273a 2027 4553 5427 2c0a 2020 2020 2020  ': 'EST',.      
+00036d10: 2020 2720 4573 7761 7469 6e69 2028 4b69    ' Eswatini (Ki
+00036d20: 6e67 646f 6d20 6f66 2927 3a20 2753 575a  ngdom of)': 'SWZ
+00036d30: 272c 0a20 2020 2020 2020 2027 2045 7468  ',.        ' Eth
+00036d40: 696f 7069 6127 3a20 2745 5448 272c 0a20  iopia': 'ETH',. 
+00036d50: 2020 2020 2020 2027 2046 696a 6927 3a20         ' Fiji': 
+00036d60: 2746 4a49 272c 0a20 2020 2020 2020 2027  'FJI',.        '
+00036d70: 2046 696e 6c61 6e64 273a 2027 4649 4e27   Finland': 'FIN'
+00036d80: 2c0a 2020 2020 2020 2020 2720 4672 616e  ,.        ' Fran
+00036d90: 6365 273a 2027 4652 4127 2c0a 2020 2020  ce': 'FRA',.    
+00036da0: 2020 2020 2720 4761 626f 6e27 3a20 2747      ' Gabon': 'G
+00036db0: 4142 272c 0a20 2020 2020 2020 2027 2047  AB',.        ' G
+00036dc0: 616d 6269 6127 3a20 2747 4d42 272c 0a20  ambia': 'GMB',. 
+00036dd0: 2020 2020 2020 2027 2047 656f 7267 6961         ' Georgia
+00036de0: 273a 2027 4745 4f27 2c0a 2020 2020 2020  ': 'GEO',.      
+00036df0: 2020 2720 4765 726d 616e 7927 3a20 2744    ' Germany': 'D
+00036e00: 4555 272c 0a20 2020 2020 2020 2027 2047  EU',.        ' G
+00036e10: 6861 6e61 273a 2027 4748 4127 2c0a 2020  hana': 'GHA',.  
+00036e20: 2020 2020 2020 2720 4772 6565 6365 273a        ' Greece':
+00036e30: 2027 4752 4327 2c0a 2020 2020 2020 2020   'GRC',.        
+00036e40: 2720 4772 656e 6164 6127 3a20 2747 5244  ' Grenada': 'GRD
+00036e50: 272c 0a20 2020 2020 2020 2027 2047 7561  ',.        ' Gua
+00036e60: 7465 6d61 6c61 273a 2027 4754 4d27 2c0a  temala': 'GTM',.
+00036e70: 2020 2020 2020 2020 2720 4775 696e 6561          ' Guinea
+00036e80: 273a 2027 4749 4e27 2c0a 2020 2020 2020  ': 'GIN',.      
+00036e90: 2020 2720 4775 696e 6561 2d42 6973 7361    ' Guinea-Bissa
+00036ea0: 7527 3a20 2747 4e42 272c 0a20 2020 2020  u': 'GNB',.     
+00036eb0: 2020 2027 2047 7579 616e 6127 3a20 2747     ' Guyana': 'G
+00036ec0: 5559 272c 0a20 2020 2020 2020 2027 2048  UY',.        ' H
+00036ed0: 6169 7469 273a 2027 4854 4927 2c0a 2020  aiti': 'HTI',.  
+00036ee0: 2020 2020 2020 2720 486f 6e64 7572 6173        ' Honduras
+00036ef0: 273a 2027 484e 4427 2c0a 2020 2020 2020  ': 'HND',.      
+00036f00: 2020 2720 486f 6e67 204b 6f6e 672c 2043    ' Hong Kong, C
+00036f10: 6869 6e61 2028 5341 5229 273a 2027 484b  hina (SAR)': 'HK
+00036f20: 4727 2c0a 2020 2020 2020 2020 2720 4875  G',.        ' Hu
+00036f30: 6e67 6172 7927 3a20 2748 554e 272c 0a20  ngary': 'HUN',. 
+00036f40: 2020 2020 2020 2027 2049 6365 6c61 6e64         ' Iceland
+00036f50: 273a 2027 4953 4c27 2c0a 2020 2020 2020  ': 'ISL',.      
+00036f60: 2020 2720 496e 6469 6127 3a20 2749 4e44    ' India': 'IND
+00036f70: 272c 0a20 2020 2020 2020 2027 2049 6e64  ',.        ' Ind
+00036f80: 6f6e 6573 6961 273a 2027 4944 4e27 2c0a  onesia': 'IDN',.
+00036f90: 2020 2020 2020 2020 2720 4972 616e 2028          ' Iran (
+00036fa0: 4973 6c61 6d69 6320 5265 7075 626c 6963  Islamic Republic
+00036fb0: 206f 6629 273a 2027 4952 4e27 2c0a 2020   of)': 'IRN',.  
+00036fc0: 2020 2020 2020 2720 4972 6171 273a 2027        ' Iraq': '
+00036fd0: 4952 5127 2c0a 2020 2020 2020 2020 2720  IRQ',.        ' 
+00036fe0: 4972 656c 616e 6427 3a20 2749 524c 272c  Ireland': 'IRL',
+00036ff0: 0a20 2020 2020 2020 2027 2049 7372 6165  .        ' Israe
+00037000: 6c27 3a20 2749 5352 272c 0a20 2020 2020  l': 'ISR',.     
+00037010: 2020 2027 2049 7461 6c79 273a 2027 4954     ' Italy': 'IT
+00037020: 4127 2c0a 2020 2020 2020 2020 2720 4a61  A',.        ' Ja
+00037030: 6d61 6963 6127 3a20 274a 414d 272c 0a20  maica': 'JAM',. 
+00037040: 2020 2020 2020 2027 204a 6170 616e 273a         ' Japan':
+00037050: 2027 4a50 4e27 2c0a 2020 2020 2020 2020   'JPN',.        
+00037060: 2720 4a6f 7264 616e 273a 2027 4a4f 5227  ' Jordan': 'JOR'
+00037070: 2c0a 2020 2020 2020 2020 2720 4b61 7a61  ,.        ' Kaza
+00037080: 6b68 7374 616e 273a 2027 4b41 5a27 2c0a  khstan': 'KAZ',.
+00037090: 2020 2020 2020 2020 2720 4b65 6e79 6127          ' Kenya'
+000370a0: 3a20 274b 454e 272c 0a20 2020 2020 2020  : 'KEN',.       
+000370b0: 2027 204b 6972 6962 6174 6927 3a20 274b   ' Kiribati': 'K
+000370c0: 4952 272c 0a20 2020 2020 2020 2027 204b  IR',.        ' K
+000370d0: 6f72 6561 2028 5265 7075 626c 6963 206f  orea (Republic o
+000370e0: 6629 273a 2027 4b4f 5227 2c0a 2020 2020  f)': 'KOR',.    
+000370f0: 2020 2020 2720 4b75 7761 6974 273a 2027      ' Kuwait': '
+00037100: 4b57 5427 2c0a 2020 2020 2020 2020 2720  KWT',.        ' 
+00037110: 4b79 7267 797a 7374 616e 273a 2027 4b47  Kyrgyzstan': 'KG
+00037120: 5a27 2c0a 2020 2020 2020 2020 2220 4c61  Z',.        " La
+00037130: 6f20 5065 6f70 6c65 2773 2044 656d 6f63  o People's Democ
+00037140: 7261 7469 6320 5265 7075 626c 6963 223a  ratic Republic":
+00037150: 2027 4c41 4f27 2c0a 2020 2020 2020 2020   'LAO',.        
+00037160: 2720 4c61 7476 6961 273a 2027 4c56 4127  ' Latvia': 'LVA'
+00037170: 2c0a 2020 2020 2020 2020 2720 4c65 6261  ,.        ' Leba
+00037180: 6e6f 6e27 3a20 274c 424e 272c 0a20 2020  non': 'LBN',.   
+00037190: 2020 2020 2027 204c 6573 6f74 686f 273a       ' Lesotho':
+000371a0: 2027 4c53 4f27 2c0a 2020 2020 2020 2020   'LSO',.        
+000371b0: 2720 4c69 6265 7269 6127 3a20 274c 4252  ' Liberia': 'LBR
+000371c0: 272c 0a20 2020 2020 2020 2027 204c 6962  ',.        ' Lib
+000371d0: 7961 273a 2027 4c42 5927 2c0a 2020 2020  ya': 'LBY',.    
+000371e0: 2020 2020 2720 4c69 6563 6874 656e 7374      ' Liechtenst
+000371f0: 6569 6e27 3a20 274c 4945 272c 0a20 2020  ein': 'LIE',.   
+00037200: 2020 2020 2027 204c 6974 6875 616e 6961       ' Lithuania
+00037210: 273a 2027 4c54 5527 2c0a 2020 2020 2020  ': 'LTU',.      
+00037220: 2020 2720 4c75 7865 6d62 6f75 7267 273a    ' Luxembourg':
+00037230: 2027 4c55 5827 2c0a 2020 2020 2020 2020   'LUX',.        
+00037240: 2720 4d61 6461 6761 7363 6172 273a 2027  ' Madagascar': '
+00037250: 4d44 4727 2c0a 2020 2020 2020 2020 2720  MDG',.        ' 
+00037260: 4d61 6c61 7769 273a 2027 4d57 4927 2c0a  Malawi': 'MWI',.
+00037270: 2020 2020 2020 2020 2720 4d61 6c61 7973          ' Malays
+00037280: 6961 273a 2027 4d59 5327 2c0a 2020 2020  ia': 'MYS',.    
+00037290: 2020 2020 2720 4d61 6c64 6976 6573 273a      ' Maldives':
+000372a0: 2027 4d44 5627 2c0a 2020 2020 2020 2020   'MDV',.        
+000372b0: 2720 4d61 6c69 273a 2027 4d4c 4927 2c0a  ' Mali': 'MLI',.
+000372c0: 2020 2020 2020 2020 2720 4d61 6c74 6127          ' Malta'
+000372d0: 3a20 274d 4c54 272c 0a20 2020 2020 2020  : 'MLT',.       
+000372e0: 2027 204d 6172 7368 616c 6c20 4973 6c61   ' Marshall Isla
+000372f0: 6e64 7327 3a20 274d 484c 272c 0a20 2020  nds': 'MHL',.   
+00037300: 2020 2020 2027 204d 6175 7269 7461 6e69       ' Mauritani
+00037310: 6127 3a20 274d 5254 272c 0a20 2020 2020  a': 'MRT',.     
+00037320: 2020 2027 204d 6175 7269 7469 7573 273a     ' Mauritius':
+00037330: 2027 4d55 5327 2c0a 2020 2020 2020 2020   'MUS',.        
+00037340: 2720 4d65 7869 636f 273a 2027 4d45 5827  ' Mexico': 'MEX'
+00037350: 2c0a 2020 2020 2020 2020 2720 4d69 6372  ,.        ' Micr
+00037360: 6f6e 6573 6961 2028 4665 6465 7261 7465  onesia (Federate
+00037370: 6420 5374 6174 6573 206f 6629 273a 2027  d States of)': '
+00037380: 4653 4d27 2c0a 2020 2020 2020 2020 2720  FSM',.        ' 
+00037390: 4d6f 6c64 6f76 6120 2852 6570 7562 6c69  Moldova (Republi
+000373a0: 6320 6f66 2927 3a20 274d 4441 272c 0a20  c of)': 'MDA',. 
+000373b0: 2020 2020 2020 2027 204d 6f6e 676f 6c69         ' Mongoli
+000373c0: 6127 3a20 274d 4e47 272c 0a20 2020 2020  a': 'MNG',.     
+000373d0: 2020 2027 204d 6f6e 7465 6e65 6772 6f27     ' Montenegro'
+000373e0: 3a20 274d 4e45 272c 0a20 2020 2020 2020  : 'MNE',.       
+000373f0: 2027 204d 6f72 6f63 636f 273a 2027 4d41   ' Morocco': 'MA
+00037400: 5227 2c0a 2020 2020 2020 2020 2720 4d6f  R',.        ' Mo
+00037410: 7a61 6d62 6971 7565 273a 2027 4d4f 5a27  zambique': 'MOZ'
+00037420: 2c0a 2020 2020 2020 2020 2720 4d79 616e  ,.        ' Myan
+00037430: 6d61 7227 3a20 274d 4d52 272c 0a20 2020  mar': 'MMR',.   
+00037440: 2020 2020 2027 204e 616d 6962 6961 273a       ' Namibia':
+00037450: 2027 4e41 4d27 2c0a 2020 2020 2020 2020   'NAM',.        
+00037460: 2720 4e65 7061 6c27 3a20 274e 504c 272c  ' Nepal': 'NPL',
+00037470: 0a20 2020 2020 2020 2027 204e 6574 6865  .        ' Nethe
+00037480: 726c 616e 6473 273a 2027 4e4c 4427 2c0a  rlands': 'NLD',.
+00037490: 2020 2020 2020 2020 2720 4e65 7720 5a65          ' New Ze
+000374a0: 616c 616e 6427 3a20 274e 5a4c 272c 0a20  aland': 'NZL',. 
+000374b0: 2020 2020 2020 2027 204e 6963 6172 6167         ' Nicarag
+000374c0: 7561 273a 2027 4e49 4327 2c0a 2020 2020  ua': 'NIC',.    
+000374d0: 2020 2020 2720 4e69 6765 7227 3a20 274e      ' Niger': 'N
+000374e0: 4552 272c 0a20 2020 2020 2020 2027 204e  ER',.        ' N
+000374f0: 6967 6572 6961 273a 2027 4e47 4127 2c0a  igeria': 'NGA',.
+00037500: 2020 2020 2020 2020 2720 4e6f 7274 6820          ' North 
+00037510: 4d61 6365 646f 6e69 6127 3a20 274d 4b44  Macedonia': 'MKD
+00037520: 272c 0a20 2020 2020 2020 2027 204e 6f72  ',.        ' Nor
+00037530: 7761 7927 3a20 274e 4f52 272c 0a20 2020  way': 'NOR',.   
+00037540: 2020 2020 2027 204f 6d61 6e27 3a20 274f       ' Oman': 'O
+00037550: 4d4e 272c 0a20 2020 2020 2020 2027 2050  MN',.        ' P
+00037560: 616b 6973 7461 6e27 3a20 2750 414b 272c  akistan': 'PAK',
+00037570: 0a20 2020 2020 2020 2027 2050 616c 6175  .        ' Palau
+00037580: 273a 2027 504c 5727 2c0a 2020 2020 2020  ': 'PLW',.      
+00037590: 2020 2720 5061 6c65 7374 696e 652c 2053    ' Palestine, S
+000375a0: 7461 7465 206f 6627 3a20 2750 5345 272c  tate of': 'PSE',
+000375b0: 0a20 2020 2020 2020 2027 2050 616e 616d  .        ' Panam
+000375c0: 6127 3a20 2750 414e 272c 0a20 2020 2020  a': 'PAN',.     
+000375d0: 2020 2027 2050 6170 7561 204e 6577 2047     ' Papua New G
+000375e0: 7569 6e65 6127 3a20 2750 4e47 272c 0a20  uinea': 'PNG',. 
+000375f0: 2020 2020 2020 2027 2050 6172 6167 7561         ' Paragua
+00037600: 7927 3a20 2750 5259 272c 0a20 2020 2020  y': 'PRY',.     
+00037610: 2020 2027 2050 6572 7527 3a20 2750 4552     ' Peru': 'PER
+00037620: 272c 0a20 2020 2020 2020 2027 2050 6869  ',.        ' Phi
+00037630: 6c69 7070 696e 6573 273a 2027 5048 4c27  lippines': 'PHL'
+00037640: 2c0a 2020 2020 2020 2020 2720 506f 6c61  ,.        ' Pola
+00037650: 6e64 273a 2027 504f 4c27 2c0a 2020 2020  nd': 'POL',.    
+00037660: 2020 2020 2720 506f 7274 7567 616c 273a      ' Portugal':
+00037670: 2027 5052 5427 2c0a 2020 2020 2020 2020   'PRT',.        
+00037680: 2720 5161 7461 7227 3a20 2751 4154 272c  ' Qatar': 'QAT',
+00037690: 0a20 2020 2020 2020 2027 2052 6f6d 616e  .        ' Roman
+000376a0: 6961 273a 2027 524f 5527 2c0a 2020 2020  ia': 'ROU',.    
+000376b0: 2020 2020 2720 5275 7373 6961 6e20 4665      ' Russian Fe
+000376c0: 6465 7261 7469 6f6e 273a 2027 5255 5327  deration': 'RUS'
+000376d0: 2c0a 2020 2020 2020 2020 2720 5277 616e  ,.        ' Rwan
+000376e0: 6461 273a 2027 5257 4127 2c0a 2020 2020  da': 'RWA',.    
+000376f0: 2020 2020 2720 5361 696e 7420 4b69 7474      ' Saint Kitt
+00037700: 7320 616e 6420 4e65 7669 7327 3a20 274b  s and Nevis': 'K
+00037710: 4e41 272c 0a20 2020 2020 2020 2027 2053  NA',.        ' S
+00037720: 6169 6e74 204c 7563 6961 273a 2027 4c43  aint Lucia': 'LC
+00037730: 4127 2c0a 2020 2020 2020 2020 2720 5361  A',.        ' Sa
+00037740: 696e 7420 5669 6e63 656e 7420 616e 6420  int Vincent and 
+00037750: 7468 6520 4772 656e 6164 696e 6573 273a  the Grenadines':
+00037760: 2027 5643 5427 2c0a 2020 2020 2020 2020   'VCT',.        
+00037770: 2720 5361 6d6f 6127 3a20 2757 534d 272c  ' Samoa': 'WSM',
+00037780: 0a20 2020 2020 2020 2027 2053 616f 2054  .        ' Sao T
+00037790: 6f6d 6520 616e 6420 5072 696e 6369 7065  ome and Principe
+000377a0: 273a 2027 5354 5027 2c0a 2020 2020 2020  ': 'STP',.      
+000377b0: 2020 2720 5361 7564 6920 4172 6162 6961    ' Saudi Arabia
+000377c0: 273a 2027 5341 5527 2c0a 2020 2020 2020  ': 'SAU',.      
+000377d0: 2020 2720 5365 6e65 6761 6c27 3a20 2753    ' Senegal': 'S
+000377e0: 454e 272c 0a20 2020 2020 2020 2027 2053  EN',.        ' S
+000377f0: 6572 6269 6127 3a20 2753 5242 272c 0a20  erbia': 'SRB',. 
+00037800: 2020 2020 2020 2027 2053 6579 6368 656c         ' Seychel
+00037810: 6c65 7327 3a20 2753 5943 272c 0a20 2020  les': 'SYC',.   
+00037820: 2020 2020 2027 2053 6965 7272 6120 4c65       ' Sierra Le
+00037830: 6f6e 6527 3a20 2753 4c45 272c 0a20 2020  one': 'SLE',.   
+00037840: 2020 2020 2027 2053 696e 6761 706f 7265       ' Singapore
+00037850: 273a 2027 5347 5027 2c0a 2020 2020 2020  ': 'SGP',.      
+00037860: 2020 2720 536c 6f76 616b 6961 273a 2027    ' Slovakia': '
+00037870: 5356 4b27 2c0a 2020 2020 2020 2020 2720  SVK',.        ' 
+00037880: 536c 6f76 656e 6961 273a 2027 5356 4e27  Slovenia': 'SVN'
+00037890: 2c0a 2020 2020 2020 2020 2720 536f 6c6f  ,.        ' Solo
+000378a0: 6d6f 6e20 4973 6c61 6e64 7327 3a20 2753  mon Islands': 'S
+000378b0: 4c42 272c 0a20 2020 2020 2020 2027 2053  LB',.        ' S
+000378c0: 6f75 7468 2041 6672 6963 6127 3a20 275a  outh Africa': 'Z
+000378d0: 4146 272c 0a20 2020 2020 2020 2027 2053  AF',.        ' S
+000378e0: 6f75 7468 2053 7564 616e 273a 2027 5353  outh Sudan': 'SS
+000378f0: 4427 2c0a 2020 2020 2020 2020 2720 5370  D',.        ' Sp
+00037900: 6169 6e27 3a20 2745 5350 272c 0a20 2020  ain': 'ESP',.   
+00037910: 2020 2020 2027 2053 7269 204c 616e 6b61       ' Sri Lanka
+00037920: 273a 2027 4c4b 4127 2c0a 2020 2020 2020  ': 'LKA',.      
+00037930: 2020 2720 5375 6461 6e27 3a20 2753 444e    ' Sudan': 'SDN
+00037940: 272c 0a20 2020 2020 2020 2027 2053 7572  ',.        ' Sur
+00037950: 696e 616d 6527 3a20 2753 5552 272c 0a20  iname': 'SUR',. 
+00037960: 2020 2020 2020 2027 2053 7765 6465 6e27         ' Sweden'
+00037970: 3a20 2753 5745 272c 0a20 2020 2020 2020  : 'SWE',.       
+00037980: 2027 2053 7769 747a 6572 6c61 6e64 273a   ' Switzerland':
+00037990: 2027 4348 4527 2c0a 2020 2020 2020 2020   'CHE',.        
+000379a0: 2720 5379 7269 616e 2041 7261 6220 5265  ' Syrian Arab Re
+000379b0: 7075 626c 6963 273a 2027 5359 5227 2c0a  public': 'SYR',.
+000379c0: 2020 2020 2020 2020 2720 5461 6a69 6b69          ' Tajiki
+000379d0: 7374 616e 273a 2027 544a 4b27 2c0a 2020  stan': 'TJK',.  
+000379e0: 2020 2020 2020 2720 5461 6e7a 616e 6961        ' Tanzania
+000379f0: 2028 556e 6974 6564 2052 6570 7562 6c69   (United Republi
+00037a00: 6320 6f66 2927 3a20 2754 5a41 272c 0a20  c of)': 'TZA',. 
+00037a10: 2020 2020 2020 2027 2054 6861 696c 616e         ' Thailan
+00037a20: 6427 3a20 2754 4841 272c 0a20 2020 2020  d': 'THA',.     
+00037a30: 2020 2027 2054 696d 6f72 2d4c 6573 7465     ' Timor-Leste
+00037a40: 273a 2027 544c 5327 2c0a 2020 2020 2020  ': 'TLS',.      
+00037a50: 2020 2720 546f 676f 273a 2027 5447 4f27    ' Togo': 'TGO'
+00037a60: 2c0a 2020 2020 2020 2020 2720 546f 6e67  ,.        ' Tong
+00037a70: 6127 3a20 2754 4f4e 272c 0a20 2020 2020  a': 'TON',.     
+00037a80: 2020 2027 2054 7269 6e69 6461 6420 616e     ' Trinidad an
+00037a90: 6420 546f 6261 676f 273a 2027 5454 4f27  d Tobago': 'TTO'
+00037aa0: 2c0a 2020 2020 2020 2020 2720 5475 6e69  ,.        ' Tuni
+00037ab0: 7369 6127 3a20 2754 554e 272c 0a20 2020  sia': 'TUN',.   
+00037ac0: 2020 2020 2027 2054 7572 6b65 7927 3a20       ' Turkey': 
+00037ad0: 2754 5552 272c 0a20 2020 2020 2020 2027  'TUR',.        '
+00037ae0: 2054 7572 6b6d 656e 6973 7461 6e27 3a20   Turkmenistan': 
+00037af0: 2754 4b4d 272c 0a20 2020 2020 2020 2027  'TKM',.        '
+00037b00: 2055 6761 6e64 6127 3a20 2755 4741 272c   Uganda': 'UGA',
+00037b10: 0a20 2020 2020 2020 2027 2055 6b72 6169  .        ' Ukrai
+00037b20: 6e65 273a 2027 554b 5227 2c0a 2020 2020  ne': 'UKR',.    
+00037b30: 2020 2020 2720 556e 6974 6564 2041 7261      ' United Ara
+00037b40: 6220 456d 6972 6174 6573 273a 2027 4152  b Emirates': 'AR
+00037b50: 4527 2c0a 2020 2020 2020 2020 2720 556e  E',.        ' Un
+00037b60: 6974 6564 204b 696e 6764 6f6d 273a 2027  ited Kingdom': '
+00037b70: 4742 5227 2c0a 2020 2020 2020 2020 2720  GBR',.        ' 
+00037b80: 556e 6974 6564 2053 7461 7465 7327 3a20  United States': 
+00037b90: 2755 5341 272c 0a20 2020 2020 2020 2027  'USA',.        '
+00037ba0: 2055 7275 6775 6179 273a 2027 5552 5927   Uruguay': 'URY'
+00037bb0: 2c0a 2020 2020 2020 2020 2720 557a 6265  ,.        ' Uzbe
+00037bc0: 6b69 7374 616e 273a 2027 555a 4227 2c0a  kistan': 'UZB',.
+00037bd0: 2020 2020 2020 2020 2720 5661 6e75 6174          ' Vanuat
+00037be0: 7527 3a20 2756 5554 272c 0a20 2020 2020  u': 'VUT',.     
+00037bf0: 2020 2027 2056 656e 657a 7565 6c61 2028     ' Venezuela (
+00037c00: 426f 6c69 7661 7269 616e 2052 6570 7562  Bolivarian Repub
+00037c10: 6c69 6320 6f66 2927 3a20 2756 454e 272c  lic of)': 'VEN',
+00037c20: 0a20 2020 2020 2020 2027 2056 6965 7420  .        ' Viet 
+00037c30: 4e61 6d27 3a20 2756 4e4d 272c 0a20 2020  Nam': 'VNM',.   
+00037c40: 2020 2020 2027 2059 656d 656e 273a 2027       ' Yemen': '
+00037c50: 5945 4d27 2c0a 2020 2020 2020 2020 2720  YEM',.        ' 
+00037c60: 5a61 6d62 6961 273a 2027 5a4d 4227 2c0a  Zambia': 'ZMB',.
+00037c70: 2020 2020 2020 2020 2720 5a69 6d62 6162          ' Zimbab
+00037c80: 7765 273a 2027 5a57 4527 2c0a 2020 2020  we': 'ZWE',.    
+00037c90: 2020 2020 2748 756d 616e 2044 6576 656c      'Human Devel
+00037ca0: 6f70 6d65 6e74 273a 204e 6f6e 652c 0a20  opment': None,. 
+00037cb0: 2020 2020 2020 2027 5665 7279 2068 6967         'Very hig
+00037cc0: 6820 6875 6d61 6e20 6465 7665 6c6f 706d  h human developm
+00037cd0: 656e 7427 3a20 4e6f 6e65 2c0a 2020 2020  ent': None,.    
+00037ce0: 2020 2020 2748 6967 6820 6875 6d61 6e20      'High human 
+00037cf0: 6465 7665 6c6f 706d 656e 7427 3a20 4e6f  development': No
+00037d00: 6e65 2c0a 2020 2020 2020 2020 274d 6564  ne,.        'Med
+00037d10: 6975 6d20 6875 6d61 6e20 6465 7665 6c6f  ium human develo
+00037d20: 706d 656e 7427 3a20 4e6f 6e65 2c0a 2020  pment': None,.  
+00037d30: 2020 2020 2020 274c 6f77 2068 756d 616e        'Low human
+00037d40: 2064 6576 656c 6f70 6d65 6e74 273a 204e   development': N
+00037d50: 6f6e 652c 0a20 2020 2020 2020 2027 4465  one,.        'De
+00037d60: 7665 6c6f 7069 6e67 2043 6f75 6e74 7269  veloping Countri
+00037d70: 6573 273a 204e 6f6e 652c 0a20 2020 2020  es': None,.     
+00037d80: 2020 2027 5265 6769 6f6e 7327 3a20 4e6f     'Regions': No
+00037d90: 6e65 2c0a 2020 2020 2020 2020 2741 7261  ne,.        'Ara
+00037da0: 6220 5374 6174 6573 273a 204e 6f6e 652c  b States': None,
+00037db0: 0a20 2020 2020 2020 2027 4561 7374 2041  .        'East A
+00037dc0: 7369 6120 616e 6420 7468 6520 5061 6369  sia and the Paci
+00037dd0: 6669 6327 3a20 4e6f 6e65 2c0a 2020 2020  fic': None,.    
+00037de0: 2020 2020 2745 7572 6f70 6520 616e 6420      'Europe and 
+00037df0: 4365 6e74 7261 6c20 4173 6961 273a 204e  Central Asia': N
+00037e00: 6f6e 652c 0a20 2020 2020 2020 2027 4c61  one,.        'La
+00037e10: 7469 6e20 416d 6572 6963 6120 616e 6420  tin America and 
+00037e20: 7468 6520 4361 7269 6262 6561 6e27 3a20  the Caribbean': 
+00037e30: 4e6f 6e65 2c0a 2020 2020 2020 2020 2753  None,.        'S
+00037e40: 6f75 7468 2041 7369 6127 3a20 4e6f 6e65  outh Asia': None
+00037e50: 2c0a 2020 2020 2020 2020 2753 7562 2d53  ,.        'Sub-S
+00037e60: 6168 6172 616e 2041 6672 6963 6127 3a20  aharan Africa': 
+00037e70: 4e6f 6e65 2c0a 2020 2020 2020 2020 274c  None,.        'L
+00037e80: 6561 7374 2044 6576 656c 6f70 6564 2043  east Developed C
+00037e90: 6f75 6e74 7269 6573 273a 204e 6f6e 652c  ountries': None,
+00037ea0: 0a20 2020 2020 2020 2027 536d 616c 6c20  .        'Small 
+00037eb0: 4973 6c61 6e64 2044 6576 656c 6f70 696e  Island Developin
+00037ec0: 6720 5374 6174 6573 273a 204e 6f6e 652c  g States': None,
+00037ed0: 0a20 2020 2020 2020 2027 4f72 6761 6e69  .        'Organi
+00037ee0: 7a61 7469 6f6e 2066 6f72 2045 636f 6e6f  zation for Econo
+00037ef0: 6d69 6320 436f 2d6f 7065 7261 7469 6f6e  mic Co-operation
+00037f00: 2061 6e64 2044 6576 656c 6f70 6d65 6e74   and Development
+00037f10: 273a 204e 6f6e 652c 0a20 2020 2020 2020  ': None,.       
+00037f20: 2027 576f 726c 6427 3a20 2757 6f72 6c64   'World': 'World
+00037f30: 272c 0a20 2020 207d 0a0a 2020 2020 6461  ',.    }..    da
+00037f40: 7461 2e69 6e64 6578 203d 2064 6174 612e  ta.index = data.
+00037f50: 6c6f 635b 3a2c 2027 436f 756e 7472 7927  loc[:, 'Country'
+00037f60: 5d2e 6d61 7028 7265 6769 6f6e 4d61 7070  ].map(regionMapp
+00037f70: 696e 6729 0a0a 2020 2020 6461 7461 2e69  ing)..    data.i
+00037f80: 6e64 6578 5b64 6174 612e 696e 6465 782e  ndex[data.index.
+00037f90: 6475 706c 6963 6174 6564 2829 5d0a 2020  duplicated()].  
+00037fa0: 2020 6461 7461 203d 2064 6174 612e 6c6f    data = data.lo
+00037fb0: 635b 3a2c 2079 6561 7243 6f6c 756d 6e73  c[:, yearColumns
+00037fc0: 5d0a 2020 2020 6461 7461 203d 2064 6174  ].    data = dat
+00037fd0: 612e 6c6f 635b 7e64 6174 612e 696e 6465  a.loc[~data.inde
+00037fe0: 782e 6973 6e75 6c6c 2829 2c20 3a5d 2e61  x.isnull(), :].a
+00037ff0: 7374 7970 6528 666c 6f61 7429 0a0a 2020  stype(float)..  
+00038000: 2020 6d65 7461 203d 207b 0a20 2020 2020    meta = {.     
+00038010: 2020 2027 656e 7469 7479 273a 2027 4844     'entity': 'HD
+00038020: 495f 4875 6d61 6e5f 6465 7665 6c6f 706d  I_Human_developm
+00038030: 656e 745f 696e 6465 7827 2c0a 2020 2020  ent_index',.    
+00038040: 2020 2020 2773 6365 6e61 7269 6f27 3a20      'scenario': 
+00038050: 2748 6973 746f 7269 6327 2c0a 2020 2020  'Historic',.    
+00038060: 2020 2020 2775 6e69 7427 3a20 2764 696d      'unit': 'dim
+00038070: 656e 7369 6f6e 6c65 7373 272c 0a20 2020  ensionless',.   
+00038080: 2020 2020 2027 736f 7572 6365 273a 2073       'source': s
+00038090: 6f75 7263 654d 6574 615b 2753 4f55 5243  ourceMeta['SOURC
+000380a0: 455f 4944 275d 2c0a 2020 2020 7d0a 2020  E_ID'],.    }.  
+000380b0: 2020 7461 626c 6520 3d20 6474 2e44 6174    table = dt.Dat
+000380c0: 6174 6162 6c65 2864 6174 612c 206d 6574  atable(data, met
+000380d0: 613d 6d65 7461 290a 2020 2020 7461 626c  a=meta).    tabl
+000380e0: 652e 6765 6e65 7261 7465 5461 626c 6549  e.generateTableI
+000380f0: 4428 290a 0a20 2020 2064 742e 636f 6d6d  D()..    dt.comm
+00038100: 6974 5461 626c 6573 285b 7461 626c 655d  itTables([table]
+00038110: 2c20 2748 4449 2064 6174 6120 7570 6461  , 'HDI data upda
+00038120: 7465 272c 2073 6f75 7263 654d 6574 612c  te', sourceMeta,
+00038130: 2075 7064 6174 653d 5472 7565 290a 0a0a   update=True)...
+00038140: 6465 6620 554e 5f57 5050 5f32 3031 395f  def UN_WPP_2019_
+00038150: 696d 706f 7274 2829 3a0a 2020 2020 736f  import():.    so
+00038160: 7572 6365 4d65 7461 203d 207b 0a20 2020  urceMeta = {.   
+00038170: 2020 2020 2027 534f 5552 4345 5f49 4427       'SOURCE_ID'
+00038180: 3a20 2755 4e5f 5750 5032 3031 3927 2c0a  : 'UN_WPP2019',.
+00038190: 2020 2020 2020 2020 2763 6f6c 6c65 6374          'collect
+000381a0: 6564 5f62 7927 3a20 2741 4727 2c0a 2020  ed_by': 'AG',.  
+000381b0: 2020 2020 2020 2764 6174 6527 3a20 6474        'date': dt
+000381c0: 2e63 6f72 652e 6765 745f 6461 7465 5f73  .core.get_date_s
+000381d0: 7472 696e 6728 292c 0a20 2020 2020 2020  tring(),.       
+000381e0: 2027 736f 7572 6365 5f75 726c 273a 2027   'source_url': '
+000381f0: 6874 7470 733a 2f2f 706f 7075 6c61 7469  https://populati
+00038200: 6f6e 2e75 6e2e 6f72 672f 7770 702f 446f  on.un.org/wpp/Do
+00038210: 776e 6c6f 6164 2f53 7461 6e64 6172 642f  wnload/Standard/
+00038220: 506f 7075 6c61 7469 6f6e 2f27 2c0a 2020  Population/',.  
+00038230: 2020 2020 2020 276c 6963 656e 6365 273a        'licence':
+00038240: 2027 6f70 656e 2073 6f75 7263 6527 2c0a   'open source',.
+00038250: 2020 2020 7d0a 0a20 2020 206d 6170 7069      }..    mappi
+00038260: 6e67 4469 6374 203d 207b 0a20 2020 2020  ngDict = {.     
+00038270: 2020 2069 6e74 2878 293a 2079 0a20 2020     int(x): y.   
+00038280: 2020 2020 2066 6f72 2078 2c20 7920 696e       for x, y in
+00038290: 207a 6970 2864 742e 6d61 7070 2e63 6f75   zip(dt.mapp.cou
+000382a0: 6e74 7269 6573 2e63 6f64 6573 2e6e 756d  ntries.codes.num
+000382b0: 4953 4f2c 2064 742e 6d61 7070 2e63 6f75  ISO, dt.mapp.cou
+000382c0: 6e74 7269 6573 2e63 6f64 6573 2e69 6e64  ntries.codes.ind
+000382d0: 6578 290a 2020 2020 2020 2020 6966 206e  ex).        if n
+000382e0: 6f74 2028 7064 2e6e 702e 6973 6e61 6e28  ot (pd.np.isnan(
+000382f0: 7829 290a 2020 2020 7d0a 2020 2020 6d61  x)).    }.    ma
+00038300: 7070 696e 6744 6963 745b 3930 305d 203d  ppingDict[900] =
+00038310: 2027 576f 726c 6427 0a20 2020 2053 4f55   'World'.    SOU
+00038320: 5243 4520 3d20 2255 4e5f 5750 5032 3031  RCE = "UN_WPP201
+00038330: 3922 0a20 2020 2053 4f55 5243 455f 5041  9".    SOURCE_PA
+00038340: 5448 203d 206f 732e 7061 7468 2e6a 6f69  TH = os.path.joi
+00038350: 6e28 6474 2e63 6f6e 6669 672e 5041 5448  n(dt.config.PATH
+00038360: 5f54 4f5f 4441 5441 5348 454c 462c 2027  _TO_DATASHELF, '
+00038370: 7261 7764 6174 612f 554e 5f57 5050 3230  rawdata/UN_WPP20
+00038380: 3139 2729 0a20 2020 206d 6574 6153 6574  19').    metaSet
+00038390: 7570 203d 207b 0a20 2020 2020 2020 2027  up = {.        '
+000383a0: 736f 7572 6365 273a 2053 4f55 5243 452c  source': SOURCE,
+000383b0: 0a20 2020 2020 2020 2027 656e 7469 7479  .        'entity
+000383c0: 273a 2027 706f 7075 6c61 7469 6f6e 272c  ': 'population',
+000383d0: 0a20 2020 2020 2020 2027 756e 6974 273a  .        'unit':
+000383e0: 2027 7468 6f75 7361 6e64 7327 2c0a 2020   'thousands',.  
+000383f0: 2020 2020 2020 2763 6174 6567 6f72 7927        'category'
+00038400: 3a20 2774 6f74 616c 272c 0a20 2020 207d  : 'total',.    }
+00038410: 0a0a 2020 2020 2320 6368 616e 6765 2073  ..    # change s
+00038420: 6574 7570 0a20 2020 2065 7863 656c 5365  etup.    excelSe
+00038430: 7475 7020 3d20 6469 6374 2829 0a20 2020  tup = dict().   
+00038440: 2065 7863 656c 5365 7475 705b 2766 696c   excelSetup['fil
+00038450: 6550 6174 6827 5d20 3d20 534f 5552 4345  ePath'] = SOURCE
+00038460: 5f50 4154 480a 2020 2020 6578 6365 6c53  _PATH.    excelS
+00038470: 6574 7570 5b27 6669 6c65 4e61 6d65 275d  etup['fileName']
+00038480: 203d 2027 5750 5032 3031 395f 504f 505f   = 'WPP2019_POP_
+00038490: 4630 315f 315f 544f 5441 4c5f 504f 5055  F01_1_TOTAL_POPU
+000384a0: 4c41 5449 4f4e 5f42 4f54 485f 5345 5845  LATION_BOTH_SEXE
+000384b0: 532e 786c 7378 270a 2020 2020 6578 6365  S.xlsx'.    exce
+000384c0: 6c53 6574 7570 5b27 7368 6565 744e 616d  lSetup['sheetNam
+000384d0: 6527 5d20 3d20 2745 5354 494d 4154 4553  e'] = 'ESTIMATES
+000384e0: 270a 2020 2020 6578 6365 6c53 6574 7570  '.    excelSetup
+000384f0: 5b27 7469 6d65 436f 6c49 6478 275d 203d  ['timeColIdx'] =
+00038500: 2028 2748 3137 272c 2027 434a 3137 2729   ('H17', 'CJ17')
+00038510: 0a20 2020 2065 7863 656c 5365 7475 705b  .    excelSetup[
+00038520: 2773 7061 6365 526f 7749 6478 275d 203d  'spaceRowIdx'] =
+00038530: 2028 2745 3138 272c 2027 4533 3036 2729   ('E18', 'E306')
+00038540: 0a0a 2020 2020 7461 626c 6573 203d 206c  ..    tables = l
+00038550: 6973 7428 290a 0a20 2020 2023 2067 6174  ist()..    # gat
+00038560: 6865 7220 6869 7374 6f72 6963 2064 6174  her historic dat
+00038570: 610a 2020 2020 2320 2020 2020 2020 2069  a.    #        i
+00038580: 746f 6f6c 203d 2055 4e5f 5750 5028 6578  tool = UN_WPP(ex
+00038590: 6365 6c53 6574 7570 290a 2020 2020 6d65  celSetup).    me
+000385a0: 7461 5365 7475 705b 2773 6365 6e61 7269  taSetup['scenari
+000385b0: 6f27 5d20 3d20 2768 6973 746f 7269 6327  o'] = 'historic'
+000385c0: 0a20 2020 2065 7874 7261 6374 6f72 203d  .    extractor =
+000385d0: 2064 742e 696f 2e45 7863 656c 5265 6164   dt.io.ExcelRead
+000385e0: 6572 2865 7863 656c 5365 7475 7029 0a20  er(excelSetup). 
+000385f0: 2020 2074 6162 6c65 203d 2065 7874 7261     table = extra
+00038600: 6374 6f72 2e67 6174 6865 7244 6174 6128  ctor.gatherData(
+00038610: 290a 2020 2020 7461 626c 6520 3d20 7461  ).    table = ta
+00038620: 626c 652e 7265 706c 6163 6528 27e2 80a6  ble.replace('...
+00038630: 272c 2070 642e 6e70 2e6e 616e 290a 2020  ', pd.np.nan).  
+00038640: 2020 7461 626c 655b 276e 6577 496e 6465    table['newInde
+00038650: 7827 5d20 3d20 7461 626c 652e 696e 6465  x'] = table.inde
+00038660: 780a 2020 2020 7461 626c 655b 276e 6577  x.    table['new
+00038670: 496e 6465 7827 5d20 3d20 7461 626c 652e  Index'] = table.
+00038680: 696e 6465 782e 746f 5f73 6572 6965 7328  index.to_series(
+00038690: 292e 6d61 7028 6d61 7070 696e 6744 6963  ).map(mappingDic
+000386a0: 7429 0a20 2020 2074 6162 6c65 2e6c 6f63  t).    table.loc
+000386b0: 5b70 642e 6973 6e75 6c6c 2874 6162 6c65  [pd.isnull(table
+000386c0: 5b27 6e65 7749 6e64 6578 275d 292c 2027  ['newIndex']), '
+000386d0: 6e65 7749 6e64 6578 275d 203d 2074 6162  newIndex'] = tab
+000386e0: 6c65 2e69 6e64 6578 5b0a 2020 2020 2020  le.index[.      
+000386f0: 2020 7064 2e69 736e 756c 6c28 7461 626c    pd.isnull(tabl
+00038700: 655b 276e 6577 496e 6465 7827 5d29 0a20  e['newIndex']). 
+00038710: 2020 205d 0a20 2020 2074 6162 6c65 203d     ].    table =
+00038720: 2074 6162 6c65 2e73 6574 5f69 6e64 6578   table.set_index
+00038730: 2827 6e65 7749 6e64 6578 2729 0a20 2020  ('newIndex').   
+00038740: 206e 6577 4964 7820 3d20 5b6d 6170 7069   newIdx = [mappi
+00038750: 6e67 4469 6374 5b78 5d20 666f 7220 7820  ngDict[x] for x 
+00038760: 696e 2074 6162 6c65 2e69 6e64 6578 2069  in table.index i
+00038770: 6620 7820 696e 206d 6170 7069 6e67 4469  f x in mappingDi
+00038780: 6374 2e6b 6579 7328 295d 0a20 2020 2074  ct.keys()].    t
+00038790: 6162 6c65 732e 6170 7065 6e64 2864 742e  ables.append(dt.
+000387a0: 4461 7461 7461 626c 6528 7461 626c 652c  Datatable(table,
+000387b0: 206d 6574 613d 6d65 7461 5365 7475 7029   meta=metaSetup)
+000387c0: 290a 0a20 2020 2023 2067 6174 6865 7220  )..    # gather 
+000387d0: 7072 6f6a 6563 7469 6e6f 730a 2020 2020  projectinos.    
+000387e0: 2320 6578 6365 6c53 6574 7570 5b27 7469  # excelSetup['ti
+000387f0: 6d65 436f 6c49 6478 275d 2020 3d20 2827  meColIdx']  = ('
+00038800: 4631 3727 2c20 2743 5731 3727 290a 0a20  F17', 'CW17').. 
+00038810: 2020 2073 6365 6e44 6963 7420 3d20 7b0a     scenDict = {.
+00038820: 2020 2020 2020 2020 2750 524f 4a45 4354          'PROJECT
+00038830: 494f 4e5f 4c4f 5727 3a20 274c 4f57 2056  ION_LOW': 'LOW V
+00038840: 4152 4941 4e54 272c 0a20 2020 2020 2020  ARIANT',.       
+00038850: 2027 5052 4f4a 4543 5449 4f4e 5f4d 4544   'PROJECTION_MED
+00038860: 273a 2027 4d45 4449 554d 2056 4152 4941  ': 'MEDIUM VARIA
+00038870: 4e54 272c 0a20 2020 2020 2020 2027 5052  NT',.        'PR
+00038880: 4f4a 4543 5449 4f4e 5f48 4927 3a20 2748  OJECTION_HI': 'H
+00038890: 4947 4820 5641 5249 414e 5427 2c0a 2020  IGH VARIANT',.  
+000388a0: 2020 7d0a 2020 2020 2320 6974 6f6f 6c20    }.    # itool 
+000388b0: 3d20 554e 5f57 5050 2865 7863 656c 5365  = UN_WPP(excelSe
+000388c0: 7475 7029 0a0a 2020 2020 666f 7220 7363  tup)..    for sc
+000388d0: 656e 6172 696f 2c20 7368 6565 744e 616d  enario, sheetNam
+000388e0: 6520 696e 2073 6365 6e44 6963 742e 6974  e in scenDict.it
+000388f0: 656d 7328 293a 0a20 2020 2020 2020 206d  ems():.        m
+00038900: 6574 6153 6574 7570 5b27 7363 656e 6172  etaSetup['scenar
+00038910: 696f 275d 203d 2073 6365 6e61 7269 6f0a  io'] = scenario.
+00038920: 2020 2020 2020 2020 6578 6365 6c53 6574          excelSet
+00038930: 7570 5b27 7368 6565 744e 616d 6527 5d20  up['sheetName'] 
+00038940: 3d20 7368 6565 744e 616d 650a 2020 2020  = sheetName.    
+00038950: 2020 2020 6578 7472 6163 746f 7220 3d20      extractor = 
+00038960: 6474 2e69 6f2e 4578 6365 6c52 6561 6465  dt.io.ExcelReade
+00038970: 7228 6578 6365 6c53 6574 7570 290a 2020  r(excelSetup).  
+00038980: 2020 2020 2020 7461 626c 6520 3d20 6578        table = ex
+00038990: 7472 6163 746f 722e 6761 7468 6572 4461  tractor.gatherDa
+000389a0: 7461 2829 0a20 2020 2020 2020 2074 6162  ta().        tab
+000389b0: 6c65 203d 2074 6162 6c65 2e72 6570 6c61  le = table.repla
+000389c0: 6365 2827 e280 a627 2c20 7064 2e6e 702e  ce('...', pd.np.
+000389d0: 6e61 6e29 0a20 2020 2020 2020 2074 6162  nan).        tab
+000389e0: 6c65 5b27 6e65 7749 6e64 6578 275d 203d  le['newIndex'] =
+000389f0: 2074 6162 6c65 2e69 6e64 6578 0a20 2020   table.index.   
+00038a00: 2020 2020 2074 6162 6c65 5b27 6e65 7749       table['newI
+00038a10: 6e64 6578 275d 203d 2074 6162 6c65 2e69  ndex'] = table.i
+00038a20: 6e64 6578 2e74 6f5f 7365 7269 6573 2829  ndex.to_series()
+00038a30: 2e6d 6170 286d 6170 7069 6e67 4469 6374  .map(mappingDict
+00038a40: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
+00038a50: 6c6f 635b 7064 2e69 736e 756c 6c28 7461  loc[pd.isnull(ta
+00038a60: 626c 655b 276e 6577 496e 6465 7827 5d29  ble['newIndex'])
+00038a70: 2c20 276e 6577 496e 6465 7827 5d20 3d20  , 'newIndex'] = 
+00038a80: 7461 626c 652e 696e 6465 785b 0a20 2020  table.index[.   
+00038a90: 2020 2020 2020 2020 2070 642e 6973 6e75           pd.isnu
+00038aa0: 6c6c 2874 6162 6c65 5b27 6e65 7749 6e64  ll(table['newInd
+00038ab0: 6578 275d 290a 2020 2020 2020 2020 5d0a  ex']).        ].
+00038ac0: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
+00038ad0: 7461 626c 652e 7365 745f 696e 6465 7828  table.set_index(
+00038ae0: 276e 6577 496e 6465 7827 290a 2020 2020  'newIndex').    
+00038af0: 2020 2020 7461 626c 6573 2e61 7070 656e      tables.appen
+00038b00: 6428 6474 2e44 6174 6174 6162 6c65 2874  d(dt.Datatable(t
+00038b10: 6162 6c65 2c20 6d65 7461 3d6d 6574 6153  able, meta=metaS
+00038b20: 6574 7570 2929 0a20 2020 2023 2525 0a20  etup)).    #%%. 
+00038b30: 2020 2064 6566 2061 6464 5f45 5528 7461     def add_EU(ta
+00038b40: 626c 6529 3a0a 2020 2020 2020 2020 4555  ble):.        EU
+00038b50: 5f43 4f55 4e54 5249 4553 203d 206c 6973  _COUNTRIES = lis
+00038b60: 7428 6474 2e6d 6170 702e 7265 6769 6f6e  t(dt.mapp.region
+00038b70: 732e 4555 3238 2e6d 656d 6265 7273 4f66  s.EU28.membersOf
+00038b80: 2827 4555 3238 2729 290a 2020 2020 2020  ('EU28')).      
+00038b90: 2020 7461 626c 652e 6c6f 635b 2745 5532    table.loc['EU2
+00038ba0: 3827 5d20 3d20 7461 626c 652e 6c6f 635b  8'] = table.loc[
+00038bb0: 4555 5f43 4f55 4e54 5249 4553 5d2e 7375  EU_COUNTRIES].su
+00038bc0: 6d28 290a 2020 2020 2020 2020 7265 7475  m().        retu
+00038bd0: 726e 2074 6162 6c65 0a0a 2020 2020 7461  rn table..    ta
+00038be0: 626c 6573 203d 205b 6164 645f 4555 2874  bles = [add_EU(t
+00038bf0: 6162 6c65 2920 666f 7220 7461 626c 6520  able) for table 
+00038c00: 696e 2074 6162 6c65 735d 0a0a 2020 2020  in tables]..    
+00038c10: 6474 2e63 6f6d 6d69 7454 6162 6c65 7328  dt.commitTables(
+00038c20: 7461 626c 6573 2c20 2755 4e57 5050 3230  tables, 'UNWPP20
+00038c30: 3137 2064 6174 6127 2c20 736f 7572 6365  17 data', source
+00038c40: 4d65 7461 2c20 6170 7065 6e64 5f64 6174  Meta, append_dat
+00038c50: 613d 5472 7565 2c20 7570 6461 7465 3d54  a=True, update=T
+00038c60: 7275 6529 0a20 2020 2072 6574 7572 6e20  rue).    return 
+00038c70: 7461 626c 6573 0a0a 0a69 6620 636f 6e66  tables...if conf
+00038c80: 6967 2e44 4542 5547 3a0a 2020 2020 7072  ig.DEBUG:.    pr
+00038c90: 696e 7428 2752 6177 2073 6f75 7263 6573  int('Raw sources
+00038ca0: 206c 6f61 6465 6420 696e 207b 3a32 2e34   loaded in {:2.4
+00038cb0: 667d 2073 6563 6f6e 6473 272e 666f 726d  f} seconds'.form
+00038cc0: 6174 2874 696d 652e 7469 6d65 2829 202d  at(time.time() -
+00038cd0: 2074 7429 290a 0a0a 2325 2520 496d 706f   tt))...#%% Impo
+00038ce0: 7274 2065 7861 6d70 6c65 0a69 6620 5f5f  rt example.if __
+00038cf0: 6e61 6d65 5f5f 203d 3d20 275f 5f6d 6169  name__ == '__mai
+00038d00: 6e5f 5f27 3a0a 2020 2020 2320 7864 6667  n__':.    # xdfg
+00038d10: 0a20 2020 2022 2222 0a20 2020 2043 6f6e  .    """.    Con
+00038d20: 6669 670a 2020 2020 2222 220a 2020 2020  fig.    """.    
+00038d30: 7570 6461 7465 5f63 6f6e 7465 6e74 203d  update_content =
+00038d40: 2054 7275 650a 0a20 2020 2022 2222 200a   True..    """ .
+00038d50: 2020 2020 496e 6974 6961 6c69 7a65 2063      Initialize c
+00038d60: 6c61 7373 3a0a 2020 2020 5468 6973 2077  lass:.    This w
+00038d70: 696c 6c20 6c6f 6164 2074 6865 206d 6170  ill load the map
+00038d80: 7069 6e67 2066 696c 652c 2072 6561 6420  ping file, read 
+00038d90: 7468 6520 6461 7461 2061 6e64 2070 7265  the data and pre
+00038da0: 7061 7265 2074 6865 2061 6464 6974 696f  pare the additio
+00038db0: 6e61 6c0a 2020 2020 6d65 7461 2069 6e66  nal.    meta inf
+00038dc0: 6f72 6d61 7469 6f6e 732e 0a20 2020 2022  ormations..    "
+00038dd0: 2222 0a20 2020 2023 2072 6561 6465 7220  "".    # reader 
+00038de0: 3d20 5052 494d 4150 5f48 4953 5428 7665  = PRIMAP_HIST(ve
+00038df0: 7273 696f 6e3d 2276 322e 335f 6e6f 5f72  rsion="v2.3_no_r
+00038e00: 6f75 6e64 696e 675f 3238 5f4a 756c 5f32  ounding_28_Jul_2
+00038e10: 3032 3122 2c20 7965 6172 3d32 3032 3129  021", year=2021)
+00038e20: 0a20 2020 2023 2072 6561 6465 7220 3d20  .    # reader = 
+00038e30: 5049 4b5f 4e44 4328 3230 3231 2c20 7665  PIK_NDC(2021, ve
+00038e40: 7273 696f 6e20 3d20 2776 312e 302e 3227  rsion = 'v1.0.2'
+00038e50: 290a 2020 2020 2320 7265 6164 6572 203d  ).    # reader =
+00038e60: 2050 5249 4d41 5028 7965 6172 203d 2032   PRIMAP(year = 2
+00038e70: 3032 3129 0a20 2020 2023 2072 6561 6465  021).    # reade
+00038e80: 7220 3d20 4949 4153 4128 2745 4e47 4147  r = IIASA('ENGAG
+00038e90: 455f 3230 3231 272c 2027 656e 6761 6765  E_2021', 'engage
 00038ea0: 2729 0a20 2020 2023 2072 6561 6465 7220  ').    # reader 
-00038eb0: 3d20 4949 4153 4128 2749 5043 435f 4152  = IIASA('IPCC_AR
-00038ec0: 3527 2c20 6461 7461 5f66 696c 6520 3d27  5', data_file ='
-00038ed0: 2f6d 6564 6961 2f73 665f 446f 6375 6d65  /media/sf_Docume
-00038ee0: 6e74 732f 6461 7461 7368 656c 665f 7630  nts/datashelf_v0
-00038ef0: 332f 7261 7764 6174 612f 4152 355f 6461  3/rawdata/AR5_da
-00038f00: 7461 6261 7365 2f61 7235 5f70 7562 6c69  tabase/ar5_publi
-00038f10: 635f 7665 7273 696f 6e31 3032 5f63 6f6d  c_version102_com
-00038f20: 7061 7265 5f63 6f6d 7061 7265 5f32 3031  pare_compare_201
-00038f30: 3530 3632 392d 3133 3030 3030 2e63 7376  50629-130000.csv
-00038f40: 2729 0a20 2020 2072 6561 6465 7220 3d20  ').    reader = 
-00038f50: 4949 4153 4128 0a20 2020 2020 2020 2027  IIASA(.        '
-00038f60: 4144 5641 4e43 4527 2c0a 2020 2020 2020  ADVANCE',.      
-00038f70: 2020 6461 7461 5f66 696c 653d 272f 6d65    data_file='/me
-00038f80: 6469 612f 7366 5f44 6f63 756d 656e 7473  dia/sf_Documents
-00038f90: 2f64 6174 6173 6865 6c66 5f76 3033 2f72  /datashelf_v03/r
-00038fa0: 6177 6461 7461 2f41 4456 414e 4345 5f44  awdata/ADVANCE_D
-00038fb0: 422f 4144 5641 4e43 455f 5379 6e74 6865  B/ADVANCE_Synthe
-00038fc0: 7369 735f 7665 7273 696f 6e31 3031 5f63  sis_version101_c
-00038fd0: 6f6d 7061 7265 5f32 3031 3930 3631 392d  ompare_20190619-
-00038fe0: 3134 3332 3030 2e63 7376 272c 0a20 2020  143200.csv',.   
-00038ff0: 2029 0a20 2020 2023 2072 6561 6465 7220   ).    # reader 
-00039000: 3d20 4949 4153 4128 2749 5043 435f 5352  = IIASA('IPCC_SR
-00039010: 3135 272c 2027 6961 6d63 3135 2729 0a20  15', 'iamc15'). 
-00039020: 2020 2023 2072 6561 6465 7220 3d20 4949     # reader = II
-00039030: 4153 4128 2749 5043 435f 5352 3135 272c  ASA('IPCC_SR15',
-00039040: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
-00039050: 2020 2020 2020 6461 7461 5f66 696c 6520        data_file 
-00039060: 3d27 2f6d 6564 6961 2f73 665f 446f 6375  ='/media/sf_Docu
-00039070: 6d65 6e74 732f 6461 7461 7368 656c 665f  ments/datashelf_
-00039080: 7630 332f 7261 7764 6174 612f 4941 4d43  v03/rawdata/IAMC
-00039090: 3135 5f32 3031 3962 2f69 616d 6331 355f  15_2019b/iamc15_
-000390a0: 7363 656e 6172 696f 5f64 6174 615f 616c  scenario_data_al
-000390b0: 6c5f 7265 6769 6f6e 735f 7232 2e30 2e78  l_regions_r2.0.x
-000390c0: 6c73 7827 2c0a 2020 2020 2320 2020 2020  lsx',.    #     
-000390d0: 2020 2020 2020 2020 2020 206d 6574 615f             meta_
-000390e0: 6669 6c65 203d 272f 6d65 6469 612f 7366  file ='/media/sf
-000390f0: 5f44 6f63 756d 656e 7473 2f64 6174 6173  _Documents/datas
-00039100: 6865 6c66 5f76 3033 2f72 6177 6461 7461  helf_v03/rawdata
-00039110: 2f49 414d 4331 355f 3230 3139 622f 7372  /IAMC15_2019b/sr
-00039120: 3135 5f6d 6574 6164 6174 615f 696e 6469  15_metadata_indi
-00039130: 6361 746f 7273 5f72 322e 302e 786c 7378  cators_r2.0.xlsx
-00039140: 2729 0a20 2020 2023 2073 6466 0a20 2020  ').    # sdf.   
-00039150: 2022 2222 200a 2020 2020 5072 6f63 6573   """ .    Proces
-00039160: 7320 6461 7461 3a0a 2020 2020 5468 6973  s data:.    This
-00039170: 2077 696c 6c20 7072 6f63 6573 7320 7468   will process th
-00039180: 6520 6461 7461 2061 6363 6f72 6469 6e67  e data according
-00039190: 2074 6f20 7468 6520 6d61 7070 696e 6720   to the mapping 
-000391a0: 6669 6c65 2061 6e64 2066 696c 6c20 6120  file and fill a 
-000391b0: 6c69 7374 206f 6620 0a20 2020 2074 6162  list of .    tab
-000391c0: 6c65 7320 7768 6963 6820 6172 6520 746f  les which are to
-000391d0: 2062 6520 6164 6465 6420 746f 2074 6865   be added to the
-000391e0: 2064 6174 6162 6173 652e 0a20 2020 200a   database..    .
-000391f0: 2020 2020 4578 636c 7564 6564 2074 6162      Excluded tab
-00039200: 6c65 7320 7769 6c6c 2062 6520 6c69 7374  les will be list
-00039210: 6564 2073 6570 6572 6174 656c 7920 666f  ed seperately fo
-00039220: 7220 7265 7669 6577 2e0a 2020 2020 2222  r review..    ""
-00039230: 220a 2020 2020 2320 6669 6c74 6572 5f76  ".    # filter_v
-00039240: 6172 203d 206c 616d 6264 6120 7820 3a20  ar = lambda x : 
-00039250: 616e 7928 5b78 2e73 7461 7274 7377 6974  any([x.startswit
-00039260: 6828 7661 7229 2066 6f72 2076 6172 2069  h(var) for var i
-00039270: 6e20 5b27 456d 6973 7369 6f6e 7327 2c0a  n ['Emissions',.
-00039280: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-00039290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000392a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000392b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000392c0: 2027 5072 696d 6172 7927 2c0a 2020 2020   'Primary',.    
-000392d0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+00038eb0: 3d20 4949 4153 4128 274e 4746 535f 3230  = IIASA('NGFS_20
+00038ec0: 3231 272c 2027 6e67 6673 5f32 2729 0a20  21', 'ngfs_2'). 
+00038ed0: 2020 2023 2072 6561 6465 7220 3d20 4949     # reader = II
+00038ee0: 4153 4128 2743 445f 4c49 4e4b 5327 2c20  ASA('CD_LINKS', 
+00038ef0: 2763 646c 696e 6b73 2729 0a20 2020 2023  'cdlinks').    #
+00038f00: 2072 6561 6465 7220 3d20 4949 4153 4128   reader = IIASA(
+00038f10: 2749 5043 435f 4152 3527 2c20 6461 7461  'IPCC_AR5', data
+00038f20: 5f66 696c 6520 3d27 2f6d 6564 6961 2f73  _file ='/media/s
+00038f30: 665f 446f 6375 6d65 6e74 732f 6461 7461  f_Documents/data
+00038f40: 7368 656c 665f 7630 332f 7261 7764 6174  shelf_v03/rawdat
+00038f50: 612f 4152 355f 6461 7461 6261 7365 2f61  a/AR5_database/a
+00038f60: 7235 5f70 7562 6c69 635f 7665 7273 696f  r5_public_versio
+00038f70: 6e31 3032 5f63 6f6d 7061 7265 5f63 6f6d  n102_compare_com
+00038f80: 7061 7265 5f32 3031 3530 3632 392d 3133  pare_20150629-13
+00038f90: 3030 3030 2e63 7376 2729 0a20 2020 2072  0000.csv').    r
+00038fa0: 6561 6465 7220 3d20 4949 4153 4128 0a20  eader = IIASA(. 
+00038fb0: 2020 2020 2020 2027 4144 5641 4e43 4527         'ADVANCE'
+00038fc0: 2c0a 2020 2020 2020 2020 6461 7461 5f66  ,.        data_f
+00038fd0: 696c 653d 272f 6d65 6469 612f 7366 5f44  ile='/media/sf_D
+00038fe0: 6f63 756d 656e 7473 2f64 6174 6173 6865  ocuments/datashe
+00038ff0: 6c66 5f76 3033 2f72 6177 6461 7461 2f41  lf_v03/rawdata/A
+00039000: 4456 414e 4345 5f44 422f 4144 5641 4e43  DVANCE_DB/ADVANC
+00039010: 455f 5379 6e74 6865 7369 735f 7665 7273  E_Synthesis_vers
+00039020: 696f 6e31 3031 5f63 6f6d 7061 7265 5f32  ion101_compare_2
+00039030: 3031 3930 3631 392d 3134 3332 3030 2e63  0190619-143200.c
+00039040: 7376 272c 0a20 2020 2029 0a20 2020 2023  sv',.    ).    #
+00039050: 2072 6561 6465 7220 3d20 4949 4153 4128   reader = IIASA(
+00039060: 2749 5043 435f 5352 3135 272c 2027 6961  'IPCC_SR15', 'ia
+00039070: 6d63 3135 2729 0a20 2020 2023 2072 6561  mc15').    # rea
+00039080: 6465 7220 3d20 4949 4153 4128 2749 5043  der = IIASA('IPC
+00039090: 435f 5352 3135 272c 0a20 2020 2023 2020  C_SR15',.    #  
+000390a0: 2020 2020 2020 2020 2020 2020 2020 6461                da
+000390b0: 7461 5f66 696c 6520 3d27 2f6d 6564 6961  ta_file ='/media
+000390c0: 2f73 665f 446f 6375 6d65 6e74 732f 6461  /sf_Documents/da
+000390d0: 7461 7368 656c 665f 7630 332f 7261 7764  tashelf_v03/rawd
+000390e0: 6174 612f 4941 4d43 3135 5f32 3031 3962  ata/IAMC15_2019b
+000390f0: 2f69 616d 6331 355f 7363 656e 6172 696f  /iamc15_scenario
+00039100: 5f64 6174 615f 616c 6c5f 7265 6769 6f6e  _data_all_region
+00039110: 735f 7232 2e30 2e78 6c73 7827 2c0a 2020  s_r2.0.xlsx',.  
+00039120: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+00039130: 2020 206d 6574 615f 6669 6c65 203d 272f     meta_file ='/
+00039140: 6d65 6469 612f 7366 5f44 6f63 756d 656e  media/sf_Documen
+00039150: 7473 2f64 6174 6173 6865 6c66 5f76 3033  ts/datashelf_v03
+00039160: 2f72 6177 6461 7461 2f49 414d 4331 355f  /rawdata/IAMC15_
+00039170: 3230 3139 622f 7372 3135 5f6d 6574 6164  2019b/sr15_metad
+00039180: 6174 615f 696e 6469 6361 746f 7273 5f72  ata_indicators_r
+00039190: 322e 302e 786c 7378 2729 0a20 2020 2023  2.0.xlsx').    #
+000391a0: 2073 6466 0a20 2020 2022 2222 200a 2020   sdf.    """ .  
+000391b0: 2020 5072 6f63 6573 7320 6461 7461 3a0a    Process data:.
+000391c0: 2020 2020 5468 6973 2077 696c 6c20 7072      This will pr
+000391d0: 6f63 6573 7320 7468 6520 6461 7461 2061  ocess the data a
+000391e0: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
+000391f0: 6d61 7070 696e 6720 6669 6c65 2061 6e64  mapping file and
+00039200: 2066 696c 6c20 6120 6c69 7374 206f 6620   fill a list of 
+00039210: 0a20 2020 2074 6162 6c65 7320 7768 6963  .    tables whic
+00039220: 6820 6172 6520 746f 2062 6520 6164 6465  h are to be adde
+00039230: 6420 746f 2074 6865 2064 6174 6162 6173  d to the databas
+00039240: 652e 0a20 2020 200a 2020 2020 4578 636c  e..    .    Excl
+00039250: 7564 6564 2074 6162 6c65 7320 7769 6c6c  uded tables will
+00039260: 2062 6520 6c69 7374 6564 2073 6570 6572   be listed seper
+00039270: 6174 656c 7920 666f 7220 7265 7669 6577  ately for review
+00039280: 2e0a 2020 2020 2222 220a 2020 2020 2320  ..    """.    # 
+00039290: 6669 6c74 6572 5f76 6172 203d 206c 616d  filter_var = lam
+000392a0: 6264 6120 7820 3a20 616e 7928 5b78 2e73  bda x : any([x.s
+000392b0: 7461 7274 7377 6974 6828 7661 7229 2066  tartswith(var) f
+000392c0: 6f72 2076 6172 2069 6e20 5b27 456d 6973  or var in ['Emis
+000392d0: 7369 6f6e 7327 2c0a 2020 2020 2320 2020  sions',.    #   
 000392e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000392f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00039300: 2020 2020 2020 2020 2020 2020 2027 5365               'Se
-00039310: 636f 6e64 6172 7927 0a20 2020 2023 2020  condary'.    #  
-00039320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00039300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00039310: 2020 2020 2020 2020 2027 5072 696d 6172           'Primar
+00039320: 7927 2c0a 2020 2020 2320 2020 2020 2020  y',.    #       
 00039330: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00039340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00039350: 2020 2020 2020 2020 2020 2747 4450 272c            'GDP',
-00039360: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
-00039370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00039350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00039360: 2020 2020 2027 5365 636f 6e64 6172 7927       'Secondary'
+00039370: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
 00039380: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00039390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000393a0: 2020 2750 6f70 756c 6174 696f 6e27 5d5d    'Population']]
-000393b0: 290a 2020 2020 6961 6d63 5f66 696c 7465  ).    iamc_filte
-000393c0: 7220 3d20 7b0a 2020 2020 2020 2020 2320  r = {.        # 
-000393d0: 2776 6172 6961 626c 6527 203a 205b 0a20  'variable' : [. 
-000393e0: 2020 2020 2020 2023 2027 456d 6973 7369         # 'Emissi
-000393f0: 6f6e 732a 2a27 2c0a 2020 2020 2020 2020  ons**',.        
-00039400: 2320 2750 7269 6d61 7279 2a2a 272c 0a20  # 'Primary**',. 
-00039410: 2020 2020 2020 2023 2027 5365 636f 6e64         # 'Second
-00039420: 6172 792a 2a27 0a20 2020 2020 2020 2023  ary**'.        #
-00039430: 2027 4744 502a 2a27 2c0a 2020 2020 2020   'GDP**',.      
-00039440: 2020 2320 2750 6f70 756c 6174 696f 6e2a    # 'Population*
-00039450: 2a27 0a20 2020 2020 2020 2023 2027 5375  *'.        # 'Su
-00039460: 6273 6964 6965 732a 2a27 2c0a 2020 2020  bsidies**',.    
-00039470: 2020 2020 2320 2750 7269 6365 2a2a 272c      # 'Price**',
-00039480: 0a20 2020 2020 2020 2023 2027 496e 7665  .        # 'Inve
-00039490: 7374 6d65 6e74 732a 2a27 2c0a 2020 2020  stments**',.    
-000394a0: 2020 2020 2320 2743 6172 626f 6e20 5365      # 'Carbon Se
-000394b0: 7175 6573 7472 6174 696f 2a2a 272c 0a20  questratio**',. 
-000394c0: 2020 2020 2020 2023 2027 4361 7061 6369         # 'Capaci
-000394d0: 7479 2a2a 272c 0a20 2020 2020 2020 2023  ty**',.        #
-000394e0: 2027 4375 6d75 6c61 7469 7665 2043 6170   'Cumulative Cap
-000394f0: 6163 6974 792a 2a27 0a20 2020 2020 2020  acity**'.       
-00039500: 2023 205d 0a20 2020 207d 0a20 2020 2023   # ].    }.    #
-00039510: 206d 6f64 656c 7320 3d20 5b27 4149 4d2f   models = ['AIM/
-00039520: 4875 622d 496e 6469 6120 322e 3227 2c0a  Hub-India 2.2',.
-00039530: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-00039540: 2741 494d 2f48 7562 2d54 6861 696c 616e  'AIM/Hub-Thailan
-00039550: 6420 322e 3227 2c0a 2020 2020 2320 2020  d 2.2',.    #   
-00039560: 2020 2020 2020 2020 2741 494d 2f48 7562          'AIM/Hub
-00039570: 2d4a 6170 616e 2032 2e31 272c 0a20 2020  -Japan 2.1',.   
-00039580: 2023 2020 2020 2020 2020 2020 2020 2027   #             '
-00039590: 4149 4d2f 4875 622d 4368 696e 6120 322e  AIM/Hub-China 2.
-000395a0: 3227 2c0a 2020 2020 2320 2020 2020 2020  2',.    #       
-000395b0: 2020 2020 2020 2741 494d 2f48 7562 2d4b        'AIM/Hub-K
-000395c0: 6f72 6561 2032 2e30 272c 0a20 2020 2023  orea 2.0',.    #
-000395d0: 2020 2020 2020 2020 2020 2020 2027 4149               'AI
-000395e0: 4d2f 4875 622d 5669 6574 6e61 6d20 322e  M/Hub-Vietnam 2.
-000395f0: 3227 2c0a 2020 2020 2320 2020 2020 2020  2',.    #       
-00039600: 2020 2020 2020 2741 494d 2f43 4745 2056        'AIM/CGE V
-00039610: 322e 3227 2c0a 2020 2020 2320 2020 2020  2.2',.    #     
-00039620: 2020 2020 2020 2020 2743 4f46 4645 4520          'COFFEE 
-00039630: 312e 3127 5d0a 2020 2020 2320 6d6f 6465  1.1'].    # mode
-00039640: 6c73 203d 205b 2754 4941 4d2d 4543 4e20  ls = ['TIAM-ECN 
-00039650: 312e 3127 2c0a 2020 2020 2320 2020 2020  1.1',.    #     
-00039660: 274d 4553 5341 4745 6978 2d47 4c4f 4249  'MESSAGEix-GLOBI
-00039670: 4f4d 2056 312e 3227 2c20 274d 4553 5341  OM V1.2', 'MESSA
-00039680: 4745 6978 2d47 4c4f 4249 4f4d 2031 2e31  GEix-GLOBIOM 1.1
-00039690: 272c 2027 5749 5443 4820 352e 3027 2c0a  ', 'WITCH 5.0',.
-000396a0: 2020 2020 2320 2020 2020 2747 454d 2d45      #     'GEM-E
-000396b0: 3320 5632 3032 3127 2c20 2752 454d 494e  3 V2021', 'REMIN
-000396c0: 442d 4d41 6750 4945 2032 2e31 2d34 2e32  D-MAgPIE 2.1-4.2
-000396d0: 272c 2027 494d 4147 4520 332e 3027 2c0a  ', 'IMAGE 3.0',.
-000396e0: 2020 2020 2320 2020 2020 2750 4f4c 4553      #     'POLES
-000396f0: 2d4a 5243 2045 4e47 4147 4527 5d0a 0a20  -JRC ENGAGE'].. 
-00039700: 2020 2023 2069 616d 635f 6669 6c74 6572     # iamc_filter
-00039710: 203d 207b 2776 6172 6961 626c 6527 203a   = {'variable' :
-00039720: 205b 0a20 2020 2023 2020 2020 2020 2020   [.    #        
-00039730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00039740: 2027 456d 6973 7369 6f6e 737c 434f 3227   'Emissions|CO2'
-00039750: 2c0a 2020 2020 2320 2020 2020 2020 2020  ,.    #         
-00039760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00039770: 2745 6d69 7373 696f 6e73 7c43 4834 272c  'Emissions|CH4',
-00039780: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
-00039790: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000397a0: 456d 6973 7369 6f6e 737c 4e32 4f27 2c0a  Emissions|N2O',.
-000397b0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-000397c0: 2020 2020 2020 2020 2020 2020 2020 2745                'E
-000397d0: 6d69 7373 696f 6e73 7c46 2d47 6173 6573  missions|F-Gases
-000397e0: 272c 0a20 2020 2023 2020 2020 2020 2020  ',.    #        
-000397f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00039800: 2027 456d 6973 7369 6f6e 737c 4b79 6f2a   'Emissions|Kyo*
-00039810: 2a27 5d7d 0a20 2020 206d 6f64 656c 7320  *']}.    models 
-00039820: 3d20 4e6f 6e65 0a20 2020 2023 2074 6162  = None.    # tab
-00039830: 6c65 735f 746f 5f63 6f6d 6d69 742c 2065  les_to_commit, e
-00039840: 7863 6c75 6465 6454 6162 6c65 7320 3d20  xcludedTables = 
-00039850: 7265 6164 6572 2e67 6174 6865 724d 6170  reader.gatherMap
-00039860: 7065 6444 6174 615f 7465 7374 286d 6f64  pedData_test(mod
-00039870: 656c 732c 2069 616d 635f 6669 6c74 6572  els, iamc_filter
-00039880: 3d69 616d 635f 6669 6c74 6572 290a 2020  =iamc_filter).  
-00039890: 2020 7461 626c 6573 5f74 6f5f 636f 6d6d    tables_to_comm
-000398a0: 6974 2c20 6578 636c 7564 6564 5461 626c  it, excludedTabl
-000398b0: 6573 203d 2072 6561 6465 722e 6761 7468  es = reader.gath
-000398c0: 6572 4d61 7070 6564 4461 7461 2869 616d  erMappedData(iam
+000393a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000393b0: 2020 2747 4450 272c 0a20 2020 2023 2020    'GDP',.    #  
+000393c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000393d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000393e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000393f0: 2020 2020 2020 2020 2020 2750 6f70 756c            'Popul
+00039400: 6174 696f 6e27 5d5d 290a 2020 2020 6961  ation']]).    ia
+00039410: 6d63 5f66 696c 7465 7220 3d20 7b0a 2020  mc_filter = {.  
+00039420: 2020 2020 2020 2320 2776 6172 6961 626c        # 'variabl
+00039430: 6527 203a 205b 0a20 2020 2020 2020 2023  e' : [.        #
+00039440: 2027 456d 6973 7369 6f6e 732a 2a27 2c0a   'Emissions**',.
+00039450: 2020 2020 2020 2020 2320 2750 7269 6d61          # 'Prima
+00039460: 7279 2a2a 272c 0a20 2020 2020 2020 2023  ry**',.        #
+00039470: 2027 5365 636f 6e64 6172 792a 2a27 0a20   'Secondary**'. 
+00039480: 2020 2020 2020 2023 2027 4744 502a 2a27         # 'GDP**'
+00039490: 2c0a 2020 2020 2020 2020 2320 2750 6f70  ,.        # 'Pop
+000394a0: 756c 6174 696f 6e2a 2a27 0a20 2020 2020  ulation**'.     
+000394b0: 2020 2023 2027 5375 6273 6964 6965 732a     # 'Subsidies*
+000394c0: 2a27 2c0a 2020 2020 2020 2020 2320 2750  *',.        # 'P
+000394d0: 7269 6365 2a2a 272c 0a20 2020 2020 2020  rice**',.       
+000394e0: 2023 2027 496e 7665 7374 6d65 6e74 732a   # 'Investments*
+000394f0: 2a27 2c0a 2020 2020 2020 2020 2320 2743  *',.        # 'C
+00039500: 6172 626f 6e20 5365 7175 6573 7472 6174  arbon Sequestrat
+00039510: 696f 2a2a 272c 0a20 2020 2020 2020 2023  io**',.        #
+00039520: 2027 4361 7061 6369 7479 2a2a 272c 0a20   'Capacity**',. 
+00039530: 2020 2020 2020 2023 2027 4375 6d75 6c61         # 'Cumula
+00039540: 7469 7665 2043 6170 6163 6974 792a 2a27  tive Capacity**'
+00039550: 0a20 2020 2020 2020 2023 205d 0a20 2020  .        # ].   
+00039560: 207d 0a20 2020 2023 206d 6f64 656c 7320   }.    # models 
+00039570: 3d20 5b27 4149 4d2f 4875 622d 496e 6469  = ['AIM/Hub-Indi
+00039580: 6120 322e 3227 2c0a 2020 2020 2320 2020  a 2.2',.    #   
+00039590: 2020 2020 2020 2020 2741 494d 2f48 7562          'AIM/Hub
+000395a0: 2d54 6861 696c 616e 6420 322e 3227 2c0a  -Thailand 2.2',.
+000395b0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+000395c0: 2741 494d 2f48 7562 2d4a 6170 616e 2032  'AIM/Hub-Japan 2
+000395d0: 2e31 272c 0a20 2020 2023 2020 2020 2020  .1',.    #      
+000395e0: 2020 2020 2020 2027 4149 4d2f 4875 622d         'AIM/Hub-
+000395f0: 4368 696e 6120 322e 3227 2c0a 2020 2020  China 2.2',.    
+00039600: 2320 2020 2020 2020 2020 2020 2020 2741  #             'A
+00039610: 494d 2f48 7562 2d4b 6f72 6561 2032 2e30  IM/Hub-Korea 2.0
+00039620: 272c 0a20 2020 2023 2020 2020 2020 2020  ',.    #        
+00039630: 2020 2020 2027 4149 4d2f 4875 622d 5669       'AIM/Hub-Vi
+00039640: 6574 6e61 6d20 322e 3227 2c0a 2020 2020  etnam 2.2',.    
+00039650: 2320 2020 2020 2020 2020 2020 2020 2741  #             'A
+00039660: 494d 2f43 4745 2056 322e 3227 2c0a 2020  IM/CGE V2.2',.  
+00039670: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+00039680: 2743 4f46 4645 4520 312e 3127 5d0a 2020  'COFFEE 1.1'].  
+00039690: 2020 2320 6d6f 6465 6c73 203d 205b 2754    # models = ['T
+000396a0: 4941 4d2d 4543 4e20 312e 3127 2c0a 2020  IAM-ECN 1.1',.  
+000396b0: 2020 2320 2020 2020 274d 4553 5341 4745    #     'MESSAGE
+000396c0: 6978 2d47 4c4f 4249 4f4d 2056 312e 3227  ix-GLOBIOM V1.2'
+000396d0: 2c20 274d 4553 5341 4745 6978 2d47 4c4f  , 'MESSAGEix-GLO
+000396e0: 4249 4f4d 2031 2e31 272c 2027 5749 5443  BIOM 1.1', 'WITC
+000396f0: 4820 352e 3027 2c0a 2020 2020 2320 2020  H 5.0',.    #   
+00039700: 2020 2747 454d 2d45 3320 5632 3032 3127    'GEM-E3 V2021'
+00039710: 2c20 2752 454d 494e 442d 4d41 6750 4945  , 'REMIND-MAgPIE
+00039720: 2032 2e31 2d34 2e32 272c 2027 494d 4147   2.1-4.2', 'IMAG
+00039730: 4520 332e 3027 2c0a 2020 2020 2320 2020  E 3.0',.    #   
+00039740: 2020 2750 4f4c 4553 2d4a 5243 2045 4e47    'POLES-JRC ENG
+00039750: 4147 4527 5d0a 0a20 2020 2023 2069 616d  AGE']..    # iam
+00039760: 635f 6669 6c74 6572 203d 207b 2776 6172  c_filter = {'var
+00039770: 6961 626c 6527 203a 205b 0a20 2020 2023  iable' : [.    #
+00039780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00039790: 2020 2020 2020 2020 2027 456d 6973 7369           'Emissi
+000397a0: 6f6e 737c 434f 3227 2c0a 2020 2020 2320  ons|CO2',.    # 
+000397b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000397c0: 2020 2020 2020 2020 2745 6d69 7373 696f          'Emissio
+000397d0: 6e73 7c43 4834 272c 0a20 2020 2023 2020  ns|CH4',.    #  
+000397e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000397f0: 2020 2020 2020 2027 456d 6973 7369 6f6e         'Emission
+00039800: 737c 4e32 4f27 2c0a 2020 2020 2320 2020  s|N2O',.    #   
+00039810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00039820: 2020 2020 2020 2745 6d69 7373 696f 6e73        'Emissions
+00039830: 7c46 2d47 6173 6573 272c 0a20 2020 2023  |F-Gases',.    #
+00039840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00039850: 2020 2020 2020 2020 2027 456d 6973 7369           'Emissi
+00039860: 6f6e 737c 4b79 6f2a 2a27 5d7d 0a20 2020  ons|Kyo**']}.   
+00039870: 206d 6f64 656c 7320 3d20 4e6f 6e65 0a20   models = None. 
+00039880: 2020 2023 2074 6162 6c65 735f 746f 5f63     # tables_to_c
+00039890: 6f6d 6d69 742c 2065 7863 6c75 6465 6454  ommit, excludedT
+000398a0: 6162 6c65 7320 3d20 7265 6164 6572 2e67  ables = reader.g
+000398b0: 6174 6865 724d 6170 7065 6444 6174 615f  atherMappedData_
+000398c0: 7465 7374 286d 6f64 656c 732c 2069 616d  test(models, iam
 000398d0: 635f 6669 6c74 6572 3d69 616d 635f 6669  c_filter=iamc_fi
-000398e0: 6c74 6572 290a 0a20 2020 2023 2046 6f72  lter)..    # For
-000398f0: 2072 6576 6965 773a 0a20 2020 2023 2074   review:.    # t
-00039900: 6162 6c65 4944 7320 3d20 5b74 6162 6c65  ableIDs = [table
-00039910: 2e49 4420 666f 7220 7461 626c 6520 696e  .ID for table in
-00039920: 2074 6162 6c65 4c69 7374 5d0a 2020 2020   tableList].    
-00039930: 2320 636c 6561 6e54 6162 6c65 4c69 7374  # cleanTableList
-00039940: 203d 205b 6474 2e74 6f6f 6c73 2e63 6c65   = [dt.tools.cle
-00039950: 616e 4461 7461 5461 626c 6528 7461 626c  anDataTable(tabl
-00039960: 6529 2066 6f72 2074 6162 6c65 2069 6e20  e) for table in 
-00039970: 7461 626c 654c 6973 740a 0a20 2020 2023  tableList..    #
-00039980: 2066 696e 6420 656d 7074 7920 7461 626c   find empty tabl
-00039990: 7365 0a20 2020 2023 205b 782e 4944 2066  se.    # [x.ID f
-000399a0: 6f72 2078 2069 6e20 7461 626c 654c 6973  or x in tableLis
-000399b0: 7420 6966 206c 656e 2878 2e69 6e64 6578  t if len(x.index
-000399c0: 2920 3d3d 305d 0a0a 2020 2020 2325 250a  ) ==0]..    #%%.
-000399d0: 2020 2020 2320 6e65 775f 6578 636c 7564      # new_exclud
-000399e0: 655f 7461 626c 6573 203d 206c 6973 7428  e_tables = list(
-000399f0: 290a 2020 2020 2320 6e65 775f 7461 626c  ).    # new_tabl
-00039a00: 6573 5f74 6f5f 636f 6d6d 6974 203d 206c  es_to_commit = l
-00039a10: 6973 7428 290a 2020 2020 2320 666f 7220  ist().    # for 
-00039a20: 7461 626c 6520 696e 2065 7863 6c75 6465  table in exclude
-00039a30: 6454 6162 6c65 733a 0a20 2020 2023 2020  dTables:.    #  
-00039a40: 2020 2074 6162 6c65 2e6d 6574 6120 3d20     table.meta = 
-00039a50: 6164 6170 745f 6d65 7461 2874 6162 6c65  adapt_meta(table
-00039a60: 2e6d 6574 6129 0a0a 2020 2020 2320 2020  .meta)..    #   
-00039a70: 2020 6966 2064 742e 636f 7265 2e63 6865    if dt.core.che
-00039a80: 636b 5f74 6162 6c65 2874 6162 6c65 293a  ck_table(table):
-00039a90: 0a20 2020 2023 2020 2020 2020 2020 206e  .    #         n
-00039aa0: 6577 5f65 7863 6c75 6465 5f74 6162 6c65  ew_exclude_table
-00039ab0: 732e 6170 7065 6e64 2874 6162 6c65 290a  s.append(table).
-00039ac0: 2020 2020 2320 2020 2020 656c 7365 3a0a      #     else:.
-00039ad0: 2020 2020 2320 2020 2020 2020 2020 6e65      #         ne
-00039ae0: 775f 7461 626c 6573 5f74 6f5f 636f 6d6d  w_tables_to_comm
-00039af0: 6974 2e61 7070 656e 6428 7461 626c 6529  it.append(table)
-00039b00: 0a20 2020 2023 2023 2525 0a20 2020 2023  .    # #%%.    #
-00039b10: 2020 2063 6f6d 7061 7265 5f72 6567 696f     compare_regio
-00039b20: 6e73 203d 2073 6574 2829 0a20 2020 2023  ns = set().    #
-00039b30: 2020 2066 6f72 2074 6162 6c65 2069 6e20     for table in 
-00039b40: 7461 626c 6573 5f74 6f5f 636f 6d6d 6974  tables_to_commit
-00039b50: 3a0a 2020 2020 2320 2020 2020 2020 636f  :.    #       co
-00039b60: 6d70 6172 655f 7265 6769 6f6e 735f 7461  mpare_regions_ta
-00039b70: 626c 6520 3d20 5b78 2066 6f72 2078 2069  ble = [x for x i
-00039b80: 6e20 7461 626c 652e 696e 6465 7820 6966  n table.index if
-00039b90: 2027 2852 2720 696e 2078 5d0a 2020 2020   '(R' in x].    
-00039ba0: 2320 2020 2020 2020 636f 6d70 6172 655f  #       compare_
-00039bb0: 7265 6769 6f6e 7320 3d20 636f 6d70 6172  regions = compar
-00039bc0: 655f 7265 6769 6f6e 732e 756e 696f 6e28  e_regions.union(
-00039bd0: 7365 7428 636f 6d70 6172 655f 7265 6769  set(compare_regi
-00039be0: 6f6e 735f 7461 626c 6529 290a 0a20 2020  ons_table))..   
-00039bf0: 2023 2020 2023 2525 0a20 2020 2023 2020   #   #%%.    #  
-00039c00: 2066 6f72 2074 6162 6c65 2069 6e20 7461   for table in ta
-00039c10: 626c 6573 5f74 6f5f 636f 6d6d 6974 3a0a  bles_to_commit:.
-00039c20: 2020 2020 2320 2020 2020 2020 7461 626c      #       tabl
-00039c30: 6520 203d 2073 656c 662e 6164 645f 7374  e  = self.add_st
-00039c40: 616e 6461 7264 5f72 6567 696f 6e28 7461  andard_region(ta
-00039c50: 626c 652c 2073 656c 662e 7265 6769 6f6e  ble, self.region
-00039c60: 5f6d 6170 7069 6e67 5b27 656e 6761 6765  _mapping['engage
-00039c70: 275d 290a 2020 2020 2320 2020 2020 2020  ']).    #       
-00039c80: 7364 660a 2020 2020 2325 250a 2020 2020  sdf.    #%%.    
-00039c90: 2320 6465 6620 7374 616e 6461 7264 6973  # def standardis
-00039ca0: 655f 7265 6769 6f6e 7328 7461 626c 6529  e_regions(table)
-00039cb0: 3a0a 0a20 2020 2023 2525 0a20 2020 2023  :..    #%%.    #
-00039cc0: 2022 2222 0a20 2020 2023 2055 7064 6174   """.    # Updat
-00039cd0: 6520 6461 7461 6261 7365 3a0a 0a20 2020  e database:..   
-00039ce0: 2023 2054 6869 7320 7769 6c6c 2061 6464   # This will add
-00039cf0: 2074 6865 2074 6162 6c65 7320 696e 2074   the tables in t
-00039d00: 6865 206c 6973 7420 746f 2074 6865 2064  he list to the d
-00039d10: 6174 6162 6173 6520 616e 6420 7769 6c6c  atabase and will
-00039d20: 2061 6c73 6f20 6164 6420 7468 650a 2020   also add the.  
-00039d30: 2020 2320 6d61 7070 696e 6720 6669 6c65    # mapping file
-00039d40: 2074 6f20 7468 6520 7265 706f 7369 746f   to the reposito
-00039d50: 7279 2e0a 2020 2020 2320 2222 220a 0a20  ry..    # """.. 
-00039d60: 2020 2072 6561 6465 722e 7570 6461 7465     reader.update
-00039d70: 5f64 6174 6162 6173 6528 7461 626c 6573  _database(tables
-00039d80: 5f74 6f5f 636f 6d6d 6974 2c20 7570 6461  _to_commit, upda
-00039d90: 7465 436f 6e74 656e 743d 4661 6c73 6529  teContent=False)
-00039da0: 0a0a 2325 250a                           ..#%%.
+000398e0: 6c74 6572 290a 2020 2020 7461 626c 6573  lter).    tables
+000398f0: 5f74 6f5f 636f 6d6d 6974 2c20 6578 636c  _to_commit, excl
+00039900: 7564 6564 5461 626c 6573 203d 2072 6561  udedTables = rea
+00039910: 6465 722e 6761 7468 6572 4d61 7070 6564  der.gatherMapped
+00039920: 4461 7461 2869 616d 635f 6669 6c74 6572  Data(iamc_filter
+00039930: 3d69 616d 635f 6669 6c74 6572 290a 0a20  =iamc_filter).. 
+00039940: 2020 2023 2046 6f72 2072 6576 6965 773a     # For review:
+00039950: 0a20 2020 2023 2074 6162 6c65 4944 7320  .    # tableIDs 
+00039960: 3d20 5b74 6162 6c65 2e49 4420 666f 7220  = [table.ID for 
+00039970: 7461 626c 6520 696e 2074 6162 6c65 4c69  table in tableLi
+00039980: 7374 5d0a 2020 2020 2320 636c 6561 6e54  st].    # cleanT
+00039990: 6162 6c65 4c69 7374 203d 205b 6474 2e74  ableList = [dt.t
+000399a0: 6f6f 6c73 2e63 6c65 616e 4461 7461 5461  ools.cleanDataTa
+000399b0: 626c 6528 7461 626c 6529 2066 6f72 2074  ble(table) for t
+000399c0: 6162 6c65 2069 6e20 7461 626c 654c 6973  able in tableLis
+000399d0: 740a 0a20 2020 2023 2066 696e 6420 656d  t..    # find em
+000399e0: 7074 7920 7461 626c 7365 0a20 2020 2023  pty tablse.    #
+000399f0: 205b 782e 4944 2066 6f72 2078 2069 6e20   [x.ID for x in 
+00039a00: 7461 626c 654c 6973 7420 6966 206c 656e  tableList if len
+00039a10: 2878 2e69 6e64 6578 2920 3d3d 305d 0a0a  (x.index) ==0]..
+00039a20: 2020 2020 2325 250a 2020 2020 2320 6e65      #%%.    # ne
+00039a30: 775f 6578 636c 7564 655f 7461 626c 6573  w_exclude_tables
+00039a40: 203d 206c 6973 7428 290a 2020 2020 2320   = list().    # 
+00039a50: 6e65 775f 7461 626c 6573 5f74 6f5f 636f  new_tables_to_co
+00039a60: 6d6d 6974 203d 206c 6973 7428 290a 2020  mmit = list().  
+00039a70: 2020 2320 666f 7220 7461 626c 6520 696e    # for table in
+00039a80: 2065 7863 6c75 6465 6454 6162 6c65 733a   excludedTables:
+00039a90: 0a20 2020 2023 2020 2020 2074 6162 6c65  .    #     table
+00039aa0: 2e6d 6574 6120 3d20 6164 6170 745f 6d65  .meta = adapt_me
+00039ab0: 7461 2874 6162 6c65 2e6d 6574 6129 0a0a  ta(table.meta)..
+00039ac0: 2020 2020 2320 2020 2020 6966 2064 742e      #     if dt.
+00039ad0: 636f 7265 2e63 6865 636b 5f74 6162 6c65  core.check_table
+00039ae0: 2874 6162 6c65 293a 0a20 2020 2023 2020  (table):.    #  
+00039af0: 2020 2020 2020 206e 6577 5f65 7863 6c75         new_exclu
+00039b00: 6465 5f74 6162 6c65 732e 6170 7065 6e64  de_tables.append
+00039b10: 2874 6162 6c65 290a 2020 2020 2320 2020  (table).    #   
+00039b20: 2020 656c 7365 3a0a 2020 2020 2320 2020    else:.    #   
+00039b30: 2020 2020 2020 6e65 775f 7461 626c 6573        new_tables
+00039b40: 5f74 6f5f 636f 6d6d 6974 2e61 7070 656e  _to_commit.appen
+00039b50: 6428 7461 626c 6529 0a20 2020 2023 2023  d(table).    # #
+00039b60: 2525 0a20 2020 2023 2020 2063 6f6d 7061  %%.    #   compa
+00039b70: 7265 5f72 6567 696f 6e73 203d 2073 6574  re_regions = set
+00039b80: 2829 0a20 2020 2023 2020 2066 6f72 2074  ().    #   for t
+00039b90: 6162 6c65 2069 6e20 7461 626c 6573 5f74  able in tables_t
+00039ba0: 6f5f 636f 6d6d 6974 3a0a 2020 2020 2320  o_commit:.    # 
+00039bb0: 2020 2020 2020 636f 6d70 6172 655f 7265        compare_re
+00039bc0: 6769 6f6e 735f 7461 626c 6520 3d20 5b78  gions_table = [x
+00039bd0: 2066 6f72 2078 2069 6e20 7461 626c 652e   for x in table.
+00039be0: 696e 6465 7820 6966 2027 2852 2720 696e  index if '(R' in
+00039bf0: 2078 5d0a 2020 2020 2320 2020 2020 2020   x].    #       
+00039c00: 636f 6d70 6172 655f 7265 6769 6f6e 7320  compare_regions 
+00039c10: 3d20 636f 6d70 6172 655f 7265 6769 6f6e  = compare_region
+00039c20: 732e 756e 696f 6e28 7365 7428 636f 6d70  s.union(set(comp
+00039c30: 6172 655f 7265 6769 6f6e 735f 7461 626c  are_regions_tabl
+00039c40: 6529 290a 0a20 2020 2023 2020 2023 2525  e))..    #   #%%
+00039c50: 0a20 2020 2023 2020 2066 6f72 2074 6162  .    #   for tab
+00039c60: 6c65 2069 6e20 7461 626c 6573 5f74 6f5f  le in tables_to_
+00039c70: 636f 6d6d 6974 3a0a 2020 2020 2320 2020  commit:.    #   
+00039c80: 2020 2020 7461 626c 6520 203d 2073 656c      table  = sel
+00039c90: 662e 6164 645f 7374 616e 6461 7264 5f72  f.add_standard_r
+00039ca0: 6567 696f 6e28 7461 626c 652c 2073 656c  egion(table, sel
+00039cb0: 662e 7265 6769 6f6e 5f6d 6170 7069 6e67  f.region_mapping
+00039cc0: 5b27 656e 6761 6765 275d 290a 2020 2020  ['engage']).    
+00039cd0: 2320 2020 2020 2020 7364 660a 2020 2020  #       sdf.    
+00039ce0: 2325 250a 2020 2020 2320 6465 6620 7374  #%%.    # def st
+00039cf0: 616e 6461 7264 6973 655f 7265 6769 6f6e  andardise_region
+00039d00: 7328 7461 626c 6529 3a0a 0a20 2020 2023  s(table):..    #
+00039d10: 2525 0a20 2020 2023 2022 2222 0a20 2020  %%.    # """.   
+00039d20: 2023 2055 7064 6174 6520 6461 7461 6261   # Update databa
+00039d30: 7365 3a0a 0a20 2020 2023 2054 6869 7320  se:..    # This 
+00039d40: 7769 6c6c 2061 6464 2074 6865 2074 6162  will add the tab
+00039d50: 6c65 7320 696e 2074 6865 206c 6973 7420  les in the list 
+00039d60: 746f 2074 6865 2064 6174 6162 6173 6520  to the database 
+00039d70: 616e 6420 7769 6c6c 2061 6c73 6f20 6164  and will also ad
+00039d80: 6420 7468 650a 2020 2020 2320 6d61 7070  d the.    # mapp
+00039d90: 696e 6720 6669 6c65 2074 6f20 7468 6520  ing file to the 
+00039da0: 7265 706f 7369 746f 7279 2e0a 2020 2020  repository..    
+00039db0: 2320 2222 220a 0a20 2020 2072 6561 6465  # """..    reade
+00039dc0: 722e 7570 6461 7465 5f64 6174 6162 6173  r.update_databas
+00039dd0: 6528 7461 626c 6573 5f74 6f5f 636f 6d6d  e(tables_to_comm
+00039de0: 6974 2c20 7570 6461 7465 436f 6e74 656e  it, updateConten
+00039df0: 743d 4661 6c73 6529 0a0a 2325 250a       t=False)..#%%.
```

### Comparing `datatoolbox-0.5.4/datatoolbox/data_structures.py` & `datatoolbox-0.5.5/datatoolbox/data_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 by any computations using datatables.
 """
 
 import pandas as pd
 import matplotlib.pylab as plt
 import numpy as np
 import xarray as xr
-from copy import copy
+import pint
+from copy import copy, deepcopy
 import ast
 from . import core
 from . import config
 import traceback
 from . import util
 import os
 from . import tools
@@ -73,14 +74,17 @@
         if ('_timeformat' in self.meta.keys()) and (
             self.meta['_timeformat'] != '%Y' and self.meta['_timeformat'] != 'Y'
         ):
             self.columns_to_datetime()
 
         self.attrs = self.meta
 
+    @property
+    def units(self):
+        return self.meta['unit']
     def info(self):
         """
         Returns information about the dataframe like shape, index and column
         extend and the number of non-nan entries.
 
         Returns
         -------
@@ -136,18 +140,20 @@
                 )
                 meta[fld] = values[0]
             return meta
 
         meta = {
             **extract_unique_values(idf.data, pyam.IAMC_IDX, ['region']),
             **extract_unique_values(idf.meta, idf.meta.columns, ['exclude']),
-        }
+        }   
 
         data = idf.data.pivot_table(
-            index=['region'], columns=idf.time_col
+            index=['region'], 
+            columns=idf.time_col,
+            aggfunc='sum',
         ).value.rename_axis(  # column name
             columns=None
         )
 
         return cls(data, meta=meta)
 
     @classmethod
@@ -661,15 +667,15 @@
 
         if isinstance(other, Datatable):
 
             if other.meta['entity'] != self.meta['entity']:
                 #                print(other.meta['entity'] )
                 #                print(self.meta['entity'])
                 raise (BaseException('Physical entities do not match, please correct'))
-            if other.meta['unit'] != self.meta['unit']:
+            if other.units != self.meta['unit']:
                 other = other.convert(self.meta['unit'])
 
         out = pd.concat([self, other], **kwargs)
 
         # only copy required keys
         out.meta = {
             key: value
@@ -695,26 +701,31 @@
 
         Returns
         -------
         out : datatable
             DESCRIPTION.
 
         """
-        if isinstance(other, Datatable):
-
-            if self.meta['unit'] == other.meta['unit']:
+        if isinstance(other, (Datatable, pint.Quantity)):
+              
+            if self.meta['unit'] == other.units:
                 factor = 1
             else:
-                factor = core.getUnit(other.meta['unit']).to(self.meta['unit']).m
-
-            rhs = pd.DataFrame(other * factor)
+                factor = core.getUnit(other.units).to(self.meta['unit']).m
+            if isinstance(other, pint.Quantity):
+                rhs = other.m
+            else:
+                rhs = pd.DataFrame(other * factor)
             out = Datatable(super(Datatable, self.copy()).__add__(rhs))
 
             out.meta['unit'] = self.meta['unit']
             out.meta['source'] = 'calculation'
+            
+        # elif isinstance(ur(df1.meta['unit']),pint.Quantity):
+            
         else:
             out = Datatable(super(Datatable, self).__add__(other))
             out.meta['unit'] = self.meta['unit']
             out.meta['source'] = 'calculation'
         return out
 
     __radd__ = __add__
@@ -731,79 +742,90 @@
 
         Returns
         -------
         out : datatable
             DESCRIPTION.
 
         """
-        if isinstance(other, Datatable):
-            if self.meta['unit'] == other.meta['unit']:
+        if isinstance(other, (Datatable, pint.Quantity)):
+            if self.meta['unit'] == other.units:
                 factor = 1
             else:
-                factor = core.getUnit(other.meta['unit']).to(self.meta['unit']).m
-            rhs = pd.DataFrame(other * factor)
+                factor = core.getUnit(other.units).to(self.meta['unit']).m
+            if isinstance(other, pint.Quantity):
+                rhs = other.m
+            else:
+                rhs = pd.DataFrame(other * factor)
             out = Datatable(super(Datatable, self).__sub__(rhs))
             out.meta['unit'] = self.meta['unit']
             out.meta['source'] = 'calculation'
         else:
             out = Datatable(super(Datatable, self).__sub__(other))
             out.meta['unit'] = self.meta['unit']
             out.meta['source'] = 'calculation'
         return out
 
     def __rsub__(self, other):
         """
         Equivalent to __sub__
         """
-        if isinstance(other, Datatable):
-            if self.meta['unit'] == other.meta['unit']:
+        if isinstance(other, (Datatable, pint.Quantity)):
+            if self.meta['unit'] == other.units:
                 factor = 1
             else:
-                factor = core.getUnit(other.meta['unit']).to(self.meta['unit']).m
+                factor = core.getUnit(other.units).to(self.meta['unit']).m
+            if isinstance(other, pint.Quantity):
+                other = other.m
             out = Datatable(super(Datatable, self).__rsub__(other * factor))
             out.meta['unit'] = self.meta['unit']
             out.meta['source'] = 'calculation'
         else:
             out = Datatable(super(Datatable, self).__rsub__(other))
             out.meta['unit'] = self.meta['unit']
             out.meta['source'] = 'calculation'
         return out
 
     def __mul__(self, other):
-        if isinstance(other, Datatable):
-            newUnit = core.getUnit(self.meta['unit']) * core.getUnit(other.meta['unit'])
+        if isinstance(other, (Datatable, pint.Quantity)):
+            newUnit = core.getUnit(self.meta['unit']) * core.getUnit(other.units)
+            if isinstance(other, pint.Quantity):
+                other = other.m
             out = Datatable(super(Datatable, self).__mul__(other))
             out.meta['unit'] = str(newUnit.u)
             out.meta['source'] = 'calculation'
             out.values[:] *= newUnit.m
         else:
             out = Datatable(super(Datatable, self).__mul__(other))
             out.meta['unit'] = self.meta['unit']
             out.meta['source'] = 'calculation'
         return out
 
     __rmul__ = __mul__
 
     def __truediv__(self, other):
-        if isinstance(other, Datatable):
-            newUnit = core.getUnit(self.meta['unit']) / core.getUnit(other.meta['unit'])
+        if isinstance(other, (Datatable, pint.Quantity)):
+            newUnit = core.getUnit(self.meta['unit']) / core.getUnit(other.units)
+            if isinstance(other, pint.Quantity):
+                other = other.m
             out = Datatable(super(Datatable, self).__truediv__(other))
             out.meta['unit'] = str(newUnit.u)
             out.meta['source'] = 'calculation'
             out.values[:] *= newUnit.m
         else:
             out = Datatable(super(Datatable, self).__truediv__(other))
             out.meta['unit'] = self.meta['unit']
             out.meta['source'] = 'calculation'
         return out
 
     #    __rtruediv__ = __truediv__
     def __rtruediv__(self, other):
-        if isinstance(other, Datatable):
-            newUnit = core.getUnit(other.meta['unit']) / core.getUnit(self.meta['unit'])
+        if isinstance(other, (Datatable, pint.Quantity)):
+            newUnit = core.getUnit(other.units) / core.getUnit(self.meta['unit'])
+            if isinstance(other, pint.Quantity):
+                other = other.m
             out = Datatable(super(Datatable, self).__rtruediv__(other))
             out.meta['unit'] = str(newUnit.u)
             out.meta['source'] = 'calculation'
             out.values[:] *= newUnit.m
         else:
             out = Datatable(super(Datatable, self).__rtruediv__(other))
             out.meta['unit'] = str((core.getUnit(self.meta['unit']) ** -1).u)
@@ -987,16 +1009,19 @@
 
             tables[tableKey].convert(newUnit)
             tables[tableKey].meta['unit'] = newUnit
             tables.inventory.loc[tableKey, 'unit'] = newUnit
 
         return tables
 
-    def copy(self):
-        return copy(self)
+    def copy(self, deep=False):
+        if deep:
+            return deepcopy(self)
+        else:
+            return copy(self)
 
     def remove(self, tableID):
         """
         Remove table form tableSet.
 
         Parameters
         ----------
@@ -1436,15 +1461,15 @@
         long_df = pd.DataFrame(long_df)
         return long_df
 
     def to_pyam(self):
 
         import pyam
 
-        long_table = self.to_LongTable()
+        long_table = self.copy(deep=True).to_LongTable()
         long_table.index.name = None
 
         # make sure that region does not contain any nan values
         na_mask = long_table['region'].isnull()
         if config.DEBUG and (sum(na_mask) > 0):
             print(f'Removing {sum(na_mask)} nan items in region index')
         long_table = long_table[~na_mask]
@@ -1559,18 +1584,18 @@
         if meta_dims is not None:
             data = _add_required_meta(data, meta, stacked_dims)
 
         return cls.from_wide_dataframe(data, meta, stacked_dims)
 
     @classmethod
     def from_query(cls, query, stacked_dims={'pathway': ("model", "scenario")}):
-        dimensions = ['model', 'scenario', 'region', 'variable', 'source', 'unit']
-        data = query.as_wide_dataframe(meta_list=dimensions)
-
-        return cls.from_wide_dataframe(data, meta=None, stacked_dims=stacked_dims)
+        #dimensions = ['model', 'scenario', 'region', 'variable', 'source', 'unit']
+        # data = query.as_wide_dataframe(meta_list=dimensions)
+        return tools.xarray.load_as_xdataset(query, stacked_dims=stacked_dims)
+        #return cls.from_wide_dataframe(data, meta=None, stacked_dims=stacked_dims)
 
 
 class Visualization:
     """
     This class addes handy built-in visualizations to datatables
     """
```

### Comparing `datatoolbox-0.5.4/datatoolbox/database.py` & `datatoolbox-0.5.5/datatoolbox/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import os
 import git
 import tqdm
 import time
 import copy
 import types
 
+from threading import Thread
 import traceback
 from collections import defaultdict
 from pathlib import Path
 import shutil
 
 import pandas as pd
 import numpy as np
@@ -104,16 +105,20 @@
         in the config is empty.
         """
         tt = time.time()
         self.path = config.PATH_TO_DATASHELF
 
         if not os.path.exists(os.path.join(self.path, "inventory.csv")):
             self.create_empty_datashelf(config.MODULE_PATH, self.path)
-
+            
+        tt2 = time.time()
         self.gitManager = GitRepository_Manager(config)
+        if config.DEBUG:
+            print("Git Manager loaded in {:2.4f} seconds".format(time.time() - tt2))
+
         self.INVENTORY_PATH = os.path.join(self.path, "inventory.csv")
         self.inventory = self._load_inventory(self.INVENTORY_PATH)
         self.sources = self.gitManager.sources
 
         # check for patch
         if "tag" not in self.sources.columns:
             from .patches import patch_050_update_sources_csv
@@ -140,28 +145,32 @@
             self.commitTables(
                 tablesToCommit,
                 message="added dummy tables of source B",
                 sourceMetaDict=source_meta,
             )
             print("Added test tables to Sandbox datashelf")
 
-        # remote update checks
-        self.check_for_new_remote_data()
+        
+        
 
     #%% private functions
 
     def _addNewSource(self, sourceMetaDict):
         """
         Private
         Adds new source to the sources table
         """
         source_ID = sourceMetaDict["SOURCE_ID"]
 
+                
         if not self.sourceExists(source_ID):
-
+            
+            # check if source is aready online
+            if self.gitManager.check_if_online_repo_exists(source_ID):
+                raise(Exception(f"Souce with name {source_ID} exists already online. Use dt.importSourceFromRemote() do create a local copy. Review the data and consider adding to the existing dataset"))
             sourcePath = os.path.join(
                 config.PATH_TO_DATASHELF, "database", sourceMetaDict["SOURCE_ID"]
             )
             self.gitManager.init_new_repo(sourcePath, source_ID, sourceMetaDict)
 
         else:
             print("source already exists")
@@ -188,22 +197,14 @@
         datatable = datatable.sort_index(axis="index")
         datatable = datatable.sort_index(axis="columns")
 
         self.isConsistentTable(datatable)
 
         self._gitAddTable(datatable, source, filePath)
 
-    def _check_online_data(self):
-        curr_date = pd.to_datetime(core.get_time_string()).date()
-        last_access_date = pd.to_datetime(
-            self.gitManager._get_last_remote_access()
-        ).date()
-
-        return curr_date > last_access_date
-
     def _checkTablesOnDisk(self, sourceID=None):
         notExistingTables = list()
 
         if sourceID is None:
             table_list = self.inventory.index
         else:
             table_list = self.inventory.index[self.inventory.source == sourceID]
@@ -362,77 +363,18 @@
         sourcesDf.to_csv(datashelf / "sources.csv")
 
         # creates inventory.csv that contains all data tables from all sources
         inventoryDf = pd.DataFrame(columns=config.INVENTORY_FIELDS)
         inventoryDf.to_csv(datashelf / "inventory.csv")
         git.Repo.init(datashelf)
 
-    def check_for_new_remote_data(self, update=False):
-        remote_repo_path = os.path.join(
-            config.PATH_TO_DATASHELF, "remote_sources", "source_states.csv"
-        )
-        if os.path.exists(remote_repo_path):
-            remote_sources_df_before = pd.read_csv(remote_repo_path, index_col=0)
-
-        if update or self._check_online_data():
-            # check for remote data
-            try:
-                print("Looking for new online sources...", end="")
-                self.gitManager._pull_remote_sources()
-                print("Done!")
-            except:
-                print("Could not check online data repository")
-                import traceback
-
-                traceback.print_exc()
-
-        if not os.path.exists(remote_repo_path):
-            print("No information about remote data available")
-            print("Consider run again with update = True")
-
-        else:
-            remote_sources_df = pd.read_csv(remote_repo_path, index_col=0)
-
-            sources_with_update = pd.DataFrame(
-                columns=["local version", "remote version"]
-            )
-            for sourceID in remote_sources_df.index:
-
-                if sourceID not in self.sources.index:
-                    continue
-                remote_tag = remote_sources_df.loc[sourceID, "tag"]
-                local_tag = self.sources.loc[sourceID, "tag"]
-                if not isinstance(local_tag, str):
-                    # no tag
-
-                    # check if remote hash as same tag
-                    remote_hash = remote_sources_df.loc["test_AR6", "hash"]
-                    local_hash = self.gitManager.get_hash_of_source(sourceID)
-                    if remote_hash == local_hash:
-                        print(f"Applying tag from remote for source {sourceID}")
-                        self.sources.loc[sourceID, "tag"] = remote_tag
-                    continue
-
-                if float(remote_tag[1:]) > float(local_tag[1:]):
-                    sources_with_update.loc[sourceID] = local_tag, remote_tag
-
-            if len(sources_with_update) > 0:
-                print("The following source have newer versions available:")
-
-                print(tabulate(sources_with_update, headers="keys", tablefmt="psql"))
-
-            new_entries = remote_sources_df.index.difference(
-                remote_sources_df_before.index
-            )
-            if len(new_entries) > 0:
-                print("The following new sources have been added:")
-                df_news = remote_sources_df.loc[new_entries, ["tag", "last_to_update"]]
-                df_news.columns = ["version", "updated_by"]
-                print(tabulate(df_news, headers="keys", tablefmt="psql"))
-
+    def check_for_new_remote_data (self, update=False):
+        # redirecting to gitManager function
+        return self.gitManager.check_for_new_remote_data(update)
+    
     def info(self):
         """
         Shows the most inmportant information about the status of the database
         """
 
         print("######## Database informations: #############")
         print("Your database is located at: " + self.path)
@@ -851,15 +793,15 @@
         ------
         tables : list of Datatable
         message : str
         sourceMetaDict [Optional] :  dict
         append_data [optinal]  : bool to choose if new data is added to the existing
                                  table (new data does not overwrite old data)
         update : [optional]    : bool to choose if the exting data is updated
-        overwrire : [optional] : bool to choose if data is overwriten (new data
+        overwrite : [optional] : bool to choose if data is overwriten (new data
                                  overwrites old data)
         cleanTables [optional] : bool (default: true) to choose if tables are
                                  cleaned before commit
 
         TODO: Check flags
         """
         # create a new source if not extisting
@@ -1332,46 +1274,109 @@
     """
 
     #%% Magicc methods
     def __init__(self, config, debugmode=False):
         self.PATH_TO_DATASHELF = config.PATH_TO_DATASHELF
         self.sources = pd.read_csv(config.SOURCE_FILE, index_col="SOURCE_ID")
 
+        remote_repo_path = os.path.join(
+            config.PATH_TO_DATASHELF, "remote_sources", "source_states.csv"
+        )
+        if os.path.exists(remote_repo_path):
+            self.remote_sources = pd.read_csv(remote_repo_path, index_col=0)
+            
+            
+            new_items, updated_items = self._get_difference_to_remote()
+            n_new_entries = len(new_items)
+            n_updated_sources = len(updated_items)
+            if n_new_entries + n_updated_sources  > 0:
+                print('Remote: ',end='')
+                if n_new_entries >0:
+                   print(f'({n_new_entries}) new sources', end='')
+                    
+                if n_updated_sources > 0:
+                    print(f' and ({len(updated_items)}) updated sources', end='')
+                print(' are available online (see dt.available_remote_data_updates)')
+                
+        else:
+            print('Remote: not setup')
+        
         self.repositories = dict()
         self.updatedRepos = set()
         self.validatedRepos = set()
         self.filesToAdd = defaultdict(list)
-
+        
+        # remote update checks (only once per day)
+        self._init_remote_repo()
+        
+        
         if not debugmode:
             for sourceID in self.sources.index:
                 repoPath = os.path.join(self.PATH_TO_DATASHELF, "database", sourceID)
                 self.repositories[sourceID] = git.Repo(repoPath)
                 self.verifyGitHash(sourceID)
 
             self.repositories["main"] = git.Repo(self.PATH_TO_DATASHELF)
             self._validateRepository("main")
         else:
             print("Git manager initialized in debugmode")
 
+        self.check_for_new_remote_data()
+        
     def __getitem__(self, sourceID):
         """
         Retrieve `sourceID` from repositories dictionary and ensure cleanliness
         """
         repo = self.repositories[sourceID]
         if sourceID not in self.validatedRepos:
             self._validateRepository(sourceID)
         return repo
 
     #%% Private methods
-    def _init_remote_repo(self):
+    
+    def _get_difference_to_remote(self):
+        
+        new_items = self.remote_sources.index.difference(
+            self.sources.index
+        )
+        compare_df = self.sources.copy()
+        compare_df['remote_tag'] = self.remote_sources['tag']
+        compare_df = compare_df[(~compare_df.tag.isnull()) &(~compare_df.remote_tag.isnull())]
+        
+        updated_items = compare_df.index[(
+            compare_df.tag.apply(lambda x : float(x[1:])) < compare_df.remote_tag.apply(lambda x : float(x[1:]))
+            )]
+        
+        
+        
+        return new_items, updated_items
+    
+    def _check_online_data(self):
+        curr_date = pd.to_datetime(core.get_time_string()).date()
+        last_access_date = pd.to_datetime(
+            self._get_last_remote_access()
+        ).date()
 
+        return pd.isna(last_access_date) or curr_date > last_access_date
+  
+    def _init_remote_repo(self):   
         remote_repo_path = os.path.join(config.PATH_TO_DATASHELF, "remote_sources")
-        if os.path.exist(remote_repo_path):
+        if os.path.exists(remote_repo_path):
             self.remote_repo = self._get_remote_sources_repo()
-
+            
+            dpath = os.path.join(
+            config.PATH_TO_DATASHELF,
+            "remote_sources",
+            "source_states.csv",
+                )
+            self.remote_sources = pd.read_csv(dpath, index_col=0)
+        else:
+            #create empty dummy
+            self.remote_sources = pd.DataFrame()
+            
     def _get_remote_sources_repo(self):
         remote_repo_path = os.path.join(config.PATH_TO_DATASHELF, "remote_sources")
         remote_repo = git.Repo(remote_repo_path)
 
         # self.remote_repo = remote_repo()
         return remote_repo
 
@@ -1477,18 +1482,19 @@
                 tag = f'v{float(latest_tag.name.replace("v",""))+1:1.1f}'
 
         # update remote sources csv
         repo.create_tag(tag)
         # tag = repo.tags[-1].name
         rem_sources_df.loc[repoName, :] = (hash, tag, user)
         rem_sources_df.to_csv(dpath)
-
+        
         remote_repo.index.add("source_states.csv")
         remote_repo.index.commit("remote source update" + " by " + config.CRUNCHER)
-
+        
+        self.remote_sources = rem_sources_df
         return repo
 
     def _gitUpdateFile(self, repoName, filePath):
         pass
 
     def _validateRepository(self, sourceID):
         """
@@ -1511,14 +1517,63 @@
         config.DB_READ_ONLY = False
         if config.DEBUG:
             print("Repo {} is clean".format(sourceID))
         self.validatedRepos.add(sourceID)
         return True
 
     #%% Public methods
+    
+    def check_if_online_repo_exists(self, sourceID):
+        return sourceID in self.remote_sources.index
+    
+    def check_for_new_remote_data(self, force_check=False, foreground=False):
+
+        if (force_check or self._check_online_data()) and not ("PYTEST_CURRENT_TEST" in os.environ):
+                
+            # check for remote data
+            try:
+                if foreground:
+                    print("Looking for new online sources...", end='')
+                    self._pull_remote_sources()
+                    print("Done!")    
+                else:
+                    print("Looking for new online sources in the backgound")
+                    thread = Thread(target=self._pull_remote_sources)
+                    thread.start()
+                # 
+                # print("Done!")
+            except:
+                print("Could not check online data repository")
+                import traceback
+
+                traceback.print_exc()
+                
+    def available_remote_data_updates(self):
+        
+        new_items, updated_items = self._get_difference_to_remote()
+        
+        print('New items:')
+        print(tabulate(
+            self.remote_sources.loc[new_items, ['tag', 'last_to_update']], 
+            headers="keys", tablefmt="psql"))
+        
+        print('Sources with newer data:')
+        
+        df = pd.concat(
+            [
+                self.sources.loc[updated_items, ['tag']].rename(columns={'tag':'local_tag'}),
+                self.remote_sources.loc[updated_items, ['tag']].rename(columns={'tag':'remote_tag'}),
+            ], axis=1)
+        print(tabulate(
+            df, 
+            headers="keys", tablefmt="psql"))
+    
+        
+
+
     def get_source_repo_failsave(self, sourceID):
         """
         Retrieve `sourceID` from repositories dictionary without checks
         """
         repoPath = os.path.join(self.PATH_TO_DATASHELF, "database", sourceID)
         repo = git.Repo(repoPath)
         return repo
```

### Comparing `datatoolbox-0.5.4/datatoolbox/greenhouse_gas_database.py` & `datatoolbox-0.5.5/datatoolbox/greenhouse_gas_database.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/init_tools.py` & `datatoolbox-0.5.5/datatoolbox/init_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/interfaces.py` & `datatoolbox-0.5.5/datatoolbox/interfaces.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/io_tools.py` & `datatoolbox-0.5.5/datatoolbox/io_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/mapping.py` & `datatoolbox-0.5.5/datatoolbox/mapping.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/naming_convention.py` & `datatoolbox-0.5.5/datatoolbox/naming_convention.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/patches.py` & `datatoolbox-0.5.5/datatoolbox/patches.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/pint_definitions.txt` & `datatoolbox-0.5.5/datatoolbox/pint_definitions.txt`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/sets.py` & `datatoolbox-0.5.5/datatoolbox/sets.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,14 @@
                 'PRT',
                 'ROU',
                 'SVK',
                 'SVN',
                 'SWE',
             ]
         )
-
         self.EU27 = set(
             [
                 'AUT',
                 'BEL',
                 'BGR',
                 'CYP',
                 'CZE',
@@ -256,14 +255,15 @@
                 'PRT',
                 'ROU',
                 'SVK',
                 'SVN',
                 'SWE',
             ]
         )
+     
 
         self.LDCS = set(
             [
                 "AGO",
                 "BEN",
                 "BFA",
                 "BDI",
```

### Comparing `datatoolbox-0.5.4/datatoolbox/templates.py` & `datatoolbox-0.5.5/datatoolbox/templates.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/CRF_extract_CA_2021.xlsx` & `datatoolbox-0.5.5/datatoolbox/tools/CRF_extract_CA_2021.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN` & `datatoolbox-0.5.5/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/IEA_B2DS_4.SCEN` & `datatoolbox-0.5.5/datatoolbox/tools/IEA_B2DS_4.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/WEO_2019_test.SCEN` & `datatoolbox-0.5.5/datatoolbox/tools/WEO_2019_test.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/conversion_to_v0.3.py` & `datatoolbox-0.5.5/datatoolbox/tools/conversion_to_v0.3.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/excel.py` & `datatoolbox-0.5.5/datatoolbox/tools/excel.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/for_datatables.py` & `datatoolbox-0.5.5/datatoolbox/tools/for_datatables.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/html.py` & `datatoolbox-0.5.5/datatoolbox/tools/html.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/kaya_idendentiy_decomposition.py` & `datatoolbox-0.5.5/datatoolbox/tools/kaya_idendentiy_decomposition.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/magicc6.py` & `datatoolbox-0.5.5/datatoolbox/tools/magicc6.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/matplotlib.py` & `datatoolbox-0.5.5/datatoolbox/tools/matplotlib.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/pandas.py` & `datatoolbox-0.5.5/datatoolbox/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/py_magicc_tools.py` & `datatoolbox-0.5.5/datatoolbox/tools/py_magicc_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/pyam.py` & `datatoolbox-0.5.5/datatoolbox/tools/pyam.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/renaming_DB.py` & `datatoolbox-0.5.5/datatoolbox/tools/renaming_DB.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/run_MAGICC_startup_simple.xlsx` & `datatoolbox-0.5.5/datatoolbox/tools/run_MAGICC_startup_simple.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/run_magicc6.m` & `datatoolbox-0.5.5/datatoolbox/tools/run_magicc6.m`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/statistics.py` & `datatoolbox-0.5.5/datatoolbox/tools/statistics.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/test.docx` & `datatoolbox-0.5.5/datatoolbox/tools/test.docx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/word.py` & `datatoolbox-0.5.5/datatoolbox/tools/word.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tools/xarray.py` & `datatoolbox-0.5.5/datatoolbox/tools/xarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
     ds = xr.merge(data)
 
     return ds
 
 
 def load_as_xdataset(
     query_results,
-    dimensions=['model', 'scenario', 'region', 'time'],
+    dimensions=['model', 'scenario', 'region', 'time', 'source'],
     stacked_dims={'pathway': ('model', 'scenario')},
     native_regions=False,
 ):
     """
     Returns xarry dataset pruduced from a database result. Differenty variables
     are stored as key variables. The xarray dimensions (coordiantes) are defined
     by the provided dimensions. A multi-index for a coordinate can be created
```

### Comparing `datatoolbox-0.5.4/datatoolbox/tutorials/00_search_find_and_access_data.py` & `datatoolbox-0.5.5/datatoolbox/tutorials/00_search_find_and_access_data.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tutorials/01_emission_comparison.py` & `datatoolbox-0.5.5/datatoolbox/tutorials/01_emission_comparison.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tutorials/02_unit_conversion.py` & `datatoolbox-0.5.5/datatoolbox/tutorials/02_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tutorials/03_intermediate_example.py` & `datatoolbox-0.5.5/datatoolbox/tutorials/03_intermediate_example.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tutorials/04_sources.py` & `datatoolbox-0.5.5/datatoolbox/tutorials/04_sources.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tutorials/06_xarray_examples.py` & `datatoolbox-0.5.5/datatoolbox/tutorials/06_xarray_examples.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tutorials/07_renewable_share_compuation.py` & `datatoolbox-0.5.5/datatoolbox/tutorials/07_renewable_share_compuation.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tutorials/08_low_carbon_fuel_computation.py` & `datatoolbox-0.5.5/datatoolbox/tutorials/08_low_carbon_fuel_computation.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tutorials/introduction_v1.ipynb` & `datatoolbox-0.5.5/datatoolbox/tutorials/introduction_v1.ipynb`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/tutorials/jump_start.py` & `datatoolbox-0.5.5/datatoolbox/tutorials/jump_start.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/util.py` & `datatoolbox-0.5.5/datatoolbox/util.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox/workflows.py` & `datatoolbox-0.5.5/datatoolbox/workflows.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/datatoolbox.egg-info/PKG-INFO` & `datatoolbox-0.5.5/datatoolbox.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatoolbox
-Version: 0.5.4
+Version: 0.5.5
 Summary: The Python Data Toolbox
 Home-page: https://gitlab.com/climateanalytics/datatoolbox
 Author: Andreas Geiges
 Author-email: a.geiges@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `datatoolbox-0.5.4/datatoolbox.egg-info/SOURCES.txt` & `datatoolbox-0.5.5/datatoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/doc/Makefile` & `datatoolbox-0.5.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/doc/conf.py` & `datatoolbox-0.5.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/doc/figures/ID_meta_data.svg` & `datatoolbox-0.5.5/doc/figures/ID_meta_data.svg`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/doc/figures/config_input.png` & `datatoolbox-0.5.5/doc/figures/config_input.png`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/doc/first_steps.md` & `datatoolbox-0.5.5/doc/first_steps.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/doc/installation.md` & `datatoolbox-0.5.5/doc/installation.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/doc/license.rst` & `datatoolbox-0.5.5/doc/license.rst`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/doc/make.bat` & `datatoolbox-0.5.5/doc/make.bat`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/documentation/Datatoolbox - First steps.md` & `datatoolbox-0.5.5/documentation/Datatoolbox - First steps.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/readthedocs.yml` & `datatoolbox-0.5.5/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/setup.py` & `datatoolbox-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             "pycountry",
             "fuzzywuzzy",
             "tqdm",
             "pyam-iamc",
             "networkx",
             "pint_xarray",
             "openpyxl",
+            "tabulate",
             "xarray",
             "deprecated",],
         }
     rtn = setup(**setup_kwargs)
 
 if __name__ == "__main__":
     main()
```

### Comparing `datatoolbox-0.5.4/tests/test_calculations.py` & `datatoolbox-0.5.5/tests/test_calculations.py`

 * *Files 9% similar despite different names*

```diff
@@ -199,7 +199,18 @@
     # TODO:use with new pandas version
     # assert_frame_equal(obs, exp)
     
     npt.assert_array_almost_equal(obs, exp, decimal = 5)
     assert obs.loc[:,2020].isnull().all()
     assert obs.meta['unit']   == exp.meta['unit']
     assert obs.meta['source'] == 'calculation'
+
+ur = dt.core.ur
+def test_computation_with_pint_quantities():
+    df1 + (1* ur('Mt CO2'))
+    df1 - (2* ur('Mt CO2'))
+    df1 * (1* ur('kg /(Mt CO2)'))
+    df1 / (1* ur('Mt CO2 /kg'))
+    
+def test_rhs_computation_with_pint_quantities():
+    (100* ur('Mt CO2 /kg')) / df1
+    (100* ur('Mt CO2 /kg')) * df1
```

### Comparing `datatoolbox-0.5.4/tests/test_converters.py` & `datatoolbox-0.5.5/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/tests/test_database.py` & `datatoolbox-0.5.5/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/tests/test_dataset.py` & `datatoolbox-0.5.5/tests/test_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,21 +21,27 @@
 
 def test_sel_methods():
     res = dt.findp(variable = ['Numbers|Ones',
                                'Numbers|Fives']) # find all
     ds = dt.DataSet.from_query(res)
     
     sub = ds.sel(scenario='Historic')
-    assert dict(sub.dims) =={'year': 5, 'region': 4,'source': 1, 'model': 1}
+    
+    exp ={'time': 5, 'region': 4,'source': 1, 'model': 1}
+    assert all([exp[key] == dict(sub.dims)[key] for key in exp.keys()])
     
     sub = ds.sel(region="DEU")
-    assert dict(sub.dims) == {'year': 5, 'source': 1,'pathway': 1}
     
-    sub = ds.sel(year=2012)
-    assert dict(sub.dims) == {'region': 4, 'source': 1,'pathway': 1}
+    exp = {'time': 5, 'source': 1,'pathway': 1}
+    
+    
+    sub = ds.sel(time=2012)
+    
+    exp =  {'region': 4, 'source': 1,'pathway': 1}
+    assert all([exp[key] == dict(sub.dims)[key] for key in exp.keys()])
 
 def test_unit_conversion():
     res = dt.findp(variable = ['Numbers|One',
                                'Numbers|Fives']) # find all
     ds = dt.DataSet.from_query(res)
     mm_data = ds['Numbers|Fives'].pint.to('mm')
```

### Comparing `datatoolbox-0.5.4/tests/test_datatable.py` & `datatoolbox-0.5.5/tests/test_datatable.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/tests/test_io.py` & `datatoolbox-0.5.5/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/tests/test_pyam.py` & `datatoolbox-0.5.5/tests/test_pyam.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,17 +48,17 @@
         assert (table_in.values == table_out.values).all()
         assert (table_in.index == table_out.index).all()
         assert (table_in.columns == table_out.columns).all()
 
 def test_lossless_conversion():
     
     exp = df.copy().clean() # copy initial datatable
-    
+    print(exp)
     idf = exp.to_pyam() # create IamDataFrame
-    
     obs = dt.Datatable.from_pyam(idf)
     
     assert pd.testing.assert_frame_equal(obs,exp) is None
 
 if __name__ == '__main__':
     test_import()
     test_to_pyam_interface()
+    test_lossless_conversion()
```

### Comparing `datatoolbox-0.5.4/tests/test_tableset.py` & `datatoolbox-0.5.5/tests/test_tableset.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/tests/test_tools.py` & `datatoolbox-0.5.5/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/tests/test_units.py` & `datatoolbox-0.5.5/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/tests/test_utilities.py` & `datatoolbox-0.5.5/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/tests/test_xarray.py` & `datatoolbox-0.5.5/tests/test_xarray.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.4/tests/util_for_testing.py` & `datatoolbox-0.5.5/tests/util_for_testing.py`

 * *Files identical despite different names*

