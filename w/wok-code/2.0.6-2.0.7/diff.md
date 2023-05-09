# Comparing `tmp/wok_code-2.0.6.tar.gz` & `tmp/wok_code-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wok_code-2.0.6.tar", last modified: Sun Apr 23 14:00:37 2023, max compression
+gzip compressed data, was "dist/wok_code-2.0.7.tar", last modified: Tue May  9 17:25:50 2023, max compression
```

## Comparing `wok_code-2.0.6.tar` & `wok_code-2.0.7.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:00:37.516086 wok_code-2.0.6/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1607 2023-04-23 14:00:37.516086 wok_code-2.0.6/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    47023 2023-04-23 14:00:36.000000 wok_code-2.0.6/README.rst
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-04-23 14:00:37.516086 wok_code-2.0.6/setup.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3729 2023-04-21 12:32:35.000000 wok_code-2.0.6/setup.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:00:37.516086 wok_code-2.0.6/wok_code/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       81 2023-01-27 10:18:10.000000 wok_code-2.0.6/wok_code/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/__main__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6744 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/cvt_csv_2_xml.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20904 2023-04-15 08:02:21.000000 wok_code-2.0.6/wok_code/cvt_script
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1150 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/cvt_script.man
--rw-r--r--   0 odoo      (1000) odoo      (1000)    11286 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/do_git_checkout_new_branch.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3052 2023-02-12 19:40:51.000000 wok_code-2.0.6/wok_code/do_gitignore.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2646 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/do_set_utf8.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2176 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/eval_gtin.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7186 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/gen_addons_table.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)     1413 2022-12-13 19:22:06.000000 wok_code-2.0.6/wok_code/install_python_3_from_source.sh
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3082 2023-04-23 10:48:07.000000 wok_code-2.0.6/wok_code/pgconf.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6896 2023-01-21 13:24:11.000000 wok_code-2.0.6/wok_code/please.man
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     8389 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/pypi.sh
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      205 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/rm_dir_with_space.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:00:37.516086 wok_code-2.0.6/wok_code/scripts/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      606 2023-04-21 11:43:14.000000 wok_code-2.0.6/wok_code/scripts/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:00:37.516086 wok_code-2.0.6/wok_code/scripts/config/
--rw-r--r--   0 odoo      (1000) odoo      (1000)      373 2023-04-12 10:49:14.000000 wok_code-2.0.6/wok_code/scripts/config/globals.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)        0 2023-04-12 07:23:52.000000 wok_code-2.0.6/wok_code/scripts/config/globals_xml.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)      893 2023-04-12 07:02:48.000000 wok_code-2.0.6/wok_code/scripts/config/to_new_api.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)      224 2023-04-12 07:55:02.000000 wok_code-2.0.6/wok_code/scripts/config/to_odoo_py2.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)      173 2023-04-12 07:50:10.000000 wok_code-2.0.6/wok_code/scripts/config/to_odoo_py3.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)      698 2023-04-12 06:43:18.000000 wok_code-2.0.6/wok_code/scripts/config/to_old_api.yml
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5357 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/cvt_csv_2_rst.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    21516 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/cvt_csv_coa.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    40728 2023-04-14 14:10:51.000000 wok_code-2.0.6/wok_code/scripts/deploy_odoo.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/scripts/dist_pkg.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    17827 2023-04-15 08:02:21.000000 wok_code-2.0.6/wok_code/scripts/dist_pkg.sh
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    26398 2023-04-17 21:30:54.000000 wok_code-2.0.6/wok_code/scripts/do_migrate.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5937 2023-04-14 14:07:01.000000 wok_code-2.0.6/wok_code/scripts/do_odoo_site.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    83221 2023-04-03 11:40:32.000000 wok_code-2.0.6/wok_code/scripts/gen_readme.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1225 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/generate_random_codes.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)    10070 2023-01-27 08:05:01.000000 wok_code-2.0.6/wok_code/scripts/license_mgnt.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    10100 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/lint_2_compare.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6457 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/main.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4990 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/makepo_it.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    31823 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/odoo_dependencies.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    40102 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/odoo_translation.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    25546 2023-04-14 14:07:09.000000 wok_code-2.0.6/wok_code/scripts/odoo_translation_old.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    22434 2023-04-14 14:07:18.000000 wok_code-2.0.6/wok_code/scripts/please.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    63670 2023-04-15 08:02:21.000000 wok_code-2.0.6/wok_code/scripts/please.sh
--rw-r--r--   0 odoo      (1000) odoo      (1000)     7066 2023-04-14 14:09:03.000000 wok_code-2.0.6/wok_code/scripts/please_apache.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)     5550 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/please_z0bug.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/scripts/run_odoo_debug.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3729 2023-04-23 13:50:03.000000 wok_code-2.0.6/wok_code/scripts/setup.info
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    71159 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/scripts/to_pep8.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    30263 2023-04-02 15:30:34.000000 wok_code-2.0.6/wok_code/scripts/wget_odoo_repositories.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7804 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/ssh.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:00:37.516086 wok_code-2.0.6/wok_code/tests/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2028 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/tests/test_filepo.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6539 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/tests/test_gen_readme.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4939 2023-03-25 15:14:36.000000 wok_code-2.0.6/wok_code/tests/test_license_mgnt.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)     2229 2023-04-14 14:09:46.000000 wok_code-2.0.6/wok_code/tests/test_please.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1672 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/to_oca.2p8
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5228 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/to_pep8.2p8
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2667 2022-12-09 05:08:44.000000 wok_code-2.0.6/wok_code/to_zero.2p8
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    32228 2023-04-15 08:02:21.000000 wok_code-2.0.6/wok_code/topep8
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:00:37.516086 wok_code-2.0.6/wok_code.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1607 2023-04-23 14:00:37.000000 wok_code-2.0.6/wok_code.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1896 2023-04-23 14:00:37.000000 wok_code-2.0.6/wok_code.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-04-23 14:00:37.000000 wok_code-2.0.6/wok_code.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      838 2023-04-23 14:00:37.000000 wok_code-2.0.6/wok_code.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 06:35:40.000000 wok_code-2.0.6/wok_code.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       68 2023-04-23 14:00:37.000000 wok_code-2.0.6/wok_code.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        9 2023-04-23 14:00:37.000000 wok_code-2.0.6/wok_code.egg-info/top_level.txt
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:25:50.000000 wok_code-2.0.7/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        9 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 06:35:40.000000 wok_code-2.0.7/wok_code.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      950 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1931 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       64 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1730 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-09 17:25:50.000000 wok_code-2.0.7/setup.cfg
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/__main__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3056 2023-05-09 13:43:39.000000 wok_code-2.0.7/wok_code/do_gitignore.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7186 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/gen_addons_table.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      205 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/rm_dir_with_space.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3082 2023-04-23 10:48:07.000000 wok_code-2.0.7/wok_code/pgconf.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code/tests/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6539 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/tests/test_gen_readme.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)     2229 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/tests/test_please.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2028 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/tests/test_filepo.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4939 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/tests/test_license_mgnt.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7806 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/ssh.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     8389 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/pypi.sh
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6744 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/cvt_csv_2_xml.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code/scripts/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    64039 2023-04-30 14:24:57.000000 wok_code-2.0.7/wok_code/scripts/please.sh
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    71159 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/to_pep8.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3912 2023-05-09 17:24:49.000000 wok_code-2.0.7/wok_code/scripts/setup.info
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6865 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/main.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4990 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/makepo_it.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    21516 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/cvt_csv_coa.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/scripts/run_odoo_debug.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    17827 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/dist_pkg.sh
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1225 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/generate_random_codes.py
+-rwxr-xr-x   0 odoo      (1000) odoo      (1000)    29444 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/run_odoo_debug.sh
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    30263 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/wget_odoo_repositories.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code/scripts/config/
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      224 2023-04-12 07:55:02.000000 wok_code-2.0.7/wok_code/scripts/config/to_odoo_py2.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      173 2023-04-12 07:50:10.000000 wok_code-2.0.7/wok_code/scripts/config/to_odoo_py3.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      893 2023-04-12 07:02:48.000000 wok_code-2.0.7/wok_code/scripts/config/to_new_api.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      373 2023-04-12 10:49:14.000000 wok_code-2.0.7/wok_code/scripts/config/globals.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      698 2023-04-12 06:43:18.000000 wok_code-2.0.7/wok_code/scripts/config/to_old_api.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)        0 2023-04-12 07:23:52.000000 wok_code-2.0.7/wok_code/scripts/config/globals_xml.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)     7066 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/please_apache.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/scripts/dist_pkg.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    26398 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/do_migrate.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    25546 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/odoo_translation_old.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    83221 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/gen_readme.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    10100 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/lint_2_compare.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    42912 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/deploy_odoo.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)     5550 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/please_z0bug.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    46376 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/odoo_translation.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    31823 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/odoo_dependencies.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)    10070 2023-01-27 08:05:01.000000 wok_code-2.0.7/wok_code/scripts/license_mgnt.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5357 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/cvt_csv_2_rst.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    22434 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/please.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5937 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/do_odoo_site.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      606 2023-04-21 11:43:14.000000 wok_code-2.0.7/wok_code/scripts/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2176 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/eval_gtin.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)    14663 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/do_git_checkout_new_branch.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    32228 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/topep8
+-rwxr-xr-x   0 odoo      (1000) odoo      (1000)     2242 2023-05-02 18:41:06.000000 wok_code-2.0.7/wok_code/install_python_3_from_source.sh
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1150 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/cvt_script.man
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1672 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/to_oca.2p8
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2646 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/do_set_utf8.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6896 2023-01-21 13:24:11.000000 wok_code-2.0.7/wok_code/please.man
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2667 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/to_zero.2p8
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5228 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/to_pep8.2p8
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       81 2023-01-27 10:18:10.000000 wok_code-2.0.7/wok_code/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20904 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/cvt_script
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3912 2023-05-09 16:01:24.000000 wok_code-2.0.7/setup.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1730 2023-05-09 17:25:50.000000 wok_code-2.0.7/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    47243 2023-05-09 17:25:50.000000 wok_code-2.0.7/README.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `wok_code-2.0.6/PKG-INFO` & `wok_code-2.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: wok_code
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python developers tools
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
 Project-URL: Source, https://github.com/zeroincombenze/tools
+Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
+Description: 
+        Various tools at your fingertips.
+        
+        The available tools are:
+        
+        * cvt_csv_2_rst.py: convert csv file into rst file
+        * cvt_csv_2_xml.py: convert csv file into xml file
+        * cvt_script: parse bash script and convert to meet company standard
+        * gen_readme.py: generate documentation files, mainly README.rst
+        * odoo_dependency.py: show odoo dependencies and/or Odoo module tree
+        * odoo_translation.py: manage Odoo translation
+        * pep8: parse source .py file to meet pep8 and convert across Odoo versions
+        * please: developer shell
+        * wget_odoo_repositories.py: get repository names from github.com
+        
 Keywords: linux travis development
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Operating System :: OS Independent
-
-
-Various tools at your fingertips.
-
-The available tools are:
-
-* cvt_csv_2_rst.py: convert csv file into rst file
-* cvt_csv_2_xml.py: convert csv file into xml file
-* cvt_script: parse bash script and convert to meet company standard
-* gen_readme.py: generate documentation files, mainly README.rst
-* odoo_dependency.py: show odoo dependencies and/or Odoo module tree
-* odoo_translation.py: manage Odoo translation
-* pep8: parse source .py file to meet pep8 and convert across Odoo versions
-* please: developer shell
-* wget_odoo_repositories.py: get repository names from github.com
-
-
```

### Comparing `wok_code-2.0.6/README.rst` & `wok_code-2.0.7/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 ==============
-wok_code 2.0.6
+wok_code 2.0.7
 ==============
 
 
 
 |Maturity| |Build Status| |Coverage Status| |license gpl|
 
 
@@ -841,14 +841,24 @@
     ./install_tools.sh -Ud
     source /opt/odoo/devel/activate_tools
 
 
 History
 -------
 
+2.0.7 (2023-05-08)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] deply_odoo: new action git-push
+* [REF] odoo_translation: new implementation
+* [FIX] run_odoo_debug: minor fixes
+* [NEW] do_git_checkout_new_branch: new command
+* [IMP] install_python3_from_source: improvements
+* [FIX] ssh.py: scp with port not 22
+
 2.0.6 (2023-02-23)
 ~~~~~~~~~~~~~~~~~~
 
 * [IMP] ssh.py: -m -s switches accept path with user and host
 * [IMP] deploy_odoo: new property status to display
 * [IMP] deploy_odoo: new switches -l and -x
 * [NEW] do_git_checkout_new_branch.py
@@ -918,19 +928,14 @@
 ~~~~~~~~~~~~~~~~~~~~
 
 * [FIX] deploy_odoo: add path in addons_path of directory exists
 * [FIX] deploy_odoo: clone oca repositories with --single-branch option
 * [IMP] manage_pypi: improvements
 * [FIX] please lint|test
 
-2.0.0.1 (2022-09-07)
-~~~~~~~~~~~~~~~~~~~~
-
-* [FIX] please test: with debug
-
 
 
 |
 |
 
 Credits
 =======
@@ -950,15 +955,15 @@
 
 
 
 |
 
 This module is part of tools project.
 
-Last Update / Ultimo aggiornamento: 2023-04-23
+Last Update / Ultimo aggiornamento: 2023-05-09
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
 .. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
     :target: https://travis-ci.com/zeroincombenze/tools
     :alt: github.com
```

### Comparing `wok_code-2.0.6/setup.py` & `wok_code-2.0.7/wok_code/scripts/setup.info`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     install_requires.append('translators')
     install_requires.append('twine')
 else:
     install_requires.append('twine==1.15.0')
 
 setup(
     name='wok_code',
-    version='2.0.6',
+    version='2.0.7',
     description='Python developers tools',
     long_description="""
 Various tools at your fingertips.
 
 The available tools are:
 
 * cvt_csv_2_rst.py: convert csv file into rst file
@@ -56,14 +56,15 @@
     packages=find_packages(exclude=['docs', 'examples', 'tests', 'egg-info', 'junk']),
     package_data={
         '': [
             'scripts/setup.info',
             'scripts/dist_pkg.sh',
             'scripts/please.sh',
             'scripts/config/*',
+            'scripts/run_odoo_debug.sh',
             './please.man',
             './cvt_script',
             './cvt_script.man',
             './topep8',
             './to_oca.2p8',
             './to_zero.2p8',
             './to_pep8.2p8',
@@ -74,14 +75,16 @@
     entry_points={
         'console_scripts': [
             'wok_code-info = wok_code.scripts.main:main',
             'cvt_csv_2_rst.py = wok_code.scripts.cvt_csv_2_rst:main',
             'cvt_csv_coa = wok_code.scripts.cvt_csv_coa:main',
             'deploy_odoo = wok_code.scripts.deploy_odoo:main',
             'dist_pkg = wok_code.scripts.dist_pkg:main',
+            'do_gitignore = wok_code.do_gitignore:main',
+            'do_git_checkout_new_branch = wok_code.do_git_checkout_new_branch:main',
             'do_migrate = wok_code.scripts.do_migrate:main',
             'do_odoo_site.py = wok_code.scripts.do_odoo_site:main',
             'gen_readme.py = wok_code.scripts.gen_readme:main',
             'lint_2_compare = wok_code.scripts.lint_2_compare:main',
             'makepo_it.py = wok_code.scripts.makepo_it:main',
             'odoo_dependencies.py = wok_code.scripts.odoo_dependencies:main',
             'odoo_translation.py = wok_code.scripts.odoo_translation:main',
```

### Comparing `wok_code-2.0.6/wok_code/cvt_csv_2_xml.py` & `wok_code-2.0.7/wok_code/cvt_csv_2_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 try:
     from z0lib import z0lib
 except ImportError:
     import z0lib
 
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 msg_time = time.time()
 
 
 def msg_burst(text):
     global msg_time
     t = time.time() - msg_time
```

### Comparing `wok_code-2.0.6/wok_code/cvt_script` & `wok_code-2.0.7/wok_code/cvt_script`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.6
+__version__=2.0.7
 
 #//Only human upgradable code/
 # blk1 => z0librc
 # blk2 => odoorc
 # blk3 => travisrc
 # blk4 => zarrc
 # blk8 => TESTDIR= ...
```

### Comparing `wok_code-2.0.6/wok_code/cvt_script.man` & `wok_code-2.0.7/wok_code/cvt_script.man`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.6/wok_code/do_git_checkout_new_branch.py` & `wok_code-2.0.7/wok_code/do_git_checkout_new_branch.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 import re
 import sys
 import os
 import argparse
 
 from z0lib import z0lib
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 
 class RepoCheckout(object):
 
     def __init__(self, opt_args):
         self.opt_args = opt_args
         if opt_args.odoo_branch not in ("16.0", "15.0", "14.0", "13.0", "12.0", "11.0",
                                         "10,0", "9.0", "8.0", "7.0", "6.1"):
             print("Invalid Odoo branch")
             exit(2)
         if (
-            not opt_args.oca_path
-            or not os.path.isdir(os.path.expanduser(opt_args.oca_path))
+            not opt_args.origin_path
+            or not os.path.isdir(os.path.expanduser(opt_args.origin_path))
         ):
-            print("Missed OCA path: use -o PATH!")
+            print("Missed origin path: use --origin-path=PATH!")
             exit(2)
-        self.opt_args.oca_path = os.path.expanduser(opt_args.oca_path)
+        if self.opt_args.origin_path not in (".", "./"):
+            self.opt_args.origin_path = os.path.expanduser(opt_args.origin_path)
         if not opt_args.target_path:
             print("Missed target path: use -p PATH!")
             exit(2)
         self.opt_args.target_path = os.path.expanduser(opt_args.target_path)
         if not opt_args.git_org:
             print("Missed git organization: use -G ORG!")
             exit(2)
@@ -64,161 +65,218 @@
             else:
                 git_url = "https://github.com/%s" % git_org
         return git_url, git_org
 
     def is_git_repo(self, path):
         return os.path.isdir(os.path.join(path, ".git"))
 
-    def build_new_repo(self, repo, oca_path):
-        target_path = self.opt_args.target_path if repo == "OCB" else os.path.join(
-            self.opt_args.target_path, repo)
-        if os.path.isdir(target_path):
-            if not self.opt_args.update:
-                print("Path %s already exists!" % target_path)
-                return 1
-        else:
-            z0lib.run_traced("cd %s" % os.path.dirname(target_path),
-                             verbose=self.opt_args.verbose,
-                             dry_run=self.opt_args.dry_run)
+    def build_new_repo(self, repo, origin_path):
+        def git_clone(repo, target_path):
+            if os.getcwd() != target_path:
+                z0lib.run_traced("cd %s" % os.path.dirname(target_path),
+                                 verbose=self.opt_args.verbose,
+                                 dry_run=self.opt_args.dry_run)
             git_repo = self.git_url + "/" + repo
             if repo == "OCB":
                 z0lib.run_traced(
                     ("git clone %s %s --depth=1 --no-single-branch "
                      "--no-recurse-submodules")
                     % (git_repo, os.path.basename(target_path)),
                     verbose=self.opt_args.verbose,
                     dry_run=self.opt_args.dry_run)
             else:
                 z0lib.run_traced("git clone %s --depth=1 --no-single-branch" % git_repo,
                                  verbose=self.opt_args.verbose,
                                  dry_run=self.opt_args.dry_run)
-        if not os.path.isdir(target_path):
-            print("Directory %s not created" % target_path)
-            return 0
-        z0lib.run_traced("cd %s" % target_path,
-                         verbose=self.opt_args.verbose,
-                         dry_run=self.opt_args.dry_run)
-        z0lib.run_traced("git checkout -b %s" % self.opt_args.odoo_branch,
-                         verbose=self.opt_args.verbose,
-                         dry_run=self.opt_args.dry_run)
-        sts, stdout, stderr = z0lib.run_traced("git branch",
-                                               verbose=self.opt_args.verbose,
-                                               dry_run=self.opt_args.dry_run)
-        for ln in stdout.split("\n"):
-            if not ln or ln.startswith("*"):
-                continue
-            z0lib.run_traced("git branch -D %s" % ln.strip(),
-                             verbose=self.opt_args.verbose,
-                             dry_run=self.opt_args.dry_run)
-        if repo == "OCB":
-            for p in os.listdir(oca_path):
-                if (
-                    p.startswith(".")
-                    or p.startswith("_")
-                    or os.path.isdir(os.path.join(oca_path, p, ".git"))
-                ):
-                    continue
-                src = os.path.join(oca_path, p)
-                if os.path.isfile(src):
-                    z0lib.run_traced("cp %s %s" % (src, target_path),
-                                     verbose=self.opt_args.verbose,
-                                     dry_run=self.opt_args.dry_run)
-                else:
-                    z0lib.run_traced("rsync -avzC --delete  --exclude \".*/\" %s/ %s/"
-                                     % (src, os.path.join(target_path, p)),
-                                     verbose=self.opt_args.verbose,
-                                     dry_run=self.opt_args.dry_run)
-        else:
-            z0lib.run_traced("rsync -avzC --delete  --exclude \".*/\" %s/ %s/"
-                             % (oca_path, target_path),
+
+        def git_checkout(target_path):
+            if os.getcwd() != target_path:
+                z0lib.run_traced("cd %s" % target_path,
+                                 verbose=self.opt_args.verbose,
+                                 dry_run=self.opt_args.dry_run)
+            z0lib.run_traced("git checkout -b %s" % self.opt_args.odoo_branch,
                              verbose=self.opt_args.verbose,
                              dry_run=self.opt_args.dry_run)
-        for p in os.listdir(target_path):
-            if (
-                p.startswith(".")
-                or p.startswith("_")
-                or p in ("egg-info", "readme")
-                or os.path.isdir(os.path.join(oca_path, p, ".git"))
-            ):
-                continue
-            src = os.path.join(target_path, p)
-            if not os.path.exists(os.path.join(oca_path, p)):
-                if os.path.isfile(src):
-                    z0lib.run_traced("rm -f %s" % src,
-                                     verbose=self.opt_args.verbose,
-                                     dry_run=self.opt_args.dry_run)
-                else:
-                    z0lib.run_traced("rm -fR %s" % src,
-                                     verbose=self.opt_args.verbose,
-                                     dry_run=self.opt_args.dry_run)
-        z0lib.run_traced("cd %s" % oca_path,
-                         verbose=self.opt_args.verbose,
-                         dry_run=self.opt_args.dry_run)
-        sts, stdout, stderr = z0lib.run_traced("git remote -v",
-                                               verbose=self.opt_args.verbose,
-                                               dry_run=self.opt_args.dry_run)
-        if sts == 0 and stdout:
-            url = ""
+
+        def git_delete_unrelated_branch(target_path):
+            if os.getcwd() != target_path:
+                z0lib.run_traced("cd %s" % target_path,
+                                 verbose=self.opt_args.verbose,
+                                 dry_run=self.opt_args.dry_run)
+            sts, stdout, stderr = z0lib.run_traced("git branch",
+                                                   verbose=self.opt_args.verbose,
+                                                   dry_run=self.opt_args.dry_run)
             for ln in stdout.split("\n"):
-                lns = ln.split()
-                if lns[0] == "origin":
-                    url = lns[1]
-                    break
-            if url:
-                if os.getcwd() != target_path:
-                    z0lib.run_traced("cd %s" % target_path,
-                                     verbose=self.opt_args.verbose,
-                                     dry_run=self.opt_args.dry_run)
-                z0lib.run_traced("git remote add oca %s" % url,
+                if not ln or ln.startswith("*"):
+                    continue
+                z0lib.run_traced("git branch -D %s" % ln.strip(),
+                                 verbose=self.opt_args.verbose,
+                                 dry_run=self.opt_args.dry_run)
+
+        def git_add_all(target_path):
+            if os.getcwd() != target_path:
+                z0lib.run_traced("cd %s" % target_path,
                                  verbose=self.opt_args.verbose,
                                  dry_run=self.opt_args.dry_run)
-        if sts == 0 and self.opt_args.save_git:
+            z0lib.run_traced("git add ./",
+                             verbose=self.opt_args.verbose,
+                             dry_run=self.opt_args.dry_run)
+
+        def git_push(target_path):
             if os.getcwd() != target_path:
                 z0lib.run_traced("cd %s" % target_path,
                                  verbose=self.opt_args.verbose,
                                  dry_run=self.opt_args.dry_run)
             found = False
             sts, stdout, stderr = z0lib.run_traced("git branch")
             if sts == 0 and stdout:
                 regex = r"^[*]* +" + self.opt_args.odoo_branch + r" *$"
                 for ln in stdout.split("\n"):
                     if re.match(regex, ln):
                         found = True
                         break
-            if found and self.opt_args.remove_remote_branch:
+            if found and self.opt_args.remove_unrelated_branch:
                 z0lib.run_traced("git push origin delete %s"
                                  % self.opt_args.odoo_branch,
                                  verbose=self.opt_args.verbose,
                                  dry_run=self.opt_args.dry_run)
                 found = False
-            z0lib.run_traced("git add ./",
-                             verbose=self.opt_args.verbose,
-                             dry_run=self.opt_args.dry_run)
             z0lib.run_traced("git commit --no-verify -m \"[NEW] Initial setup %s\""
                              % self.opt_args.odoo_branch,
                              verbose=self.opt_args.verbose,
                              dry_run=self.opt_args.dry_run)
             if found:
                 z0lib.run_traced("git push",
                                  verbose=self.opt_args.verbose,
                                  dry_run=self.opt_args.dry_run)
             else:
                 z0lib.run_traced("git push --set-upstream origin %s"
                                  % self.opt_args.odoo_branch,
                                  verbose=self.opt_args.verbose,
                                  dry_run=self.opt_args.dry_run)
+
+        def rsync_origin_path(repo, origin_path, target_path):
+            exclude_path = self.opt_args.exclude_path.split(",")
+            exclude_opt = "--exclude \".*/\""
+            for p in exclude_path:
+                exclude_opt += " --exclude \"/%s\"" % p
+            if repo == "OCB":
+                for p in os.listdir(origin_path):
+                    if (
+                        p.startswith(".")
+                        or p.startswith("_")
+                        or os.path.isdir(os.path.join(origin_path, p, ".git"))
+                        or p in exclude_path
+                    ):
+                        continue
+                    src = os.path.join(origin_path, p)
+                    if os.path.isfile(src):
+                        z0lib.run_traced("cp %s %s" % (src, target_path),
+                                         verbose=self.opt_args.verbose,
+                                         dry_run=self.opt_args.dry_run)
+                    else:
+                        z0lib.run_traced(
+                            "rsync -avz --delete %s %s/ %s/"
+                            % (exclude_opt, src, os.path.join(target_path, p)),
+                            verbose=self.opt_args.verbose,
+                            dry_run=self.opt_args.dry_run)
+            else:
+                z0lib.run_traced("rsync -avz --delete %s %s/ %s/"
+                                 % (exclude_opt, origin_path, target_path),
+                                 verbose=self.opt_args.verbose,
+                                 dry_run=self.opt_args.dry_run)
+            for p in os.listdir(target_path):
+                if (
+                    p.startswith(".")
+                    or p.startswith("_")
+                    or p in ("egg-info", "readme")
+                    or os.path.isdir(os.path.join(origin_path, p, ".git"))
+                ):
+                    continue
+                src = os.path.join(target_path, p)
+                if not os.path.exists(os.path.join(origin_path, p)):
+                    if os.path.isfile(src):
+                        z0lib.run_traced("rm -f %s" % src,
+                                         verbose=self.opt_args.verbose,
+                                         dry_run=self.opt_args.dry_run)
+                    else:
+                        z0lib.run_traced("rm -fR %s" % src,
+                                         verbose=self.opt_args.verbose,
+                                         dry_run=self.opt_args.dry_run)
+            if repo == "OCB":
+                z0lib.run_traced("do_gitignore ./",
+                                 verbose=self.opt_args.verbose,
+                                 dry_run=self.opt_args.dry_run)
+            if os.getcwd() != origin_path:
+                z0lib.run_traced("cd %s" % origin_path,
+                                 verbose=self.opt_args.verbose,
+                                 dry_run=self.opt_args.dry_run)
+            sts, stdout, stderr = z0lib.run_traced("git remote -v",
+                                                   verbose=self.opt_args.verbose,
+                                                   dry_run=self.opt_args.dry_run)
+            url = ""
+            if sts == 0 and stdout:
+                for ln in stdout.split("\n"):
+                    lns = ln.split()
+                    if len(lns) < 2:
+                        continue
+                    elif lns[0] == "origin":
+                        url = lns[1]
+                        break
+            if url:
+                if os.getcwd() != target_path:
+                    z0lib.run_traced("cd %s" % target_path,
+                                     verbose=self.opt_args.verbose,
+                                     dry_run=self.opt_args.dry_run)
+                url_upstream = ""
+                for ln in stdout.split("\n"):
+                    lns = ln.split()
+                    if len(lns) < 2:
+                        continue
+                    elif lns[0] == "upstream":
+                        url_upstream = lns[1]
+                        break
+                if url_upstream:
+                    z0lib.run_traced("git remote remove upstream",
+                                     verbose=self.opt_args.verbose,
+                                     dry_run=self.opt_args.dry_run)
+                z0lib.run_traced("git remote add upstream %s" % url,
+                                 verbose=self.opt_args.verbose,
+                                 dry_run=self.opt_args.dry_run)
+
+        target_path = self.opt_args.target_path if repo == "OCB" else os.path.join(
+            self.opt_args.target_path, repo)
+        if os.path.isdir(target_path):
+            if not self.opt_args.update:
+                print("Path %s already exists!" % target_path)
+                return 1
+        git_clone(repo, target_path)
+        if not os.path.isdir(target_path):
+            print("Directory %s not created" % target_path)
+            return 0
+        git_checkout(target_path)
+        git_delete_unrelated_branch(target_path)
+        if self.opt_args.origin_path not in (".", "./"):
+            rsync_origin_path(repo, origin_path, target_path)
+        elif repo == "OCB":
+            z0lib.run_traced("gitignore ./",
+                             verbose=self.opt_args.verbose,
+                             dry_run=self.opt_args.dry_run)
+        git_add_all(target_path)
+        if self.opt_args.save_git:
+            git_push(target_path)
         return 0
 
-    def git_checkout(self):
-        path = self.opt_args.oca_path
+    def do_git_checkout(self):
+        path = self.opt_args.origin_path
         if self.is_git_repo(path):
             sts = self.build_new_repo("OCB", path)
         if sts == 0:
-            for repo in sorted(os.listdir(self.opt_args.oca_path)):
-                path = os.path.join(self.opt_args.oca_path, repo)
+            for repo in sorted(os.listdir(self.opt_args.origin_path)):
+                path = os.path.join(self.opt_args.origin_path, repo)
                 if self.is_git_repo(path):
                     sts = self.build_new_repo(repo, path)
                     if sts:
                         break
         return sts
 
 
@@ -228,25 +286,37 @@
         description="Create new repo branch",
         epilog="© 2022-2023 by SHS-AV s.r.l."
     )
     parser.add_argument("-b", "--odoo-branch",
                         dest="odoo_branch",
                         help="New Odoo branch")
     parser.add_argument("-G", "--git-org",
-                        help="Git organization")
+                        help="Git organization to checkout")
     parser.add_argument("-n", "--dry-run", action="store_true")
-    parser.add_argument("-o", "--oca-path",
-                        help="Local directory")
+    parser.add_argument(
+        "-o", "--origin-path",
+        help="Local origin directory to merge or ./ if not origin (best is OCA path)")
     parser.add_argument("-p", "--target-path",
-                        help="Local directory")
-    parser.add_argument("-R", "--remove-remote-branch", action="store_true")
-    parser.add_argument("-S", "--save-git", action="store_true")
-    parser.add_argument("-U", "--update", action="store_true")
+                        help="Local directory for checkout")
+    parser.add_argument(
+        "-R",  "--remove-unrelated-branch",
+        help="Remove not required unrelated branch from local directory",
+        action="store_true")
+    parser.add_argument("-S",  "--save-git",
+                        help="Execute git pull after checkout",
+                        action="store_true")
+    parser.add_argument("-U",
+                        "--update",
+                        help="Update target directory if exists",
+                        action="store_true")
     parser.add_argument("-v", "--verbose", action="count", default=0)
     parser.add_argument("-V", "--version", action="version", version=__version__)
+    parser.add_argument("-x", "--exclude-path",
+                        help="Directories to exclude (comma separated)",
+                        default="setup,venv_odoo")
     opt_args = parser.parse_args(cli_args)
     repo = RepoCheckout(opt_args)
-    return repo.git_checkout()
+    return repo.do_git_checkout()
 
 
 if __name__ == "__main__":
     exit(main(None))
```

### Comparing `wok_code-2.0.6/wok_code/do_gitignore.py` & `wok_code-2.0.7/wok_code/do_gitignore.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,8 +87,8 @@
     else:
         print('Path %s does not exist!' % sys.argv[0])
         return 2
     return 0
 
 
 if __name__ == "__main__":
-    exit(main(None))
+    exit(main(sys.argv))
```

### Comparing `wok_code-2.0.6/wok_code/do_set_utf8.py` & `wok_code-2.0.7/wok_code/do_set_utf8.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.6/wok_code/eval_gtin.py` & `wok_code-2.0.7/wok_code/eval_gtin.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.6/wok_code/gen_addons_table.py` & `wok_code-2.0.7/wok_code/gen_addons_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from past.builtins import cmp
 
 standard_library.install_aliases()  # noqa: E402
 
 
 MARKERS = r'(\[//\]: # \(addons\))|(\[//\]: # \(end addons\))'
 MANIFESTS = ('__openerp__.py', '__manifest__.py')
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 
 class UserError(Exception):
     def __init__(self, msg):
         self.msg = msg
```

### Comparing `wok_code-2.0.6/wok_code/pgconf.py` & `wok_code-2.0.7/wok_code/pgconf.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.6/wok_code/please.man` & `wok_code-2.0.7/wok_code/please.man`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.6/wok_code/pypi.sh` & `wok_code-2.0.7/wok_code/pypi.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # set -x
-__version__=2.0.6
+__version__=2.0.7
 if [[ -z $HOME_DEVEL || ! -d $HOME_DEVEL ]]; then
   [[ -d $HOME/odoo/devel ]] && HOME_DEVEL="$HOME/odoo/devel" || HOME_DEVEL="$HOME/devel"
 fi
 
 run_traced() {
     local xcmd="$1"
     local sts=0
```

### Comparing `wok_code-2.0.6/wok_code/scripts/__init__.py` & `wok_code-2.0.7/wok_code/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.6/wok_code/scripts/config/to_new_api.yml` & `wok_code-2.0.7/wok_code/scripts/config/to_new_api.yml`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.6/wok_code/scripts/config/to_old_api.yml` & `wok_code-2.0.7/wok_code/scripts/config/to_old_api.yml`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.6/wok_code/scripts/cvt_csv_2_rst.py` & `wok_code-2.0.7/wok_code/scripts/cvt_csv_2_rst.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 try:
     from z0lib import z0lib
 except ImportError:
     import z0lib
 
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 msg_time = time.time()
 
 
 def msg_burst(text):
     global msg_time
     t = time.time() - msg_time
```

### Comparing `wok_code-2.0.6/wok_code/scripts/cvt_csv_coa.py` & `wok_code-2.0.7/wok_code/scripts/cvt_csv_coa.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import argparse
 import time
 
 from os0 import os0
 from python_plus import unicodes
 from clodoo import transodoo
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 msg_time = time.time()
 VALID_ACTIONS = ("export-comparable", "export-full", "export-z0bug", "export-group")
 VERSIONS = ["6.1", "7.0", "8.0", "9.0", "10.0", "11.0", "12.0", "13.0", "14.0"]
 
 
 class CvtCsvFile(object):
```

### Comparing `wok_code-2.0.6/wok_code/scripts/deploy_odoo.py` & `wok_code-2.0.7/wok_code/scripts/deploy_odoo.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     from wok_code.scripts.wget_odoo_repositories import main as get_list_from_url
 try:
     from clodoo.clodoo import build_odoo_param
 except ImportError:
     from clodoo import build_odoo_param
 
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 MANIFEST_FILES = ["__manifest__.py", "__odoo__.py", "__openerp__.py", "__terp__.py"]
 
 ODOO_VALID_VERSIONS = (
     "16.0",
     "15.0",
     "14.0",
@@ -118,31 +118,31 @@
     "path": "%(path)-56.56s",
     "stash": "%(stash)5.5s",
     "status": "%(status)s",
 }
 
 
 class OdooDeploy(object):
-    """Odoo organization/branch repositories
+    """Odoo's organization/branch repositories
     self.repo_list is the repositories list of self.repo_info
     self.repo_info contains repository information
     * BRANCH: git branch
     * PATH: repository path
     * URL: git URL
     * GIT_ORG: git organization
     * STS: os status
     """
 
     def __init__(self, opt_args):
         self.opt_args = opt_args
         self.opt_args.git_orgs = self.opt_args.git_orgs or []
-        self.get_addons_from_config_file()
         self.addons_path = []
         self.master_branch = ""
         self.target_path = ""
+        self.get_addons_from_config_file()
 
         if self.opt_args.action in ("clone", "reclone"):
             if not self.opt_args.odoo_branch:
                 print("***** Missing Odoo branch: 12.0 will be used!")
                 self.opt_args.odoo_branch = "12.0"
             if not self.opt_args.git_orgs:
                 print("***** Missing git orgs: oca will be used!")
@@ -170,14 +170,17 @@
         if not self.repo_list and not self.opt_args.target_path:
             self.get_repo_from_config()
 
         if not self.repo_list:
             self.target_path = os.path.expanduser(self.opt_args.target_path)
             self.get_repo_from_path()
 
+        if not self.repo_list:
+            print("***** No repositories found!")
+
         for repo in self.repo_list:
             path = self.repo_info[repo]["PATH"]
             git_org = self.opt_args.git_orgs[0] if self.opt_args.git_orgs else "oca"
             if os.path.isdir(path):
                 z0lib.run_traced("cd %s" % path, verbose=False, dry_run=False)
                 sts, repo_branch, git_url, stash_list = self.get_remote_info(
                     verbose=False
@@ -248,14 +251,16 @@
             elif git_org == "oca":
                 git_url = "https://github.com/%s" % git_org.upper()
             else:
                 git_url = "https://github.com/%s" % git_org
         return git_url, git_org
 
     def get_repo_from_switch(self):
+        self.repo_list = []
+        self.repo_info = {}
         for repo in self.opt_args.repos.split(","):
             self.repo_info[repo] = {
                 "PATH": self.get_path_of_repo(repo),
                 "#": 1
             }
         self.repo_list = sorted(self.repo_info.keys())
         if "OCB" in self.repo_list:
@@ -396,17 +401,17 @@
             opts.append("-b")
             opts.append(branch)
         opts.append("-l")
         opts.append(self.opt_args.local_reps)
         # opts.append("l10n-italy,l10n-italy-supplemental")
         opts.append("-G")
         opts.append(SHORT_NAMES.get(git_org, git_org))
-        if self.opt_args.extra:
+        if self.opt_args.extra_repo:
             opts.append("-x")
-            opts.append(self.opt_args.extra)
+            opts.append(self.opt_args.extra_repo)
         opts.append("--return-repos")
         if only_ocb:
             content = ["OCB"]
         else:
             content = get_list_from_url(opts)
         for repo in content:
             if repo not in self.repo_list:
@@ -744,21 +749,55 @@
                 sleep(1)
         if sts:
             print("Invalid branch %s" % branch)
         sleep(1)
         cmd = "git pull"
         return self.run_traced(cmd)[0], repo_branch
 
+    def git_push(self, repo, tgtdir):
+        if os.getcwd() != tgtdir:
+            self.run_traced("cd %s" % tgtdir)
+        sts, repo_branch, git_url, stash_list = self.get_remote_info()
+        if os.path.islink(tgtdir):
+            return sts, repo_branch
+        cmd = "git push"
+        sts, stdout, stderr = self.run_traced(cmd, verbose=False)
+        if sts:
+            sts, stdout, stderr = z0lib.run_traced("git branch -r",
+                                                   verbose=self.opt_args.verbose)
+            tag = "origin/%s" % repo_branch
+            for ln in stdout.split("\n"):
+                if tag in ln:
+                    if not self.opt_args.assume_yes:
+                        print("Remove remote branch %s of %s!" % (repo_branch, repo))
+                        dummy = input("Delete (y/n)? ")
+                    if self.opt_args.assume_yes or dummy.lower().startswith("y"):
+                        self.run_traced("git push origin -d %s" % repo_branch,
+                                        verbose=self.opt_args.verbose)
+                    self.run_traced(
+                        "git commit --no-verify -m \"[NEW] Initial setup %s\""
+                        % repo_branch,
+                        verbose=self.opt_args.verbose)
+                    break
+            cmd = "git push --set-upstream origin %s" % repo_branch
+            sts, stdout, stderr = self.run_traced(cmd, verbose=self.opt_args.verbose)
+        sleep(1)
+        if sts == 0:
+            sts, repo_branch, git_url, stash_list = self.get_remote_info()
+        if sts:
+            print("***ERROR\n%s\n%s" % (stdout, stderr))
+        return sts, repo_branch
+
     def download_single_repo(self, repo, git_org=None, branch=None):
         git_org = git_org or self.git_org
         branch = branch or self.opt_args.odoo_branch
         odoo_master_branch = build_odoo_param("FULLVER", odoo_vid=branch)
         git_url = stash_list = ""
         tgtdir = self.get_path_of_repo(repo)
-        if self.opt_args.action == "update":
+        if self.opt_args.action in ("update", "git-push"):
             if not os.path.isdir(tgtdir):
                 return 127
             if os.getcwd() != tgtdir:
                 self.run_traced("cd %s" % tgtdir)
             sts, repo_branch, git_url, stash_list = self.get_remote_info()
             if sts == 0:
                 org_url, repo, repo_org = self.data_from_url(git_url)
@@ -773,15 +812,15 @@
                 git_url = self.repo_info[repo].get("URL")
                 if not git_url:
                     git_url, git_org = self.get_git_org_n_url(git_org)
                     git_url = git_url + "/" + repo + ".git"
         if not git_url:
             return 127
         bakdir = ""
-        if os.path.isdir(tgtdir) and self.opt_args.action != "update":
+        if os.path.isdir(tgtdir) and self.opt_args.action not in ("update", "git-push"):
             if self.opt_args.skip_if_exist:
                 return self.git_pull(tgtdir, branch, master_branch=odoo_master_branch)
             elif not self.opt_args.assume_yes:
                 print("Path %s of repo %s already exists!" % (tgtdir, repo))
                 dummy = input("Delete (y/n)? ")
                 if not dummy.lower().startswith("y"):
                     return 3
@@ -795,14 +834,16 @@
             elif not os.path.islink(tgtdir):
                 cmd = "rm -fR %s" % tgtdir
                 self.run_traced(cmd)
         if os.path.isdir(tgtdir) and self.opt_args.action == "update":
             sts, remote_branch = self.git_pull(
                 tgtdir, branch, master_branch=odoo_master_branch
             )
+        elif os.path.isdir(tgtdir) and self.opt_args.action == "git-push":
+            sts, remote_branch = self.git_push(repo, tgtdir)
         else:
             sts, remote_branch = self.git_clone(
                 git_url,
                 tgtdir,
                 branch,
                 master_branch=odoo_master_branch,
                 compact=True if git_org in ("odoo", "oca") else False,
@@ -840,15 +881,15 @@
             self.add_addons_path(tgtdir, repo)
         if sts:
             print("*** Error ***")
             if not self.opt_args.verbose:
                 dummy = input("Press RET to continue ...")
         return sts
 
-    def list_data(self):
+    def action_list(self):
         print("Odoo main version..........: %s" % self.master_branch)
         if self.opt_args.config:
             print("Odoo configuration file....: %s" % self.opt_args.config)
         fmt_list = self.opt_args.format.split(",")
         fmt = ""
         datas = {}
         for item in fmt_list:
@@ -870,15 +911,15 @@
                 "stash": "stash" if self.repo_info[repo].get("STASH") else "",
             }
             print(fmt % datas)
         if self.opt_args.show_addons:
             print()
             print(",".join(self.addons_path))
 
-    def list_repo_info(self):
+    def action_status(self):
         print("Odoo main version..........: %s" % self.master_branch)
         if self.opt_args.config:
             print("Odoo configuration file....: %s" % self.opt_args.config)
         fmt_list = self.opt_args.format.split(",")
         fmt = ""
         datas = {}
         for item in fmt_list:
@@ -909,26 +950,26 @@
                 "status": git_stat,
             }
             print(fmt % datas)
         if self.opt_args.show_addons:
             print()
             print(",".join(self.addons_path))
 
-    def download_or_pull_repo(self):
+    def action_download_or_pull_repo(self):
         print("Odoo main version..........: %s" % self.master_branch)
         if self.opt_args.config:
             print("Odoo configuration file....: %s" % self.opt_args.config)
         for repo in self.repo_list:
             self.download_single_repo(repo)
         if self.opt_args.verbose and self.addons_path:
             print("addons_path = %s" % ",".join(self.addons_path))
         if self.opt_args.update_addons_conf:
             self.update_conf()
         if self.opt_args.verbose:
-            self.list_repo_info()
+            self.action_status()
 
 
 def main(cli_args=None):
     cli_args = cli_args or sys.argv[1:]
     parser = argparse.ArgumentParser(
         description="Manage Odoo repositories", epilog="© 2021-2023 by SHS-AV s.r.l."
     )
@@ -953,15 +994,15 @@
     )
     parser.add_argument("-c", "--config", help="Odoo configuration file")
     parser.add_argument("-D", "--default-gitorg", default="zero")
     # parser.add_argument("-d", "--deployment-mode", help="may be tree,server,odoo")
     parser.add_argument(
         "-e", "--skip-if-exist",
         action="store_true",
-        help="Use this switch  to add missed repositories when you reclone"
+        help="Use this switch to add missed repositories when you reclone"
     )
     parser.add_argument(
         "-F",
         "--format",
         help=("Use 1 or + of " "sts,repo,branch,git_org,git_url,path,stash,status"),
         default="sts,repo,branch,git_org,git_url,path,stash",
     )
@@ -997,42 +1038,46 @@
         "-N",
         "--clone",
         action="store_true",
         help="Deprecated: use 'clone' action!",
     )
     parser.add_argument("-n", "--dry-run", action="store_true")
     parser.add_argument(
+        "-o", "--origin",
+        help="Declare origin repo for 'merge' action"
+    )
+    parser.add_argument(
         "-O", "--link-oca", action="store_true", help="Link to more OCA repositories"
     )
     parser.add_argument("-p", "--target-path", help="Local directory")
     parser.add_argument(
         "-R", "--reclone", action="store_true", help="Deprecated: use 'reclone' action!"
     )
     parser.add_argument(
         "-r", "--repos",
-        help="Declare specific repositories to managa, comma separated"
+        help="Declare specific repositories to manage, comma separated"
     )
     parser.add_argument(
         "-S", "--status", action="store_true", help="Deprecated: use 'status' action!"
     )
     parser.add_argument(
         "-U",
         "--only-update",
         action="store_true",
         help="Deprecated: use 'update' action!",
     )
     parser.add_argument("-v", "--verbose", action="count", default=0)
     parser.add_argument("-V", "--version", action="version", version=__version__)
     parser.add_argument(
-        "-x", "--extra",
+        "-x", "--extra-repo",
         help="May be: all,none,connector,devel,maintainer,oca,odoo,vertical"
     )
     parser.add_argument("-y", "--assume-yes", action="store_true")
     parser.add_argument(
-        "action", nargs="?", help="May be clone,list,reclone,status,update"
+        "action", nargs="?", help="May be clone,git-push,list,reclone,status,update"
     )
     opt_args = parser.parse_args(cli_args)
 
     if not opt_args.action:
         if opt_args.clone:
             opt_args.action = "clone"
         elif opt_args.list:
@@ -1042,32 +1087,33 @@
         elif opt_args.status:
             opt_args.action = "status"
         elif opt_args.only_update:
             opt_args.action = "update"
     opt_args.git_orgs = opt_args.git_orgs.split(",") if opt_args.git_orgs else []
 
     if (
-        opt_args.action != "update"
-        and opt_args.action != "clone"
-        and opt_args.action != "reclone"
-        and opt_args.action != "list"
-        and opt_args.action != "status"
+        opt_args.action not in ("clone",
+                                "git-push",
+                                "list",
+                                "reclone",
+                                "status",
+                                "update")
     ):
         print("No valid action issued!")
         exit(1)
 
     if opt_args.repos and not opt_args.target_path:
         print("No path issued for declared repositories")
         exit(1)
 
     deploy = OdooDeploy(opt_args)
     if opt_args.action == "list":
-        deploy.list_data()
+        deploy.action_list()
     elif opt_args.action == "status":
-        deploy.list_repo_info()
+        deploy.action_status()
     else:
-        deploy.download_or_pull_repo()
+        deploy.action_download_or_pull_repo()
     return 0
 
 
 if __name__ == "__main__":
     exit(main())
```

### Comparing `wok_code-2.0.6/wok_code/scripts/dist_pkg.py` & `wok_code-2.0.7/wok_code/scripts/run_odoo_debug.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.6/wok_code/scripts/dist_pkg.sh` & `wok_code-2.0.7/wok_code/scripts/dist_pkg.sh`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.6
+__version__=2.0.7
 
 # main
 OPTOPTS=(h        C         c        D        F         f         n            O         o        P         p         q           R         S        u       V           v           W          w         -)
 OPTDEST=(opt_help opt_cpush opt_conf opt_push opt_fetch opt_force opt_dry_run  opt_cpush opt_ids  opt_cpush opt_dpath opt_verbose opt_cpush opt_sts  opt_upd opt_version opt_verbose opt_whatis opt_cpush opt_sync)
 OPTACTI=("+"      "*>"      "="      "*>"     "1>"      1         1            "*>"      "=>"     "*>"      "="       0           "*>"      "=>"     1       "*"         "+"         "=>"       "*>"      "1>")
 OPTDEFL=(1        ""        ""       ""       0         0         0            ""        ""       ""        ""        0           ""        ""       0       ""          -1          ""         ""        0)
 OPTMETA=("help"   "commit"  "file"   ""       "fetch"   ""        "do nothing" ""        "prj_id" "push"    "path"    "quiet"     "replace" "status" "upd"   "version"   "verbose"   "param"    "wep"     "sync")
```

### Comparing `wok_code-2.0.6/wok_code/scripts/do_migrate.py` & `wok_code-2.0.7/wok_code/scripts/do_migrate.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import argparse
 import re
 import lxml.etree as ET
 import yaml
 from python_plus import _b
 from z0lib import z0lib
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 # RULES: every rule is list has the following format:
 # EREGEX, (ACTION, PARAMETERS), ...
 # where
 # - EREGEX is an enhanced regular expression to apply the rule.
 # - ACTION is the action to apply on current line
 # - PARAMETERS are the values to supply on action
```

### Comparing `wok_code-2.0.6/wok_code/scripts/do_odoo_site.py` & `wok_code-2.0.7/wok_code/scripts/do_odoo_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     SSLCertificateKeyFile
     Include /etc/letsencrypt/options-ssl-apache.conf
     SSLCertificateChainFile
 </VirtualHost>
 </IfModule>
 """
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 
 class CreateConfig(object):
 
     def __init__(self, domain, opt_args):
         self.opt_args = opt_args
         if "." in domain:
```

### Comparing `wok_code-2.0.6/wok_code/scripts/gen_readme.py` & `wok_code-2.0.7/wok_code/scripts/gen_readme.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     from python_plus.python_plus import _b, _c, _u
 except ImportError:
     from python_plus import _b, _c, _u
 # import pdb
 standard_library.install_aliases()
 
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 RED = "\033[1;31m"
 GREEN = "\033[1;32m"
 YELLOW = "\033[1;33m"
 CLEAR = "\033[0;m"
 GIT_USER = {
     "zero": "zeroincombenze",
```

### Comparing `wok_code-2.0.6/wok_code/scripts/generate_random_codes.py` & `wok_code-2.0.7/wok_code/scripts/generate_random_codes.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 # import os
 import argparse
 from random import random, randint
 import vatnumber
 
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 
 def gen_vatnumber(opt_args):
     found = False
     while not found:
         seed = "%7.7s%3.03i" % (random() * 10000000, randint(1, 99))
         for i in range(10):
```

### Comparing `wok_code-2.0.6/wok_code/scripts/license_mgnt.py` & `wok_code-2.0.7/wok_code/scripts/license_mgnt.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.6/wok_code/scripts/lint_2_compare.py` & `wok_code-2.0.7/wok_code/scripts/lint_2_compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 import argparse
 from lxml import etree
 
 from python_plus import _b, _u
 from z0lib import z0lib
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 
 IGNORE_DIRS = (".idea", ".git", "egg-info", "setup")
 
 
 def get_names(left_path, right_path):
     left_base = right_base = ''
```

### Comparing `wok_code-2.0.6/wok_code/scripts/main.py` & `wok_code-2.0.7/wok_code/scripts/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# template 20
+# template 21
 """
 Various tools at your fingertips.
 
 The available tools are:
 
 * cvt_csv_2_rst.py: convert csv file into rst file
 * cvt_csv_2_xml.py: convert csv file into xml file
@@ -19,15 +19,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
@@ -103,20 +103,28 @@
                             else:
                                 fd.write(help_text)
                         if verbose:
                             print("$ gzip -c %s > %s" % (full_fn, tgt_fn))
                         continue
                     if lib_path:
                         tgt_fn = os.path.join(lib_path, base)
-                        try:
-                            shutil.copy(full_fn, tgt_fn)
-                            if verbose:
-                                print("$ cp %s %s" % (full_fn, tgt_fn))
-                        except shutil.SameFileError:
-                            pass
+                        if sys.version_info[0] == 3:
+                            try:
+                                shutil.copy(full_fn, tgt_fn)
+                                if verbose:
+                                    print("$ cp %s %s" % (full_fn, tgt_fn))
+                            except shutil.SameFileError:
+                                pass
+                        else:
+                            try:
+                                shutil.copy(full_fn, tgt_fn)
+                                if verbose:
+                                    print("$ cp %s %s" % (full_fn, tgt_fn))
+                            except BaseException:
+                                pass
                     # TODO> compatibility mode
                     tgt_fn = os.path.join(bin_path, base)
                     if os.path.isfile(tgt_fn):
                         os.unlink(tgt_fn)
                     if not os.path.exists(tgt_fn):
                         if verbose:
                             print("$ ln -s %s %s" % (full_fn, tgt_fn))
```

### Comparing `wok_code-2.0.6/wok_code/scripts/makepo_it.py` & `wok_code-2.0.7/wok_code/scripts/makepo_it.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from __future__ import print_function
 
 import os.path
 import sys
 import argparse
 # import pdb
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 PO_DEFAULT = """
 # Translation of Odoo Server.
 # This file contains the translation of the following modules:
 #   * MODULE
 #
 msgid ""
```

### Comparing `wok_code-2.0.6/wok_code/scripts/odoo_dependencies.py` & `wok_code-2.0.7/wok_code/scripts/odoo_dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 except ImportError:
     from z0lib import z0lib
 try:
     from clodoo import clodoo
 except ImportError:
     import clodoo
 
-__version__ = '2.0.6'
+__version__ = '2.0.7'
 
 
 MANIFEST_FILES = ['__manifest__.py', '__odoo__.py', '__openerp__.py', '__terp__.py']
 MAX_DEEP = 20
 UNDEF_DEEP = MAX_DEEP + 5
 MISSED = 99
```

### Comparing `wok_code-2.0.6/wok_code/scripts/odoo_translation.py` & `wok_code-2.0.7/wok_code/scripts/odoo_translation.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,17 +8,22 @@
 from time import time, sleep
 import argparse
 import re
 import collections
 from babel.messages import pofile
 from openpyxl import load_workbook, Workbook
 
+try:
+    from clodoo import clodoo
+except ImportError:
+    import clodoo
+
 # from python_plus import unicodes
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 
 MODULE_SEP = "\ufffa"
 
 # (<en>, <it>, <module>, <result>, ovverride)
 TEST_DATA = [
     ("name", "nome", None, "nome"),
@@ -71,14 +76,27 @@
     ("Customer SEPA account", None, None, "Conto cliente SEPA"),
     ("Customer SEPA account", "Conto cliente SEPA", None, "Conto cliente SEPA", True),
     ("Account (Credit)", "Conto (avere)", None, "Conto (avere)"),
     ("Account (Credit)", None, "l10n_it", "Conto (Avere)"),
     ("Other Info", "Altre informazioni", None, "Altre informazioni"),
     ("Other Info", "Altre info", "l10n_it", "Altre info"),
 ]
+
+TNL_TYPES = (
+    'ir.actions.act_window,name',
+    'ir.model,name',
+    'ir.model.fields.field_description',
+    'ir.module.category,name',
+    'ir.module.module,description'
+    'ir.module.module,shortdesc',
+    'ir.module.module,summary',
+    'ir.ui.menu,name',
+    'ir.ui.view,arch_db',
+)
+
 msg_time = time()
 
 
 def msg_burst(text):
     global msg_time
     t = time() - msg_time
     if t > 5:
@@ -431,14 +449,16 @@
                 hash_key += hash_orig[ix]
             ix += 1
         return term_tnxl, hash_key
 
     def do_dict_item(
         self, msg_orig, msg_tnxl, action=None, override=None, module=None, is_tag=None,
     ):
+        if not msg_orig:
+            return msg_orig
         action = action or ("build_dict" if override else "translate")
         if self.get_untransable_token(msg_orig):
             return msg_orig
         if not msg_tnxl:
             msg_tnxl = msg_orig
         msg_orig = msg_orig.replace("’", "'")
         msg_tnxl = msg_tnxl.replace("’", "'")
@@ -777,15 +797,16 @@
                 row = {}
                 for ncol, cell in enumerate(nrow):
                     row[colnames[ncol]] = (
                         cell.value.replace("\\n", "\n") if cell.value else cell.value
                     )
                 if not row["msgid"] or not row["msgstr"]:
                     continue
-                msg_burst('%s ...' % row["msgid"])
+                if self.opt_args.verbose:
+                    msg_burst('%s ...' % row["msgid"])
                 if "hashkey" in row and row["hashkey"]:
                     if row["hashkey"] not in self.dict:
                         self.dict[row["hashkey"]] = (row["msgid"], row["msgstr"])
                 else:
                     self.do_dict_item(row["msgid"],
                                       row["msgstr"],
                                       action="build_dict",
@@ -834,36 +855,159 @@
         ):
             self.do_dict_item(msg_orig,
                               msg_tnxl,
                               action="build_dict",
                               is_tag=is_tag)
 
     def build_dict(self):
-        # if self.opt_args.file_xlsx:
-        #     root = self.get_home_devel()
-        #     if root:
-        #         dict_name = os.path.join(
-        #             root, 'pypi', 'tools', 'odoo_template_tnl.xlsx')
-        #         if os.path.isfile(dict_name):
-        #             self.load_terms_from_xlsx(dict_name)
-        #     self.load_terms_from_xlsx(self.opt_args.file_xlsx)
-        if not self.opt_args.module_name:
+        if self.opt_args.database and self.opt_args.file_xlsx:
+            self.load_terms_from_xlsx(self.opt_args.file_xlsx)
+        elif not self.opt_args.module_name:
             target_path = os.path.abspath(self.opt_args.target_path)
             self.do_work_on_path(target_path, None)
             for root, dirs, files in os.walk(target_path,
                                              topdown=True,
                                              followlinks=False):
                 dirs[:] = [
                     d
                     for d in dirs
                     if d not in (".git", "__to_remove", "doc", "setup", ".idea")
                 ]
                 for base in dirs:
                     self.do_work_on_path(root, base, action="build_dict")
 
+    def install_lang(self, lang, ctx):
+        model = 'res.lang'
+        vals = {
+            'lang': lang,
+        }
+        ids = clodoo.searchL8(ctx, model, [('code', '=', lang)])
+        if not ids:
+            if self.opt_args.verbose:
+                print('Language %s not installed: installing it now' % lang)
+            id = clodoo.createL8(ctx, 'base.language.install', vals)
+            clodoo.executeL8(ctx, 'base.language.install', 'lang_install', [id])
+            clodoo.writeL8(ctx, "res.users", ctx["user_id"], {"lang": lang})
+        elif self.opt_args.verbose:
+            print('Found language %s' % lang)
+        if not clodoo.searchL8(ctx, "ir.translation", [("lang", "=", lang)]):
+            if self.opt_args.verbose:
+                print('No term found for language %s: loading translation' % lang)
+            id = clodoo.createL8(ctx, 'base.update.translations', vals)
+            clodoo.executeL8(ctx, 'base.update.translations', 'act_update', [id])
+
+    def connect_db(self, database):
+        try:
+            uid, ctx = clodoo.oerp_set_env(
+                confn=self.opt_args.config,
+                db=database,
+                oe_version=self.opt_args.odoo_branch)
+        except BaseException:
+            print("No DB %s found" % self.opt_args.database)
+            ctx = None
+        return ctx
+
+    def translate_db(self):
+        # ir.translation contains Odoo translation terms
+        # @src: original (english) term
+        # @source: evaluated field with source code information
+        # @value: translated term
+        # @name: is environment name; value may be:
+        #   - type model: "model name,field name"
+        #   - type code: "source file name", format 'addons/MODULE_PATH'
+        #   - type selection: "MODULE_PATH,field name"
+        # @type: may be [code,constraint,model,selection,sql_constraint]
+        # @module: module which added term
+        # @state: may be [translated, to_translate]
+        # @res_id: id of term means:
+        #   - type model: record id of model in name
+        #   - type code: line number in source code (in name)
+        # Report translations are in ir.ui.view model
+        #
+        def write_term(term):
+            ctr_write = 0
+            term_tnl = term
+            if term.lang != self.opt_args.lang:
+                domain = [
+                    ("lang", "=", self.opt_args.lang),
+                    ("src", "=", term.src),
+                    ("type", "=", term.type),
+                    ("name", "=", term.name),
+                    ("module", "=", term.module),
+                ]
+                term_tnl = clodoo.browseL8(
+                    ctx, model_translation, clodoo.searchL8(
+                        ctx, model_translation, domain))
+                if len(term_tnl):
+                    term_tnl = term_tnl[0]
+            value = self.translate_item(term.src, term.value)
+            if not term_tnl:
+                if value != term.value:
+                    vals = {
+                        "lang": self.opt_args.lang,
+                        "value": value,
+                        "state": "translated",
+                        "res_id": term.res_id,
+                    }
+                    for name in ("src", "source", "type", "name", "module"):
+                        vals[name] = term[name]
+                    clodoo.createL8(ctx, model_translation, vals)
+                    ctr_write += 1
+            elif value != term_tnl.value:
+                try:
+                    clodoo.writeL8(ctx, model_translation, term.id,
+                                   {"value": value, "state": "translated"})
+                except BaseException as e:
+                    print("Error %s for term %s" % (e, term.src))
+                ctr_write += 1
+            return ctr_write
+
+        if not os.path.isfile(self.opt_args.config):
+            print("File %s not found!" % self.opt_args.config)
+            return 1
+        ctr_read = ctr_write = 0
+        for database in self.opt_args.database.split(","):
+            ctx = self.connect_db(database)
+            if ctx is None:
+                continue
+            ctx["lang"] = self.opt_args.lang
+            self.install_lang(self.opt_args.lang, ctx)
+            model_translation = 'ir.translation'
+            # model_field = 'ir.model.fields'
+            # last_term = ""
+            # for field in clodoo.browseL8(
+            #     ctx, model_field, clodoo.searchL8(
+            #         ctx, model_field, [], order="field_description")):
+            #     if field.field_description == last_term:
+            #         continue
+            #     last_term = field.field_description
+            #     if self.opt_args.verbose:
+            #         msg_burst('%s ...' % field.field_description)
+            #     domain = [
+            #         ('lang', 'in', ['en_US', self.opt_args.lang]),
+            #         ("src", "=ilike", field.field_description)
+            #     ]
+            #     for term in clodoo.browseL8(
+            #         ctx, model_translation, clodoo.searchL8(
+            #             ctx, model_translation, domain)):
+            #         ctr_read += 1
+            #         ctr_write += write_term(term)
+            for term in clodoo.browseL8(
+                ctx, model_translation, clodoo.searchL8(
+                    ctx, model_translation, [
+                        # ("type", "!=", "code"),
+                        ('lang', 'in', ['en_US', self.opt_args.lang])])):
+                if self.opt_args.verbose:
+                    msg_burst('%s ...' % term.src)
+                ctr_read += 1
+                ctr_write += write_term(term)
+        if self.opt_args.verbose:
+            print("%d records read, %d records written" % (ctr_read, ctr_write))
+        return 0
+
     def translate_module(self):
         module = self.opt_args.module_name
         target_path = os.path.abspath(self.opt_args.target_path)
         if module == "OCB" and os.path.isfile(os.path.join(target_path, "odoo-bin")):
             self.do_work_on_path(target_path, None, action="translate")
         elif module == os.path.basename(target_path):
             self.do_work_on_path(target_path, None, action="translate")
@@ -925,14 +1069,19 @@
         "--odoo-branch",
         dest="odoo_branch",
         default="12.0",
         help="Default Odoo version",
     )
     parser.add_argument("-c", "--config", help="Odoo configuration file")
     parser.add_argument(
+        "-d",
+        "--database",
+        help="Database to translate",
+    )
+    parser.add_argument(
         "-G",
         "--git-orgs",
         help="Git organizations, comma separated - " "May be: oca librerp or zero",
     )
     parser.add_argument("-l", "--lang", default="it_IT", help="Language")
     parser.add_argument("-m", "--module-name")
     parser.add_argument("-n", "--dry-run", action="store_true")
@@ -950,15 +1099,21 @@
     if odoo_tnxl.opt_args.test:
         odoo_tnxl.load_terms_for_test()
     elif odoo_tnxl.opt_args.file_xlsx or odoo_tnxl.opt_args.target_path:
         odoo_tnxl.build_dict()
     else:
         print("Invalid parameters: please set xlsx file or Odoo path")
         return 1
-    if odoo_tnxl.opt_args.module_name:
+    if (
+        odoo_tnxl.opt_args.database
+        and odoo_tnxl.opt_args.file_xlsx
+        and not odoo_tnxl.opt_args.rewrite_xlsx
+    ):
+        odoo_tnxl.translate_db()
+    elif odoo_tnxl.opt_args.module_name:
         odoo_tnxl.translate_module()
     if odoo_tnxl.opt_args.rewrite_xlsx:
         odoo_tnxl.write_xlsx()
     if odoo_tnxl.opt_args.test:
         print("")
         print("")
         print("Test starting ...")
```

### Comparing `wok_code-2.0.6/wok_code/scripts/odoo_translation_old.py` & `wok_code-2.0.7/wok_code/scripts/odoo_translation_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     from z0lib import z0lib
 try:
     from clodoo import clodoo
 except ImportError:
     import clodoo
 
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 MAX_RECS = 100
 PUNCT = [' ', '.', ',', '!', ':']
 TNL_DICT = {}
 TNL_ACTION = {}
 SYNTAX = {'string': re.compile('"([^"\\\n]|\\.|\\\n)*"')}
 VERSIONS = ('16.0', '15.0', '14.0', '13.0', '12.0', '11.0',
```

### Comparing `wok_code-2.0.6/wok_code/scripts/please.py` & `wok_code-2.0.7/wok_code/scripts/please.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 except ImportError:
     from .please_z0bug import PleaseZ0bug                                  # noqa: F401
 try:
     from please_apache import PleaseApache                                 # noqa: F401
 except ImportError:
     from .please_apache import PleaseApache                                # noqa: F401
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 KNOWN_ACTIONS = [
     "help",
     "chkconfig",
     "config",
     "docs",
     "duplicate",
```

### Comparing `wok_code-2.0.6/wok_code/scripts/please.sh` & `wok_code-2.0.7/wok_code/scripts/please.sh`

 * *Files 2% similar despite different names*

```diff
@@ -506,54 +506,54 @@
     run_traced "libreoffice $xfile"
   else
     echo "No file odoo_default_tnl.xlsx found!"
   fi
   return $STS_STS_SUCCESS
 }
 
-do_edit_translation_from_pofile() {
-  local xfile
-  local confn db module odoo_fver sts=$STS_FAILED opts pyv pofile
-  if [[ ! "$PRJNAME" == "Odoo" ]]; then
-    echo "No Odoo module"
-    return $STS_FAILED
-  fi
-  module="."
-  odoo_fver=$(build_odoo_param FULLVER '.')
-  pofile="$(build_odoo_param PKGPATH '.')/i18n/it.po"
-  module=$(build_odoo_param PKGNAME '.')
-  if [[ -z "$odoo_fver" || -z "$module" ]]; then
-    echo "Invalid Odoo environment!"
-    return $STS_FAILED
-  fi
-  odoo_ver=$(echo $odoo_fver | grep --color=never -Eo '[0-9]+' | head -n1)
-  if [[ ! -f "$pofile" ]]; then
-    echo "File $pofile not found!"
-    return $STS_FAILED
-  fi
-  pyv=$(python3 --version 2>&1 | grep --color=never -Eo "[0-9]+\.[0-9]+")
-  [[ -n "$pyv" ]] && pyver="-p $pyv"
-  pyver="-p 2.7" #debug
-  [[ ! -d $HOME/clodoo/venv ]] && \
-    run_traced "vem $pyver create $HOME/clodoo/venv" && \
-    run_traced "vem $HOME/clodoo/venv install xlrd" && \
-    run_traced "vem $HOME/clodoo/venv install Babel" && \
-    run_traced "vem $HOME/clodoo/venv install clodoo"
-  run_traced "pushd $HOME/clodoo >/dev/null"
-  [ $opt_verbose -ne 0 ] && opts="-v" || opts="-q"
-  [ $opt_dbg -ne 0 ] && opts="${opts}B"
-  run_traced "vem $HOME/clodoo/venv exec \"odoo_translation.py $opts -b$odoo_fver -m $module -R $pofile\""
-  sts=$?
-  run_traced "popd >/dev/null"
-  return $sts
-
-  [[ -f "$HOME_DEVEL/pypi/tools/odoo_default_tnl.xlsx" ]] && xfile="$HOME_DEVEL/pypi/tools/odoo_default_tnl.xlsx"
-  [[ -n "$xfile" ]] && run_traced "libreoffice $xfile" || echo "No file odoo_default_tnl.xlsx found!"
-  return $STS_STS_SUCCESS
-}
+#do_edit_translation_from_pofile() {
+#  local xfile
+#  local confn db module odoo_fver sts=$STS_FAILED opts pyv pofile
+#  if [[ ! "$PRJNAME" == "Odoo" ]]; then
+#    echo "No Odoo module"
+#    return $STS_FAILED
+#  fi
+#  module="."
+#  odoo_fver=$(build_odoo_param FULLVER '.')
+#  pofile="$(build_odoo_param PKGPATH '.')/i18n/it.po"
+#  module=$(build_odoo_param PKGNAME '.')
+#  if [[ -z "$odoo_fver" || -z "$module" ]]; then
+#    echo "Invalid Odoo environment!"
+#    return $STS_FAILED
+#  fi
+#  odoo_ver=$(echo $odoo_fver | grep --color=never -Eo '[0-9]+' | head -n1)
+#  if [[ ! -f "$pofile" ]]; then
+#    echo "File $pofile not found!"
+#    return $STS_FAILED
+#  fi
+#  pyv=$(python3 --version 2>&1 | grep --color=never -Eo "[0-9]+\.[0-9]+")
+#  [[ -n "$pyv" ]] && pyver="-p $pyv"
+#  pyver="-p 2.7" #debug
+#  [[ ! -d $HOME/clodoo/venv ]] && \
+#    run_traced "vem $pyver create $HOME/clodoo/venv" && \
+#    run_traced "vem $HOME/clodoo/venv install xlrd" && \
+#    run_traced "vem $HOME/clodoo/venv install Babel" && \
+#    run_traced "vem $HOME/clodoo/venv install clodoo"
+#  run_traced "pushd $HOME/clodoo >/dev/null"
+#  [ $opt_verbose -ne 0 ] && opts="-v" || opts="-q"
+#  [ $opt_dbg -ne 0 ] && opts="${opts}B"
+#  run_traced "vem $HOME/clodoo/venv exec \"odoo_translation.py $opts -b$odoo_fver -m $module -R $pofile\""
+#  sts=$?
+#  run_traced "popd >/dev/null"
+#  return $sts
+#
+#  [[ -f "$HOME_DEVEL/pypi/tools/odoo_default_tnl.xlsx" ]] && xfile="$HOME_DEVEL/pypi/tools/odoo_default_tnl.xlsx"
+#  [[ -n "$xfile" ]] && run_traced "libreoffice $xfile" || echo "No file odoo_default_tnl.xlsx found!"
+#  return $STS_STS_SUCCESS
+#}
 
 do_edit_untranslated() {
   local xfile
   [[ -f "$HOME/odoo_default_tnl.csv" ]] && run_traced "libreoffice $HOME/odoo_default_tnl.csv" || echo "No file odoo_default_tnl.csv found!"
   return $STS_STS_SUCCESS
 }
 
@@ -1041,15 +1041,15 @@
   set_executable
   if [ "$PRJNAME" == "Odoo" ]; then
     if [[ ! $LGITPATH =~ (14\.0|13\.0|12\.0|11\.0|10\.0|9\.0|8\.0|7\.0|6\.1) ]]; then
       echo "Missing or invalid target Odoo version"
       exit 1
     fi
     cur_ver=""
-    for ver in 14.0 13.0 12.0 11.0 10.0 9.0 8.0 7.0 6.1; do
+    for ver in 16.0 15.0 14.0 13.0 12.0 11.0 10.0 9.0 8.0 7.0 6.1; do
       if [[ $PWD =~ $HOME/$ver ]]; then
         cur_ver="$ver"
         break
       fi
     done
     if [ -z "$cur_ver" ]; then
       echo "Unrecognized Odoo version"
@@ -1106,21 +1106,17 @@
   if [[ -z "$db" ]]; then
     echo "No DB matched! use:"
     echo "$0 export -d DB"
     return $STS_FAILED
   fi
   stat=$(psql -U$u -Atc "select state from ir_module_module where name = '$module'" $db)
   [[ -z "$stat" || $stat == "uninstalled" ]] && echo "Module $module not installed in $db!" && exit $sts
-  # dbdt=$(psql -U$u -Atc "select write_date from ir_module_module where name='$module' and state='installed'" $db)
-  # [[ -n "$dbdt" ]] && dbdt=$(date -d "$dbdt" +"%s") || dbdt="999999999999999999"
-  # podt=$(stat -c "%Y" $pofile)
-  # ((dbdt < podt)) && run_traced "run_odoo_debug -b$odoo_fver -usm $module -d $db"
   dbdt=$(psql -U$u -Atc "select value from ir_config_parameter where key='database.create_date'" $db)
   podt=$(grep "PO-Revision-Date:" $pofile | grep -Eo "[0-9]{4}-[0-9]{2}-[0-9]{2}.[0-9]{2}:[0-9]{2}")
-  [[ $opt_force -ne 0 || $dbdt > $podt ]] && run_traced "run_odoo_debug -b$odoo_fver -em $module -d $db" || echo "PO file more recent of DB: use -f to force export or choise another DB"
+  [[ $opt_force -ne 0 || $dbdt > $podt ]] && run_traced "run_odoo_debug -b$odoo_fver -em $module -d $db" || echo "PO file more recent of DB: use -f to force export or choice another DB"
   sts=$?
   return $sts
 }
 
 do_import() {
   wlog "do_import '$1' '$2' '$3'"
   local db dbdt dummy DBs m module odoo_fver path pofile sts=$STS_FAILED u
@@ -1178,38 +1174,56 @@
     fi
   done
 }
 
 do_translate() {
   wlog "do_translate '$1' '$2' '$3'"
   local db dbdt dummy DBs m module odoo_fver path sts=$STS_FAILED u x
-  local confn opts pofile
+  local opt_multi confn opts pofile
   if [[ $PRJNAME != "Odoo" ]]; then
     echo "This action can be issued only on Odoo projects"
     return $sts
   fi
+  opt_multi=1
   odoo_fver=$(build_odoo_param FULLVER ".")
   m=$(build_odoo_param MAJVER ".")
   module=$(build_odoo_param PKGNAME ".")
   if [[ -z "$module" ]]; then
     echo "Invalid environment!"
     return $sts
   fi
   pofile="$PKGPATH/i18n/it.po"
   if [[ ! -f $pofile ]]; then
     echo "File $pofile not found!"
     return $sts
   fi
-  confn=$(readlink -f $HOME_DEVEL/../clodoo/confs)/${odoo_fver/./-}.conf
+  # confn=$(readlink -f $HOME_DEVEL/../clodoo/confs)/${odoo_fver/./-}.conf
+  confn=$(build_odoo_param CONFN ".")
   [[ ! -f $confn ]] && echo "Configuration file $confn not found!" && return $sts
-  echo "$0 translate -d DB"
-  do_export
   [[ $opt_verbose -ne 0 ]] && opts="-v" || opts="-q"
   [[ $opt_dbg -ne 0 ]] && opts="${opts}B"
-  run_traced "odoo_translation.py $opts -b$odoo_fver -m $module -c $confn -p $pofile"
+  db="$opt_db"
+  u=$(get_dbuser $m)
+  if [[ -z "$db" ]]; then
+    DBs=$(psql -U$u -Atl | awk -F'|' '{print $1}' | tr "\n" '|')
+    DBs="^(${DBs:0: -1})\$"
+    for x in "test_${module}" test_odoo_ tnl test demo; do
+      [[ ${x}_$m =~ $DBs ]] && db="${x}_$m" && break
+      [[ $x$m =~ $DBs ]] && db="$x$m" && break
+      [[ $x =~ $DBs ]] && db="$x" && break
+    done
+  fi
+  if [[ -z "$db" ]]; then
+    echo "No DB matched! use:"
+    echo "$0 translate -d DB"
+    return $STS_FAILED
+  fi
+  run_traced "odoo_translation.py $opts -b$odoo_fver -m $module -c $confn -d$db"
+  do_export
+  # run_traced "odoo_translation.py $opts -b$odoo_fver -m $module -c $confn -p $pofile"
   sts=$?
   return $sts
 }
 
 do_lint() {
     wlog "do_lint '$1' '$2' '$3'"
     local sts=$STS_FAILED s x
@@ -1366,15 +1380,15 @@
 }
 
 do_replica() {
   # do_replica(pkgname file)
   local cur_ver fn srcfn tp ver
   if [[ $PRJNAME == "Odoo" ]]; then
     cur_ver=""
-    for ver in 14.0 13.0 12.0 11.0 10.0 9.0 8.0 7.0 6.1; do
+    for ver in 16.0 15.0 14.0 13.0 12.0 11.0 10.0 9.0 8.0 7.0 6.1; do
       if [[ $PWD =~ $HOME/$ver ]]; then
         cur_ver="$ver"
         break
       fi
     done
     if [[ -z "$cur_ver" ]]; then
       echo "Unrecognized Odoo version"
@@ -1385,15 +1399,15 @@
     if [[ -d "$fn" ]]; then
       tp="d"
     elif [[ ! -f "$fn" ]]; then
       echo "File $fn not found"
       exit 1
     fi
     srcfn=$(readlink -f $fn)
-    for ver in 14.0 13.0 12.0 11.0 10.0 9.0 8.0 7.0 6.1; do
+    for ver in 16.0 15.0 14.0 13.0 12.0 11.0 10.0 9.0 8.0 7.0 6.1; do
       if [ "$ver" != "$cur_ver" ]; then
         tgtfn="${srcfn/$cur_ver/$ver}"
         if [ "$tp" == "f" ]; then
           tgtdir=$(dirname "$tgtfn")
           if [[ -d "$tgtdir" ]]; then
             echo "cp $srcfn $tgtfn"
             cp $srcfn $tgtfn
@@ -1636,15 +1650,15 @@
 OPTLONG=(help     debug   branch     config   odoo-conf from-date database force     keep     log       ""      dry-run     ""       ""      ""        quiet       ""    test      ""      version     verbose)
 OPTDEST=(opt_help opt_dbg opt_branch opt_conf opt_ocfn  opt_date  opt_db   opt_force opt_keep opt_log   opt_mis opt_dry_run opt_ids  opt_oca opt_dpath opt_verbose opt_r test_mode opt_uop opt_version opt_verbose)
 OPTACTI=("+"      "+"     "="        "="      "="       "="       "="      1         1        "="       1       1           "=>"     1       "="       0           1     1         1       "*"         "+")
 OPTDEFL=(1        0       ""         ""       ""        ""        ""       0         0        ""        0       0           ""       0       ""        0           0     0         0       ""          -1)
 OPTMETA=("help"   ""      "branch"   "file"   "file"    "diff"    "name"   ""       "keep"   "logfile" ""      "noop"       "prj_id" ""      "path"    "quiet"     "rxt" "test"    "uop"   "version"   "verbose")
 OPTHELP=("this help, type '$THIS help' for furthermore info"
   "debug mode"
-  "branch: must be 6.1 7.0 8.0 9.0 10.0 11.0 12.0 13.0 or 14.0"
+  "branch: must be 6.1 7.0 8.0 9.0 10.0 11.0 12.0 13.0 14.0 15.0 or 16.0"
   "configuration file (def .travis.conf)"
   "odoo configuration file"
   "date to search in log"
   "database name"
   "force copy (push) | build (publish/test) | set_exec (wep) | full (status)"
   "keep coverage statistics in annotate test/keep original repository | tests/ in publish"
   "log file name"
```

### Comparing `wok_code-2.0.6/wok_code/scripts/please_apache.py` & `wok_code-2.0.7/wok_code/scripts/please_apache.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 try:
     import ConfigParser
 except ImportError:
     import configparser as ConfigParser
 
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 APACHE_TEMPLATE = """##################################################################
 # Odoo service %(odoo_branch)s
 # Domain: <%(protocol)s://%(domain)s>
 #
 <VirtualHost *:%(apache_port)s>
     ServerAdmin %(email)s
```

### Comparing `wok_code-2.0.6/wok_code/scripts/please_z0bug.py` & `wok_code-2.0.7/wok_code/scripts/please_z0bug.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 
 class PleaseZ0bug(object):
 
     def __init__(self, please):
         self.please = please
```

### Comparing `wok_code-2.0.6/wok_code/scripts/run_odoo_debug.py` & `wok_code-2.0.7/wok_code/scripts/dist_pkg.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.6/wok_code/scripts/setup.info` & `wok_code-2.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     install_requires.append('translators')
     install_requires.append('twine')
 else:
     install_requires.append('twine==1.15.0')
 
 setup(
     name='wok_code',
-    version='2.0.6',
+    version='2.0.7',
     description='Python developers tools',
     long_description="""
 Various tools at your fingertips.
 
 The available tools are:
 
 * cvt_csv_2_rst.py: convert csv file into rst file
@@ -56,14 +56,15 @@
     packages=find_packages(exclude=['docs', 'examples', 'tests', 'egg-info', 'junk']),
     package_data={
         '': [
             'scripts/setup.info',
             'scripts/dist_pkg.sh',
             'scripts/please.sh',
             'scripts/config/*',
+            'scripts/run_odoo_debug.sh',
             './please.man',
             './cvt_script',
             './cvt_script.man',
             './topep8',
             './to_oca.2p8',
             './to_zero.2p8',
             './to_pep8.2p8',
@@ -74,14 +75,16 @@
     entry_points={
         'console_scripts': [
             'wok_code-info = wok_code.scripts.main:main',
             'cvt_csv_2_rst.py = wok_code.scripts.cvt_csv_2_rst:main',
             'cvt_csv_coa = wok_code.scripts.cvt_csv_coa:main',
             'deploy_odoo = wok_code.scripts.deploy_odoo:main',
             'dist_pkg = wok_code.scripts.dist_pkg:main',
+            'do_gitignore = wok_code.do_gitignore:main',
+            'do_git_checkout_new_branch = wok_code.do_git_checkout_new_branch:main',
             'do_migrate = wok_code.scripts.do_migrate:main',
             'do_odoo_site.py = wok_code.scripts.do_odoo_site:main',
             'gen_readme.py = wok_code.scripts.gen_readme:main',
             'lint_2_compare = wok_code.scripts.lint_2_compare:main',
             'makepo_it.py = wok_code.scripts.makepo_it:main',
             'odoo_dependencies.py = wok_code.scripts.odoo_dependencies:main',
             'odoo_translation.py = wok_code.scripts.odoo_translation:main',
```

### Comparing `wok_code-2.0.6/wok_code/scripts/to_pep8.py` & `wok_code-2.0.7/wok_code/scripts/to_pep8.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 except ImportError:
     import z0lib
 try:
     from python_plus.python_plus import _c, _u
 except ImportError:
     from python_plus import _c, _u
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 LICENSES = ('gpl', 'agpl', 'lgpl', 'opl', 'oee')
 METAS = ('0', '6.1', '7.0', '8.0', '9.0', '10.0', '11.0', '12.0', '13.0', '14.0')
 AUTHORS_TEMPLATE = """
 * LibrERP enterprise network <LibrERP-network>
 * SHS-AV s.r.l. <https://www.zeroincombenze.it>
 * Didotech s.r.l. <https://www.didotech.com>
```

### Comparing `wok_code-2.0.6/wok_code/scripts/wget_odoo_repositories.py` & `wok_code-2.0.7/wok_code/scripts/wget_odoo_repositories.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #     from z0lib.z0lib import z0lib
 # except ImportError:
 #     try:
 #         from z0lib import z0lib
 #     except ImportError:
 #         import z0lib
 
-__version__ = '2.0.6'
+__version__ = '2.0.7'
 
 ROOT_URL = 'https://api.github.com/repos/zeroincombenze/'
 USER_URL = 'https://api.github.com/users/'
 REPNAME_ACC_CLO = 'OCB'
 DEVEL_REPS = [
     'Odoo-samples',
     'VME',
```

### Comparing `wok_code-2.0.6/wok_code/ssh.py` & `wok_code-2.0.7/wok_code/ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import os
 import sys
 
-__version__ = '2.0.6'
+__version__ = '2.0.7'
 
 
 def get_remote_user():
     local_user = os.environ['USER']
     user = None
     default_user = None
     for key, item in DATA[host].items():
@@ -60,15 +60,15 @@
     return 'rsync -avz %s %s %s' % (param, source, dest)
 
 
 def get_cmd_scp(host, user, source, dest, recurse):
     param = DATA[host][user].get('param', "").replace("-p", "-P")
     if recurse:
         if param.startswith("-"):
-            param += "r"
+            param += " -r"
         else:
             param = "-r"
     passwd = DATA[host][user].get('passwd')
     if source.startswith("@"):
         source = "%s@%s:%s" % (user, host, source[1:])
     elif dest.startswith("@"):
         dest = "%s@%s:%s" % (user, host, dest[1:])
```

### Comparing `wok_code-2.0.6/wok_code/tests/test_filepo.py` & `wok_code-2.0.7/wok_code/tests/test_filepo.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.6/wok_code/tests/test_gen_readme.py` & `wok_code-2.0.7/wok_code/tests/test_gen_readme.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import os
 import sys
 
 from python_plus import _c
 from z0lib import z0lib
 from zerobug import z0test, z0testodoo
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 MODULE_ID = 'z0bug_odoo'
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 ODOO_VERSIONS = ('7.0', '10.0', '12.0')
 
 DESCR_FN = r"""Lorem ipsum
```

### Comparing `wok_code-2.0.6/wok_code/tests/test_license_mgnt.py` & `wok_code-2.0.7/wok_code/tests/test_license_mgnt.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 import os
 import sys
 
 from wok_code.scripts import license_mgnt
 from zerobug import z0test, z0testodoo
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 MODULE_ID = 'devel_tool'
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 
 
 def version():
```

### Comparing `wok_code-2.0.6/wok_code/tests/test_please.py` & `wok_code-2.0.7/wok_code/tests/test_please.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 import sys
 
 from z0lib import z0lib
 from zerobug import z0test
 
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 MODULE_ID = 'wok_code'
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 
 
 def version():
```

### Comparing `wok_code-2.0.6/wok_code/to_oca.2p8` & `wok_code-2.0.7/wok_code/to_oca.2p8`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.6/wok_code/to_pep8.2p8` & `wok_code-2.0.7/wok_code/to_pep8.2p8`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.6/wok_code/to_zero.2p8` & `wok_code-2.0.7/wok_code/to_zero.2p8`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.6/wok_code/topep8` & `wok_code-2.0.7/wok_code/topep8`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.6
+__version__=2.0.7
 
 # [[ -f $TDIR/../../python_plus/list_requirements.py ]] && LISTREQ=$TDIR/../../python_plus/list_requirements.py || LISTREQ=list_requirements.py
 YAML_TMPL=~/dev/pypi/z0bug_odd/z0bug_odoo/sample_files/.travis.yml
 NO_APT_GET="(build-essential|curl|git|gradle|gzip|java|lessc|less-plugin-clean-css|nodejs|npm|openssl|python-setuptools|python-simplejson|PhantomJS|rvm|ruby|sass|scss|tesseract|wget|wkhtmltopdf|zip)"
 
 expand_macro() {
   local t p v lne lne1
```

### Comparing `wok_code-2.0.6/wok_code.egg-info/PKG-INFO` & `wok_code-2.0.7/wok_code.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: wok-code
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python developers tools
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
 Project-URL: Source, https://github.com/zeroincombenze/tools
+Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
+Description: 
+        Various tools at your fingertips.
+        
+        The available tools are:
+        
+        * cvt_csv_2_rst.py: convert csv file into rst file
+        * cvt_csv_2_xml.py: convert csv file into xml file
+        * cvt_script: parse bash script and convert to meet company standard
+        * gen_readme.py: generate documentation files, mainly README.rst
+        * odoo_dependency.py: show odoo dependencies and/or Odoo module tree
+        * odoo_translation.py: manage Odoo translation
+        * pep8: parse source .py file to meet pep8 and convert across Odoo versions
+        * please: developer shell
+        * wget_odoo_repositories.py: get repository names from github.com
+        
 Keywords: linux travis development
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Operating System :: OS Independent
-
-
-Various tools at your fingertips.
-
-The available tools are:
-
-* cvt_csv_2_rst.py: convert csv file into rst file
-* cvt_csv_2_xml.py: convert csv file into xml file
-* cvt_script: parse bash script and convert to meet company standard
-* gen_readme.py: generate documentation files, mainly README.rst
-* odoo_dependency.py: show odoo dependencies and/or Odoo module tree
-* odoo_translation.py: manage Odoo translation
-* pep8: parse source .py file to meet pep8 and convert across Odoo versions
-* please: developer shell
-* wget_odoo_repositories.py: get repository names from github.com
-
-
```

### Comparing `wok_code-2.0.6/wok_code.egg-info/SOURCES.txt` & `wok_code-2.0.7/wok_code.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 wok_code/scripts/odoo_translation.py
 wok_code/scripts/odoo_translation_old.py
 wok_code/scripts/please.py
 wok_code/scripts/please.sh
 wok_code/scripts/please_apache.py
 wok_code/scripts/please_z0bug.py
 wok_code/scripts/run_odoo_debug.py
+wok_code/scripts/run_odoo_debug.sh
 wok_code/scripts/setup.info
 wok_code/scripts/to_pep8.py
 wok_code/scripts/wget_odoo_repositories.py
 wok_code/scripts/config/globals.yml
 wok_code/scripts/config/globals_xml.yml
 wok_code/scripts/config/to_new_api.yml
 wok_code/scripts/config/to_odoo_py2.yml
```

### Comparing `wok_code-2.0.6/wok_code.egg-info/entry_points.txt` & `wok_code-2.0.7/wok_code.egg-info/entry_points.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [console_scripts]
 cvt_csv_2_rst.py = wok_code.scripts.cvt_csv_2_rst:main
 cvt_csv_coa = wok_code.scripts.cvt_csv_coa:main
 deploy_odoo = wok_code.scripts.deploy_odoo:main
 dist_pkg = wok_code.scripts.dist_pkg:main
+do_git_checkout_new_branch = wok_code.do_git_checkout_new_branch:main
+do_gitignore = wok_code.do_gitignore:main
 do_migrate = wok_code.scripts.do_migrate:main
 do_odoo_site.py = wok_code.scripts.do_odoo_site:main
 gen_readme.py = wok_code.scripts.gen_readme:main
 lint_2_compare = wok_code.scripts.lint_2_compare:main
 makepo_it.py = wok_code.scripts.makepo_it:main
 odoo_dependencies.py = wok_code.scripts.odoo_dependencies:main
 odoo_translation.py = wok_code.scripts.odoo_translation:main
```

