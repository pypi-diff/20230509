# Comparing `tmp/bigflow-1.7.0.dev1.tar.gz` & `tmp/bigflow-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigflow-1.7.0.dev1.tar", last modified: Thu Feb 23 16:57:13 2023, max compression
+gzip compressed data, was "bigflow-1.7.1.tar", last modified: Tue May  9 07:24:49 2023, max compression
```

## Comparing `bigflow-1.7.0.dev1.tar` & `bigflow-1.7.1.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.623577 bigflow-1.7.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-02-23 16:57:13.623577 bigflow-1.7.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.611577 bigflow-1.7.0.dev1/bigflow/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.615577 bigflow-1.7.0.dev1/bigflow/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/bigquery/dataset_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/bigquery/dataset_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/bigquery/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/bigquery/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/bigquery/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.615577 bigflow-1.7.0.dev1/bigflow/build/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.615577 bigflow-1.7.0.dev1/bigflow/build/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/build/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/build/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/build/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/build/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/build/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/build/operate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/build/pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/build/reflect.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/build/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    35037 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/dagbuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.615577 bigflow-1.7.0.dev1/bigflow/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/dataflow/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/dataflow/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/dataflow/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/dataflow/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/konfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.615577 bigflow-1.7.0.dev1/bigflow/scaffold/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/infra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.615577 bigflow-1.7.0.dev1/bigflow/scaffold/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.615577 bigflow-1.7.0.dev1/bigflow/scaffold/templates/migrate-11/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/migrate-11/pyproject.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.615577 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/.gitignore.j2
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/deployment_config.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/pyproject.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.619577 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/resources/requirements.in.j2
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/setup.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.619577 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/test/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.619577 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/test/pi_estimator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/test/pi_estimator/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.619577 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.619577 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.619577 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/config.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.619577 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/processing.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/scaffold/templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.619577 bigflow-1.7.0.dev1/bigflow/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/testing/isolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/bigflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.615577 bigflow-1.7.0.dev1/bigflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-02-23 16:57:13.000000 bigflow-1.7.0.dev1/bigflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-02-23 16:57:13.000000 bigflow-1.7.0.dev1/bigflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 16:57:13.000000 bigflow-1.7.0.dev1/bigflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-02-23 16:57:13.000000 bigflow-1.7.0.dev1/bigflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-23 16:57:13.000000 bigflow-1.7.0.dev1/bigflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.619577 bigflow-1.7.0.dev1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/scripts/bf
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/scripts/bigflow
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 16:57:13.623577 bigflow-1.7.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.619577 bigflow-1.7.0.dev1/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.623577 bigflow-1.7.0.dev1/test/buildd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/buildd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.623577 bigflow-1.7.0.dev1/test/buildd/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/buildd/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/buildd/test_dev.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/buildd/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/buildd/test_operate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/buildd/test_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/buildd/test_reflect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/buildd/test_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.623577 bigflow-1.7.0.dev1/test/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.623577 bigflow-1.7.0.dev1/test/cli/cli_logs_duplicated_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/cli/cli_logs_duplicated_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/cli/cli_logs_duplicated_workflows/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.623577 bigflow-1.7.0.dev1/test/cli/cli_logs_log_name_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/cli/cli_logs_log_name_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/cli/cli_logs_log_name_workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.623577 bigflow-1.7.0.dev1/test/cli/cli_logs_regular_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/cli/cli_logs_regular_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/cli/cli_logs_regular_workflows/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    40776 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/cli/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.623577 bigflow-1.7.0.dev1/test/cli/test_module/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/cli/test_module/Unused1.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/cli/test_module/Unused2.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/cli/test_module/Unused3.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/cli/test_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.623577 bigflow-1.7.0.dev1/test/dagbuilder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/dagbuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/dagbuilder/test_dagbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/test_commons.py
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/test_dataflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/test_dataset_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23905 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/test_konfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/test_migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/test_scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.623577 bigflow-1.7.0.dev1/test/test_user_commons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/test_user_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/test_user_commons/test_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/test_user_commons/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/test_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 16:57:13.623577 bigflow-1.7.0.dev1/test/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/testing/nonpure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-02-23 16:56:27.000000 bigflow-1.7.0.dev1/test/testing/test_isolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-05-09 07:23:52.000000 bigflow-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 07:23:52.000000 bigflow-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-09 07:23:52.000000 bigflow-1.7.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-09 07:24:49.684204 bigflow-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-09 07:23:52.000000 bigflow-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.672204 bigflow-1.7.1/bigflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.676204 bigflow-1.7.1/bigflow/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/bigquery/dataset_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/bigquery/dataset_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/bigquery/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/bigquery/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/bigquery/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.676204 bigflow-1.7.1/bigflow/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.676204 bigflow-1.7.1/bigflow/build/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/operate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/reflect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35088 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/dagbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.676204 bigflow-1.7.1/bigflow/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/dataflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/dataflow/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/dataflow/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/dataflow/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/konfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.676204 bigflow-1.7.1/bigflow/scaffold/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/infra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.676204 bigflow-1.7.1/bigflow/scaffold/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.676204 bigflow-1.7.1/bigflow/scaffold/templates/migrate-11/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/migrate-11/pyproject.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/scaffold/templates/new-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/.gitignore.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/deployment_config.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/pyproject.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/scaffold/templates/new-project/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/resources/requirements.in.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/setup.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/scaffold/templates/new-project/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/test/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/scaffold/templates/new-project/test/pi_estimator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/test/pi_estimator/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/config.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/processing.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/testing/isolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.676204 bigflow-1.7.1/bigflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-09 07:24:49.000000 bigflow-1.7.1/bigflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-09 07:24:49.000000 bigflow-1.7.1/bigflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:24:49.000000 bigflow-1.7.1/bigflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-09 07:24:49.000000 bigflow-1.7.1/bigflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 07:24:49.000000 bigflow-1.7.1/bigflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-09 07:23:52.000000 bigflow-1.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-09 07:23:52.000000 bigflow-1.7.1/scripts/bf
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-09 07:23:52.000000 bigflow-1.7.1/scripts/bigflow
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 07:24:49.684204 bigflow-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-09 07:23:52.000000 bigflow-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/buildd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/buildd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/buildd/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/buildd/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/buildd/test_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/buildd/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/buildd/test_operate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/buildd/test_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/buildd/test_reflect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/buildd/test_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/cli/cli_logs_duplicated_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/cli_logs_duplicated_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/cli_logs_duplicated_workflows/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/cli/cli_logs_log_name_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/cli_logs_log_name_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/cli_logs_log_name_workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/cli/cli_logs_regular_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/cli_logs_regular_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/cli_logs_regular_workflows/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41823 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/cli/test_module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/test_module/Unused1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/test_module/Unused2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/test_module/Unused3.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/test_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/dagbuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/dagbuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/dagbuilder/test_dagbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_dataset_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23905 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_konfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/test_user_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_user_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_user_commons/test_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_user_commons/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/testing/nonpure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/testing/test_isolate.py
```

### Comparing `bigflow-1.7.0.dev1/LICENSE` & `bigflow-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/NOTICE` & `bigflow-1.7.1/NOTICE`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/PKG-INFO` & `bigflow-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigflow
-Version: 1.7.0.dev1
+Version: 1.7.1
 Summary: BigQuery client wrapper with clean API
 Home-page: https://github.com/allegro/bigflow
 Author: Pogranicze
 Author-email: pogranicze-team@allegro.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -58,15 +58,15 @@
 Start from installing BigFlow on your local machine.
 Next, go through the BigFlow [tutorial](./docs/tutorial.md).
 
 ## Installing BigFlow
 
 **Prerequisites**. Before you start, make sure you have the following software installed:
 
-1. [Python](https://www.python.org/downloads/) >= 3.7
+1. [Python](https://www.python.org/downloads/) = 3.8
 2. [Google Cloud SDK](https://cloud.google.com/sdk/docs/downloads-interactive)
 3. [Docker Engine](https://docs.docker.com/engine/install/)
 
 You can install the `bigflow` package globally, but we recommend
 installing it locally with `venv`, in your project's folder:
 
 ```bash
```

### Comparing `bigflow-1.7.0.dev1/README.md` & `bigflow-1.7.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 Start from installing BigFlow on your local machine.
 Next, go through the BigFlow [tutorial](./docs/tutorial.md).
 
 ## Installing BigFlow
 
 **Prerequisites**. Before you start, make sure you have the following software installed:
 
-1. [Python](https://www.python.org/downloads/) >= 3.7
+1. [Python](https://www.python.org/downloads/) = 3.8
 2. [Google Cloud SDK](https://cloud.google.com/sdk/docs/downloads-interactive)
 3. [Docker Engine](https://docs.docker.com/engine/install/)
 
 You can install the `bigflow` package globally, but we recommend
 installing it locally with `venv`, in your project's folder:
 
 ```bash
```

### Comparing `bigflow-1.7.0.dev1/bigflow/__init__.py` & `bigflow-1.7.1/bigflow/__init__.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/bigquery/__init__.py` & `bigflow-1.7.1/bigflow/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/bigquery/dataset_configuration.py` & `bigflow-1.7.1/bigflow/bigquery/dataset_configuration.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/bigquery/dataset_manager.py` & `bigflow-1.7.1/bigflow/bigquery/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/bigquery/interactive.py` & `bigflow-1.7.1/bigflow/bigquery/interactive.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/bigquery/interface.py` & `bigflow-1.7.1/bigflow/bigquery/interface.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/bigquery/job.py` & `bigflow-1.7.1/bigflow/bigquery/job.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/build/dev.py` & `bigflow-1.7.1/bigflow/build/dev.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/build/dist.py` & `bigflow-1.7.1/bigflow/build/dist.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/build/legacy.py` & `bigflow-1.7.1/bigflow/build/legacy.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/build/operate.py` & `bigflow-1.7.1/bigflow/build/operate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/build/pip.py` & `bigflow-1.7.1/bigflow/build/pip.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/build/reflect.py` & `bigflow-1.7.1/bigflow/build/reflect.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/build/spec.py` & `bigflow-1.7.1/bigflow/build/spec.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/cli.py` & `bigflow-1.7.1/bigflow/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,16 @@
     _create_start_project_parser(subparsers)
     _create_logs_parser(subparsers)
 
     _create_build_requirements_parser(subparsers)
 
     _create_codegen_parser(subparsers)
 
-    return parser.parse_args(args)
+    bigflow_only_args = parser.parse_known_args(args)[0]
+    return bigflow_only_args
 
 
 def _create_logs_parser(subparsers):
     subparsers.add_parser('logs', description='Returns a link leading to a workflow logs in GCP Logging.')
 
 
 def _create_start_project_parser(subparsers):
```

### Comparing `bigflow-1.7.0.dev1/bigflow/commons.py` & `bigflow-1.7.1/bigflow/commons.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/configuration.py` & `bigflow-1.7.1/bigflow/configuration.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/dagbuilder.py` & `bigflow-1.7.1/bigflow/dagbuilder.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/dataflow/io.py` & `bigflow-1.7.1/bigflow/dataflow/io.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/dataflow/job.py` & `bigflow-1.7.1/bigflow/dataflow/job.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/dataflow/ml.py` & `bigflow-1.7.1/bigflow/dataflow/ml.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/dataflow/options.py` & `bigflow-1.7.1/bigflow/dataflow/options.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/deploy.py` & `bigflow-1.7.1/bigflow/deploy.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/konfig.py` & `bigflow-1.7.1/bigflow/konfig.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/migrate.py` & `bigflow-1.7.1/bigflow/migrate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/resources.py` & `bigflow-1.7.1/bigflow/resources.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/scaffold/infra.py` & `bigflow-1.7.1/bigflow/scaffold/infra.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/scaffold/scaffold.py` & `bigflow-1.7.1/bigflow/scaffold/scaffold.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/scaffold/templates/README.txt` & `bigflow-1.7.1/bigflow/scaffold/templates/README.txt`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/.gitignore.j2` & `bigflow-1.7.1/bigflow/scaffold/templates/new-project/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/Dockerfile` & `bigflow-1.7.1/bigflow/scaffold/templates/new-project/Dockerfile`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/README.md` & `bigflow-1.7.1/bigflow/scaffold/templates/new-project/README.md`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/deployment_config.py.j2` & `bigflow-1.7.1/bigflow/scaffold/templates/new-project/deployment_config.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2` & `bigflow-1.7.1/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2` & `bigflow-1.7.1/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2` & `bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2` & `bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2` & `bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2` & `bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2` & `bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/scaffold/templating.py` & `bigflow-1.7.1/bigflow/scaffold/templating.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/testing/isolate.py` & `bigflow-1.7.1/bigflow/testing/isolate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/version.py` & `bigflow-1.7.1/bigflow/version.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow/workflow.py` & `bigflow-1.7.1/bigflow/workflow.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow.egg-info/PKG-INFO` & `bigflow-1.7.1/bigflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigflow
-Version: 1.7.0.dev1
+Version: 1.7.1
 Summary: BigQuery client wrapper with clean API
 Home-page: https://github.com/allegro/bigflow
 Author: Pogranicze
 Author-email: pogranicze-team@allegro.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -58,15 +58,15 @@
 Start from installing BigFlow on your local machine.
 Next, go through the BigFlow [tutorial](./docs/tutorial.md).
 
 ## Installing BigFlow
 
 **Prerequisites**. Before you start, make sure you have the following software installed:
 
-1. [Python](https://www.python.org/downloads/) >= 3.7
+1. [Python](https://www.python.org/downloads/) = 3.8
 2. [Google Cloud SDK](https://cloud.google.com/sdk/docs/downloads-interactive)
 3. [Docker Engine](https://docs.docker.com/engine/install/)
 
 You can install the `bigflow` package globally, but we recommend
 installing it locally with `venv`, in your project's folder:
 
 ```bash
```

### Comparing `bigflow-1.7.0.dev1/bigflow.egg-info/SOURCES.txt` & `bigflow-1.7.1/bigflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/bigflow.egg-info/requires.txt` & `bigflow-1.7.1/bigflow.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -61,8 +61,8 @@
 [bigquery]
 google-cloud-bigquery<4,>=1.6
 db-dtypes>=1.0.5
 pandas<2,>=0.25
 six<2,>=1.14
 
 [dataflow]
-apache-beam[gcp]<2.44,>=2.24
+apache-beam[gcp]<2.46,>=2.24
```

### Comparing `bigflow-1.7.0.dev1/setup.py` & `bigflow-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/buildd/test_dev.py` & `bigflow-1.7.1/test/buildd/test_dev.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/buildd/test_dist.py` & `bigflow-1.7.1/test/buildd/test_dist.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/buildd/test_operate.py` & `bigflow-1.7.1/test/buildd/test_operate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/buildd/test_pip.py` & `bigflow-1.7.1/test/buildd/test_pip.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/buildd/test_reflect.py` & `bigflow-1.7.1/test/buildd/test_reflect.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/buildd/test_spec.py` & `bigflow-1.7.1/test/buildd/test_spec.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/cli/test_cli.py` & `bigflow-1.7.1/test/cli/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from bigflow.deploy import AuthorizationType
 
 from bigflow.testing.isolate import ForkIsolateMixin
 from bigflow.cli import *
 from bigflow.cli import _ConsoleStreamLogHandler
 
 from test import mixins
+from test.cli.test_module.Unused1 import PARAM_REQUIRED_BY_JOB
 
 TESTS_DIR = Path(__file__).parent
 
 
 class CliTestCase(
     mixins.PrototypedDirMixin,
     ForkIsolateMixin,
@@ -107,15 +108,15 @@
     def test_should_walk_through_all_workflows_inside_package_tree(self):
         # when
         res = walk_workflows(TEST_MODULE_PATH)
 
         # then
         res = sorted(res, key=lambda r: r.workflow_id)
 
-        self.assertEqual(5, len(res))
+        self.assertEqual(6, len(res))
         self.assertEqual('ID_1', res[0].workflow_id)
         self.assertEqual('@once', res[0].schedule_interval)
         self.assertEqual('ID_2', res[1].workflow_id)
         self.assertNotEqual('@once', res[1].schedule_interval)
 
     def test_should_find_existing_workflow(self):
         # when
@@ -238,14 +239,28 @@
         # when
         cli_run(root_package, full_job_id="ID_3.J_ID_3")
         cli_run(root_package, full_job_id="ID_3.J_ID_3")
 
         # then
         self.assert_started_jobs(['J_ID_3', 'J_ID_3'])
 
+    @mock.patch('bigflow.cli.find_root_package')
+    def test_should_run_workflow_with_additional_args(self, find_package_mock):
+        # given
+        root_package = TESTS_DIR / "test_module"
+        find_package_mock.return_value = root_package
+        command = ["run", "--workflow", "ID_6", "--project-package", str(root_package), PARAM_REQUIRED_BY_JOB, "param"]
+        sys.argv = command  # simulates running from command line
+
+        # when
+        cli(command)
+
+        # then the additional args should be passed to the job
+        self.assert_started_jobs(['J_ID_7'])
+
     def test_should_read_project_package_if_set(self):
         # given
         args = lambda: None
         expected = "ROOT_VALUE"
         args.project_package = expected
 
         # when
@@ -656,14 +671,20 @@
         # when
         cli(['build-dags'])
 
         # then
         _cli_build_dags_mock.assert_called_with(Namespace(operation='build-dags', start_time=None, workflow=None, verbose=False))
 
         # when
+        cli(['build-dags', '--additional-param', 'param'])
+
+        # then ignore additional params
+        _cli_build_dags_mock.assert_called_with(Namespace(operation='build-dags', start_time=None, workflow=None, verbose=False))
+
+        # when
         cli(['build-dags', '-t', '2020-01-01 00:00:00'])
 
         # then
         _cli_build_dags_mock.assert_called_with(Namespace(operation='build-dags', start_time='2020-01-01 00:00:00', workflow=None, verbose=False))
 
         # when
         cli(['build-dags', '-w', 'some_workflow'])
@@ -914,14 +935,20 @@
             vault_endpoint_verify=True,
         )
 
         # then
         _cli_build_mock.assert_called_with(args)
 
         # when
+        cli(['build', '--additional-param', 'param'])
+
+        # then ignore unknown params
+        _cli_build_mock.assert_called_with(args)
+
+        # when
         cli(['build', '--start-time', '2020-01-01 00:00:00'])
 
         # then
         args.start_time = '2020-01-01 00:00:00'
         _cli_build_mock.assert_called_with(args)
 
         # when
```

### Comparing `bigflow-1.7.0.dev1/test/cli/test_module/Unused1.py` & `bigflow-1.7.1/test/cli/test_module/Unused1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import sys
+
 import bigflow as bf
 from bigflow.bigquery.interactive import InteractiveDatasetManager as Dataset
 
 PROJECT_ID = 'put-you-project-id-here'
+PARAM_REQUIRED_BY_JOB = '--param-required-by-job'
 
 dataset = Dataset(
     project_id=PROJECT_ID,
     dataset_name='bigflow_cheatsheet',
     external_tables={
         '311_requests': '{}.external_data.311_requests'.format(PROJECT_ID)
     },
@@ -21,13 +24,20 @@
 class ExampleJob:
     def __init__(self, id):
         self.id = id
 
     def execute(self, context):
         started_jobs.append(self.id)
 
+class ExampleJobWithParams:
+    def __init__(self, id):
+        self.id = id
+
+    def execute(self, context):
+        sys.argv.index('--param-required-by-job')
+        started_jobs.append(self.id)
+
 workflow_1 = bf.Workflow(workflow_id="ID_1", definition=[wait_for_requests.to_job(), wait_for_requests.to_job()], schedule_interval="@once")
 workflow_2 = bf.Workflow(workflow_id="ID_2", definition=[wait_for_requests.to_job()])
 workflow_3 = bf.Workflow(workflow_id="ID_3", definition=[ExampleJob("J_ID_3"), ExampleJob("J_ID_4")])
 workflow_4 = bf.Workflow(workflow_id="ID_4", definition=[ExampleJob("J_ID_5")])
-
-print("AAA")
+workflow_5 = bf.Workflow(workflow_id="ID_6", definition=[ExampleJobWithParams("J_ID_7")])
```

### Comparing `bigflow-1.7.0.dev1/test/dagbuilder/test_dagbuilder.py` & `bigflow-1.7.1/test/dagbuilder/test_dagbuilder.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/test_commons.py` & `bigflow-1.7.1/test/test_commons.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/test_configuration.py` & `bigflow-1.7.1/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/test_dataflow.py` & `bigflow-1.7.1/test/test_dataflow.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/test_deploy.py` & `bigflow-1.7.1/test/test_deploy.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/test_interactive.py` & `bigflow-1.7.1/test/test_interactive.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/test_job.py` & `bigflow-1.7.1/test/test_job.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/test_konfig.py` & `bigflow-1.7.1/test/test_konfig.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/test_migrate.py` & `bigflow-1.7.1/test/test_migrate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/test_resources.py` & `bigflow-1.7.1/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/test_scaffold.py` & `bigflow-1.7.1/test/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/test_user_commons/test_labels.py` & `bigflow-1.7.1/test/test_user_commons/test_labels.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/test_user_commons/test_sensor.py` & `bigflow-1.7.1/test/test_user_commons/test_sensor.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/test_version.py` & `bigflow-1.7.1/test/test_version.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/test_workflow.py` & `bigflow-1.7.1/test/test_workflow.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.0.dev1/test/testing/test_isolate.py` & `bigflow-1.7.1/test/testing/test_isolate.py`

 * *Files identical despite different names*

