# Comparing `tmp/troubadix-23.5.1.tar.gz` & `tmp/troubadix-23.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troubadix-23.5.1.tar", max compression
+gzip compressed data, was "troubadix-23.5.2.tar", max compression
```

## Comparing `troubadix-23.5.1.tar` & `troubadix-23.5.2.tar`

### file list

```diff
@@ -1,194 +1,194 @@
--rw-r--r--   0        0        0    35149 2023-05-08 12:20:15.848211 troubadix-23.5.1/LICENSE
--rw-r--r--   0        0        0     2730 2023-05-08 12:20:15.848211 troubadix-23.5.1/README.md
--rw-r--r--   0        0        0     2412 2023-05-08 12:20:15.852209 troubadix-23.5.1/pyproject.toml
--rw-r--r--   0        0        0      716 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/__init__.py
--rw-r--r--   0        0        0      716 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/helper/__init__.py
--rw-r--r--   0        0        0     8416 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/helper/test_linguistic_exception_handler.py
--rw-r--r--   0        0        0     1940 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/helper/test_patterns.py
--rw-r--r--   0        0        0     2396 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/__init__.py
--rw-r--r--   0        0        0     1012 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/fail.nasl
--rw-r--r--   0        0        0     1291 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/fail2.nasl
--rw-r--r--   0        0        0     2100 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test.nasl
--rw-r--r--   0        0        0     2061 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_badwords.py
--rw-r--r--   0        0        0     5109 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_copyright_text.py
--rw-r--r--   0        0        0     6961 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_copyright_year.py
--rw-r--r--   0        0        0     5004 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_creation_date.py
--rw-r--r--   0        0        0     5881 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_cve_format.py
--rw-r--r--   0        0        0     4914 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_cvss_format.py
--rw-r--r--   0        0        0     8970 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_dependencies.py
--rw-r--r--   0        0        0     5808 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_dependency_category_order.py
--rw-r--r--   0        0        0     5589 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_deprecated_dependency.py
--rw-r--r--   0        0        0     4545 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_deprecated_functions.py
--rw-r--r--   0        0        0     2394 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_double_end_points.py
--rw-r--r--   0        0        0     3504 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_duplicate_oid.py
--rw-r--r--   0        0        0     4686 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_duplicated_script_tags.py
--rw-r--r--   0        0        0     3906 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_encoding.py
--rw-r--r--   0        0        0     1982 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/fail_bad_new_line.nasl
--rw-r--r--   0        0        0      246 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/fail_badwords.nasl
--rw-r--r--   0        0        0     1979 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/fail_name_and_copyright_newline.nasl
--rw-r--r--   0        0        0     1965 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/fail_name_newline.nasl
--rwxr-xr-x   0        0        0     1012 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/fail_permissions.nasl
--rw-r--r--   0        0        0      150 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/fail_spelling.nasl
--rw-r--r--   0        0        0     2213 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/fail.nasl
--rw-r--r--   0        0        0      246 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/fail_badwords.nasl
--rw-r--r--   0        0        0     1990 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl
--rw-r--r--   0        0        0     1987 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl
--rw-r--r--   0        0        0     2134 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl
--rw-r--r--   0        0        0     1023 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/runner/fail.nasl
--rw-r--r--   0        0        0     1302 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl
--rw-r--r--   0        0        0     2122 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/runner/test.nasl
--rw-r--r--   0        0        0     2119 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl
--rw-r--r--   0        0        0     1023 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/test.inc
--rw-r--r--   0        0        0     2122 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/test.nasl
--rw-r--r--   0        0        0     2976 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/nasl/warning.nasl
--rw-r--r--   0        0        0     1012 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/ok_permissions.nasl
--rw-r--r--   0        0        0     2100 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_files/test_oid.nasl
--rw-r--r--   0        0        0     4548 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_forking_nasl_functions.py
--rw-r--r--   0        0        0     2271 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_get_kb_on_services.py
--rw-r--r--   0        0        0     9438 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_grammar.py
--rw-r--r--   0        0        0     6936 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_http_links_in_tags.py
--rw-r--r--   0        0        0     4730 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_illegal_characters.py
--rw-r--r--   0        0        0     5965 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_log_messages.py
--rw-r--r--   0        0        0     6174 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_malformed_dependencies.py
--rw-r--r--   0        0        0    21051 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_misplaced_compare_in_if.py
--rw-r--r--   0        0        0     3585 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_missing_desc_exit.py
--rw-r--r--   0        0        0     3101 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_missing_tag_solution.py
--rw-r--r--   0        0        0     4688 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_newlines.py
--rw-r--r--   0        0        0    40813 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_overlong_script_tags.py
--rw-r--r--   0        0        0     4294 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_prod_svc_detect_in_vulnvt.py
--rw-r--r--   0        0        0     4594 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_qod.py
--rw-r--r--   0        0        0     5844 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_reporting_consistency.py
--rw-r--r--   0        0        0     3371 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_script_add_preference_type.py
--rw-r--r--   0        0        0     2353 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_script_calls_empty_values.py
--rw-r--r--   0        0        0     2799 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_script_calls_recommended.py
--rw-r--r--   0        0        0     2650 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_script_category.py
--rw-r--r--   0        0        0     3469 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_script_copyright.py
--rw-r--r--   0        0        0     3877 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_script_family.py
--rw-r--r--   0        0        0     3079 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_script_tag_form.py
--rw-r--r--   0        0        0     3086 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_script_tag_whitespaces.py
--rw-r--r--   0        0        0     3313 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_script_tags_mandatory.py
--rw-r--r--   0        0        0     4858 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_script_version_and_last_modification_tags.py
--rw-r--r--   0        0        0     3016 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_script_xref_form.py
--rw-r--r--   0        0        0     2189 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_script_xref_url.py
--rw-r--r--   0        0        0     6599 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_security_messages.py
--rw-r--r--   0        0        0     3021 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_set_get_kb_calls.py
--rw-r--r--   0        0        0     7260 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_solution_text.py
--rw-r--r--   0        0        0     3306 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_solution_type.py
--rw-r--r--   0        0        0     2827 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_spelling.py
--rw-r--r--   0        0        0     1813 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_tabs.py
--rw-r--r--   0        0        0     6297 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_todo_tbd.py
--rw-r--r--   0        0        0     2398 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_trailing_spaces_tabs.py
--rw-r--r--   0        0        0     3868 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_using_display.py
--rw-r--r--   0        0        0    24134 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_valid_oid.py
--rw-r--r--   0        0        0     4154 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_valid_script_tag_names.py
--rw-r--r--   0        0        0     1947 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_vt_file_permissions.py
--rw-r--r--   0        0        0     5189 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/plugins/test_vt_placement.py
--rw-r--r--   0        0        0      716 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/standalone_plugins/__init__.py
--rw-r--r--   0        0        0      716 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/standalone_plugins/changed_packages/__init__.py
--rw-r--r--   0        0        0      716 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/standalone_plugins/changed_packages/markers/__init__.py
--rw-r--r--   0        0        0     3075 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py
--rw-r--r--   0        0        0     2620 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/standalone_plugins/changed_packages/markers/test_added_release.py
--rw-r--r--   0        0        0     1792 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py
--rw-r--r--   0        0        0     3258 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/standalone_plugins/changed_packages/markers/test_changed_update.py
--rw-r--r--   0        0        0     3584 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py
--rw-r--r--   0        0        0     3780 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/standalone_plugins/changed_packages/test_changed_packages.py
--rw-r--r--   0        0        0     2427 2023-05-08 12:20:15.852209 troubadix-23.5.1/tests/standalone_plugins/changed_packages/test_package.py
--rw-r--r--   0        0        0     2977 2023-05-08 12:20:15.856208 troubadix-23.5.1/tests/standalone_plugins/test_changed_cves.py
--rw-r--r--   0        0        0     2952 2023-05-08 12:20:15.856208 troubadix-23.5.1/tests/standalone_plugins/test_changed_oid.py
--rw-r--r--   0        0        0     3962 2023-05-08 12:20:15.856208 troubadix-23.5.1/tests/standalone_plugins/test_last_modification.py
--rw-r--r--   0        0        0     7347 2023-05-08 12:20:15.856208 troubadix-23.5.1/tests/standalone_plugins/test_no_solution.py
--rw-r--r--   0        0        0     6293 2023-05-08 12:20:15.856208 troubadix-23.5.1/tests/standalone_plugins/test_version_updated.py
--rw-r--r--   0        0        0     4768 2023-05-08 12:20:15.856208 troubadix-23.5.1/tests/test_argparser.py
--rw-r--r--   0        0        0     3947 2023-05-08 12:20:15.856208 troubadix-23.5.1/tests/test_helper.py
--rw-r--r--   0        0        0     3671 2023-05-08 12:20:15.856208 troubadix-23.5.1/tests/test_naslinter.py
--rw-r--r--   0        0        0     3399 2023-05-08 12:20:15.856208 troubadix-23.5.1/tests/test_reporter.py
--rw-r--r--   0        0        0     2517 2023-05-08 12:20:15.856208 troubadix-23.5.1/tests/test_results.py
--rw-r--r--   0        0        0    17972 2023-05-08 12:20:15.856208 troubadix-23.5.1/tests/test_runner.py
--rw-r--r--   0        0        0      716 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/__init__.py
--rw-r--r--   0        0        0      103 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/__version__.py
--rw-r--r--   0        0        0     6999 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/argparser.py
--rw-r--r--   0        0        0      338 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/codespell/codespell.additions
--rw-r--r--   0        0        0   125039 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/codespell/codespell.exclude
--rw-r--r--   0        0        0      756 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/codespell/codespell.ignore
--rw-r--r--   0        0        0     1061 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/helper/__init__.py
--rw-r--r--   0        0        0     3105 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/helper/helper.py
--rw-r--r--   0        0        0     6811 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/helper/linguistic_exception_handler.py
--rw-r--r--   0        0        0     9370 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/helper/patterns.py
--rw-r--r--   0        0        0     3508 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugin.py
--rw-r--r--   0        0        0     7013 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/__init__.py
--rw-r--r--   0        0        0     3633 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/badwords.py
--rw-r--r--   0        0        0     3583 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/copyright_text.py
--rw-r--r--   0        0        0     3334 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/copyright_year.py
--rw-r--r--   0        0        0     3357 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/creation_date.py
--rw-r--r--   0        0        0     3400 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/cve_format.py
--rw-r--r--   0        0        0     2309 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/cvss_format.py
--rw-r--r--   0        0        0     4456 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/dependencies.py
--rw-r--r--   0        0        0     7316 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/dependency_category_order.py
--rw-r--r--   0        0        0     4137 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/deprecated_dependency.py
--rw-r--r--   0        0        0     2568 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/deprecated_functions.py
--rw-r--r--   0        0        0     2509 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/double_end_points.py
--rw-r--r--   0        0        0     2652 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/duplicate_oid.py
--rw-r--r--   0        0        0     3179 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/duplicated_script_tags.py
--rw-r--r--   0        0        0     2090 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/encoding.py
--rw-r--r--   0        0        0     6014 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/forking_nasl_functions.py
--rw-r--r--   0        0        0     3401 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/get_kb_on_services.py
--rw-r--r--   0        0        0     8348 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/grammar.py
--rw-r--r--   0        0        0     7157 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/http_links_in_tags.py
--rw-r--r--   0        0        0     4406 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/illegal_characters.py
--rw-r--r--   0        0        0     2960 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/log_messages.py
--rw-r--r--   0        0        0     3000 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/malformed_dependencies.py
--rw-r--r--   0        0        0     5330 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/misplaced_compare_in_if.py
--rw-r--r--   0        0        0     2411 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/missing_desc_exit.py
--rw-r--r--   0        0        0     2828 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/missing_tag_solution.py
--rw-r--r--   0        0        0     2788 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/newlines.py
--rw-r--r--   0        0        0     2373 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/overlong_script_tags.py
--rw-r--r--   0        0        0     4185 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/prod_svc_detect_in_vulnvt.py
--rw-r--r--   0        0        0     3790 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/qod.py
--rw-r--r--   0        0        0     4043 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/reporting_consistency.py
--rw-r--r--   0        0        0     3193 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/script_add_preference_type.py
--rw-r--r--   0        0        0     2512 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/script_calls_empty_values.py
--rw-r--r--   0        0        0     3137 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/script_calls_recommended.py
--rw-r--r--   0        0        0     2184 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/script_category.py
--rw-r--r--   0        0        0     2310 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/script_copyright.py
--rw-r--r--   0        0        0     4023 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/script_family.py
--rw-r--r--   0        0        0     1773 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/script_tag_form.py
--rw-r--r--   0        0        0     1861 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/script_tag_whitespaces.py
--rw-r--r--   0        0        0     2630 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/script_tags_mandatory.py
--rw-r--r--   0        0        0     7026 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/script_version_and_last_modification_tags.py
--rw-r--r--   0        0        0     1848 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/script_xref_form.py
--rw-r--r--   0        0        0     2875 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/script_xref_url.py
--rw-r--r--   0        0        0     4708 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/security_messages.py
--rw-r--r--   0        0        0     3415 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/set_get_kb_calls.py
--rw-r--r--   0        0        0     5852 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/solution_text.py
--rw-r--r--   0        0        0     2602 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/solution_type.py
--rw-r--r--   0        0        0     9638 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/spelling.py
--rw-r--r--   0        0        0     1319 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/tabs.py
--rw-r--r--   0        0        0     1733 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/todo_tbd.py
--rw-r--r--   0        0        0     2049 2023-05-08 12:20:15.856208 troubadix-23.5.1/troubadix/plugins/trailing_spaces_tabs.py
--rw-r--r--   0        0        0     4046 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/plugins/using_display.py
--rw-r--r--   0        0        0    16627 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/plugins/valid_oid.py
--rw-r--r--   0        0        0     3447 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/plugins/valid_script_tag_names.py
--rw-r--r--   0        0        0     3285 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/plugins/variable_assigned_in_if.py
--rw-r--r--   0        0        0     1521 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/plugins/vt_file_permissions.py
--rw-r--r--   0        0        0     2800 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/plugins/vt_placement.py
--rw-r--r--   0        0        0     9176 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/reporter.py
--rw-r--r--   0        0        0     2632 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/results.py
--rw-r--r--   0        0        0     5172 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/runner.py
--rw-r--r--   0        0        0       22 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/standalone_plugins/__init__.py
--rw-r--r--   0        0        0     2921 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/standalone_plugins/changed_cves.py
--rw-r--r--   0        0        0     4074 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/standalone_plugins/changed_oid.py
--rw-r--r--   0        0        0     5742 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/changed_packages.py
--rw-r--r--   0        0        0      923 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/marker/__init__.py
--rw-r--r--   0        0        0     1797 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py
--rw-r--r--   0        0        0     1486 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/marker/added_release.py
--rw-r--r--   0        0        0     1124 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py
--rw-r--r--   0        0        0     1952 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/marker/changed_update.py
--rw-r--r--   0        0        0     1632 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py
--rw-r--r--   0        0        0     1278 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/marker/marker.py
--rw-r--r--   0        0        0     2743 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/package.py
--rw-r--r--   0        0        0     1028 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/standalone_plugins/common.py
--rw-r--r--   0        0        0     4616 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/standalone_plugins/last_modification.py
--rw-r--r--   0        0        0     8463 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/standalone_plugins/no_solution.py
--rw-r--r--   0        0        0     4263 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/standalone_plugins/version_updated.py
--rw-r--r--   0        0        0     6045 2023-05-08 12:20:15.860207 troubadix-23.5.1/troubadix/troubadix.py
--rw-r--r--   0        0        0     4129 1970-01-01 00:00:00.000000 troubadix-23.5.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-09 10:26:14.399202 troubadix-23.5.2/LICENSE
+-rw-r--r--   0        0        0     2730 2023-05-09 10:26:14.399202 troubadix-23.5.2/README.md
+-rw-r--r--   0        0        0     2412 2023-05-09 10:26:14.403202 troubadix-23.5.2/pyproject.toml
+-rw-r--r--   0        0        0      716 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/helper/__init__.py
+-rw-r--r--   0        0        0     8416 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/helper/test_linguistic_exception_handler.py
+-rw-r--r--   0        0        0     1940 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/helper/test_patterns.py
+-rw-r--r--   0        0        0     2396 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/__init__.py
+-rw-r--r--   0        0        0     1012 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/fail.nasl
+-rw-r--r--   0        0        0     1291 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/fail2.nasl
+-rw-r--r--   0        0        0     2100 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test.nasl
+-rw-r--r--   0        0        0     2061 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_badwords.py
+-rw-r--r--   0        0        0     5109 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_copyright_text.py
+-rw-r--r--   0        0        0     6961 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_copyright_year.py
+-rw-r--r--   0        0        0     5004 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_creation_date.py
+-rw-r--r--   0        0        0     5881 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_cve_format.py
+-rw-r--r--   0        0        0     4914 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_cvss_format.py
+-rw-r--r--   0        0        0     8970 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_dependencies.py
+-rw-r--r--   0        0        0     5808 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_dependency_category_order.py
+-rw-r--r--   0        0        0     5589 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_deprecated_dependency.py
+-rw-r--r--   0        0        0     4545 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_deprecated_functions.py
+-rw-r--r--   0        0        0     2394 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_double_end_points.py
+-rw-r--r--   0        0        0     3504 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_duplicate_oid.py
+-rw-r--r--   0        0        0     4686 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_duplicated_script_tags.py
+-rw-r--r--   0        0        0     3906 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_encoding.py
+-rw-r--r--   0        0        0     1982 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/fail_bad_new_line.nasl
+-rw-r--r--   0        0        0      246 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/fail_badwords.nasl
+-rw-r--r--   0        0        0     1979 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/fail_name_and_copyright_newline.nasl
+-rw-r--r--   0        0        0     1965 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/fail_name_newline.nasl
+-rwxr-xr-x   0        0        0     1012 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/fail_permissions.nasl
+-rw-r--r--   0        0        0      150 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/fail_spelling.nasl
+-rw-r--r--   0        0        0     2213 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/fail.nasl
+-rw-r--r--   0        0        0      246 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/fail_badwords.nasl
+-rw-r--r--   0        0        0     1990 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl
+-rw-r--r--   0        0        0     1987 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl
+-rw-r--r--   0        0        0     2134 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl
+-rw-r--r--   0        0        0     1023 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/runner/fail.nasl
+-rw-r--r--   0        0        0     1302 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl
+-rw-r--r--   0        0        0     2122 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/runner/test.nasl
+-rw-r--r--   0        0        0     2119 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl
+-rw-r--r--   0        0        0     1023 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/test.inc
+-rw-r--r--   0        0        0     2122 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/test.nasl
+-rw-r--r--   0        0        0     2976 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/nasl/warning.nasl
+-rw-r--r--   0        0        0     1012 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/ok_permissions.nasl
+-rw-r--r--   0        0        0     2100 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_files/test_oid.nasl
+-rw-r--r--   0        0        0     4548 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_forking_nasl_functions.py
+-rw-r--r--   0        0        0     2271 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_get_kb_on_services.py
+-rw-r--r--   0        0        0     9438 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_grammar.py
+-rw-r--r--   0        0        0     6936 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_http_links_in_tags.py
+-rw-r--r--   0        0        0     4730 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_illegal_characters.py
+-rw-r--r--   0        0        0     5965 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_log_messages.py
+-rw-r--r--   0        0        0     6174 2023-05-09 10:26:14.403202 troubadix-23.5.2/tests/plugins/test_malformed_dependencies.py
+-rw-r--r--   0        0        0    21051 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_misplaced_compare_in_if.py
+-rw-r--r--   0        0        0     3585 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_missing_desc_exit.py
+-rw-r--r--   0        0        0     3101 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_missing_tag_solution.py
+-rw-r--r--   0        0        0     4688 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_newlines.py
+-rw-r--r--   0        0        0    40813 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_overlong_script_tags.py
+-rw-r--r--   0        0        0     4294 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_prod_svc_detect_in_vulnvt.py
+-rw-r--r--   0        0        0     4594 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_qod.py
+-rw-r--r--   0        0        0     5844 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_reporting_consistency.py
+-rw-r--r--   0        0        0     3371 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_script_add_preference_type.py
+-rw-r--r--   0        0        0     2353 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_script_calls_empty_values.py
+-rw-r--r--   0        0        0     2799 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_script_calls_recommended.py
+-rw-r--r--   0        0        0     2650 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_script_category.py
+-rw-r--r--   0        0        0     3469 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_script_copyright.py
+-rw-r--r--   0        0        0     3877 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_script_family.py
+-rw-r--r--   0        0        0     3079 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_script_tag_form.py
+-rw-r--r--   0        0        0     6010 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_script_tag_whitespaces.py
+-rw-r--r--   0        0        0     3313 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_script_tags_mandatory.py
+-rw-r--r--   0        0        0     4858 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_script_version_and_last_modification_tags.py
+-rw-r--r--   0        0        0     3016 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_script_xref_form.py
+-rw-r--r--   0        0        0     2189 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_script_xref_url.py
+-rw-r--r--   0        0        0     6599 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_security_messages.py
+-rw-r--r--   0        0        0     3021 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_set_get_kb_calls.py
+-rw-r--r--   0        0        0     7260 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_solution_text.py
+-rw-r--r--   0        0        0     3306 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_solution_type.py
+-rw-r--r--   0        0        0     2827 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_spelling.py
+-rw-r--r--   0        0        0     1813 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_tabs.py
+-rw-r--r--   0        0        0     6297 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_todo_tbd.py
+-rw-r--r--   0        0        0     2398 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_trailing_spaces_tabs.py
+-rw-r--r--   0        0        0     3868 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_using_display.py
+-rw-r--r--   0        0        0    24134 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_valid_oid.py
+-rw-r--r--   0        0        0     4154 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_valid_script_tag_names.py
+-rw-r--r--   0        0        0     1947 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_vt_file_permissions.py
+-rw-r--r--   0        0        0     5189 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/plugins/test_vt_placement.py
+-rw-r--r--   0        0        0      716 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/standalone_plugins/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/standalone_plugins/changed_packages/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/standalone_plugins/changed_packages/markers/__init__.py
+-rw-r--r--   0        0        0     3075 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py
+-rw-r--r--   0        0        0     2620 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/standalone_plugins/changed_packages/markers/test_added_release.py
+-rw-r--r--   0        0        0     1792 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py
+-rw-r--r--   0        0        0     3258 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/standalone_plugins/changed_packages/markers/test_changed_update.py
+-rw-r--r--   0        0        0     3584 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py
+-rw-r--r--   0        0        0     3780 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/standalone_plugins/changed_packages/test_changed_packages.py
+-rw-r--r--   0        0        0     2427 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/standalone_plugins/changed_packages/test_package.py
+-rw-r--r--   0        0        0     2977 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/standalone_plugins/test_changed_cves.py
+-rw-r--r--   0        0        0     2952 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/standalone_plugins/test_changed_oid.py
+-rw-r--r--   0        0        0     3962 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/standalone_plugins/test_last_modification.py
+-rw-r--r--   0        0        0     7347 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/standalone_plugins/test_no_solution.py
+-rw-r--r--   0        0        0     6293 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/standalone_plugins/test_version_updated.py
+-rw-r--r--   0        0        0     4768 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/test_argparser.py
+-rw-r--r--   0        0        0     3947 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/test_helper.py
+-rw-r--r--   0        0        0     3671 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/test_naslinter.py
+-rw-r--r--   0        0        0     3399 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/test_reporter.py
+-rw-r--r--   0        0        0     2517 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/test_results.py
+-rw-r--r--   0        0        0    17972 2023-05-09 10:26:14.407202 troubadix-23.5.2/tests/test_runner.py
+-rw-r--r--   0        0        0      716 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/__init__.py
+-rw-r--r--   0        0        0      103 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/__version__.py
+-rw-r--r--   0        0        0     6999 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/argparser.py
+-rw-r--r--   0        0        0      338 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/codespell/codespell.additions
+-rw-r--r--   0        0        0   125039 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/codespell/codespell.exclude
+-rw-r--r--   0        0        0      756 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/codespell/codespell.ignore
+-rw-r--r--   0        0        0     1061 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/helper/__init__.py
+-rw-r--r--   0        0        0     3105 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/helper/helper.py
+-rw-r--r--   0        0        0     6811 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/helper/linguistic_exception_handler.py
+-rw-r--r--   0        0        0     9370 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/helper/patterns.py
+-rw-r--r--   0        0        0     3508 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/plugin.py
+-rw-r--r--   0        0        0     7013 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/plugins/__init__.py
+-rw-r--r--   0        0        0     3633 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/plugins/badwords.py
+-rw-r--r--   0        0        0     3583 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/plugins/copyright_text.py
+-rw-r--r--   0        0        0     3334 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/plugins/copyright_year.py
+-rw-r--r--   0        0        0     3357 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/plugins/creation_date.py
+-rw-r--r--   0        0        0     3400 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/plugins/cve_format.py
+-rw-r--r--   0        0        0     2309 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/plugins/cvss_format.py
+-rw-r--r--   0        0        0     4456 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/plugins/dependencies.py
+-rw-r--r--   0        0        0     7316 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/plugins/dependency_category_order.py
+-rw-r--r--   0        0        0     4137 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/plugins/deprecated_dependency.py
+-rw-r--r--   0        0        0     2568 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/plugins/deprecated_functions.py
+-rw-r--r--   0        0        0     2509 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/plugins/double_end_points.py
+-rw-r--r--   0        0        0     2652 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/plugins/duplicate_oid.py
+-rw-r--r--   0        0        0     3179 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/plugins/duplicated_script_tags.py
+-rw-r--r--   0        0        0     2090 2023-05-09 10:26:14.407202 troubadix-23.5.2/troubadix/plugins/encoding.py
+-rw-r--r--   0        0        0     6014 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/forking_nasl_functions.py
+-rw-r--r--   0        0        0     3401 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/get_kb_on_services.py
+-rw-r--r--   0        0        0     8348 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/grammar.py
+-rw-r--r--   0        0        0     7157 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/http_links_in_tags.py
+-rw-r--r--   0        0        0     4406 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/illegal_characters.py
+-rw-r--r--   0        0        0     2960 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/log_messages.py
+-rw-r--r--   0        0        0     3000 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/malformed_dependencies.py
+-rw-r--r--   0        0        0     5330 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/misplaced_compare_in_if.py
+-rw-r--r--   0        0        0     2411 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/missing_desc_exit.py
+-rw-r--r--   0        0        0     2828 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/missing_tag_solution.py
+-rw-r--r--   0        0        0     2788 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/newlines.py
+-rw-r--r--   0        0        0     2373 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/overlong_script_tags.py
+-rw-r--r--   0        0        0     4185 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/prod_svc_detect_in_vulnvt.py
+-rw-r--r--   0        0        0     3790 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/qod.py
+-rw-r--r--   0        0        0     4043 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/reporting_consistency.py
+-rw-r--r--   0        0        0     3193 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/script_add_preference_type.py
+-rw-r--r--   0        0        0     2512 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/script_calls_empty_values.py
+-rw-r--r--   0        0        0     3137 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/script_calls_recommended.py
+-rw-r--r--   0        0        0     2184 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/script_category.py
+-rw-r--r--   0        0        0     2310 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/script_copyright.py
+-rw-r--r--   0        0        0     4023 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/script_family.py
+-rw-r--r--   0        0        0     1773 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/script_tag_form.py
+-rw-r--r--   0        0        0     2172 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/script_tag_whitespaces.py
+-rw-r--r--   0        0        0     2630 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/script_tags_mandatory.py
+-rw-r--r--   0        0        0     7026 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/script_version_and_last_modification_tags.py
+-rw-r--r--   0        0        0     1848 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/script_xref_form.py
+-rw-r--r--   0        0        0     2875 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/script_xref_url.py
+-rw-r--r--   0        0        0     4708 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/security_messages.py
+-rw-r--r--   0        0        0     3415 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/set_get_kb_calls.py
+-rw-r--r--   0        0        0     5852 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/solution_text.py
+-rw-r--r--   0        0        0     2602 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/solution_type.py
+-rw-r--r--   0        0        0     9638 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/spelling.py
+-rw-r--r--   0        0        0     1319 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/tabs.py
+-rw-r--r--   0        0        0     1733 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/todo_tbd.py
+-rw-r--r--   0        0        0     2049 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/trailing_spaces_tabs.py
+-rw-r--r--   0        0        0     4046 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/using_display.py
+-rw-r--r--   0        0        0    16627 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/valid_oid.py
+-rw-r--r--   0        0        0     3447 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/valid_script_tag_names.py
+-rw-r--r--   0        0        0     3285 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/variable_assigned_in_if.py
+-rw-r--r--   0        0        0     1521 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/vt_file_permissions.py
+-rw-r--r--   0        0        0     2800 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/plugins/vt_placement.py
+-rw-r--r--   0        0        0     9176 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/reporter.py
+-rw-r--r--   0        0        0     2632 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/results.py
+-rw-r--r--   0        0        0     5172 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/runner.py
+-rw-r--r--   0        0        0       22 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/standalone_plugins/__init__.py
+-rw-r--r--   0        0        0     2921 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/standalone_plugins/changed_cves.py
+-rw-r--r--   0        0        0     4074 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/standalone_plugins/changed_oid.py
+-rw-r--r--   0        0        0     5742 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/changed_packages.py
+-rw-r--r--   0        0        0      923 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/marker/__init__.py
+-rw-r--r--   0        0        0     1797 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py
+-rw-r--r--   0        0        0     1486 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/marker/added_release.py
+-rw-r--r--   0        0        0     1124 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py
+-rw-r--r--   0        0        0     1952 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/marker/changed_update.py
+-rw-r--r--   0        0        0     1632 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py
+-rw-r--r--   0        0        0     1278 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/marker/marker.py
+-rw-r--r--   0        0        0     2743 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/package.py
+-rw-r--r--   0        0        0     1028 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/standalone_plugins/common.py
+-rw-r--r--   0        0        0     4616 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/standalone_plugins/last_modification.py
+-rw-r--r--   0        0        0     8463 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/standalone_plugins/no_solution.py
+-rw-r--r--   0        0        0     4263 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/standalone_plugins/version_updated.py
+-rw-r--r--   0        0        0     6045 2023-05-09 10:26:14.411202 troubadix-23.5.2/troubadix/troubadix.py
+-rw-r--r--   0        0        0     4129 1970-01-01 00:00:00.000000 troubadix-23.5.2/PKG-INFO
```

### Comparing `troubadix-23.5.1/LICENSE` & `troubadix-23.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/README.md` & `troubadix-23.5.2/README.md`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/pyproject.toml` & `troubadix-23.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troubadix"
-version = "23.5.1"
+version = "23.5.2"
 description = "A linting and QA check tool for NASL files"
 authors = ["Greenbone <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/greenbone/troubadix"
 homepage = "https://github.com/greenbone/troubadix"
```

### Comparing `troubadix-23.5.1/tests/__init__.py` & `troubadix-23.5.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/helper/__init__.py` & `troubadix-23.5.2/tests/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/helper/test_linguistic_exception_handler.py` & `troubadix-23.5.2/tests/helper/test_linguistic_exception_handler.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/helper/test_patterns.py` & `troubadix-23.5.2/tests/helper/test_patterns.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/__init__.py` & `troubadix-23.5.2/tests/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/fail.nasl` & `troubadix-23.5.2/tests/plugins/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/fail2.nasl` & `troubadix-23.5.2/tests/plugins/fail2.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test.nasl` & `troubadix-23.5.2/tests/plugins/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_badwords.py` & `troubadix-23.5.2/tests/plugins/test_badwords.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_copyright_text.py` & `troubadix-23.5.2/tests/plugins/test_copyright_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_copyright_year.py` & `troubadix-23.5.2/tests/plugins/test_copyright_year.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_creation_date.py` & `troubadix-23.5.2/tests/plugins/test_creation_date.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_cve_format.py` & `troubadix-23.5.2/tests/plugins/test_cve_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_cvss_format.py` & `troubadix-23.5.2/tests/plugins/test_cvss_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_dependencies.py` & `troubadix-23.5.2/tests/plugins/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_dependency_category_order.py` & `troubadix-23.5.2/tests/plugins/test_dependency_category_order.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_deprecated_dependency.py` & `troubadix-23.5.2/tests/plugins/test_deprecated_dependency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_deprecated_functions.py` & `troubadix-23.5.2/tests/plugins/test_deprecated_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_double_end_points.py` & `troubadix-23.5.2/tests/plugins/test_double_end_points.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_duplicate_oid.py` & `troubadix-23.5.2/tests/plugins/test_duplicate_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_duplicated_script_tags.py` & `troubadix-23.5.2/tests/plugins/test_duplicated_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_encoding.py` & `troubadix-23.5.2/tests/plugins/test_encoding.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/fail_bad_new_line.nasl` & `troubadix-23.5.2/tests/plugins/test_files/fail_bad_new_line.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/fail_name_and_copyright_newline.nasl` & `troubadix-23.5.2/tests/plugins/test_files/fail_name_and_copyright_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/fail_name_newline.nasl` & `troubadix-23.5.2/tests/plugins/test_files/fail_name_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/fail_permissions.nasl` & `troubadix-23.5.2/tests/plugins/test_files/fail_permissions.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/fail.nasl` & `troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl` & `troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl` & `troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl` & `troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/runner/fail.nasl` & `troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/runner/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl` & `troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/runner/test.nasl` & `troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/runner/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl` & `troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/test.inc` & `troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/test.inc`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/nasl/21.04/test.nasl` & `troubadix-23.5.2/tests/plugins/test_files/nasl/21.04/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/nasl/warning.nasl` & `troubadix-23.5.2/tests/plugins/test_files/nasl/warning.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/ok_permissions.nasl` & `troubadix-23.5.2/tests/plugins/test_files/ok_permissions.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_files/test_oid.nasl` & `troubadix-23.5.2/tests/plugins/test_files/test_oid.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_forking_nasl_functions.py` & `troubadix-23.5.2/tests/plugins/test_forking_nasl_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_get_kb_on_services.py` & `troubadix-23.5.2/tests/plugins/test_get_kb_on_services.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_grammar.py` & `troubadix-23.5.2/tests/plugins/test_grammar.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_http_links_in_tags.py` & `troubadix-23.5.2/tests/plugins/test_http_links_in_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_illegal_characters.py` & `troubadix-23.5.2/tests/plugins/test_illegal_characters.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_log_messages.py` & `troubadix-23.5.2/tests/plugins/test_log_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_malformed_dependencies.py` & `troubadix-23.5.2/tests/plugins/test_malformed_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_misplaced_compare_in_if.py` & `troubadix-23.5.2/tests/plugins/test_misplaced_compare_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_missing_desc_exit.py` & `troubadix-23.5.2/tests/plugins/test_missing_desc_exit.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_missing_tag_solution.py` & `troubadix-23.5.2/tests/plugins/test_missing_tag_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_newlines.py` & `troubadix-23.5.2/tests/plugins/test_newlines.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_overlong_script_tags.py` & `troubadix-23.5.2/tests/plugins/test_overlong_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_prod_svc_detect_in_vulnvt.py` & `troubadix-23.5.2/tests/plugins/test_prod_svc_detect_in_vulnvt.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_qod.py` & `troubadix-23.5.2/tests/plugins/test_qod.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_reporting_consistency.py` & `troubadix-23.5.2/tests/plugins/test_reporting_consistency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_script_add_preference_type.py` & `troubadix-23.5.2/tests/plugins/test_script_add_preference_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_script_calls_empty_values.py` & `troubadix-23.5.2/tests/plugins/test_script_calls_empty_values.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_script_calls_recommended.py` & `troubadix-23.5.2/tests/plugins/test_script_calls_recommended.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_script_category.py` & `troubadix-23.5.2/tests/plugins/test_script_category.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_script_copyright.py` & `troubadix-23.5.2/tests/plugins/test_script_copyright.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_script_family.py` & `troubadix-23.5.2/tests/plugins/test_script_family.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_script_tag_form.py` & `troubadix-23.5.2/tests/plugins/test_script_tag_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_script_tag_whitespaces.py` & `troubadix-23.5.2/tests/plugins/test_script_xref_form.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,73 +15,73 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from pathlib import Path
 
 from tests.plugins import PluginTestCase
 from troubadix.plugin import LinterError
-from troubadix.plugins.script_tag_whitespaces import CheckScriptTagWhitespaces
+from troubadix.plugins.script_xref_form import CheckScriptXrefForm
 
 
-class CheckScriptTagWhitespacesTestCase(PluginTestCase):
+class CheckScriptXrefFormTestCase(PluginTestCase):
     path = Path("some/file.nasl")
 
     def test_ok(self):
-        content = '  script_tag(name: "foo", value:"bar");\n'
+        content = '  script_xref(name: "foo", value:"bar");\n'
         fake_context = self.create_file_plugin_context(
             nasl_file=self.path, file_content=content
         )
-        plugin = CheckScriptTagWhitespaces(fake_context)
+        plugin = CheckScriptXrefForm(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
     def test_exclude_inc_file(self):
         path = Path("some/file.inc")
         fake_context = self.create_file_plugin_context(nasl_file=path)
-        plugin = CheckScriptTagWhitespaces(fake_context)
+        plugin = CheckScriptXrefForm(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
-    def test_leading_whitespace(self):
-        content = '  script_tag(name: "foo", value:" bar");\n'
+    def test_wrong_name(self):
+        content = '  script_xref(nammmme: "foo", value:"bar");\n'
         fake_context = self.create_file_plugin_context(
             nasl_file=self.path, file_content=content
         )
-        plugin = CheckScriptTagWhitespaces(fake_context)
+        plugin = CheckScriptXrefForm(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 1)
         self.assertIsInstance(results[0], LinterError)
         self.assertEqual(
-            'script_tag(name: "foo", value:" bar");: value contains a leading'
-            " or trailing whitespace character",
+            'script_xref(nammmme: "foo", value:"bar");: does not conform to'
+            ' script_xref(name:"<name>", value:<value>);',
             results[0].message,
         )
 
-    def test_trailing_whitespace(self):
-        content = '  script_tag(name: "foo", value:"bar\n");\n'
+    def test_wrong_value(self):
+        content = '  script_xref(name: "foo", valueeeee:"bar");\n'
         fake_context = self.create_file_plugin_context(
             nasl_file=self.path, file_content=content
         )
-        plugin = CheckScriptTagWhitespaces(fake_context)
+        plugin = CheckScriptXrefForm(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 1)
         self.assertIsInstance(results[0], LinterError)
 
-    def test_trailing_whitespace_newline(self):
-        content = '  script_tag(name: "foo", value:"foo\nbar\n");\n'
+    def test_wrong_missing_parameters(self):
+        content = '  script_xref("foo", "bar");\n'
         fake_context = self.create_file_plugin_context(
             nasl_file=self.path, file_content=content
         )
-        plugin = CheckScriptTagWhitespaces(fake_context)
+        plugin = CheckScriptXrefForm(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 1)
         self.assertIsInstance(results[0], LinterError)
```

### Comparing `troubadix-23.5.1/tests/plugins/test_script_tags_mandatory.py` & `troubadix-23.5.2/tests/plugins/test_script_tags_mandatory.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_script_version_and_last_modification_tags.py` & `troubadix-23.5.2/tests/plugins/test_script_version_and_last_modification_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_script_xref_form.py` & `troubadix-23.5.2/tests/plugins/test_script_xref_url.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,73 +15,49 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from pathlib import Path
 
 from tests.plugins import PluginTestCase
 from troubadix.plugin import LinterError
-from troubadix.plugins.script_xref_form import CheckScriptXrefForm
+from troubadix.plugins.script_xref_url import CheckScriptXrefUrl
 
 
-class CheckScriptXrefFormTestCase(PluginTestCase):
+class CheckScriptXrefUrlTestCase(PluginTestCase):
     path = Path("some/file.nasl")
 
     def test_ok(self):
-        content = '  script_xref(name: "foo", value:"bar");\n'
+        content = '  script_xref(name:"URL", value:"http://www.example.com");\n'
         fake_context = self.create_file_plugin_context(
             nasl_file=self.path, file_content=content
         )
-        plugin = CheckScriptXrefForm(fake_context)
+        plugin = CheckScriptXrefUrl(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
     def test_exclude_inc_file(self):
         path = Path("some/file.inc")
         fake_context = self.create_file_plugin_context(nasl_file=path)
-        plugin = CheckScriptXrefForm(fake_context)
+        plugin = CheckScriptXrefUrl(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
-    def test_wrong_name(self):
-        content = '  script_xref(nammmme: "foo", value:"bar");\n'
+    def test_invalid_url(self):
+        content = '  script_xref(name:"URL", value:"www.example.com");\n'
         fake_context = self.create_file_plugin_context(
             nasl_file=self.path, file_content=content
         )
-        plugin = CheckScriptXrefForm(fake_context)
+        plugin = CheckScriptXrefUrl(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 1)
         self.assertIsInstance(results[0], LinterError)
         self.assertEqual(
-            'script_xref(nammmme: "foo", value:"bar");: does not conform to'
-            ' script_xref(name:"<name>", value:<value>);',
+            'script_xref(name:"URL", value:"www.example.com");: Invalid URL'
+            " value",
             results[0].message,
         )
-
-    def test_wrong_value(self):
-        content = '  script_xref(name: "foo", valueeeee:"bar");\n'
-        fake_context = self.create_file_plugin_context(
-            nasl_file=self.path, file_content=content
-        )
-        plugin = CheckScriptXrefForm(fake_context)
-
-        results = list(plugin.run())
-
-        self.assertEqual(len(results), 1)
-        self.assertIsInstance(results[0], LinterError)
-
-    def test_wrong_missing_parameters(self):
-        content = '  script_xref("foo", "bar");\n'
-        fake_context = self.create_file_plugin_context(
-            nasl_file=self.path, file_content=content
-        )
-        plugin = CheckScriptXrefForm(fake_context)
-
-        results = list(plugin.run())
-
-        self.assertEqual(len(results), 1)
-        self.assertIsInstance(results[0], LinterError)
```

### Comparing `troubadix-23.5.1/tests/plugins/test_script_xref_url.py` & `troubadix-23.5.2/tests/plugins/test_vt_file_permissions.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,51 +13,47 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from pathlib import Path
 
-from tests.plugins import PluginTestCase
 from troubadix.plugin import LinterError
-from troubadix.plugins.script_xref_url import CheckScriptXrefUrl
+from troubadix.plugins.vt_file_permissions import CheckVTFilePermissions
 
+from . import PluginTestCase
 
-class CheckScriptXrefUrlTestCase(PluginTestCase):
-    path = Path("some/file.nasl")
 
+class CheckVTFilePermissionsTestCase(PluginTestCase):
     def test_ok(self):
-        content = '  script_xref(name:"URL", value:"http://www.example.com");\n'
         fake_context = self.create_file_plugin_context(
-            nasl_file=self.path, file_content=content
+            nasl_file=Path(__file__).parent
+            / "test_files"
+            / "ok_permissions.nasl"
         )
-        plugin = CheckScriptXrefUrl(fake_context)
 
-        results = list(plugin.run())
-
-        self.assertEqual(len(results), 0)
-
-    def test_exclude_inc_file(self):
-        path = Path("some/file.inc")
-        fake_context = self.create_file_plugin_context(nasl_file=path)
-        plugin = CheckScriptXrefUrl(fake_context)
+        plugin = CheckVTFilePermissions(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
 
-    def test_invalid_url(self):
-        content = '  script_xref(name:"URL", value:"www.example.com");\n'
+    def test_nok(self):
         fake_context = self.create_file_plugin_context(
-            nasl_file=self.path, file_content=content
+            nasl_file=Path(__file__).parent
+            / "test_files"
+            / "fail_permissions.nasl"
         )
-        plugin = CheckScriptXrefUrl(fake_context)
+
+        plugin = CheckVTFilePermissions(fake_context)
 
         results = list(plugin.run())
 
         self.assertEqual(len(results), 1)
         self.assertIsInstance(results[0], LinterError)
         self.assertEqual(
-            'script_xref(name:"URL", value:"www.example.com");: Invalid URL'
-            " value",
             results[0].message,
+            "VT has invalid file permissions: -rwxr-xr-x.\n"
+            "NASL scripts must not be executable.\n"
+            "Typical file permissions are '644' (-rw-r--r-) "
+            "and `664` (-rw-rw-r-)",
         )
```

### Comparing `troubadix-23.5.1/tests/plugins/test_security_messages.py` & `troubadix-23.5.2/tests/plugins/test_security_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_set_get_kb_calls.py` & `troubadix-23.5.2/tests/plugins/test_set_get_kb_calls.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_solution_text.py` & `troubadix-23.5.2/tests/plugins/test_solution_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_solution_type.py` & `troubadix-23.5.2/tests/plugins/test_solution_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_spelling.py` & `troubadix-23.5.2/tests/plugins/test_spelling.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_tabs.py` & `troubadix-23.5.2/tests/plugins/test_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_todo_tbd.py` & `troubadix-23.5.2/tests/plugins/test_todo_tbd.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_trailing_spaces_tabs.py` & `troubadix-23.5.2/tests/plugins/test_trailing_spaces_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_using_display.py` & `troubadix-23.5.2/tests/plugins/test_using_display.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_valid_oid.py` & `troubadix-23.5.2/tests/plugins/test_valid_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_valid_script_tag_names.py` & `troubadix-23.5.2/tests/plugins/test_valid_script_tag_names.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/plugins/test_vt_file_permissions.py` & `troubadix-23.5.2/troubadix/plugins/script_xref_form.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,49 +11,42 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+import re
 from pathlib import Path
+from typing import Iterator
 
-from troubadix.plugin import LinterError
-from troubadix.plugins.vt_file_permissions import CheckVTFilePermissions
+from troubadix.helper.patterns import get_xref_pattern
+from troubadix.plugin import FileContentPlugin, LinterError, LinterResult
 
-from . import PluginTestCase
 
+class CheckScriptXrefForm(FileContentPlugin):
+    name = "check_script_xref_form"
 
-class CheckVTFilePermissionsTestCase(PluginTestCase):
-    def test_ok(self):
-        fake_context = self.create_file_plugin_context(
-            nasl_file=Path(__file__).parent
-            / "test_files"
-            / "ok_permissions.nasl"
-        )
-
-        plugin = CheckVTFilePermissions(fake_context)
-
-        results = list(plugin.run())
-
-        self.assertEqual(len(results), 0)
-
-    def test_nok(self):
-        fake_context = self.create_file_plugin_context(
-            nasl_file=Path(__file__).parent
-            / "test_files"
-            / "fail_permissions.nasl"
-        )
-
-        plugin = CheckVTFilePermissions(fake_context)
-
-        results = list(plugin.run())
-
-        self.assertEqual(len(results), 1)
-        self.assertIsInstance(results[0], LinterError)
-        self.assertEqual(
-            results[0].message,
-            "VT has invalid file permissions: -rwxr-xr-x.\n"
-            "NASL scripts must not be executable.\n"
-            "Typical file permissions are '644' (-rw-r--r-) "
-            "and `664` (-rw-rw-r-)",
-        )
+    def check_content(
+        self,
+        nasl_file: Path,
+        file_content: str,
+    ) -> Iterator[LinterResult]:
+        """
+        Checks for correct parameters for script_xref calls
+        """
+        if nasl_file.suffix == ".inc":
+            return
+
+        matches = re.finditer(r"script_xref\(.*\);", file_content)
+        if matches:
+            for match in matches:
+                if match:
+                    if not get_xref_pattern(name=r".*", value=r".*").match(
+                        match.group(0)
+                    ):
+                        yield LinterError(
+                            f"{match.group(0)}: does not conform to"
+                            ' script_xref(name:"<name>", value:<value>);',
+                            file=nasl_file,
+                            plugin=self.name,
+                        )
```

### Comparing `troubadix-23.5.1/tests/plugins/test_vt_placement.py` & `troubadix-23.5.2/tests/plugins/test_vt_placement.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/standalone_plugins/__init__.py` & `troubadix-23.5.2/tests/standalone_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/standalone_plugins/changed_packages/__init__.py` & `troubadix-23.5.2/tests/standalone_plugins/changed_packages/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/standalone_plugins/changed_packages/markers/__init__.py` & `troubadix-23.5.2/tests/standalone_plugins/changed_packages/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py` & `troubadix-23.5.2/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/standalone_plugins/changed_packages/markers/test_added_release.py` & `troubadix-23.5.2/tests/standalone_plugins/changed_packages/markers/test_added_release.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py` & `troubadix-23.5.2/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/standalone_plugins/changed_packages/markers/test_changed_update.py` & `troubadix-23.5.2/tests/standalone_plugins/changed_packages/markers/test_changed_update.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py` & `troubadix-23.5.2/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/standalone_plugins/changed_packages/test_changed_packages.py` & `troubadix-23.5.2/tests/standalone_plugins/changed_packages/test_changed_packages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/standalone_plugins/changed_packages/test_package.py` & `troubadix-23.5.2/tests/standalone_plugins/changed_packages/test_package.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/standalone_plugins/test_changed_cves.py` & `troubadix-23.5.2/tests/standalone_plugins/test_changed_cves.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/standalone_plugins/test_changed_oid.py` & `troubadix-23.5.2/tests/standalone_plugins/test_changed_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/standalone_plugins/test_last_modification.py` & `troubadix-23.5.2/tests/standalone_plugins/test_last_modification.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/standalone_plugins/test_no_solution.py` & `troubadix-23.5.2/tests/standalone_plugins/test_no_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/standalone_plugins/test_version_updated.py` & `troubadix-23.5.2/tests/standalone_plugins/test_version_updated.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/test_argparser.py` & `troubadix-23.5.2/tests/test_argparser.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/test_helper.py` & `troubadix-23.5.2/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/test_naslinter.py` & `troubadix-23.5.2/tests/test_naslinter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/test_reporter.py` & `troubadix-23.5.2/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/test_results.py` & `troubadix-23.5.2/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/tests/test_runner.py` & `troubadix-23.5.2/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/__init__.py` & `troubadix-23.5.2/troubadix/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/argparser.py` & `troubadix-23.5.2/troubadix/argparser.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/codespell/codespell.exclude` & `troubadix-23.5.2/troubadix/codespell/codespell.exclude`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/codespell/codespell.ignore` & `troubadix-23.5.2/troubadix/codespell/codespell.ignore`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/helper/__init__.py` & `troubadix-23.5.2/troubadix/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/helper/helper.py` & `troubadix-23.5.2/troubadix/helper/helper.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/helper/linguistic_exception_handler.py` & `troubadix-23.5.2/troubadix/helper/linguistic_exception_handler.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/helper/patterns.py` & `troubadix-23.5.2/troubadix/helper/patterns.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugin.py` & `troubadix-23.5.2/troubadix/plugin.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/__init__.py` & `troubadix-23.5.2/troubadix/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/badwords.py` & `troubadix-23.5.2/troubadix/plugins/badwords.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/copyright_text.py` & `troubadix-23.5.2/troubadix/plugins/copyright_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/copyright_year.py` & `troubadix-23.5.2/troubadix/plugins/copyright_year.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/creation_date.py` & `troubadix-23.5.2/troubadix/plugins/creation_date.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/cve_format.py` & `troubadix-23.5.2/troubadix/plugins/cve_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/cvss_format.py` & `troubadix-23.5.2/troubadix/plugins/cvss_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/dependencies.py` & `troubadix-23.5.2/troubadix/plugins/dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/dependency_category_order.py` & `troubadix-23.5.2/troubadix/plugins/dependency_category_order.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/deprecated_dependency.py` & `troubadix-23.5.2/troubadix/plugins/deprecated_dependency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/deprecated_functions.py` & `troubadix-23.5.2/troubadix/plugins/deprecated_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/double_end_points.py` & `troubadix-23.5.2/troubadix/plugins/double_end_points.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/duplicate_oid.py` & `troubadix-23.5.2/troubadix/plugins/duplicate_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/duplicated_script_tags.py` & `troubadix-23.5.2/troubadix/plugins/duplicated_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/encoding.py` & `troubadix-23.5.2/troubadix/plugins/encoding.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/forking_nasl_functions.py` & `troubadix-23.5.2/troubadix/plugins/forking_nasl_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/get_kb_on_services.py` & `troubadix-23.5.2/troubadix/plugins/get_kb_on_services.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/grammar.py` & `troubadix-23.5.2/troubadix/plugins/grammar.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/http_links_in_tags.py` & `troubadix-23.5.2/troubadix/plugins/http_links_in_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/illegal_characters.py` & `troubadix-23.5.2/troubadix/plugins/illegal_characters.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/log_messages.py` & `troubadix-23.5.2/troubadix/plugins/log_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/malformed_dependencies.py` & `troubadix-23.5.2/troubadix/plugins/malformed_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/misplaced_compare_in_if.py` & `troubadix-23.5.2/troubadix/plugins/misplaced_compare_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/missing_desc_exit.py` & `troubadix-23.5.2/troubadix/plugins/missing_desc_exit.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/missing_tag_solution.py` & `troubadix-23.5.2/troubadix/plugins/missing_tag_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/newlines.py` & `troubadix-23.5.2/troubadix/plugins/newlines.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/overlong_script_tags.py` & `troubadix-23.5.2/troubadix/plugins/overlong_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/prod_svc_detect_in_vulnvt.py` & `troubadix-23.5.2/troubadix/plugins/prod_svc_detect_in_vulnvt.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/qod.py` & `troubadix-23.5.2/troubadix/plugins/qod.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/reporting_consistency.py` & `troubadix-23.5.2/troubadix/plugins/reporting_consistency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/script_add_preference_type.py` & `troubadix-23.5.2/troubadix/plugins/script_add_preference_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/script_calls_empty_values.py` & `troubadix-23.5.2/troubadix/plugins/script_calls_empty_values.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/script_calls_recommended.py` & `troubadix-23.5.2/troubadix/plugins/script_calls_recommended.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/script_category.py` & `troubadix-23.5.2/troubadix/plugins/script_category.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/script_copyright.py` & `troubadix-23.5.2/troubadix/plugins/script_copyright.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/script_family.py` & `troubadix-23.5.2/troubadix/plugins/script_family.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/script_tag_form.py` & `troubadix-23.5.2/troubadix/plugins/script_tag_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/script_tag_whitespaces.py` & `troubadix-23.5.2/troubadix/plugins/script_tag_whitespaces.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,18 +12,23 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import re
+from itertools import chain
 from pathlib import Path
 from typing import Iterator
 
-from troubadix.helper.patterns import _get_tag_pattern
+from troubadix.helper import SpecialScriptTag
+from troubadix.helper.patterns import (
+    _get_special_script_tag_pattern,
+    _get_tag_pattern,
+)
 from troubadix.plugin import FileContentPlugin, LinterError, LinterResult
 
 
 class CheckScriptTagWhitespaces(FileContentPlugin):
     name = "check_script_tag_whitespaces"
 
     def check_content(
@@ -34,18 +39,24 @@
         """
         Checks a given file content if a script tag value contains a leading or
         trailing whitespace character
         """
         if nasl_file.suffix == ".inc":
             return
 
-        matches = _get_tag_pattern(name=r".+?", flags=re.S).finditer(
+        tag_matches = _get_tag_pattern(name=r".+?", flags=re.S).finditer(
             file_content
         )
 
+        name_matches = _get_special_script_tag_pattern(
+            name=SpecialScriptTag.NAME.value
+        ).finditer(file_content)
+
+        matches = chain(tag_matches, name_matches)
+
         for match in matches:
             if re.match(r"^\s+.*", match.group("value")) or re.match(
                 r".*\s+$", match.group("value"), flags=re.S
             ):
                 yield LinterError(
                     f"{match.group(0)}: value contains a leading or"
                     " trailing whitespace character",
```

### Comparing `troubadix-23.5.1/troubadix/plugins/script_tags_mandatory.py` & `troubadix-23.5.2/troubadix/plugins/script_tags_mandatory.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/script_version_and_last_modification_tags.py` & `troubadix-23.5.2/troubadix/plugins/script_version_and_last_modification_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/script_xref_form.py` & `troubadix-23.5.2/troubadix/plugins/todo_tbd.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Greenbone AG
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -13,40 +13,44 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import re
 from pathlib import Path
-from typing import Iterator
+from typing import Iterable, Iterator
 
-from troubadix.helper.patterns import get_xref_pattern
-from troubadix.plugin import FileContentPlugin, LinterError, LinterResult
+from ..helper import is_ignore_file
+from ..plugin import LineContentPlugin, LinterResult, LinterWarning
 
+_IGNORE_FILES = [
+    "gb_openvas",
+    "gb_gsa_",
+    "http_func.inc",
+    "misc_func.inc",
+]
 
-class CheckScriptXrefForm(FileContentPlugin):
-    name = "check_script_xref_form"
 
-    def check_content(
+class CheckTodoTbd(LineContentPlugin):
+    """This step checks if a given VT contains the words TODO, TBD
+    or @todo as a comment.
+    """
+
+    name = "check_todo_tbd"
+
+    def check_lines(
         self,
         nasl_file: Path,
-        file_content: str,
+        lines: Iterable[str],
     ) -> Iterator[LinterResult]:
-        """
-        Checks for correct parameters for script_xref calls
-        """
-        if nasl_file.suffix == ".inc":
+        if is_ignore_file(nasl_file, _IGNORE_FILES):
             return
 
-        matches = re.finditer(r"script_xref\(.*\);", file_content)
-        if matches:
-            for match in matches:
-                if match:
-                    if not get_xref_pattern(name=r".*", value=r".*").match(
-                        match.group(0)
-                    ):
-                        yield LinterError(
-                            f"{match.group(0)}: does not conform to"
-                            ' script_xref(name:"<name>", value:<value>);',
-                            file=nasl_file,
-                            plugin=self.name,
-                        )
+        for index, line in enumerate(lines, start=1):
+            match = re.search("##? *(TODO|TBD|@todo):?", line)
+            if match is not None:
+                yield LinterWarning(
+                    "VT contains #TODO/TBD/@todo keywords.",
+                    file=nasl_file,
+                    plugin=self.name,
+                    line=index,
+                )
```

### Comparing `troubadix-23.5.1/troubadix/plugins/script_xref_url.py` & `troubadix-23.5.2/troubadix/plugins/script_xref_url.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/security_messages.py` & `troubadix-23.5.2/troubadix/plugins/security_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/set_get_kb_calls.py` & `troubadix-23.5.2/troubadix/plugins/set_get_kb_calls.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/solution_text.py` & `troubadix-23.5.2/troubadix/plugins/solution_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/solution_type.py` & `troubadix-23.5.2/troubadix/plugins/solution_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/spelling.py` & `troubadix-23.5.2/troubadix/plugins/spelling.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/tabs.py` & `troubadix-23.5.2/troubadix/plugins/tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/todo_tbd.py` & `troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Greenbone AG
+# Copyright (C) 2023 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,46 +11,24 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import re
-from pathlib import Path
-from typing import Iterable, Iterator
+from typing import List
 
-from ..helper import is_ignore_file
-from ..plugin import LineContentPlugin, LinterResult, LinterWarning
-
-_IGNORE_FILES = [
-    "gb_openvas",
-    "gb_gsa_",
-    "http_func.inc",
-    "misc_func.inc",
-]
-
-
-class CheckTodoTbd(LineContentPlugin):
-    """This step checks if a given VT contains the words TODO, TBD
-    or @todo as a comment.
-    """
-
-    name = "check_todo_tbd"
-
-    def check_lines(
-        self,
-        nasl_file: Path,
-        lines: Iterable[str],
-    ) -> Iterator[LinterResult]:
-        if is_ignore_file(nasl_file, _IGNORE_FILES):
-            return
-
-        for index, line in enumerate(lines, start=1):
-            match = re.search("##? *(TODO|TBD|@todo):?", line)
-            if match is not None:
-                yield LinterWarning(
-                    "VT contains #TODO/TBD/@todo keywords.",
-                    file=nasl_file,
-                    plugin=self.name,
-                    line=index,
-                )
+from troubadix.standalone_plugins.changed_packages.package import (
+    Direction,
+    Package,
+    Reasons,
+)
+
+from .marker import Marker
+
+
+class AddedUdeb(Marker):
+    @staticmethod
+    def mark(new_packages: List[Package]):
+        for package in new_packages:
+            if package.name.endswith("-udeb"):
+                package.reasons[Reasons.ADDED_UDEB] = Direction.ACTIVE
```

### Comparing `troubadix-23.5.1/troubadix/plugins/trailing_spaces_tabs.py` & `troubadix-23.5.2/troubadix/plugins/trailing_spaces_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/using_display.py` & `troubadix-23.5.2/troubadix/plugins/using_display.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/valid_oid.py` & `troubadix-23.5.2/troubadix/plugins/valid_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/valid_script_tag_names.py` & `troubadix-23.5.2/troubadix/plugins/valid_script_tag_names.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/variable_assigned_in_if.py` & `troubadix-23.5.2/troubadix/plugins/variable_assigned_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/vt_file_permissions.py` & `troubadix-23.5.2/troubadix/plugins/vt_file_permissions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/plugins/vt_placement.py` & `troubadix-23.5.2/troubadix/plugins/vt_placement.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/reporter.py` & `troubadix-23.5.2/troubadix/reporter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/results.py` & `troubadix-23.5.2/troubadix/results.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/runner.py` & `troubadix-23.5.2/troubadix/runner.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/standalone_plugins/changed_cves.py` & `troubadix-23.5.2/troubadix/standalone_plugins/changed_cves.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/standalone_plugins/changed_oid.py` & `troubadix-23.5.2/troubadix/standalone_plugins/changed_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/changed_packages.py` & `troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/changed_packages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/marker/__init__.py` & `troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/marker/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py` & `troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/marker/added_release.py` & `troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/marker/added_release.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py` & `troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,13 +22,30 @@
     Package,
     Reasons,
 )
 
 from .marker import Marker
 
 
-class AddedUdeb(Marker):
-    @staticmethod
-    def mark(new_packages: List[Package]):
-        for package in new_packages:
-            if package.name.endswith("-udeb"):
-                package.reasons[Reasons.ADDED_UDEB] = Direction.ACTIVE
+class DroppedArchitecture(Marker):
+    @classmethod
+    def mark(cls, missing_packages: List[Package], new_packages: List[Package]):
+        for package in missing_packages:
+            if not ":" in package.name:
+                continue
+
+            other_package = cls._find_package(
+                Package(
+                    package.name.split(":")[0],
+                    package.version,
+                    package.release,
+                ),
+                new_packages,
+            )
+
+            if not other_package:
+                continue
+
+            package.reasons[Reasons.DROPPED_ARCHITECTURE] = Direction.PASSIVE
+            other_package.reasons[
+                Reasons.DROPPED_ARCHITECTURE
+            ] = Direction.ACTIVE
```

### Comparing `troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/marker/changed_update.py` & `troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/marker/changed_update.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/marker/marker.py` & `troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/marker/marker.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/standalone_plugins/changed_packages/package.py` & `troubadix-23.5.2/troubadix/standalone_plugins/changed_packages/package.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/standalone_plugins/common.py` & `troubadix-23.5.2/troubadix/standalone_plugins/common.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/standalone_plugins/last_modification.py` & `troubadix-23.5.2/troubadix/standalone_plugins/last_modification.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/standalone_plugins/no_solution.py` & `troubadix-23.5.2/troubadix/standalone_plugins/no_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/standalone_plugins/version_updated.py` & `troubadix-23.5.2/troubadix/standalone_plugins/version_updated.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/troubadix/troubadix.py` & `troubadix-23.5.2/troubadix/troubadix.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.5.1/PKG-INFO` & `troubadix-23.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troubadix
-Version: 23.5.1
+Version: 23.5.2
 Summary: A linting and QA check tool for NASL files
 Home-page: https://github.com/greenbone/troubadix
 License: GPL-3.0-or-later
 Author: Greenbone
 Author-email: info@greenbone.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

