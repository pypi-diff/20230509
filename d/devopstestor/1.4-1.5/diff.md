# Comparing `tmp/devopstestor-1.4.tar.gz` & `tmp/devopstestor-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopstestor-1.4.tar", last modified: Mon Apr 17 12:51:36 2023, max compression
+gzip compressed data, was "devopstestor-1.5.tar", last modified: Tue May  9 13:53:53 2023, max compression
```

## Comparing `devopstestor-1.4.tar` & `devopstestor-1.5.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.171841 devopstestor-1.4/
--rw-rw-rw-   0 root         (0) root         (0)    22958 2023-04-17 12:51:22.000000 devopstestor-1.4/LICENCE
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-04-17 12:51:22.000000 devopstestor-1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      706 2023-04-17 12:51:36.170841 devopstestor-1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-04-17 12:51:22.000000 devopstestor-1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.138838 devopstestor-1.4/devopstestor/
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.143839 devopstestor-1.4/devopstestor/config/
--rw-rw-rw-   0 root         (0) root         (0)     2837 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/config/arguments.yml
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/config/core.yml
--rw-rw-rw-   0 root         (0) root         (0)      778 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/config/machine.yml
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/config/provisionner.yml
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/config/report.yml
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/config/source_manager.yml
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/config/testcase.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.143839 devopstestor-1.4/devopstestor/src/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.145839 devopstestor-1.4/devopstestor/src/abstract/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/abstract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5424 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/abstract/abstract_machine_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/abstract/abstract_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     3498 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/abstract/abstract_report.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/abstract/abstract_source_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.148839 devopstestor-1.4/devopstestor/src/core/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5805 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/devopstestor.py
--rw-rw-rw-   0 root         (0) root         (0)     1469 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/devopstestor_client.py
--rw-rw-rw-   0 root         (0) root         (0)     2228 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/devopstestor_server.py
--rw-rw-rw-   0 root         (0) root         (0)     7926 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/global_config_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8219 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/machines_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     4851 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/ordonnanceur.py
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/report_render_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2083 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/source_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/testcase_executor_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.150839 devopstestor-1.4/devopstestor/src/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2808 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/lib/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/lib/core_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/lib/json_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2719 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/lib/log_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    11155 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/lib/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.152839 devopstestor-1.4/devopstestor/src/machine/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/machine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2093 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/machine/debug_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     7573 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/machine/docker_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     3754 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/machine/local_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     7547 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/machine/vagrant_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.154839 devopstestor-1.4/devopstestor/src/provisionner/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/provisionner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/provisionner/empty_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     4850 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/provisionner/logstash_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     8768 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/provisionner/minion_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/provisionner/systemd_provisionner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.157840 devopstestor-1.4/devopstestor/src/reporting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/campaign_report.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/deployment_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5666 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/report_elk_renderer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.158840 devopstestor-1.4/devopstestor/src/reporting/report_html_renderer/
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/report_html_renderer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9223 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja
--rw-rw-rw-   0 root         (0) root         (0)     7258 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/report_text_renderer.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/scenario_report.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/testcase_report.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/verifier_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.160840 devopstestor-1.4/devopstestor/src/scenarios/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/scenarios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/scenarios/devopstestor.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/scenarios/logstash.py
--rw-rw-rw-   0 root         (0) root         (0)     6385 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/scenarios/mock_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/scenarios/systemd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.161840 devopstestor-1.4/devopstestor/src/sources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2604 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/sources/copytemplate_source_accessor.py
--rw-rw-rw-   0 root         (0) root         (0)     2334 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/sources/dirlink_source_accessor.py
--rw-rw-rw-   0 root         (0) root         (0)     2587 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/sources/git_source_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.163840 devopstestor-1.4/devopstestor/src/testcase/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/testcase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8757 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/testcase/scenario_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     6314 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/testcase/test_case.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/testcase/testcase_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     3114 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/testcase/tests_cases_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.133838 devopstestor-1.4/devopstestor/testconf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.136838 devopstestor-1.4/devopstestor/testconf/verifiers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.164840 devopstestor-1.4/devopstestor/testconf/verifiers/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/fixtures/context_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/fixtures/logstash_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.165840 devopstestor-1.4/devopstestor/testconf/verifiers/service/
--rw-rw-rw-   0 root         (0) root         (0)     4529 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/service/http_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.165840 devopstestor-1.4/devopstestor/testconf/verifiers/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.165840 devopstestor-1.4/devopstestor/testconf/verifiers/tests/http_logger/
--rw-rw-rw-   0 root         (0) root         (0)     1317 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.166840 devopstestor-1.4/devopstestor/testconf/verifiers/tests/logstash/
--rw-rw-rw-   0 root         (0) root         (0)     5411 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.167840 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.168841 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/filesystem/
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.168841 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/packages/
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.169840 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/systemd/
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py
--rw-rw-rw-   0 root         (0) root         (0)     2256 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py
--rw-rw-rw-   0 root         (0) root         (0)     3336 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.169840 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/users/
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.169840 devopstestor-1.4/devopstestor/testconf/verifiers/utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.170841 devopstestor-1.4/devopstestor/testconf/verifiers/utils/logstash/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/utils/logstash/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6214 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py
--rw-rw-rw-   0 root         (0) root         (0)     4964 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/utils/verififier_luncher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.140838 devopstestor-1.4/devopstestor.egg-info/
--rw-r--r--   0 root         (0) root         (0)      706 2023-04-17 12:51:36.000000 devopstestor-1.4/devopstestor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4372 2023-04-17 12:51:36.000000 devopstestor-1.4/devopstestor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 12:51:36.000000 devopstestor-1.4/devopstestor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-04-17 12:51:36.000000 devopstestor-1.4/devopstestor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 12:51:36.000000 devopstestor-1.4/devopstestor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 12:51:36.171841 devopstestor-1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-04-17 12:51:22.000000 devopstestor-1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.704228 devopstestor-1.5/
+-rw-rw-rw-   0 root         (0) root         (0)    22958 2023-05-09 13:53:39.000000 devopstestor-1.5/LICENCE
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-05-09 13:53:39.000000 devopstestor-1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      706 2023-05-09 13:53:53.703227 devopstestor-1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-05-09 13:53:39.000000 devopstestor-1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.670224 devopstestor-1.5/devopstestor/
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.674224 devopstestor-1.5/devopstestor/config/
+-rw-rw-rw-   0 root         (0) root         (0)     2837 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/config/arguments.yml
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/config/core.yml
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/config/machine.yml
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/config/provisionner.yml
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/config/report.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/config/source_manager.yml
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/config/testcase.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.674224 devopstestor-1.5/devopstestor/src/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.676225 devopstestor-1.5/devopstestor/src/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/abstract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5424 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/abstract/abstract_machine_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/abstract/abstract_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3498 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/abstract/abstract_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/abstract/abstract_source_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.680225 devopstestor-1.5/devopstestor/src/core/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5805 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/core/devopstestor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/core/devopstestor_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2228 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/core/devopstestor_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     7926 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/core/global_config_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8219 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/core/machines_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4851 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/core/ordonnanceur.py
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/core/report_render_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2083 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/core/source_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/core/testcase_executor_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.682225 devopstestor-1.5/devopstestor/src/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2808 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/lib/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/lib/core_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/lib/json_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/lib/log_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    11155 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/lib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.684225 devopstestor-1.5/devopstestor/src/machine/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/machine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/machine/debug_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     7573 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/machine/docker_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     3754 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/machine/local_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     7560 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/machine/vagrant_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.686226 devopstestor-1.5/devopstestor/src/provisionner/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/provisionner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/provisionner/empty_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/provisionner/logstash_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     8768 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/provisionner/minion_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/provisionner/systemd_provisionner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.689226 devopstestor-1.5/devopstestor/src/reporting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/reporting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/reporting/campaign_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/reporting/deployment_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5666 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/reporting/report_elk_renderer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.690226 devopstestor-1.5/devopstestor/src/reporting/report_html_renderer/
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/reporting/report_html_renderer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9223 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja
+-rw-rw-rw-   0 root         (0) root         (0)     7258 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/reporting/report_text_renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/reporting/scenario_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/reporting/testcase_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/reporting/verifier_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.692226 devopstestor-1.5/devopstestor/src/scenarios/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/scenarios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/scenarios/devopstestor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/scenarios/logstash.py
+-rw-rw-rw-   0 root         (0) root         (0)     6385 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/scenarios/mock_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/scenarios/systemd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.693226 devopstestor-1.5/devopstestor/src/sources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2604 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/sources/copytemplate_source_accessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/sources/dirlink_source_accessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2587 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/sources/git_source_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.695227 devopstestor-1.5/devopstestor/src/testcase/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/testcase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8757 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/testcase/scenario_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6314 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/testcase/test_case.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/testcase/testcase_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3114 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/src/testcase/tests_cases_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.664223 devopstestor-1.5/devopstestor/testconf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.667224 devopstestor-1.5/devopstestor/testconf/verifiers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.697227 devopstestor-1.5/devopstestor/testconf/verifiers/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/fixtures/context_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/fixtures/logstash_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.697227 devopstestor-1.5/devopstestor/testconf/verifiers/service/
+-rw-rw-rw-   0 root         (0) root         (0)     4529 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/service/http_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.697227 devopstestor-1.5/devopstestor/testconf/verifiers/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.698227 devopstestor-1.5/devopstestor/testconf/verifiers/tests/http_logger/
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.698227 devopstestor-1.5/devopstestor/testconf/verifiers/tests/logstash/
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/tests/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.699227 devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.700227 devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/filesystem/
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.700227 devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/packages/
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.701227 devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/systemd/
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py
+-rw-rw-rw-   0 root         (0) root         (0)     3336 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.702227 devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/users/
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.702227 devopstestor-1.5/devopstestor/testconf/verifiers/utils/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.703227 devopstestor-1.5/devopstestor/testconf/verifiers/utils/logstash/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/utils/logstash/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6214 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4964 2023-05-09 13:53:39.000000 devopstestor-1.5/devopstestor/testconf/verifiers/utils/verififier_luncher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 13:53:53.671224 devopstestor-1.5/devopstestor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      706 2023-05-09 13:53:53.000000 devopstestor-1.5/devopstestor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-05-09 13:53:53.000000 devopstestor-1.5/devopstestor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 13:53:53.000000 devopstestor-1.5/devopstestor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-05-09 13:53:53.000000 devopstestor-1.5/devopstestor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 13:53:53.000000 devopstestor-1.5/devopstestor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 13:53:53.704228 devopstestor-1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2023-05-09 13:53:39.000000 devopstestor-1.5/setup.py
```

### Comparing `devopstestor-1.4/LICENCE` & `devopstestor-1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/PKG-INFO` & `devopstestor-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopstestor
-Version: 1.4
+Version: 1.5
 Summary: Framwork to auto test machine provisioning
 Home-page: https://gitlab.com/alexis.porzier.pro/devopstestor
 Author: Alexis PORZIER
 Author-email: alexis.porzier.pro@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `devopstestor-1.4/devopstestor/config/arguments.yml` & `devopstestor-1.5/devopstestor/config/arguments.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/config/machine.yml` & `devopstestor-1.5/devopstestor/config/machine.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/config/report.yml` & `devopstestor-1.5/devopstestor/config/report.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/config/source_manager.yml` & `devopstestor-1.5/devopstestor/config/source_manager.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/config/testcase.yml` & `devopstestor-1.5/devopstestor/config/testcase.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/abstract/abstract_machine_controller.py` & `devopstestor-1.5/devopstestor/src/abstract/abstract_machine_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/abstract/abstract_provisionner.py` & `devopstestor-1.5/devopstestor/src/abstract/abstract_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/abstract/abstract_report.py` & `devopstestor-1.5/devopstestor/src/abstract/abstract_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/abstract/abstract_source_accessor.py` & `devopstestor-1.5/devopstestor/src/abstract/abstract_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/core/devopstestor.py` & `devopstestor-1.5/devopstestor/src/core/devopstestor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/core/devopstestor_client.py` & `devopstestor-1.5/devopstestor/src/core/devopstestor_client.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/core/devopstestor_server.py` & `devopstestor-1.5/devopstestor/src/core/devopstestor_server.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/core/global_config_factory.py` & `devopstestor-1.5/devopstestor/src/core/global_config_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/core/machines_factory.py` & `devopstestor-1.5/devopstestor/src/core/machines_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/core/ordonnanceur.py` & `devopstestor-1.5/devopstestor/src/core/ordonnanceur.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/core/report_render_manager.py` & `devopstestor-1.5/devopstestor/src/core/report_render_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/core/source_manager.py` & `devopstestor-1.5/devopstestor/src/core/source_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/core/testcase_executor_factory.py` & `devopstestor-1.5/devopstestor/src/core/testcase_executor_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/lib/config.py` & `devopstestor-1.5/devopstestor/src/lib/config.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/lib/core_utils.py` & `devopstestor-1.5/devopstestor/src/lib/core_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/lib/json_utils.py` & `devopstestor-1.5/devopstestor/src/lib/json_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/lib/log_manager.py` & `devopstestor-1.5/devopstestor/src/lib/log_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/lib/utils.py` & `devopstestor-1.5/devopstestor/src/lib/utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/machine/debug_controller.py` & `devopstestor-1.5/devopstestor/src/machine/debug_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/machine/docker_controller.py` & `devopstestor-1.5/devopstestor/src/machine/docker_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/machine/local_controller.py` & `devopstestor-1.5/devopstestor/src/machine/local_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/machine/vagrant_controller.py` & `devopstestor-1.5/devopstestor/src/machine/vagrant_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             local_path += "/"
 
         with settings(host_string=self.vagrant.user_hostname_port(vm_name=self.vagrant_vm_name),
             key_filename = self.vagrant.keyfile(vm_name=self.vagrant_vm_name),
             disable_known_hosts = True, warn_only=True):
 
             rsync_project(remote_dir=vm_path, local_dir=local_path, ssh_opts="-o StrictHostKeyChecking=no",
-                         exclude=['.git'])
+                         exclude=['.git'], delete=True)
     
 
     def run_cmd(self, command: str, workdir:str=None) -> tuple:
         """
         Lance une commande sur la VM.
         """
         ret=-1
```

### Comparing `devopstestor-1.4/devopstestor/src/provisionner/empty_provisionner.py` & `devopstestor-1.5/devopstestor/src/provisionner/empty_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/provisionner/logstash_provisionner.py` & `devopstestor-1.5/devopstestor/src/provisionner/logstash_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/provisionner/minion_provisionner.py` & `devopstestor-1.5/devopstestor/src/provisionner/minion_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/provisionner/systemd_provisionner.py` & `devopstestor-1.5/devopstestor/src/provisionner/systemd_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/reporting/report_elk_renderer.py` & `devopstestor-1.5/devopstestor/src/reporting/report_elk_renderer.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/reporting/report_html_renderer/__init__.py` & `devopstestor-1.5/devopstestor/src/reporting/report_html_renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja` & `devopstestor-1.5/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/reporting/report_text_renderer.py` & `devopstestor-1.5/devopstestor/src/reporting/report_text_renderer.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/reporting/scenario_report.py` & `devopstestor-1.5/devopstestor/src/reporting/scenario_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/reporting/testcase_report.py` & `devopstestor-1.5/devopstestor/src/reporting/testcase_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/reporting/verifier_report.py` & `devopstestor-1.5/devopstestor/src/reporting/verifier_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/scenarios/devopstestor.py` & `devopstestor-1.5/devopstestor/src/scenarios/devopstestor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/scenarios/logstash.py` & `devopstestor-1.5/devopstestor/src/scenarios/logstash.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/scenarios/mock_utils.py` & `devopstestor-1.5/devopstestor/src/scenarios/mock_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/scenarios/systemd.py` & `devopstestor-1.5/devopstestor/src/scenarios/systemd.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/sources/copytemplate_source_accessor.py` & `devopstestor-1.5/devopstestor/src/sources/copytemplate_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/sources/dirlink_source_accessor.py` & `devopstestor-1.5/devopstestor/src/sources/dirlink_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/sources/git_source_accessor.py` & `devopstestor-1.5/devopstestor/src/sources/git_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/testcase/scenario_executor.py` & `devopstestor-1.5/devopstestor/src/testcase/scenario_executor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/testcase/test_case.py` & `devopstestor-1.5/devopstestor/src/testcase/test_case.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/testcase/testcase_executor.py` & `devopstestor-1.5/devopstestor/src/testcase/testcase_executor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/src/testcase/tests_cases_loader.py` & `devopstestor-1.5/devopstestor/src/testcase/tests_cases_loader.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/testconf/verifiers/fixtures/context_fixtures.py` & `devopstestor-1.5/devopstestor/testconf/verifiers/fixtures/context_fixtures.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py` & `devopstestor-1.5/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/testconf/verifiers/service/http_logger.py` & `devopstestor-1.5/devopstestor/testconf/verifiers/service/http_logger.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py` & `devopstestor-1.5/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py` & `devopstestor-1.5/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py` & `devopstestor-1.5/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py` & `devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py` & `devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py` & `devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py` & `devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py` & `devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py` & `devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py` & `devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py` & `devopstestor-1.5/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py` & `devopstestor-1.5/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor/testconf/verifiers/utils/verififier_luncher.py` & `devopstestor-1.5/devopstestor/testconf/verifiers/utils/verififier_luncher.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/devopstestor.egg-info/PKG-INFO` & `devopstestor-1.5/devopstestor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopstestor
-Version: 1.4
+Version: 1.5
 Summary: Framwork to auto test machine provisioning
 Home-page: https://gitlab.com/alexis.porzier.pro/devopstestor
 Author: Alexis PORZIER
 Author-email: alexis.porzier.pro@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `devopstestor-1.4/devopstestor.egg-info/SOURCES.txt` & `devopstestor-1.5/devopstestor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devopstestor-1.4/setup.py` & `devopstestor-1.5/setup.py`

 * *Files identical despite different names*

