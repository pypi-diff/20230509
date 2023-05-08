# Comparing `tmp/dkist-processing-common-2.6.0.tar.gz` & `tmp/dkist-processing-common-2.6.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-2.6.0.tar", last modified: Fri May  5 17:43:19 2023, max compression
+gzip compressed data, was "dkist-processing-common-2.6.1rc1.tar", last modified: Mon May  8 23:00:27 2023, max compression
```

## Comparing `dkist-processing-common-2.6.0.tar` & `dkist-processing-common-2.6.1rc1.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 17:43:19.110773 dkist-processing-common-2.6.0/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    13093 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4324 2023-05-05 17:43:19.110773 dkist-processing-common-2.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 17:43:19.098773 dkist-processing-common-2.6.0/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 17:43:19.098773 dkist-processing-common-2.6.0/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 17:43:19.102773 dkist-processing-common-2.6.0/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 17:43:19.102773 dkist-processing-common-2.6.0/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6987 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 17:43:19.102773 dkist-processing-common-2.6.0/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4769 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4192 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/models/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3408 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     7365 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 17:43:19.102773 dkist-processing-common-2.6.0/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     5720 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/parsers/unique_bud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 17:43:19.106773 dkist-processing-common-2.6.0/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11470 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     8152 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10675 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 17:43:19.106773 dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2459 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/fits.py
--rw-rw-rw-   0 root         (0) root         (0)     6718 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13155 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 17:43:19.106773 dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8226 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47886 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     7123 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)    18550 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 17:43:19.110773 dkist-processing-common-2.6.0/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24490 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     8808 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)    12961 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_fits_flowers.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_l1_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6276 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10499 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36040 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11128 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    14952 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 17:43:19.102773 dkist-processing-common-2.6.0/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4324 2023-05-05 17:43:19.000000 dkist-processing-common-2.6.0/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4188 2023-05-05 17:43:19.000000 dkist-processing-common-2.6.0/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-05 17:43:19.000000 dkist-processing-common-2.6.0/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-05-05 17:43:19.000000 dkist-processing-common-2.6.0/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-05 17:43:19.000000 dkist-processing-common-2.6.0/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 17:43:19.110773 dkist-processing-common-2.6.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 17:43:19.110773 dkist-processing-common-2.6.0/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-05-05 17:43:19.110773 dkist-processing-common-2.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-05 17:43:12.000000 dkist-processing-common-2.6.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 23:00:27.910485 dkist-processing-common-2.6.1rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13093 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-05-08 23:00:27.910485 dkist-processing-common-2.6.1rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 23:00:27.898486 dkist-processing-common-2.6.1rc1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/changelog/137.misc.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 23:00:27.898486 dkist-processing-common-2.6.1rc1/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 23:00:27.898486 dkist-processing-common-2.6.1rc1/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 23:00:27.898486 dkist-processing-common-2.6.1rc1/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6987 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 23:00:27.902485 dkist-processing-common-2.6.1rc1/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4769 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/models/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     7365 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 23:00:27.902485 dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     5720 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/unique_bud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 23:00:27.902485 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11470 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     8152 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10675 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 23:00:27.906485 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2459 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     6718 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13155 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 23:00:27.906485 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8226 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47886 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     8002 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8859 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    18550 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 23:00:27.910485 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24490 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     8808 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    12961 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_fits_flowers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_l1_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6276 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10502 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36040 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11128 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14952 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 23:00:27.898486 dkist-processing-common-2.6.1rc1/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-05-08 23:00:27.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4211 2023-05-08 23:00:27.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-08 23:00:27.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-05-08 23:00:27.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-08 23:00:27.000000 dkist-processing-common-2.6.1rc1/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 23:00:27.910485 dkist-processing-common-2.6.1rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 23:00:27.910485 dkist-processing-common-2.6.1rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-05-08 23:00:27.910485 dkist-processing-common-2.6.1rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-08 23:00:20.000000 dkist-processing-common-2.6.1rc1/setup.py
```

### Comparing `dkist-processing-common-2.6.0/.gitignore` & `dkist-processing-common-2.6.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/.pre-commit-config.yaml` & `dkist-processing-common-2.6.1rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/CHANGELOG.rst` & `dkist-processing-common-2.6.1rc1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/PKG-INFO` & `dkist-processing-common-2.6.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 2.6.0
+Version: 2.6.1rc1
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-2.6.0/README.rst` & `dkist-processing-common-2.6.1rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/bitbucket-pipelines.yml` & `dkist-processing-common-2.6.1rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/check_changelog_updated.sh` & `dkist-processing-common-2.6.1rc1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/_util/config.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/_util/constants.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/_util/tags.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/manual.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/models/constants.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/models/graphql.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/models/json_encoder.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/models/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/models/message.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/models/parameters.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/models/quality.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/models/tags.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/parsers/time.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tasks/base.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/fits.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,72 +18,80 @@
 that makes the rest of the pipeline easy to write.
 
 In other words, we can find exactly the frame we need (tags) and, once we have it, we never need to look
 at a different frame to get information (constants).
 """
 import json
 import logging
+from abc import ABC
+from abc import abstractmethod
 from typing import TypeVar
 
 from dkist_processing_common.models.constants import BudName
 from dkist_processing_common.models.flower_pot import FlowerPot
 from dkist_processing_common.models.flower_pot import Stem
 from dkist_processing_common.models.flower_pot import Thorn
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.parsers.experiment_id_bud import ContributingExperimentIdsBud
 from dkist_processing_common.parsers.experiment_id_bud import ExperimentIdBud
-from dkist_processing_common.parsers.l0_fits_access import L0FitsAccess
 from dkist_processing_common.parsers.proposal_id_bud import ContributingProposalIdsBud
 from dkist_processing_common.parsers.proposal_id_bud import ProposalIdBud
 from dkist_processing_common.parsers.time import AverageCadenceBud
 from dkist_processing_common.parsers.time import MaximumCadenceBud
 from dkist_processing_common.parsers.time import MinimumCadenceBud
 from dkist_processing_common.parsers.time import TaskExposureTimesBud
 from dkist_processing_common.parsers.time import VarianceCadenceBud
 from dkist_processing_common.parsers.unique_bud import UniqueBud
 from dkist_processing_common.tasks.base import WorkflowTaskBase
 from dkist_processing_common.tasks.mixin.fits import FitsDataMixin
-from dkist_processing_common.tasks.mixin.input_dataset import InputDatasetMixin
 
 
-__all__ = ["ParseL0InputData"]
+__all__ = ["ParseL0InputDataBase", "ParseDataBase", "DEFAULT_CONSTANT_FLOWERS"]
 
 
 logger = logging.getLogger(__name__)
 S = TypeVar("S", bound=Stem)
 
 
-class ParseL0InputData(WorkflowTaskBase, InputDatasetMixin, FitsDataMixin):
-    """Common task to populate pipeline Constants and group files with tags by scanning headers."""
+DEFAULT_CONSTANT_FLOWERS = [
+    UniqueBud(constant_name=BudName.instrument.value, metadata_key="instrument"),
+    ProposalIdBud(),
+    ContributingProposalIdsBud(),
+    ExperimentIdBud(),
+    ContributingExperimentIdsBud(),
+    AverageCadenceBud(),
+    MaximumCadenceBud(),
+    MinimumCadenceBud(),
+    VarianceCadenceBud(),
+    TaskExposureTimesBud(stem_name=BudName.dark_exposure_times.value, ip_task_type="dark"),
+]
+
+
+class ParseDataBase(WorkflowTaskBase, FitsDataMixin, ABC):
+    """Base class for tasks which need to parse some already tagged data and set constants and/or add additional tags to them."""
 
     @property
-    def constant_flowers(self) -> list[S]:
+    @abstractmethod
+    def constant_buds(self) -> list[S]:
         """Define the constants used."""
-        return [
-            UniqueBud(constant_name=BudName.instrument.value, metadata_key="instrument"),
-            ProposalIdBud(),
-            ContributingProposalIdsBud(),
-            ExperimentIdBud(),
-            ContributingExperimentIdsBud(),
-            AverageCadenceBud(),
-            MaximumCadenceBud(),
-            MinimumCadenceBud(),
-            VarianceCadenceBud(),
-            TaskExposureTimesBud(stem_name=BudName.dark_exposure_times.value, ip_task_type="dark"),
-        ]
 
     @property
+    @abstractmethod
     def tag_flowers(self) -> list[S]:
         """Define the Tags to apply."""
-        return []
 
     @property
+    @abstractmethod
     def fits_parsing_class(self):
         """Class used to parse the input data."""
-        return L0FitsAccess
+
+    @property
+    @abstractmethod
+    def tags_for_input_frames(self) -> list[Tag]:
+        """Define the tags for the data that will be parsed."""
 
     def run(self) -> None:
         """Run method for this task."""
         with self.apm_task_step("Check that input frames exist"):
             self.check_input_frames()
 
         with self.apm_task_step("Ingest all input files"):
@@ -96,34 +104,34 @@
             self.tag_petals(tag_pot)
 
     def make_flower_pots(self) -> tuple[FlowerPot, FlowerPot]:
         """Ingest all headers."""
         tag_pot = FlowerPot()
         constant_pot = FlowerPot()
         tag_pot.flowers += self.tag_flowers
-        constant_pot.flowers += self.constant_flowers
+        constant_pot.flowers += self.constant_buds
 
         for fits_obj in self.input_frames:
             filepath = fits_obj.name
             tag_pot.add_dirt(filepath, fits_obj)
             constant_pot.add_dirt(filepath, fits_obj)
 
         return tag_pot, constant_pot
 
     @property
     def input_frames(self):
         """Return a fits access generator containing the input fits objects."""
         return self.fits_data_read_fits_access(
-            tags=[Tag.input(), Tag.frame()], cls=self.fits_parsing_class
+            tags=self.tags_for_input_frames, cls=self.fits_parsing_class
         )
 
     def check_input_frames(self):
         """Make sure that at least one tagged frame exists before doing anything else."""
-        if self.scratch.count_all(tags=[Tag.input(), Tag.frame()]) == 0:
-            raise ValueError("No frames were tagged with INPUT and FRAME")
+        if self.scratch.count_all(tags=self.tags_for_input_frames) == 0:
+            raise ValueError(f"No frames were tagged with {self.tags_for_input_frames}")
 
     def update_constants(self, constant_pot: FlowerPot):
         """
         Update pipeline Constants.
 
         Parameters
         ----------
@@ -167,7 +175,34 @@
         for flower in tag_pot:
             with self.apm_processing_step(f"Applying {flower.stem_name} tag to files"):
                 logger.info(f"Applying {flower.stem_name} tag to files")
                 for petal in flower.petals:
                     tag = Tag.format_tag(flower.stem_name, petal.value)
                     for path in petal.keys:
                         self.tag(path, tag)
+
+
+class ParseL0InputDataBase(ParseDataBase, ABC):
+    """
+    Common task to populate pipeline Constants and group files with tags by scanning headers.
+
+    A minimum of configuration is needed to define the fits_parsing_class. e.g.
+    >>> class ParseL0VispInputData(ParseL0InputDataBase):
+    >>>     @property
+    >>>     def fits_parsing_class(self):
+    >>>         return VispL0FitsAccess
+    """
+
+    @property
+    def constant_buds(self) -> list[S]:
+        """Define the constants used."""
+        return DEFAULT_CONSTANT_FLOWERS
+
+    @property
+    def tag_flowers(self) -> list[S]:
+        """Define the Tags to apply."""
+        return []
+
+    @property
+    def tags_for_input_frames(self) -> list[Tag]:
+        """Define the tags for the data that will be parsed."""
+        return [Tag.input(), Tag.frame()]
```

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_fits_flowers.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_fits_flowers.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_l1_output_data_base.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_l1_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from dkist_processing_common.models.flower_pot import Thorn
 from dkist_processing_common.models.tags import StemName
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.parsers.single_value_single_key_flower import (
     SingleValueSingleKeyFlower,
 )
 from dkist_processing_common.parsers.unique_bud import UniqueBud
-from dkist_processing_common.tasks.parse_l0_input_data import ParseL0InputData
+from dkist_processing_common.tasks.parse_l0_input_data import ParseL0InputDataBase
 
 
 class VispHeaders(Spec122Dataset):
     def __init__(
         self,
         num_mod: int,
         num_files_per_mod: int,
@@ -146,21 +146,21 @@
     return [PickyBud(stem_name="PICKY_BUD")]
 
 
 @pytest.fixture(scope="function")
 def parse_inputs_task(
     tmp_path, visp_flowers, visp_buds, empty_flowers, empty_buds, picky_buds, recipe_run_id
 ):
-    class TaskClass(ParseL0InputData):
+    class TaskClass(ParseL0InputDataBase):
         @property
         def tag_flowers(self):
             return visp_flowers + empty_flowers
 
         @property
-        def constant_flowers(self):
+        def constant_buds(self):
             return visp_buds + empty_buds + picky_buds
 
         @property
         def fits_parsing_class(self):
             return ViSPFitsAccess
 
         def run(self):
@@ -193,22 +193,22 @@
         yield task
         task.scratch.purge()
         task.constants._purge()
 
 
 @pytest.fixture()
 def visp_parse_inputs_task(tmp_path, visp_flowers, visp_buds, recipe_run_id):
-    class TaskClass(ParseL0InputData):
+    class TaskClass(ParseL0InputDataBase):
         @property
         def tag_flowers(self):
             return super().tag_flowers + visp_flowers
 
         @property
-        def constant_flowers(self):
-            return super().constant_flowers + visp_buds
+        def constant_buds(self):
+            return super().constant_buds + visp_buds
 
         @property
         def fits_parsing_class(self):
             return ViSPFitsAccess
 
         def run(self):
             pass
```

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-2.6.1rc1/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-2.6.1rc1/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 2.6.0
+Version: 2.6.1rc1
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-2.6.1rc1/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
+changelog/137.misc.rst
 dkist_processing_common/__init__.py
 dkist_processing_common/manual.py
 dkist_processing_common.egg-info/PKG-INFO
 dkist_processing_common.egg-info/SOURCES.txt
 dkist_processing_common.egg-info/dependency_links.txt
 dkist_processing_common.egg-info/requires.txt
 dkist_processing_common.egg-info/top_level.txt
```

### Comparing `dkist-processing-common-2.6.0/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-2.6.1rc1/dkist_processing_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/docs/Makefile` & `dkist-processing-common-2.6.1rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/docs/conf.py` & `dkist-processing-common-2.6.1rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/docs/make.bat` & `dkist-processing-common-2.6.1rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/licenses/LICENSE.rst` & `dkist-processing-common-2.6.1rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/pyproject.toml` & `dkist-processing-common-2.6.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.0/setup.cfg` & `dkist-processing-common-2.6.1rc1/setup.cfg`

 * *Files identical despite different names*

