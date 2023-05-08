# Comparing `tmp/sqlmesh-0.7.1.dev33.tar.gz` & `tmp/sqlmesh-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmesh-0.7.1.dev33.tar", last modified: Fri May  5 17:14:06 2023, max compression
+gzip compressed data, was "sqlmesh-0.8.0.tar", last modified: Mon May  8 23:29:21 2023, max compression
```

## Comparing `sqlmesh-0.7.1.dev33.tar` & `sqlmesh-0.8.0.tar`

### file list

```diff
@@ -1,745 +1,774 @@
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.444072 sqlmesh-0.7.1.dev33/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.034505 sqlmesh-0.7.1.dev33/.circleci/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1872 2023-04-17 00:43:26.000000 sqlmesh-0.7.1.dev33/.circleci/config.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4515 2023-05-04 16:23:36.000000 sqlmesh-0.7.1.dev33/.circleci/continue_config.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)       66 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/.dockerignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2152 2023-04-17 00:43:26.000000 sqlmesh-0.7.1.dev33/.gitignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1900 2023-03-27 22:28:21.000000 sqlmesh-0.7.1.dev33/.pre-commit-config.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      234 2023-03-31 20:18:29.000000 sqlmesh-0.7.1.dev33/.readthedocs.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      135 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/Dockerfile.api
--rw-r--r--   0 eakmanrq   (501) staff       (20)      383 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/Dockerfile.app
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11346 2023-03-21 00:57:17.000000 sqlmesh-0.7.1.dev33/LICENSE
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1855 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/Makefile
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2187 2023-05-05 17:14:06.444245 sqlmesh-0.7.1.dev33/PKG-INFO
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1192 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/README.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1188 2023-05-04 16:23:36.000000 sqlmesh-0.7.1.dev33/docker-compose.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.037154 sqlmesh-0.7.1.dev33/docs/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.010765 sqlmesh-0.7.1.dev33/docs/_readthedocs/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.037407 sqlmesh-0.7.1.dev33/docs/_readthedocs/html/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-31 20:18:29.000000 sqlmesh-0.7.1.dev33/docs/_readthedocs/html/.keep
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9965 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/docs/comparisons.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.039416 sqlmesh-0.7.1.dev33/docs/concepts/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.039870 sqlmesh-0.7.1.dev33/docs/concepts/architecture/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1334 2023-03-27 03:14:49.000000 sqlmesh-0.7.1.dev33/docs/concepts/architecture/serialization.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1113 2023-03-27 03:14:49.000000 sqlmesh-0.7.1.dev33/docs/concepts/architecture/snapshots.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6689 2023-04-20 16:12:45.000000 sqlmesh-0.7.1.dev33/docs/concepts/audits.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3866 2023-03-27 03:14:49.000000 sqlmesh-0.7.1.dev33/docs/concepts/environments.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5952 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/docs/concepts/glossary.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)       13 2023-03-27 03:14:49.000000 sqlmesh-0.7.1.dev33/docs/concepts/hooks.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3086 2023-05-04 16:23:36.000000 sqlmesh-0.7.1.dev33/docs/concepts/macros.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.041104 sqlmesh-0.7.1.dev33/docs/concepts/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9934 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/docs/concepts/models/model_kinds.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8189 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/docs/concepts/models/overview.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7171 2023-03-27 03:14:56.000000 sqlmesh-0.7.1.dev33/docs/concepts/models/python_models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4938 2023-03-27 03:14:56.000000 sqlmesh-0.7.1.dev33/docs/concepts/models/seed_models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5356 2023-03-27 03:14:56.000000 sqlmesh-0.7.1.dev33/docs/concepts/models/sql_models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6637 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/docs/concepts/overview.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.041354 sqlmesh-0.7.1.dev33/docs/concepts/plans/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    43124 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/docs/concepts/plans/model_versioning.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9954 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/docs/concepts/plans.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5699 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/docs/concepts/tests.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      607 2023-04-14 19:58:28.000000 sqlmesh-0.7.1.dev33/docs/development.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.043536 sqlmesh-0.7.1.dev33/docs/guides/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2874 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/docs/guides/connections.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1309 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/docs/guides/migrations.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10756 2023-04-06 22:49:28.000000 sqlmesh-0.7.1.dev33/docs/guides/models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6133 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/docs/guides/multi_repo.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2142 2023-04-20 16:12:45.000000 sqlmesh-0.7.1.dev33/docs/guides/projects.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.050821 sqlmesh-0.7.1.dev33/docs/guides/scheduling/
--rw-r--r--   0 eakmanrq   (501) staff       (20)   740917 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/docs/guides/scheduling/airflow_successful_plan_apply.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   379880 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/docs/guides/scheduling/airflow_successful_setup.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5664 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/docs/guides/scheduling.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1854 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/docs/guides/testing.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5459 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/docs/index.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      297 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/docs/installation.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.054706 sqlmesh-0.7.1.dev33/docs/integrations/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.055327 sqlmesh-0.7.1.dev33/docs/integrations/airflow/
--rw-r--r--   0 eakmanrq   (501) staff       (20)   487944 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/docs/integrations/airflow/airflow_sqlmesh_state_connection.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3516 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/docs/integrations/airflow.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7801 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/docs/integrations/dbt.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    24066 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/docs/integrations/engines.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7711 2023-05-05 16:10:21.000000 sqlmesh-0.7.1.dev33/docs/integrations/github.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.065116 sqlmesh-0.7.1.dev33/docs/integrations/images/
--rw-r--r--   0 eakmanrq   (501) staff       (20)   194172 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/docs/integrations/images/github_deployed_plans.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   271175 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/docs/integrations/images/github_env_summary.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   451584 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/docs/integrations/images/github_prod_plan_preview.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   174084 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/docs/integrations/images/github_reviewers.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   634144 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/docs/integrations/images/github_test_summary.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)      217 2023-03-27 01:55:02.000000 sqlmesh-0.7.1.dev33/docs/integrations/overview.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      665 2023-03-28 15:29:23.000000 sqlmesh-0.7.1.dev33/docs/prerequisites.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12925 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/docs/quick_start.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.070447 sqlmesh-0.7.1.dev33/docs/reference/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6093 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/docs/reference/cli.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15318 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/docs/reference/configuration.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4579 2023-04-20 16:12:45.000000 sqlmesh-0.7.1.dev33/docs/reference/notebook.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1127 2023-03-27 03:14:49.000000 sqlmesh-0.7.1.dev33/docs/reference/overview.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)       14 2023-03-27 03:14:49.000000 sqlmesh-0.7.1.dev33/docs/reference/python.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)       16 2023-03-27 03:14:49.000000 sqlmesh-0.7.1.dev33/docs/release_notes.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      122 2023-03-31 20:18:29.000000 sqlmesh-0.7.1.dev33/docs/requirements.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3249 2023-03-27 01:55:02.000000 sqlmesh-0.7.1.dev33/docs/sqlmesh.png
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.070763 sqlmesh-0.7.1.dev33/examples/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.073181 sqlmesh-0.7.1.dev33/examples/airflow/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1713 2023-04-08 22:07:58.000000 sqlmesh-0.7.1.dev33/examples/airflow/Dockerfile.template
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2164 2023-04-14 19:58:28.000000 sqlmesh-0.7.1.dev33/examples/airflow/Makefile
--rw-r--r--   0 eakmanrq   (501) staff       (20)      942 2023-01-20 19:02:18.000000 sqlmesh-0.7.1.dev33/examples/airflow/README.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/airflow/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.073393 sqlmesh-0.7.1.dev33/examples/airflow/dags/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      263 2023-03-21 21:04:44.000000 sqlmesh-0.7.1.dev33/examples/airflow/dags/sqlmesh_integration.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3515 2023-04-08 22:07:58.000000 sqlmesh-0.7.1.dev33/examples/airflow/docker_compose_decorator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)       12 2023-01-20 19:02:18.000000 sqlmesh-0.7.1.dev33/examples/airflow/requirements.txt
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.074052 sqlmesh-0.7.1.dev33/examples/airflow/spark_conf/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      872 2023-01-20 19:02:18.000000 sqlmesh-0.7.1.dev33/examples/airflow/spark_conf/hive-site.xml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      151 2023-01-20 19:02:18.000000 sqlmesh-0.7.1.dev33/examples/airflow/spark_conf/spark-defaults.conf
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.012127 sqlmesh-0.7.1.dev33/examples/multi/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.074297 sqlmesh-0.7.1.dev33/examples/multi/repo_1/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.074543 sqlmesh-0.7.1.dev33/examples/multi/repo_1/audits/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/examples/multi/repo_1/audits/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      193 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/examples/multi/repo_1/config.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.074723 sqlmesh-0.7.1.dev33/examples/multi/repo_1/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/examples/multi/repo_1/macros/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/examples/multi/repo_1/macros/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.075299 sqlmesh-0.7.1.dev33/examples/multi/repo_1/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/examples/multi/repo_1/models/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)       63 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/examples/multi/repo_1/models/a.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       53 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/examples/multi/repo_1/models/b.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.075516 sqlmesh-0.7.1.dev33/examples/multi/repo_1/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/examples/multi/repo_1/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.075638 sqlmesh-0.7.1.dev33/examples/multi/repo_2/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.075915 sqlmesh-0.7.1.dev33/examples/multi/repo_2/audits/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/examples/multi/repo_2/audits/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      193 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/examples/multi/repo_2/config.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.076671 sqlmesh-0.7.1.dev33/examples/multi/repo_2/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/examples/multi/repo_2/macros/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/examples/multi/repo_2/macros/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.077197 sqlmesh-0.7.1.dev33/examples/multi/repo_2/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/examples/multi/repo_2/models/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)       64 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/examples/multi/repo_2/models/c.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       53 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/examples/multi/repo_2/models/d.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.077541 sqlmesh-0.7.1.dev33/examples/multi/repo_2/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/examples/multi/repo_2/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.078105 sqlmesh-0.7.1.dev33/examples/sushi/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.7.1.dev33/examples/sushi/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.078592 sqlmesh-0.7.1.dev33/examples/sushi/audits/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      105 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi/audits/items.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      119 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi/audits/order_items.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      852 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/examples/sushi/config.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.078879 sqlmesh-0.7.1.dev33/examples/sushi/data/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-06 17:30:39.000000 sqlmesh-0.7.1.dev33/examples/sushi/data/.keep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      551 2023-01-20 19:02:18.000000 sqlmesh-0.7.1.dev33/examples/sushi/helper.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.079073 sqlmesh-0.7.1.dev33/examples/sushi/hooks/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi/hooks/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi/hooks/hooks.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.079311 sqlmesh-0.7.1.dev33/examples/sushi/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.7.1.dev33/examples/sushi/macros/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      233 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/examples/sushi/macros/macros.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.082604 sqlmesh-0.7.1.dev33/examples/sushi/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      934 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/examples/sushi/models/customer_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      223 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/examples/sushi/models/customers.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1911 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/examples/sushi/models/items.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1912 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/examples/sushi/models/order_items.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1643 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/examples/sushi/models/orders.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      346 2023-04-11 16:01:14.000000 sqlmesh-0.7.1.dev33/examples/sushi/models/top_waiters.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      465 2023-04-14 20:24:08.000000 sqlmesh-0.7.1.dev33/examples/sushi/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      123 2023-02-17 23:03:10.000000 sqlmesh-0.7.1.dev33/examples/sushi/models/waiter_names.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      691 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/examples/sushi/models/waiter_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      197 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi/models/waiters.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.082796 sqlmesh-0.7.1.dev33/examples/sushi/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-01-20 19:02:18.000000 sqlmesh-0.7.1.dev33/examples/sushi/seeds/waiter_names.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.083068 sqlmesh-0.7.1.dev33/examples/sushi/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1459 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi/tests/test_customer_revenue_by_day.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.085182 sqlmesh-0.7.1.dev33/examples/sushi_dbt/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       15 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/.gitignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)       41 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/.user.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.085343 sqlmesh-0.7.1.dev33/examples/sushi_dbt/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      299 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      507 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.086100 sqlmesh-0.7.1.dev33/examples/sushi_dbt/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      941 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/macros/incremental.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/macros/log_value.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.101031 sqlmesh-0.7.1.dev33/examples/sushi_dbt/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1125 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/models/customer_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/models/customers.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      182 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/models/schema.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      309 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/models/top_waiters.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      389 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      752 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/models/waiter_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      186 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/models/waiters.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.013219 sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.102262 sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/customers/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.102826 sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/customers/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/customers/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      663 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/customers/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.103294 sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/customers/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      117 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/customers/macros/current_engine.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       65 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.103511 sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/customers/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/customers/models/schema.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.103616 sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/customers/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.104044 sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/customers/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.104168 sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/customers/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/customers/tests/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1092 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/profiles.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.104950 sqlmesh-0.7.1.dev33/examples/sushi_dbt/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2327 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/seeds/items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10472 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/seeds/order_items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9746 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/seeds/orders.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)       97 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/seeds/properties.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/seeds/waiter_names.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.105095 sqlmesh-0.7.1.dev33/examples/sushi_dbt/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.105186 sqlmesh-0.7.1.dev33/examples/sushi_dbt/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.7.1.dev33/examples/sushi_dbt/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.105361 sqlmesh-0.7.1.dev33/examples/wursthall/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/wursthall/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.013953 sqlmesh-0.7.1.dev33/examples/wursthall/audits/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.105551 sqlmesh-0.7.1.dev33/examples/wursthall/audits/db/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      141 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/wursthall/audits/db/order_f.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       79 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/examples/wursthall/config.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.105802 sqlmesh-0.7.1.dev33/examples/wursthall/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/wursthall/macros/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      531 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/examples/wursthall/macros/macros.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.105953 sqlmesh-0.7.1.dev33/examples/wursthall/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/wursthall/models/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.106662 sqlmesh-0.7.1.dev33/examples/wursthall/models/db/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      433 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/examples/wursthall/models/db/customer_d.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      256 2023-04-27 17:28:43.000000 sqlmesh-0.7.1.dev33/examples/wursthall/models/db/item_d.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3158 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/examples/wursthall/models/db/order_f.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      542 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/examples/wursthall/models/db/order_item_f.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.107467 sqlmesh-0.7.1.dev33/examples/wursthall/models/src/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/wursthall/models/src/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1652 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/examples/wursthall/models/src/customer_details.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      120 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/wursthall/models/src/menu_item_details.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3414 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/examples/wursthall/models/src/order_item_details.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      892 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/wursthall/models/src/shared.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.014320 sqlmesh-0.7.1.dev33/examples/wursthall/seeds/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.107623 sqlmesh-0.7.1.dev33/examples/wursthall/seeds/src/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7416 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/wursthall/seeds/src/menu_item_details.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.107928 sqlmesh-0.7.1.dev33/examples/wursthall/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      888 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/wursthall/tests/test_customer_d.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      955 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/examples/wursthall/tests/test_order_item_f.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2113 2023-05-03 20:33:57.000000 sqlmesh-0.7.1.dev33/mkdocs.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.108077 sqlmesh-0.7.1.dev33/pdoc/
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)     1153 2023-03-28 16:31:06.000000 sqlmesh-0.7.1.dev33/pdoc/cli.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.108459 sqlmesh-0.7.1.dev33/pdoc/templates/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      131 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/pdoc/templates/module.html.jinja2
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.108685 sqlmesh-0.7.1.dev33/posts/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.112584 sqlmesh-0.7.1.dev33/posts/virtual_data_environments/
--rw-r--r--   0 eakmanrq   (501) staff       (20)   318753 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/posts/virtual_data_environments/change_categorization.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   274526 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/posts/virtual_data_environments/isolated_rigid_envs.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   163619 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/posts/virtual_data_environments/partial_breaking.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   298971 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/posts/virtual_data_environments/stateful_envs.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   366545 2023-04-19 01:45:56.000000 sqlmesh-0.7.1.dev33/posts/virtual_data_environments/virtual_envs.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)  1344487 2023-04-19 01:45:57.000000 sqlmesh-0.7.1.dev33/posts/virtual_data_environments/virtual_envs_end_to_end.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)    18638 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/posts/virtual_data_environments.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      734 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/pytest.ini
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1501 2023-05-05 17:14:06.444980 sqlmesh-0.7.1.dev33/setup.cfg
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3437 2023-05-05 16:10:17.000000 sqlmesh-0.7.1.dev33/setup.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.123197 sqlmesh-0.7.1.dev33/sqlmesh/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        3 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/sqlmesh/.airflowignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3950 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/sqlmesh/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      175 2023-05-05 17:14:05.000000 sqlmesh-0.7.1.dev33/sqlmesh/_version.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.124182 sqlmesh-0.7.1.dev33/sqlmesh/cicd/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/cicd/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      694 2023-05-05 16:10:21.000000 sqlmesh-0.7.1.dev33/sqlmesh/cicd/bot.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.125296 sqlmesh-0.7.1.dev33/sqlmesh/cli/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      898 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/sqlmesh/cli/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4775 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/cli/example_project.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10729 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/cli/main.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1433 2023-04-19 01:45:57.000000 sqlmesh-0.7.1.dev33/sqlmesh/cli/options.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.132099 sqlmesh-0.7.1.dev33/sqlmesh/core/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      261 2023-05-05 16:10:21.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/_typing.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.132854 sqlmesh-0.7.1.dev33/sqlmesh/core/audit/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      449 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/audit/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1071 2023-04-14 20:24:08.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/audit/builtin.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8238 2023-05-04 16:23:36.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/audit/definition.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.149192 sqlmesh-0.7.1.dev33/sqlmesh/core/config/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      722 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/config/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4412 2023-04-14 19:58:28.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/config/base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1001 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/config/categorizer.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      940 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/config/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    21184 2023-05-04 23:22:11.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/config/connection.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      972 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/config/gateway.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3351 2023-04-20 16:12:45.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/config/loader.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1655 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/config/model.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6095 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/config/root.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8617 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/config/scheduler.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    37996 2023-05-05 16:17:12.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/console.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      826 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/constants.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    36318 2023-05-05 16:10:20.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8904 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/context_diff.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    17484 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/dialect.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.167365 sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2626 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      762 2023-01-17 23:57:22.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/_typing.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    29575 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4818 2023-05-04 16:23:36.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/base_postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4238 2023-04-14 22:30:56.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/base_spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    17690 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      402 2023-04-19 01:45:57.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/databricks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1939 2023-05-04 23:22:11.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/databricks_api.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1992 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/duckdb.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2018 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/logical_merge.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1909 2023-05-04 16:23:36.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6511 2023-05-04 16:23:36.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1181 2023-03-31 20:18:23.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/shared.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2658 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/snowflake.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4879 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1849 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/environment.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      742 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/hooks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12673 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/loader.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    19952 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/macros.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.185718 sqlmesh-0.7.1.dev33/sqlmesh/core/model/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      594 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/model/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1746 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/model/cache.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1300 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/model/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2417 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/model/decorator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    47558 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/model/definition.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8348 2023-05-04 16:23:36.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/model/kind.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13069 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/model/meta.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2017 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/model/seed.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2314 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/notification_target.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.186300 sqlmesh-0.7.1.dev33/sqlmesh/core/plan/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      238 2023-05-05 16:55:11.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/plan/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    25407 2023-05-05 16:55:25.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/plan/definition.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8565 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/plan/evaluator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11720 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/renderer.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15386 2023-04-14 20:24:08.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/scheduler.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    20418 2023-04-19 01:45:57.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/schema_diff.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.187424 sqlmesh-0.7.1.dev33/sqlmesh/core/snapshot/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      527 2023-05-02 20:52:55.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/snapshot/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1990 2023-03-27 01:55:02.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/snapshot/categorizer.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    35781 2023-05-05 16:17:12.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/snapshot/definition.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    19245 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/snapshot/evaluator.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.197392 sqlmesh-0.7.1.dev33/sqlmesh/core/state_sync/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      692 2023-04-14 19:58:28.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/state_sync/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13382 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/state_sync/base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    14349 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/state_sync/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    20769 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/state_sync/engine_adapter.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10885 2023-05-04 16:23:36.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/test.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      982 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/core/user.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.203445 sqlmesh-0.7.1.dev33/sqlmesh/dbt/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       79 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/dbt/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9390 2023-04-14 22:30:56.000000 sqlmesh-0.7.1.dev33/sqlmesh/dbt/adapter.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    17485 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/dbt/basemodel.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11231 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/sqlmesh/dbt/builtin.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1762 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/sqlmesh/dbt/column.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4978 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/dbt/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5087 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/sqlmesh/dbt/context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8670 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/dbt/loader.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9851 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/dbt/model.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    14335 2023-05-04 16:23:36.000000 sqlmesh-0.7.1.dev33/sqlmesh/dbt/package.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3807 2023-05-04 16:23:36.000000 sqlmesh-0.7.1.dev33/sqlmesh/dbt/profile.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4843 2023-05-04 16:23:36.000000 sqlmesh-0.7.1.dev33/sqlmesh/dbt/project.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      927 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/dbt/seed.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3137 2023-04-19 01:45:57.000000 sqlmesh-0.7.1.dev33/sqlmesh/dbt/source.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13618 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/dbt/target.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      291 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/dbt/util.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.203798 sqlmesh-0.7.1.dev33/sqlmesh/engines/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/sqlmesh/engines/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4437 2023-03-22 20:26:36.000000 sqlmesh-0.7.1.dev33/sqlmesh/engines/commands.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.204275 sqlmesh-0.7.1.dev33/sqlmesh/engines/spark/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/sqlmesh/engines/spark/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3414 2023-03-22 20:32:25.000000 sqlmesh-0.7.1.dev33/sqlmesh/engines/spark/app.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.205065 sqlmesh-0.7.1.dev33/sqlmesh/engines/spark/db_api/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/sqlmesh/engines/spark/db_api/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      148 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/sqlmesh/engines/spark/db_api/errors.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2571 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/engines/spark/db_api/spark_session.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.205686 sqlmesh-0.7.1.dev33/sqlmesh/integrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/sqlmesh/integrations/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.213173 sqlmesh-0.7.1.dev33/sqlmesh/integrations/github/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-05-03 23:47:13.000000 sqlmesh-0.7.1.dev33/sqlmesh/integrations/github/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.213753 sqlmesh-0.7.1.dev33/sqlmesh/integrations/github/cicd/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/integrations/github/cicd/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5608 2023-05-05 16:10:21.000000 sqlmesh-0.7.1.dev33/sqlmesh/integrations/github/cicd/command.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    23538 2023-05-05 16:55:11.000000 sqlmesh-0.7.1.dev33/sqlmesh/integrations/github/cicd/controller.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1553 2023-05-04 16:23:36.000000 sqlmesh-0.7.1.dev33/sqlmesh/integrations/llm.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13960 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/magics.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.215883 sqlmesh-0.7.1.dev33/sqlmesh/migrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-14 19:58:28.000000 sqlmesh-0.7.1.dev33/sqlmesh/migrations/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1749 2023-04-14 19:58:28.000000 sqlmesh-0.7.1.dev33/sqlmesh/migrations/v0001_init.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      103 2023-04-19 01:45:57.000000 sqlmesh-0.7.1.dev33/sqlmesh/migrations/v0002_remove_identify.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1183 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/sqlmesh/migrations/v0003_move_batch_size.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      534 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/sqlmesh/py.typed
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.216650 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.230532 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-05 17:38:29.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4020 2023-04-14 19:58:28.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/api.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8128 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/client.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3888 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    18863 2023-05-05 16:10:21.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/dag_generator.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.271156 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/hooks/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-15 19:26:11.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/hooks/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2132 2023-03-22 20:54:22.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/hooks/bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      868 2023-03-22 20:54:22.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/hooks/redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8508 2023-03-22 20:33:52.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/integration.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.273868 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1444 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6307 2023-03-22 20:26:36.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/databricks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2549 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      877 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/notification.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1322 2023-04-19 01:45:57.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1211 2023-01-20 20:10:57.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1340 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/snowflake.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5222 2023-03-22 20:26:36.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/spark_submit.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11104 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/targets.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4660 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/plan.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1292 2023-04-14 19:58:28.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/plugin.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4139 2023-04-14 19:58:28.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/state_sync.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5878 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/util.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.277374 sqlmesh-0.7.1.dev33/sqlmesh/utils/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4386 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/utils/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3593 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/sqlmesh/utils/cache.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8053 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/utils/concurrency.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7530 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/utils/connection_pool.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      410 2022-12-30 00:03:50.000000 sqlmesh-0.7.1.dev33/sqlmesh/utils/conversions.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4329 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/utils/dag.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7606 2023-05-05 15:43:05.000000 sqlmesh-0.7.1.dev33/sqlmesh/utils/date.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1289 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/sqlmesh/utils/errors.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    16133 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/sqlmesh/utils/jinja.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15093 2023-04-06 22:49:28.000000 sqlmesh-0.7.1.dev33/sqlmesh/utils/metaprogramming.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      888 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/utils/pandas.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1609 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/utils/pydantic.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1534 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/sqlmesh/utils/rich.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6487 2023-04-19 01:45:57.000000 sqlmesh-0.7.1.dev33/sqlmesh/utils/transactional_file.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1419 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/sqlmesh/utils/yaml.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.123956 sqlmesh-0.7.1.dev33/sqlmesh.egg-info/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2187 2023-05-05 17:14:05.000000 sqlmesh-0.7.1.dev33/sqlmesh.egg-info/PKG-INFO
--rw-r--r--   0 eakmanrq   (501) staff       (20)    21707 2023-05-05 17:14:05.000000 sqlmesh-0.7.1.dev33/sqlmesh.egg-info/SOURCES.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)        1 2023-05-05 17:14:05.000000 sqlmesh-0.7.1.dev33/sqlmesh.egg-info/dependency_links.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)      178 2023-05-05 17:14:05.000000 sqlmesh-0.7.1.dev33/sqlmesh.egg-info/entry_points.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)      949 2023-05-05 17:14:05.000000 sqlmesh-0.7.1.dev33/sqlmesh.egg-info/requires.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)       12 2023-05-05 17:14:05.000000 sqlmesh-0.7.1.dev33/sqlmesh.egg-info/top_level.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)    21020 2023-03-27 03:14:56.000000 sqlmesh-0.7.1.dev33/sqlmesh.svg
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.289423 sqlmesh-0.7.1.dev33/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/tests/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      285 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/tests/common_fixtures.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4037 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/tests/conftest.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.300927 sqlmesh-0.7.1.dev33/tests/core/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/tests/core/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.307103 sqlmesh-0.7.1.dev33/tests/core/engine_adapter/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/tests/core/engine_adapter/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    28082 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2114 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_base_postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1244 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_base_spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7847 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1227 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_databricks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4916 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_duckdb.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1569 2023-04-19 01:45:57.000000 sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7850 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3191 2023-04-19 01:45:57.000000 sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7063 2023-05-04 16:23:36.000000 sqlmesh-0.7.1.dev33/tests/core/test_audit.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6995 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/tests/core/test_config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      850 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/core/test_connection_config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10041 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/tests/core/test_context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2749 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/tests/core/test_dialect.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      464 2022-12-28 16:53:44.000000 sqlmesh-0.7.1.dev33/tests/core/test_environment.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    26773 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/tests/core/test_integration.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6699 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/tests/core/test_macros.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    26371 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/tests/core/test_model.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    17081 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/tests/core/test_plan.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3890 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/tests/core/test_plan_evaluator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4647 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/tests/core/test_scheduler.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    32235 2023-04-19 01:45:57.000000 sqlmesh-0.7.1.dev33/tests/core/test_schema_diff.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      857 2023-01-06 18:44:22.000000 sqlmesh-0.7.1.dev33/tests/core/test_seed.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    29629 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/tests/core/test_snapshot.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10299 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/tests/core/test_snapshot_evaluator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    24610 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/tests/core/test_state_sync.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.308602 sqlmesh-0.7.1.dev33/tests/dbt/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-16 20:33:14.000000 sqlmesh-0.7.1.dev33/tests/dbt/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      739 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/tests/dbt/conftest.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2537 2023-04-19 01:45:57.000000 sqlmesh-0.7.1.dev33/tests/dbt/test_adapter.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13195 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/tests/dbt/test_config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    17095 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/tests/dbt/test_transformation.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.308891 sqlmesh-0.7.1.dev33/tests/engines/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/tests/engines/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.309453 sqlmesh-0.7.1.dev33/tests/engines/spark/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/tests/engines/spark/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      357 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/tests/engines/spark/conftest.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1503 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/tests/engines/spark/test_db_api.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.018231 sqlmesh-0.7.1.dev33/tests/fixtures/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.016831 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.311016 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.311180 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      299 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/config.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.016965 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/dbt_packages/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1055 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.311297 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/logs/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10264 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.311621 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      941 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/macros/incremental.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/macros/log_value.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.322730 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/models/schema.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      334 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      389 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      863 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      196 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/models/waiters.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.017453 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.322952 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.323222 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      663 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.323614 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      117 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       65 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.324315 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1155 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      108 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      193 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.324595 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.324724 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.324837 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)       41 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      540 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/profiles.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1250 2023-04-19 01:45:57.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/seed_sources.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.325199 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       42 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/seeds/properties.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.325371 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.325755 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/source_data/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2327 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/source_data/items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10472 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9746 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/source_data/orders.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.325928 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.326258 sqlmesh-0.7.1.dev33/tests/fixtures/migrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9823 2023-04-14 19:58:28.000000 sqlmesh-0.7.1.dev33/tests/fixtures/migrations/environments.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)    25229 2023-04-14 19:58:28.000000 sqlmesh-0.7.1.dev33/tests/fixtures/migrations/snapshots.json
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.326657 sqlmesh-0.7.1.dev33/tests/schedulers/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/tests/schedulers/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.327987 sqlmesh-0.7.1.dev33/tests/schedulers/airflow/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/tests/schedulers/airflow/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1414 2023-01-20 19:02:18.000000 sqlmesh-0.7.1.dev33/tests/schedulers/airflow/conftest.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.328465 sqlmesh-0.7.1.dev33/tests/schedulers/airflow/operators/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/tests/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4442 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/tests/schedulers/airflow/operators/test_hwm_sensor.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4392 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/tests/schedulers/airflow/operators/test_targets.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9920 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/tests/schedulers/airflow/test_client.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1345 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/tests/schedulers/airflow/test_end_to_end.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6222 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/tests/schedulers/airflow/test_integration.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6054 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/tests/schedulers/airflow/test_plan.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.330929 sqlmesh-0.7.1.dev33/tests/utils/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/tests/utils/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1118 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/tests/utils/test_cache.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3580 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/tests/utils/test_concurrency.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6430 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/tests/utils/test_connection_pool.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1381 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/tests/utils/test_dag.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1818 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/tests/utils/test_date.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      551 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/tests/utils/test_filesystem.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5516 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/tests/utils/test_jinja.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5790 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/tests/utils/test_metaprogramming.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2501 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/tests/utils/test_pandas.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      518 2022-12-05 19:41:13.000000 sqlmesh-0.7.1.dev33/tests/utils/test_pydantic.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2911 2023-04-17 00:43:26.000000 sqlmesh-0.7.1.dev33/tests/utils/test_transactional_file.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1194 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/tests/utils/test_yaml.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.331189 sqlmesh-0.7.1.dev33/tests/web/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.7.1.dev33/tests/web/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    16226 2023-05-04 16:23:36.000000 sqlmesh-0.7.1.dev33/tests/web/test_main.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.331571 sqlmesh-0.7.1.dev33/web/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.7.1.dev33/web/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.341778 sqlmesh-0.7.1.dev33/web/client/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1104 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/.eslintrc.js
--rw-r--r--   0 eakmanrq   (501) staff       (20)       94 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/.gitignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)      129 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/.prettierignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)      403 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/web/client/.prettierrc.js
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1076 2023-03-27 22:28:21.000000 sqlmesh-0.7.1.dev33/web/client/index.html
--rw-r--r--   0 eakmanrq   (501) staff       (20)    37689 2023-04-27 17:30:24.000000 sqlmesh-0.7.1.dev33/web/client/openapi.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)      330 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/orval.config.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)   408504 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/web/client/package-lock.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2389 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/web/client/package.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1642 2023-04-17 00:43:26.000000 sqlmesh-0.7.1.dev33/web/client/playwright.config.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)       82 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/web/client/postcss.config.js
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.018814 sqlmesh-0.7.1.dev33/web/client/public/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.342057 sqlmesh-0.7.1.dev33/web/client/public/favicons/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2473 2023-03-27 01:55:02.000000 sqlmesh-0.7.1.dev33/web/client/public/favicons/favicon.ico
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.342885 sqlmesh-0.7.1.dev33/web/client/src/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.343722 sqlmesh-0.7.1.dev33/web/client/src/api/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1236 2023-04-20 17:40:30.000000 sqlmesh-0.7.1.dev33/web/client/src/api/channels.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5243 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/web/client/src/api/index.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3247 2023-03-22 20:27:52.000000 sqlmesh-0.7.1.dev33/web/client/src/api/instance.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.019079 sqlmesh-0.7.1.dev33/web/client/src/assets/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.019192 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.346510 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74500 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74524 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74368 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    73964 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    68940 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    67284 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74116 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    73916 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.351195 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    55004 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-Black.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56384 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57104 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-Bold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    62320 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56652 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    61688 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57680 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-Italic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    53148 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-Light.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57060 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56836 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-Medium.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    61460 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    52820 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-Roman.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    59176 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    63876 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    60768 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    81732 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    60992 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    64792 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.352721 sqlmesh-0.7.1.dev33/web/client/src/context/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4126 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/web/client/src/context/context.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6470 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/web/client/src/context/editor.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      923 2023-04-14 20:24:08.000000 sqlmesh-0.7.1.dev33/web/client/src/context/fileTree.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2187 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/web/client/src/context/lineage.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2661 2023-04-14 19:58:28.000000 sqlmesh-0.7.1.dev33/web/client/src/context/plan.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1562 2023-03-22 22:04:55.000000 sqlmesh-0.7.1.dev33/web/client/src/context/theme.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.353454 sqlmesh-0.7.1.dev33/web/client/src/hooks/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      308 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/web/client/src/hooks/useActiveFocus.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      817 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/web/client/src/hooks/useLocalStorage.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9555 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/web/client/src/index.css
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.019427 sqlmesh-0.7.1.dev33/web/client/src/library/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.020670 sqlmesh-0.7.1.dev33/web/client/src/library/components/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.353722 sqlmesh-0.7.1.dev33/web/client/src/library/components/banner/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1705 2023-04-20 17:40:30.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/banner/Banner.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.353977 sqlmesh-0.7.1.dev33/web/client/src/library/components/button/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4517 2023-03-27 01:55:02.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/button/Button.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.354263 sqlmesh-0.7.1.dev33/web/client/src/library/components/button/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3516 2023-03-27 01:55:02.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/button/tests/Button.spec.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.354505 sqlmesh-0.7.1.dev33/web/client/src/library/components/divider/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      856 2023-03-22 22:04:55.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/divider/Divider.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.354754 sqlmesh-0.7.1.dev33/web/client/src/library/components/divider/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      632 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/divider/tests/Divider.spec.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.368731 sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1992 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/Editor.css
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5764 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/Editor.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8518 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/EditorCode.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2718 2023-04-14 20:24:08.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/EditorFooter.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1990 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/EditorIndicator.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9819 2023-04-14 20:24:08.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/EditorInspector.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11905 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/EditorPreview.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3527 2023-04-27 18:23:33.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/EditorTabs.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.369227 sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/extensions/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5820 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5744 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/extensions/index.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1538 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/help.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.370120 sqlmesh-0.7.1.dev33/web/client/src/library/components/fileTree/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10852 2023-04-14 20:24:08.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/fileTree/Directory.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6045 2023-04-14 20:24:08.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/fileTree/File.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2997 2023-04-14 20:24:08.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/fileTree/FileTree.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      562 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/fileTree/help.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.377208 sqlmesh-0.7.1.dev33/web/client/src/library/components/graph/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      159 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/graph/Graph.css
--rw-r--r--   0 eakmanrq   (501) staff       (20)    14454 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/graph/Graph.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7679 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/graph/help.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.378274 sqlmesh-0.7.1.dev33/web/client/src/library/components/ide/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4342 2023-04-14 20:24:08.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/ide/ActivePlan.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4933 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/ide/IDE.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    22356 2023-03-27 22:28:21.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/ide/RunPlan.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.379345 sqlmesh-0.7.1.dev33/web/client/src/library/components/input/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2087 2023-03-28 20:12:46.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/input/Input.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      688 2023-03-22 22:04:55.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/input/InputToggle.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.379586 sqlmesh-0.7.1.dev33/web/client/src/library/components/loading/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      486 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/loading/Loading.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.380227 sqlmesh-0.7.1.dev33/web/client/src/library/components/logo/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2292 2023-03-22 22:04:55.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/logo/Spinner.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4637 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/logo/SqlMesh.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8042 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/logo/Tobiko.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.395338 sqlmesh-0.7.1.dev33/web/client/src/library/components/modal/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1560 2023-03-22 22:04:55.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/modal/Modal.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1953 2023-03-27 01:55:02.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/modal/ModalConfirmation.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1447 2023-03-27 01:55:02.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/modal/ModalDrawer.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.399850 sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9269 2023-04-20 17:40:30.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/Plan.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6775 2023-03-27 01:55:02.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/PlanActions.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1312 2023-03-28 20:12:46.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/PlanBackfillDates.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10448 2023-04-14 20:24:08.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/PlanChangePreview.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4920 2023-04-20 17:40:30.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/PlanHeader.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15855 2023-04-20 17:40:30.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/PlanWizard.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9926 2023-03-27 22:28:21.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12528 2023-04-20 17:40:30.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/context.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3444 2023-03-27 01:55:02.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/help.spec.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2155 2023-03-22 20:27:52.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/help.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2599 2023-04-20 17:40:30.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/hooks.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.400182 sqlmesh-0.7.1.dev33/web/client/src/library/components/progress/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      713 2023-03-27 01:55:02.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/progress/Progress.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.400534 sqlmesh-0.7.1.dev33/web/client/src/library/components/report/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1047 2023-04-20 17:40:30.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/report/ReportTestsErrors.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.401922 sqlmesh-0.7.1.dev33/web/client/src/library/components/root/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      526 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/root/Footer.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1921 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/root/Header.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/root/Main.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      443 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/root/Root.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.402567 sqlmesh-0.7.1.dev33/web/client/src/library/components/splitPane/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      788 2023-03-22 22:04:55.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/splitPane/SplitPane.css
--rw-r--r--   0 eakmanrq   (501) staff       (20)      541 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/splitPane/SplitPane.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.402889 sqlmesh-0.7.1.dev33/web/client/src/library/components/tasksOverview/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11713 2023-04-14 20:24:08.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/tasksOverview/TasksOverview.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.403194 sqlmesh-0.7.1.dev33/web/client/src/library/components/toggle/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1453 2023-03-27 01:55:02.000000 sqlmesh-0.7.1.dev33/web/client/src/library/components/toggle/Toggle.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1197 2023-03-27 01:55:02.000000 sqlmesh-0.7.1.dev33/web/client/src/main.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.420650 sqlmesh-0.7.1.dev33/web/client/src/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1647 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/src/models/artifact.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3472 2023-04-06 22:49:28.000000 sqlmesh-0.7.1.dev33/web/client/src/models/directory.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4190 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/web/client/src/models/environment.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2190 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/web/client/src/models/file.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      173 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/web/client/src/models/index.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      766 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/web/client/src/models/initial.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      200 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/web/client/src/routes.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.421250 sqlmesh-0.7.1.dev33/web/client/src/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       35 2023-01-20 19:02:18.000000 sqlmesh-0.7.1.dev33/web/client/src/tests/setup.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      541 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/web/client/src/tests/utils.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.421848 sqlmesh-0.7.1.dev33/web/client/src/types/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      467 2023-03-22 22:04:55.000000 sqlmesh-0.7.1.dev33/web/client/src/types/enum.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      137 2023-03-22 22:04:55.000000 sqlmesh-0.7.1.dev33/web/client/src/types/index.d.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.422367 sqlmesh-0.7.1.dev33/web/client/src/utils/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4102 2023-03-27 01:55:02.000000 sqlmesh-0.7.1.dev33/web/client/src/utils/index.spec.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5413 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/web/client/src/utils/index.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.422634 sqlmesh-0.7.1.dev33/web/client/src/workers/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      113 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/src/workers/index.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.423097 sqlmesh-0.7.1.dev33/web/client/src/workers/sqlglot/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1105 2023-04-14 20:24:08.000000 sqlmesh-0.7.1.dev33/web/client/src/workers/sqlglot/sqlglot.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1578 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/src/workers/sqlglot/worker.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5879 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/web/client/tailwind.config.js
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.423267 sqlmesh-0.7.1.dev33/web/client/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      170 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/tests/initial.spec.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1141 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/client/tsconfig.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1297 2023-04-17 00:43:26.000000 sqlmesh-0.7.1.dev33/web/client/vite.config.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.437320 sqlmesh-0.7.1.dev33/web/server/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.7.1.dev33/web/server/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.437639 sqlmesh-0.7.1.dev33/web/server/api/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-17 04:56:29.000000 sqlmesh-0.7.1.dev33/web/server/api/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-05-05 17:14:06.443829 sqlmesh-0.7.1.dev33/web/server/api/endpoints/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      784 2023-04-14 20:24:08.000000 sqlmesh-0.7.1.dev33/web/server/api/endpoints/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4564 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/web/server/api/endpoints/commands.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      840 2023-05-05 16:09:43.000000 sqlmesh-0.7.1.dev33/web/server/api/endpoints/context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1858 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/web/server/api/endpoints/directories.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      721 2023-04-19 01:45:57.000000 sqlmesh-0.7.1.dev33/web/server/api/endpoints/environments.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      637 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/web/server/api/endpoints/events.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5383 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/web/server/api/endpoints/files.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3283 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/web/server/api/endpoints/lineage.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      962 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/web/server/api/endpoints/models.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3635 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/web/server/api/endpoints/plan.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3775 2023-04-20 17:40:30.000000 sqlmesh-0.7.1.dev33/web/server/console.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1534 2023-05-02 01:23:18.000000 sqlmesh-0.7.1.dev33/web/server/main.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5777 2023-04-25 19:48:01.000000 sqlmesh-0.7.1.dev33/web/server/models.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      260 2023-04-04 21:33:39.000000 sqlmesh-0.7.1.dev33/web/server/openapi.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2421 2023-04-27 17:30:24.000000 sqlmesh-0.7.1.dev33/web/server/settings.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2114 2023-03-17 21:52:31.000000 sqlmesh-0.7.1.dev33/web/server/sse.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2461 2023-04-19 01:45:57.000000 sqlmesh-0.7.1.dev33/web/server/utils.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1003 2023-05-04 16:23:36.000000 sqlmesh-0.7.1.dev33/web/server/watcher.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.650666 sqlmesh-0.8.0/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.558666 sqlmesh-0.8.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1872 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4515 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/.circleci/continue_config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       66 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/.dockerignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1900 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/.readthedocs.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/Dockerfile.api
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/Dockerfile.app
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11346 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1855 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1979 2023-05-08 23:29:21.650666 sqlmesh-0.8.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1192 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1188 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docker-compose.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.562666 sqlmesh-0.8.0/docs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.542666 sqlmesh-0.8.0/docs/_readthedocs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.562666 sqlmesh-0.8.0/docs/_readthedocs/html/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/_readthedocs/html/.keep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9965 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/comparisons.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.562666 sqlmesh-0.8.0/docs/concepts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.562666 sqlmesh-0.8.0/docs/concepts/architecture/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/concepts/architecture/serialization.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1113 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/concepts/architecture/snapshots.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6689 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/concepts/audits.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3866 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/concepts/environments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5952 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/concepts/glossary.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/concepts/hooks.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3086 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/concepts/macros.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.562666 sqlmesh-0.8.0/docs/concepts/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9934 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/concepts/models/model_kinds.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8189 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/concepts/models/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7171 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/concepts/models/python_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4938 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/concepts/models/seed_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5356 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/concepts/models/sql_models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6637 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/concepts/overview.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.562666 sqlmesh-0.8.0/docs/concepts/plans/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43124 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/concepts/plans/model_versioning.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9954 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/concepts/plans.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5699 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/concepts/tests.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/development.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.562666 sqlmesh-0.8.0/docs/guides/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2874 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/guides/connections.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1309 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/guides/migrations.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/guides/models.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6133 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/guides/multi_repo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2142 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/guides/projects.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.566666 sqlmesh-0.8.0/docs/guides/scheduling/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   740917 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/guides/scheduling/airflow_successful_plan_apply.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   379880 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/guides/scheduling/airflow_successful_setup.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5664 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/guides/scheduling.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1854 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/guides/testing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5459 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/index.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/installation.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.566666 sqlmesh-0.8.0/docs/integrations/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.566666 sqlmesh-0.8.0/docs/integrations/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   487944 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/integrations/airflow/airflow_sqlmesh_state_connection.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3516 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/integrations/airflow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7801 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/integrations/dbt.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24066 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/integrations/engines.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.566666 sqlmesh-0.8.0/docs/integrations/github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   194172 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/integrations/github/github_deployed_plans.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   271175 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/integrations/github/github_env_summary.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   451584 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/integrations/github/github_prod_plan_preview.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   174084 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/integrations/github/github_reviewers.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   634144 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/integrations/github/github_test_summary.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7744 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/integrations/github.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      217 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/integrations/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/prerequisites.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12925 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/quick_start.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.570666 sqlmesh-0.8.0/docs/reference/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6093 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/reference/cli.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15318 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/reference/configuration.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4579 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/reference/notebook.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/reference/overview.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/reference/python.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/release_notes.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3249 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/docs/sqlmesh.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.570666 sqlmesh-0.8.0/examples/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.570666 sqlmesh-0.8.0/examples/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/airflow/Dockerfile.template
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2164 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/airflow/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      942 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/airflow/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/airflow/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.570666 sqlmesh-0.8.0/examples/airflow/dags/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/airflow/dags/sqlmesh_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3515 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/airflow/docker_compose_decorator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/airflow/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.570666 sqlmesh-0.8.0/examples/airflow/spark_conf/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/airflow/spark_conf/hive-site.xml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/airflow/spark_conf/spark-defaults.conf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.546666 sqlmesh-0.8.0/examples/multi/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.570666 sqlmesh-0.8.0/examples/multi/repo_1/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.570666 sqlmesh-0.8.0/examples/multi/repo_1/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/multi/repo_1/audits/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/multi/repo_1/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.570666 sqlmesh-0.8.0/examples/multi/repo_1/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/multi/repo_1/macros/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/multi/repo_1/macros/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.570666 sqlmesh-0.8.0/examples/multi/repo_1/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/multi/repo_1/models/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/multi/repo_1/models/a.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/multi/repo_1/models/b.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.570666 sqlmesh-0.8.0/examples/multi/repo_1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/multi/repo_1/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.570666 sqlmesh-0.8.0/examples/multi/repo_2/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.570666 sqlmesh-0.8.0/examples/multi/repo_2/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/multi/repo_2/audits/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/multi/repo_2/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.570666 sqlmesh-0.8.0/examples/multi/repo_2/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/multi/repo_2/macros/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/multi/repo_2/macros/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.574666 sqlmesh-0.8.0/examples/multi/repo_2/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/multi/repo_2/models/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/multi/repo_2/models/c.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/multi/repo_2/models/d.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.574666 sqlmesh-0.8.0/examples/multi/repo_2/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/multi/repo_2/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.574666 sqlmesh-0.8.0/examples/sushi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.574666 sqlmesh-0.8.0/examples/sushi/audits/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/audits/items.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/audits/order_items.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      852 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.574666 sqlmesh-0.8.0/examples/sushi/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/data/.keep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.574666 sqlmesh-0.8.0/examples/sushi/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/hooks/hooks.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.574666 sqlmesh-0.8.0/examples/sushi/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/macros/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/macros/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.574666 sqlmesh-0.8.0/examples/sushi/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      934 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1911 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/models/items.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1912 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/models/order_items.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/models/orders.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/models/waiter_names.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      197 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.574666 sqlmesh-0.8.0/examples/sushi/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.574666 sqlmesh-0.8.0/examples/sushi/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1459 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi/tests/test_customer_revenue_by_day.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.578666 sqlmesh-0.8.0/examples/sushi_dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/.user.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.578666 sqlmesh-0.8.0/examples/sushi_dbt/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      299 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      507 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.578666 sqlmesh-0.8.0/examples/sushi_dbt/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/macros/incremental.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/macros/log_value.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.578666 sqlmesh-0.8.0/examples/sushi_dbt/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1125 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/models/schema.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      752 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.546666 sqlmesh-0.8.0/examples/sushi_dbt/packages/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.578666 sqlmesh-0.8.0/examples/sushi_dbt/packages/customers/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.578666 sqlmesh-0.8.0/examples/sushi_dbt/packages/customers/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      663 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/packages/customers/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.578666 sqlmesh-0.8.0/examples/sushi_dbt/packages/customers/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      117 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.578666 sqlmesh-0.8.0/examples/sushi_dbt/packages/customers/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/packages/customers/models/schema.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.578666 sqlmesh-0.8.0/examples/sushi_dbt/packages/customers/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.578666 sqlmesh-0.8.0/examples/sushi_dbt/packages/customers/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.578666 sqlmesh-0.8.0/examples/sushi_dbt/packages/customers/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/packages/customers/tests/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1092 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/profiles.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.578666 sqlmesh-0.8.0/examples/sushi_dbt/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/seeds/items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10472 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/seeds/order_items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9746 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/seeds/orders.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/seeds/properties.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.578666 sqlmesh-0.8.0/examples/sushi_dbt/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.578666 sqlmesh-0.8.0/examples/sushi_dbt/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/sushi_dbt/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.582666 sqlmesh-0.8.0/examples/wursthall/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.546666 sqlmesh-0.8.0/examples/wursthall/audits/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.582666 sqlmesh-0.8.0/examples/wursthall/audits/db/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/audits/db/order_f.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.582666 sqlmesh-0.8.0/examples/wursthall/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/macros/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      531 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/macros/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.582666 sqlmesh-0.8.0/examples/wursthall/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/models/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.582666 sqlmesh-0.8.0/examples/wursthall/models/db/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      433 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/models/db/customer_d.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/models/db/item_d.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3158 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/models/db/order_f.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      542 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/models/db/order_item_f.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.582666 sqlmesh-0.8.0/examples/wursthall/models/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/models/src/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1652 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/models/src/customer_details.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      120 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/models/src/menu_item_details.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3414 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/models/src/order_item_details.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      892 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/models/src/shared.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.546666 sqlmesh-0.8.0/examples/wursthall/seeds/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.582666 sqlmesh-0.8.0/examples/wursthall/seeds/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7416 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/seeds/src/menu_item_details.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.582666 sqlmesh-0.8.0/examples/wursthall/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/tests/test_customer_d.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/examples/wursthall/tests/test_order_item_f.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2113 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/mkdocs.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.582666 sqlmesh-0.8.0/pdoc/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1153 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/pdoc/cli.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.582666 sqlmesh-0.8.0/pdoc/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      131 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/pdoc/templates/module.html.jinja2
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.582666 sqlmesh-0.8.0/posts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.586666 sqlmesh-0.8.0/posts/virtual_data_environments/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   318753 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/posts/virtual_data_environments/change_categorization.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   274526 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/posts/virtual_data_environments/isolated_rigid_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   163619 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/posts/virtual_data_environments/partial_breaking.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   298971 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/posts/virtual_data_environments/stateful_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   366545 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/posts/virtual_data_environments/virtual_envs.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1344487 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/posts/virtual_data_environments/virtual_envs_end_to_end.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18638 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/posts/virtual_data_environments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      734 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/pytest.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1501 2023-05-08 23:29:21.654667 sqlmesh-0.8.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3463 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.586666 sqlmesh-0.8.0/sqlmesh/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        3 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/.airflowignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3950 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-05-08 23:29:21.000000 sqlmesh-0.8.0/sqlmesh/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.586666 sqlmesh-0.8.0/sqlmesh/cicd/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/cicd/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      694 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/cicd/bot.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.590666 sqlmesh-0.8.0/sqlmesh/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      898 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4775 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/cli/example_project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10729 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/cli/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1433 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/cli/options.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.590666 sqlmesh-0.8.0/sqlmesh/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      261 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/_typing.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.590666 sqlmesh-0.8.0/sqlmesh/core/audit/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      449 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/audit/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1071 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/audit/builtin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8238 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/audit/definition.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.594666 sqlmesh-0.8.0/sqlmesh/core/config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      722 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/config/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4412 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/config/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1001 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/config/categorizer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/config/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21184 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/config/connection.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/config/gateway.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3351 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/config/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1655 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/config/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6095 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/config/root.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8617 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/config/scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    37996 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/console.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36563 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8904 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/context_diff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17484 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/dialect.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.594666 sqlmesh-0.8.0/sqlmesh/core/engine_adapter/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2626 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/engine_adapter/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      762 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/engine_adapter/_typing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29575 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/engine_adapter/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4818 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/engine_adapter/base_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4238 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/engine_adapter/base_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17690 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/engine_adapter/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/engine_adapter/databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1939 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/engine_adapter/databricks_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1992 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/engine_adapter/duckdb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2018 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/engine_adapter/logical_merge.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1909 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/engine_adapter/postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6511 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/engine_adapter/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1181 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/engine_adapter/shared.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2658 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/engine_adapter/snowflake.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4879 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/engine_adapter/spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1849 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/environment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/hooks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12673 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19952 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/macros.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.598666 sqlmesh-0.8.0/sqlmesh/core/model/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      594 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/model/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1746 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/model/cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1300 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/model/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2417 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/model/decorator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    47558 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/model/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8348 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/model/kind.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13069 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/model/meta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2017 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/model/seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2314 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/notification_target.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.598666 sqlmesh-0.8.0/sqlmesh/core/plan/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/plan/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25407 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/plan/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8565 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/plan/evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11720 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/renderer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15386 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20418 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/schema_diff.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.598666 sqlmesh-0.8.0/sqlmesh/core/snapshot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/snapshot/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1990 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/snapshot/categorizer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35781 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/snapshot/definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19245 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/snapshot/evaluator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.598666 sqlmesh-0.8.0/sqlmesh/core/state_sync/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      692 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/state_sync/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13382 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/state_sync/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14349 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/state_sync/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20769 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/state_sync/engine_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10885 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      982 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/core/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.602666 sqlmesh-0.8.0/sqlmesh/dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9400 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10462 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/basemodel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10282 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/builtin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1762 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3984 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5834 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6977 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8032 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/manifest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9876 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3435 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/package.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3807 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3760 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2849 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13618 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/target.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/dbt/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.602666 sqlmesh-0.8.0/sqlmesh/engines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/engines/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4437 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/engines/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.602666 sqlmesh-0.8.0/sqlmesh/engines/spark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/engines/spark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3414 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/engines/spark/app.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.602666 sqlmesh-0.8.0/sqlmesh/engines/spark/db_api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/engines/spark/db_api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/engines/spark/db_api/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2571 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/engines/spark/db_api/spark_session.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.602666 sqlmesh-0.8.0/sqlmesh/integrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/integrations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.602666 sqlmesh-0.8.0/sqlmesh/integrations/github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/integrations/github/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.602666 sqlmesh-0.8.0/sqlmesh/integrations/github/cicd/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/integrations/github/cicd/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5743 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/integrations/github/cicd/command.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23708 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/integrations/github/cicd/controller.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1553 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/integrations/llm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13960 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/magics.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.602666 sqlmesh-0.8.0/sqlmesh/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/migrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/migrations/v0001_init.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/migrations/v0002_remove_identify.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1183 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/migrations/v0003_move_batch_size.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      534 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/py.typed
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.602666 sqlmesh-0.8.0/sqlmesh/schedulers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.606666 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4020 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8128 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3888 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18863 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/dag_generator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.606666 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2132 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/hooks/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      868 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/hooks/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8508 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/integration.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.606666 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6307 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2549 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/notification.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1322 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1340 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/snowflake.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5222 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/spark_submit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11104 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/targets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4660 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1292 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4139 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/state_sync.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5878 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/schedulers/airflow/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.610666 sqlmesh-0.8.0/sqlmesh/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4664 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3593 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/utils/cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8053 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/utils/concurrency.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7530 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/utils/connection_pool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/utils/conversions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4329 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/utils/dag.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7606 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/utils/date.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1289 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/utils/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16080 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/utils/jinja.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15093 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/utils/metaprogramming.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/utils/pandas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1609 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/utils/pydantic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/utils/rich.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6487 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/utils/transactional_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1419 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh/utils/yaml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.586666 sqlmesh-0.8.0/sqlmesh.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1979 2023-05-08 23:29:21.000000 sqlmesh-0.8.0/sqlmesh.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22624 2023-05-08 23:29:21.000000 sqlmesh-0.8.0/sqlmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-08 23:29:21.000000 sqlmesh-0.8.0/sqlmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      177 2023-05-08 23:29:21.000000 sqlmesh-0.8.0/sqlmesh.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      960 2023-05-08 23:29:21.000000 sqlmesh-0.8.0/sqlmesh.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-08 23:29:21.000000 sqlmesh-0.8.0/sqlmesh.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21020 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/sqlmesh.svg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.610666 sqlmesh-0.8.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      285 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/common_fixtures.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4037 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.610666 sqlmesh-0.8.0/tests/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.614666 sqlmesh-0.8.0/tests/core/engine_adapter/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/engine_adapter/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28082 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/engine_adapter/test_base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2114 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/engine_adapter/test_base_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1244 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/engine_adapter/test_base_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7847 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/engine_adapter/test_bigquery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1227 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/engine_adapter/test_databricks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4916 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/engine_adapter/test_duckdb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1569 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/engine_adapter/test_postgres.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7850 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/engine_adapter/test_redshift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3191 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/engine_adapter/test_spark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7063 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_audit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6995 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      850 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_connection_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10041 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2749 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_dialect.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_environment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26773 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6699 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_macros.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26371 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17081 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3890 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_plan_evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4647 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32235 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_schema_diff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      857 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_seed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29671 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_snapshot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10299 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_snapshot_evaluator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24610 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/core/test_state_sync.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.614666 sqlmesh-0.8.0/tests/dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/dbt/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      739 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/dbt/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2319 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/dbt/test_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11417 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/dbt/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2632 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/dbt/test_manifest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12926 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/dbt/test_transformation.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.614666 sqlmesh-0.8.0/tests/engines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/engines/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.614666 sqlmesh-0.8.0/tests/engines/spark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/engines/spark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      357 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/engines/spark/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1503 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/engines/spark/test_db_api.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.554666 sqlmesh-0.8.0/tests/fixtures/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.550666 sqlmesh-0.8.0/tests/fixtures/dbt/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.614666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.614666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      299 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.550666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/dbt_packages/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1017 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.614666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/logs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10264 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.618666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/macros/incremental.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/macros/log_value.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.618666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/models/schema.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      196 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/models/waiters.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.550666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.618666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.618666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      663 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.618666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/macros/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      117 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.618666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1155 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.618666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.618666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.618666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/profiles.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1250 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/seed_sources.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.618666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/seeds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/seeds/properties.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.618666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/snapshots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.618666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/source_data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2327 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/source_data/items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10472 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9746 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/source_data/orders.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.618666 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/tests/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.618666 sqlmesh-0.8.0/tests/fixtures/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9823 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/migrations/environments.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25229 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/fixtures/migrations/snapshots.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.618666 sqlmesh-0.8.0/tests/schedulers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/schedulers/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.622666 sqlmesh-0.8.0/tests/schedulers/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/schedulers/airflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1414 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/schedulers/airflow/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.622666 sqlmesh-0.8.0/tests/schedulers/airflow/operators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4442 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/schedulers/airflow/operators/test_hwm_sensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4392 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/schedulers/airflow/operators/test_targets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9970 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/schedulers/airflow/test_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/schedulers/airflow/test_end_to_end.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6222 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/schedulers/airflow/test_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6054 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/schedulers/airflow/test_plan.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.622666 sqlmesh-0.8.0/tests/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1118 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/utils/test_cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3580 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/utils/test_concurrency.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6430 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/utils/test_connection_pool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1381 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/utils/test_dag.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1818 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/utils/test_date.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/utils/test_filesystem.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7335 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/utils/test_jinja.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5790 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/utils/test_metaprogramming.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2501 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/utils/test_pandas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/utils/test_pydantic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2911 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/utils/test_transactional_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1194 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/utils/test_yaml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.622666 sqlmesh-0.8.0/tests/web/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/web/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15704 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/tests/web/test_main.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.622666 sqlmesh-0.8.0/web/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.626666 sqlmesh-0.8.0/web/client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/.eslintrc.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       94 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/.prettierignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/.prettierrc.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.626666 sqlmesh-0.8.0/web/client/dist/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.630666 sqlmesh-0.8.0/web/client/dist/assets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74500 2023-05-08 23:29:10.000000 sqlmesh-0.8.0/web/client/dist/assets/CircularStd-Black-52659624.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74368 2023-05-08 23:29:10.000000 sqlmesh-0.8.0/web/client/dist/assets/CircularStd-Bold-0e6c076d.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74116 2023-05-08 23:29:10.000000 sqlmesh-0.8.0/web/client/dist/assets/CircularStd-Medium-2f373e53.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23980 2023-05-08 23:29:10.000000 sqlmesh-0.8.0/web/client/dist/assets/Plan-55e4c139.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    55004 2023-05-08 23:29:10.000000 sqlmesh-0.8.0/web/client/dist/assets/Publico-Black-e6bd2ea2.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    57104 2023-05-08 23:29:10.000000 sqlmesh-0.8.0/web/client/dist/assets/Publico-Bold-c79acd56.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    56836 2023-05-08 23:29:10.000000 sqlmesh-0.8.0/web/client/dist/assets/Publico-Medium-01b4a891.otf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43918 2023-05-08 23:29:10.000000 sqlmesh-0.8.0/web/client/dist/assets/index-5ace865e.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  2657026 2023-05-08 23:29:10.000000 sqlmesh-0.8.0/web/client/dist/assets/index-df610617.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-05-08 23:29:10.000000 sqlmesh-0.8.0/web/client/dist/assets/worker-e891d118.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.630666 sqlmesh-0.8.0/web/client/dist/favicons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2473 2023-05-08 23:29:06.000000 sqlmesh-0.8.0/web/client/dist/favicons/favicon.ico
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1150 2023-05-08 23:29:10.000000 sqlmesh-0.8.0/web/client/dist/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1076 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    40470 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/openapi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      330 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/orval.config.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   408504 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/package-lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2389 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1642 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/playwright.config.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/postcss.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.554666 sqlmesh-0.8.0/web/client/public/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.630666 sqlmesh-0.8.0/web/client/public/favicons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2473 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/public/favicons/favicon.ico
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.630666 sqlmesh-0.8.0/web/client/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.630666 sqlmesh-0.8.0/web/client/src/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/api/channels.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5243 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/api/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3247 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/api/instance.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.554666 sqlmesh-0.8.0/web/client/src/assets/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.554666 sqlmesh-0.8.0/web/client/src/assets/fonts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.634666 sqlmesh-0.8.0/web/client/src/assets/fonts/Circular STD/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74500 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74524 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74368 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    73964 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    68940 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    67284 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    74116 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    73916 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.634666 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    55004 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-Black.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56384 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57104 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    62320 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56652 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61688 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57680 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-Italic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    53148 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-Light.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    57060 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    56836 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-Medium.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61460 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    52820 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-Roman.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    59176 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    63876 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60768 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    81732 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60992 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    64792 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.638666 sqlmesh-0.8.0/web/client/src/context/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4126 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/context/context.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6470 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/context/editor.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      923 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/context/fileTree.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2187 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/context/lineage.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2661 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/context/plan.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1562 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/context/theme.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.638666 sqlmesh-0.8.0/web/client/src/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/hooks/useActiveFocus.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      817 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/hooks/useLocalStorage.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9555 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/index.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.554666 sqlmesh-0.8.0/web/client/src/library/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.554666 sqlmesh-0.8.0/web/client/src/library/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.638666 sqlmesh-0.8.0/web/client/src/library/components/banner/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1705 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/banner/Banner.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.638666 sqlmesh-0.8.0/web/client/src/library/components/button/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4941 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/button/Button.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.638666 sqlmesh-0.8.0/web/client/src/library/components/button/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3516 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/button/tests/Button.spec.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.638666 sqlmesh-0.8.0/web/client/src/library/components/container/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/container/Container.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.638666 sqlmesh-0.8.0/web/client/src/library/components/divider/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/divider/Divider.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.638666 sqlmesh-0.8.0/web/client/src/library/components/divider/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      632 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/divider/tests/Divider.spec.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.638666 sqlmesh-0.8.0/web/client/src/library/components/documentation/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9874 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/documentation/Documentation.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.638666 sqlmesh-0.8.0/web/client/src/library/components/editor/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1992 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/editor/Editor.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9877 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/editor/Editor.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8603 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/editor/EditorCode.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2759 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/editor/EditorFooter.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1990 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/editor/EditorIndicator.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11489 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/editor/EditorInspector.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11927 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/editor/EditorPreview.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3517 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/editor/EditorTabs.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.638666 sqlmesh-0.8.0/web/client/src/library/components/editor/extensions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5664 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5373 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/editor/extensions/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1538 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/editor/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.642666 sqlmesh-0.8.0/web/client/src/library/components/fileTree/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10852 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/fileTree/Directory.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6045 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/fileTree/File.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2624 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/fileTree/FileTree.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      562 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/fileTree/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.642666 sqlmesh-0.8.0/web/client/src/library/components/graph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      159 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/graph/Graph.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14594 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/graph/Graph.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7679 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/graph/help.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.642666 sqlmesh-0.8.0/web/client/src/library/components/input/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2138 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/input/Input.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/input/InputToggle.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.642666 sqlmesh-0.8.0/web/client/src/library/components/loading/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      486 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/loading/Loading.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.642666 sqlmesh-0.8.0/web/client/src/library/components/logo/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2292 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/logo/Spinner.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4637 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/logo/SqlMesh.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8042 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/logo/Tobiko.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.642666 sqlmesh-0.8.0/web/client/src/library/components/modal/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1560 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/modal/Modal.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1953 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/modal/ModalConfirmation.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1447 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/modal/ModalDrawer.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.642666 sqlmesh-0.8.0/web/client/src/library/components/plan/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9210 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/plan/Plan.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6775 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/plan/PlanActions.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/plan/PlanBackfillDates.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10500 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/plan/PlanChangePreview.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4920 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/plan/PlanHeader.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16230 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/plan/PlanWizard.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9926 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12528 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/plan/context.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3444 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/plan/help.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2155 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/plan/help.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2599 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/plan/hooks.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.642666 sqlmesh-0.8.0/web/client/src/library/components/progress/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/progress/Progress.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.646666 sqlmesh-0.8.0/web/client/src/library/components/report/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1047 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/report/ReportTestsErrors.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.646666 sqlmesh-0.8.0/web/client/src/library/components/splitPane/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/splitPane/SplitPane.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      541 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/splitPane/SplitPane.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.646666 sqlmesh-0.8.0/web/client/src/library/components/tasksOverview/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12419 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/tasksOverview/TasksOverview.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.646666 sqlmesh-0.8.0/web/client/src/library/components/toggle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1453 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/components/toggle/Toggle.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.554666 sqlmesh-0.8.0/web/client/src/library/pages/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.646666 sqlmesh-0.8.0/web/client/src/library/pages/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2566 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/pages/docs/Content.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3240 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/pages/docs/Docs.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3947 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/pages/docs/Search.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2283 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/pages/docs/SourceList.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.646666 sqlmesh-0.8.0/web/client/src/library/pages/editor/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2389 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/pages/editor/Editor.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.646666 sqlmesh-0.8.0/web/client/src/library/pages/ide/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4623 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/pages/ide/ActivePlan.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4508 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/pages/ide/IDE.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22083 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/pages/ide/RunPlan.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/pages/ide/context.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.646666 sqlmesh-0.8.0/web/client/src/library/pages/root/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/pages/root/Footer.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1921 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/pages/root/Header.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      843 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/library/pages/root/NotFound.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1516 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/main.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.646666 sqlmesh-0.8.0/web/client/src/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1647 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/models/artifact.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3472 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/models/directory.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4190 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/models/environment.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2330 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/models/file.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      173 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/models/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/models/initial.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1234 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/routes.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.646666 sqlmesh-0.8.0/web/client/src/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/tests/setup.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      541 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/tests/utils.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.646666 sqlmesh-0.8.0/web/client/src/types/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      467 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/types/enum.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/types/index.d.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.650666 sqlmesh-0.8.0/web/client/src/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4102 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/utils/index.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5536 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/utils/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.650666 sqlmesh-0.8.0/web/client/src/workers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/workers/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.650666 sqlmesh-0.8.0/web/client/src/workers/sqlglot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1105 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/workers/sqlglot/sqlglot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1578 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/src/workers/sqlglot/worker.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5879 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/tailwind.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.650666 sqlmesh-0.8.0/web/client/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/tests/initial.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/tsconfig.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1297 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/client/vite.config.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.650666 sqlmesh-0.8.0/web/server/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.650666 sqlmesh-0.8.0/web/server/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/api/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 23:29:21.650666 sqlmesh-0.8.0/web/server/api/endpoints/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      784 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/api/endpoints/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4564 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/api/endpoints/commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      840 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/api/endpoints/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1858 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/api/endpoints/directories.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      721 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/api/endpoints/environments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      637 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/api/endpoints/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5383 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/api/endpoints/files.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3283 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/api/endpoints/lineage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2811 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/api/endpoints/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3635 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/api/endpoints/plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4093 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/console.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6648 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      260 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/openapi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2421 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2114 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/sse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2716 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1003 2023-05-08 23:29:16.000000 sqlmesh-0.8.0/web/server/watcher.py
```

### Comparing `sqlmesh-0.7.1.dev33/.circleci/config.yml` & `sqlmesh-0.8.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/.circleci/continue_config.yml` & `sqlmesh-0.8.0/.circleci/continue_config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/.gitignore` & `sqlmesh-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/.pre-commit-config.yaml` & `sqlmesh-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/LICENSE` & `sqlmesh-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/Makefile` & `sqlmesh-0.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/PKG-INFO` & `sqlmesh-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,14 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.7.1.dev33
-Summary: UNKNOWN
+Version: 0.8.0
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
-Description: ![SQLMesh logo](sqlmesh.svg)
-        
-        SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
-        
-        For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
-        
-        ## Geting Started
-        Install SQLMesh through [pypi](https://pypi.org/project/sqlmesh/) by running:
-        
-        ```pip install sqlmesh```
-        
-        Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
-        
-        ## Join our community
-        We'd love to join you on your data journey. Connect with us in the following ways:
-        
-        * Join the [Tobiko Slack community](https://tobikodata.com/slack) to ask questions, or just to say hi!
-        * File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
-        * Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
-        
-        ## Contribution
-        Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -43,7 +18,31 @@
 Provides-Extra: dbt
 Provides-Extra: github
 Provides-Extra: llm
 Provides-Extra: postgres
 Provides-Extra: redshift
 Provides-Extra: snowflake
 Provides-Extra: web
+License-File: LICENSE
+
+![SQLMesh logo](sqlmesh.svg)
+
+SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
+
+For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
+
+## Geting Started
+Install SQLMesh through [pypi](https://pypi.org/project/sqlmesh/) by running:
+
+```pip install sqlmesh```
+
+Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
+
+## Join our community
+We'd love to join you on your data journey. Connect with us in the following ways:
+
+* Join the [Tobiko Slack community](https://tobikodata.com/slack) to ask questions, or just to say hi!
+* File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
+* Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
+
+## Contribution
+Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
```

### Comparing `sqlmesh-0.7.1.dev33/README.md` & `sqlmesh-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docker-compose.yml` & `sqlmesh-0.8.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/comparisons.md` & `sqlmesh-0.8.0/docs/comparisons.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/concepts/architecture/serialization.md` & `sqlmesh-0.8.0/docs/concepts/architecture/serialization.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/concepts/architecture/snapshots.md` & `sqlmesh-0.8.0/docs/concepts/architecture/snapshots.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/concepts/audits.md` & `sqlmesh-0.8.0/docs/concepts/audits.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/concepts/environments.md` & `sqlmesh-0.8.0/docs/concepts/environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/concepts/glossary.md` & `sqlmesh-0.8.0/docs/concepts/glossary.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/concepts/macros.md` & `sqlmesh-0.8.0/docs/concepts/macros.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/concepts/models/model_kinds.md` & `sqlmesh-0.8.0/docs/concepts/models/model_kinds.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/concepts/models/overview.md` & `sqlmesh-0.8.0/docs/concepts/models/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/concepts/models/python_models.md` & `sqlmesh-0.8.0/docs/concepts/models/python_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/concepts/models/seed_models.md` & `sqlmesh-0.8.0/docs/concepts/models/seed_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/concepts/models/sql_models.md` & `sqlmesh-0.8.0/docs/concepts/models/sql_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/concepts/overview.md` & `sqlmesh-0.8.0/docs/concepts/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/concepts/plans/model_versioning.png` & `sqlmesh-0.8.0/docs/concepts/plans/model_versioning.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/concepts/plans.md` & `sqlmesh-0.8.0/docs/concepts/plans.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/concepts/tests.md` & `sqlmesh-0.8.0/docs/concepts/tests.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/development.md` & `sqlmesh-0.8.0/docs/development.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/guides/connections.md` & `sqlmesh-0.8.0/docs/guides/connections.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/guides/migrations.md` & `sqlmesh-0.8.0/docs/guides/migrations.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/guides/models.md` & `sqlmesh-0.8.0/docs/guides/models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/guides/multi_repo.md` & `sqlmesh-0.8.0/docs/guides/multi_repo.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/guides/projects.md` & `sqlmesh-0.8.0/docs/guides/projects.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/guides/scheduling/airflow_successful_plan_apply.png` & `sqlmesh-0.8.0/docs/guides/scheduling/airflow_successful_plan_apply.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/guides/scheduling/airflow_successful_setup.png` & `sqlmesh-0.8.0/docs/guides/scheduling/airflow_successful_setup.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/guides/scheduling.md` & `sqlmesh-0.8.0/docs/guides/scheduling.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/guides/testing.md` & `sqlmesh-0.8.0/docs/guides/testing.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/index.md` & `sqlmesh-0.8.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/integrations/airflow/airflow_sqlmesh_state_connection.png` & `sqlmesh-0.8.0/docs/integrations/airflow/airflow_sqlmesh_state_connection.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/integrations/airflow.md` & `sqlmesh-0.8.0/docs/integrations/airflow.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/integrations/dbt.md` & `sqlmesh-0.8.0/docs/integrations/dbt.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/integrations/engines.md` & `sqlmesh-0.8.0/docs/integrations/engines.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/integrations/github.md` & `sqlmesh-0.8.0/docs/integrations/github.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # GitHub Actions CI/CD Bot
 
 ## Features
 ### Automated Unit Tests with Error Summary
-![Automated Unit Tests with Error Summary](images/github_test_summary.png)
+![Automated Unit Tests with Error Summary](github/github_test_summary.png)
 ### Automatically create PR Environments that represent the code changes in the PR
-![Environment Summary](images/github_env_summary.png)
+![Environment Summary](github/github_env_summary.png)
 ### Enforce that certain reviewers have approved of the PR before it can be merged
-![Required Approver](images/github_reviewers.png)
+![Required Approver](github/github_reviewers.png)
 ### Preview Prod Plans before Deploying
-![Preview Prod Plans](images/github_prod_plan_preview.png)
+![Preview Prod Plans](github/github_prod_plan_preview.png)
 ### Automatic deployments to production and merge
-![Deployed Plans](images/github_deployed_plans.png)
+![Deployed Plans](github/github_deployed_plans.png)
 
 ### Combined these feature provide
 * The ability to preview what will be deployed to production before it is deployed
 * Gapless deployments to production by ensuring that dates loaded in dev tables match what is currently in production
 * Full transparency into what exists in PR environment and what will be deployed to production - no surprises!
 * The ability to sync your code and your data to ensure what is in your main branch is in production
 
@@ -139,19 +139,19 @@
       # Required to post comments
       issues: write
       # Required to update check runs
       checks: write
       # Required to merge
       pull-requests: write
     env:
-      SQLMESH__CONNECTIONS__DATABRICKS__TYPE: "databricks"
-      SQLMESH__CONNECTIONS__DATABRICKS__SERVER_HOSTNAME: "XXXXXXXXXXXXXXX"
-      SQLMESH__CONNECTIONS__DATABRICKS__HTTP_PATH: "XXXXXXXXXXXX"
-      SQLMESH__CONNECTIONS__DATABRICKS__ACCESS_TOKEN: ${{ secrets.DATABRICKS_TOKEN }}
-      SQLMESH__DEFAULT_CONNECTION: "databricks"
+      SQLMESH__GATEWAYS__DATABRICKS__CONNECTION__TYPE: "databricks"
+      SQLMESH__GATEWAYS__DATABRICKS__CONNECTION__SERVER_HOSTNAME: "XXXXXXXXXXXXXXX"
+      SQLMESH__GATEWAYS__DATABRICKS__CONNECTION__HTTP_PATH: "XXXXXXXXXXXX"
+      SQLMESH__GATEWAYS__DATABRICKS__CONNECTION__ACCESS_TOKEN: ${{ secrets.DATABRICKS_TOKEN }}
+      SQLMESH__DEFAULT_GATEWAY: "databricks"
     steps:
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: '3.9'
       - name: Checkout PR branch
         uses: actions/checkout@v3
```

### Comparing `sqlmesh-0.7.1.dev33/docs/integrations/images/github_deployed_plans.png` & `sqlmesh-0.8.0/docs/integrations/github/github_deployed_plans.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/integrations/images/github_env_summary.png` & `sqlmesh-0.8.0/docs/integrations/github/github_env_summary.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/integrations/images/github_prod_plan_preview.png` & `sqlmesh-0.8.0/docs/integrations/github/github_prod_plan_preview.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/integrations/images/github_reviewers.png` & `sqlmesh-0.8.0/docs/integrations/github/github_reviewers.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/integrations/images/github_test_summary.png` & `sqlmesh-0.8.0/docs/integrations/github/github_test_summary.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/prerequisites.md` & `sqlmesh-0.8.0/docs/prerequisites.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/quick_start.md` & `sqlmesh-0.8.0/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/reference/cli.md` & `sqlmesh-0.8.0/docs/reference/cli.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/reference/configuration.md` & `sqlmesh-0.8.0/docs/reference/configuration.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/reference/notebook.md` & `sqlmesh-0.8.0/docs/reference/notebook.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/reference/overview.md` & `sqlmesh-0.8.0/docs/reference/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/docs/sqlmesh.png` & `sqlmesh-0.8.0/docs/sqlmesh.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/airflow/Dockerfile.template` & `sqlmesh-0.8.0/examples/airflow/Dockerfile.template`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/airflow/Makefile` & `sqlmesh-0.8.0/examples/airflow/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/airflow/README.md` & `sqlmesh-0.8.0/examples/airflow/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/airflow/docker_compose_decorator.py` & `sqlmesh-0.8.0/examples/airflow/docker_compose_decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/airflow/spark_conf/hive-site.xml` & `sqlmesh-0.8.0/examples/airflow/spark_conf/hive-site.xml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/sushi/config.py` & `sqlmesh-0.8.0/examples/sushi/config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/sushi/helper.py` & `sqlmesh-0.8.0/examples/sushi/helper.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/sushi/models/customer_revenue_by_day.sql` & `sqlmesh-0.8.0/examples/sushi/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/sushi/models/items.py` & `sqlmesh-0.8.0/examples/sushi/models/items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/sushi/models/order_items.py` & `sqlmesh-0.8.0/examples/sushi/models/order_items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/sushi/models/orders.py` & `sqlmesh-0.8.0/examples/sushi/models/orders.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/sushi/models/waiter_revenue_by_day.sql` & `sqlmesh-0.8.0/examples/sushi/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/sushi/tests/test_customer_revenue_by_day.yaml` & `sqlmesh-0.8.0/examples/sushi/tests/test_customer_revenue_by_day.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/sushi_dbt/macros/incremental.sql` & `sqlmesh-0.8.0/examples/sushi_dbt/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/sushi_dbt/models/customer_revenue_by_day.sql` & `sqlmesh-0.8.0/examples/sushi_dbt/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/sushi_dbt/models/waiter_revenue_by_day.sql` & `sqlmesh-0.8.0/examples/sushi_dbt/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/sushi_dbt/packages/customers/dbt_project.yml` & `sqlmesh-0.8.0/examples/sushi_dbt/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/sushi_dbt/profiles.yml` & `sqlmesh-0.8.0/examples/sushi_dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/sushi_dbt/seeds/items.csv` & `sqlmesh-0.8.0/examples/sushi_dbt/seeds/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/sushi_dbt/seeds/order_items.csv` & `sqlmesh-0.8.0/examples/sushi_dbt/seeds/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/sushi_dbt/seeds/orders.csv` & `sqlmesh-0.8.0/examples/sushi_dbt/seeds/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/wursthall/macros/macros.py` & `sqlmesh-0.8.0/examples/wursthall/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/wursthall/models/db/order_f.py` & `sqlmesh-0.8.0/examples/wursthall/models/db/order_f.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/wursthall/models/db/order_item_f.sql` & `sqlmesh-0.8.0/examples/wursthall/models/db/order_item_f.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/wursthall/models/src/customer_details.py` & `sqlmesh-0.8.0/examples/wursthall/models/src/customer_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/wursthall/models/src/order_item_details.py` & `sqlmesh-0.8.0/examples/wursthall/models/src/order_item_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/wursthall/models/src/shared.py` & `sqlmesh-0.8.0/examples/wursthall/models/src/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/wursthall/seeds/src/menu_item_details.csv` & `sqlmesh-0.8.0/examples/wursthall/seeds/src/menu_item_details.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/wursthall/tests/test_customer_d.yaml` & `sqlmesh-0.8.0/examples/wursthall/tests/test_customer_d.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/examples/wursthall/tests/test_order_item_f.yaml` & `sqlmesh-0.8.0/examples/wursthall/tests/test_order_item_f.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/mkdocs.yml` & `sqlmesh-0.8.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/pdoc/cli.py` & `sqlmesh-0.8.0/pdoc/cli.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/posts/virtual_data_environments/change_categorization.png` & `sqlmesh-0.8.0/posts/virtual_data_environments/change_categorization.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/posts/virtual_data_environments/isolated_rigid_envs.png` & `sqlmesh-0.8.0/posts/virtual_data_environments/isolated_rigid_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/posts/virtual_data_environments/partial_breaking.png` & `sqlmesh-0.8.0/posts/virtual_data_environments/partial_breaking.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/posts/virtual_data_environments/stateful_envs.png` & `sqlmesh-0.8.0/posts/virtual_data_environments/stateful_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/posts/virtual_data_environments/virtual_envs.png` & `sqlmesh-0.8.0/posts/virtual_data_environments/virtual_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/posts/virtual_data_environments/virtual_envs_end_to_end.png` & `sqlmesh-0.8.0/posts/virtual_data_environments/virtual_envs_end_to_end.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/posts/virtual_data_environments.md` & `sqlmesh-0.8.0/posts/virtual_data_environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/pytest.ini` & `sqlmesh-0.8.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/setup.cfg` & `sqlmesh-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/setup.py` & `sqlmesh-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         "dev": [
             f"apache-airflow=={os.environ.get('AIRFLOW_VERSION', '2.3.3')}",
             "autoflake==1.7.7",
             "google-cloud-bigquery",
             "google-cloud-bigquery-storage",
             "black==22.6.0",
             "dbt-core",
+            "dbt-duckdb",
             "Faker",
             "google-auth",
             "isort==5.10.1",
             "mkdocs-include-markdown-plugin==4.0.3",
             "mkdocs-material==9.0.5",
             "mypy~=1.0.0",
             "ipywidgets",
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/__init__.py` & `sqlmesh-0.8.0/sqlmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/cicd/bot.py` & `sqlmesh-0.8.0/sqlmesh/cicd/bot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/cli/__init__.py` & `sqlmesh-0.8.0/sqlmesh/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/cli/example_project.py` & `sqlmesh-0.8.0/sqlmesh/cli/example_project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/cli/main.py` & `sqlmesh-0.8.0/sqlmesh/cli/main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/cli/options.py` & `sqlmesh-0.8.0/sqlmesh/cli/options.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/audit/builtin.py` & `sqlmesh-0.8.0/sqlmesh/core/audit/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/audit/definition.py` & `sqlmesh-0.8.0/sqlmesh/core/audit/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/config/__init__.py` & `sqlmesh-0.8.0/sqlmesh/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/config/base.py` & `sqlmesh-0.8.0/sqlmesh/core/config/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/config/categorizer.py` & `sqlmesh-0.8.0/sqlmesh/core/config/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/config/common.py` & `sqlmesh-0.8.0/sqlmesh/core/config/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/config/connection.py` & `sqlmesh-0.8.0/sqlmesh/core/config/connection.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/config/gateway.py` & `sqlmesh-0.8.0/sqlmesh/core/config/gateway.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/config/loader.py` & `sqlmesh-0.8.0/sqlmesh/core/config/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/config/model.py` & `sqlmesh-0.8.0/sqlmesh/core/config/model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/config/root.py` & `sqlmesh-0.8.0/sqlmesh/core/config/root.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/config/scheduler.py` & `sqlmesh-0.8.0/sqlmesh/core/config/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/console.py` & `sqlmesh-0.8.0/sqlmesh/core/console.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/constants.py` & `sqlmesh-0.8.0/sqlmesh/core/constants.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/context.py` & `sqlmesh-0.8.0/sqlmesh/core/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -725,14 +725,17 @@
         and the python graphviz library.
 
         Args:
             path: filename to save the dag to
             format: The desired format to use when rending the dag
         """
         graph = self.get_dag(format=format)
+        # We know graphviz is installed because the command above would have failed if it was not. This allows
+        # us to then catch the specific error that occurs when the system install is missing.
+        import graphviz  # type: ignore
 
         try:
             return graph.render(path, format=format)
         except graphviz.backend.execute.ExecutableNotFound as e:
             raise MissingDependencyError(
                 "Graphviz is pip-installed but the system install is missing. Instructions: https://graphviz.org/download/"
             ) from e
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/context_diff.py` & `sqlmesh-0.8.0/sqlmesh/core/context_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/dialect.py` & `sqlmesh-0.8.0/sqlmesh/core/dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/__init__.py` & `sqlmesh-0.8.0/sqlmesh/core/engine_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/_typing.py` & `sqlmesh-0.8.0/sqlmesh/core/engine_adapter/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/base.py` & `sqlmesh-0.8.0/sqlmesh/core/engine_adapter/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/base_postgres.py` & `sqlmesh-0.8.0/sqlmesh/core/engine_adapter/base_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/base_spark.py` & `sqlmesh-0.8.0/sqlmesh/core/engine_adapter/base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/bigquery.py` & `sqlmesh-0.8.0/sqlmesh/core/engine_adapter/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/databricks_api.py` & `sqlmesh-0.8.0/sqlmesh/core/engine_adapter/databricks_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/duckdb.py` & `sqlmesh-0.8.0/sqlmesh/core/engine_adapter/duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/logical_merge.py` & `sqlmesh-0.8.0/sqlmesh/core/engine_adapter/logical_merge.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/postgres.py` & `sqlmesh-0.8.0/sqlmesh/core/engine_adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/redshift.py` & `sqlmesh-0.8.0/sqlmesh/core/engine_adapter/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/shared.py` & `sqlmesh-0.8.0/sqlmesh/core/engine_adapter/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/snowflake.py` & `sqlmesh-0.8.0/sqlmesh/core/engine_adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/engine_adapter/spark.py` & `sqlmesh-0.8.0/sqlmesh/core/engine_adapter/spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/environment.py` & `sqlmesh-0.8.0/sqlmesh/core/environment.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/hooks.py` & `sqlmesh-0.8.0/sqlmesh/core/hooks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/loader.py` & `sqlmesh-0.8.0/sqlmesh/core/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/macros.py` & `sqlmesh-0.8.0/sqlmesh/core/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/model/__init__.py` & `sqlmesh-0.8.0/sqlmesh/core/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/model/cache.py` & `sqlmesh-0.8.0/sqlmesh/core/model/cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/model/common.py` & `sqlmesh-0.8.0/sqlmesh/core/model/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/model/decorator.py` & `sqlmesh-0.8.0/sqlmesh/core/model/decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/model/definition.py` & `sqlmesh-0.8.0/sqlmesh/core/model/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/model/kind.py` & `sqlmesh-0.8.0/sqlmesh/core/model/kind.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/model/meta.py` & `sqlmesh-0.8.0/sqlmesh/core/model/meta.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/model/seed.py` & `sqlmesh-0.8.0/sqlmesh/core/model/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/notification_target.py` & `sqlmesh-0.8.0/sqlmesh/core/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/plan/definition.py` & `sqlmesh-0.8.0/sqlmesh/core/plan/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/plan/evaluator.py` & `sqlmesh-0.8.0/sqlmesh/core/plan/evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/renderer.py` & `sqlmesh-0.8.0/sqlmesh/core/renderer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/scheduler.py` & `sqlmesh-0.8.0/sqlmesh/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/schema_diff.py` & `sqlmesh-0.8.0/sqlmesh/core/schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/snapshot/__init__.py` & `sqlmesh-0.8.0/sqlmesh/core/snapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/snapshot/categorizer.py` & `sqlmesh-0.8.0/sqlmesh/core/snapshot/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/snapshot/definition.py` & `sqlmesh-0.8.0/sqlmesh/core/snapshot/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/snapshot/evaluator.py` & `sqlmesh-0.8.0/sqlmesh/core/snapshot/evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/state_sync/__init__.py` & `sqlmesh-0.8.0/sqlmesh/core/state_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/state_sync/base.py` & `sqlmesh-0.8.0/sqlmesh/core/state_sync/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/state_sync/common.py` & `sqlmesh-0.8.0/sqlmesh/core/state_sync/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/state_sync/engine_adapter.py` & `sqlmesh-0.8.0/sqlmesh/core/state_sync/engine_adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/test.py` & `sqlmesh-0.8.0/sqlmesh/core/test.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/core/user.py` & `sqlmesh-0.8.0/sqlmesh/core/user.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/dbt/adapter.py` & `sqlmesh-0.8.0/sqlmesh/dbt/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,18 @@
 
 
 class BaseAdapter(abc.ABC):
     def __init__(
         self,
         jinja_macros: JinjaMacroRegistry,
         jinja_globals: t.Optional[t.Dict[str, t.Any]] = None,
-        dialect: str = "",
     ):
         self.jinja_macros = jinja_macros
-        self.jinja_globals = jinja_globals or {}
-        self.dialect = dialect
+        self.jinja_globals = jinja_globals.copy() if jinja_globals else {}
+        self.jinja_globals["adapter"] = self
 
     @abc.abstractmethod
     def get_relation(self, database: str, schema: str, identifier: str) -> t.Optional[BaseRelation]:
         """Returns a single relation that matches the provided path."""
 
     @abc.abstractmethod
     def list_relations(self, database: t.Optional[str], schema: str) -> t.List[BaseRelation]:
@@ -74,26 +73,23 @@
 
     @abc.abstractmethod
     def quote(self, identifier: str) -> str:
         """Returns a quoted identifeir."""
 
     def dispatch(self, name: str, package: t.Optional[str] = None) -> t.Callable:
         """Returns a dialect-specific version of a macro with the given name."""
-        dialect_name = f"{self.dialect}__{name}"
-        default_name = f"default__{name}"
-
+        target_type = self.jinja_globals["target"]["type"]
         references_to_try = [
-            MacroReference(package=package, name=dialect_name),
-            MacroReference(package=package, name=default_name),
+            MacroReference(package=f"{package}_{target_type}", name=f"{target_type}__{name}"),
+            MacroReference(package=package, name=f"{target_type}__{name}"),
+            MacroReference(package=package, name=f"default__{name}"),
         ]
 
         for reference in references_to_try:
-            macro_callable = self.jinja_macros.build_macro(
-                reference, **{**self.jinja_globals, "adapter": self}
-            )
+            macro_callable = self.jinja_macros.build_macro(reference, **self.jinja_globals)
             if macro_callable is not None:
                 return macro_callable
 
         raise ConfigError(f"Macro '{name}', package '{package}' was not found.")
 
 
 class ParsetimeAdapter(BaseAdapter):
@@ -137,15 +133,15 @@
         self,
         engine_adapter: EngineAdapter,
         jinja_macros: JinjaMacroRegistry,
         jinja_globals: t.Optional[t.Dict[str, t.Any]] = None,
     ):
         from dbt.adapters.base.relation import Policy
 
-        super().__init__(jinja_macros, jinja_globals=jinja_globals, dialect=engine_adapter.dialect)
+        super().__init__(jinja_macros, jinja_globals=jinja_globals)
 
         self.engine_adapter = engine_adapter
         # All engines quote by default except Snowflake
         quote_param = engine_adapter.DIALECT != "snowflake"
         self.quote_policy = Policy(
             database=quote_param,
             schema=quote_param,
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/dbt/basemodel.py` & `sqlmesh-0.8.0/sqlmesh/dbt/basemodel.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,59 @@
 from __future__ import annotations
 
 import typing as t
 from abc import abstractmethod
 from enum import Enum
 from pathlib import Path
 
-from dbt.adapters.base import BaseRelation
 from dbt.contracts.relation import RelationType
-from jinja2 import nodes
-from jinja2.exceptions import UndefinedError
 from pydantic import Field, validator
 from sqlglot.helper import ensure_list
 
-from sqlmesh.core import constants as c
 from sqlmesh.core import dialect as d
 from sqlmesh.core.config.base import UpdateStrategy
 from sqlmesh.core.model import Model
-from sqlmesh.dbt.adapter import ParsetimeAdapter
 from sqlmesh.dbt.column import (
     ColumnConfig,
     column_descriptions_to_sqlmesh,
     column_types_to_sqlmesh,
-    yaml_to_columns,
 )
 from sqlmesh.dbt.common import DbtConfig, GeneralConfig, QuotingConfig, SqlStr
-from sqlmesh.dbt.context import DbtContext
 from sqlmesh.utils import AttributeDict
 from sqlmesh.utils.conversions import ensure_bool
-from sqlmesh.utils.date import date_dict
 from sqlmesh.utils.errors import ConfigError
-from sqlmesh.utils.jinja import MacroReference, extract_macro_references
+from sqlmesh.utils.jinja import MacroReference
 from sqlmesh.utils.pydantic import PydanticModel
 
+if t.TYPE_CHECKING:
+    from sqlmesh.dbt.context import DbtContext
+
+
 BMC = t.TypeVar("BMC", bound="BaseModelConfig")
 
 
 class Dependencies(PydanticModel):
     """
     DBT dependencies for a model, macro, etc.
 
     Args:
         macros: The references to macros
         sources: The "source_name.table_name" for source tables used
         refs: The table_name for models used
-        variables: The names of variables used, mapped to a flag that indicates whether their
-            definition is optional or not.
     """
 
     macros: t.Set[MacroReference] = set()
     sources: t.Set[str] = set()
     refs: t.Set[str] = set()
-    variables: t.Set[str] = set()
 
     def union(self, other: Dependencies) -> Dependencies:
         dependencies = Dependencies()
         dependencies.macros = self.macros | other.macros
         dependencies.sources = self.sources | other.sources
         dependencies.refs = self.refs | other.refs
-        dependencies.variables = self.variables | other.variables
 
         return dependencies
 
     def dict(self, *args: t.Any, **kwargs: t.Any) -> t.Dict[str, t.Any]:
         # See https://github.com/pydantic/pydantic/issues/1090
         exclude = kwargs.pop("exclude", None) or set()
 
@@ -97,15 +89,14 @@
     Args:
         owner: The owner of the model.
         stamp: An optional arbitrary string sequence used to create new model versions without making
             changes to any of the functional components of the definition.
         storage_format: The storage format used to store the physical table, only applicable in certain engines.
             (eg. 'parquet')
         path: The file path of the model
-        target_schema: The schema for the profile target
         dependencies: The macro, source, var, and ref dependencies used to execute the model and its hooks
         database: Database the model is stored in
         schema: Custom schema name added to the model schema name
         alias: Relation identifier for this model instead of the filename
         pre-hook: List of SQL statements to run before the model is built
         post-hook: List of SQL statements to run after the model is built
         full_refresh: Forces the model to always do a full refresh or never do a full refresh
@@ -115,20 +106,19 @@
     """
 
     # sqlmesh fields
     owner: t.Optional[str] = None
     stamp: t.Optional[str] = None
     storage_format: t.Optional[str] = None
     path: Path = Path()
-    target_schema: str = ""
     dependencies: Dependencies = Dependencies()
 
     # DBT configuration fields
+    schema_: str = Field("", alias="schema")
     database: t.Optional[str] = None
-    schema_: t.Optional[str] = Field(None, alias="schema")
     alias: t.Optional[str] = None
     pre_hook: t.List[Hook] = Field([], alias="pre-hook")
     post_hook: t.List[Hook] = Field([], alias="post-hook")
     full_refresh: t.Optional[bool] = None
     grants: t.Dict[str, t.List[str]] = {}
     columns: t.Dict[str, ColumnConfig] = {}
     quoting: QuotingConfig = Field(default_factory=QuotingConfig)
@@ -152,21 +142,14 @@
     def _validate_bool(cls, v: str) -> bool:
         return ensure_bool(v)
 
     @validator("grants", pre=True)
     def _validate_grants(cls, v: t.Dict[str, str]) -> t.Dict[str, t.List[str]]:
         return {key: ensure_list(value) for key, value in v.items()}
 
-    @validator("columns", pre=True)
-    def _validate_columns(cls, v: t.Any) -> t.Dict[str, ColumnConfig]:
-        if isinstance(v, dict) and all(isinstance(col, ColumnConfig) for col in v.values()):
-            return v
-
-        return yaml_to_columns(v)
-
     _FIELD_UPDATE_STRATEGY: t.ClassVar[t.Dict[str, UpdateStrategy]] = {
         **GeneralConfig._FIELD_UPDATE_STRATEGY,
         **{
             "grants": UpdateStrategy.KEY_EXTEND,
             "path": UpdateStrategy.IMMUTABLE,
             "pre-hook": UpdateStrategy.EXTEND,
             "post-hook": UpdateStrategy.EXTEND,
@@ -193,15 +176,15 @@
         return SqlStr("")
 
     @property
     def table_schema(self) -> str:
         """
         Get the full schema name
         """
-        return "_".join(part for part in (self.target_schema, self.schema_) if part)
+        return self.schema_
 
     @property
     def table_name(self) -> str:
         """
         Get the table name
         """
         return self.alias or self.path.stem
@@ -289,29 +272,14 @@
                 for exp in d.parse(
                     hook.sql, default_dialect=self.model_dialect or model_context.dialect
                 )
             ],
             **optional_kwargs,
         }
 
-    def render_config(self: BMC, context: DbtContext) -> BMC:
-        rendered = super().render_config(context)
-        rendered = ModelSqlRenderer(context, rendered).enriched_config
-
-        rendered_dependencies = rendered.dependencies
-        for dependency in rendered_dependencies.refs:
-            model = context.models.get(dependency)
-            if model and model.materialized == Materialization.EPHEMERAL:
-                rendered.dependencies = rendered.dependencies.union(
-                    model.render_config(context).dependencies
-                )
-                rendered.dependencies.refs.discard(dependency)
-
-        return rendered
-
     @abstractmethod
     def to_sqlmesh(self, context: DbtContext) -> Model:
         """Convert DBT model into sqlmesh Model"""
 
     def _context_for_dependencies(
         self, context: DbtContext, dependencies: Dependencies
     ) -> DbtContext:
@@ -334,139 +302,9 @@
                 sources[source] = context.sources[source]
             else:
                 raise ConfigError(f"Source '{source}' was not found for model '{self.table_name}'.")
 
         model_context.sources = sources
         model_context.seeds = seeds
         model_context.models = models
-        model_context.variables = {
-            name: value
-            for name, value in context.variables.items()
-            if name in dependencies.variables
-        }
 
         return model_context
-
-
-class ModelSqlRenderer(t.Generic[BMC]):
-    def __init__(self, context: DbtContext, config: BMC):
-        from sqlmesh.dbt.builtin import create_builtin_globals
-
-        self.context = context
-        self.config = config
-
-        self._captured_dependencies: Dependencies = Dependencies()
-        self._rendered_sql: t.Optional[str] = None
-        self._enriched_config: BMC = config.copy()
-
-        self._jinja_globals = create_builtin_globals(
-            jinja_macros=context.jinja_macros,
-            jinja_globals={
-                **context.jinja_globals,
-                **date_dict(c.EPOCH, c.EPOCH, c.EPOCH),
-                "config": lambda *args, **kwargs: "",
-                "ref": self._ref,
-                "var": self._var,
-                "source": self._source,
-                "this": self.config.relation_info,
-                "model": self.config.model_function(),
-                "schema": self.config.table_schema,
-            },
-            engine_adapter=None,
-        )
-
-        # Set the adapter separately since it requires jinja globals to passed into it.
-        self._jinja_globals["adapter"] = ModelSqlRenderer.TrackingAdapter(
-            self,
-            context.jinja_macros,
-            jinja_globals=self._jinja_globals,
-            dialect=context.engine_adapter.dialect if context.engine_adapter else "",
-        )
-
-        self.jinja_env = self.context.jinja_macros.build_environment(**self._jinja_globals)
-
-    @property
-    def enriched_config(self) -> BMC:
-        if self._rendered_sql is None:
-            self._enriched_config = self._update_with_sql_config(self._enriched_config)
-            self._enriched_config.dependencies = Dependencies(
-                macros=extract_macro_references(self._enriched_config.all_sql)
-            )
-            self.render()
-            self._enriched_config.dependencies = self._enriched_config.dependencies.union(
-                self._captured_dependencies
-            )
-        return self._enriched_config
-
-    def render(self) -> str:
-        if self._rendered_sql is None:
-            try:
-                self._rendered_sql = self.jinja_env.from_string(
-                    self._enriched_config.all_sql
-                ).render()
-            except UndefinedError as e:
-                raise ConfigError(e.message)
-        return self._rendered_sql
-
-    def _update_with_sql_config(self, config: BMC) -> BMC:
-        def _extract_value(node: t.Any) -> t.Any:
-            if not isinstance(node, nodes.Node):
-                return node
-            if isinstance(node, nodes.Const):
-                return _extract_value(node.value)
-            if isinstance(node, nodes.TemplateData):
-                return _extract_value(node.data)
-            if isinstance(node, nodes.List):
-                return [_extract_value(val) for val in node.items]
-            if isinstance(node, nodes.Dict):
-                return {_extract_value(pair.key): _extract_value(pair.value) for pair in node.items}
-            if isinstance(node, nodes.Tuple):
-                return tuple(_extract_value(val) for val in node.items)
-
-            return self.jinja_env.from_string(nodes.Template([nodes.Output([node])])).render()
-
-        for call in self.jinja_env.parse(self._enriched_config.sql_embedded_config).find_all(
-            nodes.Call
-        ):
-            if not isinstance(call.node, nodes.Name) or call.node.name != "config":
-                continue
-            config = config.update_with(
-                {kwarg.key: _extract_value(kwarg.value) for kwarg in call.kwargs}
-            )
-
-        return config
-
-    def _ref(self, package_name: str, model_name: t.Optional[str] = None) -> BaseRelation:
-        self._captured_dependencies.refs.add(package_name)
-        return BaseRelation.create()
-
-    def _var(self, name: str, default: t.Optional[str] = None) -> t.Any:
-        if default is None and name not in self.context.variables:
-            raise ConfigError(
-                f"Variable '{name}' was not found for model '{self.config.table_name}'."
-            )
-        self._captured_dependencies.variables.add(name)
-        return self.context.variables.get(name, default)
-
-    def _source(self, source_name: str, table_name: str) -> BaseRelation:
-        full_name = ".".join([source_name, table_name])
-        self._captured_dependencies.sources.add(full_name)
-        return BaseRelation.create()
-
-    class TrackingAdapter(ParsetimeAdapter):
-        def __init__(self, outer_self: ModelSqlRenderer, *args: t.Any, **kwargs: t.Any):
-            super().__init__(*args, **kwargs)
-            self.outer_self = outer_self
-            self.context = outer_self.context
-
-        def dispatch(self, name: str, package: t.Optional[str] = None) -> t.Callable:
-            macros = (
-                self.context.jinja_macros.packages.get(package, {})
-                if package is not None
-                else self.context.jinja_macros.root_macros
-            )
-            for target_name in macros:
-                if target_name.endswith(f"__{name}"):
-                    self.outer_self._captured_dependencies.macros.add(
-                        MacroReference(package=package, name=target_name)
-                    )
-            return super().dispatch(name, package=package)
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/dbt/builtin.py` & `sqlmesh-0.8.0/sqlmesh/dbt/builtin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from __future__ import annotations
 
 import json
 import os
-import sys
 import typing as t
 from ast import literal_eval
-from pathlib import Path
 
 import agate
 import jinja2
+from dbt import version
 from dbt.adapters.base import BaseRelation
 from dbt.contracts.relation import Policy
 from ruamel.yaml import YAMLError
 
 from sqlmesh.core.engine_adapter import EngineAdapter
 from sqlmesh.dbt.adapter import ParsetimeAdapter, RuntimeAdapter
-from sqlmesh.dbt.context import DbtContext
-from sqlmesh.dbt.package import PackageLoader
 from sqlmesh.utils import AttributeDict, yaml
 from sqlmesh.utils.errors import ConfigError, MacroEvalError
 from sqlmesh.utils.jinja import JinjaMacroRegistry, MacroReturnVal
 
 
 class Exceptions:
     def raise_compiler_error(self, msg: str) -> None:
@@ -246,38 +243,17 @@
 def _try_literal_eval(value: str) -> t.Any:
     try:
         return literal_eval(value)
     except (ValueError, SyntaxError, MemoryError):
         return value
 
 
-def _dbt_macro_registry() -> JinjaMacroRegistry:
-    registry = JinjaMacroRegistry()
-
-    try:
-        site_packages = next(
-            p for p in sys.path if "site-packages" in p and Path(p, "dbt").exists()
-        )
-    except:
-        return registry
-
-    for project_file in Path(site_packages).glob("dbt/include/*/dbt_project.yml"):
-        if project_file.parent.stem == "starter_project":
-            continue
-        context = DbtContext(project_root=project_file.parent, jinja_macros=JinjaMacroRegistry())
-        package = PackageLoader(context).load()
-        registry.add_macros(package.macro_infos, package="dbt")
-
-    return registry
-
-
-DBT_MACRO_REGISTRY = _dbt_macro_registry()
-
 BUILTIN_GLOBALS = {
     "api": Api(),
+    "dbt_version": version.__version__,
     "env_var": env_var,
     "exceptions": Exceptions(),
     "flags": Flags(),
     "fromjson": from_json,
     "fromyaml": from_yaml,
     "is_incremental": is_incremental,
     "log": no_log,
@@ -363,18 +339,12 @@
                 "run_query": lambda *args, **kwargs: None,
                 "statement": lambda *args, **kwargs: "",
                 "log": no_log,
                 "print": no_log,
             }
         )
 
-    builtin_globals.update(jinja_globals)
-    if "dbt" not in builtin_globals:
-        builtin_globals["dbt"] = DBT_MACRO_REGISTRY.build_environment(
-            **builtin_globals
-        ).globals.get("dbt", {})
-
-    return builtin_globals
+    return {**builtin_globals, **jinja_globals}
 
 
 def create_builtin_filters() -> t.Dict[str, t.Callable]:
     return BUILTIN_FILTERS
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/dbt/column.py` & `sqlmesh-0.8.0/sqlmesh/dbt/column.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/dbt/common.py` & `sqlmesh-0.8.0/sqlmesh/dbt/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 from sqlglot.helper import ensure_list
 
 from sqlmesh.core.config.base import BaseConfig, UpdateStrategy
 from sqlmesh.utils.conversions import ensure_bool, try_str_to_bool
 from sqlmesh.utils.errors import ConfigError
 from sqlmesh.utils.yaml import load
 
-if t.TYPE_CHECKING:
-    from sqlmesh.dbt.context import DbtContext
-
-
 T = t.TypeVar("T", bound="GeneralConfig")
 
 
 PROJECT_FILENAME = "dbt_project.yml"
 
 JINJA_ONLY = {
     "adapter",
@@ -62,14 +58,18 @@
 
 
 class QuotingConfig(DbtConfig):
     database: bool = True
     schema_: bool = Field(True, alias="schema")
     identifier: bool = True
 
+    @validator("database", "schema_", "identifier", pre=True)
+    def _validate_bool(cls, v: str) -> bool:
+        return ensure_bool(v)
+
 
 class GeneralConfig(DbtConfig):
     """
     General DBT configuration properties for models, sources, seeds, columns, etc.
 
     Args:
         description: Description of element
@@ -133,35 +133,7 @@
         Replace the contents of this instance with the passed in instance.
 
         Args:
             other: The instance to apply to this instance
         """
         for field in other.__fields_set__:
             setattr(self, field, getattr(other, field))
-
-    def render_config(self: T, context: DbtContext) -> T:
-        def render_value(val: t.Any) -> t.Any:
-            if type(val) is not SqlStr and type(val) is str:
-                val = context.render(val)
-            elif isinstance(val, GeneralConfig):
-                for name in val.__fields__:
-                    setattr(val, name, render_value(getattr(val, name)))
-            elif isinstance(val, list):
-                for i in range(len(val)):
-                    val[i] = render_value(val[i])
-            elif isinstance(val, set):
-                for set_val in val:
-                    val.remove(set_val)
-                    val.add(render_value(set_val))
-            elif isinstance(val, dict):
-                for k in val:
-                    val[k] = render_value(val[k])
-
-            return val
-
-        rendered = self.copy(deep=True)
-        for name in rendered.__fields__:
-            value = getattr(rendered, name)
-            if value is not None:
-                setattr(rendered, name, render_value(value))
-
-        return rendered
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/dbt/context.py` & `sqlmesh-0.8.0/sqlmesh/dbt/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import typing as t
 from dataclasses import dataclass, field, replace
 from pathlib import Path
 
 from sqlmesh.core.engine_adapter import EngineAdapter
+from sqlmesh.dbt.manifest import ManifestHelper
 from sqlmesh.dbt.target import TargetConfig
 from sqlmesh.utils import AttributeDict
-from sqlmesh.utils.errors import ConfigError
+from sqlmesh.utils.errors import ConfigError, SQLMeshError
 from sqlmesh.utils.jinja import JinjaGlobalAttribute, JinjaMacroRegistry
 
 if t.TYPE_CHECKING:
     from jinja2 import Environment
 
     from sqlmesh.dbt.model import ModelConfig
     from sqlmesh.dbt.seed import SeedConfig
@@ -20,38 +21,61 @@
 
 @dataclass
 class DbtContext:
     """Context for DBT environment"""
 
     project_root: Path = Path()
     target_name: t.Optional[str] = None
-    project_name: t.Optional[str] = None
     profile_name: t.Optional[str] = None
     project_schema: t.Optional[str] = None
     jinja_macros: JinjaMacroRegistry = field(
-        default_factory=lambda: JinjaMacroRegistry(create_builtins_module="sqlmesh.dbt")
+        default_factory=lambda: JinjaMacroRegistry(
+            create_builtins_module="sqlmesh.dbt", top_level_packages=["dbt"]
+        )
     )
 
     engine_adapter: t.Optional[EngineAdapter] = None
 
+    _project_name: t.Optional[str] = None
     _variables: t.Dict[str, t.Any] = field(default_factory=dict)
     _models: t.Dict[str, ModelConfig] = field(default_factory=dict)
     _seeds: t.Dict[str, SeedConfig] = field(default_factory=dict)
     _sources: t.Dict[str, SourceConfig] = field(default_factory=dict)
     _refs: t.Dict[str, str] = field(default_factory=dict)
 
     _target: t.Optional[TargetConfig] = None
 
     _jinja_environment: t.Optional[Environment] = None
 
+    _manifest: t.Optional[ManifestHelper] = None
+
     @property
     def dialect(self) -> str:
         return self.engine_adapter.dialect if self.engine_adapter is not None else ""
 
     @property
+    def project_name(self) -> t.Optional[str]:
+        return self._project_name
+
+    @project_name.setter
+    def project_name(self, project_name: str) -> None:
+        self._project_name = project_name
+        self.jinja_macros.root_package_name = project_name
+
+    @property
+    def manifest(self) -> ManifestHelper:
+        if self._manifest is None:
+            raise SQLMeshError("Manifest is not set in the context.")
+        return self._manifest
+
+    @manifest.setter
+    def manifest(self, mainfest: ManifestHelper) -> None:
+        self._manifest = mainfest
+
+    @property
     def variables(self) -> t.Dict[str, t.Any]:
         return self._variables
 
     @variables.setter
     def variables(self, variables: t.Dict[str, t.Any]) -> None:
         self._variables = {}
         self.add_variables(variables)
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/dbt/loader.py` & `sqlmesh-0.8.0/sqlmesh/dbt/loader.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,21 +9,18 @@
 from sqlmesh.core.config import Config, GatewayConfig
 from sqlmesh.core.hooks import HookRegistry
 from sqlmesh.core.loader import Loader
 from sqlmesh.core.macros import MacroRegistry
 from sqlmesh.core.model import Model, ModelCache
 from sqlmesh.dbt.basemodel import BMC, BaseModelConfig
 from sqlmesh.dbt.context import DbtContext
-from sqlmesh.dbt.model import ModelConfig
 from sqlmesh.dbt.profile import Profile
 from sqlmesh.dbt.project import Project
-from sqlmesh.dbt.seed import SeedConfig
 from sqlmesh.dbt.target import TargetConfig
 from sqlmesh.utils import UniqueKeyDict
-from sqlmesh.utils.cache import FileCache
 
 logger = logging.getLogger(__name__)
 
 
 def sqlmesh_config(project_root: t.Optional[Path] = None, **kwargs: t.Any) -> Config:
     project_root = project_root or Path()
     context = DbtContext(project_root=project_root)
@@ -62,49 +59,36 @@
             self._track_file(path)
 
         context = project.context.copy()
 
         macros_mtimes: t.List[float] = []
 
         for package_name, package in project.packages.items():
-            context.jinja_macros.add_macros(
-                package.macro_infos,
-                package=package_name if package_name != context.project_name else None,
-            )
+            context.variables = package.variables
+            context.add_sources(package.sources)
+            context.add_seeds(package.seeds)
+            context.add_models(package.models)
             macros_mtimes.extend(
                 [
                     self._path_mtimes[m.path]
                     for m in package.macros.values()
                     if m.path in self._path_mtimes
                 ]
             )
 
+        for package_name, macro_infos in context.manifest.all_macros.items():
+            context.jinja_macros.add_macros(
+                macro_infos,
+                package=package_name if package_name != context.project_name else None,
+            )
+
         macros_max_mtime = max(macros_mtimes) if macros_mtimes else None
         yaml_max_mtimes = self._compute_yaml_max_mtime_per_subfolder(self._context.path)
         cache = DbtLoader._Cache(self, project, macros_max_mtime, yaml_max_mtimes)
 
-        # First render all the config and discover dependencies
-        logger.info("Rendering model configs")
-        for package in project.packages.values():
-            context.variables = package.variables
-
-            package.sources = {k: v.render_config(context) for k, v in package.sources.items()}
-            package.seeds = {
-                k: cache.get_or_load_seed_config(v.path, lambda: self._render_config(v, context))
-                for k, v in package.seeds.items()
-            }
-            package.models = {
-                k: cache.get_or_load_model_config(v.path, lambda: self._render_config(v, context))
-                for k, v in package.models.items()
-            }
-
-            context.add_sources(package.sources)
-            context.add_seeds(package.seeds)
-            context.add_models(package.models)
-
         logger.info("Converting models to sqlmesh")
         # Now that config is rendered, create the sqlmesh models
         for package in project.packages.values():
             context.variables = package.variables
             package_models: t.Dict[str, BaseModelConfig] = {**package.models, **package.seeds}
 
             models.update(
@@ -118,19 +102,14 @@
 
         return models
 
     def _load_audits(self) -> UniqueKeyDict[str, Audit]:
         return UniqueKeyDict("audits")
 
     @classmethod
-    def _render_config(cls, config: BMC, context: DbtContext) -> BMC:
-        logger.info(f"Rendering config for {config.model_name}")
-        return config.render_config(context)
-
-    @classmethod
     def _to_sqlmesh(cls, config: BMC, context: DbtContext) -> Model:
         logger.info(f"Converting {config.model_name} to sqlmesh format")
         return config.to_sqlmesh(context)
 
     def _compute_yaml_max_mtime_per_subfolder(self, root: Path) -> t.Dict[Path, float]:
         if not root.is_dir():
             return {}
@@ -163,36 +142,20 @@
             self._project = project
             self._macros_max_mtime = macros_max_mtime
             self._yaml_max_mtimes = yaml_max_mtimes
 
             target = t.cast(TargetConfig, project.context.target)
             cache_path = loader._context.path / c.CACHE / target.name
             self._model_cache = ModelCache(cache_path)
-            self._model_config_cache = FileCache(cache_path, ModelConfig, prefix="model_config")
-            self._seed_config_cache = FileCache(cache_path, SeedConfig, prefix="seed_config")
 
         def get_or_load_model(self, target_path: Path, loader: t.Callable[[], Model]) -> Model:
             return self._model_cache.get_or_load(
                 self._cache_entry_name(target_path), self._cache_entry_id(target_path), loader
             )
 
-        def get_or_load_model_config(
-            self, target_path: Path, loader: t.Callable[[], ModelConfig]
-        ) -> ModelConfig:
-            return self._model_config_cache.get_or_load(
-                self._cache_entry_name(target_path), self._cache_entry_id(target_path), loader
-            )
-
-        def get_or_load_seed_config(
-            self, target_path: Path, loader: t.Callable[[], SeedConfig]
-        ) -> SeedConfig:
-            return self._seed_config_cache.get_or_load(
-                self._cache_entry_name(target_path), self._cache_entry_id(target_path), loader
-            )
-
         def _cache_entry_name(self, target_path: Path) -> str:
             try:
                 path_for_name = target_path.absolute().relative_to(
                     self._project.context.project_root.absolute()
                 )
             except ValueError:
                 path_for_name = target_path
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/dbt/model.py` & `sqlmesh-0.8.0/sqlmesh/dbt/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,20 @@
     Model,
     ModelKind,
     ModelKindName,
     create_sql_model,
 )
 from sqlmesh.dbt.basemodel import BaseModelConfig, Materialization
 from sqlmesh.dbt.common import SqlStr
-from sqlmesh.dbt.context import DbtContext
 from sqlmesh.dbt.target import TargetConfig
 from sqlmesh.utils.errors import ConfigError
 
+if t.TYPE_CHECKING:
+    from sqlmesh.dbt.context import DbtContext
+
 INCREMENTAL_BY_TIME_STRATEGIES = set(["delete+insert", "insert_overwrite"])
 INCREMENTAL_BY_UNIQUE_KEY_STRATEGIES = set(["merge"])
 
 
 def collection_to_str(collection: t.Iterable) -> str:
     return ", ".join(f"'{item}'" for item in collection)
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/dbt/profile.py` & `sqlmesh-0.8.0/sqlmesh/dbt/profile.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/dbt/project.py` & `sqlmesh-0.8.0/sqlmesh/dbt/project.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import logging
 import typing as t
 from pathlib import Path
 
 from sqlmesh.dbt.common import PROJECT_FILENAME, load_yaml
 from sqlmesh.dbt.context import DbtContext
-from sqlmesh.dbt.package import Package, PackageLoader, ProjectConfig
+from sqlmesh.dbt.manifest import ManifestHelper
+from sqlmesh.dbt.package import Package, PackageLoader
 from sqlmesh.dbt.profile import Profile
 from sqlmesh.utils.errors import ConfigError
 
 logger = logging.getLogger(__name__)
 
 
 class Project:
@@ -53,94 +54,59 @@
         project_yaml = load_yaml(project_file_path)
 
         variables = project_yaml.get("vars", {})
         context.variables = {
             name: var for name, var in variables.items() if not isinstance(var, t.Dict)
         }
 
-        context.project_name = context.render(project_yaml.get("name", ""))
+        project_name = context.render(project_yaml.get("name", ""))
+        context.project_name = project_name
         if not context.project_name:
             raise ConfigError(f"{project_file_path.stem} must include project name.")
 
-        context.profile_name = (
-            context.render(project_yaml.get("profile", "")) or context.project_name
-        )
+        profile_name = context.render(project_yaml.get("profile", "")) or context.project_name
+        context.profile_name = profile_name
 
         profile = Profile.load(context, context.target_name)
         context.target = profile.target
 
+        context.manifest = ManifestHelper(
+            project_file_path.parent, profile.path.parent, profile_name, target=profile.target_name
+        )
+
         extra_fields = profile.target.extra
         if extra_fields:
             extra_str = ",".join(f"'{field}'" for field in extra_fields)
             logger.warning(
                 "%s adapter does not currently support %s", profile.target.type, extra_str
             )
 
         packages = {}
-        root_loader = PackageLoader(context, ProjectConfig())
+        package_loader = PackageLoader(context)
 
-        packages[context.project_name] = root_loader.load()
-        project_config = root_loader.project_config
+        packages[context.project_name] = package_loader.load(context.project_root)
 
         packages_dir = Path(
             context.render(project_yaml.get("packages-install-path", "dbt_packages"))
         )
         if not packages_dir.is_absolute():
             packages_dir = Path(context.project_root, packages_dir)
 
         for path in packages_dir.glob(f"*/{PROJECT_FILENAME}"):
-            name = context.render(load_yaml(path).get("name", ""))
-            if not name:
-                raise ConfigError(f"{path} must include package name")
-
-            package_context = context.copy()
-            package_context.project_root = path.parent
-            package_context.variables = {}
-            packages[name] = PackageLoader(
-                package_context, cls._overrides_for_package(name, project_config)
-            ).load()
+            package = package_loader.load(path.parent)
+            packages[package.name] = package
 
         for name, package in packages.items():
             package_vars = variables.get(name)
 
             if isinstance(package_vars, dict):
                 package.variables.update(package_vars)
 
         return Project(context, profile, packages)
 
-    @classmethod
-    def _overrides_for_package(cls, name: str, config: ProjectConfig) -> ProjectConfig:
-        overrides = ProjectConfig()
-
-        source_overrides = {
-            scope[1:]: value
-            for scope, value in config.source_config.items()
-            if scope and scope[0] == name
-        }
-        if source_overrides:
-            overrides.source_config = source_overrides
-
-        seed_overrides = {
-            scope[1:]: value
-            for scope, value in config.seed_config.items()
-            if scope and scope[0] == name
-        }
-        if seed_overrides:
-            overrides.seed_config = seed_overrides
-
-        model_overrides = {
-            scope[1:]: value
-            for scope, value in config.model_config.items()
-            if scope and scope[0] == name
-        }
-        if model_overrides:
-            overrides.model_config = model_overrides
-
-        return overrides
-
     @property
     def project_files(self) -> t.Set[Path]:
         paths = {self.profile.path}
         for package in self.packages.values():
             paths.update(package.files)
 
         return paths
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/dbt/seed.py` & `sqlmesh-0.8.0/sqlmesh/dbt/seed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from __future__ import annotations
 
+import typing as t
+
 from sqlmesh.core.model import Model, SeedKind, create_seed_model
 from sqlmesh.dbt.basemodel import BaseModelConfig
-from sqlmesh.dbt.context import DbtContext
+
+if t.TYPE_CHECKING:
+    from sqlmesh.dbt.context import DbtContext
 
 
 class SeedConfig(BaseModelConfig):
     """
     seedConfig contains all config parameters available to DBT seeds
 
     See https://docs.getdbt.com/reference/configs-and-properties for
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/dbt/source.py` & `sqlmesh-0.8.0/sqlmesh/dbt/source.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import typing as t
 
 from dbt.contracts.relation import RelationType
-from pydantic import Field, validator
+from pydantic import Field
 
 from sqlmesh.core.config.base import UpdateStrategy
-from sqlmesh.dbt.column import ColumnConfig, yaml_to_columns
+from sqlmesh.dbt.column import ColumnConfig
 from sqlmesh.dbt.common import GeneralConfig, QuotingConfig
 from sqlmesh.utils import AttributeDict
 
 
 class SourceConfig(GeneralConfig):
     """
     Args:
@@ -40,21 +40,14 @@
     overrides: t.Optional[str] = None
     freshness: t.Optional[t.Dict[str, t.Any]] = {}
     loaded_at_field: t.Optional[str] = None
     quoting: QuotingConfig = Field(default_factory=QuotingConfig)
     external: t.Optional[t.Dict[str, t.Any]] = {}
     columns: t.Dict[str, ColumnConfig] = {}
 
-    @validator("columns", pre=True)
-    def _validate_columns(cls, v: t.Any) -> t.Dict[str, ColumnConfig]:
-        if not isinstance(v, dict) or all(isinstance(col, ColumnConfig) for col in v.values()):
-            return v
-
-        return yaml_to_columns(v)
-
     _FIELD_UPDATE_STRATEGY: t.ClassVar[t.Dict[str, UpdateStrategy]] = {
         **GeneralConfig._FIELD_UPDATE_STRATEGY,
         **{"columns": UpdateStrategy.KEY_EXTEND},
     }
 
     @property
     def table_name(self) -> t.Optional[str]:
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/dbt/target.py` & `sqlmesh-0.8.0/sqlmesh/dbt/target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/engines/commands.py` & `sqlmesh-0.8.0/sqlmesh/engines/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/engines/spark/app.py` & `sqlmesh-0.8.0/sqlmesh/engines/spark/app.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/engines/spark/db_api/spark_session.py` & `sqlmesh-0.8.0/sqlmesh/engines/spark/db_api/spark_session.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/integrations/github/cicd/command.py` & `sqlmesh-0.8.0/sqlmesh/integrations/github/cicd/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,16 @@
 
 def _run_tests(controller: GithubController) -> bool:
     controller.update_test_check(status=GithubCheckStatus.IN_PROGRESS)
     try:
         result, failed_output = controller.run_tests()
         controller.update_test_check(
             status=GithubCheckStatus.COMPLETED,
+            # Conclusion will be updated with final status based on test results
+            conclusion=GithubCheckConclusion.NEUTRAL,
             result=result,
             failed_output=failed_output,
         )
         return result.wasSuccessful()
     except Exception:
         controller.update_test_check(
             status=GithubCheckStatus.COMPLETED, conclusion=GithubCheckConclusion.FAILURE
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/integrations/github/cicd/controller.py` & `sqlmesh-0.8.0/sqlmesh/integrations/github/cicd/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import functools
 import json
 import logging
 import os
 import pathlib
 import re
 import typing as t
 import unittest
@@ -21,15 +22,14 @@
 from sqlmesh.core.plan import LoadedSnapshotIntervals, Plan
 from sqlmesh.core.user import User
 from sqlmesh.utils.date import now
 from sqlmesh.utils.errors import CICDBotError, PlanError
 from sqlmesh.utils.pydantic import PydanticModel
 
 if t.TYPE_CHECKING:
-    from github import Github
     from github.CheckRun import CheckRun
     from github.Issue import Issue
     from github.PullRequest import PullRequest
     from github.PullRequestReview import PullRequestReview
     from github.Repository import Repository
 
     from sqlmesh.core.config import Config
@@ -171,14 +171,16 @@
     def __init__(
         self,
         paths: t.Union[str, t.Iterable[str]],
         token: str,
         config: t.Optional[t.Union[Config, str]] = None,
         event: t.Optional[GithubEvent] = None,
     ) -> None:
+        from github import Github
+
         self._paths = paths
         self._config = config
         self._token = token
         self._event = event or GithubEvent.from_env()
         self._pr_plan: t.Optional[Plan] = None
         self._prod_plan: t.Optional[Plan] = None
         self._prod_plan_with_gaps: t.Optional[Plan] = None
@@ -442,15 +444,15 @@
         failed_output: t.Optional[str] = None,
     ) -> None:
         """
         Updates the status of tests for code in the PR
         """
 
         def conclusion_handler(
-            _: GithubCheckConclusion,
+            _: GithubCheckConclusion, result: unittest.result.TestResult, failed_output: str
         ) -> t.Tuple[GithubCheckConclusion, str, t.Optional[str]]:
             if not result:
                 return GithubCheckConclusion.SKIPPED, "Skipped Tests", None
             self.console.log_test_results(
                 result, failed_output or "", self._context._test_engine_adapter.dialect
             )
             test_summary = self.console.consume_captured_output()
@@ -469,15 +471,17 @@
             status_handler=lambda status: (
                 {
                     GithubCheckStatus.IN_PROGRESS: "Running Tests",
                     GithubCheckStatus.QUEUED: "Waiting to Run Tests",
                 }[status],
                 None,
             ),
-            conclusion_handler=conclusion_handler,
+            conclusion_handler=functools.partial(
+                conclusion_handler, result=result, failed_output=failed_output
+            ),
         )
 
     def update_required_approval_check(
         self, status: GithubCheckStatus, conclusion: t.Optional[GithubCheckConclusion] = None
     ) -> None:
         """
         Updates the status of the merge commit for the required approval.
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/integrations/llm.py` & `sqlmesh-0.8.0/sqlmesh/integrations/llm.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/magics.py` & `sqlmesh-0.8.0/sqlmesh/magics.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/migrations/v0001_init.py` & `sqlmesh-0.8.0/sqlmesh/migrations/v0001_init.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/migrations/v0003_move_batch_size.py` & `sqlmesh-0.8.0/sqlmesh/migrations/v0003_move_batch_size.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py` & `sqlmesh-0.8.0/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/api.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/client.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/client.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/common.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/dag_generator.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/dag_generator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/hooks/bigquery.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/hooks/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/hooks/redshift.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/hooks/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/integration.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/bigquery.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/databricks.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/hwm_sensor.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/notification.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/notification.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/postgres.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/redshift.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/snowflake.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/spark_submit.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/spark_submit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/operators/targets.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/operators/targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/plan.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/plugin.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/plugin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/state_sync.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/state_sync.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/schedulers/airflow/util.py` & `sqlmesh-0.8.0/sqlmesh/schedulers/airflow/util.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/utils/__init__.py` & `sqlmesh-0.8.0/sqlmesh/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import re
 import sys
 import traceback
 import types
 import typing as t
 import uuid
 from contextlib import contextmanager
+from copy import deepcopy
 from functools import wraps
 from pathlib import Path
 
 T = t.TypeVar("T")
 KEY = t.TypeVar("KEY", bound=t.Hashable)
 VALUE = t.TypeVar("VALUE")
 DECORATOR_RETURN_TYPE = t.TypeVar("DECORATOR_RETURN_TYPE")
@@ -59,14 +60,21 @@
             )
         super().__setitem__(k, v)
 
 
 class AttributeDict(dict, t.Mapping[KEY, VALUE]):
     __getattr__ = dict.get
 
+    def __deepcopy__(self, memo: t.Dict[t.Any, AttributeDict]) -> AttributeDict:
+        copy: AttributeDict = AttributeDict()
+        memo[id(self)] = copy
+        for k, v in self.items():
+            copy[k] = deepcopy(v, memo)
+        return copy
+
 
 class registry_decorator:
     """A decorator that registers itself."""
 
     registry_name = ""
     _registry: t.Optional[UniqueKeyDict] = None
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/utils/cache.py` & `sqlmesh-0.8.0/sqlmesh/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/utils/concurrency.py` & `sqlmesh-0.8.0/sqlmesh/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/utils/connection_pool.py` & `sqlmesh-0.8.0/sqlmesh/utils/connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/utils/dag.py` & `sqlmesh-0.8.0/sqlmesh/utils/dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/utils/date.py` & `sqlmesh-0.8.0/sqlmesh/utils/date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/utils/errors.py` & `sqlmesh-0.8.0/sqlmesh/utils/errors.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/utils/jinja.py` & `sqlmesh-0.8.0/sqlmesh/utils/jinja.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,26 +44,14 @@
 
 
 class MacroReturnVal(Exception):
     def __init__(self, val: t.Any):
         self.value = val
 
 
-def macro_return(macro: t.Callable) -> t.Callable:
-    """Decorator to pass data back to the caller"""
-
-    def wrapper(*args: t.Any, **kwargs: t.Any) -> t.Any:
-        try:
-            return macro(*args, **kwargs)
-        except MacroReturnVal as ret:
-            return ret.value
-
-    return wrapper
-
-
 class MacroExtractor(Parser):
     def extract(self, jinja: str, dialect: str = "") -> t.Dict[str, MacroInfo]:
         """Extract a dictionary of macro definitions from a jinja string.
 
         Args:
             jinja: The jinja string to extract from.
             dialect: The dialect of SQL.
@@ -168,20 +156,26 @@
 
     Args:
         packages: The mapping from package name to a collection of macro definitions.
         root_macros: The collection of top-level macro definitions.
         global_objs: The global objects.
         create_builtins_module: The name of a module which defines the `create_builtins` factory
             function that will be used to construct builtin variables and functions.
+        root_package_name: The name of the root package. If specified root macros will be available
+            as both `root_package_name.macro_name` and `macro_name`.
+        top_level_packages: The list of top-level packages. Macros in this packages will be available
+            as both `package_name.macro_name` and `macro_name`.
     """
 
     packages: t.Dict[str, t.Dict[str, MacroInfo]] = {}
     root_macros: t.Dict[str, MacroInfo] = {}
     global_objs: t.Dict[str, JinjaGlobalAttribute] = {}
     create_builtins_module: t.Optional[str] = None
+    root_package_name: t.Optional[str] = None
+    top_level_packages: t.List[str] = []
 
     _parser_cache: t.Dict[t.Tuple[t.Optional[str], str], Template] = {}
     __environment: t.Optional[Environment] = None
 
     @validator("global_objs", pre=True)
     def _validate_attribute_dict(cls, value: t.Any) -> t.Any:
         def _attribute_dict(val: t.Dict[str, t.Any]) -> AttributeDict:
@@ -213,54 +207,49 @@
         """Builds a Python callable for a macro with the given reference.
 
         Args:
             reference: The macro reference.
         Returns:
             The macro as a Python callable or None if not found.
         """
-        global_vars = self._create_builtin_globals(kwargs)
-        if reference.package is not None and reference.name not in self.packages.get(
-            reference.package, {}
-        ):
-            global_package = global_vars.get(reference.package, {})
-            return global_package.get(reference.name)
-        if reference.package is None and reference.name not in self.root_macros:
-            return global_vars.get(reference.name)
-
-        return self._make_callable(reference.name, reference.package, {}, global_vars)
+        env: Environment = self.build_environment(**kwargs)
+        if reference.package is not None:
+            package = env.globals.get(reference.package, {})
+            return package.get(reference.name)  # type: ignore
+        return env.globals.get(reference.name)  # type: ignore
 
     def build_environment(self, **kwargs: t.Any) -> Environment:
         """Builds a new Jinja environment based on this registry."""
 
-        global_vars = self._create_builtin_globals(kwargs)
-
-        callable_cache: t.Dict[t.Tuple[t.Optional[str], str], t.Callable] = {}
+        context: t.Dict[str, t.Any] = {}
 
         root_macros = {
-            name: self._make_callable(name, None, callable_cache, global_vars)
+            name: self._MacroWrapper(name, None, self, context)
             for name, macro in self.root_macros.items()
-            if not _is_private_macro(name)
         }
 
         package_macros: t.Dict[str, t.Any] = defaultdict(AttributeDict)
         for package_name, macros in self.packages.items():
-            for macro_name, macro in macros.items():
-                if not _is_private_macro(macro_name):
-                    package_macros[package_name][macro_name] = self._make_callable(
-                        macro_name, package_name, callable_cache, global_vars
-                    )
+            for macro_name in macros:
+                package_macros[package_name][macro_name] = self._MacroWrapper(
+                    macro_name, package_name, self, context
+                )
+
+        if self.root_package_name is not None:
+            package_macros[self.root_package_name].update(root_macros)
+
+        for top_level_package_name in self.top_level_packages:
+            root_macros.update(package_macros.get(top_level_package_name, {}))
+
+        context.update(root_macros)
+        context.update(package_macros)
+        context.update(self._create_builtin_globals(kwargs))
 
         env = environment()
-        env.globals.update(
-            {
-                **root_macros,
-                **package_macros,
-                **global_vars,
-            }
-        )
+        env.globals.update(context)
         env.filters.update(self._environment.filters)
         return env
 
     def trim(self, dependencies: t.Iterable[MacroReference]) -> JinjaMacroRegistry:
         """Trims the registry by keeping only macros with given references and their transitive dependencies.
 
         Args:
@@ -270,15 +259,18 @@
             A new trimmed registry.
         """
         dependencies_by_package: t.Dict[t.Optional[str], t.Set[str]] = defaultdict(set)
         for dep in dependencies:
             dependencies_by_package[dep.package].add(dep.name)
 
         result = JinjaMacroRegistry(
-            global_objs=self.global_objs.copy(), create_builtins_module=self.create_builtins_module
+            global_objs=self.global_objs.copy(),
+            create_builtins_module=self.create_builtins_module,
+            root_package_name=self.root_package_name,
+            top_level_packages=self.top_level_packages.copy(),
         )
         for package, names in dependencies_by_package.items():
             result = result.merge(self._trim_macros(names, package))
 
         return result
 
     def merge(self, other: JinjaMacroRegistry) -> JinjaMacroRegistry:
@@ -309,110 +301,83 @@
         }
 
         return JinjaMacroRegistry(
             packages=packages,
             root_macros=root_macros,
             global_objs=global_objs,
             create_builtins_module=self.create_builtins_module or other.create_builtins_module,
+            root_package_name=self.root_package_name or other.root_package_name,
+            top_level_packages=[*self.top_level_packages, *other.top_level_packages],
         )
 
-    def _make_callable(
-        self,
-        name: str,
-        package: t.Optional[str],
-        callable_cache: t.Dict[t.Tuple[t.Optional[str], str], t.Callable],
-        macro_vars: t.Dict[str, t.Any],
-    ) -> t.Callable:
-        cache_key = (package, name)
-        if cache_key in callable_cache:
-            return callable_cache[cache_key]
-
-        macro_vars = macro_vars.copy()
-        macro = self._get_macro(name, package)
-
-        package_macros: t.Dict[str, AttributeDict] = defaultdict(AttributeDict)
-        for dependency in macro.depends_on:
-            if (dependency.package is None and dependency.name == name) or not self._macro_exists(
-                dependency.name, dependency.package or package
-            ):
-                continue
-
-            upstream_callable = self._make_callable(
-                dependency.name, dependency.package or package, callable_cache, macro_vars
-            )
-            if dependency.package is None:
-                macro_vars[dependency.name] = upstream_callable
-            else:
-                package_macros[dependency.package][dependency.name] = upstream_callable
-
-        macro_vars.update(package_macros)
-
-        template = self._parse_macro(name, package)
-        macro_callable = macro_return(
-            getattr(template.make_module(vars=macro_vars), _non_private_name(name))
-        )
-        callable_cache[cache_key] = macro_callable
-        return macro_callable
-
     def _parse_macro(self, name: str, package: t.Optional[str]) -> Template:
         cache_key = (package, name)
         if cache_key not in self._parser_cache:
             macro = self._get_macro(name, package)
 
-            definition: t.Union[str, nodes.Template] = macro.definition
+            definition: nodes.Template = self._environment.parse(macro.definition)
             if _is_private_macro(name):
                 # A workaround to expose private jinja macros.
-                definition = self._to_non_private_macro_def(name, macro.definition)
+                definition = self._to_non_private_macro_def(name, definition)
 
             self._parser_cache[cache_key] = self._environment.from_string(definition)
         return self._parser_cache[cache_key]
 
     @property
     def _environment(self) -> Environment:
         if self.__environment is None:
             self.__environment = environment()
             self.__environment.filters.update(self._create_builtin_filters())
         return self.__environment
 
-    def _trim_macros(self, names: t.Set[str], package: t.Optional[str]) -> JinjaMacroRegistry:
+    def _trim_macros(
+        self,
+        names: t.Set[str],
+        package: t.Optional[str],
+        visited: t.Optional[t.Dict[t.Optional[str], t.Set[str]]] = None,
+    ) -> JinjaMacroRegistry:
+        if visited is None:
+            visited = defaultdict(set)
+
         macros = self.packages.get(package, {}) if package is not None else self.root_macros
         trimmed_macros = {}
 
         dependencies: t.Dict[t.Optional[str], t.Set[str]] = defaultdict(set)
 
         for name in names:
-            if name in macros:
+            if name in macros and name not in visited[package]:
                 macro = macros[name]
                 trimmed_macros[name] = macro
                 for dependency in macro.depends_on:
                     dependencies[dependency.package or package].add(dependency.name)
+                visited[package].add(name)
 
         if package is not None:
             result = JinjaMacroRegistry(packages={package: trimmed_macros})
         else:
             result = JinjaMacroRegistry(root_macros=trimmed_macros)
 
         for upstream_package, upstream_names in dependencies.items():
-            result = result.merge(self._trim_macros(upstream_names, upstream_package))
+            result = result.merge(
+                self._trim_macros(upstream_names, upstream_package, visited=visited)
+            )
 
         return result
 
     def _macro_exists(self, name: str, package: t.Optional[str]) -> bool:
         return (
             name in self.packages.get(package, {})
             if package is not None
             else name in self.root_macros
         )
 
     def _get_macro(self, name: str, package: t.Optional[str]) -> MacroInfo:
         return self.packages[package][name] if package is not None else self.root_macros[name]
 
-    def _to_non_private_macro_def(self, name: str, definition: str) -> nodes.Template:
-        template = self._environment.parse(definition)
-
+    def _to_non_private_macro_def(self, name: str, template: nodes.Template) -> nodes.Template:
         for node in template.find_all((nodes.Macro, nodes.Call)):
             if isinstance(node, nodes.Macro):
                 node.name = _non_private_name(name)
             elif isinstance(node, nodes.Call) and isinstance(node.node, nodes.Name):
                 node.node.name = _non_private_name(name)
 
         return template
@@ -431,14 +396,41 @@
         """Creates Jinja builtin filters using a factory function defined in the provided module."""
         if self.create_builtins_module is not None:
             module = importlib.import_module(self.create_builtins_module)
             if hasattr(module, "create_builtin_filters"):
                 return module.create_builtin_filters()
         return {}
 
+    class _MacroWrapper:
+        def __init__(
+            self,
+            name: str,
+            package: t.Optional[str],
+            registry: JinjaMacroRegistry,
+            context: t.Dict[str, t.Any],
+        ):
+            self.name = name
+            self.package = package
+            self.context = context
+            self.registry = registry
+
+        def __call__(self, *args: t.Any, **kwargs: t.Any) -> t.Any:
+            context = self.context.copy()
+            if self.package is not None and self.package in context:
+                context.update(context[self.package])
+
+            template = self.registry._parse_macro(self.name, self.package)
+            macro_callable = getattr(
+                template.make_module(vars=context), _non_private_name(self.name)
+            )
+            try:
+                return macro_callable(*args, **kwargs)
+            except MacroReturnVal as ret:
+                return ret.value
+
 
 def _is_private_macro(name: str) -> bool:
     return name.startswith("_")
 
 
 def _non_private_name(name: str) -> str:
     return name.lstrip("_")
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/utils/metaprogramming.py` & `sqlmesh-0.8.0/sqlmesh/utils/metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/utils/pandas.py` & `sqlmesh-0.8.0/sqlmesh/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/utils/pydantic.py` & `sqlmesh-0.8.0/sqlmesh/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/utils/rich.py` & `sqlmesh-0.8.0/sqlmesh/utils/rich.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/utils/transactional_file.py` & `sqlmesh-0.8.0/sqlmesh/utils/transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh/utils/yaml.py` & `sqlmesh-0.8.0/sqlmesh/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh.egg-info/PKG-INFO` & `sqlmesh-0.8.0/sqlmesh.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,14 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.7.1.dev33
-Summary: UNKNOWN
+Version: 0.8.0
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
-Description: ![SQLMesh logo](sqlmesh.svg)
-        
-        SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
-        
-        For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
-        
-        ## Geting Started
-        Install SQLMesh through [pypi](https://pypi.org/project/sqlmesh/) by running:
-        
-        ```pip install sqlmesh```
-        
-        Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
-        
-        ## Join our community
-        We'd love to join you on your data journey. Connect with us in the following ways:
-        
-        * Join the [Tobiko Slack community](https://tobikodata.com/slack) to ask questions, or just to say hi!
-        * File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
-        * Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
-        
-        ## Contribution
-        Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -43,7 +18,31 @@
 Provides-Extra: dbt
 Provides-Extra: github
 Provides-Extra: llm
 Provides-Extra: postgres
 Provides-Extra: redshift
 Provides-Extra: snowflake
 Provides-Extra: web
+License-File: LICENSE
+
+![SQLMesh logo](sqlmesh.svg)
+
+SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
+
+For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
+
+## Geting Started
+Install SQLMesh through [pypi](https://pypi.org/project/sqlmesh/) by running:
+
+```pip install sqlmesh```
+
+Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
+
+## Join our community
+We'd love to join you on your data journey. Connect with us in the following ways:
+
+* Join the [Tobiko Slack community](https://tobikodata.com/slack) to ask questions, or just to say hi!
+* File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
+* Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
+
+## Contribution
+Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh.egg-info/SOURCES.txt` & `sqlmesh-0.8.0/sqlmesh.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,19 @@
 docs/guides/scheduling/airflow_successful_setup.png
 docs/integrations/airflow.md
 docs/integrations/dbt.md
 docs/integrations/engines.md
 docs/integrations/github.md
 docs/integrations/overview.md
 docs/integrations/airflow/airflow_sqlmesh_state_connection.png
-docs/integrations/images/github_deployed_plans.png
-docs/integrations/images/github_env_summary.png
-docs/integrations/images/github_prod_plan_preview.png
-docs/integrations/images/github_reviewers.png
-docs/integrations/images/github_test_summary.png
+docs/integrations/github/github_deployed_plans.png
+docs/integrations/github/github_env_summary.png
+docs/integrations/github/github_prod_plan_preview.png
+docs/integrations/github/github_reviewers.png
+docs/integrations/github/github_test_summary.png
 docs/reference/cli.md
 docs/reference/configuration.md
 docs/reference/notebook.md
 docs/reference/overview.md
 docs/reference/python.md
 examples/__init__.py
 examples/airflow/Dockerfile.template
@@ -257,14 +257,15 @@
 sqlmesh/dbt/adapter.py
 sqlmesh/dbt/basemodel.py
 sqlmesh/dbt/builtin.py
 sqlmesh/dbt/column.py
 sqlmesh/dbt/common.py
 sqlmesh/dbt/context.py
 sqlmesh/dbt/loader.py
+sqlmesh/dbt/manifest.py
 sqlmesh/dbt/model.py
 sqlmesh/dbt/package.py
 sqlmesh/dbt/profile.py
 sqlmesh/dbt/project.py
 sqlmesh/dbt/seed.py
 sqlmesh/dbt/source.py
 sqlmesh/dbt/target.py
@@ -357,14 +358,15 @@
 tests/core/engine_adapter/test_postgres.py
 tests/core/engine_adapter/test_redshift.py
 tests/core/engine_adapter/test_spark.py
 tests/dbt/__init__.py
 tests/dbt/conftest.py
 tests/dbt/test_adapter.py
 tests/dbt/test_config.py
+tests/dbt/test_manifest.py
 tests/dbt/test_transformation.py
 tests/engines/__init__.py
 tests/engines/spark/__init__.py
 tests/engines/spark/conftest.py
 tests/engines/spark/test_db_api.py
 tests/fixtures/dbt/sushi_test/__init__.py
 tests/fixtures/dbt/sushi_test/config.py
@@ -437,14 +439,26 @@
 web/client/package-lock.json
 web/client/package.json
 web/client/playwright.config.ts
 web/client/postcss.config.js
 web/client/tailwind.config.js
 web/client/tsconfig.json
 web/client/vite.config.ts
+web/client/dist/index.html
+web/client/dist/assets/CircularStd-Black-52659624.otf
+web/client/dist/assets/CircularStd-Bold-0e6c076d.otf
+web/client/dist/assets/CircularStd-Medium-2f373e53.otf
+web/client/dist/assets/Plan-55e4c139.js
+web/client/dist/assets/Publico-Black-e6bd2ea2.otf
+web/client/dist/assets/Publico-Bold-c79acd56.otf
+web/client/dist/assets/Publico-Medium-01b4a891.otf
+web/client/dist/assets/index-5ace865e.css
+web/client/dist/assets/index-df610617.js
+web/client/dist/assets/worker-e891d118.js
+web/client/dist/favicons/favicon.ico
 web/client/public/favicons/favicon.ico
 web/client/src/index.css
 web/client/src/main.tsx
 web/client/src/routes.tsx
 web/client/src/api/channels.ts
 web/client/src/api/index.ts
 web/client/src/api/instance.ts
@@ -481,16 +495,18 @@
 web/client/src/context/plan.ts
 web/client/src/context/theme.tsx
 web/client/src/hooks/useActiveFocus.ts
 web/client/src/hooks/useLocalStorage.ts
 web/client/src/library/components/banner/Banner.tsx
 web/client/src/library/components/button/Button.tsx
 web/client/src/library/components/button/tests/Button.spec.tsx
+web/client/src/library/components/container/Container.tsx
 web/client/src/library/components/divider/Divider.tsx
 web/client/src/library/components/divider/tests/Divider.spec.tsx
+web/client/src/library/components/documentation/Documentation.tsx
 web/client/src/library/components/editor/Editor.css
 web/client/src/library/components/editor/Editor.tsx
 web/client/src/library/components/editor/EditorCode.tsx
 web/client/src/library/components/editor/EditorFooter.tsx
 web/client/src/library/components/editor/EditorIndicator.tsx
 web/client/src/library/components/editor/EditorInspector.tsx
 web/client/src/library/components/editor/EditorPreview.tsx
@@ -501,17 +517,14 @@
 web/client/src/library/components/fileTree/Directory.tsx
 web/client/src/library/components/fileTree/File.tsx
 web/client/src/library/components/fileTree/FileTree.tsx
 web/client/src/library/components/fileTree/help.ts
 web/client/src/library/components/graph/Graph.css
 web/client/src/library/components/graph/Graph.tsx
 web/client/src/library/components/graph/help.ts
-web/client/src/library/components/ide/ActivePlan.tsx
-web/client/src/library/components/ide/IDE.tsx
-web/client/src/library/components/ide/RunPlan.tsx
 web/client/src/library/components/input/Input.tsx
 web/client/src/library/components/input/InputToggle.tsx
 web/client/src/library/components/loading/Loading.tsx
 web/client/src/library/components/logo/Spinner.tsx
 web/client/src/library/components/logo/SqlMesh.tsx
 web/client/src/library/components/logo/Tobiko.tsx
 web/client/src/library/components/modal/Modal.tsx
@@ -526,22 +539,30 @@
 web/client/src/library/components/plan/PlanWizardStepOptions.tsx
 web/client/src/library/components/plan/context.tsx
 web/client/src/library/components/plan/help.spec.ts
 web/client/src/library/components/plan/help.ts
 web/client/src/library/components/plan/hooks.ts
 web/client/src/library/components/progress/Progress.tsx
 web/client/src/library/components/report/ReportTestsErrors.tsx
-web/client/src/library/components/root/Footer.tsx
-web/client/src/library/components/root/Header.tsx
-web/client/src/library/components/root/Main.tsx
-web/client/src/library/components/root/Root.tsx
 web/client/src/library/components/splitPane/SplitPane.css
 web/client/src/library/components/splitPane/SplitPane.tsx
 web/client/src/library/components/tasksOverview/TasksOverview.tsx
 web/client/src/library/components/toggle/Toggle.tsx
+web/client/src/library/pages/docs/Content.tsx
+web/client/src/library/pages/docs/Docs.tsx
+web/client/src/library/pages/docs/Search.tsx
+web/client/src/library/pages/docs/SourceList.tsx
+web/client/src/library/pages/editor/Editor.tsx
+web/client/src/library/pages/ide/ActivePlan.tsx
+web/client/src/library/pages/ide/IDE.tsx
+web/client/src/library/pages/ide/RunPlan.tsx
+web/client/src/library/pages/ide/context.tsx
+web/client/src/library/pages/root/Footer.tsx
+web/client/src/library/pages/root/Header.tsx
+web/client/src/library/pages/root/NotFound.tsx
 web/client/src/models/artifact.ts
 web/client/src/models/directory.ts
 web/client/src/models/environment.ts
 web/client/src/models/file.ts
 web/client/src/models/index.ts
 web/client/src/models/initial.ts
 web/client/src/tests/setup.ts
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh.egg-info/requires.txt` & `sqlmesh-0.8.0/sqlmesh.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 [dev]
 apache-airflow==2.3.3
 autoflake==1.7.7
 google-cloud-bigquery
 google-cloud-bigquery-storage
 black==22.6.0
 dbt-core
+dbt-duckdb
 Faker
 google-auth
 isort==5.10.1
 mkdocs-include-markdown-plugin==4.0.3
 mkdocs-material==9.0.5
 mypy~=1.0.0
 ipywidgets
```

### Comparing `sqlmesh-0.7.1.dev33/sqlmesh.svg` & `sqlmesh-0.8.0/sqlmesh.svg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/conftest.py` & `sqlmesh-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_base.py` & `sqlmesh-0.8.0/tests/core/engine_adapter/test_base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_base_postgres.py` & `sqlmesh-0.8.0/tests/core/engine_adapter/test_base_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_base_spark.py` & `sqlmesh-0.8.0/tests/core/engine_adapter/test_base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_bigquery.py` & `sqlmesh-0.8.0/tests/core/engine_adapter/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_databricks.py` & `sqlmesh-0.8.0/tests/core/engine_adapter/test_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_duckdb.py` & `sqlmesh-0.8.0/tests/core/engine_adapter/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_postgres.py` & `sqlmesh-0.8.0/tests/core/engine_adapter/test_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_redshift.py` & `sqlmesh-0.8.0/tests/core/engine_adapter/test_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/engine_adapter/test_spark.py` & `sqlmesh-0.8.0/tests/core/engine_adapter/test_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/test_audit.py` & `sqlmesh-0.8.0/tests/core/test_audit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/test_config.py` & `sqlmesh-0.8.0/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/test_connection_config.py` & `sqlmesh-0.8.0/tests/core/test_connection_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/test_context.py` & `sqlmesh-0.8.0/tests/core/test_context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/test_dialect.py` & `sqlmesh-0.8.0/tests/core/test_dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/test_integration.py` & `sqlmesh-0.8.0/tests/core/test_integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/test_macros.py` & `sqlmesh-0.8.0/tests/core/test_macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/test_model.py` & `sqlmesh-0.8.0/tests/core/test_model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/test_plan.py` & `sqlmesh-0.8.0/tests/core/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/test_plan_evaluator.py` & `sqlmesh-0.8.0/tests/core/test_plan_evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/test_scheduler.py` & `sqlmesh-0.8.0/tests/core/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/test_schema_diff.py` & `sqlmesh-0.8.0/tests/core/test_schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/test_seed.py` & `sqlmesh-0.8.0/tests/core/test_seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/test_snapshot.py` & `sqlmesh-0.8.0/tests/core/test_snapshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,15 @@
             "pre": [],
             "owner": "owner",
             "query": "SELECT @EACH(ARRAY(1, 2), x -> x), ds FROM parent.tbl",
             "jinja_macros": {
                 "global_objs": {},
                 "packages": {},
                 "root_macros": {},
+                "top_level_packages": [],
             },
             "source_type": "sql",
             "tags": [],
         },
         "audits": [],
         "name": "name",
         "parents": [{"name": "parent.tbl", "identifier": snapshot.parents[0].identifier}],
```

### Comparing `sqlmesh-0.7.1.dev33/tests/core/test_snapshot_evaluator.py` & `sqlmesh-0.8.0/tests/core/test_snapshot_evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/core/test_state_sync.py` & `sqlmesh-0.8.0/tests/core/test_state_sync.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/dbt/conftest.py` & `sqlmesh-0.8.0/tests/dbt/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/dbt/test_adapter.py` & `sqlmesh-0.8.0/tests/dbt/test_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,9 @@
     )
 
 
 def test_adapter_dispatch(sushi_test_project: Project):
     context = sushi_test_project.context
     assert context.render("{{ adapter.dispatch('current_engine', 'customers')() }}") == "duckdb"
 
-    assert context.engine_adapter
-    context.engine_adapter.dialect = "unknown"
-    context._jinja_environment = None
-    assert context.render("{{ adapter.dispatch('current_engine', 'customers')() }}") == "default"
-
     with pytest.raises(ConfigError, match=r"Macro 'current_engine'.*was not found."):
         context.render("{{ adapter.dispatch('current_engine')() }}")
```

### Comparing `sqlmesh-0.7.1.dev33/tests/dbt/test_config.py` & `sqlmesh-0.8.0/tests/dbt/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,129 +56,83 @@
     ],
 )
 def test_update(current: t.Dict[str, t.Any], new: t.Dict[str, t.Any], expected: t.Dict[str, t.Any]):
     config = ModelConfig(**current).update_with(new)
     assert {k: v for k, v in config.dict().items() if k in expected} == expected
 
 
-def test_model_config(sushi_test_project: Project):
-    assert set(sushi_test_project.packages["sushi"].models) == {
-        "waiters",
-        "top_waiters",
-        "waiter_revenue_by_day",
-        "waiter_as_customer_by_day",
-    }
-
-    assert set(sushi_test_project.packages["customers"].models) == {
-        "customers",
-        "customer_revenue_by_day",
-    }
-
-    customer_revenue_by_day_config = sushi_test_project.packages["customers"].models[
-        "customer_revenue_by_day"
-    ]
-
-    context = sushi_test_project.context
-    context.sources = {
-        "raw.order_items": SourceConfig(target_schema="raw", name="order_items"),
-        "raw.items": SourceConfig(target_schema="raw", name="items"),
-        "raw.orders": SourceConfig(target_schema="raw", name="orders"),
-    }
-    context.variables = {}
-    rendered = customer_revenue_by_day_config.render_config(context)
-
-    expected_config = {
-        "materialized": Materialization.INCREMENTAL,
-        "incremental_strategy": "delete+insert",
-        "cluster_by": ["ds"],
-        "target_schema": "sushi",
-    }
-    actual_config = {k: getattr(rendered, k) for k, v in expected_config.items()}
-    assert actual_config == expected_config
-
-    assert rendered.model_name == "sushi.customer_revenue_by_day"
-
-
 def test_to_sqlmesh_fields(sushi_test_project: Project):
     model_config = ModelConfig(
         alias="model",
-        target_schema="schema",
-        schema_="custom",
+        schema="custom",
         database="database",
         materialized=Materialization.INCREMENTAL,
         description="test model",
         sql="SELECT 1 AS a FROM foo",
         start="Jan 1 2023",
         partitioned_by=["a"],
         cron="@hourly",
         batch_size=5,
         lookback=3,
         unique_key=["a"],
         meta={"stamp": "bar", "dialect": "duckdb"},
         owner="Sally",
     )
-    context = DbtContext(project_name="Foo")
+    context = DbtContext()
+    context.project_name = "Foo"
     context.target = DuckDbConfig(name="target", schema="foo")
     model = model_config.to_sqlmesh(context)
 
     assert isinstance(model, SqlModel)
-    assert model.name == "database.schema_custom.model"
+    assert model.name == "database.custom.model"
     assert model.description == "test model"
     assert model.query.sql() == "SELECT 1 AS a FROM foo"
     assert model.start == "Jan 1 2023"
     assert model.partitioned_by == ["a"]
     assert model.cron == "@hourly"
     assert model.stamp == "bar"
     assert model.dialect == "duckdb"
     assert model.owner == "Sally"
     kind = t.cast(IncrementalByUniqueKeyKind, model.kind)
     assert kind.batch_size == 5
     assert kind.lookback == 3
 
 
 def test_model_config_sql_no_config():
-    context = DbtContext()
     assert (
         ModelConfig(
             sql="""{{
   config(
     materialized='table',
     incremental_strategy='delete+"insert'
   )
 }}
 query"""
-        )
-        .render_config(context)
-        .sql_no_config.strip()
+        ).sql_no_config.strip()
         == "query"
     )
 
-    context.variables = {"new": "old"}
     assert (
         ModelConfig(
             sql="""{{
   config(
     materialized='table',
     incremental_strategy='delete+insert',
     post_hook=" '{{ var('new') }}' "
   )
 }}
 query"""
-        )
-        .render_config(context)
-        .sql_no_config.strip()
+        ).sql_no_config.strip()
         == "query"
     )
 
     assert (
         ModelConfig(
             sql="""before {{config(materialized='table', post_hook=" {{ var('new') }} ")}} after"""
-        )
-        .render_config(context)
-        .sql_no_config.strip()
+        ).sql_no_config.strip()
         == "before  after"
     )
 
 
 def test_variables(assert_exp_eq, sushi_test_project):
     # Case 1: using an undefined variable without a default value
     defined_variables = {}
@@ -186,36 +140,30 @@
     context = sushi_test_project.context
     context.variables = defined_variables
 
     model_config = ModelConfig(alias="test", sql="SELECT {{ var('foo') }}")
 
     kwargs = {"context": context}
 
-    with pytest.raises(ConfigError, match=r".*Variable 'foo' was not found.*"):
-        rendered = model_config.render_config(context)
-        model_config.to_sqlmesh(**kwargs)
-
     # Case 2: using a defined variable without a default value
     defined_variables["foo"] = 6
     context.variables = defined_variables
-    rendered = model_config.render_config(context)
-    assert_exp_eq(rendered.to_sqlmesh(**kwargs).render_query(), 'SELECT 6 AS "6"')
+    assert_exp_eq(model_config.to_sqlmesh(**kwargs).render_query(), 'SELECT 6 AS "6"')
 
     # Case 3: using a defined variable with a default value
     model_config.sql = "SELECT {{ var('foo', 5) }}"
+    model_config._sql_no_config = None
 
-    rendered = model_config.render_config(context)
-    assert_exp_eq(rendered.to_sqlmesh(**kwargs).render_query(), 'SELECT 6 AS "6"')
+    assert_exp_eq(model_config.to_sqlmesh(**kwargs).render_query(), 'SELECT 6 AS "6"')
 
     # Case 4: using an undefined variable with a default value
     del defined_variables["foo"]
     context.variables = defined_variables
 
-    rendered = model_config.render_config(context)
-    assert_exp_eq(rendered.to_sqlmesh(**kwargs).render_query(), 'SELECT 5 AS "5"')
+    assert_exp_eq(model_config.to_sqlmesh(**kwargs).render_query(), 'SELECT 5 AS "5"')
 
     # Finally, check that variable scoping & overwriting (some_var) works as expected
     expected_sushi_variables = {
         "top_waiters:limit": 10,
         "top_waiters:revenue": "revenue",
         "customers:boo": ["a", "b"],
     }
@@ -253,15 +201,15 @@
 def test_seed_config(sushi_test_project: Project):
     seed_configs = sushi_test_project.packages["sushi"].seeds
     assert set(seed_configs) == {"waiter_names"}
     raw_items_seed = seed_configs["waiter_names"]
 
     expected_config = {
         "path": Path(sushi_test_project.context.project_root, "seeds/waiter_names.csv"),
-        "target_schema": "sushi",
+        "schema_": "sushi",
     }
     actual_config = {k: getattr(raw_items_seed, k) for k, v in expected_config.items()}
     assert actual_config == expected_config
 
     assert raw_items_seed.model_name == "sushi.waiter_names"
```

### Comparing `sqlmesh-0.7.1.dev33/tests/dbt/test_transformation.py` & `sqlmesh-0.8.0/tests/dbt/test_transformation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,37 @@
 from pathlib import Path
 
 import agate
 import pytest
 from dbt.exceptions import CompilationError
 from sqlglot import exp, parse_one
 
-from sqlmesh.core.config.connection import DuckDBConnectionConfig
 from sqlmesh.core.context import Context, ExecutionContext
 from sqlmesh.core.model import (
     IncrementalByTimeRangeKind,
     IncrementalByUniqueKeyKind,
     ModelKind,
     ModelKindName,
 )
-from sqlmesh.dbt.builtin import create_builtin_globals
 from sqlmesh.dbt.column import (
     ColumnConfig,
     column_descriptions_to_sqlmesh,
     column_types_to_sqlmesh,
 )
 from sqlmesh.dbt.context import DbtContext
 from sqlmesh.dbt.model import Materialization, ModelConfig
 from sqlmesh.dbt.project import Project
 from sqlmesh.dbt.seed import SeedConfig
-from sqlmesh.dbt.source import SourceConfig
 from sqlmesh.dbt.target import DuckDbConfig
 from sqlmesh.utils.errors import ConfigError, MacroEvalError
 
 
 def test_model_name():
-    assert ModelConfig(target_schema="foo", path="models/bar.sql").model_name == "foo.bar"
-    assert (
-        ModelConfig(target_schema="foo", path="models/bar.sql", alias="baz").model_name == "foo.baz"
-    )
-    assert (
-        ModelConfig(target_schema="foo", path="models/bar.sql", schema_="baz").model_name
-        == "foo_baz.bar"
-    )
+    assert ModelConfig(schema="foo", path="models/bar.sql").model_name == "foo.bar"
+    assert ModelConfig(schema="foo", path="models/bar.sql", alias="baz").model_name == "foo.baz"
 
 
 def test_model_kind():
     target = DuckDbConfig(name="target", schema="foo")
 
     assert ModelConfig(materialized=Materialization.TABLE).model_kind(target) == ModelKind(
         name=ModelKindName.FULL
@@ -134,15 +125,16 @@
         "address": "Business address",
         "zipcode": "Business zipcode",
     }
 
     assert column_types_to_sqlmesh(model.columns) == expected_column_types
     assert column_descriptions_to_sqlmesh(model.columns) == expected_column_descriptions
 
-    context = DbtContext(project_name="Foo")
+    context = DbtContext()
+    context.project_name = "Foo"
     context.target = DuckDbConfig(name="target", schema="foo")
     sqlmesh_model = model.to_sqlmesh(context)
     assert sqlmesh_model.columns_to_types == expected_column_types
     assert sqlmesh_model.column_descriptions == expected_column_descriptions
 
 
 def test_seed_columns():
@@ -170,83 +162,14 @@
 
     context = DbtContext()
     sqlmesh_seed = seed.to_sqlmesh(context)
     assert sqlmesh_seed.columns_to_types == expected_column_types
     assert sqlmesh_seed.column_descriptions == expected_column_descriptions
 
 
-def test_config_containing_jinja():
-    model = ModelConfig(
-        **{
-            "pre-hook": "GRANT INSERT ON {{ source('package', 'table') }} TO admin",
-            "post-hook": "GRANT DELETE ON {{ source('package', 'table') }} TO admin",
-        },
-        target_schema="{{ var('schema') }}",
-        table_name="bar",
-        sql="SELECT * FROM {{ source('package', 'table') }}",
-        columns={
-            "address": ColumnConfig(
-                name="address", data_type="text", description="Business address"
-            ),
-            "zipcode": ColumnConfig(
-                name="zipcode",
-                data_type="varchar({{ var('size') }})",
-                description="Business zipcode",
-            ),
-        },
-    )
-
-    context = DbtContext(project_name="Foo")
-    context.target = DuckDbConfig(name="target", schema="foo")
-    context.variables = {"schema": "foo", "size": "5"}
-    model.dependencies.sources = set(["package.table"])
-    context.sources = {"package.table": SourceConfig(schema_="raw", name="baz")}
-
-    rendered = model.render_config(context)
-    assert rendered.pre_hook == model.pre_hook
-    assert rendered.sql == model.sql
-    assert rendered.target_schema != model.target_schema
-    assert rendered.target_schema == "foo"
-    assert rendered.columns["zipcode"] != model.columns["zipcode"]
-    assert rendered.columns["zipcode"].data_type == "varchar(5)"
-
-    sqlmesh_model = rendered.to_sqlmesh(context)
-    assert str(sqlmesh_model.query) == model.sql
-    assert str(sqlmesh_model.render_query()) == 'SELECT * FROM "raw"."baz" AS baz'
-    assert sqlmesh_model.columns_to_types == column_types_to_sqlmesh(rendered.columns)
-
-
-def test_config_containing_missing_dependency():
-    context = DbtContext(project_name="project")
-    context.target = DuckDbConfig(name="target", schema="foo")
-    model = ModelConfig(sql="{{ config(pre_hook=\"{{ print(ref('bar')) }}\") }} SELECT 1 FROM a")
-    with pytest.raises(ConfigError, match="'bar' was not found"):
-        model.render_config(context).to_sqlmesh(context)
-
-    model = ModelConfig(sql='{{ config(pre_hook="{{ get_table_name() }}") }} SELECT 1 FROM a')
-    with pytest.raises(ConfigError, match="get_table_name"):
-        model.render_config(context).to_sqlmesh(context)
-
-    model = ModelConfig(sql="{{ config(alias='{{ get_table_name() }}') }} SELECT 1 FROM a")
-    rendered = model.render_config(context)
-    assert rendered.alias == "{{ get_table_name() }}"
-    assert "get_table_name" not in [macro.name for macro in rendered.dependencies.macros]
-    rendered.to_sqlmesh(context)
-
-
-def test_config_containing_method():
-    context = DbtContext()
-    context.jinja_macros.global_objs.update({"get_table_name": lambda: "foo"})
-    model = ModelConfig(sql="{{ config(alias=get_table_name()) }} SELECT 1 FROM a")
-
-    rendered = model.render_config(context)
-    assert rendered.alias == "foo"
-    assert "get_table_name" not in [macro.name for macro in rendered.dependencies.macros]
-
-
 @pytest.mark.parametrize("model", ["sushi.waiters", "sushi.waiter_names"])
 def test_hooks(capsys, sushi_test_dbt_context: Context, model: str):
     waiters = sushi_test_dbt_context.models[model]
     execution_context = ExecutionContext(sushi_test_dbt_context.engine_adapter, {}, False)
     capsys.readouterr()
 
     waiters.run_pre_hooks(execution_context)
@@ -267,29 +190,19 @@
 
 def test_project_name_jinja(sushi_test_project: Project):
     context = sushi_test_project.context
     assert context.render("{{ project_name }}") == "sushi"
 
 
 def test_schema_jinja(sushi_test_project: Project):
-    model_config = ModelConfig(target_schema="sushi", sql="SELECT 1 AS one FROM {{ schema }}")
+    model_config = ModelConfig(schema="sushi", sql="SELECT 1 AS one FROM {{ schema }}")
     context = sushi_test_project.context
     model_config.to_sqlmesh(context).render_query().sql() == "SELECT 1 AS one FROM sushi AS sushi"
 
 
-def test_materialized_jinja(sushi_test_project: Project):
-    model_config = ModelConfig(
-        materialized="{{ 'table' if target.type in ['duckdb'] else 'view' }}",
-        sql="SELECT 1 AS one FROM {{ schema }}",
-    )
-    context = sushi_test_project.context
-    rendered = model_config.render_config(context)
-    assert rendered.materialized == "table"
-
-
 def test_this(assert_exp_eq, sushi_test_project: Project):
     model_config = ModelConfig(alias="test", sql="SELECT 1 AS one FROM {{ this.identifier }}")
     context = sushi_test_project.context
     assert_exp_eq(
         model_config.to_sqlmesh(context).render_query().sql(), "SELECT 1 AS one FROM test AS test"
     )
 
@@ -439,28 +352,11 @@
     assert context.render("{{ zip(12, ['a', 'b']) }}") == "None"
 
     assert context.render("{{ zip_strict([1, 2], ['a', 'b']) }}") == "[(1, 'a'), (2, 'b')]"
     with pytest.raises(TypeError):
         context.render("{{ zip_strict(12, ['a', 'b']) }}")
 
 
-def test_dbt_namespace():
-    context = DbtContext()
-    jinja_globals = create_builtin_globals(
-        jinja_macros=context.jinja_macros,
-        jinja_globals={},
-        engine_adapter=DuckDBConnectionConfig().create_engine_adapter(),
-    )
-    jinja_env = context.jinja_macros.build_environment(**jinja_globals)
-
-    assert (
-        jinja_env.from_string("{{ dbt.replace('original sentence', 'original', 'updated') }}")
-        .render()
-        .strip()
-        == """replace(
-        original sentence,
-        original,
-        updated
-    )"""
-    )
+def test_dbt_version(sushi_test_project: Project):
+    context = sushi_test_project.context
 
-    assert jinja_env.from_string("{{ dbt.hash('col')}}").render() == "md5(cast(col as TEXT))"
+    assert context.render("{{ dbt_version }}").startswith("1.")
```

### Comparing `sqlmesh-0.7.1.dev33/tests/engines/spark/test_db_api.py` & `sqlmesh-0.8.0/tests/engines/spark/test_db_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/dbt_project.yml` & `sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/dbt_project.yml`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,14 @@
   +start: Jan 1 2022
   sushi:
     +materialized: table
     +pre-hook:
       - '{{ log("pre-hook") }}'
     +post-hook: 
       - '{{ log("post-hook") }}'
-  customers:
-    +materialized: table
 
 seeds:
   sushi:
     +pre-hook:
       - '{{ log("pre-hook") }}'
     +post-hook: 
       - '{{ log("post-hook") }}'
```

### Comparing `sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy` & `sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/macros/incremental.sql` & `sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql` & `sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml` & `sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql` & `sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/profiles.yml` & `sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/seed_sources.py` & `sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/seed_sources.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/source_data/items.csv` & `sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/source_data/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/source_data/order_items.csv` & `sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/source_data/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/fixtures/dbt/sushi_test/source_data/orders.csv` & `sqlmesh-0.8.0/tests/fixtures/dbt/sushi_test/source_data/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/fixtures/migrations/environments.json` & `sqlmesh-0.8.0/tests/fixtures/migrations/environments.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/fixtures/migrations/snapshots.json` & `sqlmesh-0.8.0/tests/fixtures/migrations/snapshots.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/schedulers/airflow/conftest.py` & `sqlmesh-0.8.0/tests/schedulers/airflow/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/schedulers/airflow/operators/test_hwm_sensor.py` & `sqlmesh-0.8.0/tests/schedulers/airflow/operators/test_hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/schedulers/airflow/operators/test_targets.py` & `sqlmesh-0.8.0/tests/schedulers/airflow/operators/test_targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/schedulers/airflow/test_client.py` & `sqlmesh-0.8.0/tests/schedulers/airflow/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
                     "partitioned_by": ["a"],
                     "query": "SELECT a, ds FROM tbl",
                     "storage_format": "parquet",
                     "jinja_macros": {
                         "global_objs": {},
                         "packages": {},
                         "root_macros": {},
+                        "top_level_packages": [],
                     },
                     "source_type": "sql",
                     "tags": [],
                 },
                 "audits": [],
                 "name": "test_model",
                 "parents": [],
```

### Comparing `sqlmesh-0.7.1.dev33/tests/schedulers/airflow/test_end_to_end.py` & `sqlmesh-0.8.0/tests/schedulers/airflow/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/schedulers/airflow/test_integration.py` & `sqlmesh-0.8.0/tests/schedulers/airflow/test_integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/schedulers/airflow/test_plan.py` & `sqlmesh-0.8.0/tests/schedulers/airflow/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/utils/test_cache.py` & `sqlmesh-0.8.0/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/utils/test_concurrency.py` & `sqlmesh-0.8.0/tests/utils/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/utils/test_connection_pool.py` & `sqlmesh-0.8.0/tests/utils/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/utils/test_dag.py` & `sqlmesh-0.8.0/tests/utils/test_dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/utils/test_date.py` & `sqlmesh-0.8.0/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/utils/test_filesystem.py` & `sqlmesh-0.8.0/tests/utils/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/utils/test_jinja.py` & `sqlmesh-0.8.0/tests/utils/test_jinja.py`

 * *Files 15% similar despite different names*

```diff
@@ -180,7 +180,83 @@
 
 
 def test_global_objs():
     original_registry = JinjaMacroRegistry(global_objs={"target": AttributeDict({"test": "value"})})
 
     deserialized_registry = JinjaMacroRegistry.parse_raw(original_registry.json())
     assert deserialized_registry.global_objs["target"].test == "value"
+
+
+def test_macro_registry_recursion():
+    macros = """
+{% macro macro_a(n) %} {{ macro_b(n) }} {% endmacro %}
+
+{% macro macro_b(n) %}
+{% if n <= 0 %}
+  end
+{% else %}
+  {{ macro_a(n - 1) }}
+{% endif %}
+{% endmacro %}
+"""
+
+    extractor = MacroExtractor()
+    registry = JinjaMacroRegistry()
+
+    registry.add_macros(extractor.extract(macros))
+
+    rendered = registry.build_environment().from_string("{{ macro_a(4) }}").render()
+    assert rendered.strip() == "end"
+
+    assert registry.trim([MacroReference(name="macro_a")]).root_macros.keys() == {
+        "macro_a",
+        "macro_b",
+    }
+
+
+def test_macro_registry_recursion_with_package():
+    macros = """
+{% macro macro_a(n) %}{{ sushi.macro_b(n) }}{% endmacro %}
+j
+{% macro macro_b(n) %}
+{% if n <= 0 %}
+end
+{% else %}
+{{ sushi.macro_a(n - 1) }}
+{% endif %}
+{% endmacro %}
+"""
+
+    extractor = MacroExtractor()
+    registry = JinjaMacroRegistry(root_package_name="sushi")
+
+    registry.add_macros(extractor.extract(macros))
+
+    rendered = registry.build_environment().from_string("{{ macro_a(4) }}").render()
+    assert rendered.strip() == "end"
+
+
+def test_macro_registry_top_level_packages():
+    package_a = """
+{% macro macro_a_a() %}
+macro_a_a
+{% endmacro %}"""
+
+    local_macros = "{% macro local_macro() %}{{ macro_a_a() }}{% endmacro %}"
+
+    extractor = MacroExtractor()
+    registry = JinjaMacroRegistry(top_level_packages=["package_a"])
+
+    registry.add_macros(extractor.extract(local_macros))
+    registry.add_macros(extractor.extract(package_a), package="package_a")
+
+    rendered = (
+        registry.build_environment()
+        .from_string("{{ local_macro() }}{{ package_a.macro_a_a() }}")
+        .render()
+    )
+    rendered = [r for r in rendered.split("\n") if r]
+
+    assert rendered == [
+        "macro_a_a",
+        "macro_a_a",
+    ]
```

### Comparing `sqlmesh-0.7.1.dev33/tests/utils/test_metaprogramming.py` & `sqlmesh-0.8.0/tests/utils/test_metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/utils/test_pandas.py` & `sqlmesh-0.8.0/tests/utils/test_pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/utils/test_pydantic.py` & `sqlmesh-0.8.0/tests/utils/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/utils/test_transactional_file.py` & `sqlmesh-0.8.0/tests/utils/test_transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/utils/test_yaml.py` & `sqlmesh-0.8.0/tests/utils/test_yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/tests/web/test_main.py` & `sqlmesh-0.8.0/tests/web/test_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import pyarrow as pa  # type: ignore
 import pytest
 from fastapi.testclient import TestClient
 from pytest_mock.plugin import MockerFixture
 
 from sqlmesh.core.context import Context
 from sqlmesh.utils.errors import PlanError
-from web.server import models
 from web.server.main import api_console, app
 from web.server.settings import Settings, get_loaded_context, get_settings
 
 client = TestClient(app)
 
 
 @pytest.fixture
@@ -434,38 +433,26 @@
     response = client.post("/api/commands/fetchdf", json={"sql": "SELECT * from sushi.top_waiters"})
     assert response.status_code == 200
     with pa.ipc.open_stream(response.content) as reader:
         df = reader.read_pandas()
     assert not df.empty
 
 
+# TODO: add better tests for this endpoint
 def test_get_models(web_sushi_context: Context) -> None:
-    # TODO: add better tests for this endpoint
     response = client.get("/api/models")
-    json_models = [
-        models.Model(
-            name=model.name,
-            path=str(model._path.relative_to(web_sushi_context.path)),
-            description=model.description,
-            owner=model.owner,
-            dialect=model.dialect,
-            columns=[
-                models.Column(
-                    name=name,
-                    type=str(data_type),
-                    description=model.column_descriptions.get(name),
-                )
-                for name, data_type in model.columns_to_types.items()
-            ],
-        ).dict()
-        for model in web_sushi_context.models.values()
-    ]
 
     assert response.status_code == 200
-    assert json_models == response.json()
+
+    test_model = response.json()[0]
+
+    assert test_model.get("name")
+    assert test_model.get("path")
+    assert test_model.get("dialect")
+    assert test_model.get("columns")
 
 
 def test_render(web_sushi_context: Context) -> None:
     response = client.post("/api/commands/render", json={"model": "sushi.items"})
     assert response.status_code == 200
     assert response.json()["sql"]
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/.eslintrc.js` & `sqlmesh-0.8.0/web/client/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/index.html` & `sqlmesh-0.8.0/web/client/index.html`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/openapi.json` & `sqlmesh-0.8.0/web/client/openapi.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9961899181547619%*

 * *Differences: {"'components'": "{'schemas': {'Environment': {'properties': {'finalized_ts': "*

 * *                 "OrderedDict([('title', 'Finalized Ts'), ('type', 'integer')])}}, 'Model': "*

 * *                 "{'properties': {'details': OrderedDict([('$ref', "*

 * *                 "'#/components/schemas/ModelDetails')]), 'sql': OrderedDict([('title', 'Sql'), "*

 * *                 "('type', 'string')]), delete: ['owner']}}, 'SnapshotChangeCategory': {'enum': "*

 * *                 "{insert: [(3, 4), (4, 5)]}, 'description': 'Values are  […]*

```diff
@@ -439,14 +439,18 @@
                         ],
                         "title": "End At"
                     },
                     "expiration_ts": {
                         "title": "Expiration Ts",
                         "type": "integer"
                     },
+                    "finalized_ts": {
+                        "title": "Finalized Ts",
+                        "type": "integer"
+                    },
                     "name": {
                         "title": "Name",
                         "type": "string"
                     },
                     "plan_id": {
                         "title": "Plan Id",
                         "type": "string"
@@ -637,14 +641,24 @@
                         "title": "Detail",
                         "type": "array"
                     }
                 },
                 "title": "HTTPValidationError",
                 "type": "object"
             },
+            "IntervalUnit": {
+                "description": "IntervalUnit is the inferred granularity of an incremental model.\n\nIntervalUnit can be one of 4 types, DAY, HOUR, MINUTE. The unit is inferred\nbased on the cron schedule of a model. The minimum time delta between a sample set of dates\nis used to determine which unit a model's schedule is.",
+                "enum": [
+                    "day",
+                    "hour",
+                    "minute"
+                ],
+                "title": "IntervalUnit",
+                "type": "string"
+            },
             "LineageColumn": {
                 "properties": {
                     "models": {
                         "additionalProperties": {
                             "items": {
                                 "type": "string"
                             },
@@ -670,40 +684,156 @@
                         "title": "Columns",
                         "type": "array"
                     },
                     "description": {
                         "title": "Description",
                         "type": "string"
                     },
+                    "details": {
+                        "$ref": "#/components/schemas/ModelDetails"
+                    },
                     "dialect": {
                         "title": "Dialect",
                         "type": "string"
                     },
                     "name": {
                         "title": "Name",
                         "type": "string"
                     },
-                    "owner": {
-                        "title": "Owner",
-                        "type": "string"
-                    },
                     "path": {
                         "title": "Path",
                         "type": "string"
+                    },
+                    "sql": {
+                        "title": "Sql",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "name",
                     "path",
                     "dialect",
                     "columns"
                 ],
                 "title": "Model",
                 "type": "object"
             },
+            "ModelDetails": {
+                "properties": {
+                    "annotated": {
+                        "title": "Annotated",
+                        "type": "boolean"
+                    },
+                    "batch_size": {
+                        "title": "Batch Size",
+                        "type": "integer"
+                    },
+                    "contains_star_query": {
+                        "title": "Contains Star Query",
+                        "type": "boolean"
+                    },
+                    "cron": {
+                        "title": "Cron",
+                        "type": "string"
+                    },
+                    "cron_next": {
+                        "anyOf": [
+                            {
+                                "format": "date",
+                                "type": "string"
+                            },
+                            {
+                                "format": "date-time",
+                                "type": "string"
+                            },
+                            {
+                                "type": "string"
+                            },
+                            {
+                                "type": "integer"
+                            },
+                            {
+                                "type": "number"
+                            }
+                        ],
+                        "title": "Cron Next"
+                    },
+                    "cron_prev": {
+                        "anyOf": [
+                            {
+                                "format": "date",
+                                "type": "string"
+                            },
+                            {
+                                "format": "date-time",
+                                "type": "string"
+                            },
+                            {
+                                "type": "string"
+                            },
+                            {
+                                "type": "integer"
+                            },
+                            {
+                                "type": "number"
+                            }
+                        ],
+                        "title": "Cron Prev"
+                    },
+                    "interval_unit": {
+                        "$ref": "#/components/schemas/IntervalUnit"
+                    },
+                    "kind": {
+                        "title": "Kind",
+                        "type": "string"
+                    },
+                    "lookback": {
+                        "title": "Lookback",
+                        "type": "integer"
+                    },
+                    "owner": {
+                        "title": "Owner",
+                        "type": "string"
+                    },
+                    "partitioned_by": {
+                        "title": "Partitioned By",
+                        "type": "string"
+                    },
+                    "retention": {
+                        "title": "Retention",
+                        "type": "string"
+                    },
+                    "stamp": {
+                        "title": "Stamp",
+                        "type": "string"
+                    },
+                    "start": {
+                        "title": "Start",
+                        "type": "string"
+                    },
+                    "storage_format": {
+                        "title": "Storage Format",
+                        "type": "string"
+                    },
+                    "tags": {
+                        "title": "Tags",
+                        "type": "string"
+                    },
+                    "time_column": {
+                        "title": "Time Column",
+                        "type": "string"
+                    },
+                    "type": {
+                        "title": "Type",
+                        "type": "string"
+                    }
+                },
+                "title": "ModelDetails",
+                "type": "object"
+            },
             "ModelsDiff": {
                 "properties": {
                     "direct": {
                         "default": [],
                         "items": {
                             "$ref": "#/components/schemas/ChangeDirect"
                         },
@@ -933,32 +1063,38 @@
                 "required": [
                     "model"
                 ],
                 "title": "RenderInput",
                 "type": "object"
             },
             "SnapshotChangeCategory": {
-                "description": "Values are ordered by decreasing severity and that ordering is required.\n\nBREAKING: The change requires that snapshot modified and downstream dependencies be rebuilt\nNON_BREAKING: The change requires that only the snapshot modified be rebuilt\nNO_CHANGE: The change requires no rebuilding",
+                "description": "Values are ordered by decreasing severity and that ordering is required.\n\nBREAKING: The change requires that snapshot modified and downstream dependencies be rebuilt\nNON_BREAKING: The change requires that only the snapshot modified be rebuilt\nFORWARD_ONLY: The change requires no rebuilding\nINDIRECT_BREAKING: The change was caused indirectly and is breaking.\nINDIRECT_FORWARD_ONLY: The change was caused indirectly and is forward-only.",
                 "enum": [
                     1,
                     2,
-                    3
+                    3,
+                    4,
+                    5
                 ],
                 "title": "SnapshotChangeCategory",
                 "type": "integer"
             },
             "SnapshotDataVersion": {
                 "additionalProperties": false,
                 "properties": {
                     "change_category": {
                         "$ref": "#/components/schemas/SnapshotChangeCategory"
                     },
                     "fingerprint": {
                         "$ref": "#/components/schemas/SnapshotFingerprint"
                     },
+                    "temp_version": {
+                        "title": "Temp Version",
+                        "type": "string"
+                    },
                     "version": {
                         "title": "Version",
                         "type": "string"
                     }
                 },
                 "required": [
                     "fingerprint",
@@ -1051,14 +1187,18 @@
                         "default": [],
                         "items": {
                             "$ref": "#/components/schemas/SnapshotDataVersion"
                         },
                         "title": "Previous Versions",
                         "type": "array"
                     },
+                    "temp_version": {
+                        "title": "Temp Version",
+                        "type": "string"
+                    },
                     "version": {
                         "title": "Version",
                         "type": "string"
                     }
                 },
                 "required": [
                     "name",
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/package-lock.json` & `sqlmesh-0.8.0/web/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/package.json` & `sqlmesh-0.8.0/web/client/package.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/playwright.config.ts` & `sqlmesh-0.8.0/web/client/playwright.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/public/favicons/favicon.ico` & `sqlmesh-0.8.0/web/client/dist/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/api/channels.ts` & `sqlmesh-0.8.0/web/client/src/api/channels.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/api/index.ts` & `sqlmesh-0.8.0/web/client/src/api/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/api/instance.ts` & `sqlmesh-0.8.0/web/client/src/api/instance.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf` & `sqlmesh-0.8.0/web/client/dist/assets/CircularStd-Black-52659624.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf` & `sqlmesh-0.8.0/web/client/dist/assets/CircularStd-Bold-0e6c076d.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf` & `sqlmesh-0.8.0/web/client/dist/assets/CircularStd-Medium-2f373e53.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-Black.otf` & `sqlmesh-0.8.0/web/client/dist/assets/Publico-Black-e6bd2ea2.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-Bold.otf` & `sqlmesh-0.8.0/web/client/dist/assets/Publico-Bold-c79acd56.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-Italic.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-Light.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-Light.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-Medium.otf` & `sqlmesh-0.8.0/web/client/dist/assets/Publico-Medium-01b4a891.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/Publico-Roman.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/Publico-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf` & `sqlmesh-0.8.0/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/context/context.ts` & `sqlmesh-0.8.0/web/client/src/context/context.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/context/editor.ts` & `sqlmesh-0.8.0/web/client/src/context/editor.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/context/fileTree.ts` & `sqlmesh-0.8.0/web/client/src/context/fileTree.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/context/lineage.tsx` & `sqlmesh-0.8.0/web/client/src/context/lineage.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/context/plan.ts` & `sqlmesh-0.8.0/web/client/src/context/plan.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/context/theme.tsx` & `sqlmesh-0.8.0/web/client/src/context/theme.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/hooks/useLocalStorage.ts` & `sqlmesh-0.8.0/web/client/src/hooks/useLocalStorage.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/index.css` & `sqlmesh-0.8.0/web/client/src/index.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/banner/Banner.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/banner/Banner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/button/Button.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/button/Button.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -99,15 +99,19 @@
   [EnumSize.lg, `px-4 py-3 text-lg border-4`],
 ])
 
 const Button = makeButton(
   React.forwardRef<HTMLButtonElement, PropsButton>(ButtonPlain),
 )
 
-export { VARIANT, SHAPE, SIZE, Button, makeButton }
+const ButtonLink = makeButton(
+  React.forwardRef<HTMLDivElement, PropsButton>(ButtonLinkPlain),
+)
+
+export { VARIANT, SHAPE, SIZE, Button, ButtonLink, makeButton }
 
 function ButtonPlain(
   {
     type = 'button',
     disabled = false,
     children = [],
     form,
@@ -130,14 +134,30 @@
       className={className}
     >
       {children}
     </button>
   )
 }
 
+function ButtonLinkPlain(
+  { children = [], autoFocus, tabIndex, className }: PropsButton,
+  ref?: React.ForwardedRef<HTMLDivElement>,
+): JSX.Element {
+  return (
+    <div
+      ref={ref}
+      autoFocus={autoFocus}
+      tabIndex={tabIndex}
+      className={className}
+    >
+      {children}
+    </div>
+  )
+}
+
 function makeButton<TElement = HTMLButtonElement>(
   Component: React.ElementType,
 ): React.ForwardRefExoticComponent<
   PropsButton & React.RefAttributes<TElement>
 > {
   return React.forwardRef<TElement, PropsButton>(function Wrapper(
     {
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/button/tests/Button.spec.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/button/tests/Button.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/divider/Divider.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/divider/Divider.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/divider/tests/Divider.spec.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/divider/tests/Divider.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/Editor.css` & `sqlmesh-0.8.0/web/client/src/library/components/editor/Editor.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/EditorCode.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/editor/EditorCode.tsx`

 * *Files 13% similar despite different names*

```diff
@@ -1,228 +1,237 @@
-import { useCallback, useEffect, useMemo } from 'react'
+import React, { useCallback, useEffect, useMemo, useState } from 'react'
 import CodeMirror from '@uiw/react-codemirror'
 import { python } from '@codemirror/lang-python'
+import { sql } from '@codemirror/lang-sql'
 import { StreamLanguage } from '@codemirror/language'
 import { type KeyBinding, keymap } from '@codemirror/view'
 import { yaml } from '@codemirror/legacy-modes/mode/yaml'
 import { type Extension } from '@codemirror/state'
-import { type File } from '~/api/client'
+import { type Model, type File } from '~/api/client'
 import { useStoreFileTree } from '~/context/fileTree'
 import {
   events,
   SqlMeshModel,
   HoverTooltip,
   useSqlMeshExtension,
 } from './extensions'
 import { dracula, tomorrow } from 'thememirror'
 import { useColorScheme, EnumColorScheme } from '~/context/theme'
 
-import {
-  apiCancelFiles,
-  apiCancelPlanRun,
-  useApiFileByPath,
-  useApiPlanRun,
-  useMutationApiSaveFile,
-} from '~/api'
+import { useApiFileByPath, useApiPlanRun, useMutationApiSaveFile } from '~/api'
 import {
   debounceAsync,
   debounceSync,
   isFalse,
   isStringEmptyOrNil,
+  isStringNotEmpty,
 } from '~/utils'
 import { isCancelledError, useQueryClient } from '@tanstack/react-query'
 import { useStoreContext } from '~/context/context'
-import { type EditorTab, useStoreEditor } from '~/context/editor'
-import { EnumFileExtensions } from '@models/file'
+import { useStoreEditor, type Lineage } from '~/context/editor'
+import {
+  EnumFileExtensions,
+  type ModelFile,
+  type FileExtensions,
+} from '@models/file'
+import clsx from 'clsx'
+import Loading from '@components/loading/Loading'
+import Spinner from '@components/logo/Spinner'
+
+function CodeEditorDefault({
+  type,
+  content = '',
+  children,
+}: {
+  type: FileExtensions
+  content: string
+  children: (options: {
+    extensions: Extension[]
+    content: string
+  }) => JSX.Element
+}): JSX.Element {
+  const { mode } = useColorScheme()
+
+  const extensions = useMemo(() => {
+    return [
+      mode === EnumColorScheme.Dark ? dracula : tomorrow,
+      type === EnumFileExtensions.Python && python(),
+      type === EnumFileExtensions.YAML && StreamLanguage.define(yaml),
+      type === EnumFileExtensions.YML && StreamLanguage.define(yaml),
+      type === EnumFileExtensions.SQL && sql(),
+    ].filter(Boolean) as Extension[]
+  }, [type, mode])
 
-export default function CodeEditor({ tab }: { tab: EditorTab }): JSX.Element {
+  return (
+    <div className="flex overflow-auto h-full">
+      {children({ extensions, content })}
+    </div>
+  )
+}
+
+function CodeEditorSQLMesh({
+  content = '',
+  children,
+}: {
+  content?: string
+  children: (options: {
+    extensions: Extension[]
+    content: string
+  }) => JSX.Element
+}): JSX.Element {
   const { mode } = useColorScheme()
+
   const [SqlMeshDialect, SqlMeshDialectCleanUp] = useSqlMeshExtension()
 
   const models = useStoreContext(s => s.models)
-  const files = useStoreFileTree(s => s.files)
-  const selectFile = useStoreFileTree(s => s.selectFile)
 
-  const previewLineage = useStoreEditor(s => s.previewLineage)
-  const tabs = useStoreEditor(s => s.tabs)
-  const dialects = useStoreEditor(s => s.dialects)
   const engine = useStoreEditor(s => s.engine)
-  const refreshTab = useStoreEditor(s => s.refreshTab)
-  const closeTab = useStoreEditor(s => s.closeTab)
-  const selectTab = useStoreEditor(s => s.selectTab)
-  const createTab = useStoreEditor(s => s.createTab)
-
-  const handleEngineWorkerMessage = useCallback(
-    (e: MessageEvent): void => {
-      const t = tabs.get(tab.file)
-
-      if (t == null) return
-
-      if (e.data.topic === 'parse') {
-        t.isValid = e.data.payload?.type !== 'error' || tab.file.content === ''
-      }
-
-      if (e.data.topic === 'dialect') {
-        t.dialectOptions = e.data.payload
-      }
-    },
-    [tab.file],
-  )
+  const dialects = useStoreEditor(s => s.dialects)
+
+  const [dialectOptions, setDialectOptions] = useState<{
+    types: string
+    keywords: string
+  }>()
+
+  const updateDialectOptions = useCallback((e: MessageEvent): void => {
+    if (e.data.topic === 'dialect') {
+      setDialectOptions(e.data.payload)
+    }
+  }, [])
 
   const dialectsTitles = useMemo(
     () => dialects.map(d => d.dialect_title),
     [dialects],
   )
 
   const extensions = useMemo(() => {
-    const model = models.get(tab.file.path)
-    const columns = new Set(
-      Object.keys(previewLineage ?? {})
-        .map(modelName => models.get(modelName)?.columns.map(c => c.name))
-        .flat()
-        .filter(Boolean) as string[],
-    )
-
     return [
       mode === EnumColorScheme.Dark ? dracula : tomorrow,
-      HoverTooltip(models),
-      events(models, files, selectFile),
-      model != null && SqlMeshModel(models, model, columns),
-      tab.file.extension === EnumFileExtensions.Python && python(),
-      tab.file.extension === EnumFileExtensions.YAML &&
-        StreamLanguage.define(yaml),
-      tab.file.extension === EnumFileExtensions.SQL &&
-        tab.dialectOptions != null &&
-        SqlMeshDialect(models, tab.file, tab.dialectOptions, dialectsTitles),
-    ].filter(Boolean) as Extension[]
-  }, [
-    tab.file,
-    tab.dialectOptions,
-    models,
-    mode,
-    files,
-    dialectsTitles,
-    previewLineage,
-  ])
-
-  const keymaps = useMemo(
-    () => [
-      {
-        key: 'Mod-Alt-[',
-        preventDefault: true,
-        run() {
-          selectTab(createTab())
+      SqlMeshDialect(models, dialectOptions, dialectsTitles),
+    ]
+  }, [mode, dialectsTitles, dialectOptions])
 
-          return true
-        },
-      },
-      {
-        key: 'Mod-Alt-]',
-        preventDefault: true,
-        run() {
-          closeTab(tab.file)
-
-          return true
-        },
-      },
-    ],
-    [closeTab, selectTab, createTab, tab.file],
-  )
+  useEffect(() => {
+    return () => {
+      SqlMeshDialectCleanUp()
+    }
+  }, [])
 
   useEffect(() => {
-    engine.addEventListener('message', handleEngineWorkerMessage)
+    engine.addEventListener('message', updateDialectOptions)
 
     return () => {
-      engine.removeEventListener('message', handleEngineWorkerMessage)
-
-      SqlMeshDialectCleanUp()
+      engine.removeEventListener('message', updateDialectOptions)
     }
-  }, [handleEngineWorkerMessage])
+  }, [updateDialectOptions])
 
   useEffect(() => {
     engine.postMessage({
-      topic: 'parse',
-      payload: tab.file.content,
+      topic: 'dialect',
     })
-  }, [tab.file.content])
-
-  function updateFileContent(value: string): void {
-    tab.file.content = value
-    tab.isSaved = isFalse(tab.file.isChanged)
+  }, [content])
 
-    refreshTab()
-  }
-
-  return tab.file.isLocal ? (
-    <CodeEditorFileLocal
-      keymaps={keymaps}
-      extensions={extensions}
-      tab={tab}
-      onChange={updateFileContent}
-    />
-  ) : (
-    <CodeEditorFileRemote
-      keymaps={keymaps}
-      extensions={extensions}
-      tab={tab}
-      onChange={updateFileContent}
-    />
+  return (
+    <div className="flex overflow-auto h-full">
+      {children({ extensions, content })}
+    </div>
   )
 }
 
-function CodeEditorFileLocal({
-  keymaps,
-  extensions,
-  tab,
-  onChange,
+function CodeEditorRemoteFile({
+  path,
+  children,
 }: {
-  keymaps: KeyBinding[]
-  extensions: Extension[]
-  tab: EditorTab
-  onChange: (value: string) => void
+  path: string
+  children: (options: { file: ModelFile }) => JSX.Element
 }): JSX.Element {
-  const extensionKeymap = useMemo(() => keymap.of([...keymaps]), [keymaps])
+  const files = useStoreFileTree(s => s.files)
 
-  const extensionsAll = useMemo(
-    () => [...extensions, extensionKeymap],
-    [extensionKeymap, extensions],
-  )
+  const { refetch: getFileContent } = useApiFileByPath(path)
+  const debouncedGetFileContent = debounceAsync(getFileContent, 1000, true)
 
-  return (
-    <CodeMirror
-      height="100%"
-      width="100%"
-      className="w-full h-full overflow-auto text-sm font-mono"
-      value={tab.file.content}
-      extensions={extensionsAll}
-      onChange={onChange}
-    />
+  const [file, setFile] = useState<ModelFile>()
+
+  useEffect(() => {
+    const file = files.get(path)
+
+    if (file == null) return
+    if (isStringNotEmpty(file.content)) {
+      setFile(file)
+      return
+    }
+
+    debouncedGetFileContent({
+      throwOnError: true,
+    })
+      .then(({ data }) => {
+        file.updateContent(data?.content ?? '')
+
+        setFile(file)
+      })
+      .catch(error => {
+        if (isCancelledError(error)) {
+          console.log('getFileContent', 'Request aborted by React Query')
+        } else {
+          console.log('getFileContent', error)
+        }
+      })
+  }, [files, path])
+
+  return file == null ? (
+    <div className="flex justify-center items-center w-full h-full">
+      <Loading className="inline-block ">
+        <Spinner className="w-5 h-5 border border-neutral-10 mr-4" />
+        <h3 className="text-xl">Waiting for file...</h3>
+      </Loading>
+    </div>
+  ) : (
+    children({ file })
   )
 }
 
-function CodeEditorFileRemote({
-  keymaps,
-  extensions,
-  tab,
-  onChange,
-}: {
-  keymaps: KeyBinding[]
-  extensions: Extension[]
-  tab: EditorTab
-  onChange: (value: string) => void
-}): JSX.Element {
-  const client = useQueryClient()
+export function useSQLMeshModelExtensions(
+  path?: string,
+  lineage: Record<string, Lineage> = {},
+  handleModelClick?: (model: Model) => void,
+): Extension[] {
+  if (path == null) return []
 
   const models = useStoreContext(s => s.models)
+  const files = useStoreFileTree(s => s.files)
+
+  const extensions = useMemo(() => {
+    const model = models.get(path)
+    const columns = new Set(
+      Object.keys(lineage)
+        .map(modelName => models.get(modelName)?.columns.map(c => c.name))
+        .flat()
+        .filter(Boolean) as string[],
+    )
+
+    return [
+      HoverTooltip(models),
+      handleModelClick != null && events(models, handleModelClick),
+      model != null && SqlMeshModel(models, model, columns),
+    ].filter(Boolean) as Extension[]
+  }, [path, models, files])
+
+  return extensions
+}
+
+export function useSQLMeshModelKeymaps(file?: ModelFile): KeyBinding[] {
+  if (file == null) return []
+
+  const client = useQueryClient()
+
   const environment = useStoreContext(s => s.environment)
 
-  const engine = useStoreEditor(s => s.engine)
   const refreshTab = useStoreEditor(s => s.refreshTab)
 
-  const { refetch: getFileContent } = useApiFileByPath(tab.file.path)
+  const { refetch: getFileContent } = useApiFileByPath(file.path)
   const debouncedGetFileContent = debounceAsync(getFileContent, 1000, true)
 
   const mutationSaveFile = useMutationApiSaveFile(client, {
     onSuccess: saveChangeSuccess,
   })
 
   const { refetch: planRun } = useApiPlanRun(environment.name, {
@@ -233,113 +242,102 @@
 
   const debouncedPlanRun = useCallback(debounceAsync(planRun, 1000, true), [
     planRun,
   ])
 
   const debouncedSaveChange = useCallback(
     debounceSync(saveChange, 1000, true),
-    [tab],
-  )
-
-  const extensionKeymap = useMemo(
-    () =>
-      keymap.of([
-        ...keymaps,
-        {
-          mac: 'Cmd-s',
-          win: 'Ctrl-s',
-          linux: 'Ctrl-s',
-          preventDefault: true,
-          run() {
-            debouncedSaveChange(tab.file.content)
-
-            return true
-          },
-        },
-      ]),
-    [debouncedSaveChange, keymaps, tab.file.content],
+    [file],
   )
 
-  const extensionsAll = useMemo(
-    () => [...extensions, extensionKeymap],
-    [extensionKeymap, extensions],
-  )
-
-  useEffect(() => {
-    return () => {
-      debouncedPlanRun.cancel()
-      debouncedGetFileContent.cancel()
-
-      apiCancelPlanRun(client)
-      apiCancelFiles(client)
-    }
-  }, [])
-
   useEffect(() => {
-    if (isStringEmptyOrNil(tab.file.content)) {
+    if (isStringEmptyOrNil(file.content)) {
       debouncedGetFileContent({
         throwOnError: true,
       })
         .then(({ data }) => {
-          const model = models.get(tab.file.path)
-
-          tab.file.updateContent(data?.content ?? '')
-
-          if (model != null) {
-            tab.dialect = model.dialect
-
-            engine.postMessage({
-              topic: 'dialect',
-              payload: model.dialect,
-            })
-          }
-
-          engine.postMessage({
-            topic: 'parse',
-            payload: tab.file.content,
-          })
+          file.updateContent(data?.content ?? '')
         })
         .catch(error => {
           if (isCancelledError(error)) {
             console.log('getFileContent', 'Request aborted by React Query')
           } else {
             console.log('getFileContent', error)
-
-            tab.isSaved = false
-            tab.isValid = false
           }
         })
         .finally(() => {
           refreshTab()
         })
     }
-  }, [tab.file.path])
+  }, [file.path])
 
   function saveChange(): void {
+    if (file == null) return
+
     mutationSaveFile.mutate({
-      path: tab.file.path,
-      body: { content: tab.file.content },
+      path: file.path,
+      body: { content: file.content },
     })
   }
 
-  function saveChangeSuccess(file: File): void {
-    if (file == null) return
+  function saveChangeSuccess(newfile: File): void {
+    if (newfile == null || file == null) return
 
-    tab.file.updateContent(file.content)
-    tab.isSaved = true
+    file.updateContent(newfile.content)
 
     refreshTab()
 
     void debouncedPlanRun()
   }
 
+  return [
+    {
+      mac: 'Cmd-s',
+      win: 'Ctrl-s',
+      linux: 'Ctrl-s',
+      preventDefault: true,
+      run() {
+        debouncedSaveChange(file.content)
+
+        return true
+      },
+    },
+  ]
+}
+
+const CodeEditor = function CodeEditor({
+  keymaps = [],
+  extensions = [],
+  content = '',
+  onChange,
+  className,
+}: {
+  content?: string
+  keymaps?: KeyBinding[]
+  extensions?: Extension[]
+  onChange?: (value: string) => void
+  className?: string
+}): JSX.Element {
+  const extensionKeymap = useMemo(() => keymap.of([...keymaps]), [keymaps])
+  const extensionsAll = useMemo(
+    () => [...extensions, extensionKeymap],
+    [extensionKeymap, extensions],
+  )
+
   return (
     <CodeMirror
       height="100%"
       width="100%"
-      className="w-full h-full overflow-auto text-sm font-mono"
-      value={tab.file.content}
+      className={clsx('flex w-full h-full text-sm font-mono', className)}
+      value={content}
       extensions={extensionsAll}
       onChange={onChange}
+      readOnly={isFalse(Boolean(onChange))}
     />
   )
 }
+
+CodeEditor.Default = CodeEditorDefault
+CodeEditor.SQLMeshDialect = CodeEditorSQLMesh
+CodeEditor.RemoteFile = CodeEditorRemoteFile
+
+export default CodeEditor
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/EditorFooter.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/editor/EditorFooter.tsx`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     engine.postMessage({
       topic: 'dialect',
       payload: tab.dialect,
     })
   }
 
   return (
-    <div className="mr-4">
+    <div className="flex w-full mr-4 overflow-hidden items-center">
       <EditorIndicator
         className="mr-2"
         text="Valid"
       >
         <EditorIndicator.Light ok={tab.isValid} />
       </EditorIndicator>
       {tab.file.isRemote && (
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/EditorIndicator.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/editor/EditorIndicator.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/EditorInspector.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/editor/EditorInspector.tsx`

 * *Files 24% similar despite different names*

```diff
@@ -8,24 +8,28 @@
   type EvaluateInputEnd,
   type RenderInputEnd,
   type EvaluateInputLatest,
   type RenderInputLatest,
   fetchdfApiCommandsFetchdfPost,
   renderApiCommandsRenderPost,
   evaluateApiCommandsEvaluatePost,
+  type Model,
 } from '~/api/client'
 import { type ResponseWithDetail } from '~/api/instance'
 import { useStoreContext } from '~/context/context'
 import { EnumSize, EnumVariant } from '~/types/enum'
 import { isFalse, toDate, toDateFormat } from '~/utils'
 import { Button } from '../button/Button'
 import { Divider } from '../divider/Divider'
 import Input from '../input/Input'
 import { type EditorTab, useStoreEditor } from '~/context/editor'
 import { getTableDataFromArrowStreamResult } from './help'
+import { Tab } from '@headlessui/react'
+import Documentation from '@components/documentation/Documentation'
+import Banner from '@components/banner/Banner'
 
 interface FormModel {
   model?: string
   start: EvaluateInputStart | RenderInputStart
   end: EvaluateInputEnd | RenderInputEnd
   latest: EvaluateInputLatest | RenderInputLatest
   limit: number
@@ -39,38 +43,46 @@
 const LIMIT = 1000
 
 export default function EditorInspector({
   tab,
 }: {
   tab: EditorTab
 }): JSX.Element {
+  const models = useStoreContext(s => s.models)
+  const model = useMemo(() => models.get(tab.file.path), [tab, models])
+
   return (
     <div
       className={clsx(
         'flex flex-col w-full h-full items-center overflow-hidden',
       )}
     >
-      {tab.file.isSQLMeshModel ? (
-        <InspectorModel tab={tab} />
+      {tab.file.isSQLMeshModel && model != null ? (
+        <InspectorModel
+          tab={tab}
+          model={model}
+        />
       ) : (
         <InspectorSql tab={tab} />
       )}
     </div>
   )
 }
 
-function InspectorModel({ tab }: { tab: EditorTab }): JSX.Element {
-  const models = useStoreContext(s => s.models)
-
+function InspectorModel({
+  tab,
+  model,
+}: {
+  tab: EditorTab
+  model: Model
+}): JSX.Element {
   const setPreviewQuery = useStoreEditor(s => s.setPreviewQuery)
   const setPreviewConsole = useStoreEditor(s => s.setPreviewConsole)
   const setPreviewTable = useStoreEditor(s => s.setPreviewTable)
 
-  const model = useMemo(() => models.get(tab.file.path), [tab, models])
-
   const [form, setForm] = useState<FormModel>({
     start: toDateFormat(toDate(Date.now() - DAY)),
     end: toDateFormat(new Date()),
     latest: toDateFormat(toDate(Date.now() - DAY)),
     limit: 1000,
   })
 
@@ -120,117 +132,155 @@
             setPreviewConsole(error.message)
           }
         })
     }
   }
 
   return (
-    <>
-      <InspectorForm>
-        <form className="my-3">
-          {model != null && (
-            <FormFieldset>
-              <ModelName modelName={model.name} />
-            </FormFieldset>
-          )}
-          {isFalse(shouldEvaluate) && (
-            <FormFieldset>
-              <Banner action="evaluate the model" />
-            </FormFieldset>
+    <Tab.Group>
+      <Tab.List className="w-full whitespace-nowrap px-2 pt-3 flex justigy-between items-center">
+        <Tab
+          className={({ selected }) =>
+            clsx(
+              'inline-block text-sm font-medium px-3 py-1 mr-2 last-child:mr-0 rounded-md relative',
+              selected
+                ? 'bg-secondary-500 text-secondary-100 cursor-default'
+                : 'bg-secondary-10 cursor-pointer',
+            )
+          }
+        >
+          Actions
+        </Tab>
+        <Tab
+          className={({ selected }) =>
+            clsx(
+              'inline-block text-sm font-medium px-3 py-1 mr-2 last-child:mr-0 rounded-md relative',
+              selected
+                ? 'bg-secondary-500 text-secondary-100 cursor-default'
+                : 'bg-secondary-10 cursor-pointer',
+            )
+          }
+        >
+          Docs
+        </Tab>
+      </Tab.List>
+      <Tab.Panels className="h-full w-full overflow-hidden">
+        <Tab.Panel
+          className={clsx(
+            'flex flex-col w-full h-full pt-4 relative px-2 overflow-hidden',
+            'ring-white ring-opacity-60 ring-offset-2 ring-offset-blue-400 focus:outline-none focus:ring-2',
           )}
-          <fieldset className="my-3 px-3">
-            <Input
-              className="w-full mx-0"
-              label="Start Date"
-              placeholder="02/11/2023"
-              value={form.start}
-              onInput={(e: React.ChangeEvent<HTMLInputElement>) => {
-                e.stopPropagation()
-
-                setForm({
-                  ...form,
-                  start: e.target.value ?? '',
-                })
-              }}
-            />
-            <Input
-              className="w-full mx-0"
-              label="End Date"
-              placeholder="02/13/2023"
-              value={form.end}
-              onInput={(e: React.ChangeEvent<HTMLInputElement>) => {
-                e.stopPropagation()
-
-                setForm({
-                  ...form,
-                  end: e.target.value ?? '',
-                })
-              }}
-            />
-            <Input
-              className="w-full mx-0"
-              label="Latest Date"
-              placeholder="02/13/2023"
-              value={form.latest}
-              onInput={(e: React.ChangeEvent<HTMLInputElement>) => {
-                e.stopPropagation()
-
-                setForm({
-                  ...form,
-                  latest: e.target.value ?? '',
-                })
-              }}
-            />
-            <Input
-              className="w-full mx-0"
-              type="number"
-              label="Limit"
-              placeholder="1000"
-              value={form.limit}
-              onInput={(e: React.ChangeEvent<HTMLInputElement>) => {
-                e.stopPropagation()
-
-                setForm({
-                  ...form,
-                  limit: e.target.valueAsNumber ?? LIMIT,
-                })
-              }}
-            />
-          </fieldset>
-        </form>
-      </InspectorForm>
-      <Divider />
-      <InspectorActions>
-        <div className="flex w-full justify-between">
-          <div className="flex">
-            <Button
-              size={EnumSize.sm}
-              variant={EnumVariant.Alternative}
-              disabled={isFalse(shouldEvaluate)}
-            >
-              Validate
-            </Button>
-          </div>
-          {tab.file.isSQLMeshModel && (
-            <Button
-              size={EnumSize.sm}
-              variant={EnumVariant.Alternative}
-              disabled={isFalse(shouldEvaluate)}
-              onClick={e => {
-                e.stopPropagation()
-
-                evaluateModel()
-              }}
-            >
-              Evaluate
-            </Button>
+        >
+          <InspectorForm>
+            <form className="my-3">
+              {isFalse(shouldEvaluate) && (
+                <FormFieldset>
+                  <Banner variant={EnumVariant.Warning}>
+                    <Banner.Description className="w-full mr-2 text-sm">
+                      Please fill out all fields to <b>evaluate the model</b>.
+                    </Banner.Description>
+                  </Banner>
+                </FormFieldset>
+              )}
+              <fieldset className="my-3 px-3">
+                <Input
+                  className="w-full mx-0"
+                  label="Start Date"
+                  placeholder="02/11/2023"
+                  value={form.start}
+                  onInput={(e: React.ChangeEvent<HTMLInputElement>) => {
+                    e.stopPropagation()
+
+                    setForm({
+                      ...form,
+                      start: e.target.value ?? '',
+                    })
+                  }}
+                />
+                <Input
+                  className="w-full mx-0"
+                  label="End Date"
+                  placeholder="02/13/2023"
+                  value={form.end}
+                  onInput={(e: React.ChangeEvent<HTMLInputElement>) => {
+                    e.stopPropagation()
+
+                    setForm({
+                      ...form,
+                      end: e.target.value ?? '',
+                    })
+                  }}
+                />
+                <Input
+                  className="w-full mx-0"
+                  label="Latest Date"
+                  placeholder="02/13/2023"
+                  value={form.latest}
+                  onInput={(e: React.ChangeEvent<HTMLInputElement>) => {
+                    e.stopPropagation()
+
+                    setForm({
+                      ...form,
+                      latest: e.target.value ?? '',
+                    })
+                  }}
+                />
+                <Input
+                  className="w-full mx-0"
+                  type="number"
+                  label="Limit"
+                  placeholder="1000"
+                  value={form.limit}
+                  onInput={(e: React.ChangeEvent<HTMLInputElement>) => {
+                    e.stopPropagation()
+
+                    setForm({
+                      ...form,
+                      limit: e.target.valueAsNumber ?? LIMIT,
+                    })
+                  }}
+                />
+              </fieldset>
+            </form>
+          </InspectorForm>
+          <Divider />
+          <InspectorActions>
+            <div className="flex w-full justify-end">
+              {tab.file.isSQLMeshModel && (
+                <Button
+                  size={EnumSize.sm}
+                  variant={EnumVariant.Alternative}
+                  disabled={isFalse(shouldEvaluate)}
+                  onClick={e => {
+                    e.stopPropagation()
+
+                    evaluateModel()
+                  }}
+                >
+                  Evaluate
+                </Button>
+              )}
+            </div>
+          </InspectorActions>
+        </Tab.Panel>
+        <Tab.Panel
+          className={clsx(
+            'w-full h-full ring-white ring-opacity-60 ring-offset-2 ring-offset-blue-400 focus:outline-none focus:ring-2 p-2',
           )}
-        </div>
-      </InspectorActions>
-    </>
+        >
+          <Documentation
+            model={model}
+            withCode={false}
+            withModel={false}
+            withQuery={tab.file.isSQLMeshModelSQL}
+            withDescription={false}
+          />
+        </Tab.Panel>
+      </Tab.Panels>
+    </Tab.Group>
   )
 }
 
 function InspectorSql({ tab }: { tab: EditorTab }): JSX.Element {
   const setPreviewQuery = useStoreEditor(s => s.setPreviewQuery)
   const setPreviewConsole = useStoreEditor(s => s.setPreviewConsole)
   const setPreviewTable = useStoreEditor(s => s.setPreviewTable)
@@ -266,15 +316,19 @@
 
   return (
     <>
       <InspectorForm>
         <form className="my-3 w-full">
           {isFalse(shouldSendQuery) && (
             <FormFieldset>
-              <Banner action="run the query" />
+              <Banner variant={EnumVariant.Warning}>
+                <Banner.Description className="w-full mr-2 text-sm">
+                  Please fill out all fields to <b>run the query</b>.
+                </Banner.Description>
+              </Banner>
             </FormFieldset>
           )}
           <fieldset className="mb-4">
             <Input
               className="w-full mx-0"
               type="number"
               label="Limit"
@@ -334,28 +388,7 @@
 function InspectorActions({
   children,
 }: {
   children: React.ReactNode
 }): JSX.Element {
   return <div className="flex w-full py-1 px-2 justify-end">{children}</div>
 }
-
-function Banner({ action }: { action: string }): JSX.Element {
-  return (
-    <div className="p-4 bg-warning-10 text-warning-600 rounded-lg">
-      <p className="text-sm">
-        Please fill out all fields to <b>{action}</b>.
-      </p>
-    </div>
-  )
-}
-
-function ModelName({ modelName }: { modelName: string }): JSX.Element {
-  return (
-    <div className="text-sm font-bold whitespace-nowrap">
-      <h3 className="ml-2">Model Name</h3>
-      <p className="mt-1 px-2 py-1 bg-secondary-10 text-secondary-500 dark:text-primary-500 dark:bg-primary-10 text-xs rounded">
-        {modelName}
-      </p>
-    </div>
-  )
-}
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/EditorPreview.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/editor/EditorPreview.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -337,10 +337,11 @@
     <div className="w-full h-full flex items-center justify-center bg-primary-10">
       <Loading hasSpinner>Loading Lineage...</Loading>
     </div>
   ) : (
     <Graph
       lineage={previewLineage}
       highlightedNodes={highlightedNodes}
+      models={models}
     />
   )
 }
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/EditorTabs.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/editor/EditorTabs.tsx`

 * *Files 9% similar despite different names*

```diff
@@ -44,22 +44,22 @@
         }}
       >
         <PlusIcon className="inline-block w-3 h-4 text-secondary-500 dark:text-primary-500" />
       </Button>
       <ul className="w-full whitespace-nowrap min-h-[2rem] max-h-[2rem] overflow-hidden overflow-x-auto scrollbar scrollbar--horizontal">
         {tabsLocal.map((tab, idx) => (
           <Tab
-            key={tab.file.id}
+            key={tab.id}
             tab={tab}
             title={`Custom SQL ${idx + 1}`}
           />
         ))}
         {tabsRemote.map(tab => (
           <Tab
-            key={tab.file.id}
+            key={tab.id}
             tab={tab}
             title={tab.file.name}
           />
         ))}
       </ul>
     </div>
   )
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts` & `sqlmesh-0.8.0/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts`

 * *Files 10% similar despite different names*

```diff
@@ -2,55 +2,48 @@
   completeFromList,
   type CompletionContext,
   type Completion,
 } from '@codemirror/autocomplete'
 import { keywordCompletionSource, SQLDialect } from '@codemirror/lang-sql'
 import { LanguageSupport } from '@codemirror/language'
 import { type Model } from '~/api/client'
-import { type ModelFile } from '~/models'
 import { isFalse } from '~/utils'
 import { sqlglotWorker } from '~/workers'
 
 const cache = new Map<string, (e: MessageEvent) => void>()
 const WHITE_SPACE = ' '
 
 type ExtensionCleanUp = () => void
 type ExtensionSqlMeshDialect = (
   models: Map<string, Model>,
-  file: ModelFile,
-  options: { types: string; keywords: string },
+  options?: { types: string; keywords: string },
   dialects?: string[],
 ) => LanguageSupport
 
 export function useSqlMeshExtension(): [
   ExtensionSqlMeshDialect,
   ExtensionCleanUp,
 ] {
   const SqlMeshDialectExtension: ExtensionSqlMeshDialect =
     function SqlMeshDialectExtension(
       models,
-      file,
       options,
       dialects?,
     ): LanguageSupport {
-      const SQLTypes = options.types
-      const SQLKeywords = options.keywords
+      const SQLTypes = (options?.types ?? '') + WHITE_SPACE
+      const SQLKeywords = (options?.keywords ?? '') + WHITE_SPACE
       const SQLMeshModelDictionary = SQLMeshModelKeywords(dialects)
       const SQLMeshKeywords =
         'model name kind owner cron start storage_format time_column partitioned_by pre post batch_size audits dialect'
       const SQLMeshTypes =
         'seed full incremental_by_time_range incremental_by_unique_key view embedded'
 
       const lang = SQLDialect.define({
-        keywords:
-          SQLKeywords +
-          (file.isSQLMeshModel ? SQLMeshKeywords : '') +
-          WHITE_SPACE,
-        types:
-          SQLTypes + (file.isSQLMeshModel ? SQLMeshTypes : '') + WHITE_SPACE,
+        keywords: SQLKeywords + SQLMeshKeywords + WHITE_SPACE,
+        types: SQLTypes + SQLMeshTypes + WHITE_SPACE,
       })
 
       const tables: Completion[] = Array.from(
         new Set(Object.values(models)),
       ).map(label => ({
         label,
         type: 'keyword',
@@ -101,15 +94,15 @@
               .some(
                 ([start, end]: [number, number]) =>
                   ctx.pos >= start && ctx.pos <= end,
               )
 
             let suggestions: Completion[] = tables
 
-            if (isFalse(isInsideModel) || isFalse(file.isSQLMeshModel)) {
+            if (isFalse(isInsideModel)) {
               if (keywordFrom != null)
                 return await completeFromList(suggestions)(ctx)
 
               return await keywordCompletionSource(lang)(ctx)
             }
 
             suggestions = SQLMeshModelDictionary.get('keywords') ?? []
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/extensions/index.ts` & `sqlmesh-0.8.0/web/client/src/library/components/editor/extensions/index.ts`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,14 @@
   Decoration,
   type ViewUpdate,
   EditorView,
   type Tooltip,
   hoverTooltip,
 } from '@codemirror/view'
 import { type Model } from '~/api/client'
-import { type ModelFile } from '~/models'
 
 import { useSqlMeshExtension } from './SqlMeshDialect'
 import { isFalse } from '@utils/index'
 
 export { useSqlMeshExtension }
 
 export function SqlMeshModel(
@@ -42,20 +41,31 @@
       decorations: value => value.decorations,
     },
   )
 }
 
 export function events(
   models: Map<string, Model>,
-  files: Map<ID, ModelFile>,
-  selectFile: (file: ModelFile) => void,
+  handler: (model: Model) => void,
 ): Extension {
   return EditorView.domEventHandlers({
     click(event: MouseEvent) {
-      handleClickOnSqlMeshModel(event, models, files, selectFile)
+      if (event.target == null) return
+
+      const el = event.target as HTMLElement
+      const modelName =
+        el.getAttribute('model') ?? el.parentElement?.getAttribute('model')
+
+      if (modelName == null) return
+
+      const model = models.get(modelName)
+
+      if (model == null) return
+
+      handler(model)
     },
   })
 }
 
 export function HoverTooltip(models: Map<string, Model>): Extension {
   return hoverTooltip(
     (view: EditorView, pos: number, side: number): Tooltip | null => {
@@ -182,33 +192,7 @@
         decoration != null && decorations.push(decoration)
       },
     })
   }
 
   return Decoration.set(decorations)
 }
-
-function handleClickOnSqlMeshModel(
-  event: MouseEvent,
-  models: Map<string, Model>,
-  files: Map<ID, ModelFile>,
-  selectFile: (file: ModelFile) => void,
-): void {
-  if (event.target == null) return
-
-  const el = event.target as HTMLElement
-  const modelName =
-    el.getAttribute('model') ?? el.parentElement?.getAttribute('model')
-
-  if (modelName == null) return
-
-  const model = models.get(modelName)
-
-  if (model == null) return
-
-  const id = model.path as ID
-  const file = files.get(id)
-
-  if (file != null) {
-    selectFile(file)
-  }
-}
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/editor/help.ts` & `sqlmesh-0.8.0/web/client/src/library/components/editor/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/fileTree/Directory.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/fileTree/Directory.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/fileTree/File.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/fileTree/File.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/fileTree/FileTree.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/fileTree/FileTree.tsx`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,40 @@
 import { type MouseEvent, useEffect, useState } from 'react'
 import clsx from 'clsx'
-import { type Directory as DirectoryApi } from '../../../api/client'
 import ModalConfirmation from '../modal/ModalConfirmation'
 import type { Confirmation } from '../modal/ModalConfirmation'
 import { Button } from '../button/Button'
 import { isNotNil } from '~/utils'
 import Directory from './Directory'
-import { useStoreFileTree } from '~/context/fileTree'
+import { type ModelDirectory } from '@models/directory'
 
 /* TODO:
   - add ability to create file or directory on top level
   - add context menu
   - add drag and drop
   - add copy and paste
   - add move
   - add search
 */
 
 interface PropsFolderTree extends React.HTMLAttributes<HTMLElement> {
-  project?: DirectoryApi
+  project?: ModelDirectory
 }
 
 export default function FolderTree({
   project,
   className,
 }: PropsFolderTree): JSX.Element {
-  const directory = useStoreFileTree(s => s.project)
-  const setFiles = useStoreFileTree(s => s.setFiles)
-  const setProject = useStoreFileTree(s => s.setProject)
-
   const [confirmation, setConfirmation] = useState<Confirmation | undefined>()
   const [showConfirmation, setShowConfirmation] = useState(false)
 
   useEffect(() => {
     setShowConfirmation(isNotNil(confirmation))
   }, [confirmation])
 
-  useEffect(() => {
-    setFiles(directory?.allFiles ?? [])
-  }, [directory])
-
-  useEffect(() => {
-    setProject(project)
-  }, [project])
-
   return (
     <div
       className={clsx(
         'py-2 px-1 overflow-hidden overflow-y-auto text-sm scrollbar scrollbar--vertical',
         className,
       )}
     >
@@ -93,16 +80,16 @@
               setShowConfirmation(false)
             }}
           >
             {confirmation?.noText ?? 'Cancel'}
           </Button>
         </ModalConfirmation.Actions>
       </ModalConfirmation>
-      {directory != null && (
+      {project != null && (
         <Directory
-          directory={directory}
+          directory={project}
           setConfirmation={setConfirmation}
         />
       )}
     </div>
   )
 }
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/fileTree/help.ts` & `sqlmesh-0.8.0/web/client/src/library/components/fileTree/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/graph/Graph.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/graph/Graph.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -26,33 +26,34 @@
 } from './help'
 import { debounceAsync, isArrayNotEmpty, isFalse, isTrue } from '../../../utils'
 import { EnumSize, EnumVariant } from '~/types/enum'
 import { useStoreContext } from '@context/context'
 import { ArrowRightCircleIcon } from '@heroicons/react/24/solid'
 import { useStoreLineage, useStoreReactFlow } from '@context/lineage'
 import clsx from 'clsx'
-import { type Column } from '@api/client'
+import { type Model, type Column } from '@api/client'
 import { useStoreFileTree } from '@context/fileTree'
 import { useApiColumnLineage } from '@api/index'
 import { useStoreEditor, type Lineage } from '@context/editor'
 import Loading from '@components/loading/Loading'
 import Spinner from '@components/logo/Spinner'
 import './Graph.css'
+import { type ModelFile } from '@models/file'
 
 const Flow = memo(function Flow({
   lineage,
   closeGraph,
   highlightedNodes = [],
+  models,
 }: {
   lineage: Record<string, Lineage>
   closeGraph?: () => void
   highlightedNodes?: string[]
+  models: Map<string, Model>
 }): JSX.Element {
-  const models = useStoreContext(s => s.models)
-
   const nodes = useStoreReactFlow(s => s.nodes)
   const edges = useStoreReactFlow(s => s.edges)
   const setNodes = useStoreReactFlow(s => s.setNodes)
   const setEdges = useStoreReactFlow(s => s.setEdges)
   const onNodesChange = useStoreReactFlow(s => s.onNodesChange)
   const onEdgesChange = useStoreReactFlow(s => s.onEdgesChange)
   const onConnect = useStoreReactFlow(s => s.onConnect)
@@ -171,20 +172,21 @@
   const selectFile = useStoreFileTree(s => s.selectFile)
 
   const activeEdges = useStoreLineage(s => s.activeEdges)
   const addActiveEdges = useStoreLineage(s => s.addActiveEdges)
   const removeActiveEdges = useStoreLineage(s => s.removeActiveEdges)
 
   const model = models.get(data.label)
-  const file = model != null ? files.get(model.path) : undefined
   const columns = model != null ? model.columns : []
 
   const [showColumns, setShowColumns] = useState(
     columns.length <= COLUMS_LIMIT_DEFAULT,
   )
+  const [file, setFile] = useState<ModelFile>()
+
   const toggleEdgeById = useCallback(
     function toggleEdgeById(
       action: 'add' | 'remove',
       edgeIds: [string, string],
       connections: { ins: string[]; outs: string[] } = { ins: [], outs: [] },
     ): void {
       const edges = [
@@ -217,14 +219,20 @@
         hidden.push(column)
       }
     })
 
     return [visible, hidden]
   }, [columns, showColumns, activeEdges])
 
+  useEffect(() => {
+    if (model == null) return
+
+    setFile(files.get(model.path))
+  }, [files, model])
+
   return (
     <div
       className={clsx(
         'text-xs font-semibold text-secondary-500 dark:text-primary-100 rounded-xl shadow-lg relative z-1',
         isTrue(data.isHighlighted) && 'border-4 border-brand-500',
       )}
     >
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/graph/help.ts` & `sqlmesh-0.8.0/web/client/src/library/components/graph/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/ide/ActivePlan.tsx` & `sqlmesh-0.8.0/web/client/src/library/pages/ide/ActivePlan.tsx`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import { Button } from '@components/button/Button'
+import TasksOverview from '@components/tasksOverview/TasksOverview'
 import { Popover, Transition } from '@headlessui/react'
 import { useQueryClient } from '@tanstack/react-query'
 import clsx from 'clsx'
 import { Fragment, type MouseEvent } from 'react'
 import { apiCancelPlanApply } from '~/api'
 import { useStoreContext } from '~/context/context'
 import {
@@ -9,16 +11,14 @@
   type PlanState,
   useStorePlan,
   EnumPlanState,
   EnumPlanAction,
   EnumPlanApplyType,
 } from '~/context/plan'
 import { EnumSize, EnumVariant } from '~/types/enum'
-import { Button } from '../button/Button'
-import TasksOverview from '../tasksOverview/TasksOverview'
 
 export default function ActivePlan({
   plan,
 }: {
   plan: PlanProgress
 }): JSX.Element {
   const client = useQueryClient()
@@ -61,22 +61,30 @@
             leave="transition ease-in duration-150"
             leaveFrom="opacity-100 translate-y-0"
             leaveTo="opacity-0 translate-y-1"
           >
             <Popover.Panel className="absolute right-1 z-10 mt-8 transform">
               <div className="overflow-hidden rounded-lg bg-theme shadow-lg ring-1 ring-black ring-opacity-5">
                 <TasksOverview tasks={plan.tasks}>
-                  {({ total, completed, models }) => (
+                  {({
+                    total,
+                    completed,
+                    models,
+                    completedBatches,
+                    totalBatches,
+                  }) => (
                     <>
                       <TasksOverview.Summary
                         environment={environment.name}
                         planState={planState}
                         headline="Most Recent Plan"
                         completed={completed}
                         total={total}
+                        completedBatches={completedBatches}
+                        totalBatches={totalBatches}
                         updateType={
                           plan.type === EnumPlanApplyType.Virtual
                             ? 'Virtual'
                             : 'Backfill'
                         }
                         updatedAt={plan.updated_at}
                       />
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/ide/IDE.tsx` & `sqlmesh-0.8.0/web/client/src/library/pages/ide/IDE.tsx`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,52 @@
-import { Divider } from '../divider/Divider'
-import { useEffect, useState, lazy, useCallback } from 'react'
+import { useEffect, useCallback } from 'react'
+import { useQueryClient } from '@tanstack/react-query'
 import {
   useApiFiles,
   useApiEnvironments,
   apiCancelGetEnvironments,
   apiCancelFiles,
   useApiModels,
   apiCancelModels,
 } from '../../../api'
-import { EnumPlanAction, useStorePlan } from '../../../context/plan'
+import { useStorePlan } from '../../../context/plan'
 import { useChannelEvents } from '../../../api/channels'
-import SplitPane from '../splitPane/SplitPane'
-import { isArrayEmpty, isFalse, isTrue, debounceAsync } from '~/utils'
+import { isArrayEmpty, debounceAsync } from '~/utils'
 import { useStoreContext } from '~/context/context'
-import PlanProvider from '../plan/context'
+import { Divider } from '@components/divider/Divider'
+import Container from '@components/container/Container'
 import RunPlan from './RunPlan'
 import ActivePlan from './ActivePlan'
-import { Dialog } from '@headlessui/react'
-import { useQueryClient } from '@tanstack/react-query'
-import ModalSidebar from '../modal/ModalDrawer'
-import Editor from '../editor/Editor'
-import FileTree from '../fileTree/FileTree'
+import { ArrowLongRightIcon } from '@heroicons/react/24/solid'
+import { Button } from '@components/button/Button'
+import { EnumSize, EnumVariant } from '~/types/enum'
+import { Link, Outlet, useLocation, useNavigate } from 'react-router-dom'
+import { EnumRoutes } from '~/routes'
+import { useIDE } from './context'
+import { useStoreFileTree } from '@context/fileTree'
+
+export default function IDE(): JSX.Element {
+  const location = useLocation()
+  const navigate = useNavigate()
 
-const Plan = lazy(async () => await import('../plan/Plan'))
-
-export function IDE(): JSX.Element {
   const client = useQueryClient()
 
-  const environment = useStoreContext(s => s.environment)
-  const initialStartDate = useStoreContext(s => s.initialStartDate)
-  const initialEndDate = useStoreContext(s => s.initialEndDate)
+  const { setIsPlanOpen } = useIDE()
+
   const addSyncronizedEnvironments = useStoreContext(
     s => s.addSyncronizedEnvironments,
   )
   const setModels = useStoreContext(s => s.setModels)
 
   const activePlan = useStorePlan(s => s.activePlan)
-  const setPlanAction = useStorePlan(s => s.setAction)
   const updateTasks = useStorePlan(s => s.updateTasks)
 
-  const [isPlanOpen, setIsPlanOpen] = useState(false)
-  const [isClosingModal, setIsClosingModal] = useState(false)
+  const directory = useStoreFileTree(s => s.project)
+  const setFiles = useStoreFileTree(s => s.setFiles)
+  const setProject = useStoreFileTree(s => s.setProject)
 
   const [subscribe] = useChannelEvents()
 
   const { data: dataModels, refetch: getModels } = useApiModels()
   const { data: project, refetch: getFiles } = useApiFiles()
   const { data: contextEnvironemnts, refetch: getEnvironments } =
     useApiEnvironments()
@@ -79,80 +81,72 @@
 
       unsubscribeTasks?.()
       unsubscribeModels?.()
     }
   }, [])
 
   useEffect(() => {
+    if (location.pathname === EnumRoutes.Ide) {
+      navigate(EnumRoutes.IdeEditor)
+    }
+  }, [location])
+
+  useEffect(() => {
     if (
       contextEnvironemnts == null ||
       isArrayEmpty(Object.keys(contextEnvironemnts))
     )
       return
 
     addSyncronizedEnvironments(Object.values(contextEnvironemnts))
   }, [contextEnvironemnts])
 
   useEffect(() => {
     setModels(dataModels)
   }, [dataModels])
 
+  useEffect(() => {
+    setFiles(directory?.allFiles ?? [])
+  }, [directory])
+
+  useEffect(() => {
+    setProject(project)
+  }, [project])
+
   function showRunPlan(): void {
     setIsPlanOpen(true)
   }
 
-  function closeModal(): void {
-    setIsClosingModal(true)
-  }
+  const isActivePageEditor = location.pathname === EnumRoutes.IdeEditor
 
   return (
-    <>
+    <Container.Page>
       <div className="w-full flex justify-between items-center min-h-[2rem] z-50">
         <div className="px-3 flex items-center whitespace-nowrap">
           <h3 className="font-bold text-primary-500">
             <span className="inline-block">/</span>
             {project?.name}
           </h3>
+          <ArrowLongRightIcon className="w-8 mx-4 text-neutral-50" />
+          <Button
+            size={EnumSize.sm}
+            variant={EnumVariant.Neutral}
+          >
+            {isActivePageEditor ? (
+              <Link to={EnumRoutes.IdeDocs}>Docs</Link>
+            ) : (
+              <Link to={EnumRoutes.IdeEditor}>Editor</Link>
+            )}
+          </Button>
         </div>
-        <div className="px-3 flex items-center min-w-[10rem] justify-end">
-          <RunPlan showRunPlan={showRunPlan} />
-          {activePlan != null && <ActivePlan plan={activePlan} />}
-        </div>
+        {isActivePageEditor && (
+          <div className="px-3 flex items-center min-w-[10rem] justify-end">
+            <RunPlan showRunPlan={showRunPlan} />
+            {activePlan != null && <ActivePlan plan={activePlan} />}
+          </div>
+        )}
       </div>
       <Divider />
-      {environment != null && (
-        <SplitPane
-          sizes={[20, 80]}
-          minSize={[160]}
-          snapOffset={0}
-          className="flex w-full h-full overflow-hidden"
-        >
-          <FileTree project={project} />
-          <Editor />
-        </SplitPane>
-      )}
-      <ModalSidebar
-        show={isPlanOpen && isFalse(isClosingModal)}
-        afterLeave={() => {
-          setPlanAction(EnumPlanAction.None)
-          setIsClosingModal(false)
-          setIsPlanOpen(false)
-        }}
-      >
-        <Dialog.Panel className="bg-theme border-8 border-r-0 border-secondary-10 dark:border-primary-10 absolute w-[90%] md:w-[75%] xl:w-[60%] h-full right-0">
-          <PlanProvider>
-            <Plan
-              environment={environment}
-              isInitialPlanRun={
-                environment?.isDefault == null || isTrue(environment?.isDefault)
-              }
-              disabled={isClosingModal}
-              initialStartDate={initialStartDate}
-              initialEndDate={initialEndDate}
-              onClose={closeModal}
-            />
-          </PlanProvider>
-        </Dialog.Panel>
-      </ModalSidebar>
-    </>
+      <Outlet />
+    </Container.Page>
   )
 }
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/ide/RunPlan.tsx` & `sqlmesh-0.8.0/web/client/src/library/pages/ide/RunPlan.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -1,54 +1,49 @@
 import { Menu, Popover, Transition } from '@headlessui/react'
 import { ChevronDownIcon, CheckCircleIcon } from '@heroicons/react/24/solid'
-import { useQueryClient } from '@tanstack/react-query'
 import clsx from 'clsx'
 import {
   useState,
   useEffect,
   Fragment,
   type MouseEvent,
   useMemo,
   useCallback,
 } from 'react'
-import {
-  apiCancelGetEnvironments,
-  apiCancelPlanRun,
-  useApiEnvironments,
-  useApiPlanRun,
-} from '~/api'
+import { useApiEnvironments, useApiPlanRun } from '~/api'
 import { type ContextEnvironment } from '~/api/client'
 import { useStoreContext } from '~/context/context'
 import { useStorePlan, EnumPlanState, EnumPlanAction } from '~/context/plan'
 import { type ModelEnvironment } from '~/models/environment'
 import { EnumSize, EnumVariant } from '~/types/enum'
 import {
   isArrayNotEmpty,
   includes,
   isFalse,
   isStringEmptyOrNil,
   debounceAsync,
 } from '~/utils'
-import { Button, makeButton, type ButtonSize } from '../button/Button'
-import { Divider } from '../divider/Divider'
-import Input from '../input/Input'
-import Spinner from '../logo/Spinner'
+import { Button, makeButton, type ButtonSize } from '@components/button/Button'
+import { Divider } from '@components/divider/Divider'
+import Input from '@components/input/Input'
+import Spinner from '@components/logo/Spinner'
 import ModalConfirmation, {
   type Confirmation,
-} from '../modal/ModalConfirmation'
-import { EnumPlanChangeType, type PlanChangeType } from '../plan/context'
-import PlanChangePreview from '../plan/PlanChangePreview'
+} from '@components/modal/ModalConfirmation'
+import {
+  EnumPlanChangeType,
+  type PlanChangeType,
+} from '@components/plan/context'
+import PlanChangePreview from '@components/plan/PlanChangePreview'
 
 export default function RunPlan({
   showRunPlan,
 }: {
   showRunPlan: () => void
 }): JSX.Element {
-  const client = useQueryClient()
-
   const planState = useStorePlan(s => s.state)
   const planAction = useStorePlan(s => s.action)
   const setPlanState = useStorePlan(s => s.setState)
   const setPlanAction = useStorePlan(s => s.setAction)
   const setActivePlan = useStorePlan(s => s.setActivePlan)
 
   const environment = useStoreContext(s => s.environment)
@@ -91,24 +86,14 @@
             startPlan()
           },
         }
       : undefined
   }, [environment])
 
   useEffect(() => {
-    return () => {
-      debouncedGetEnvironemnts.cancel()
-      debouncedPlanRun.cancel()
-
-      apiCancelPlanRun(client)
-      apiCancelGetEnvironments(client)
-    }
-  }, [])
-
-  useEffect(() => {
     debouncedPlanRun().finally(() => {
       if (shouldStartPlanAutomatically) {
         startPlan()
         setShouldSartPlanAutomatically(false)
       }
     })
   }, [environment, shouldStartPlanAutomatically])
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/input/Input.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/input/Input.tsx`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
   label,
   info,
   value = '',
   placeholder,
   className,
   size = EnumSize.md,
   disabled = false,
+  autoFocus = false,
   onInput,
 }: PropsInput): JSX.Element {
   return (
     <div className={clsx('inline-block relative m-1', className)}>
       {label != null && <InputLabel>{label}</InputLabel>}
       <input
         className={clsx(
@@ -37,14 +38,15 @@
           isTrue(disabled) && 'opacity-50 cursor-not-allowed',
         )}
         type={type}
         value={value}
         placeholder={placeholder}
         onInput={onInput}
         disabled={disabled}
+        autoFocus={autoFocus}
       />
       {info != null && <InputInfo>{info}</InputInfo>}
     </div>
   )
 }
 
 function InputLabel({
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/input/InputToggle.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/input/InputToggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/logo/Spinner.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/logo/Spinner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/logo/SqlMesh.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/logo/SqlMesh.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/logo/Tobiko.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/logo/Tobiko.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/modal/Modal.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/modal/Modal.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/modal/ModalConfirmation.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/modal/ModalConfirmation.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/modal/ModalDrawer.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/modal/ModalDrawer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/Plan.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/plan/Plan.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,15 @@
 import {
   EnumPlanState,
   EnumPlanAction,
   useStorePlan,
   EnumPlanApplyType,
 } from '~/context/plan'
 import { Divider } from '~/library/components/divider/Divider'
-import {
-  useApiPlanRun,
-  useApiPlanApply,
-  apiCancelPlanRun,
-  apiCancelPlanApply,
-} from '~/api'
+import { useApiPlanRun, useApiPlanApply, apiCancelPlanApply } from '~/api'
 import {
   type ContextEnvironmentEnd,
   type ContextEnvironmentStart,
 } from '~/api/client'
 import PlanWizard from './PlanWizard'
 import PlanHeader from './PlanHeader'
 import PlanActions from './PlanActions'
@@ -101,16 +96,14 @@
       },
     ])
 
     return () => {
       debouncedPlanRun.cancel()
 
       unsubscribeTests?.()
-
-      apiCancelPlanRun(client)
     }
   }, [])
 
   useEffect(() => {
     dispatch([
       {
         type: EnumPlanActions.External,
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/PlanActions.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/plan/PlanActions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/PlanBackfillDates.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/plan/PlanBackfillDates.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/PlanChangePreview.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/plan/PlanChangePreview.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   headline,
   type,
   className,
 }: PropsPlanChangePreview): JSX.Element {
   return (
     <div
       className={clsx(
-        'flex flex-col rounded-md p-4 overflow-auto',
+        'flex flex-col rounded-md p-4 overflow-auto scrollbar scrollbar--vertical scrollbar--horizontal',
         type === EnumPlanChangeType.Add && 'bg-success-10',
         type === EnumPlanChangeType.Remove && 'bg-danger-10',
         type === EnumPlanChangeType.Direct && 'bg-secondary-10',
         type === EnumPlanChangeType.Indirect && 'bg-warning-10',
         type === 'metadata' && 'bg-neutral-10',
         className,
       )}
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/PlanHeader.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/plan/PlanHeader.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/PlanWizard.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/plan/PlanWizard.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -329,22 +329,30 @@
                             <Suspense
                               fallback={<Spinner className="w-4 h-4 mr-2" />}
                             >
                               <TasksOverview
                                 tasks={tasks}
                                 setRefTasksOverview={setRefTasksOverview}
                               >
-                                {({ total, completed, models }) => (
+                                {({
+                                  total,
+                                  completed,
+                                  models,
+                                  completedBatches,
+                                  totalBatches,
+                                }) => (
                                   <>
                                     <TasksOverview.Summary
                                       environment={environment.name}
                                       planState={planState}
                                       headline="Target Environment"
                                       completed={completed}
                                       total={total}
+                                      completedBatches={completedBatches}
+                                      totalBatches={totalBatches}
                                       updateType={
                                         hasVirtualUpdate
                                           ? 'Virtual'
                                           : 'Backfill'
                                       }
                                       updatedAt={activeBackfill?.updated_at}
                                     />
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/PlanWizardStepOptions.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/plan/PlanWizardStepOptions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/context.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/plan/context.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/help.spec.ts` & `sqlmesh-0.8.0/web/client/src/library/components/plan/help.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/help.ts` & `sqlmesh-0.8.0/web/client/src/library/components/plan/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/plan/hooks.ts` & `sqlmesh-0.8.0/web/client/src/library/components/plan/hooks.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/progress/Progress.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/progress/Progress.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/report/ReportTestsErrors.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/report/ReportTestsErrors.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/root/Footer.tsx` & `sqlmesh-0.8.0/web/client/src/library/pages/root/Footer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/root/Header.tsx` & `sqlmesh-0.8.0/web/client/src/library/pages/root/Header.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/splitPane/SplitPane.css` & `sqlmesh-0.8.0/web/client/src/library/components/splitPane/SplitPane.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/splitPane/SplitPane.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/splitPane/SplitPane.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/tasksOverview/TasksOverview.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/tasksOverview/TasksOverview.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -17,66 +17,83 @@
 interface PropsTasks {
   tasks: PlanTasks
   setRefTasksOverview?: RefObject<HTMLDivElement>
   children: (options: {
     models?: Array<[string, PlanTaskStatus]>
     completed: number
     total: number
+    completedBatches: number
+    totalBatches: number
   }) => JSX.Element
 }
 
 const TasksOverview = function TasksOverview({
   children,
   setRefTasksOverview,
   tasks,
 }: PropsTasks): JSX.Element {
-  const { models, taskCompleted, taskTotal } = useMemo(() => {
-    const models = Object.entries(tasks)
-    const taskCompleted = models.filter(
-      ([_, { completed, total }]) => completed === total,
-    ).length
-    const taskTotal = models.length
+  const { models, taskCompleted, taskTotal, batchesTotal, batchesCompleted } =
+    useMemo(() => {
+      const models = Object.entries(tasks)
+      const taskTotal = models.length
+      let taskCompleted = 0
+      let batchesTotal = 0
+      let batchesCompleted = 0
 
-    return {
-      models,
-      taskCompleted,
-      taskTotal,
-    }
-  }, [tasks])
+      models.forEach(([_, { completed, total }]) => {
+        taskCompleted = completed === total ? taskCompleted + 1 : taskCompleted
+        batchesTotal += total
+        batchesCompleted += completed
+      })
+
+      return {
+        models,
+        taskCompleted,
+        taskTotal,
+        batchesTotal,
+        batchesCompleted,
+      }
+    }, [tasks])
 
   return (
     <div
       className="text-prose"
       ref={setRefTasksOverview}
     >
       {children({
         models,
         completed: taskCompleted,
         total: taskTotal,
+        totalBatches: batchesTotal,
+        completedBatches: batchesCompleted,
       })}
     </div>
   )
 }
 
 function TasksSummary({
   className,
   headline,
   environment,
   planState,
   completed,
   total,
   updatedAt,
   updateType,
+  completedBatches,
+  totalBatches,
 }: {
   className?: string
   headline: string
   environment: EnvironmentName
   planState: PlanState
   completed: number
   total: number
+  completedBatches: number
+  totalBatches: number
   updateType: string
   updatedAt?: string
 }): JSX.Element {
   return (
     <TasksBlock className={className}>
       <Task>
         <TaskDetails>
@@ -90,21 +107,27 @@
           <TaskDetailsProgress>
             <TaskSize
               completed={completed}
               total={total}
               unit="task"
             />
             <TaskDivider />
+            <TaskSize
+              completed={completedBatches}
+              total={totalBatches}
+              unit="batches"
+            />
+            <TaskDivider />
             <TaskProgress
-              completed={completed}
-              total={total}
+              completed={completedBatches}
+              total={totalBatches}
             />
           </TaskDetailsProgress>
         </TaskDetails>
-        <Progress progress={toRatio(completed, total)} />
+        <Progress progress={toRatio(completedBatches, totalBatches)} />
         {updatedAt != null && (
           <TaskCompletedMeta
             updatedAt={updatedAt}
             updateType={updateType}
           />
         )}
       </Task>
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/library/components/toggle/Toggle.tsx` & `sqlmesh-0.8.0/web/client/src/library/components/toggle/Toggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/models/artifact.ts` & `sqlmesh-0.8.0/web/client/src/models/artifact.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/models/directory.ts` & `sqlmesh-0.8.0/web/client/src/models/directory.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/models/environment.ts` & `sqlmesh-0.8.0/web/client/src/models/environment.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/models/file.ts` & `sqlmesh-0.8.0/web/client/src/models/file.ts`

 * *Files 12% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 import { isStringEmptyOrNil } from '@utils/index'
 
 export const EnumFileExtensions = {
   SQL: '.sql',
   Python: '.py',
   CSV: '.csv',
   YAML: '.yaml',
+  YML: '.yml',
 } as const
-
+export type FileExtensions =
+  (typeof EnumFileExtensions)[keyof typeof EnumFileExtensions]
 export interface InitialFile extends InitialArtifact, File {
   content: string
   extension: string
   is_supported: boolean
 }
 
 export class ModelFile extends ModelArtifact<InitialFile> {
   private _content: string = ''
 
   content: string
-  extension: string
+  extension: FileExtensions
   is_supported: boolean
   type?: FileType
 
   constructor(initial?: File | ModelFile, parent?: ModelDirectory) {
     super(
       (initial as ModelFile)?.isModel
         ? (initial as ModelFile).initial
@@ -33,15 +35,16 @@
             extension: initial?.extension ?? EnumFileExtensions.SQL,
             is_supported: initial?.is_supported ?? true,
             content: initial?.content ?? '',
           },
       parent,
     )
 
-    this.extension = initial?.extension ?? this.initial.extension
+    this.extension = (initial?.extension ??
+      this.initial.extension) as FileExtensions
     this.is_supported = initial?.is_supported ?? this.initial.is_supported
     this._content = this.content = initial?.content ?? this.initial.content
     this.type = initial?.type ?? getFileType(initial?.path)
   }
 
   get isEmpty(): boolean {
     return this.content === ''
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/models/initial.ts` & `sqlmesh-0.8.0/web/client/src/models/initial.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/tests/utils.tsx` & `sqlmesh-0.8.0/web/client/src/tests/utils.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/utils/index.spec.ts` & `sqlmesh-0.8.0/web/client/src/utils/index.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/utils/index.ts` & `sqlmesh-0.8.0/web/client/src/utils/index.ts`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,18 @@
   return typeof value === 'string'
 }
 
 export function isStringEmptyOrNil(value: unknown): boolean {
   return isNil(value) || value === ''
 }
 
+export function isStringNotEmpty(value: unknown): boolean {
+  return isString(value) && (value as string).trim() !== ''
+}
+
 export function isArrayNotEmpty(value: unknown): boolean {
   return Array.isArray(value) && value.length > 0
 }
 
 export function isArrayEmpty(value: unknown): boolean {
   return Array.isArray(value) && value.length === 0
 }
```

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/workers/sqlglot/sqlglot.py` & `sqlmesh-0.8.0/web/client/src/workers/sqlglot/sqlglot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/src/workers/sqlglot/worker.ts` & `sqlmesh-0.8.0/web/client/src/workers/sqlglot/worker.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/tailwind.config.js` & `sqlmesh-0.8.0/web/client/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/tsconfig.json` & `sqlmesh-0.8.0/web/client/tsconfig.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/client/vite.config.ts` & `sqlmesh-0.8.0/web/client/vite.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/server/api/endpoints/__init__.py` & `sqlmesh-0.8.0/web/server/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/server/api/endpoints/commands.py` & `sqlmesh-0.8.0/web/server/api/endpoints/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/server/api/endpoints/context.py` & `sqlmesh-0.8.0/web/server/api/endpoints/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/server/api/endpoints/directories.py` & `sqlmesh-0.8.0/web/server/api/endpoints/directories.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/server/api/endpoints/environments.py` & `sqlmesh-0.8.0/web/server/api/endpoints/environments.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/server/api/endpoints/events.py` & `sqlmesh-0.8.0/web/server/api/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/server/api/endpoints/files.py` & `sqlmesh-0.8.0/web/server/api/endpoints/files.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/server/api/endpoints/lineage.py` & `sqlmesh-0.8.0/web/server/api/endpoints/lineage.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/server/api/endpoints/plan.py` & `sqlmesh-0.8.0/web/server/api/endpoints/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/server/console.py` & `sqlmesh-0.8.0/web/server/console.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 import json
+import traceback
 import typing as t
 import unittest
 
 from sqlmesh.core.console import TerminalConsole
 from sqlmesh.core.snapshot import Snapshot
 from sqlmesh.core.test import ModelTest
 from sqlmesh.utils.date import now_timestamp
@@ -96,7 +97,18 @@
             }
             ok = False
         self.queue.put_nowait(self._make_event(data, event="tests", ok=ok))
 
     def log_success(self, msg: str) -> None:
         self.queue.put_nowait(self._make_event(msg))
         self.stop_snapshot_progress()
+
+    def log_exception(self, exc: Exception) -> None:
+        """Log an exception."""
+        self.queue.put_nowait(
+            self._make_event(
+                {"details": str(exc), "traceback": traceback.format_exc()}, event="errors", ok=False
+            )
+        )
+
+
+api_console = ApiConsole()
```

### Comparing `sqlmesh-0.7.1.dev33/web/server/main.py` & `sqlmesh-0.8.0/web/server/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 import pathlib
 
 from fastapi import FastAPI
 from fastapi.responses import HTMLResponse
 from fastapi.staticfiles import StaticFiles
 
 from web.server.api.endpoints import api_router
-from web.server.console import ApiConsole
+from web.server.console import api_console
 from web.server.watcher import watch_project
 
 app = FastAPI()
-api_console = ApiConsole()
 
 app.include_router(api_router, prefix="/api")
 WEB_DIRECTORY = pathlib.Path(__file__).parent.parent
 
 
 @app.on_event("startup")
 async def startup_event() -> None:
```

### Comparing `sqlmesh-0.7.1.dev33/web/server/models.py` & `sqlmesh-0.8.0/web/server/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import enum
 import pathlib
 import typing as t
 
 from pydantic import BaseModel, validator
 
 from sqlmesh.core.context_diff import ContextDiff
+from sqlmesh.core.model.meta import IntervalUnit
 from sqlmesh.core.snapshot.definition import SnapshotChangeCategory
 from sqlmesh.utils.date import TimeLike
 
 SUPPORTED_EXTENSIONS = {".py", ".sql", ".yaml", ".yml", ".csv"}
 
 
 class FileType(str, enum.Enum):
@@ -116,28 +117,28 @@
                         change_category=current.change_category,
                     )
                 )
             elif context_diff.metadata_updated(snapshot_name):
                 metadata.add(snapshot_name)
 
         direct_change_model_names = [change.model_name for change in direct]
+        indirect_change_model_names = [change.model_name for change in indirect]
+
+        for change in indirect:
+            change.direct = [
+                model_name
+                for model_name in change.direct
+                if model_name in direct_change_model_names
+                or model_name in indirect_change_model_names
+            ]
+            change.direct.reverse()
 
         return ModelsDiff(
             direct=direct,
-            indirect=[
-                ChangeIndirect(
-                    model_name=change.model_name,
-                    direct=[
-                        model_name
-                        for model_name in change.direct
-                        if model_name in direct_change_model_names
-                    ],
-                )
-                for change in indirect
-            ],
+            indirect=indirect,
             metadata=metadata,
         )
 
 
 class ContextEnvironmentChanges(BaseModel):
     added: t.Set[str]
     removed: t.Set[str]
@@ -169,21 +170,43 @@
 
 class Column(BaseModel):
     name: str
     type: str
     description: t.Optional[str]
 
 
+class ModelDetails(BaseModel):
+    owner: t.Optional[str] = None
+    kind: t.Optional[str] = None
+    batch_size: t.Optional[int] = None
+    cron: t.Optional[str] = None
+    stamp: t.Optional[str] = None
+    start: t.Optional[str] = None
+    retention: t.Optional[str] = None
+    storage_format: t.Optional[str] = None
+    time_column: t.Optional[str] = None
+    tags: t.Optional[str] = None
+    partitioned_by: t.Optional[str] = None
+    lookback: t.Optional[int] = None
+    cron_prev: t.Optional[TimeLike] = None
+    cron_next: t.Optional[TimeLike] = None
+    interval_unit: t.Optional[IntervalUnit] = None
+    annotated: t.Optional[bool] = None
+    contains_star_query: t.Optional[bool] = None
+    type: t.Optional[str] = None
+
+
 class Model(BaseModel):
     name: str
     path: str
     dialect: str
-    description: t.Optional[str]
-    owner: t.Optional[str]
     columns: t.List[Column]
+    description: t.Optional[str] = None
+    details: t.Optional[ModelDetails] = None
+    sql: t.Optional[str] = None
 
 
 class RenderInput(BaseModel):
     model: str
     start: t.Optional[TimeLike] = None
     end: t.Optional[TimeLike] = None
     latest: t.Optional[TimeLike] = None
```

### Comparing `sqlmesh-0.7.1.dev33/web/server/settings.py` & `sqlmesh-0.8.0/web/server/settings.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/server/sse.py` & `sqlmesh-0.8.0/web/server/sse.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.7.1.dev33/web/server/utils.py` & `sqlmesh-0.8.0/web/server/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 from __future__ import annotations
 
 import asyncio
+import functools
 import io
 import traceback
 import typing as t
 from pathlib import Path, PurePath
 
 import pandas as pd
 import pyarrow as pa  # type: ignore
 from fastapi import Depends, HTTPException
 from starlette.responses import StreamingResponse
 from starlette.status import HTTP_404_NOT_FOUND, HTTP_422_UNPROCESSABLE_ENTITY
 
 from sqlmesh.core.context import Context
+from web.server.console import api_console
 from web.server.settings import get_context
 
 R = t.TypeVar("R")
 
 
 class ArrowStreamingResponse(StreamingResponse):
     def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
         kwargs["media_type"] = "application/vnd.apache.arrow.stream"
         super().__init__(*args, **kwargs)
 
 
 async def run_in_executor(func: t.Callable[..., R], *args: t.Any) -> R:
     """Run in the default loop's executor"""
+
+    @functools.wraps(func)
+    def func_wrapper() -> R:
+        try:
+            return func(*args)
+        except Exception as e:
+            api_console.log_exception(e)
+            raise e
+
     loop = asyncio.get_running_loop()
-    return await loop.run_in_executor(None, func, *args)
+    return await loop.run_in_executor(None, func_wrapper)
 
 
 def validate_path(
     path: str,
     context: Context = Depends(get_context),
 ) -> str:
     resolved_path = context.path.resolve()
```

### Comparing `sqlmesh-0.7.1.dev33/web/server/watcher.py` & `sqlmesh-0.8.0/web/server/watcher.py`

 * *Files identical despite different names*

