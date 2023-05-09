# Comparing `tmp/osc-lib-2.6.2.tar.gz` & `tmp/osc-lib-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc-lib-2.6.2.tar", last modified: Wed Aug 24 13:23:41 2022, max compression
+gzip compressed data, was "osc-lib-2.7.0.tar", last modified: Mon Feb 13 16:18:23 2023, max compression
```

## Comparing `osc-lib-2.6.2.tar` & `osc-lib-2.7.0.tar`

### file list

```diff
@@ -1,139 +1,140 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.457710 osc-lib-2.6.2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-08-24 13:23:01.000000 osc-lib-2.6.2/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2022-08-24 13:23:01.000000 osc-lib-2.6.2/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2022-08-24 13:23:01.000000 osc-lib-2.6.2/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2022-08-24 13:23:01.000000 osc-lib-2.6.2/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6411 2022-08-24 13:23:41.000000 osc-lib-2.6.2/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35944 2022-08-24 13:23:41.000000 osc-lib-2.6.2/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3095 2022-08-24 13:23:01.000000 osc-lib-2.6.2/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-08-24 13:23:01.000000 osc-lib-2.6.2/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3776 2022-08-24 13:23:41.457710 osc-lib-2.6.2/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2356 2022-08-24 13:23:01.000000 osc-lib-2.6.2/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.441708 osc-lib-2.6.2/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4843 2022-08-24 13:23:01.000000 osc-lib-2.6.2/doc/Makefile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.441708 osc-lib-2.6.2/doc/ext/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:01.000000 osc-lib-2.6.2/doc/ext/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1437 2022-08-24 13:23:01.000000 osc-lib-2.6.2/doc/ext/apidoc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2022-08-24 13:23:01.000000 osc-lib-2.6.2/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.441708 osc-lib-2.6.2/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7882 2022-08-24 13:23:01.000000 osc-lib-2.6.2/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.441708 osc-lib-2.6.2/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      980 2022-08-24 13:23:01.000000 osc-lib-2.6.2/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2022-08-24 13:23:01.000000 osc-lib-2.6.2/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.441708 osc-lib-2.6.2/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2022-08-24 13:23:01.000000 osc-lib-2.6.2/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.441708 osc-lib-2.6.2/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2022-08-24 13:23:01.000000 osc-lib-2.6.2/doc/source/user/change_log.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2022-08-24 13:23:01.000000 osc-lib-2.6.2/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3865 2022-08-24 13:23:01.000000 osc-lib-2.6.2/doc/source/user/transition.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2022-08-24 13:23:01.000000 osc-lib-2.6.2/lower-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.441708 osc-lib-2.6.2/osc_lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.445709 osc-lib-2.6.2/osc_lib/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12900 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/api/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8202 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/api/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3129 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/api/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.445709 osc-lib-2.6.2/osc_lib/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/cli/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9379 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/cli/client_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1584 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/cli/format_columns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2803 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/cli/identity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10430 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/cli/parseractions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9806 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/clientmanager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.445709 osc-lib-2.6.2/osc_lib/command/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/command/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/command/command.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/command/commandmanager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1139 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/command/timing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3394 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7110 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/logs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19050 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.449709 osc-lib-2.6.2/osc_lib/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.449709 osc-lib-2.6.2/osc_lib/tests/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/api/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16739 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/api/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3383 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/api/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.449709 osc-lib-2.6.2/osc_lib/tests/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/cli/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8483 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/cli/test_client_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2941 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/cli/test_format_columns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3368 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/cli/test_identity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14128 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/cli/test_parseractions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.449709 osc-lib-2.6.2/osc_lib/tests/command/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/command/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1684 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/command/test_command.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2962 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/command/test_timing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5822 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15321 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/test_clientmanager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8697 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/test_logs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20246 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/test_shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.449709 osc-lib-2.6.2/osc_lib/tests/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14444 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2428 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/utils/test_columns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11622 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/utils/test_tags.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36608 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/tests/utils/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.449709 osc-lib-2.6.2/osc_lib/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27403 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3844 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/utils/columns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7531 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/utils/tags.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2022-08-24 13:23:01.000000 osc-lib-2.6.2/osc_lib/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.445709 osc-lib-2.6.2/osc_lib.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3776 2022-08-24 13:23:41.000000 osc-lib-2.6.2/osc_lib.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3661 2022-08-24 13:23:41.000000 osc-lib-2.6.2/osc_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-08-24 13:23:41.000000 osc-lib-2.6.2/osc_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-08-24 13:23:41.000000 osc-lib-2.6.2/osc_lib.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-08-24 13:23:41.000000 osc-lib-2.6.2/osc_lib.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2022-08-24 13:23:41.000000 osc-lib-2.6.2/osc_lib.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2022-08-24 13:23:41.000000 osc-lib-2.6.2/osc_lib.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.437708 osc-lib-2.6.2/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.453710 osc-lib-2.6.2/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2707 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/1.0-summary-47dcce446d6a512b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/add-KeyValueAppendAction-class-f830e71152d6b91e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/add-MultiKeyValueCommaAction-class-01dd254a287d70d2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/add_sdk_utils-d0c338eba682f2c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/arg-precedence-1ba9fd6929650830.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/auth-type-none-d96760912605f822.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/bug-1558690-1528b637f2c0a449.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/bug-1630822-mask-password-on-debug-20dcdf1c54e84fa1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/bug-2004898-686577a07e791051.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/bug-2006480-436489d39643e76c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/direct-openstacksdk-535a179f3c645cc0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/drop-py2-support-60c93244107d5778.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/find-project-203bf867619c557e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/keystone-to-keystone-9b2e55b051775322.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/none-auth-cli-48ab0e48d4852941.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/os-profile-as-environment-variable-a5e232e9ca7c5171.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/remove-babel-50abc5b548455bb2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/remove-group-subclass-82134e6915c7c782.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/save-results-4473cb5731c0c763.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/notes/shell-argv-decode-cdc13dc0c4ec07af.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.457710 osc-lib-2.6.2/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.457710 osc-lib-2.6.2/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:41.457710 osc-lib-2.6.2/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10159 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-08-24 13:23:01.000000 osc-lib-2.6.2/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2022-08-24 13:23:01.000000 osc-lib-2.6.2/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2022-08-24 13:23:41.457710 osc-lib-2.6.2/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-08-24 13:23:01.000000 osc-lib-2.6.2/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      461 2022-08-24 13:23:01.000000 osc-lib-2.6.2/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2113 2022-08-24 13:23:01.000000 osc-lib-2.6.2/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.252546 osc-lib-2.7.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-02-13 16:17:53.000000 osc-lib-2.7.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-02-13 16:17:53.000000 osc-lib-2.7.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-02-13 16:17:53.000000 osc-lib-2.7.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      807 2023-02-13 16:17:53.000000 osc-lib-2.7.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6441 2023-02-13 16:18:23.000000 osc-lib-2.7.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36129 2023-02-13 16:18:23.000000 osc-lib-2.7.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1690 2023-02-13 16:17:53.000000 osc-lib-2.7.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-13 16:17:53.000000 osc-lib-2.7.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3776 2023-02-13 16:18:23.252546 osc-lib-2.7.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2356 2023-02-13 16:17:53.000000 osc-lib-2.7.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.240546 osc-lib-2.7.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4843 2023-02-13 16:17:53.000000 osc-lib-2.7.0/doc/Makefile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.240546 osc-lib-2.7.0/doc/ext/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:17:53.000000 osc-lib-2.7.0/doc/ext/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1437 2023-02-13 16:17:53.000000 osc-lib-2.7.0/doc/ext/apidoc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-02-13 16:17:53.000000 osc-lib-2.7.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.240546 osc-lib-2.7.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7877 2023-02-13 16:17:53.000000 osc-lib-2.7.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.240546 osc-lib-2.7.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      980 2023-02-13 16:17:53.000000 osc-lib-2.7.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2023-02-13 16:17:53.000000 osc-lib-2.7.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.240546 osc-lib-2.7.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-02-13 16:17:53.000000 osc-lib-2.7.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.240546 osc-lib-2.7.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-02-13 16:17:53.000000 osc-lib-2.7.0/doc/source/user/change_log.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2023-02-13 16:17:53.000000 osc-lib-2.7.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3865 2023-02-13 16:17:53.000000 osc-lib-2.7.0/doc/source/user/transition.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2023-02-13 16:17:53.000000 osc-lib-2.7.0/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.240546 osc-lib-2.7.0/osc_lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.244546 osc-lib-2.7.0/osc_lib/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12900 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/api/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8202 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/api/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3129 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/api/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.244546 osc-lib-2.7.0/osc_lib/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/cli/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9379 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/cli/client_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1584 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/cli/format_columns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2803 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/cli/identity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10430 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/cli/parseractions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9806 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/clientmanager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.244546 osc-lib-2.7.0/osc_lib/command/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/command/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/command/command.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/command/commandmanager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1139 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/command/timing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3394 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7110 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/logs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19050 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.244546 osc-lib-2.7.0/osc_lib/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.244546 osc-lib-2.7.0/osc_lib/tests/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/api/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16739 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/api/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3383 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/api/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.244546 osc-lib-2.7.0/osc_lib/tests/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/cli/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8483 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/cli/test_client_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2941 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/cli/test_format_columns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3368 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/cli/test_identity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14128 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/cli/test_parseractions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.248546 osc-lib-2.7.0/osc_lib/tests/command/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/command/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1684 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/command/test_command.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2962 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/command/test_timing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5822 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15321 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/test_clientmanager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8697 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/test_logs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20246 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/test_shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.248546 osc-lib-2.7.0/osc_lib/tests/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14444 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2428 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/utils/test_columns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11622 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/utils/test_tags.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36608 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/tests/utils/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.248546 osc-lib-2.7.0/osc_lib/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27403 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3844 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/utils/columns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7531 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/utils/tags.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2023-02-13 16:17:53.000000 osc-lib-2.7.0/osc_lib/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.244546 osc-lib-2.7.0/osc_lib.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3776 2023-02-13 16:18:23.000000 osc-lib-2.7.0/osc_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3689 2023-02-13 16:18:23.000000 osc-lib-2.7.0/osc_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-13 16:18:23.000000 osc-lib-2.7.0/osc_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-13 16:18:23.000000 osc-lib-2.7.0/osc_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-13 16:18:23.000000 osc-lib-2.7.0/osc_lib.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-02-13 16:18:23.000000 osc-lib-2.7.0/osc_lib.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2023-02-13 16:18:23.000000 osc-lib-2.7.0/osc_lib.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.236546 osc-lib-2.7.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.248546 osc-lib-2.7.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2707 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/1.0-summary-47dcce446d6a512b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/add-KeyValueAppendAction-class-f830e71152d6b91e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/add-MultiKeyValueCommaAction-class-01dd254a287d70d2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/add_sdk_utils-d0c338eba682f2c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/arg-precedence-1ba9fd6929650830.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/auth-type-none-d96760912605f822.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/bug-1558690-1528b637f2c0a449.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/bug-1630822-mask-password-on-debug-20dcdf1c54e84fa1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/bug-2004898-686577a07e791051.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/bug-2006480-436489d39643e76c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/direct-openstacksdk-535a179f3c645cc0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/drop-py2-support-60c93244107d5778.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/find-project-203bf867619c557e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/keystone-to-keystone-9b2e55b051775322.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/none-auth-cli-48ab0e48d4852941.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/os-profile-as-environment-variable-a5e232e9ca7c5171.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/remove-babel-50abc5b548455bb2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/remove-group-subclass-82134e6915c7c782.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/save-results-4473cb5731c0c763.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/notes/shell-argv-decode-cdc13dc0c4ec07af.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.252546 osc-lib-2.7.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.252546 osc-lib-2.7.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:18:23.252546 osc-lib-2.7.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10151 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-13 16:17:53.000000 osc-lib-2.7.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2023-02-13 16:17:53.000000 osc-lib-2.7.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2023-02-13 16:18:23.252546 osc-lib-2.7.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-13 16:17:53.000000 osc-lib-2.7.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      461 2023-02-13 16:17:53.000000 osc-lib-2.7.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2119 2023-02-13 16:17:53.000000 osc-lib-2.7.0/tox.ini
```

### Comparing `osc-lib-2.6.2/.zuul.yaml` & `osc-lib-2.7.0/.zuul.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ---
 - project:
     templates:
       - check-requirements
       - openstack-lower-constraints-jobs
-      - openstack-python3-zed-jobs
+      - openstack-python3-antelope-jobs
       - osc-tox-unit-tips
       - publish-openstack-docs-pti
       - release-notes-jobs-python3
     check:
       jobs:
         - osc-functional-devstack:
             required-projects:
```

### Comparing `osc-lib-2.6.2/AUTHORS` & `osc-lib-2.7.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,15 @@
 jiaxi <jiaxi@unitedstack.com>
 jichenjc <jichenjc@cn.ibm.com>
 kavithahr <kavitha.r@nectechnologies.in>
 lijunjie <lijunjie@cloudin.cn>
 lin-hua-cheng <os.lcheng@gmail.com>
 luqitao <qtlu@fiberhome.com>
 maaoyu <maaoyu@inspur.com>
+niuke <niuke19970315@163.com>
 pengyuesheng <pengyuesheng@gohighsec.com>
 qingszhao <zhao.daqing@99cloud.net>
 qtang <qtang@vmware.com>
 rabi <ramishra@redhat.com>
 reedip <reedip.banerjee@nectechnologies.in>
 songwenping <songwenping@inspur.com>
 sunyajing <yajing.sun@easystack.cn>
```

### Comparing `osc-lib-2.6.2/ChangeLog` & `osc-lib-2.7.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+2.7.0
+-----
+
+* Remove Python 3 guide in HACKING
+* Add Python3 antelope unit tests
+* Update master for stable/zed
+* remove unicode prefix from code
+
 2.6.2
 -----
 
 * doc: Comment out language option
 
 2.6.1
 -----
@@ -21,14 +29,15 @@
 
 2.5.0
 -----
 
 * Respect 'interface' key from clouds.yaml
 * Replace allow\_get check with allow\_fetch
 * Fix TestTagHelps for python3.10
+* tox: Ignore .venv files for flake8
 * Add Python3 yoga unit tests
 * Update master for stable/xena
 
 2.4.2
 -----
 
 * Moving IRC network reference to OFTC
```

### Comparing `osc-lib-2.6.2/LICENSE` & `osc-lib-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/PKG-INFO` & `osc-lib-2.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: osc-lib
-Version: 2.6.2
+Version: 2.7.0
 Summary: OpenStackClient Library
 Home-page: https://docs.openstack.org/osc-lib/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =======
         osc-lib
```

### Comparing `osc-lib-2.6.2/README.rst` & `osc-lib-2.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/doc/Makefile` & `osc-lib-2.7.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/doc/ext/apidoc.py` & `osc-lib-2.7.0/doc/ext/apidoc.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/doc/source/conf.py` & `osc-lib-2.7.0/doc/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 # The encoding of source files.
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = u'OpenStackClient CLI Base'
+project = 'OpenStackClient CLI Base'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
@@ -182,16 +182,16 @@
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual])
 # .
 latex_documents = [
     ('index', 'OpenStackCommandLineClient.tex',
-    u'OpenStack Command Line Client Documentation',
-    u'OpenStack'),
+    'OpenStack Command Line Client Documentation',
+    'OpenStack'),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 #latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -224,16 +224,16 @@
 # -- Options for Texinfo output -----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     ('index', 'OpenStackCommandLineClient',
-    u'OpenStack Command Line Client Documentation',
-    u'OpenStack', 'OpenStackCommandLineClient',
+    'OpenStack Command Line Client Documentation',
+    'OpenStack', 'OpenStackCommandLineClient',
      'One line description of project.',
      'Miscellaneous'),
 ]
 
 # Documents to append as an appendix to all manuals.
 #texinfo_appendices = []
```

### Comparing `osc-lib-2.6.2/doc/source/contributor/index.rst` & `osc-lib-2.7.0/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/doc/source/user/transition.rst` & `osc-lib-2.7.0/doc/source/user/transition.rst`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/lower-constraints.txt` & `osc-lib-2.7.0/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/__init__.py` & `osc-lib-2.7.0/osc_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/api/api.py` & `osc-lib-2.7.0/osc_lib/api/api.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/api/auth.py` & `osc-lib-2.7.0/osc_lib/api/auth.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/api/utils.py` & `osc-lib-2.7.0/osc_lib/api/utils.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/cli/client_config.py` & `osc-lib-2.7.0/osc_lib/cli/client_config.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/cli/format_columns.py` & `osc-lib-2.7.0/osc_lib/cli/format_columns.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/cli/identity.py` & `osc-lib-2.7.0/osc_lib/cli/identity.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/cli/parseractions.py` & `osc-lib-2.7.0/osc_lib/cli/parseractions.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/clientmanager.py` & `osc-lib-2.7.0/osc_lib/clientmanager.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/command/command.py` & `osc-lib-2.7.0/osc_lib/command/command.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/command/commandmanager.py` & `osc-lib-2.7.0/osc_lib/command/commandmanager.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/command/timing.py` & `osc-lib-2.7.0/osc_lib/command/timing.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/exceptions.py` & `osc-lib-2.7.0/osc_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/i18n.py` & `osc-lib-2.7.0/osc_lib/i18n.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/logs.py` & `osc-lib-2.7.0/osc_lib/logs.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/shell.py` & `osc-lib-2.7.0/osc_lib/shell.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/api/fakes.py` & `osc-lib-2.7.0/osc_lib/tests/api/fakes.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/api/test_api.py` & `osc-lib-2.7.0/osc_lib/tests/api/test_api.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/api/test_utils.py` & `osc-lib-2.7.0/osc_lib/tests/api/test_utils.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/cli/test_client_config.py` & `osc-lib-2.7.0/osc_lib/tests/cli/test_client_config.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/cli/test_format_columns.py` & `osc-lib-2.7.0/osc_lib/tests/cli/test_format_columns.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/cli/test_identity.py` & `osc-lib-2.7.0/osc_lib/tests/cli/test_identity.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/cli/test_parseractions.py` & `osc-lib-2.7.0/osc_lib/tests/cli/test_parseractions.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/command/test_command.py` & `osc-lib-2.7.0/osc_lib/tests/command/test_command.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/command/test_timing.py` & `osc-lib-2.7.0/osc_lib/tests/command/test_timing.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/fakes.py` & `osc-lib-2.7.0/osc_lib/tests/fakes.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/test_clientmanager.py` & `osc-lib-2.7.0/osc_lib/tests/test_clientmanager.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/test_logs.py` & `osc-lib-2.7.0/osc_lib/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/test_shell.py` & `osc-lib-2.7.0/osc_lib/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/utils/__init__.py` & `osc-lib-2.7.0/osc_lib/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/utils/test_columns.py` & `osc-lib-2.7.0/osc_lib/tests/utils/test_columns.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/utils/test_tags.py` & `osc-lib-2.7.0/osc_lib/tests/utils/test_tags.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/tests/utils/test_utils.py` & `osc-lib-2.7.0/osc_lib/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/utils/__init__.py` & `osc-lib-2.7.0/osc_lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/utils/columns.py` & `osc-lib-2.7.0/osc_lib/utils/columns.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/utils/tags.py` & `osc-lib-2.7.0/osc_lib/utils/tags.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib/version.py` & `osc-lib-2.7.0/osc_lib/version.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/osc_lib.egg-info/PKG-INFO` & `osc-lib-2.7.0/osc_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: osc-lib
-Version: 2.6.2
+Version: 2.7.0
 Summary: OpenStackClient Library
 Home-page: https://docs.openstack.org/osc-lib/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =======
         osc-lib
```

### Comparing `osc-lib-2.6.2/osc_lib.egg-info/SOURCES.txt` & `osc-lib-2.7.0/osc_lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -107,9 +107,10 @@
 releasenotes/source/train.rst
 releasenotes/source/unreleased.rst
 releasenotes/source/ussuri.rst
 releasenotes/source/victoria.rst
 releasenotes/source/wallaby.rst
 releasenotes/source/xena.rst
 releasenotes/source/yoga.rst
+releasenotes/source/zed.rst
 releasenotes/source/_static/.placeholder
 releasenotes/source/_templates/.placeholder
```

### Comparing `osc-lib-2.6.2/releasenotes/notes/1.0-summary-47dcce446d6a512b.yaml` & `osc-lib-2.7.0/releasenotes/notes/1.0-summary-47dcce446d6a512b.yaml`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/releasenotes/notes/keystone-to-keystone-9b2e55b051775322.yaml` & `osc-lib-2.7.0/releasenotes/notes/keystone-to-keystone-9b2e55b051775322.yaml`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/releasenotes/source/conf.py` & `osc-lib-2.7.0/releasenotes/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,16 @@
 #
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = u'osc-lib Release Notes'
-copyright = u'2016, osc-lib Developers'
+project = 'osc-lib Release Notes'
+copyright = '2016, osc-lib Developers'
 
 # openstackdocstheme options
 openstackdocs_repo_name = 'openstack/osc-lib'
 openstackdocs_auto_name = False
 openstackdocs_use_storyboard = True
 
 # Release notes do not need a version in the title, they span
@@ -258,16 +258,16 @@
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [(
     'index',
     'OSC_LIBReleaseNotes.tex',
-    u'osc-lib Release Notes Documentation',
-    u'osc-lib Developers',
+    'osc-lib Release Notes Documentation',
+    'osc-lib Developers',
     'manual'),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 #
 # latex_logo = None
@@ -297,16 +297,16 @@
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [(
     'index',
     'osc_libreleasenotes',
-    u'osc-lib Release Notes Documentation',
-    [u'osc-lib Developers'],
+    'osc-lib Release Notes Documentation',
+    ['osc-lib Developers'],
     1,
 )]
 
 # If true, show URL addresses after external links.
 #
 # man_show_urls = False
 
@@ -315,16 +315,16 @@
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [(
     'index',
     'OSC_LIBReleaseNotes',
-    u'osc-lib Release Notes Documentation',
-    u'osc-lib Developers',
+    'osc-lib Release Notes Documentation',
+    'osc-lib Developers',
     'OSC_LIBReleaseNotes',
     'Common base library for OpenStackClient plugins.',
     'Miscellaneous',
 )]
 
 # Documents to append as an appendix to all manuals.
 #
```

### Comparing `osc-lib-2.6.2/setup.cfg` & `osc-lib-2.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/setup.py` & `osc-lib-2.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `osc-lib-2.6.2/tox.ini` & `osc-lib-2.7.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
   sphinx-build -a -E -W -d doc/build/doctrees -b html doc/source doc/build/html
 
 [testenv:releasenotes]
 commands = sphinx-build -a -E -W -d releasenotes/build/doctrees -b html releasenotes/source releasenotes/build/html
 
 [flake8]
 show-source = True
-exclude = .git,.tox,dist,doc,*lib/python*,*egg,build,tools
+exclude = .venv,.git,.tox,dist,doc,*lib/python*,*egg,build,tools
 # If 'ignore' is not set there are default errors and warnings that are set
 # Doc: http://flake8.readthedocs.org/en/latest/config.html#default
 ignore = W504
 import-order-style = pep8
 application-import-names = osc_lib
 filename = *.py
```

