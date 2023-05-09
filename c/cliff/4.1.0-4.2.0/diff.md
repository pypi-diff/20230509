# Comparing `tmp/cliff-4.1.0.tar.gz` & `tmp/cliff-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliff-4.1.0.tar", last modified: Fri Nov 18 14:37:36 2022, max compression
+gzip compressed data, was "cliff-4.2.0.tar", last modified: Mon Feb 13 16:10:51 2023, max compression
```

## Comparing `cliff-4.1.0.tar` & `cliff-4.2.0.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:36.373151 cliff-4.1.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2022-11-18 14:37:09.000000 cliff-4.1.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2022-11-18 14:37:09.000000 cliff-4.1.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4343 2022-11-18 14:37:36.000000 cliff-4.1.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2022-11-18 14:37:09.000000 cliff-4.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24750 2022-11-18 14:37:36.000000 cliff-4.1.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2022-11-18 14:37:09.000000 cliff-4.1.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1935 2022-11-18 14:37:36.373151 cliff-4.1.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2022-11-18 14:37:09.000000 cliff-4.1.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2022-11-18 14:37:09.000000 cliff-4.1.0/bandit.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:36.361147 cliff-4.1.0/cliff/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3811 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/_argparse.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16720 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1613 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/columns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7452 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/command.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5860 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/commandmanager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6529 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/complete.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4834 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/display.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:36.361147 cliff-4.1.0/cliff/formatters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/formatters/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2604 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/formatters/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1807 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/formatters/commaseparated.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1863 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/formatters/json_format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2377 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/formatters/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7418 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/formatters/table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1400 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/formatters/value.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1757 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/formatters/yaml_format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5683 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/help.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1953 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/hooks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8444 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/interactive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4653 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/lister.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1888 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/show.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13016 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/sphinxext.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:36.365149 cliff-4.1.0/cliff/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2011 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test__argparse.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19882 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1872 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_columns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7837 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_command.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13898 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_command_hooks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10890 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_commandmanager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6880 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_complete.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2967 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_formatters_csv.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3980 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_formatters_json.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3369 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_formatters_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24444 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_formatters_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2220 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_formatters_value.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_formatters_yaml.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6893 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_help.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3537 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_interactive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6699 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_lister.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2523 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_show.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8454 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_sphinxext.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1379 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1391 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/tests/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4784 2022-11-18 14:37:09.000000 cliff-4.1.0/cliff/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:36.361147 cliff-4.1.0/cliff.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1935 2022-11-18 14:37:36.000000 cliff-4.1.0/cliff.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2627 2022-11-18 14:37:36.000000 cliff-4.1.0/cliff.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-11-18 14:37:36.000000 cliff-4.1.0/cliff.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2022-11-18 14:37:36.000000 cliff-4.1.0/cliff.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-11-18 14:37:36.000000 cliff-4.1.0/cliff.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-11-18 14:37:36.000000 cliff-4.1.0/cliff.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2022-11-18 14:37:36.000000 cliff-4.1.0/cliff.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2022-11-18 14:37:36.000000 cliff-4.1.0/cliff.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:36.365149 cliff-4.1.0/demoapp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      960 2022-11-18 14:37:09.000000 cliff-4.1.0/demoapp/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:36.369150 cliff-4.1.0/demoapp/cliffdemo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:09.000000 cliff-4.1.0/demoapp/cliffdemo/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2022-11-18 14:37:09.000000 cliff-4.1.0/demoapp/cliffdemo/__main__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2022-11-18 14:37:09.000000 cliff-4.1.0/demoapp/cliffdemo/encoding.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1510 2022-11-18 14:37:09.000000 cliff-4.1.0/demoapp/cliffdemo/hook.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2022-11-18 14:37:09.000000 cliff-4.1.0/demoapp/cliffdemo/list.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2022-11-18 14:37:09.000000 cliff-4.1.0/demoapp/cliffdemo/main.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2022-11-18 14:37:09.000000 cliff-4.1.0/demoapp/cliffdemo/show.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2022-11-18 14:37:09.000000 cliff-4.1.0/demoapp/cliffdemo/simple.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2022-11-18 14:37:09.000000 cliff-4.1.0/demoapp/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:36.369150 cliff-4.1.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2022-11-18 14:37:09.000000 cliff-4.1.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:36.369150 cliff-4.1.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8458 2022-11-18 14:37:09.000000 cliff-4.1.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:36.369150 cliff-4.1.0/doc/source/contributors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1612 2022-11-18 14:37:09.000000 cliff-4.1.0/doc/source/contributors/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2022-11-18 14:37:09.000000 cliff-4.1.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:36.369150 cliff-4.1.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2022-11-18 14:37:09.000000 cliff-4.1.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:36.369150 cliff-4.1.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2022-11-18 14:37:09.000000 cliff-4.1.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:36.369150 cliff-4.1.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2022-11-18 14:37:09.000000 cliff-4.1.0/doc/source/user/complete.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9043 2022-11-18 14:37:09.000000 cliff-4.1.0/doc/source/user/demoapp.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2022-11-18 14:37:09.000000 cliff-4.1.0/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2022-11-18 14:37:09.000000 cliff-4.1.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2679 2022-11-18 14:37:09.000000 cliff-4.1.0/doc/source/user/interactive_mode.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2782 2022-11-18 14:37:09.000000 cliff-4.1.0/doc/source/user/introduction.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3632 2022-11-18 14:37:09.000000 cliff-4.1.0/doc/source/user/list_commands.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3521 2022-11-18 14:37:09.000000 cliff-4.1.0/doc/source/user/show_commands.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7114 2022-11-18 14:37:09.000000 cliff-4.1.0/doc/source/user/sphinxext.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:36.373151 cliff-4.1.0/integration-tests/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      477 2022-11-18 14:37:09.000000 cliff-4.1.0/integration-tests/neutronclient-tip.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      599 2022-11-18 14:37:09.000000 cliff-4.1.0/integration-tests/openstackclient-tip.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:36.353145 cliff-4.1.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-18 14:37:36.373151 cliff-4.1.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2022-11-18 14:37:09.000000 cliff-4.1.0/releasenotes/notes/add-Lister-sort-direction-5f34dba3c9743572.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2022-11-18 14:37:09.000000 cliff-4.1.0/releasenotes/notes/command-group-8c00f260340a130c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2022-11-18 14:37:09.000000 cliff-4.1.0/releasenotes/notes/comparable-FormattableColumn-31c0030ced70b7fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2022-11-18 14:37:09.000000 cliff-4.1.0/releasenotes/notes/drop-python27-support-b16c9e5a9e2000ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2022-11-18 14:37:09.000000 cliff-4.1.0/releasenotes/notes/handle-none-values-when-sorting-de40e36c66ad95ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2022-11-18 14:37:09.000000 cliff-4.1.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1771 2022-11-18 14:37:36.373151 cliff-4.1.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2022-11-18 14:37:09.000000 cliff-4.1.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2022-11-18 14:37:09.000000 cliff-4.1.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1518 2022-11-18 14:37:09.000000 cliff-4.1.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:51.396054 cliff-4.2.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2023-02-13 16:10:11.000000 cliff-4.2.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2023-02-13 16:10:11.000000 cliff-4.2.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4343 2023-02-13 16:10:51.000000 cliff-4.2.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2023-02-13 16:10:11.000000 cliff-4.2.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24814 2023-02-13 16:10:51.000000 cliff-4.2.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2023-02-13 16:10:11.000000 cliff-4.2.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1935 2023-02-13 16:10:51.400054 cliff-4.2.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2023-02-13 16:10:11.000000 cliff-4.2.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2023-02-13 16:10:11.000000 cliff-4.2.0/bandit.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:51.384055 cliff-4.2.0/cliff/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3811 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/_argparse.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16720 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1613 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/columns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7452 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/command.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5860 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/commandmanager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6529 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/complete.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4834 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/display.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:51.388054 cliff-4.2.0/cliff/formatters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/formatters/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2604 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/formatters/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1807 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/formatters/commaseparated.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1863 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/formatters/json_format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2377 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/formatters/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7418 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/formatters/table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1400 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/formatters/value.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1757 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/formatters/yaml_format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5695 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/help.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1953 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/hooks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8444 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/interactive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4653 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/lister.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1888 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/show.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13016 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/sphinxext.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:51.392054 cliff-4.2.0/cliff/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2011 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test__argparse.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19882 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1872 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_columns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7837 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_command.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13898 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_command_hooks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10890 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_commandmanager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6880 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_complete.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2967 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_formatters_csv.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3980 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_formatters_json.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3369 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_formatters_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24444 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_formatters_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2220 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_formatters_value.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_formatters_yaml.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6891 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_help.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3537 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_interactive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6699 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_lister.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2523 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_show.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8454 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_sphinxext.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1379 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1391 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/tests/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4784 2023-02-13 16:10:11.000000 cliff-4.2.0/cliff/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:51.384055 cliff-4.2.0/cliff.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1935 2023-02-13 16:10:51.000000 cliff-4.2.0/cliff.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2699 2023-02-13 16:10:51.000000 cliff-4.2.0/cliff.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-13 16:10:51.000000 cliff-4.2.0/cliff.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2023-02-13 16:10:51.000000 cliff-4.2.0/cliff.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-13 16:10:51.000000 cliff-4.2.0/cliff.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-13 16:10:51.000000 cliff-4.2.0/cliff.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-02-13 16:10:51.000000 cliff-4.2.0/cliff.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2023-02-13 16:10:51.000000 cliff-4.2.0/cliff.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:51.392054 cliff-4.2.0/demoapp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      960 2023-02-13 16:10:11.000000 cliff-4.2.0/demoapp/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:51.392054 cliff-4.2.0/demoapp/cliffdemo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:11.000000 cliff-4.2.0/demoapp/cliffdemo/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-02-13 16:10:11.000000 cliff-4.2.0/demoapp/cliffdemo/__main__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2023-02-13 16:10:11.000000 cliff-4.2.0/demoapp/cliffdemo/encoding.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1510 2023-02-13 16:10:11.000000 cliff-4.2.0/demoapp/cliffdemo/hook.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-02-13 16:10:11.000000 cliff-4.2.0/demoapp/cliffdemo/list.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2023-02-13 16:10:11.000000 cliff-4.2.0/demoapp/cliffdemo/main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2023-02-13 16:10:11.000000 cliff-4.2.0/demoapp/cliffdemo/show.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2023-02-13 16:10:11.000000 cliff-4.2.0/demoapp/cliffdemo/simple.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2023-02-13 16:10:11.000000 cliff-4.2.0/demoapp/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:51.392054 cliff-4.2.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2023-02-13 16:10:11.000000 cliff-4.2.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:51.396054 cliff-4.2.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8458 2023-02-13 16:10:11.000000 cliff-4.2.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:51.396054 cliff-4.2.0/doc/source/contributors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1612 2023-02-13 16:10:11.000000 cliff-4.2.0/doc/source/contributors/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2023-02-13 16:10:11.000000 cliff-4.2.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:51.396054 cliff-4.2.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2023-02-13 16:10:11.000000 cliff-4.2.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:51.396054 cliff-4.2.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2023-02-13 16:10:11.000000 cliff-4.2.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:51.396054 cliff-4.2.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2023-02-13 16:10:11.000000 cliff-4.2.0/doc/source/user/complete.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9043 2023-02-13 16:10:11.000000 cliff-4.2.0/doc/source/user/demoapp.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-02-13 16:10:11.000000 cliff-4.2.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-02-13 16:10:11.000000 cliff-4.2.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2679 2023-02-13 16:10:11.000000 cliff-4.2.0/doc/source/user/interactive_mode.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2782 2023-02-13 16:10:11.000000 cliff-4.2.0/doc/source/user/introduction.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3632 2023-02-13 16:10:11.000000 cliff-4.2.0/doc/source/user/list_commands.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3521 2023-02-13 16:10:11.000000 cliff-4.2.0/doc/source/user/show_commands.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7114 2023-02-13 16:10:11.000000 cliff-4.2.0/doc/source/user/sphinxext.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:51.396054 cliff-4.2.0/integration-tests/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      477 2023-02-13 16:10:11.000000 cliff-4.2.0/integration-tests/neutronclient-tip.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      599 2023-02-13 16:10:11.000000 cliff-4.2.0/integration-tests/openstackclient-tip.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:51.380055 cliff-4.2.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:10:51.396054 cliff-4.2.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2023-02-13 16:10:11.000000 cliff-4.2.0/releasenotes/notes/add-Lister-sort-direction-5f34dba3c9743572.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-02-13 16:10:11.000000 cliff-4.2.0/releasenotes/notes/command-group-8c00f260340a130c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2023-02-13 16:10:11.000000 cliff-4.2.0/releasenotes/notes/comparable-FormattableColumn-31c0030ced70b7fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-02-13 16:10:11.000000 cliff-4.2.0/releasenotes/notes/drop-python27-support-b16c9e5a9e2000ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2023-02-13 16:10:11.000000 cliff-4.2.0/releasenotes/notes/handle-none-values-when-sorting-de40e36c66ad95ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-02-13 16:10:11.000000 cliff-4.2.0/releasenotes/notes/strip-period-from-help-strings-be368e5cf5bd5269.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-02-13 16:10:11.000000 cliff-4.2.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1771 2023-02-13 16:10:51.400054 cliff-4.2.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2023-02-13 16:10:11.000000 cliff-4.2.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-02-13 16:10:11.000000 cliff-4.2.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1518 2023-02-13 16:10:11.000000 cliff-4.2.0/tox.ini
```

### Comparing `cliff-4.1.0/.zuul.yaml` & `cliff-4.2.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/AUTHORS` & `cliff-4.2.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/ChangeLog` & `cliff-4.2.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+4.2.0
+-----
+
+* Strip trailing periods when getting description
+
 4.1.0
 -----
 
 * columns: Useful \_\_str\_\_, \_\_repr\_\_ implementation
 * Add Python3 antelope unit tests
 
 4.0.0
```

### Comparing `cliff-4.1.0/LICENSE` & `cliff-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/PKG-INFO` & `cliff-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cliff
-Version: 4.1.0
+Version: 4.2.0
 Summary: Command Line Interface Formulation Framework
 Home-page: https://docs.openstack.org/cliff/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `cliff-4.1.0/README.rst` & `cliff-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/_argparse.py` & `cliff-4.2.0/cliff/_argparse.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/app.py` & `cliff-4.2.0/cliff/app.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/columns.py` & `cliff-4.2.0/cliff/columns.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/command.py` & `cliff-4.2.0/cliff/command.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/commandmanager.py` & `cliff-4.2.0/cliff/commandmanager.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/complete.py` & `cliff-4.2.0/cliff/complete.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/display.py` & `cliff-4.2.0/cliff/display.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/formatters/base.py` & `cliff-4.2.0/cliff/formatters/base.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/formatters/commaseparated.py` & `cliff-4.2.0/cliff/formatters/commaseparated.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/formatters/json_format.py` & `cliff-4.2.0/cliff/formatters/json_format.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/formatters/shell.py` & `cliff-4.2.0/cliff/formatters/shell.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/formatters/table.py` & `cliff-4.2.0/cliff/formatters/table.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/formatters/value.py` & `cliff-4.2.0/cliff/formatters/value.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/formatters/yaml_format.py` & `cliff-4.2.0/cliff/formatters/yaml_format.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/help.py` & `cliff-4.2.0/cliff/help.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                     if cmd.deprecated:
                         continue
                 except Exception as err:
                     out.write('Could not instantiate %r: %s\n' % (ep, err))
                     if namespace.debug:
                         traceback.print_exc(file=out)
                     continue
-                one_liner = cmd.get_description().split('\n')[0]
+                one_liner = cmd.get_description().split('\n')[0].rstrip('.')
                 dist_name = dist_for_obj(factory)
                 if dist_name and dist_name != app_dist:
                     dist_info = ' (' + dist_name + ')'
                     if color:
                         dist_info = '\033[90m%s\033[39m' % dist_info
                 else:
                     dist_info = ''
```

### Comparing `cliff-4.1.0/cliff/hooks.py` & `cliff-4.2.0/cliff/hooks.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/interactive.py` & `cliff-4.2.0/cliff/interactive.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/lister.py` & `cliff-4.2.0/cliff/lister.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/show.py` & `cliff-4.2.0/cliff/show.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/sphinxext.py` & `cliff-4.2.0/cliff/sphinxext.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/base.py` & `cliff-4.2.0/cliff/tests/base.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test__argparse.py` & `cliff-4.2.0/cliff/tests/test__argparse.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_app.py` & `cliff-4.2.0/cliff/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_columns.py` & `cliff-4.2.0/cliff/tests/test_columns.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_command.py` & `cliff-4.2.0/cliff/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_command_hooks.py` & `cliff-4.2.0/cliff/tests/test_command_hooks.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_commandmanager.py` & `cliff-4.2.0/cliff/tests/test_commandmanager.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_complete.py` & `cliff-4.2.0/cliff/tests/test_complete.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_formatters_csv.py` & `cliff-4.2.0/cliff/tests/test_formatters_csv.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_formatters_json.py` & `cliff-4.2.0/cliff/tests/test_formatters_json.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_formatters_shell.py` & `cliff-4.2.0/cliff/tests/test_formatters_shell.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_formatters_table.py` & `cliff-4.2.0/cliff/tests/test_formatters_table.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_formatters_value.py` & `cliff-4.2.0/cliff/tests/test_formatters_value.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_formatters_yaml.py` & `cliff-4.2.0/cliff/tests/test_formatters_yaml.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_help.py` & `cliff-4.2.0/cliff/tests/test_help.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,16 +99,16 @@
         except help.HelpExit:
             pass
         help_text = stdout.getvalue()
         basecommand = os.path.split(sys.argv[0])[1]
         self.assertIn('usage: %s [--version]' % basecommand, help_text)
         self.assertRegex(help_text, 'option(s|al arguments):\n  --version')
         expected = (
-            '  one            Test command.\n'
-            '  three word command  Test command.\n'
+            '  one            Test command\n'
+            '  three word command  Test command\n'
         )
         self.assertIn(expected, help_text)
 
     def test_list_deprecated_commands(self):
         # FIXME(dhellmann): Are commands tied too closely to the app? Or
         # do commands know too much about apps by using them to get to the
         # command manager?
```

### Comparing `cliff-4.1.0/cliff/tests/test_interactive.py` & `cliff-4.2.0/cliff/tests/test_interactive.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_lister.py` & `cliff-4.2.0/cliff/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_show.py` & `cliff-4.2.0/cliff/tests/test_show.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_sphinxext.py` & `cliff-4.2.0/cliff/tests/test_sphinxext.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/test_utils.py` & `cliff-4.2.0/cliff/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/tests/utils.py` & `cliff-4.2.0/cliff/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff/utils.py` & `cliff-4.2.0/cliff/utils.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/cliff.egg-info/PKG-INFO` & `cliff-4.2.0/cliff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cliff
-Version: 4.1.0
+Version: 4.2.0
 Summary: Command Line Interface Formulation Framework
 Home-page: https://docs.openstack.org/cliff/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `cliff-4.1.0/cliff.egg-info/SOURCES.txt` & `cliff-4.2.0/cliff.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -91,8 +91,9 @@
 doc/source/user/sphinxext.rst
 integration-tests/neutronclient-tip.sh
 integration-tests/openstackclient-tip.sh
 releasenotes/notes/add-Lister-sort-direction-5f34dba3c9743572.yaml
 releasenotes/notes/command-group-8c00f260340a130c.yaml
 releasenotes/notes/comparable-FormattableColumn-31c0030ced70b7fb.yaml
 releasenotes/notes/drop-python27-support-b16c9e5a9e2000ef.yaml
-releasenotes/notes/handle-none-values-when-sorting-de40e36c66ad95ca.yaml
+releasenotes/notes/handle-none-values-when-sorting-de40e36c66ad95ca.yaml
+releasenotes/notes/strip-period-from-help-strings-be368e5cf5bd5269.yaml
```

### Comparing `cliff-4.1.0/cliff.egg-info/entry_points.txt` & `cliff-4.2.0/cliff.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/demoapp/README.rst` & `cliff-4.2.0/demoapp/README.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/demoapp/cliffdemo/hook.py` & `cliff-4.2.0/demoapp/cliffdemo/hook.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/demoapp/cliffdemo/main.py` & `cliff-4.2.0/demoapp/cliffdemo/main.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/demoapp/cliffdemo/show.py` & `cliff-4.2.0/demoapp/cliffdemo/show.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/demoapp/cliffdemo/simple.py` & `cliff-4.2.0/demoapp/cliffdemo/simple.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/demoapp/setup.py` & `cliff-4.2.0/demoapp/setup.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/doc/source/conf.py` & `cliff-4.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/doc/source/contributors/index.rst` & `cliff-4.2.0/doc/source/contributors/index.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/doc/source/install/index.rst` & `cliff-4.2.0/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/doc/source/reference/index.rst` & `cliff-4.2.0/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/doc/source/user/complete.rst` & `cliff-4.2.0/doc/source/user/complete.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/doc/source/user/demoapp.rst` & `cliff-4.2.0/doc/source/user/demoapp.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/doc/source/user/interactive_mode.rst` & `cliff-4.2.0/doc/source/user/interactive_mode.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/doc/source/user/introduction.rst` & `cliff-4.2.0/doc/source/user/introduction.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/doc/source/user/list_commands.rst` & `cliff-4.2.0/doc/source/user/list_commands.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/doc/source/user/show_commands.rst` & `cliff-4.2.0/doc/source/user/show_commands.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/doc/source/user/sphinxext.rst` & `cliff-4.2.0/doc/source/user/sphinxext.rst`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/integration-tests/openstackclient-tip.sh` & `cliff-4.2.0/integration-tests/openstackclient-tip.sh`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/releasenotes/notes/add-Lister-sort-direction-5f34dba3c9743572.yaml` & `cliff-4.2.0/releasenotes/notes/add-Lister-sort-direction-5f34dba3c9743572.yaml`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/setup.cfg` & `cliff-4.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/setup.py` & `cliff-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `cliff-4.1.0/tox.ini` & `cliff-4.2.0/tox.ini`

 * *Files identical despite different names*

